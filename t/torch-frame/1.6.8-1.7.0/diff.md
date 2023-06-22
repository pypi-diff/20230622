# Comparing `tmp/torch-frame-1.6.8.tar.gz` & `tmp/torch-frame-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\torch-frame-1.6.8.tar", last modified: Thu Mar 23 15:50:27 2023, max compression
+gzip compressed data, was "dist\torch-frame-1.7.0.tar", last modified: Thu Jun 22 03:43:47 2023, max compression
```

## Comparing `torch-frame-1.6.8.tar` & `torch-frame-1.7.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/
--rw-rw-rw-   0        0        0      516 2023-03-23 15:50:27.000000 torch-frame-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     3955 2022-08-21 10:11:12.000000 torch-frame-1.6.8/README.md
--rw-rw-rw-   0        0        0       42 2023-03-23 15:50:27.000000 torch-frame-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1608 2023-03-23 15:45:41.000000 torch-frame-1.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/torch_frame/
--rw-rw-rw-   0        0        0      343 2022-08-21 10:11:12.000000 torch-frame-1.6.8/torch_frame/__init__.py
--rw-rw-rw-   0        0        0      104 2022-10-29 16:33:51.000000 torch-frame-1.6.8/torch_frame/_get_logger.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/torch_frame/datasets/
--rw-rw-rw-   0        0        0        0 2022-11-12 08:18:56.000000 torch-frame-1.6.8/torch_frame/datasets/__init__.py
--rw-rw-rw-   0        0        0     1632 2022-11-12 08:24:37.000000 torch-frame-1.6.8/torch_frame/datasets/dataset_wrappers.py
--rw-rw-rw-   0        0        0     6280 2022-08-20 06:57:53.000000 torch-frame-1.6.8/torch_frame/ddp_trainer.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/torch_frame/hooks/
--rw-rw-rw-   0        0        0      164 2022-08-21 08:37:48.000000 torch-frame-1.6.8/torch_frame/hooks/__init__.py
--rw-rw-rw-   0        0        0     3547 2022-10-01 08:11:49.000000 torch-frame-1.6.8/torch_frame/hooks/checkpoint_hook.py
--rw-rw-rw-   0        0        0     5506 2022-10-17 14:31:24.000000 torch-frame-1.6.8/torch_frame/hooks/eval_hook.py
--rw-rw-rw-   0        0        0     2897 2022-01-05 16:01:30.000000 torch-frame-1.6.8/torch_frame/hooks/hookbase.py
--rw-rw-rw-   0        0        0     5181 2022-05-29 11:46:20.000000 torch-frame-1.6.8/torch_frame/hooks/logger_hook.py
--rw-rw-rw-   0        0        0     4526 2022-01-04 14:56:31.000000 torch-frame-1.6.8/torch_frame/lr_scheduler.py
--rw-rw-rw-   0        0        0    24493 2022-10-01 07:00:00.000000 torch-frame-1.6.8/torch_frame/trainer.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/torch_frame/utils/
--rw-rw-rw-   0        0        0      197 2022-07-23 16:05:47.000000 torch-frame-1.6.8/torch_frame/utils/__init__.py
--rw-rw-rw-   0        0        0     2877 2021-12-28 15:17:35.000000 torch-frame-1.6.8/torch_frame/utils/config_parser.py
--rw-rw-rw-   0        0        0      474 2022-07-10 14:07:55.000000 torch-frame-1.6.8/torch_frame/utils/dist_utils.py
--rw-rw-rw-   0        0        0     1534 2022-01-09 15:26:45.000000 torch-frame-1.6.8/torch_frame/utils/history_buffer.py
--rw-rw-rw-   0        0        0     4762 2022-08-20 06:57:53.000000 torch-frame-1.6.8/torch_frame/utils/logger.py
--rw-rw-rw-   0        0        0     5926 2022-08-26 15:29:40.000000 torch-frame-1.6.8/torch_frame/utils/metric.py
--rw-rw-rw-   0        0        0     5089 2022-07-10 14:17:20.000000 torch-frame-1.6.8/torch_frame/utils/misc.py
--rw-rw-rw-   0        0        0     1153 2022-07-23 16:09:27.000000 torch-frame-1.6.8/torch_frame/utils/progress_bar.py
--rw-rw-rw-   0        0        0     2422 2022-11-08 15:26:22.000000 torch-frame-1.6.8/torch_frame/utils/test_speed.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/torch_frame/vision/
--rw-rw-rw-   0        0        0       52 2022-03-13 15:20:23.000000 torch-frame-1.6.8/torch_frame/vision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/torch_frame/vision/augmentations/
--rw-rw-rw-   0        0        0       43 2022-02-20 14:36:40.000000 torch-frame-1.6.8/torch_frame/vision/augmentations/__init__.py
--rw-rw-rw-   0        0        0      756 2022-08-20 08:01:58.000000 torch-frame-1.6.8/torch_frame/vision/augmentations/base.py
--rw-rw-rw-   0        0        0    10161 2022-03-15 06:49:07.000000 torch-frame-1.6.8/torch_frame/vision/augmentations/boxes.py
--rw-rw-rw-   0        0        0     2779 2023-03-23 15:45:03.000000 torch-frame-1.6.8/torch_frame/vision/augmentations/colors.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/torch_frame/vision/tools/
--rw-rw-rw-   0        0        0       31 2022-03-13 15:20:39.000000 torch-frame-1.6.8/torch_frame/vision/tools/__init__.py
--rw-rw-rw-   0        0        0    14776 2022-08-26 15:29:40.000000 torch-frame-1.6.8/torch_frame/vision/tools/object_detection.py
-drwxrwxrwx   0        0        0        0 2023-03-23 15:50:27.000000 torch-frame-1.6.8/torch_frame.egg-info/
--rw-rw-rw-   0        0        0      516 2023-03-23 15:50:26.000000 torch-frame-1.6.8/torch_frame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1121 2023-03-23 15:50:26.000000 torch-frame-1.6.8/torch_frame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 15:50:26.000000 torch-frame-1.6.8/torch_frame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-03-23 15:50:26.000000 torch-frame-1.6.8/torch_frame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-23 15:50:26.000000 torch-frame-1.6.8/torch_frame.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/
+-rw-rw-rw-   0        0        0      516 2023-06-22 03:43:47.000000 torch-frame-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4512 2023-06-22 03:40:48.000000 torch-frame-1.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 03:43:47.000000 torch-frame-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2023-06-22 03:40:48.000000 torch-frame-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame/
+-rw-rw-rw-   0        0        0      372 2023-06-22 03:27:40.000000 torch-frame-1.7.0/torch_frame/__init__.py
+-rw-rw-rw-   0        0        0      104 2022-10-29 16:33:51.000000 torch-frame-1.7.0/torch_frame/_get_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame/datasets/
+-rw-rw-rw-   0        0        0       69 2023-06-22 03:27:40.000000 torch-frame-1.7.0/torch_frame/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-06-22 03:27:40.000000 torch-frame-1.7.0/torch_frame/datasets/dataloader_wrappers.py
+-rw-rw-rw-   0        0        0     1690 2023-06-22 03:27:40.000000 torch-frame-1.7.0/torch_frame/datasets/dataset_wrappers.py
+-rw-rw-rw-   0        0        0     6280 2022-08-20 06:57:53.000000 torch-frame-1.7.0/torch_frame/ddp_trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame/hooks/
+-rw-rw-rw-   0        0        0      164 2022-08-21 08:37:48.000000 torch-frame-1.7.0/torch_frame/hooks/__init__.py
+-rw-rw-rw-   0        0        0     3547 2022-10-01 08:11:49.000000 torch-frame-1.7.0/torch_frame/hooks/checkpoint_hook.py
+-rw-rw-rw-   0        0        0     5506 2022-10-17 14:31:24.000000 torch-frame-1.7.0/torch_frame/hooks/eval_hook.py
+-rw-rw-rw-   0        0        0     2897 2022-01-05 16:01:30.000000 torch-frame-1.7.0/torch_frame/hooks/hookbase.py
+-rw-rw-rw-   0        0        0     5181 2022-05-29 11:46:20.000000 torch-frame-1.7.0/torch_frame/hooks/logger_hook.py
+-rw-rw-rw-   0        0        0     4526 2022-01-04 14:56:31.000000 torch-frame-1.7.0/torch_frame/lr_scheduler.py
+-rw-rw-rw-   0        0        0    24441 2023-06-22 03:06:35.000000 torch-frame-1.7.0/torch_frame/trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame/utils/
+-rw-rw-rw-   0        0        0      197 2022-07-23 16:05:47.000000 torch-frame-1.7.0/torch_frame/utils/__init__.py
+-rw-rw-rw-   0        0        0     2877 2021-12-28 15:17:35.000000 torch-frame-1.7.0/torch_frame/utils/config_parser.py
+-rw-rw-rw-   0        0        0      474 2022-07-10 14:07:55.000000 torch-frame-1.7.0/torch_frame/utils/dist_utils.py
+-rw-rw-rw-   0        0        0     1534 2022-01-09 15:26:45.000000 torch-frame-1.7.0/torch_frame/utils/history_buffer.py
+-rw-rw-rw-   0        0        0     4762 2022-08-20 06:57:53.000000 torch-frame-1.7.0/torch_frame/utils/logger.py
+-rw-rw-rw-   0        0        0     5926 2022-08-26 15:29:40.000000 torch-frame-1.7.0/torch_frame/utils/metric.py
+-rw-rw-rw-   0        0        0     5089 2022-07-10 14:17:20.000000 torch-frame-1.7.0/torch_frame/utils/misc.py
+-rw-rw-rw-   0        0        0     1153 2022-07-23 16:09:27.000000 torch-frame-1.7.0/torch_frame/utils/progress_bar.py
+-rw-rw-rw-   0        0        0     2422 2022-11-08 15:26:22.000000 torch-frame-1.7.0/torch_frame/utils/test_speed.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame/vision/
+-rw-rw-rw-   0        0        0       52 2022-03-13 15:20:23.000000 torch-frame-1.7.0/torch_frame/vision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame/vision/augmentations/
+-rw-rw-rw-   0        0        0       43 2022-02-20 14:36:40.000000 torch-frame-1.7.0/torch_frame/vision/augmentations/__init__.py
+-rw-rw-rw-   0        0        0      756 2022-08-20 08:01:58.000000 torch-frame-1.7.0/torch_frame/vision/augmentations/base.py
+-rw-rw-rw-   0        0        0    10161 2022-03-15 06:49:07.000000 torch-frame-1.7.0/torch_frame/vision/augmentations/boxes.py
+-rw-rw-rw-   0        0        0     2779 2023-03-23 15:45:03.000000 torch-frame-1.7.0/torch_frame/vision/augmentations/colors.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame/vision/tools/
+-rw-rw-rw-   0        0        0       31 2022-03-13 15:20:39.000000 torch-frame-1.7.0/torch_frame/vision/tools/__init__.py
+-rw-rw-rw-   0        0        0    14776 2022-08-26 15:29:40.000000 torch-frame-1.7.0/torch_frame/vision/tools/object_detection.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-06-22 03:43:46.000000 torch-frame-1.7.0/torch_frame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-06-22 03:43:47.000000 torch-frame-1.7.0/torch_frame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 03:43:46.000000 torch-frame-1.7.0/torch_frame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-22 03:43:46.000000 torch-frame-1.7.0/torch_frame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 03:43:46.000000 torch-frame-1.7.0/torch_frame.egg-info/top_level.txt
```

### Comparing `torch-frame-1.6.8/PKG-INFO` & `torch-frame-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-frame
-Version: 1.6.8
+Version: 1.7.0
 Summary: 用于深度学习快速实现代码的框架
 Home-page: https://github.com/darknli/Pytorch-Frame/tree/main/torch_frame
 Author: Darkn Lxs
 Author-email: 1187220556@qq.com
 License: UNKNOWN
 Description: 见readme
 Platform: UNKNOWN
