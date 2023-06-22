# Comparing `tmp/rapid_videocr-2.1.7-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 12203 bytes, number of entries: 9
--rw-r--r--  2.0 unx      133 b- defN 23-May-12 02:06 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx    13354 b- defN 23-May-12 02:06 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     1880 b- defN 23-May-12 02:06 rapid_videocr/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4133 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      766 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/RECORD
-9 files, 31797 bytes uncompressed, 10873 bytes compressed:  65.8%
+Zip file size: 14935 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-22 04:09 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx     4811 b- defN 23-Jun-22 04:09 rapid_videocr/main.py
+-rw-r--r--  2.0 unx    12743 b- defN 23-Jun-22 04:09 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     2756 b- defN 23-Jun-22 04:09 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx     1297 b- defN 23-Jun-22 04:09 rapid_videocr/video_sub_finder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4648 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      934 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/RECORD
+11 files, 38885 bytes uncompressed, 13345 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
 Filename: rapid_videocr/__init__.py
 Comment: 
 
+Filename: rapid_videocr/main.py
+Comment: 
+
 Filename: rapid_videocr/rapid_videocr.py
 Comment: 
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
-Filename: rapid_videocr-2.1.7.dist-info/LICENSE
+Filename: rapid_videocr/video_sub_finder.py
+Comment: 
+
+Filename: rapid_videocr-2.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.1.7.dist-info/METADATA
+Filename: rapid_videocr-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.1.7.dist-info/WHEEL
+Filename: rapid_videocr-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.1.7.dist-info/entry_points.txt
+Filename: rapid_videocr-2.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.1.7.dist-info/top_level.txt
+Filename: rapid_videocr-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.1.7.dist-info/RECORD
+Filename: rapid_videocr-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/__init__.py

```diff
@@ -1,4 +1,5 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
+from .main import RapidVideoSubFinderOCR
 from .rapid_videocr import RapidVideOCR, RapidVideOCRError
```

## rapid_videocr/rapid_videocr.py

