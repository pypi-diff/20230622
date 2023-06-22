# Comparing `tmp/imagetocsv-0.2.1-py2.py3-none-any.whl.zip` & `tmp/imagetocsv-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 11924 bytes, number of entries: 15
--rw-r--r--  2.0 unx      191 b- defN 22-Nov-09 21:48 imagetocsv/__init__.py
--rw-r--r--  2.0 unx     2282 b- defN 22-Nov-10 00:58 imagetocsv/cli.py
--rw-r--r--  2.0 unx      614 b- defN 22-Nov-09 23:26 imagetocsv/hardcoded_options.py
--rw-r--r--  2.0 unx     7282 b- defN 22-Nov-14 00:02 imagetocsv/imagetocsv.py
--rw-r--r--  2.0 unx     1646 b- defN 22-Nov-09 23:58 imagetocsv/pathing.py
+Zip file size: 12591 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-22 13:25 imagetocsv/__init__.py
+-rw-r--r--  2.0 unx     2880 b- defN 23-Jun-22 13:27 imagetocsv/cli.py
+-rw-r--r--  2.0 unx      617 b- defN 23-Jun-22 13:25 imagetocsv/hardcoded_options.py
+-rw-r--r--  2.0 unx     7449 b- defN 23-Jun-22 13:35 imagetocsv/imagetocsv.py
+-rw-r--r--  2.0 unx     1708 b- defN 23-Jun-22 13:25 imagetocsv/pathing.py
 -rw-r--r--  2.0 unx      541 b- defN 22-Nov-14 00:02 imagetocsv/string_modifiers.py
--rw-r--r--  2.0 unx     1028 b- defN 22-Nov-14 00:02 imagetocsv/tempfile.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-22 13:25 imagetocsv/tempfile.py
 -rw-r--r--  2.0 unx      181 b- defN 22-Nov-09 23:51 imagetocsv/examples/__init__.py
--rw-r--r--  2.0 unx      159 b- defN 22-Nov-14 16:15 imagetocsv-0.2.1.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx     1070 b- defN 22-Nov-14 16:15 imagetocsv-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     9708 b- defN 22-Nov-14 16:15 imagetocsv-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Nov-14 16:15 imagetocsv-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 22-Nov-14 16:15 imagetocsv-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 22-Nov-14 16:15 imagetocsv-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1244 b- defN 22-Nov-14 16:15 imagetocsv-0.2.1.dist-info/RECORD
-15 files, 26118 bytes uncompressed, 9856 bytes compressed:  62.3%
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jun-22 13:36 imagetocsv-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17036 b- defN 23-Jun-22 13:36 imagetocsv-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 13:36 imagetocsv-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-22 13:36 imagetocsv-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-22 13:36 imagetocsv-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1150 b- defN 23-Jun-22 13:36 imagetocsv-1.0.0.dist-info/RECORD
+14 files, 34045 bytes uncompressed, 10675 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -18,29 +18,26 @@
 
 Filename: imagetocsv/tempfile.py
 Comment: 
 
 Filename: imagetocsv/examples/__init__.py
 Comment: 
 
-Filename: imagetocsv-0.2.1.dist-info/AUTHORS.rst
+Filename: imagetocsv-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: imagetocsv-0.2.1.dist-info/LICENSE
+Filename: imagetocsv-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: imagetocsv-0.2.1.dist-info/METADATA
+Filename: imagetocsv-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: imagetocsv-0.2.1.dist-info/WHEEL
+Filename: imagetocsv-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: imagetocsv-0.2.1.dist-info/entry_points.txt
+Filename: imagetocsv-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: imagetocsv-0.2.1.dist-info/top_level.txt
-Comment: 
-
-Filename: imagetocsv-0.2.1.dist-info/RECORD
+Filename: imagetocsv-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imagetocsv/__init__.py

```diff
@@ -1,7 +1,7 @@
 """Top-level package for ImageToCSV."""
 from .imagetocsv import imagetocsv
 
 __author__ = """Troy Sincomb"""
 __email__ = "troysincomb@gmail.com"
-__version__ = "0.1.0"
+__version__ = "1.0.0"
 __all__ = ["imagetocsv"]
```

## imagetocsv/cli.py