```

### Comparing `torch-frame-1.6.8/README.md` & `torch-frame-1.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 # Pytorch Frame
 原代码来自https://github.com/machineko/coreml_torch_utils
 ，此为改版
-# 更新
+# 版本更新
+## v1.6 相关更新
 * v1.6.3 
   * 添加了EvalTotalHook，在所有数据跑完之后才开始计算指标。
   * 添加了metric模块，并增加了目标检测评估指标MAP的metric。
   * 调整了代码层级结构，使其扩展性更强。
 * v1.6.2
   * 完善了training时每个step模型返回的类型，支持：
     * torch.Tensor，返回的是需要backward的tensor，即为total loss
     * dict，返回的是各路loss头，需要注意的是，这种不应加入total loss，因为torch-frame会自动合并其结果给出total loss
     * tuple， 二元组，分别为
       * backward_params：跟梯度回传、模型参数更新有关，可选torch.Tensor或dict，参考前两种
       * metric_params：dict，纯指标参数，不参与梯度回传
+* v1.6.3
+  * 调整代码结构，增强通用性
+  * 加入多卡计算验证集指标的hook
+* v1.6.4
+  * 加入目标检测map的metric和相应的hook
+* v1.6.5
+  * 修复EvalTotalHook bug
+* v1.6.6
+  * 加入gpu型号性能评估的函数gpu_cnn_speed
+* v1.6.7
+  * 优化打印日志体验
+* v1.6.8
+  * 修复个别环境colors模块调用崩溃的问题
+## v1.7 相关更新
+* v1.7.0
+  * 取消iter机制，减少每个epoch开始之前的卡顿
+  * 加入高效获取数据的模块，如InfiniteDataLoader
 
 # 安装
 pip install torch-frame
 
 # 单卡训练
 使用Trainer训练，例如下面伪代码
 ```commandline
```