```diff
@@ -6,24 +6,28 @@
 from typing import List, Tuple, Union
 
 import cv2
 import numpy as np
 from rapidocr_onnxruntime import RapidOCR
 from tqdm import tqdm
 
-from .utils import CropByProject, mkdir
+from .utils import CropByProject, get_logger, mkdir
 
 CUR_DIR = Path(__file__).resolve().parent
+logger = get_logger()
 
 
-class RapidVideOCR():
-    def __init__(self, is_concat_rec: bool = False,
-                 concat_batch: int = 10,
-                 out_format: str = 'all',
-                 is_print_console: bool = False) -> None:
+class RapidVideOCR:
+    def __init__(
+        self,
+        is_concat_rec: bool = False,
+        concat_batch: int = 10,
+        out_format: str = 'all',
+        is_print_console: bool = False,
+    ) -> None:
         """Init
 
         Args:
             is_concat_rec (bool, optional): Whether to single recognition. Defaults to False.
             concat_batch (int, optional): The batch of concating image nums in concat recognition mode. Defaults to 10.
             out_format (str, optional): Output format of subtitle(srt, txt, all). Defaults to 'all'.
             is_print_console (bool, optional): Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.
@@ -32,18 +36,20 @@
         self.cropper = CropByProject()
 
         self.batch_size = concat_batch
         self.is_concat_rec = is_concat_rec
         self.out_format = out_format
         self.is_print_console = is_print_console
 
-    def __call__(self,
-                 video_sub_finder_dir: Union[str, Path],
-                 save_dir: Union[str, Path],
-                 save_name: str = 'result') -> None:
+    def __call__(
+        self,
+        video_sub_finder_dir: Union[str, Path],
+        save_dir: Union[str, Path],
+        save_name: str = 'result',
+    ) -> None:
         """call
 
         Args:
             video_sub_finder_dir (Union[str, Path]): RGBImages or TXTImages from VideoSubFinder app.
             save_dir (Union[str, Path]): The directory of saving the srt/txt file.
 
         Raises:
@@ -59,21 +65,22 @@
         save_dir = Path(save_dir)
         mkdir(save_dir)
 
         img_list = list(Path(video_sub_finder_dir).glob('*.jpeg'))
         img_list = sorted(img_list, key=self.get_sort_key)
         if not img_list:
             raise RapidVideOCRError(
-                f'{video_sub_finder_dir} has not images with jpeg as suffix.')
+                f'{video_sub_finder_dir} has not images with jpeg as suffix.'
+            )
 
         if self.is_concat_rec:
-            print('Running with concat recognition.')
+            logger.info('[OCR] Running with concat recognition.')
             srt_result, txt_result = self.concat_rec(img_list, is_txt_dir)
         else:
-            print('Running with single recognition.')
+            logger.info('[OCR] Running with single recognition.')
             srt_result, txt_result = self.single_rec(img_list)
 
         self.export_file(save_dir, save_name, srt_result, txt_result)
 
         if self.is_print_console:
             self.print_console(txt_result)
 
@@ -91,43 +98,41 @@
             dt_boxes, rec_res = self.run_ocr(img)
             if rec_res:
                 txts = self.process_same_line(dt_boxes, rec_res)
                 srt_result.append(f'{i+1}\n{time_str}\n{txts}\n')
                 txt_result.append(f'{txts}\n')
         return srt_result, txt_result
 
-    def concat_rec(self, img_list: List[np.ndarray],
-                   is_txt_dir: bool) -> Tuple[List, List]:
+    def concat_rec(
+        self, img_list: List[np.ndarray], is_txt_dir: bool
+    ) -> Tuple[List, List]:
         srt_result, txt_result = [], []
 
         img_nums = len(img_list)
         for start_i in tqdm(range(0, img_nums, self.batch_size), desc='OCR'):
             end_i = min(img_nums, start_i + self.batch_size)
 
-            concat_img, img_coordinates, img_paths = self.get_batch(img_list,
-                                                                    start_i,
-                                                                    end_i,
-                                                                    is_txt_dir)
+            concat_img, img_coordinates, img_paths = self.get_batch(
+                img_list, start_i, end_i, is_txt_dir
+            )
             dt_boxes, rec_res = self.run_ocr(concat_img)
             if not rec_res:
                 continue
 
-            srt_part, txt_part = self.get_match_results(start_i,
-                                                        img_coordinates,
-                                                        dt_boxes,
-                                                        rec_res,
-                                                        img_paths)
+            srt_part, txt_part = self.get_match_results(
+                start_i, img_coordinates, dt_boxes, rec_res, img_paths
+            )
             srt_result.extend(srt_part)
             txt_result.extend(txt_part)
         return srt_result, txt_result
 
-    def get_batch(self, img_list: List[str],
-                  start: int, end: int,
-                  is_txt_dir: bool) -> Tuple[np.ndarray, np.ndarray, List]:
-        select_imgs = img_list[start: end]
+    def get_batch(
+        self, img_list: List[str], start: int, end: int, is_txt_dir: bool
+    ) -> Tuple[np.ndarray, np.ndarray, List]:
+        select_imgs = img_list[start:end]
 
         img_list, img_coordinates, batch_img_paths = [], [], []
         for i, img_path in enumerate(select_imgs):
             batch_img_paths.append(img_path)
 
             img = cv2.imread(str(img_path))
 
@@ -138,19 +143,22 @@
 
             h, w = img.shape[:2]
             img_coordinates.append([(0, i * h), (w, (i + 1) * h)])
 
         concat_img = np.vstack(img_list)
         return concat_img, np.array(img_coordinates), batch_img_paths
 
-    def get_match_results(self, start_i: int,
-                          img_coordinates: np.ndarray,
-                          dt_boxes: np.ndarray,
-                          rec_res: List,
-                          img_paths: list) -> Tuple[List, List]:
+    def get_match_results(
+        self,
+        start_i: int,
+        img_coordinates: np.ndarray,
+        dt_boxes: np.ndarray,
+        rec_res: List,
+        img_paths: list,
+    ) -> Tuple[List, List]:
         srt_result_part, txt_result_part = [], []
 
         match_dict = {}
         y_points = img_coordinates[:, :, 1]
         left_top_boxes = dt_boxes[:, 0, :]
         for i, one_left in enumerate(left_top_boxes):
             y = one_left[1]
@@ -158,17 +166,17 @@
             index = np.argwhere(condition)
             if not index.size:
                 match_dict[i] = ''
                 continue
 
             matched_index = index.squeeze().tolist()
             matched_path = img_paths[matched_index]
-            match_dict.setdefault(matched_index, []).append([matched_path,
-                                                             dt_boxes[i],
-                                                             rec_res[i]])
+            match_dict.setdefault(matched_index, []).append(
+                [matched_path, dt_boxes[i], rec_res[i]]
+            )
 
         for k, v in match_dict.items():
             cur_frame_idx = start_i + k
             img_path, boxes, recs = list(zip(*v))
 
             time_str = self.get_time(img_path[0])
             txts = self.process_same_line(boxes, recs)
@@ -201,33 +209,36 @@
         if ocr_result is None:
             return None, None
 
         dt_boxes, rec_res, _ = list(zip(*ocr_result))
         return np.array(dt_boxes), rec_res
 
     @staticmethod
-    def padding_img(img: np.ndarray,
-                    padding_value: Tuple[int, int, int, int],
-                    padding_color: Tuple = (0, 0, 0)) -> np.ndarray:
-        padded_img = cv2.copyMakeBorder(img,
-                                        padding_value[0],
-                                        padding_value[1],
-                                        padding_value[2],
-                                        padding_value[3],
-                                        cv2.BORDER_CONSTANT,
-                                        value=padding_color)
+    def padding_img(
+        img: np.ndarray,
+        padding_value: Tuple[int, int, int, int],
+        padding_color: Tuple = (0, 0, 0),
+    ) -> np.ndarray:
+        padded_img = cv2.copyMakeBorder(
+            img,
+            padding_value[0],
+            padding_value[1],
+            padding_value[2],
+            padding_value[3],
+            cv2.BORDER_CONSTANT,
+            value=padding_color,
+        )
         return padded_img
 
     def process_same_line(self, dt_boxes, rec_res):
         rec_len = len(rec_res)
         if rec_len == 1:
             return rec_res[0]
 
-        dt_boxes_centroids = [self._compute_centroid(np.array(v))
-                              for v in dt_boxes]
+        dt_boxes_centroids = [self._compute_centroid(np.array(v)) for v in dt_boxes]
         y_centroids = np.array(dt_boxes_centroids)[:, 1].tolist()
         bool_res = self.is_same_line(y_centroids)
 
         pair_points = list(zip(range(rec_len), range(1, rec_len)))
 
         final_res, used = [], [False] * rec_len
         for is_same_line, pair_point in zip(bool_res, pair_points):
@@ -239,16 +250,21 @@
                 final_res.append(' '.join(concat_str))
             else:
                 for v in pair_point:
                     if not used[v]:
                         final_res.append(rec_res[v])
         return '\n'.join(final_res)
 
-    def export_file(self, save_dir: Union[str, Path], save_name: str,
-                    srt_result: List, txt_result: List) -> None:
+    def export_file(
+        self,
+        save_dir: Union[str, Path],
+        save_name: str,
+        srt_result: List,
+        txt_result: List,
+    ) -> None:
         if isinstance(save_dir, str):
             save_dir = Path(save_dir)
 
         srt_path = save_dir / f'{save_name}.srt'
         txt_path = save_dir / f'{save_name}.txt'
 
         if self.out_format == 'txt':
@@ -256,34 +272,32 @@
         elif self.out_format == 'srt':
             self.save_file(srt_path, srt_result)
         elif self.out_format == 'all':
             self.save_file(txt_path, txt_result)
             self.save_file(srt_path, srt_result)
         else:
             raise ValueError(f'The {self.out_format} dost not support.')
-        print(f'The result has been saved to {save_dir} directory.')
+        logger.info(f'[OCR] The result has been saved to {save_dir} directory.')
 
     def print_console(self, txt_result: List) -> None:
         for v in txt_result:
             print(v.strip())
 
     @staticmethod
-    def save_file(save_path: Union[str, Path],
-                  content: list,
-                  mode: str = 'w') -> None:
+    def save_file(save_path: Union[str, Path], content: list, mode: str = 'w') -> None:
         if not isinstance(save_path, str):
             save_path = str(save_path)
 
         if not isinstance(content, list):
             content = [content]
 
         with open(save_path, mode, encoding='utf-8') as f:
             for value in content:
                 f.write(f'{value}\n')
-        print(f'The file has been saved in the {save_path}')
+        logger.info(f'[OCR] The file has been saved in the {save_path}')
 
     @staticmethod
     def _compute_centroid(points: np.ndarray) -> List:
         """计算所给框的质心坐标
 
         :param points ([type]): (4, 2)
         :return: [description]
@@ -307,34 +321,66 @@
 
 class RapidVideOCRError(Exception):
     pass
 
 
 def main() -> None:
     parser = argparse.ArgumentParser()
-    parser.add_argument('-i', '--img_dir', type=str, required=True,
-                        help='The full path of RGBImages or TXTImages.')
-    parser.add_argument('-s', '--save_dir', type=str, default='results',
-                        help='The path of saving the recognition result. Default is "results" under the current directory.')
-    parser.add_argument('-o', '--out_format', type=str, default='all',
-                        choices=['srt', 'txt', 'all'],
-                        help='Output file format. Default is "all".')
-    parser.add_argument('-m', '--mode', type=str, default='single',
-                        choices=['single', 'concat'],
-                        help='Which mode to run (concat recognition or single recognition). Default is "single".')
-    parser.add_argument('-b', '--concat_batch', type=int, default=10,
-                        help='The batch of concating image nums in concat recognition mode. Default is 10.')
-    parser.add_argument('-p', '--print_console', type=bool,
-                        default=0, choices=[0, 1],
-                        help='Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.')
+    parser.add_argument(
+        '-i',
+        '--img_dir',
+        type=str,
+        required=True,
+        help='The full path of RGBImages or TXTImages.',
+    )
+    parser.add_argument(
+        '-s',
+        '--save_dir',
+        type=str,
+        default='outputs',
+        help='The path of saving the recognition result. Default is "outputs" under the current directory.',
+    )
+    parser.add_argument(
+        '-o',
+        '--out_format',
+        type=str,
+        default='all',
+        choices=['srt', 'txt', 'all'],
+        help='Output file format. Default is "all".',
+    )
+    parser.add_argument(
+        '-m',
+        '--mode',
+        type=str,
+        default='single',
+        choices=['single', 'concat'],
+        help='Which mode to run (concat recognition or single recognition). Default is "single".',
+    )
+    parser.add_argument(
+        '-b',
+        '--concat_batch',
+        type=int,
+        default=10,
+        help='The batch of concating image nums in concat recognition mode. Default is 10.',
+    )
+    parser.add_argument(
+        '-p',
+        '--print_console',
+        type=bool,
+        default=0,
+        choices=[0, 1],
+        help='Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.',
+    )
     args = parser.parse_args()
 
     is_concat_rec = 'concat' in args.mode
-    extractor = RapidVideOCR(is_concat_rec=is_concat_rec,
-                             concat_batch=args.concat_batch,
-                             out_format=args.out_format,
-                             is_print_console=args.print_console)
+    extractor = RapidVideOCR(
+        is_concat_rec=is_concat_rec,
+        concat_batch=args.concat_batch,
+        out_format=args.out_format,
+        is_print_console=args.print_console,
+    )
     extractor(args.img_dir, args.save_dir)
 
 
 if __name__ == '__main__':
     main()
```

