# Comparing `tmp/qps_limit-0.1.4-py3-none-any.whl.zip` & `tmp/qps_limit-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 4628 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       77 b- defN 23-Jun-21 09:44 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     8900 b- defN 23-Jun-21 09:43 qps_limit/wrapper.py
--rw-rw-r--  2.0 unx     2518 b- defN 23-Jun-21 09:44 qps_limit-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-21 09:44 qps_limit-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-21 09:44 qps_limit-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-21 09:44 qps_limit-0.1.4.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      547 b- defN 23-Jun-21 09:44 qps_limit-0.1.4.dist-info/RECORD
-7 files, 12145 bytes uncompressed, 3652 bytes compressed:  69.9%
+-rw-rw-r--  2.0 unx       77 b- defN 23-Jun-22 08:53 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     9553 b- defN 23-Jun-22 08:54 qps_limit/wrapper.py
+-rw-rw-r--  2.0 unx     2514 b- defN 23-Jun-22 08:54 qps_limit-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 08:54 qps_limit-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-22 08:54 qps_limit-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-22 08:54 qps_limit-0.1.5.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      547 b- defN 23-Jun-22 08:54 qps_limit-0.1.5.dist-info/RECORD
+7 files, 12794 bytes uncompressed, 3652 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: qps_limit/__init__.py
 Comment: 
 
 Filename: qps_limit/wrapper.py
 Comment: 
 
-Filename: qps_limit-0.1.4.dist-info/METADATA
+Filename: qps_limit-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-0.1.4.dist-info/WHEEL
+Filename: qps_limit-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-0.1.4.dist-info/top_level.txt
+Filename: qps_limit-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-0.1.4.dist-info/zip-safe
+Filename: qps_limit-0.1.5.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-0.1.4.dist-info/RECORD
+Filename: qps_limit-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 from .wrapper import MWrapper
 
 __all__ = ['MWrapper']
```

## qps_limit/wrapper.py

```diff
@@ -16,20 +16,21 @@
         time_period = time_period / max_rate
         max_rate = 1
     return AsyncLimiter(max_rate=max_rate, time_period=time_period)
 
 
 async def async_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
+    idxs: Iterable[int],
     params: Iterable[Tuple[Tuple, Dict]],
     max_qps: Optional[float],
     *,
-    max_workers=128,
+    max_workers: int = 128,
     callback: Callable = None,
-    progress=False
+    progress_queue: multiprocessing.Queue = None
 ):
     if max_qps is not None:
         limiter = get_limiter(max_qps)
 
         async def limited_func(*args, **kwargs):
             async with limiter:
                 return await func(*args, **kwargs)
@@ -42,53 +43,52 @@
         else:
             return await limited_func(*args, **kwargs)
 
     result = []
     queue = asyncio.Queue()
     jobs_cnt = 0
 
-    for idx, param in enumerate(params):
+    for idx, param in zip(idxs, params):
         await queue.put((idx, param))
         jobs_cnt += 1
 
-    if progress:
-        progress_bar = tqdm(total=jobs_cnt, desc=func.__name__, unit='req')
-
     async def worker():
         while not queue.empty():
             _idx, _param = await queue.get()
             result.append((_idx, await callback_func(*_param[0], **_param[1])))
-            if progress:
-                progress_bar.update(1)
+            if progress_queue:
+                progress_queue.put_nowait(1)
 
     await asyncio.gather(*[worker() for _ in range(max_workers)])
-    result.sort(key=lambda x: x[0])
-    return [r for _, r in result]
+    assert len(result) == jobs_cnt
+    return result
 
 
 def batch_run(
-    func,
+    func: Callable[..., Coroutine[Any, Any, Any]],
+    idxs: Iterable[int],
     params: Iterable[Tuple[Tuple, Dict]],
     max_qps: Optional[float],
     *,
-    max_workers=128,
+    max_workers: int = 128,
     callback: Callable = None,
-    progress=False
+    progress_queue: multiprocessing.Queue = None
 ):
     return asyncio.get_event_loop().run_until_complete(async_batch_run(**locals()))
 
 
 async def async_streaming_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