### Comparing `torch-frame-1.6.8/setup.py` & `torch-frame-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,33 @@
     README = readme.read()
 
 # 允许setup.py在任何路径下执行
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="torch-frame",  # 库名, 需要在pypi中唯一
-    version="1.6.8",  # 版本号
+    version="1.7.0",  # 版本号
     author="Darkn Lxs",  # 作者
-    author_email="1187220556@qq.com", # 作看都将（方便使用索类现问图后成我我们）
+    author_email="1187220556@qq.com",  # 作看都将（方便使用索类现问图后成我我们）
     description="用于深度学习快速实现代码的框架",  # 简介
     long_description="见readme",  # 详细描述（一般会写在README.md中）
     long_description_content_type="text/markdown",  # README.md中描述的语法（一般为markdown)
     url="https://github.com/darknli/Pytorch-Frame/tree/main/torch_frame",  # 库/项目主页，放该项目的远程库地址即可
     packages=setuptools.find_packages(),  # 默认值即可，这个是方便以后我们给库拓展新功能的
     classifiers=[  # 指定该库依赖的Python版本、license、操作系统之类的
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[  # 该库需要的依前库
         "termcolor",
+        "numpy",
         "opencv-python",
         "tabulate",
         "torch",
+        "pyyaml",
+        "tqdm"
     ],
     python_requires='>=3.6',
 )
 
 # python setup.py sdist bdist_wheel