## rapid_videocr/utils.py

```diff
@@ -1,40 +1,45 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
+import functools
+import logging
+import sys
 from pathlib import Path
 from typing import List
 
+import colorlog
 import cv2
 import numpy as np
 
+logger_initialized = {}
 
-class CropByProject(object):
+
+class CropByProject:
     """投影法裁剪"""
 
     def __init__(self, threshold=250):
         self.threshold = threshold
 
     def __call__(self, origin_img):
         image = cv2.cvtColor(origin_img, cv2.COLOR_BGR2GRAY)
 
         # 将图片二值化
-        retval, img = cv2.threshold(image, self.threshold, 255,
-                                    cv2.THRESH_BINARY_INV)
+        retval, img = cv2.threshold(image, self.threshold, 255, cv2.THRESH_BINARY_INV)
 
         # 使文字增长成块
         closed = cv2.dilate(img, None, iterations=1)
 
         # 水平投影
         x0, x1 = self.get_project_loc(closed, direction='width')
 
         # 竖直投影
         y0, y1 = self.get_project_loc(closed, direction='height')
 
-        return origin_img[y0: y1, x0: x1]
+        return origin_img[y0:y1, x0:x1]
 
     @staticmethod
     def get_project_loc(img, direction):
         """获得裁剪的起始和终点索引位置
         Args:
             img (ndarray): 二值化后得到的图像
             direction (str): 'width/height'
@@ -63,7 +68,36 @@
 def read_txt(txt_path: str) -> List:
     if not isinstance(txt_path, str):
         txt_path = str(txt_path)
 
     with open(txt_path, 'r', encoding='utf-8') as f:
         data = list(map(lambda x: x.rstrip('\n'), f))
     return data
+
+
+@functools.lru_cache()
+def get_logger(name='rapid_videocr'):
+    logger = logging.getLogger(name)
+    if name in logger_initialized:
+        return logger
+
+    for logger_name in logger_initialized:
+        if name.startswith(logger_name):
+            return logger
+
+    fmt_string = '%(log_color)s[%(asctime)s] [%(name)s] %(levelname)s: %(message)s'
+    log_colors = {
+        'DEBUG': 'white',
+        'INFO': 'white',
+        'WARNING': 'yellow',
+        'ERROR': 'red',
+        'CRITICAL': 'purple',
+    }
+    fmt = colorlog.ColoredFormatter(fmt_string, log_colors=log_colors)
+    stream_handler = logging.StreamHandler(stream=sys.stdout)
+    stream_handler.setFormatter(fmt)
+    logger.addHandler(stream_handler)
+
+    logger.setLevel(logging.INFO)
+    logger_initialized[name] = True
+    logger.propagate = False
+    return logger
```