```diff
@@ -9,20 +9,20 @@
 from imagetocsv import imagetocsv
 
 from .hardcoded_options import options
 
 
 @click.command()
 @click.version_option()
-@click.option(
-    "--verbose",
-    "-v",
-    is_flag=True,
-    help="Vebosity level, ex. -vvvvv for debug level logging",
-)
+# @click.option(
+#     "--verbose",
+#     "-v",
+#     is_flag=True,
+#     help="Vebosity level, ex. -vvvvv for debug level logging",
+# )
 @click.option(
     "--index_name",
     "-n",
     type=click.STRING,
     default=None,
     help="Index Name for the CSV file",
 )
@@ -30,22 +30,22 @@
     "--index",
     "-i",
     type=click.STRING,
     default=None,
     help="Index for the CSV file",
 )
 @click.option(
-    "--column_header",
+    "--columns",
     "-c",
     type=click.STRING,
     default=None,
     help="Columns for the CSV file",
 )
 @click.option(
-    "--preconfigured-options",
+    "--preconfigured-option",
     "-p",
     type=click.STRING,
     default=None,
     help="Preconfigured Index/Header Options",
 )
 @click.argument(
     "image_path",
@@ -66,38 +66,62 @@
         file_okay=True,
         dir_okay=False,
         readable=True,
         resolve_path=True,
     ),
 )
 def main(
-    verbose: bool,
     index_name: str,
-    index: str,
-    column_header: str,
-    preconfigured_options: str,
+    index: list[str],
+    columns: list[str],
+    preconfigured_option: str,
     image_path: str,
     csv_path: str,
-):
-    """Console script for imagetocsv."""
-    if preconfigured_options:
+) -> None:
+    """Console script for imagetocsv.
+
+    Parameters
+    ----------
+    verbose : bool
+        Vebosity level, ex. -vvvvv for debug level logging
+    index_name : str
+        Index Name for the CSV file
+    index : list[str]
+        Index for the CSV file
+    columns : list[str]
+        Columns for the CSV file
+    preconfigured_option : str
+        Preconfigured Index/Header Options
+    image_path : str
+        Path for input image
+    csv_path : str
+        Path for output CSV file
+
+    Raises
+    ------
+    KeyError
+        Preconfigured Option not found
+    FileNotFoundError
+        Input Image not found
+    """
+    if preconfigured_option:
         try:
-            index_name, index, column_header = options[preconfigured_options]
+            index_name, index, columns = options[preconfigured_option]
         except KeyError:
             raise KeyError(
-                f"preconfigured_options {preconfigured_options} not found, following options are available: {options}"
+                f"preconfigured_option {preconfigured_option} not found, following options are available: {options.keys()}"
             )
 
     if Path(image_path).exists() is False:
         raise FileNotFoundError(f"File {image_path} does not exist")
 
-    df = imagetocsv(image_path, index_name, index, column_header)
+    df = imagetocsv(image_path, index_name, index, columns)
+    show_index = True if index else False
 
     if csv_path and Path(csv_path).name != "-":
-        df.to_csv(csv_path, index=index, header=column_header)
+        df.to_csv(path_or_buf=csv_path, index=show_index, header=columns)
     else:
-        print(df.to_csv(index=index, header=column_header))
+        print(df.to_csv(index=show_index, header=columns), file=sys.stdout)
 
 
 if __name__ == "__main__":
-    # print("Running imagetocsv.cli.main()")
     sys.exit(main())  # pragma: no cover
```

## imagetocsv/hardcoded_options.py

```diff
@@ -1,9 +1,9 @@
 options = {
-    "bib": (
+    "chrous": (
         "Population",
         [
             "All Events",
             "Lymphocytes",
             "Single cells...",
             "Single cells...",
             "Live/Dead",
```

## imagetocsv/imagetocsv.py