```

### Comparing `torch-frame-1.6.8/torch_frame/datasets/dataset_wrappers.py` & `torch-frame-1.7.0/torch_frame/datasets/dataset_wrappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+import numpy as np
+
+
+__all__ = [
+    "RepeatDataset",
+]
+
+
 # 源自https://github.com/open-mmlab/mmdetection/blob/master/mmdet/datasets/dataset_wrappers.py
 class RepeatDataset:
     """A wrapper of repeated dataset.
 
     The length of repeated dataset will be `times` larger than the original
     dataset. This is useful when the data loading time is long but the dataset
     is small. Using RepeatDataset can reduce the data loading time between
```

### Comparing `torch-frame-1.6.8/torch_frame/ddp_trainer.py` & `torch-frame-1.7.0/torch_frame/ddp_trainer.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/hooks/checkpoint_hook.py` & `torch-frame-1.7.0/torch_frame/hooks/checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/hooks/eval_hook.py` & `torch-frame-1.7.0/torch_frame/hooks/eval_hook.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/hooks/hookbase.py` & `torch-frame-1.7.0/torch_frame/hooks/hookbase.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/hooks/logger_hook.py` & `torch-frame-1.7.0/torch_frame/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/lr_scheduler.py` & `torch-frame-1.7.0/torch_frame/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/trainer.py` & `torch-frame-1.7.0/torch_frame/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
         # counters
         self.inner_iter: int = -1  # [0, epoch_len - 1]
         self.epoch: int = -1  # [0, max_epochs - 1]
         self.start_epoch = 0  # [0, max_epochs - 1]
         self.max_epochs = max_epochs
 
         self._hooks: List[HookBase] = []
-        self._data_iter = iter(data_loader)
         self._clip_grad_norm = clip_grad_norm
         if not torch.cuda.is_available():
             enable_amp = False
             logger.warning("torch环境无法使用cuda, AMP无法使用")
         self._enable_amp = enable_amp
 
         if self._enable_amp:
@@ -270,31 +269,28 @@
         if not np.isfinite(loss_value):
             raise FloatingPointError(
                 f"Loss became infinite or NaN at epoch={self.epoch}! loss_dict = {loss_dict}."
             )
 
         self.log(self.cur_iter, **loss_dict)
 
-    def train_one_iter(self) -> None:
+    def train_one_iter(self, batch) -> None:
         """
         包含了训练的一个iter的全部操作
 
         .. Note::
             标准的学习率调节器是基于epoch的, 但torch_frame框架是基于iter的, 所以它在每次iter之后都会调用
         """
         iter_start_time = time.perf_counter()
         lr_this_iter = self.lr
 
         ######################
         # 1. 加载一个batch的数据 #
         ######################
         # 这里读取生成器的数据而非data_loader这是为了计算加载数据的耗时
-        start = time.perf_counter()
-        batch = next(self._data_iter)
-        data_time = time.perf_counter() - start
 
         #####################
         # 2. 计算loss #
         #####################
         if self._enable_amp:
             with autocast():
                 loss_info = self.model(batch)
@@ -347,28 +343,31 @@
         # 5. 调整学习率 #
         ###########################
         self.lr_scheduler.step()
 
         show_info = {k: v.detach().cpu().item() if isinstance(v, torch.Tensor) else v for k, v in loss_info.items()}
         show_info = dict(sorted(show_info.items(), key=lambda x: x[0] != "total_loss"))  # 保证total_loss在最后一位
         self.pbar.set_postfix(show_info)
-        self._update_iter_metrics(show_info, data_time, time.perf_counter() - iter_start_time, lr_this_iter)
+        self._update_iter_metrics(show_info, self.data_time, time.perf_counter() - iter_start_time, lr_this_iter)
 
     def _train_one_epoch(self) -> None:
         """执行模型一个epoch的全部操作"""
         self.model.train()
         self.pbar = ProgressBar(total=self.epoch_len, desc=f"epoch={self.epoch}", ascii=True)
-        for self.inner_iter in range(self.epoch_len):
+
+        start = time.perf_counter()
+        for self.inner_iter, batch in enumerate(self.data_loader):
+            self.data_time = time.perf_counter() - start
             self._call_hooks("before_iter")
-            self.train_one_iter()
+            self.train_one_iter(batch)
             self._call_hooks("after_iter")
             self.pbar.update(1)
+            start = time.perf_counter()
         self.pbar.close()
         del self.pbar
-        self._data_iter = iter(self.data_loader)
 
     def train(self,
               console_log_level: int = 2,
               file_log_level: int = 2) -> None:
         """
         训练入口
