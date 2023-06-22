# Comparing `tmp/array_record-0.3.0-py39-none-any.whl.zip` & `tmp/array_record-0.4.0-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3014474 bytes, number of entries: 12
+Zip file size: 3014524 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-23 21:02 array_record/__init__.py
--rw-r--r--  2.0 unx      803 b- defN 23-Jun-21 11:29 array_record/setup.py
+-rw-r--r--  2.0 unx      803 b- defN 23-Jun-22 07:39 array_record/setup.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-23 21:02 array_record/python/__init__.py
--rw-r--r--  2.0 unx    13798 b- defN 23-Jun-21 11:31 array_record/python/array_record_data_source.py
--rw-r--r--  2.0 unx    10335 b- defN 23-Jun-21 11:31 array_record/python/array_record_data_source_test.py
--rwxr-xr-x  2.0 unx  8887664 b- defN 23-Jun-21 11:37 array_record/python/array_record_module.so
--rw-r--r--  2.0 unx     4631 b- defN 23-Jun-21 11:31 array_record/python/array_record_module_test.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-21 11:37 array_record-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      502 b- defN 23-Jun-21 11:37 array_record-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-21 11:37 array_record-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-21 11:37 array_record-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1072 b- defN 23-Jun-21 11:37 array_record-0.3.0.dist-info/RECORD
-12 files, 8930268 bytes uncompressed, 3012644 bytes compressed:  66.3%
+-rw-r--r--  2.0 unx    14006 b- defN 23-Jun-22 07:40 array_record/python/array_record_data_source.py
+-rw-r--r--  2.0 unx    10340 b- defN 23-Jun-22 07:40 array_record/python/array_record_data_source_test.py
+-rwxr-xr-x  2.0 unx  8887664 b- defN 23-Jun-22 07:46 array_record/python/array_record_module.so
+-rw-r--r--  2.0 unx     4631 b- defN 23-Jun-22 07:40 array_record/python/array_record_module_test.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-22 07:46 array_record-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      502 b- defN 23-Jun-22 07:46 array_record-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-22 07:46 array_record-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-22 07:46 array_record-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1072 b- defN 23-Jun-22 07:46 array_record-0.4.0.dist-info/RECORD
+12 files, 8930481 bytes uncompressed, 3012694 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: array_record/python/array_record_module.so
 Comment: 
 
 Filename: array_record/python/array_record_module_test.py
 Comment: 
 
-Filename: array_record-0.3.0.dist-info/LICENSE
+Filename: array_record-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: array_record-0.3.0.dist-info/METADATA
+Filename: array_record-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: array_record-0.3.0.dist-info/WHEEL
+Filename: array_record-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: array_record-0.3.0.dist-info/top_level.txt
+Filename: array_record-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: array_record-0.3.0.dist-info/RECORD
+Filename: array_record-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## array_record/setup.py

```diff
@@ -6,15 +6,15 @@
 REQUIRED_PACKAGES = [
     'absl-py',
     'etils[epath]',
 ]
 
 setup(
     name='array_record',
-    version='0.3.0',
+    version='0.4.0',
     description='A file format that achieves a new frontier of IO efficiency',
     author='ArrayRecord team',
     author_email='no-reply@google.com',
     packages=find_packages(),
     include_package_data=True,
     package_data={'': ['*.so']},
     python_requires='>=3.8',
```

## array_record/python/array_record_data_source.py