## Comparing `rapid_videocr-2.1.7.dist-info/LICENSE` & `rapid_videocr-2.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapid_videocr-2.1.7.dist-info/METADATA` & `rapid_videocr-2.2.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,108 @@
 Metadata-Version: 2.1
 Name: rapid-videocr
-Version: 2.1.7
+Version: 2.2.0
 Summary: Tool for extracting hard subtitles from videos.
 Home-page: https://github.com/SWHL/RapidVideOCR.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr,videocr,subtitle
 Platform: Any
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<=3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorlog
 Requires-Dist: rapidocr-onnxruntime (>=1.2.2)
-Requires-Dist: tqdm (>=4.52.0)
+Requires-Dist: tqdm
 
 ## rapid_videocr Package
 <p align="left">
-    <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
+    <a href="https://colab.research.google.com/github/SWHL/RapidVideOCR/blob/75dae6e9804dec6e61bef98334601908dc9ec9fb/assets/RapidVideOCRDemo.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg"></a>
+    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
-    <a href="https://pypi.org/project/rapid-videocr/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapid_videocr"></a>
     <a href="https://github.com/SWHL/RapidVideOCR/stargazers"><img src="https://img.shields.io/github/stars/SWHL/RapidVideOCR?color=ccf"></a>
-    <a href="https://pepy.tech/project/rapid-videocr"><img src="https://static.pepy.tech/personalized-badge/rapid-videocr?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
+    <a href="https://pepy.tech/project/rapid-videocr">
+        <img src="https://static.pepy.tech/personalized-badge/rapid-videocr?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads">
+    </a>
+    <a href='https://rapidvideocr.readthedocs.io/en/latest/?badge=latest'>
+        <img src='https://readthedocs.org/projects/rapidvideocr/badge/?version=latest' alt='Documentation Status'/>
+    </a>
     <a href="https://semver.org/"><img alt="SemVer2.0" src="https://img.shields.io/badge/SemVer-2.0-brightgreen"></a>