```

### Comparing `torch-frame-1.6.8/torch_frame/utils/config_parser.py` & `torch-frame-1.7.0/torch_frame/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/utils/history_buffer.py` & `torch-frame-1.7.0/torch_frame/utils/history_buffer.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/utils/logger.py` & `torch-frame-1.7.0/torch_frame/utils/logger.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/utils/metric.py` & `torch-frame-1.7.0/torch_frame/utils/metric.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/utils/misc.py` & `torch-frame-1.7.0/torch_frame/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/utils/progress_bar.py` & `torch-frame-1.7.0/torch_frame/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/utils/test_speed.py` & `torch-frame-1.7.0/torch_frame/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/vision/augmentations/base.py` & `torch-frame-1.7.0/torch_frame/vision/augmentations/base.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/vision/augmentations/boxes.py` & `torch-frame-1.7.0/torch_frame/vision/augmentations/boxes.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/vision/augmentations/colors.py` & `torch-frame-1.7.0/torch_frame/vision/augmentations/colors.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame/vision/tools/object_detection.py` & `torch-frame-1.7.0/torch_frame/vision/tools/object_detection.py`

 * *Files identical despite different names*

### Comparing `torch-frame-1.6.8/torch_frame.egg-info/PKG-INFO` & `torch-frame-1.7.0/torch_frame.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-frame
-Version: 1.6.8
+Version: 1.7.0
 Summary: 用于深度学习快速实现代码的框架
 Home-page: https://github.com/darknli/Pytorch-Frame/tree/main/torch_frame
 Author: Darkn Lxs
 Author-email: 1187220556@qq.com
 License: UNKNOWN
 Description: 见readme
 Platform: UNKNOWN
```

### Comparing `torch-frame-1.6.8/torch_frame.egg-info/SOURCES.txt` & `torch-frame-1.7.0/torch_frame.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 torch_frame/trainer.py
 torch_frame.egg-info/PKG-INFO
 torch_frame.egg-info/SOURCES.txt
 torch_frame.egg-info/dependency_links.txt
 torch_frame.egg-info/requires.txt
 torch_frame.egg-info/top_level.txt
 torch_frame/datasets/__init__.py
+torch_frame/datasets/dataloader_wrappers.py
 torch_frame/datasets/dataset_wrappers.py
 torch_frame/hooks/__init__.py
 torch_frame/hooks/checkpoint_hook.py
 torch_frame/hooks/eval_hook.py
 torch_frame/hooks/hookbase.py
 torch_frame/hooks/logger_hook.py
 torch_frame/utils/__init__.py
```