+    idxs: Iterable[int],
     params: Iterable[Tuple[Tuple, Dict]],
     max_qps: Optional[float],
     *,
-    max_workers=128,
+    max_workers: int = 128,
     callback: Callable = None,
-    progress=False
+    progress_queue: multiprocessing.Queue = None
 ):
     if max_qps is not None:
         limiter = get_limiter(max_qps)
 
         async def limited_func(*args, **kwargs):
             async with limiter:
                 return await func(*args, **kwargs)
@@ -101,49 +101,43 @@
         else:
             return await limited_func(*args, **kwargs)
 
     queue = asyncio.Queue()
     result = asyncio.Queue()
     jobs_cnt = 0
 
-    for param in params:
-        await queue.put(param)
+    for idx, param in zip(idxs, params):
+        await queue.put((idx, param))
         jobs_cnt += 1
 
-    if progress:
-        pbar = tqdm(total=jobs_cnt, desc=func.__name__, unit='req')
-
-    lock = asyncio.Lock()
-
     async def worker():
         while not queue.empty():
-            async with lock:
-                _param = await queue.get()
-                _res = await callback_func(*_param[0], **_param[1])
-                await result.put(_res)
-            if progress:
-                pbar.update(1)
+            _idx, _param = await queue.get()
+            _res = await callback_func(*_param[0], **_param[1])
+            await result.put((_idx, _res))
+            if progress_queue:
+                progress_queue.put_nowait(1)
 
     asyncio.gather(*[worker() for _ in range(max_workers)])
     jobs_consume = 0
     while jobs_consume < jobs_cnt:
-        res = await result.get()
-        yield res
+        yield await result.get()
         jobs_consume += 1
     assert jobs_consume == jobs_cnt
 
 
 def streaming_batch_run(
-    func,
+    func: Callable[..., Coroutine[Any, Any, Any]],
+    idxs: Iterable[int],
     params: Iterable[Tuple[Tuple, Dict]],
     max_qps: Optional[float],
     *,
-    max_workers=128,
+    max_workers: int = 128,
     callback: Callable = None,
-    progress=False
+    progress_queue: multiprocessing.Queue = None
 ):
     async_generator = async_streaming_batch_run(**locals())
 
     def iter_over_async(ait, loop):
         ait = ait.__aiter__()
 
         async def get_next():
@@ -194,81 +188,88 @@
         self.count_iterator, self.param_iterator = itertools.tee(self.params(), 2)
         self.count = 0
         for _ in self.count_iterator:
             self.count += 1
 
         self.param_iterator, warmup_param_iterator = itertools.tee(self.param_iterator)
         warmup_cnt = 1
+        warmup_idx_iterator = (i for i in range(warmup_cnt))
         warmup_param_iterator = itertools.islice(warmup_param_iterator, warmup_cnt)
         warmup_start_time = time.time()
         if self.verbose:
             print("warm up workers with {} data".format(warmup_cnt))
         batch_run(
             func=self.func,
+            idxs=warmup_idx_iterator,
             params=warmup_param_iterator,
             max_qps=None,
-            max_workers=1,
-            progress=False
+            max_workers=1
         )
         warmup_end_time = time.time()
         avg_worker_time = (warmup_end_time - warmup_start_time) / warmup_cnt
         if self.worker_max_qps is None:
             self.max_workers = 128
         else:
             self.max_workers = min(128, self.worker_max_qps * math.ceil(avg_worker_time))
         if self.verbose:
             print("avg worker time: {:.2f}s -> set worker num: {}".format(avg_worker_time, self.max_workers))
 
+        if self.progress:
+            self.progress_queue = multiprocessing.Queue()
+            def _progress_worker():
+                progress_bar = tqdm(total=self.count, desc=self.func.__name__)
+                progress_cnt = 0
+                while progress_cnt < self.count:
+                    progress_bar.update(self.progress_queue.get())
+                    progress_cnt += 1
+                progress_bar.close()
+            self.workers.append(multiprocessing.Process(target=_progress_worker, args=()))
+        else:
+            self.progress_queue = None
+
         for mod in range(self.num_workers):