```diff
@@ -10,17 +10,14 @@
 import numpy.typing as npt
 import pandas as pd
 import pdftotext
 
 from imagetocsv.string_modifiers import fix_common_mistakes
 from imagetocsv.tempfile import NamedTemporaryFile
 
-# import pytesseract
-
-
 
 def pdftocsv(file: str) -> list[list[str]]:
     """Convert a pdf file to a list of lists of strings. We do this to keep layout information.
 
     Parameters
     ----------
     file : str
@@ -33,15 +30,17 @@
     """
     tmpchar = "*"
     special_chars = "%"
     all_positions: set[int] = set()
 
     # Find start positions of all columns
     with open(file, "rb") as f:
-        pdf = pdftotext.PDF(f, physical=True)[0]
+        pdf: str = pdftotext.PDF(f, physical=True)[0]
+        if not isinstance(pdf, str):
+            raise TypeError("PDF format not supported. Could not convert to string.")
         for line in pdf.split("\n"):
             for special_char in special_chars.split():
                 line = line.replace(f" {special_char}", f"{special_char} ")
                 line = line.replace(f"  {special_char}", f"{special_char}  ")
             line = f" {line.strip()} "
             for word in line.split():
                 if not word:
@@ -82,50 +81,52 @@
                 cell = fix_common_mistakes(cell)
                 row.append(cell)
             rows.append(row)
 
     return rows
 
 
-def add_df_indexes_headers(df: pd.DataFrame, index_name: str, index: str, column_header: str) -> pd.DataFrame:
+def add_df_indexes_headers(
+    df: pd.DataFrame, index_name: str | None, index: list[str] | None, columns: list[str] | None
+) -> pd.DataFrame:
     """Add indexes and headers to a dataframe.
 
     Parameters
     ----------
     df : pd.DataFrame
         The dataframe to add indexes and headers to.
     index_name : str, optional
         Name of the index, by default None
-    index : list[str] | str, optional
+    index : list[str] | str, optionals
         Index values, by default None
-    column_header : list[str] | str, optional
+    columns : list[str] | str, optional
         Column header values, by default None
 
     Returns
     -------
     pd.DataFrame
         The dataframe with indexes and headers.
     """
-    if column_header:
-        df.columns = column_header.split(",") if isinstance(column_header, str) else column_header
+    if columns:
+        df.columns = columns.split(",") if isinstance(columns, str) else columns
     if index:
-        df.index = index.split(",") if isinstance(index, str) else index
+        df.index = pd.Index(index.split(",") if isinstance(index, str) else index)
     if index_name:
-        df.index.name = index_name
+        df.index.name = index_name  # type: ignore
 
     return df
 
 
 def unsharp_mask(
     image: npt.NDArray[np.uint8],
     kernel_size: tuple[int, int] = (5, 5),
     sigma: float = 1.0,
     amount: float = 1.0,
     threshold: float = 0,
-):
+) -> npt.NDArray[np.uint8]:
     """Return a sharpened version of the image, using an unsharp mask.
 
     Parameters
     ----------
     image : np.ndarray
         image - The image to be sharpened.
     kernel_size : tuple[int, int], optional
@@ -152,40 +153,40 @@
         np.copyto(sharpened, image, where=low_contrast_mask)
     return sharpened
 
 
 def imagetocsv(
     file: str,
     index_name: str | None = None,
-    index: list[str] | str | None = None,
-    column_header: list[str] | str | None = None,
+    index: list[str] | None = None,
+    columns: list[str] | None = None,
 ) -> pd.DataFrame:
     """Convert an image file to a pandas DataFrame.
 
     Parameters
     ----------
     file : str
         Path to the image file.
     index_name : str, optional
         Name of the index, by default None
     index : list[str] | str, optional
         Index values, by default None
-    column_header : list[str] | str, optional
+    columns : list[str] | str, optional
         Column header values, by default None
 
     Returns
     -------
     pd.DataFrame
     """
     file = str(file)
 
     img = cv2.imread(file)
     h, w, _ = img.shape
     img = cv2.resize(img, (w * 3, h * 3))
-    img = unsharp_mask(img)
+    img = unsharp_mask(img)  # type: ignore
     grayImage = cv2.cvtColor(img, cv2.COLOR_RGB2GRAY)
     (_thresh, blackAndWhiteImage) = cv2.threshold(grayImage, 180, 255, cv2.THRESH_BINARY)
 
     # TODO: see if we can use pytesseract to get the table for windows in version 0.3.0
     # custom_oem_psm_config = r"""
     #     --oem 3
     #     --psm 6
@@ -194,15 +195,15 @@
     #     -c preserve_interword_spaces=1
     #     -c tessedit_create_pdf=1
     # """
     # pdf: bytes = pytesseract.image_to_pdf_or_hocr(
     #     "blackAndWhiteImage.png", lang="eng", extension="pdf", config=custom_oem_psm_config
     # )
 
-    tmp = NamedTemporaryFile(delete=False, mode=None)
+    tmp = NamedTemporaryFile(delete=False, mode=None)  # type: ignore
     prefix: str = tmp.name
     # Tesseract cannot handle stdin so we need to write the image to a file first
     cv2.imwrite(prefix + ".png", blackAndWhiteImage)
     _ = subprocess.run(
         [
             "tesseract",
             "--oem",
@@ -225,11 +226,11 @@
     )
     # pdftotext for layout analysis
     rows = pdftocsv(prefix + ".pdf")
     # remove the temporary files in garbage collection for windows to handle it
     del tmp
     gc.collect()
 
-    df = pd.DataFrame(rows)
-    df = add_df_indexes_headers(df, index_name, index, column_header)
+    df = pd.DataFrame(data=rows)
+    df = add_df_indexes_headers(df, index_name, index, columns)
 
     return df
```