+    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
+
 ### 1. Install package by pypi.
 ```bash
 pip install rapid_videocr
 ```
 
 ### 2. Run by script.
-- RapidVideOCR API
-    ```python
-    # __init__
-    Args:
-       is_concat_rec (bool, optional): Whether to single recognition. Defaults to False.
-       concat_batch (int, optional): The batch of concating image nums in concat recognition mode. Defaults to 10.
-       out_format (str, optional): Output format of subtitle(srt, txt, all). Defaults to 'all'.
-       is_print_console (bool, optional): Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.
-
-    # __call__
-    Args:
-         video_sub_finder_dir (Union[str, Path]): RGBImages or TXTImages from VideoSubFinder app.
-         save_dir (Union[str, Path]): The directory of saving the srt/txt file.
-
-    Raises:
-        RapidVideOCRError: meet some error.
-    ```
-
-- Example:
+- Only OCR:
     ```python
     from rapid_videocr import RapidVideOCR
 
     extractor = RapidVideOCR(is_concat_rec=True,
-                             concat_batch=10,
-                             out_format='srt')
+                            concat_batch=10,
+                            out_format='srt')
 
     rgb_dir = 'RGBImages'
-    save_dir = 'result'
+    save_dir = 'outputs'
     extractor(video_sub_finder_dir=rgb_dir, save_dir=save_dir)
     ```