-            self.workers.append(
-                multiprocessing.Process(
-                    target=self._worker,
-                    args=(
-                        mod,
-                    )
-                )
-            )
+            self.workers.append(multiprocessing.Process(target=self._worker, args=(mod,)))
 
     def _worker(self, mod):
         def make_iterators():
             def iterator():
                 for idx, (args, kwargs) in enumerate(self.param_iterator):
                     if idx % self.num_workers == mod:
                         yield idx, (args, kwargs)
             a_iter, b_iter = itertools.tee(iterator(), 2)
             return (a for a, _ in a_iter), (b for _, b in b_iter)
 
         idx_iterator, param_iterator = make_iterators()
 
         if not self.streaming:
-            idxs = [idx for idx in idx_iterator]
             results = batch_run(
                 func=self.func,
+                idxs=idx_iterator,
                 params=param_iterator,
                 max_qps=self.worker_max_qps,
                 max_workers=self.max_workers,
                 callback=self.callback,
-                progress=self.progress
+                progress_queue=self.progress_queue
             )
-            assert len(idxs) == len(results)
-            for idx, res in zip(idxs, results):
+            for idx, res in results:
                 if self.ordered:
                     self.dict[idx] = res
                 else:
                     self.queue.put((idx, res))
         else:
             result_iterator = streaming_batch_run(
                 func=self.func,
+                idxs=idx_iterator,
                 params=param_iterator,
                 max_qps=self.worker_max_qps,
                 max_workers=self.max_workers,
                 callback=self.callback,
-                progress=self.progress
+                progress_queue=self.progress_queue
             )
-            for idx, res in zip(idx_iterator, result_iterator):
+            for idx, res in result_iterator:
                 if self.ordered:
                     self.dict[idx] = res
                 else:
                     self.queue.put((idx, res))
 
     def __call__(self):
         start_time = time.time()
@@ -281,14 +282,16 @@
                     pass
                 yield (consume, self.dict[consume])
                 del self.dict[consume]
             else:
                 yield self.queue.get()
             consume += 1
         assert consume == self.count
+        for worker in self.workers:
+            worker.join()
         end_time = time.time()
         if self.verbose:
             print('elapsed time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
                 end_time - start_time,
                 self.count / (end_time - start_time),
                 self.worker_max_qps * self.num_workers if self.worker_max_qps else float("inf"))
             )
```

## Comparing `qps_limit-0.1.4.dist-info/METADATA` & `qps_limit-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 0.1.4
+Version: 0.1.5
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/rate-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -56,24 +56,24 @@
 
 BTW: The wrapped function returns a structure `(idx, res)` consisting of an index of the data and the function return value. If `ordered=False` is set, the order of the returned values may be randomized for better performance.
 
 ### Example
 
 > 10 workers, each with a maximum qps of 10, to calculate the function value of `(1+1/n)^n`
 
-> Assuming that `func` is a time-consuming function, it takes 0.5 seconds to execute
+> Assuming that `func` is a time-consuming function, it takes 1.0 seconds to execute
 
 ```python
 import asyncio
 
 from qps_limit import MWrapper
 
 
 async def func(n: int):
-    await asyncio.sleep(0.5)
+    await asyncio.sleep(1.0)
     return 1 + 1 / n, n
 
 
 def params():
     for n in range(1, 1001):
         yield (), {"n": n}
 
@@ -83,17 +83,17 @@
 
 
 f = MWrapper(
     func=func,
     params=params,
     num_workers=10,
     worker_max_qps=10,
-    streaming=False,
+    streaming=True,
     callback=callback,
     progress=True,
     ordered=True,
     verbose=False
 )
 
 for idx, r in f():
-    print(idx, r)
+	print(idx, r)
 ```
```