## imagetocsv/pathing.py

```diff
@@ -1,31 +1,32 @@
 """
 Home for string tools and any other misc tool until its large enough for it's own file
 """
 from __future__ import annotations
 
 import os
 from pathlib import Path
+from typing import Any
 
 
 class cd:
     """Context manager for changing the current working directory"""
 
-    def __init__(self, newPath):
+    def __init__(self, newPath: Path | str):
         self.newPath = os.path.expanduser(newPath)
 
     def __enter__(self):
         self.savedPath = os.getcwd()
         os.chdir(self.newPath)
 
-    def __exit__(self, etype, value, traceback):
+    def __exit__(self, etype: Any, value: Any, traceback: Any):
         os.chdir(self.savedPath)
 
 
-def pathing(path: str, new: bool = False, overwrite: bool = True) -> Path:
+def pathing(path: Path | str, new: bool = False, overwrite: bool = True) -> Path:
     """Guarantees correct expansion rules for pathing.
     :param Union[str, Path] path: path of folder or file you wish to expand.
     :param bool new: will check if distination exists if new  (will check parent path regardless).
     :return: A pathlib.Path object.
     >>> pathing('~/Desktop/folderofgoodstuffs/')
     /home/user/Desktop/folderofgoodstuffs
     """
@@ -43,8 +44,8 @@
         if not path.parent.exists():
             raise ValueError(f"ERROR ::: Parent directory of {path} does not exist.")
         if path.exists() and not overwrite:
             raise ValueError(f"ERROR ::: {path} already exists!")
     else:
         if not path.exists():
             raise ValueError(f"ERROR ::: Path {path} does not exist.")
-    return
+    return path
```

## imagetocsv/tempfile.py

```diff
@@ -1,41 +1,43 @@
+from __future__ import annotations
+
 import os
 import tempfile
+from pathlib import Path
+from typing import Any
 
 
 class TemporaryFile:
-    def __init__(self, name, io, delete):
+    def __init__(self, name: str, io: Any, delete: bool):
         self.name = name
         self.__io = io
         self.__delete = delete
 
-    def __getattr__(self, k):
+    def __getattr__(self, k: Any) -> Any:
         return getattr(self.__io, k)
 
-    def __del__(self):
+    def __del__(self) -> None:
         if self.__delete:
             try:
                 os.unlink(self.name)
             except FileNotFoundError:
                 pass
 
 
-def NamedTemporaryFile(mode="w+b", bufsize=-1, suffix="", prefix="tmp", dir=None, delete=True):
+def NamedTemporaryFile(
+    mode: str | None = "w+b",
+    bufsize: int = -1,
+    suffix: str = "",
+    prefix: str = "tmp",
+    dir: Path | str | None = None,
+    delete: bool = True,
+) -> TemporaryFile:
     if not dir:
         dir = tempfile.gettempdir()
     name = os.path.join(dir, prefix + os.urandom(32).hex() + suffix)
     if mode is None:
         return TemporaryFile(name, None, delete)
     fh = open(name, "w+b", bufsize)
     if mode != "w+b":
         fh.close()
         fh = open(name, mode)
     return TemporaryFile(name, fh, delete)
-
-
-def test_ntf_del():
-    x = NamedTemporaryFile(suffix="s", prefix="p")
-    assert os.path.exists(x.name)
-    name = x.name
-    del x
-    gc.collect()
-    assert not os.path.exists(name)
```