+- Extract + OCR:
+    ```python
+    from rapid_videocr import RapidVideoSubFinderOCR
+
+    vsf_exe = r"G:\ProgramFiles\VideoSubFinder_6.10_x64\Release_x64\VideoSubFinderWXW.exe"
+    extractor = RapidVideoSubFinderOCR(vsf_exe_path=vsf_exe, is_concat_rec=True)
+
+    # video_path can be directory path or video full path.
+    video_path = 'test_files/tiny/2.mp4'
+    save_dir = 'outputs'
+    extractor(video_path, save_dir)
+    ```
 
 ### 3. Run by command line.
 - Usage:
     ```bash
     $ rapid_videocr -h
-    usage: rapid_videocr [-h] -i IMG_DIR [-s SAVE_DIR] [-o {srt,txt,all}]
-                        [-m {single,concat}] [-b CONCAT_BATCH] [-p {0,1}]
+    usage: rapid_videocr [-h] [-vsf VSF_EXE_PATH] [-video_dir VIDEO_DIR] [-i IMG_DIR] [-s SAVE_DIR] [-o {srt,txt,all}] [-m {single,concat}] [-b CONCAT_BATCH] [-p {0,1}]
 
-    optional arguments:
+    options:
     -h, --help            show this help message and exit
+    -vsf VSF_EXE_PATH, --vsf_exe_path VSF_EXE_PATH
+                            The full path of VideoSubFinderWXW.exe.
+    -video_dir VIDEO_DIR, --video_dir VIDEO_DIR
+                            The full path of video or the path of video directory.
     -i IMG_DIR, --img_dir IMG_DIR
                             The full path of RGBImages or TXTImages.
     -s SAVE_DIR, --save_dir SAVE_DIR
-                            The path of saving the recognition result. Default is
-                            "results" under the current directory.
+                            The path of saving the recognition result. Default is "outputs" under the current directory.
     -o {srt,txt,all}, --out_format {srt,txt,all}
                             Output file format. Default is "all".
     -m {single,concat}, --mode {single,concat}
-                            Which mode to run (concat recognition or single
-                            recognition). Default is "single".
+                            Which mode to run (concat recognition or single recognition). Default is "single".
     -b CONCAT_BATCH, --concat_batch CONCAT_BATCH
-                            The batch of concating image nums in concat
-                            recognition mode. Default is 10.
+                            The batch of concating image nums in concat recognition mode. Default is 10.
     -p {0,1}, --print_console {0,1}
-                            Whether to print the subtitle results to console. 1
-                            means to print results to console. Default is 0.
+                            Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.
     ```
 - Example:
+  - Only OCR:
+    ```bash
+    $ rapid_videocr -i RGBImages
+    ```
+  - Extract + OCR:
     ```bash
-    $ rapid_videocr -i RGBImages -s Results -o srt -m concat -b 10 -p 1
+    $ rapid_videocr -vsf G:\ProgramFiles\VideoSubFinder_6.10_x64\Release_x64\VideoSubFinderWXW.exe -video_dir G:\ProgramFiles\RapidVideOCR\test_files\tiny
     ```
 
 See details for [RapidVideOCR](https://github.com/SWHL/RapidVideOCR).
```

### html2text {}

```diff
@@ -1,44 +1,48 @@
-Metadata-Version: 2.1 Name: rapid-videocr Version: 2.1.7 Summary: Tool for
+Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.0 Summary: Tool for
 extracting hard subtitles from videos. Home-page: https://github.com/SWHL/
 RapidVideOCR.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: rapidocr,videocr,subtitle Platform: Any Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.7,<=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-rapidocr-onnxruntime (>=1.2.2) Requires-Dist: tqdm (>=4.52.0) ## rapid_videocr
-Package
-[https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
-img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
-img.shields.io/github/stars/SWHL/RapidVideOCR?color=ccf] [https://
-static.pepy.tech/personalized-badge/rapid-
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.6,<3.12 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: colorlog Requires-Dist: rapidocr-onnxruntime (>=1.2.2)
+Requires-Dist: tqdm ## rapid_videocr Package
+[https://colab.research.google.com/assets/colab-badge.svg] [https://
+img.shields.io/badge/Python->=3.6,<3.12-aff.svg] [https://img.shields.io/badge/
+OS-Linux%2C%20Win%2C%20Mac-pink.svg] [https://img.shields.io/github/stars/SWHL/
+RapidVideOCR?color=ccf] [https://static.pepy.tech/personalized-badge/rapid-
 videocr?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
-[SemVer2.0]
+[Documentation_Status] [SemVer2.0] [https://img.shields.io/badge/code%20style-
+black-000000.svg]
 ### 1. Install package by pypi. ```bash pip install rapid_videocr ``` ### 2.
-Run by script. - RapidVideOCR API ```python # __init__ Args: is_concat_rec
-(bool, optional): Whether to single recognition. Defaults to False.
-concat_batch (int, optional): The batch of concating image nums in concat
-recognition mode. Defaults to 10. out_format (str, optional): Output format of
-subtitle(srt, txt, all). Defaults to 'all'. is_print_console (bool, optional):
-Whether to print the subtitle results to console. 1 means to print results to
-console. Default is 0. # __call__ Args: video_sub_finder_dir (Union[str,
-Path]): RGBImages or TXTImages from VideoSubFinder app. save_dir (Union[str,
-Path]): The directory of saving the srt/txt file. Raises: RapidVideOCRError:
-meet some error. ``` - Example: ```python from rapid_videocr import
-RapidVideOCR extractor = RapidVideOCR(is_concat_rec=True, concat_batch=10,
-out_format='srt') rgb_dir = 'RGBImages' save_dir = 'result' extractor
-(video_sub_finder_dir=rgb_dir, save_dir=save_dir) ``` ### 3. Run by command
-line. - Usage: ```bash $ rapid_videocr -h usage: rapid_videocr [-h] -i IMG_DIR
-[-s SAVE_DIR] [-o {srt,txt,all}] [-m {single,concat}] [-b CONCAT_BATCH] [-p
-{0,1}] optional arguments: -h, --help show this help message and exit -
+Run by script. - Only OCR: ```python from rapid_videocr import RapidVideOCR
+extractor = RapidVideOCR(is_concat_rec=True, concat_batch=10, out_format='srt')
+rgb_dir = 'RGBImages' save_dir = 'outputs' extractor
+(video_sub_finder_dir=rgb_dir, save_dir=save_dir) ``` - Extract + OCR:
+```python from rapid_videocr import RapidVideoSubFinderOCR vsf_exe = r"G:
+\ProgramFiles\VideoSubFinder_6.10_x64\Release_x64\VideoSubFinderWXW.exe"
+extractor = RapidVideoSubFinderOCR(vsf_exe_path=vsf_exe, is_concat_rec=True) #
+video_path can be directory path or video full path. video_path = 'test_files/
+tiny/2.mp4' save_dir = 'outputs' extractor(video_path, save_dir) ``` ### 3. Run
+by command line. - Usage: ```bash $ rapid_videocr -h usage: rapid_videocr [-h]
+[-vsf VSF_EXE_PATH] [-video_dir VIDEO_DIR] [-i IMG_DIR] [-s SAVE_DIR] [-o
+{srt,txt,all}] [-m {single,concat}] [-b CONCAT_BATCH] [-p {0,1}] options: -h, -
+-help show this help message and exit -vsf VSF_EXE_PATH, --vsf_exe_path
+VSF_EXE_PATH The full path of VideoSubFinderWXW.exe. -video_dir VIDEO_DIR, --
+video_dir VIDEO_DIR The full path of video or the path of video directory. -
 i IMG_DIR, --img_dir IMG_DIR The full path of RGBImages or TXTImages. -
 s SAVE_DIR, --save_dir SAVE_DIR The path of saving the recognition result.
-Default is "results" under the current directory. -o {srt,txt,all}, --
+Default is "outputs" under the current directory. -o {srt,txt,all}, --
 out_format {srt,txt,all} Output file format. Default is "all". -m
 {single,concat}, --mode {single,concat} Which mode to run (concat recognition
 or single recognition). Default is "single". -b CONCAT_BATCH, --concat_batch
 CONCAT_BATCH The batch of concating image nums in concat recognition mode.
 Default is 10. -p {0,1}, --print_console {0,1} Whether to print the subtitle
 results to console. 1 means to print results to console. Default is 0. ``` -
-Example: ```bash $ rapid_videocr -i RGBImages -s Results -o srt -m concat -b 10
--p 1 ``` See details for [RapidVideOCR](https://github.com/SWHL/RapidVideOCR).
+Example: - Only OCR: ```bash $ rapid_videocr -i RGBImages ``` - Extract + OCR:
+```bash $ rapid_videocr -vsf G:
+\ProgramFiles\VideoSubFinder_6.10_x64\Release_x64\VideoSubFinderWXW.exe -
+video_dir G:\ProgramFiles\RapidVideOCR\test_files\tiny ``` See details for
+[RapidVideOCR](https://github.com/SWHL/RapidVideOCR).
```

## Comparing `rapid_videocr-2.1.7.dist-info/RECORD` & `rapid_videocr-2.2.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-rapid_videocr/__init__.py,sha256=Ai1-HAkB1KvpF-kDWL0-f1bpQ9CRSFTGXmBvnBRmqgE,133
-rapid_videocr/rapid_videocr.py,sha256=uyCdvEBoihw9M2ravpghs9m4AD4lJMeskcWYIT-u6w4,13354
-rapid_videocr/utils.py,sha256=9ccfktiJdGsd2bAjCQ2eMpxZIYy9u9HNcaj7qPwlIUI,1880
-rapid_videocr-2.1.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-rapid_videocr-2.1.7.dist-info/METADATA,sha256=9i5FG_blGo_TWZdOle10hv4cDH2noV4DEKkdwSUHgSQ,4133
-rapid_videocr-2.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-rapid_videocr-2.1.7.dist-info/entry_points.txt,sha256=JnS70pyEdNrH47_TUZkNUleXW8cnAe0pUHrAhJ7Lito,68
-rapid_videocr-2.1.7.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
-rapid_videocr-2.1.7.dist-info/RECORD,,
+rapid_videocr/__init__.py,sha256=eODelyqvjJaceBues-U7fmLAE3JTDkVLUTbcsWivf_Q,174
+rapid_videocr/main.py,sha256=98dis4vitu7QzAXBFxcS4yEu1JNG0eYSsykXU59jpOM,4811
+rapid_videocr/rapid_videocr.py,sha256=0BB0FREm7_PN3r_V52aKzLHA0S7nEuad492NHfijl9o,12743
+rapid_videocr/utils.py,sha256=AWQvgtn8429FnVPYdixHNYEEB4gjJRgKl4aHEcTgzBk,2756
+rapid_videocr/video_sub_finder.py,sha256=HXzgqnH91COSYe1Vfo8frApwcdl9cDQjg6X9TEYJTG8,1297
+rapid_videocr-2.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+rapid_videocr-2.2.0.dist-info/METADATA,sha256=ie5ZInEvtAdqSshy5-j8cyk_lq7Ml3laKOYgKORcXV0,4648
+rapid_videocr-2.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+rapid_videocr-2.2.0.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
+rapid_videocr-2.2.0.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
+rapid_videocr-2.2.0.dist-info/RECORD,,
```

