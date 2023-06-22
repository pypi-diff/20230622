# Comparing `tmp/python-worker-2.1.1.tar.gz` & `tmp/python-worker-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-worker-2.1.1.tar", last modified: Thu Dec 29 01:31:53 2022, max compression
+gzip compressed data, was "python-worker-2.2.0.tar", last modified: Thu Jun 22 08:55:23 2023, max compression
```

## Comparing `python-worker-2.1.1.tar` & `python-worker-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2022-12-29 01:31:53.878491 python-worker-2.1.1/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    10208 2022-12-29 01:31:53.878491 python-worker-2.1.1/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7405 2022-12-28 07:57:30.000000 python-worker-2.1.1/README.md
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2022-12-29 01:31:53.878491 python-worker-2.1.1/python_worker.egg-info/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    10208 2022-12-29 01:31:53.000000 python-worker-2.1.1/python_worker.egg-info/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      256 2022-12-29 01:31:53.000000 python-worker-2.1.1/python_worker.egg-info/SOURCES.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2022-12-29 01:31:53.000000 python-worker-2.1.1/python_worker.egg-info/dependency_links.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        9 2022-12-29 01:31:53.000000 python-worker-2.1.1/python_worker.egg-info/requires.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        7 2022-12-29 01:31:53.000000 python-worker-2.1.1/python_worker.egg-info/top_level.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2022-12-29 01:31:53.878491 python-worker-2.1.1/setup.cfg
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1253 2022-12-29 01:31:42.000000 python-worker-2.1.1/setup.py
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2022-12-29 01:31:53.878491 python-worker-2.1.1/worker/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     4212 2022-12-28 07:25:20.000000 python-worker-2.1.1/worker/__init__.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     3694 2022-12-29 01:31:26.000000 python-worker-2.1.1/worker/process.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    19813 2022-12-27 10:45:46.000000 python-worker-2.1.1/worker/worker.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 08:55:23.050560 python-worker-2.2.0/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     8314 2023-06-22 08:55:23.050560 python-worker-2.2.0/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7882 2023-06-22 08:54:57.000000 python-worker-2.2.0/README.md
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 08:55:23.050560 python-worker-2.2.0/python_worker.egg-info/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     8314 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      256 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/SOURCES.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/dependency_links.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        9 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/requires.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        7 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/top_level.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-06-22 08:55:23.050560 python-worker-2.2.0/setup.cfg
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1253 2023-06-22 08:53:37.000000 python-worker-2.2.0/setup.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 08:55:23.050560 python-worker-2.2.0/worker/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     4424 2023-06-22 08:53:21.000000 python-worker-2.2.0/worker/__init__.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     3509 2023-06-22 08:52:13.000000 python-worker-2.2.0/worker/process.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    19813 2022-12-27 10:45:46.000000 python-worker-2.2.0/worker/worker.py
```

### Comparing `python-worker-2.1.1/PKG-INFO` & `python-worker-2.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,306 +1,307 @@
-Metadata-Version: 2.1
-Name: python-worker
-Version: 2.1.1
-Summary: Simplify and master control (run and stop) the python threads (workers)
-Home-page: https://github.com/Danangjoyoo/python-worker
-Author: danangjoyoo (Agus Danangjoyo)
-Author-email: <agus.danangjoyo.blog@gmail.com>
-License: UNKNOWN
-Description: # python-worker
-        [![Downloads](https://static.pepy.tech/personalized-badge/python-worker?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/python-worker)
-        
-        ---
-        ## Description
-        A package to simplify the thread declaration directly either by using decorator or pass it through function. It also allows you to stop the running thread (worker) from any layer
-        
-        ---
-        
-        ## Installation
-        ```
-        pip install python-worker
-        ```
-        
-        ---
-        
-        ## Changelogs
-        - v1.8:
-          - Refactoring codes
-          - flexible `worker` declaration
-        - v1.9:
-          - Added Asynchronous Worker for coroutine function using `@async_worker` decorator
-        - v1.10:
-          - Added `overload` typehints for `worker` and `async_worker`
-          - Added `restart` feature for worker
-        - v2.0:
-          - Added `process` worker to enable run your function in different GIL (Global Interpreter Lock) which could give you a performance boost
-        
-        
-        ---
-        ## Basic Guide
-        `@worker` will define a function as a thread object once it run
-        
-        ```
-        import time
-        from worker import worker
-        
-        @worker
-        def go(n, sleepDur):
-            for i in range(n):
-              time.sleep(sleepDur)
-            print('done')
-        
-        go(100, 0.1)
-        ```
-        The function `go` will be running as a thread
-        
-        ---
-        
-        ## Asynchronous Guide
-        Well, if you have a coroutine function you can use `async_worker` instead
-        ```
-        import asyncio
-        from worker import async_worker
-        
-        @async_worker
-        async def go():
-            print("this is inside coroutine!")
-            for i in range(10):
-                time.sleep(0.5)
-                print(i)
-            print("done!")
-            return "result!"
-        
-        go_worker = asyncio.run(go())
-        ```
-        
-        ---
-        
-        ## Process Guide
-        A new feature called `process` is simply putting your worker on different GIL (Global Interpreter Lock) which could give you a performance boost.
-        It's implementing `multiprocessing` instead of `multithreading` which at this stage is achieving the true form of `parallelism` which is run in different environment with your function call environment
-        
-        ```
-        import time
-        import os
-        from worker import process
-        
-        @process
-        def go(n, sleepDur):
-            for i in range(n):
-                time.sleep(sleepDur)
-            print('done')
-        
-        go(100, 0.1)
-        ```
-        your function `go` will run in different process.
-        
-        To check it, you can just print out the `os.getpid()`
-        ```
-        import os
-        from worker import worker, process
-        
-        @worker(multiproc=True)
-        def run_in_new_process_from_worker(parent_pid):
-            print(f"from {parent_pid} running in a new process {os.getpid()} - from worker.mutliproc==True")
-            return "return from process"
-        
-        @process
-        def run_in_new_process(parent_pid):
-            print(f"from {parent_pid} running in a new process {os.getpid()} - from process")
-            return "return from process"
-        
-        @worker
-        def run_in_new_thread(parent_pid):
-            print(f"from {parent_pid} running in a new thread {os.getpid()} - from worker.multiproc==False")
-            return "return from thread"
-        
-        
-        print(f"this is on main thread {os.getpid()}")
-        
-        run_in_new_process_from_worker(os.getpid())
-        run_in_new_process(os.getpid())
-        run_in_new_thread(os.getpid())
-        
-        ```
-        
-        then run the script
-        ```
-        this is on main thread 29535
-        from 29535 running in a new process 29537 - from worker.mutliproc==True
-        from 29535 running in a new thread 29535 - from worker.multiproc==False
-        from 29535 running in a new process 29538 - from process
-        ```
-        
-        you can see the different of process id between running in a new process and thread
-        
-        ---
-        
-        # Additional Guides
-        
-        ## Kill / Stop / Abort the running worker
-        You can abort some workers, all workers or even all threads..
-        
-        ### Abort specific workers
-        ```
-        import time
-        from worker import worker, abort_worker
-        
-        @worker
-        def go4(n=10):
-            for i in range(n):
-                time.sleep(1)
-        
-        go4_worker = go4(10)
-        time.sleep(3)
-        abort_worker(go4_worker)
-        ```
-        or just abort it from the instance
-        ```
-        go4_worker.abort()
-        ```
-        
-        ### Abort all workers (this only abort worker threads only)
-        ```
-        from worker import abort_all_worker
-        
-        abort_all_worker()
-        ```
-        
-        ### Abort all threads (it will abort both all worker and non-worker threads)
-        ```
-        from worker import abort_all_thread
-        
-        abort_all_thread()
-        ```
-        ---
-        ## Run undefined `@worker` function
-        ```
-        import time
-        from worker import run_as_Worker
-        
-        def go(n):
-            ...
-        
-        go_worker = run_as_Worker(target=go, args=(10,))
-        ```
-        
-        ---
-        ## Get Return Value
-        How to get the return of threaded function ?
-        ```
-        @worker
-        def go(n):
-            time.sleep(n)
-            return "done"
-        
-        go_worker = go(10)
-        
-        # this will await the worker to finished and return the value
-        
-        go_result = go_worker.await
-        
-        # You can also use this if it's finished, dont have to await
-        
-        go_result = go_worker.ret
-        ```
-        
-        ##  Check/Monitor All Workers
-        ```
-        from worker import ThreadWorkerManager
-        
-        ## all created workers
-        ThreadWorkerManager.list()
-        
-        ## All active/running workers only
-        ThreadWorkerManager.list(active_only=True)
-        ```
-        it will return the information
-        ```
-        >>> ThreadWorkerManager.list()
-        ==============================================================
-        ID   |Name                |Active|Address        | WorkTime (s)
-        ==============================================================
-        0    |worker              |True  |0x7fdf1a977af0 | 4.97
-        1    |worker1             |True  |0x7fdf1a73d640 | 4.07
-        2    |worker2             |True  |0x7fdf1a73d9d0 | 3.83
-        3    |worker3             |True  |0x7fdf1a73dd00 | 3.62
-        4    |worker4             |True  |0x7fdf1a74b070 | 3.38
-        ==============================================================
-        ```
-        
-        ---
-        
-        ## Python Interactive Shell - Keyboard Interrupt (CTRL+C)
-          When you run your scripts on interactive mode
-          ```
-          python -i myScript.py
-          ```
-          you could add an abort handler with keyboard interrupt to abort your thread.
-        
-          #### Inside myScript.py
-        
-          `ThreadWorkerManager.enableKeyboardInterrupt()` allows you to abort your running workers.
-          ```
-          from worker import worker, ThreadWorkerManager
-        
-        
-          # enabling abort handler for worker into keyboard interrupt (CTRL+C)
-        
-          ThreadWorkerManager.enableKeyboardInterrupt()
-          ```
-          You could also activate exit thread which triggered by pressing the CTRL+Z. This also added an abort handler for worker into keyboard interrupt (CTRL+C).
-          ```
-          ThreadWorkerManager.disableKeyboardInterrupt(enable_exit_thread=True)
-          ```
-          Disabling abort handler for worker into keyboard interrupt (CTRL+C).
-          ```
-          ThreadWorkerManager.disableKeyboardInterrupt()
-          ```
-          Check handler status.
-          ```
-          ThreadWorkerManager.keyboard_interrupt_handler_status
-          ```
-        
-          You also can choose which workers are allowed to be aborted on keyboard interrupt
-        
-          #### Inside myScript.py
-        ```
-        from worker import worker, ThreadWorkerManager
-        
-        @worker("Uninterrupted", on_abort=lambda: print("ITS GREAT"), keyboard_interrupt=False)
-        def go_not_interrupted():
-          i = 0
-          while i < 1e3/2:
-            i += 10
-            print(i,"go_not_interrupted")
-            time.sleep(0.001)
-          return i
-        
-        @worker("Interrupted", on_abort=lambda: print("ITS GREAT"), keyboard_interrupt=True)
-        def go_interrupted():
-          i = 0
-          while i < 1e3/2:
-            i += 10
-            print(i,"go_interrupted")
-            time.sleep(0.001)
-          return i
-        
-        ThreadWorkerManagerManager.enableKeyboardInterrupt()
-        go_not_interrupted()
-        go_interrupted()
-        ```
-          run in your terminal
-          ```
-          python -i myScript.py
-          ```
-          press CTRL+C while the process is running and see the results.
-        
-Keywords: python,threading,worker,async worker,async thread,abort thread,thread stopper,thread manager,simple thread,thread monitor
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
+# python-worker
+[![Downloads](https://static.pepy.tech/personalized-badge/python-worker?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/python-worker)
+
+---
+## Description
+A package to simplify the thread declaration directly either by using decorator or pass it through function. It also allows you to stop the running thread (worker) from any layer
+
+---
+
+## Installation
+```
+pip install python-worker
+```
+
+---
+
+## Changelogs
+- v1.8:
+  - Refactoring codes
+  - flexible `worker` declaration
+- v1.9:
+  - Added Asynchronous Worker for coroutine function using `@async_worker` decorator
+- v1.10:
+  - Added `overload` typehints for `worker` and `async_worker`
+  - Added `restart` feature for worker
+- v2.0:
+  - Added `process` worker to enable run your function in different GIL (Global Interpreter Lock) which could give you a performance boost
+- v2.2:
+  - Added `async_process` worker to enable run your async function / coroutine in different GIL (Global Interpreter Lock) which could give you a performance boost
+
+
+---
+## Basic Guide
+`@worker` will define a function as a thread object once it run
+
+```
+import time
+from worker import worker
+
+@worker
+def go(n, sleepDur):
+    for i in range(n):
+      time.sleep(sleepDur)
+    print('done')
+
+go(100, 0.1)
+```
+The function `go` will be running as a thread
+
+---
+
+## Asynchronous Guide
+Well, if you have a coroutine function you can use `async_worker` instead
+```
+import asyncio
+from worker import async_worker
+
+@async_worker
+async def go():
+    print("this is inside coroutine!")
+    for i in range(10):
+        time.sleep(0.5)
+        print(i)
+    print("done!")
+    return "result!"
+
+go_worker = asyncio.run(go())
+```
+
+or run it as a process
+```
+import asyncio
+from worker import async_process
+
+@async_process
+async def go():
+    print("this is inside coroutine!")
+    for i in range(10):
+        time.sleep(0.5)
+        print(i)
+    print("done!")
+    return "result!"
+
+go_worker = asyncio.run(go())
+```
+
+---
+
+## Process Guide
+A new feature called `process` is simply putting your worker on different GIL (Global Interpreter Lock) which could give you a performance boost.
+It's implementing `multiprocessing` instead of `multithreading` which at this stage is achieving the true form of `parallelism` which is run in different environment with your function call environment
+
+```
+import time
+import os
+from worker import process
+
+@process
+def go(n, sleepDur):
+    for i in range(n):
+        time.sleep(sleepDur)
+    print('done')
+
+go(100, 0.1)
+```
+your function `go` will run in different process.
+
+To check it, you can just print out the `os.getpid()`
+```
+import os
+from worker import worker, process
+
+@worker(multiproc=True)
+def run_in_new_process_from_worker(parent_pid):
+    print(f"from {parent_pid} running in a new process {os.getpid()} - from worker.mutliproc==True")
+    return "return from process"
+
+@process
+def run_in_new_process(parent_pid):
+    print(f"from {parent_pid} running in a new process {os.getpid()} - from process")
+    return "return from process"
+
+@worker
+def run_in_new_thread(parent_pid):
+    print(f"from {parent_pid} running in a new thread {os.getpid()} - from worker.multiproc==False")
+    return "return from thread"
+
+
+print(f"this is on main thread {os.getpid()}")
+
+run_in_new_process_from_worker(os.getpid())
+run_in_new_process(os.getpid())
+run_in_new_thread(os.getpid())
+
+```
+
+then run the script
+```
+this is on main thread 29535
+from 29535 running in a new process 29537 - from worker.mutliproc==True
+from 29535 running in a new thread 29535 - from worker.multiproc==False
+from 29535 running in a new process 29538 - from process
+```
+
+you can see the different of process id between running in a new process and thread
+
+---
+
+# Additional Guides
+
+## Kill / Stop / Abort the running worker
+You can abort some workers, all workers or even all threads..
+
+### Abort specific workers
+```
+import time
+from worker import worker, abort_worker
+
+@worker
+def go4(n=10):
+    for i in range(n):
+        time.sleep(1)
+
+go4_worker = go4(10)
+time.sleep(3)
+abort_worker(go4_worker)
+```
+or just abort it from the instance
+```
+go4_worker.abort()
+```
+
+### Abort all workers (this only abort worker threads only)
+```
+from worker import abort_all_worker
+
+abort_all_worker()
+```
+
+### Abort all threads (it will abort both all worker and non-worker threads)
+```
+from worker import abort_all_thread
+
+abort_all_thread()
+```
+---
+## Run undefined `@worker` function
+```
+import time
+from worker import run_as_Worker
+
+def go(n):
+    ...
+
+go_worker = run_as_Worker(target=go, args=(10,))
+```
+
+---
+## Get Return Value
+How to get the return of threaded function ?
+```
+@worker
+def go(n):
+    time.sleep(n)
+    return "done"
+
+go_worker = go(10)
+
+# this will await the worker to finished and return the value
+
+go_result = go_worker.await
+
+# You can also use this if it's finished, dont have to await
+
+go_result = go_worker.ret
+```
+
+##  Check/Monitor All Workers
+```
+from worker import ThreadWorkerManager
+
+## all created workers
+ThreadWorkerManager.list()
+
+## All active/running workers only
+ThreadWorkerManager.list(active_only=True)
+```
+it will return the information
+```
+>>> ThreadWorkerManager.list()
+==============================================================
+ID   |Name                |Active|Address        | WorkTime (s)
+==============================================================
+0    |worker              |True  |0x7fdf1a977af0 | 4.97
+1    |worker1             |True  |0x7fdf1a73d640 | 4.07
+2    |worker2             |True  |0x7fdf1a73d9d0 | 3.83
+3    |worker3             |True  |0x7fdf1a73dd00 | 3.62
+4    |worker4             |True  |0x7fdf1a74b070 | 3.38
+==============================================================
+```
+
+---
+
+## Python Interactive Shell - Keyboard Interrupt (CTRL+C)
+  When you run your scripts on interactive mode
+  ```
+  python -i myScript.py
+  ```
+  you could add an abort handler with keyboard interrupt to abort your thread.
+
+  #### Inside myScript.py
+
+  `ThreadWorkerManager.enableKeyboardInterrupt()` allows you to abort your running workers.
+  ```
+  from worker import worker, ThreadWorkerManager
+
+
+  # enabling abort handler for worker into keyboard interrupt (CTRL+C)
+
+  ThreadWorkerManager.enableKeyboardInterrupt()
+  ```
+  You could also activate exit thread which triggered by pressing the CTRL+Z. This also added an abort handler for worker into keyboard interrupt (CTRL+C).
+  ```
+  ThreadWorkerManager.disableKeyboardInterrupt(enable_exit_thread=True)
+  ```
+  Disabling abort handler for worker into keyboard interrupt (CTRL+C).
+  ```
+  ThreadWorkerManager.disableKeyboardInterrupt()
+  ```
+  Check handler status.
+  ```
+  ThreadWorkerManager.keyboard_interrupt_handler_status
+  ```
+
+  You also can choose which workers are allowed to be aborted on keyboard interrupt
+
+  #### Inside myScript.py
+```
+from worker import worker, ThreadWorkerManager
+
+@worker("Uninterrupted", on_abort=lambda: print("ITS GREAT"), keyboard_interrupt=False)
+def go_not_interrupted():
+  i = 0
+  while i < 1e3/2:
+    i += 10
+    print(i,"go_not_interrupted")
+    time.sleep(0.001)
+  return i
+
+@worker("Interrupted", on_abort=lambda: print("ITS GREAT"), keyboard_interrupt=True)
+def go_interrupted():
+  i = 0
+  while i < 1e3/2:
+    i += 10
+    print(i,"go_interrupted")
+    time.sleep(0.001)
+  return i
+
+ThreadWorkerManagerManager.enableKeyboardInterrupt()
+go_not_interrupted()
+go_interrupted()
+```
+  run in your terminal
+  ```
+  python -i myScript.py
+  ```
+  press CTRL+C while the process is running and see the results.
```

### Comparing `python-worker-2.1.1/setup.py` & `python-worker-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '2.1.1'
+VERSION = '2.2.0'
 DESCRIPTION = 'Simplify and master control (run and stop) the python threads (workers)'
 
 # Setting up
 setup(
     name="python-worker",
     version=VERSION,
     author="danangjoyoo (Agus Danangjoyo)",
```

### Comparing `python-worker-2.1.1/worker/__init__.py` & `python-worker-2.2.0/worker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,8 +121,15 @@
 
 from .process import *
 
 def process(function: FunctionType):
     """
     Create a process worker. This function will run your function in a separate GIL
     """
-    return ProcessConnector.create_process(function)
+    return ProcessConnector.create_process(function)
+
+
+async def async_process(function: FunctionType):
+    """
+    Create an async process worker. This function will run your function in a separate GIL
+    """
+    return ProcessConnector.create_process(function)
```

### Comparing `python-worker-2.1.1/worker/process.py` & `python-worker-2.2.0/worker/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import inspect
 import json
 import logging
-from multiprocessing import Process, Pipe, get_context
+from multiprocessing import Process, Pipe
 from multiprocessing.connection import Connection
-from typing import Optional
 from types import FunctionType
 
 
 logger = logging.getLogger()
 
 
 class ProcessConnector:
@@ -59,49 +58,45 @@
         except Exception as error:
             logger.debug(error)
             raise error
         finally:
             conn.close()
 
     def create_and_run(self, *args, **kwargs):
-        ctx = get_context("fork")
-        self.parent_con, self.child_con = ctx.Pipe()
+        self.parent_con, self.child_con = Pipe()
         if self.is_async:
-            self.proc = ctx.Process(
+            self.proc = Process(
                 target=lambda: (
                     asyncio.run(
                         self.execute_in_process_event_loop(
                             self.child_con
                         )
                     )
                 )
             )
         else:
-            self.proc = ctx.Process(
+            self.proc = Process(
                 target=lambda: (
                     self.execute_in_process(
                         self.child_con
                     )
                 )
             )
         self.proc.start()
         self.parent_con.send({"args": args, "kwargs": kwargs})
         return self.parent_con
 
-    def __execute(self):
-        self.execute_in_process(self.child_con)
-
     @property
     def ret(self):
         if self.parent_con and not self.parent_con.closed and self.child_con.closed:
             self.result = self.parent_con.recv()
             self.parent_con.close()
         return self.result
 
-    def wait(self, timeout: Optional[float] = None):
+    def wait(self, timeout):
         self.proc.join(timeout)
 
     def receive(self):
         return self.parent_con.recv()
 
     @staticmethod
     def create_process(function: FunctionType):
```

### Comparing `python-worker-2.1.1/worker/worker.py` & `python-worker-2.2.0/worker/worker.py`

 * *Files identical despite different names*