## Comparing `imagetocsv-0.2.1.dist-info/LICENSE` & `imagetocsv-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `imagetocsv-0.2.1.dist-info/RECORD` & `imagetocsv-1.0.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-imagetocsv/__init__.py,sha256=4Oil-dpN_k5UrS--kaUB_g1uwfxcJp8NZEnKeVFe-bs,191
-imagetocsv/cli.py,sha256=nYnWpvicutgvZSZwuDhZwIa5atJcjL3aDKx9SazWQfo,2282
-imagetocsv/hardcoded_options.py,sha256=ccBtJ02sp8apfWa03E9Iw4cYVpma63jGp8uTI32dwtY,614
-imagetocsv/imagetocsv.py,sha256=tYb7g0uOVBTaetdi28gviIhGD1AUIKdZE0Yk9Z0OklM,7282
-imagetocsv/pathing.py,sha256=ULXvc-Rir_SVDlKu6kv2rdmN5QReTD5FVXAE0eXlWAY,1646
+imagetocsv/__init__.py,sha256=o89SFgmAE7ClhmTsXZTGG3Oz1VcOzFWB-6DkJIs5bZg,191
+imagetocsv/cli.py,sha256=8ya-lI34DaZRJS8m6V2IcINaHvRhlcJe4N9bcSnDoiY,2880
+imagetocsv/hardcoded_options.py,sha256=6J_zmmGTF4LPD6C_y5KCYGLEH1l8ToXBfSuhfCPLdvc,617
+imagetocsv/imagetocsv.py,sha256=wYHs_OQIADtySN4SQ6vBoWMI7opMZbFFoRdZrgtQ48M,7449
+imagetocsv/pathing.py,sha256=Bb5WNuQxS71F_kmMGDfEsSNon-rqvL5cObwODACw5io,1708
 imagetocsv/string_modifiers.py,sha256=xP5wIpkqMd7aDrTtQFsb_iOtVxuucDMkEHVyWxbtJkg,541
-imagetocsv/tempfile.py,sha256=cUIrK8r1GyQUY7InoQUKV0RdD62JIGrJYuueGsFMXfs,1028
+imagetocsv/tempfile.py,sha256=7q0xcpZmkafJTDJjLVzzC8T-p5eH1YiODoxqFLDpWzg,1068
 imagetocsv/examples/__init__.py,sha256=jkHYr5-VmLea6kiGbzM2nAcixHnsXjvcPK7Qx6NYiDg,181
-imagetocsv-0.2.1.dist-info/AUTHORS.rst,sha256=kmHnvbf2DR9MjRWdzGjpAByoqyo1825sjm0F68l82rE,159
-imagetocsv-0.2.1.dist-info/LICENSE,sha256=sq9kmm59tMlJ1a696kN40Hi_k3tEzygxmQEYh8KUhEg,1070
-imagetocsv-0.2.1.dist-info/METADATA,sha256=QKrNmMHJUUHn1PFAzXOmSqgSj8gWubKBam9awynzoSc,9708
-imagetocsv-0.2.1.dist-info/WHEEL,sha256=Ow1Agppnny4NfvfZK4t6N-TUVQfFCpnFCb5wBX-uuec,110
-imagetocsv-0.2.1.dist-info/entry_points.txt,sha256=tamgdFip_JqBzZa3Ej4iBfu6rMRk2RzR49DSEi_MQFI,51
-imagetocsv-0.2.1.dist-info/top_level.txt,sha256=M_z9Aml_943J79N7ofAQJ4KsihSREvhV0AMsWjqYCLI,11
-imagetocsv-0.2.1.dist-info/RECORD,,
+imagetocsv-1.0.0.dist-info/LICENSE,sha256=sq9kmm59tMlJ1a696kN40Hi_k3tEzygxmQEYh8KUhEg,1070
+imagetocsv-1.0.0.dist-info/METADATA,sha256=uNiPOCdOc6L-lYdJea8mPHUeZ0Rb0UlQ-1gD0zf2pew,17036
+imagetocsv-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+imagetocsv-1.0.0.dist-info/entry_points.txt,sha256=tamgdFip_JqBzZa3Ej4iBfu6rMRk2RzR49DSEi_MQFI,51
+imagetocsv-1.0.0.dist-info/top_level.txt,sha256=M_z9Aml_943J79N7ofAQJ4KsihSREvhV0AMsWjqYCLI,11
+imagetocsv-1.0.0.dist-info/RECORD,,
```