```diff
@@ -36,15 +36,15 @@
 import dataclasses
 import hashlib
 import itertools
 import os
 import pathlib
 import re
 import typing
-from typing import Any, Callable, List, Mapping, overload, Protocol, Sequence, Tuple, TypeVar, Union
+from typing import Any, Callable, List, Mapping, Protocol, Sequence, Tuple, TypeVar, Union
 
 from absl import flags
 from absl import logging
 from etils import epath
 
 from array_record.python.array_record_module import ArrayRecordReader
 
@@ -309,26 +309,28 @@
         filename,
         options="readahead_buffer_size:0",
         file_reader_buffer_size=32768,
     )
     _check_group_size(filename, reader)
     self._readers[reader_idx] = reader
 
-  @overload
-  def __getitem__(self, record_key: Sequence[int]) -> Sequence[bytes]:
-    ...
-
   def __getitem__(self, record_key: int) -> bytes:
-    if isinstance(record_key, int):
-      reader_idx, position = self._reader_idx_and_position(record_key)
-      self._ensure_reader_exists(reader_idx)
-      return self._readers[reader_idx].read([position])[0]
-
-    record_keys: Sequence[int] = record_key
+    if not isinstance(record_key, int):
+      logging.error(
+          "Calling ArrayRecordDataSource.__getitem__() with sequence "
+          "of record keys (%s) is deprecated. Either pass a single "
+          "integer or switch to __getitems__().",
+          record_key,
+      )
+      return self.__getitems__(record_key)
+    reader_idx, position = self._reader_idx_and_position(record_key)
+    self._ensure_reader_exists(reader_idx)
+    return self._readers[reader_idx].read([position])[0]
 
+  def __getitems__(self, record_keys: Sequence[int]) -> Sequence[bytes]:
     def read_records(
         reader_idx: int, reader_positions_and_indices: Sequence[Tuple[int, int]]
     ) -> Sequence[Tuple[Any, int]]:
       """Reads records using the given reader keeping track of the indices."""
       # Initialize readers lazily when we need to read from them.
       self._ensure_reader_exists(reader_idx)
       positions, indices = list(zip(*reader_positions_and_indices))
```

## array_record/python/array_record_data_source_test.py

```diff
@@ -93,50 +93,50 @@
   def test_array_record_data_source_single_path(self):
     indices_to_read = [0, 1, 2, 3, 4]
     expected_data = [b"0", b"1", b"2", b"3", b"4"]
     # Use a single path instead of a list of paths/file_instructions.
     with array_record_data_source.ArrayRecordDataSource(
         self.testdata_dir / "digits.array_record-00000-of-00002"
     ) as ar:
-      actual_data = ar[indices_to_read]
+      actual_data = [ar[x] for x in indices_to_read]
     self.assertEqual(expected_data, actual_data)
     self.assertTrue(all(reader is None for reader in ar._readers))
 
   def test_array_record_data_source_reverse_order(self):
     indices_to_read = [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
     expected_data = [b"9", b"8", b"7", b"6", b"5", b"4", b"3", b"2", b"1", b"0"]
     with array_record_data_source.ArrayRecordDataSource([
         self.testdata_dir / "digits.array_record-00000-of-00002",
         self.testdata_dir / "digits.array_record-00001-of-00002",
     ]) as ar:
-      actual_data = ar[indices_to_read]
+      actual_data = [ar[x] for x in indices_to_read]
     self.assertEqual(expected_data, actual_data)
     self.assertTrue(all(reader is None for reader in ar._readers))
 
   def test_array_record_data_source_random_order(self):
     # some random permutation
     indices_to_read = [3, 0, 5, 9, 2, 1, 4, 7, 8, 6]
     expected_data = [b"3", b"0", b"5", b"9", b"2", b"1", b"4", b"7", b"8", b"6"]
     with array_record_data_source.ArrayRecordDataSource([
         self.testdata_dir / "digits.array_record-00000-of-00002",
         self.testdata_dir / "digits.array_record-00001-of-00002",
     ]) as ar:
-      actual_data = ar[indices_to_read]
+      actual_data = [ar[x] for x in indices_to_read]
     self.assertEqual(expected_data, actual_data)
     self.assertTrue(all(reader is None for reader in ar._readers))
 
-  def test_array_record_data_source_single_element_lookup(self):
+  def test_array_record_data_source_batched_element_lookup(self):
     # some random permutation
     indices_to_read = [3, 0, 5, 9, 2, 1, 4, 7, 8, 6]
     expected_data = [b"3", b"0", b"5", b"9", b"2", b"1", b"4", b"7", b"8", b"6"]
     with array_record_data_source.ArrayRecordDataSource([
         self.testdata_dir / "digits.array_record-00000-of-00002",
         self.testdata_dir / "digits.array_record-00001-of-00002",
     ]) as ar:
-      actual_data = [ar[index] for index in indices_to_read]  # pytype: disable=unsupported-operands
+      actual_data = ar.__getitems__(indices_to_read)
     self.assertEqual(expected_data, actual_data)
     self.assertTrue(all(reader is None for reader in ar._readers))
 
   def test_array_record_data_source_file_instructions(self):
     file_instruction_one = DummyFileInstruction(
         filename=os.fspath(
             self.testdata_dir / "digits.array_record-00000-of-00002"
@@ -158,15 +158,15 @@
     indices_to_read = [0, 1, 2]
     expected_data = [b"2", b"7", b"8"]
 
     with array_record_data_source.ArrayRecordDataSource(
         [file_instruction_one, file_instruction_two]
     ) as ar:
       self.assertLen(ar, 3)
-      actual_data = ar[indices_to_read]
+      actual_data = [ar[x] for x in indices_to_read]
 
     self.assertEqual(expected_data, actual_data)
     self.assertTrue(all(reader is None for reader in ar._readers))
 
   def test_array_record_source_reader_idx_and_position(self):
     file_instructions = [
         # 2 records
```

