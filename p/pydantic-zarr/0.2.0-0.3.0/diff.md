# Comparing `tmp/pydantic_zarr-0.2.0.tar.gz` & `tmp/pydantic_zarr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_zarr-0.2.0.tar", max compression
+gzip compressed data, was "pydantic_zarr-0.3.0.tar", max compression
```

## Comparing `pydantic_zarr-0.2.0.tar` & `pydantic_zarr-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.2.0/LICENSE
--rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.2.0/README.md
--rw-r--r--   0        0        0      489 2023-06-06 19:15:25.723765 pydantic_zarr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       85 2023-06-03 15:04:37.431488 pydantic_zarr-0.2.0/src/pydantic_zarr/__init__.py
--rw-r--r--   0        0        0    10522 2023-06-06 19:14:28.300772 pydantic_zarr-0.2.0/src/pydantic_zarr/core.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3746 2023-06-22 03:12:34.236303 pydantic_zarr-0.3.0/README.md
+-rw-r--r--   0        0        0      489 2023-06-22 03:14:29.111501 pydantic_zarr-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-06-03 15:04:37.431488 pydantic_zarr-0.3.0/src/pydantic_zarr/__init__.py
+-rw-r--r--   0        0        0    11216 2023-06-22 03:14:05.695358 pydantic_zarr-0.3.0/src/pydantic_zarr/core.py
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pydantic_zarr-0.3.0/PKG-INFO
```

### Comparing `pydantic_zarr-0.2.0/LICENSE` & `pydantic_zarr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_zarr-0.2.0/src/pydantic_zarr/core.py` & `pydantic_zarr-0.3.0/src/pydantic_zarr/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     Generic,
     Literal,
     Mapping,
     Optional,
     TypeVar,
     Union,
 )
-from pydantic import root_validator, validator
+from pydantic import BaseModel, root_validator, validator
 
 from pydantic.generics import GenericModel
 from zarr.storage import init_group, BaseStore
 import numcodecs
 import zarr
 import os
 import numpy as np
 import numpy.typing as npt
 from numcodecs.abc import Codec
 
-TAttrs = TypeVar("TAttrs", bound=Mapping[str, Any])
+TAttrs = TypeVar("TAttrs", bound=Union[Mapping[str, Any], BaseModel])
 TItem = TypeVar("TItem", bound=Union["GroupSpec", "ArraySpec"])
 
 DimensionSeparator = Union[Literal["."], Literal["/"]]
 ZarrVersion = Union[Literal[2], Literal[3]]
 ArrayOrder = Union[Literal["C"], Literal["F"]]
 
 
@@ -80,28 +80,45 @@
                 return v
             except AttributeError:
                 pass
         return v
 
     @root_validator
     def check_ndim(cls, values):
-        if (lshape := len(values["shape"])) != (lchunks := len(values["chunks"])):
-            msg = f"""
-            Length of shape must match length of chunks. Got {lshape} elements
-            for shape and {lchunks} elements for chunks.
-            """
-            raise ValueError(msg)
+        if "shape" in values and "chunks" in values:
+            if (lshape := len(values["shape"])) != (lchunks := len(values["chunks"])):
+                msg = f"""
+                Length of shape must match length of chunks. Got {lshape} elements
+                for shape and {lchunks} elements for chunks.
+                """
+                raise ValueError(msg)
         return values
 
     @classmethod
     def from_array(cls, array: npt.NDArray[Any], **kwargs):
+        """
+        Create an ArraySpec from a numpy array-like object.
+
+        Parameters
+        ----------
+        array : object that conforms to the numpy array API.
+            The shape and dtype of this object will be used to construct an ArraySpec.
+            If the `chunks` keyword argument is not given, the shape of the array will
+            be used for the chunks.
+
+        **kwargs : keyword arguments to the ArraySpec class constructor.
+
+        Returns
+        -------
+        An instance of ArraySpec with properties derived from the provided array.
 
+        """
         return cls(
             shape=array.shape,
-            dtype=array.dtype,
+            dtype=str(array.dtype),
             chunks=kwargs.pop("chunks", array.shape),
             attrs=kwargs.pop("attrs", {}),
             **kwargs,
         )
 
     @classmethod
     def from_zarr(cls, zarray: zarr.Array):
```