## Comparing `array_record-0.3.0.dist-info/LICENSE` & `array_record-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `array_record-0.3.0.dist-info/RECORD` & `array_record-0.4.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 array_record/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-array_record/setup.py,sha256=-1_SQLzkeaFZw6vAhIsYyrqNg45nVfqH4OLd-XOdjuc,803
+array_record/setup.py,sha256=FkbMKuUA1ZMnrh02f7gHgX70TIO31zYqb1QRdDpSGxc,803
 array_record/python/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-array_record/python/array_record_data_source.py,sha256=AQCNGFnZsRykS64Cn89BGKoKuqWaQh_ml-ek0wipCss,13798
-array_record/python/array_record_data_source_test.py,sha256=pR9ETK-lBfr-5gTFsT7Kl9bzGNbdBa6eIB5YNdLIca8,10335
+array_record/python/array_record_data_source.py,sha256=xFBBt433RedsG2tBn24cV4TZTHAmo9OoxH4a6fzu2Tw,14006
+array_record/python/array_record_data_source_test.py,sha256=s4sAQpEfYo9cjVib0hvS51ggdKYdnePrXYARXoaUsEA,10340
 array_record/python/array_record_module.so,sha256=6XPkCOxBrd-ohA_rGnMkHPN5SlOA1WHjuPOQ7R9pDtI,8887664
 array_record/python/array_record_module_test.py,sha256=BWvuCt_UL5ZLmeaq6cEH7DiX4IQ_JqLdV5-1czmuaQ4,4631
-array_record-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-array_record-0.3.0.dist-info/METADATA,sha256=5GeWJEPLMSclINsJ5rGke7XvgH_U-94VrMJ6ODE4NJA,502
-array_record-0.3.0.dist-info/WHEEL,sha256=ijjRDmPkGsL9eKpOeSzmTjLbiyw0Dy8TY4QGa2Zy9J8,93
-array_record-0.3.0.dist-info/top_level.txt,sha256=tXm19-b93OrmJ3F0IKm4705VPls3c0UiF6i-r5qnn88,13
-array_record-0.3.0.dist-info/RECORD,,
+array_record-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+array_record-0.4.0.dist-info/METADATA,sha256=84debIsUo8uu7WhxQqKvKsW90Qib3hd1C0YAAIHQoMA,502
+array_record-0.4.0.dist-info/WHEEL,sha256=ijjRDmPkGsL9eKpOeSzmTjLbiyw0Dy8TY4QGa2Zy9J8,93
+array_record-0.4.0.dist-info/top_level.txt,sha256=tXm19-b93OrmJ3F0IKm4705VPls3c0UiF6i-r5qnn88,13
+array_record-0.4.0.dist-info/RECORD,,
```

