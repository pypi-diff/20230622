# Comparing `tmp/dask_awkward-2023.6.2.tar.gz` & `tmp/dask_awkward-2023.6.3.tar.gz`

## Comparing `dask_awkward-2023.6.2.tar` & `dask_awkward-2023.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/_utils.py
--rw-r--r--   0        0        0    63799 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/unproject_layout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    16791 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/LICENSE
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/pyproject.toml
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0    10098 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/_utils.py
+-rw-r--r--   0        0        0    69121 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    26852 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/unproject_layout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/LICENSE
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/README.md
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/PKG-INFO
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.6.3/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/typing.py` & `dask_awkward-2023.6.3/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/utils.py` & `dask_awkward-2023.6.3/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.6.3/src/dask_awkward/layers/layers.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import copy
 import pickle
 from collections.abc import Callable, Mapping
 from typing import TYPE_CHECKING, Any
 
 from dask.blockwise import Blockwise, BlockwiseDepDict, blockwise_token
 from dask.highlevelgraph import MaterializedLayer
+from dask.layers import DataFrameTreeReduction
 
 from dask_awkward.utils import LazyInputsDict
 
 if TYPE_CHECKING:
     from awkward.typetracer import TypeTracerReport
 
 
@@ -19,15 +20,15 @@
 
     @classmethod
     def from_blockwise(cls, layer) -> AwkwardBlockwiseLayer:
         ob = object.__new__(cls)
         ob.__dict__.update(layer.__dict__)
         return ob
 
-    def mock(self):
+    def mock(self) -> tuple[AwkwardBlockwiseLayer, Any | None]:
         layer = copy.copy(self)
         nb = layer.numblocks
         layer.numblocks = {k: tuple(1 for _ in v) for k, v in nb.items()}
         layer.__dict__.pop("_dims", None)
         return layer, None
 
     def __getstate__(self) -> dict:
@@ -201,30 +202,81 @@
                 meta=self._meta,
                 behavior=self._behavior,
             )
         return self
 
 
 class AwkwardMaterializedLayer(MaterializedLayer):
-    def __init__(self, mapping, previous_layer_name, **kwargs):
-        self.prev_name = previous_layer_name
+    def __init__(
+        self,
+        mapping: dict,
+        *,
+        previous_layer_names: list[str],
+        fn: Callable | None = None,
+        **kwargs: Any,
+    ):
+        self.previous_layer_names: list[str] = previous_layer_names
+        self.fn = fn
         super().__init__(mapping, **kwargs)
 
-    def mock(self):
+    def mock(self) -> tuple[MaterializedLayer, Any | None]:
         mapping = self.mapping.copy()
         if not mapping:
             # no partitions at all
             return self, None
         name = next(iter(mapping))[0]
 
-        if (name, 0) in mapping:
-            task = mapping[(name, 0)]
-            task = tuple(
-                (self.prev_name, 0)
-                if isinstance(v, tuple) and len(v) == 2 and v[0] == self.prev_name
-                else v
-                for v in task
-            )
+        # one previous layer name
+        #
+        # this case is used for mocking repartition or slicing where
+        # we maybe have multiple partitions that need to be included
+        # in a task.
+        if len(self.previous_layer_names) == 1:
+            prev_name: str = self.previous_layer_names[0]
+            if (name, 0) in mapping:
+                task = mapping[(name, 0)]
+                task = tuple(
+                    (prev_name, 0)
+                    if isinstance(v, tuple) and len(v) == 2 and v[0] == prev_name
+                    else v
+                    for v in task
+                )
+
+                # when using Array.partitions we need to mock that we
+                # just want the first partition.
+                if len(task) == 2 and task[1] > 0:
+                    task = (task[0], 0)
+                return MaterializedLayer({(name, 0): task}), None
+            return self, None
+
+        # more than one previous_layer_names
+        #
+        # this case is needed for dak.concatenate on axis=0; we need
+        # the first partition of _each_ of the previous layer names!
+        else:
+            if self.fn is None:
+                raise ValueError(
+                    "For multiple previous layers the fn argument cannot be None."
+                )
+            name0s = tuple((name, 0) for name in self.previous_layer_names)
+            task = (self.fn, *name0s)
             return MaterializedLayer({(name, 0): task}), None
 
         # failed to cull during column opt
         return self, None
+
+
+class AwkwardTreeReductionLayer(DataFrameTreeReduction):
+    def mock(self) -> tuple[AwkwardTreeReductionLayer, Any | None]:
+        return (
+            AwkwardTreeReductionLayer(
+                name=self.name,
+                name_input=self.name_input,
+                npartitions_input=1,
+                concat_func=self.concat_func,
+                tree_node_func=self.tree_node_func,
+                finalize_func=self.finalize_func,
+                split_every=self.split_every,
+                tree_node_name=self.tree_node_name,
+            ),
+            None,
+        )
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/_utils.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/core.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,35 +6,40 @@
 import math
 import operator
 import sys
 import warnings
 from collections.abc import Callable, Hashable, Mapping, Sequence
 from functools import cached_property, partial
 from numbers import Number
-from typing import TYPE_CHECKING, Any, TypeVar
+from typing import TYPE_CHECKING, Any, Literal, TypeVar, overload
 
 import awkward as ak
 import dask.config
 import numpy as np
 from awkward._nplikes.typetracer import (
     MaybeNone,
     OneOf,
     TypeTracerArray,
     is_unknown_scalar,
 )
-from awkward.highlevel import _dir_pattern
-from dask.base import DaskMethodsMixin, dont_optimize, is_dask_collection, tokenize
+from awkward.highlevel import NDArrayOperatorsMixin, _dir_pattern
+from dask.base import (
+    DaskMethodsMixin,
+    dont_optimize,
+    is_dask_collection,
+    tokenize,
+    unpack_collections,
+)
 from dask.blockwise import BlockwiseDep
 from dask.blockwise import blockwise as dask_blockwise
 from dask.context import globalmethod
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 from dask.threaded import get as threaded_get
 from dask.utils import IndexCallable, funcname, key_split
-from numpy.lib.mixins import NDArrayOperatorsMixin
 from tlz import first
 
 from dask_awkward.layers import AwkwardBlockwiseLayer, AwkwardMaterializedLayer
 from dask_awkward.lib.optimize import all_optimizations
 from dask_awkward.typing import AwkwardDaskCollection
 from dask_awkward.utils import (
     DaskAwkwardNotImplemented,
@@ -638,15 +643,15 @@
     @property
     def divisions(self) -> tuple[int | None, ...]:
         """Location of the collections partition boundaries."""
         return self._divisions
 
     @property
     def known_divisions(self) -> bool:
-        """True of the divisions are known (absence of ``None`` in the tuple)."""
+        """True if the divisions are known (absence of ``None`` in the tuple)."""
         return len(self.divisions) > 0 and None not in self.divisions
 
     @property
     def npartitions(self) -> int:
         """Total number of partitions."""
         return len(self.divisions) - 1
 
@@ -703,16 +708,16 @@
         raw = normalize_index(index, (self.npartitions,))
         index = tuple(slice(k, k + 1) if isinstance(k, Number) else k for k in raw)  # type: ignore
         name = f"partitions-{token}"
         new_keys = self.keys_array[index].tolist()
         dsk = {(name, i): tuple(key) for i, key in enumerate(new_keys)}
         graph = HighLevelGraph.from_collections(
             name,
-            AwkwardMaterializedLayer(dsk, previous_layer_name=self.name),
-            dependencies=[self],
+            AwkwardMaterializedLayer(dsk, previous_layer_names=[self.name]),
+            dependencies=(self,),
         )
 
         # if a single partition was requested we trivially know the new divisions.
         if len(raw) == 1 and isinstance(raw[0], int) and self.known_divisions:
             new_divisions = (
                 0,
                 self.divisions[raw[0] + 1] - self.divisions[raw[0]],  # type: ignore
@@ -839,14 +844,22 @@
             if where == 0:
                 pidx, where = 0, 0
             else:
                 pidx, where = normalize_single_outer_inner_index(self.divisions, where)  # type: ignore
             partition = self.partitions[pidx]
             if partition._meta is not None:
                 new_meta = partition._meta[where]
+                # new_meta = make_unknown_length(partition._meta)[where]
+                # new_meta = ak.Array(
+                #     ak.to_backend(
+                #         partition._meta,
+                #         "typetracer",
+                #         highlevel=False,
+                #     ).to_typetracer(forget_length=True)
+                # )[where]
 
         # if we know a new array is going to be made, just call the
         # trivial inner on the new partition.
         if isinstance(new_meta, ak.Array):
             result = partition._getitem_trivial_map_partitions(where, meta=new_meta)
             result._divisions = (0, None)
             return result
@@ -862,15 +875,15 @@
                 _outer_int_getitem_fn,
                 partition.__dask_keys__()[0],
                 where,
             )
         }
         hlg = HighLevelGraph.from_collections(
             name,
-            AwkwardMaterializedLayer(dsk, previous_layer_name=self.name),
+            AwkwardMaterializedLayer(dsk, previous_layer_names=[self.name]),
             dependencies=[partition],
         )
         if isinstance(new_meta, ak.Record):
             return new_record_object(hlg, name, meta=new_meta)
         else:
             return new_scalar_object(hlg, name, meta=new_meta)
 
@@ -929,15 +942,15 @@
             ) % step
             remainder = step - remainder if remainder < 0 else remainder
             nextdiv = math.ceil((slice_end - slice_start) / step)
             divisions.append(divisions[-1] + nextdiv)
 
         hlg = HighLevelGraph.from_collections(
             name,
-            AwkwardMaterializedLayer(dask, previous_layer_name=self.name),
+            AwkwardMaterializedLayer(dask, previous_layer_names=[self.name]),
             dependencies=[self],
         )
         return new_array_object(
             hlg,
             name,
             meta=self._meta,
             behavior=self.behavior,
@@ -1150,41 +1163,44 @@
         except (IndexError, KeyError):
             raise AttributeError(f"{attr} not in fields.")
 
     def map_partitions(
         self,
         func: Callable,
         *args: Any,
+        traverse: bool = True,
         **kwargs: Any,
     ) -> Array:
         """Map a function across all partitions of the collection.
 
         Parameters
         ----------
         func : Callable
             Function to call on all partitions.
         *args : Collections and function arguments
             Additional arguments passed to `func` after the
             collection, if arguments are Array collections
             they must be compatibly partitioned with the object this
             method is being called from.
+        traverse : bool
+            Unpack basic python containers to find dask collections.
         **kwargs : Any
             Additional keyword arguments passed to the `func`.
 
         Returns
         -------
         dask_awkward.Array
             The new collection.
 
         See Also
         --------
         dask_awkward.map_partitions
 
         """
-        return map_partitions(func, self, *args, **kwargs)
+        return map_partitions(func, self, *args, traverse=traverse, **kwargs)
 
     def eager_compute_divisions(self) -> None:
         """Force a compute of the divisions."""
         self._divisions = calculate_known_divisions(self)
 
     def clear_divisions(self) -> None:
         """Clear the divisions of a Dask Awkward Collection."""
@@ -1438,30 +1454,66 @@
     )
     layer = AwkwardBlockwiseLayer.from_blockwise(layer)
     if opt_touch_all:
         layer._opt_touch_all = True
     return layer
 
 
+class ArgsKwargsPackedFunction:
+    def __init__(self, the_fn, arg_repackers, kwarg_repacker, arg_lens_for_repackers):
+        self.fn = the_fn
+        self.arg_repackers = arg_repackers
+        self.kwarg_repacker = kwarg_repacker
+        self.arg_lens_for_repackers = arg_lens_for_repackers
+
+    def __call__(self, *args_deps_expanded):
+        """This packing function receives a list of strictly
+        ordered arguments. The first range of arguments,
+        [0:sum(self.arg_lens_for_repackers)], corresponding to
+        the origin *args of self.fn but flattened to a list of
+        dask collections and non-dask-collection-containing arguments.
+        The remainder are the dask-collection-deps of self.fn's original
+        kwargs. The lengths of expected flattened inputs for each arg are
+        specified when this class is created, and we use that to process
+        the input flattened list of arguments sequentially.
+
+        The various repackers deal with restructuring the received flattened
+        list into the shape that self.fn expects.
+        """
+        args = []
+        len_args = 0
+        for repacker, n_args in zip(self.arg_repackers, self.arg_lens_for_repackers):
+            args.append(
+                repacker(args_deps_expanded[len_args : len_args + n_args])[0]
+                if repacker is not None
+                else args_deps_expanded[len_args]
+            )
+            len_args += n_args
+        kwargs = self.kwarg_repacker(args_deps_expanded[len_args:])[0]
+        return self.fn(*args, **kwargs)
+
+
 def map_partitions(
-    fn: Callable,
+    base_fn: Callable,
     *args: Any,
     label: str | None = None,
     token: str | None = None,
     meta: Any | None = None,
     output_divisions: int | None = None,
     opt_touch_all: bool = False,
+    traverse: bool = True,
     **kwargs: Any,
 ) -> Array:
     """Map a callable across all partitions of any number of collections.
 
     Parameters
     ----------
-    fn : Callable
-        Function to apply on all partitions.
+    base_fn : Callable
+        Function to apply on all partitions, this will get wraped to
+        handle kwargs, including dask collections.
     *args : Collections and function arguments
         Arguments passed to the function. Partitioned arguments (i.e.
         Dask collections) will have `fn` applied to each partition.
         Array collection arguments they must be compatibly
         partitioned.
     label : str, optional
         Label for the Dask graph layer; if left to ``None`` (default),
@@ -1484,14 +1536,16 @@
         means constant divisions (e.g. a string based slice). Any
         value greater than 1 means the divisions were expanded by some
         operation. This argument is mainly for internal library
         function implementations.
     opt_touch_all : bool
         Touch all layers in this graph during typetracer based
         optimization.
+    traverse : bool
+        Unpack basic python containers to find dask collections.
     **kwargs : Any
         Additional keyword arguments passed to the `fn`.
 
     Returns
     -------
     dask_awkward.Array
         The new collection.
@@ -1519,155 +1573,250 @@
     dask.awkward<multiply, npartitions=2>
     >>> d.compute()
     <Array [[1, 4, 9], [16], [5, 12, 21], [32]] type='4 * var * int64'>
 
     This is effectively the same as `d = c * a`
 
     """
-    token = token or tokenize(fn, *args, meta, **kwargs)
-    label = label or funcname(fn)
+    token = token or tokenize(base_fn, *args, meta, **kwargs)
+    label = hyphenize(label or funcname(base_fn))
     name = f"{label}-{token}"
+    kwarg_flat_deps, kwarg_repacker = unpack_collections(kwargs, traverse=traverse)
+    flat_deps, _ = unpack_collections(*args, *kwargs.values(), traverse=traverse)
+
+    arg_flat_deps_expanded = []
+    arg_repackers = []
+    arg_lens_for_repackers = []
+    for arg in args:
+        this_arg_flat_deps, repacker = unpack_collections(arg, traverse=traverse)
+        if (
+            len(this_arg_flat_deps) > 0
+        ):  # if the deps list is empty this arg does not contain any dask collection, no need to repack!
+            arg_flat_deps_expanded.extend(this_arg_flat_deps)
+            arg_repackers.append(repacker)
+            arg_lens_for_repackers.append(len(this_arg_flat_deps))
+        else:
+            arg_flat_deps_expanded.append(arg)
+            arg_repackers.append(None)
+            arg_lens_for_repackers.append(1)
+
+    fn = ArgsKwargsPackedFunction(
+        base_fn,
+        arg_repackers,
+        kwarg_repacker,
+        arg_lens_for_repackers,
+    )
+
     lay = partitionwise_layer(
         fn,
         name,
-        *args,
+        *arg_flat_deps_expanded,
+        *kwarg_flat_deps,
         opt_touch_all=opt_touch_all,
-        **kwargs,
     )
-    deps = [a for a in args if is_dask_collection(a)] + [
-        v for _, v in kwargs.items() if is_dask_collection(v)
-    ]
 
     if meta is None:
-        meta = map_meta(fn, *args, **kwargs)
+        meta = map_meta(fn, *arg_flat_deps_expanded, *kwarg_flat_deps)
 
     hlg = HighLevelGraph.from_collections(
         name,
         lay,
-        dependencies=deps,
+        dependencies=flat_deps,
     )
 
     if output_divisions is not None:
         if output_divisions == 1:
-            new_divisions = deps[0].divisions
+            new_divisions = flat_deps[0].divisions
         else:
             new_divisions = tuple(
-                map(lambda x: x * output_divisions, deps[0].divisions)
+                map(lambda x: x * output_divisions, flat_deps[0].divisions)
             )
         return new_array_object(
             hlg,
             name=name,
             meta=meta,
             divisions=new_divisions,
         )
     else:
         return new_array_object(
             hlg,
             name=name,
             meta=meta,
-            npartitions=deps[0].npartitions,
+            npartitions=flat_deps[0].npartitions,
         )
 
 
-def _from_iter(obj):
-    """Try to run ak.from_iter, but have fallbacks.
+PartialReductionType = ak.Array
 
-    This function first tries to call ak.form_iter on the input (which
-    should be some iterable). We expect a list of Scalar typetracers
-    to fail, so if the call fails due to ValueError or TypeError then
-    we manually do some typetracer operations to return the proper
-    representation of the input iterable-of-typetracers.
 
-    """
-    try:
-        return ak.from_iter(obj)
-    except (ValueError, TypeError):
-        first_obj = obj[0]
+def _chunk_reducer_non_positional(
+    chunk: ak.Array | PartialReductionType,
+    is_axis_none: bool,
+    *,
+    reducer: Callable,
+    mask_identity: bool,
+) -> PartialReductionType:
+    return reducer(
+        chunk,
+        keepdims=True,
+        axis=-1 if is_axis_none else 0,
+        mask_identity=mask_identity,
+    )
 
-        if isinstance(first_obj, MaybeNone):
-            first_obj = first_obj.content
 
-        return ak.Array(
-            ak.Array(first_obj)
-            .layout.form.length_one_array()
-            .layout.to_typetracer(forget_length=True)
-        )
+def _concat_reducer_non_positional(
+    partials: list[PartialReductionType], is_axis_none: bool
+) -> ak.Array:
+    concat_axis = -1 if is_axis_none else 0
+    return ak.concatenate(partials, axis=concat_axis)
 
 
-def total_reduction_to_scalar(
+def _finalise_reducer_non_positional(
+    partial: PartialReductionType,
+    is_axis_none: bool,
+    *,
+    reducer: Callable,
+    mask_identity: bool,
+    keepdims: bool,
+) -> ak.Array:
+    return reducer(
+        partial,
+        axis=None if is_axis_none else 0,
+        keepdims=keepdims,
+        mask_identity=mask_identity,
+    )
+
+
+def _prepare_axis_none_chunk(chunk: ak.Array) -> ak.Array:
+    # TODO: this is private Awkward code. We should figure out how to export it
+    # if needed
+    (layout,) = ak._do.remove_structure(
+        ak.to_layout(chunk),
+        flatten_records=False,
+        drop_nones=False,
+        keepdims=True,
+        allow_records=False,
+    )
+    return ak.Array(layout, behavior=chunk.behavior)
+
+
+def non_trivial_reduction(
     *,
     label: str,
     array: Array,
-    meta: Any,
-    chunked_fn: Callable,
-    comb_fn: Callable | None = None,
-    agg_fn: Callable | None = None,
+    axis: Literal[0] | None,
+    is_positional: bool,
+    keepdims: bool,
+    mask_identity: bool,
+    reducer: Callable,
+    combiner: Callable | None = None,
     token: str | None = None,
     dtype: Any | None = None,
     split_every: int | bool | None = None,
-    chunked_kwargs: dict[str, Any] | None = None,
-    comb_kwargs: dict[str, Any] | None = None,
-    agg_kwargs: dict[str, Any] | None = None,
-) -> Scalar:
-    from dask.layers import DataFrameTreeReduction
+):
+    if is_positional:
+        raise NotImplementedError("positional reducers at axis=0 or axis=None")
+
+    # Regularise the axis to (0, None)
+    if axis == 0 or axis == -1 * array.ndim:
+        axis = 0
+    elif axis is not None:
+        raise ValueError(axis)
+
+    if combiner is None:
+        combiner = reducer
+
+    if is_positional:
+        assert combiner is reducer
+
+    # For `axis=None`, we prepare each array to have the following structure:
+    #   [[[ ... [x1 x2 x3 ... xN] ... ]]] (length-1 outer lists)
+    # This makes the subsequent reductions an `axis=-1` reduction
+    if axis is None:
+        prepared_array = map_partitions(_prepare_axis_none_chunk, array)
+    else:
+        prepared_array = array
+
+    chunked_fn = _chunk_reducer_non_positional
+    tree_node_fn = _chunk_reducer_non_positional
+    concat_fn = _concat_reducer_non_positional
+    finalize_fn = _finalise_reducer_non_positional
+
+    chunked_kwargs = {
+        "reducer": reducer,
+        "is_axis_none": axis is None,
+        "mask_identity": mask_identity,
+    }
+    tree_node_kwargs = {
+        "reducer": combiner,
+        "is_axis_none": axis is None,
+        "mask_identity": mask_identity,
+    }
+
+    concat_kwargs = {"is_axis_none": axis is None}
+    finalize_kwargs = {
+        "reducer": combiner,
+        "mask_identity": mask_identity,
+        "keepdims": keepdims,
+        "is_axis_none": axis is None,
+    }
+
+    from dask_awkward.layers import AwkwardTreeReductionLayer
 
-    chunked_kwargs = chunked_kwargs or {}
     token = token or tokenize(
         array,
-        chunked_fn,
-        comb_fn,
-        agg_fn,
+        reducer,
         label,
         dtype,
         split_every,
         chunked_kwargs,
-        comb_kwargs,
-        agg_kwargs,
+        tree_node_kwargs,
+        concat_kwargs,
+        finalize_kwargs,
     )
-    name_comb = f"{label}-combine-{token}"
-    name_agg = f"{label}-agg-{token}"
-
-    comb_kwargs = comb_kwargs or chunked_kwargs
-    agg_kwargs = agg_kwargs or comb_kwargs
-
-    comb_fn = comb_fn or chunked_fn
-    agg_fn = agg_fn or comb_fn
+    name_tree_node = f"{label}-tree-node-{token}"
+    name_finalize = f"{label}-finalize-{token}"
 
     chunked_fn = partial(chunked_fn, **chunked_kwargs)
-    comb_fn = partial(comb_fn, **comb_kwargs)
-    agg_fn = partial(agg_fn, **agg_kwargs)
-
-    chunked_result = map_partitions(
-        chunked_fn,
-        array,
-        meta=empty_typetracer(),
-    )
+    tree_node_fn = partial(tree_node_fn, **tree_node_kwargs)
+    concat_fn = partial(concat_fn, **concat_kwargs)
+    finalize_fn = partial(finalize_fn, **finalize_kwargs)
 
     if split_every is None:
         split_every = 8
     elif split_every is False:
         split_every = sys.maxsize
     else:
         pass
 
-    dftr = DataFrameTreeReduction(
-        name=name_agg,
-        name_input=chunked_result.name,
-        npartitions_input=chunked_result.npartitions,
-        concat_func=_from_iter,
-        tree_node_func=comb_fn,
-        finalize_func=agg_fn,
+    chunked = map_partitions(chunked_fn, prepared_array, meta=empty_typetracer())
+
+    trl = AwkwardTreeReductionLayer(
+        name=name_finalize,
+        name_input=chunked.name,
+        npartitions_input=prepared_array.npartitions,
+        concat_func=concat_fn,
+        tree_node_func=tree_node_fn,
+        finalize_func=finalize_fn,
         split_every=split_every,
-        tree_node_name=name_comb,
+        tree_node_name=name_tree_node,
     )
 
-    graph = HighLevelGraph.from_collections(
-        name_agg, dftr, dependencies=(chunked_result,)
+    graph = HighLevelGraph.from_collections(name_finalize, trl, dependencies=(chunked,))
+
+    meta = reducer(
+        array._meta,
+        axis=axis,
+        keepdims=keepdims,
+        mask_identity=mask_identity,
     )
-    return new_scalar_object(graph, name_agg, meta=meta)
+    if isinstance(meta, ak.highlevel.Array):
+        return new_array_object(graph, name_finalize, meta=meta, npartitions=1)
+    else:
+        return new_scalar_object(graph, name_finalize, meta=meta)
 
 
 def calculate_known_divisions(array: Array) -> tuple[int, ...]:
     """Determine the divisions of a collection.
 
     This function triggers an immediate computation.
 
@@ -1709,32 +1858,14 @@
 
     """
     if array._meta is not None:
         return array._meta.layout.form.type
     return None
 
 
-def ndim(array: Array) -> int:
-    """Number of dimensions before reaching a numeric type or a record.
-
-    Parameters
-    ----------
-    array : dask_awkward.Array
-        The collection
-
-    Returns
-    -------
-    int or None
-        Number of dimensions as an integer, or ``None`` if the
-        collection does not contain metadata.
-
-    """
-    return array.ndim
-
-
 def is_awkward_collection(obj: Any) -> bool:
     """Check if an object is a Dask Awkward collection.
 
     Parameters
     ----------
     obj : Any
         The object of interest.
@@ -1813,29 +1944,41 @@
 
     """
     if is_awkward_collection(obj):
         return obj._meta
     return obj
 
 
+@overload
 def to_meta(objects: Sequence[Any]) -> tuple[Any, ...]:
-    """In a sequence convert Dask Awkward collections to their metas.
+    ...
+
+
+@overload
+def to_meta(objects: dict[str, Any]) -> dict[str, Any]:
+    ...
+
+
+def to_meta(objects):
+    """Convert sequence or dict of Dask Awkward collections to their metas.
 
     Parameters
     ----------
-    objects : Sequence[Any]
-        Sequence of objects.
+    objects : Sequence[Any] or dict[str, Any]
+        Sequence or dictionary of objects to retrieve metas from.
 
     Returns
     -------
-    tuple[Any, ...]
-        The sequence of objects where collections have been replaced
-        with their metadata.
+    tuple[Any, ...] or dict[str, Any]
+        The sequence of objects (or dictionary) where collections have
+        been replaced with their metadata.
 
     """
+    if isinstance(objects, dict):
+        return {k: meta_or_identity(v) for k, v in objects.items()}
     return tuple(map(meta_or_identity, objects))
 
 
 def length_zero_array_or_identity(obj: Any) -> Any:
     if is_awkward_collection(obj):
         return ak.Array(
             obj._meta.layout.form.length_zero_array(highlevel=False),
@@ -1844,18 +1987,19 @@
     return obj
 
 
 def to_length_zero_arrays(objects: Sequence[Any]) -> tuple[Any, ...]:
     return tuple(map(length_zero_array_or_identity, objects))
 
 
-def map_meta(fn: Callable, *args: Any, **kwargs: Any) -> ak.Array | None:
-    metas = to_meta(args)
+def map_meta(fn: Callable, *deps: Any) -> ak.Array | None:
+    # NOTE: fn is assumed to be a *packed* function
+    #       as defined up in map_partitions. be careful!
     try:
-        meta = fn(*metas, **kwargs)
+        meta = fn(*to_meta(deps))
         return meta
     except Exception as err:
         # if compute-unknown-meta is False then we don't care about
         # this failure and we return None.
         if not dask.config.get("awkward.compute-unknown-meta"):
             return None
 
@@ -1870,26 +2014,24 @@
         # warning and pass to the next try-except block.
         else:
             log.warning(
                 "function call on just metas failed; will try length zero array technique"
             )
         pass
     try:
-        lzas = to_length_zero_arrays(args)
-        meta = typetracer_from_form(fn(*lzas, **kwargs).layout.form)
+        arg_lzas = to_length_zero_arrays(deps)
+        meta = typetracer_from_form(fn(*arg_lzas).layout.form)
         return meta
     except Exception:
         # if compute-unknown-meta is True and we've gotten to this
         # point, we want to throw a warning because a compute is going
         # to happen as a consequence of us not being able to determine
         # metadata.
         if dask.config.get("awkward.compute-unknown-meta"):
-            extras = (
-                f"function call: {fn}\n" f"metadata: {metas}\n" f"kwargs: {kwargs}\n"
-            )
+            extras = f"function call: {fn}\n" f"metadata: {deps}\n"
             warnings.warn(
                 "metadata could not be determined; "
                 "a compute on the first partition will occur.\n"
                 f"{extras}",
                 UserWarning,
             )
     return None
@@ -1952,23 +2094,14 @@
             if arg.known_divisions:
                 if a.divisions != arg.divisions:
                     return False
 
     return True
 
 
-def compatible_divisions(*args: Array) -> bool:
-    if not all(a.known_divisions for a in args):
-        return False
-    for arg in args[1:]:
-        if arg.divisions != args[0].divisions:
-            return False
-    return True
-
-
 def empty_typetracer() -> ak.Array:
     """Instantiate a typetracer array with unknown length.
 
     Returns
     -------
     ak.Array
         Length-less typetracer array (content-less array).
@@ -2047,7 +2180,24 @@
     -------
     awkward.Array
         Resulting highlevel typetracer Array
 
     """
     layout = form.length_zero_array(highlevel=False)
     return ak.Array(layout.to_typetracer(forget_length=True))
+
+
+def make_unknown_length(array: ak.Array) -> ak.Array:
+    """Make any highlevel Array a highlevel typetracer Array with unknown length.
+
+    Parameters
+    ----------
+    array : ak.Array
+        Array of interest
+
+    Returns
+    -------
+    ak.Array
+        Highlevel typetracer Array with unknown length.
+
+    """
+    return ak.Array(ak.to_layout(array).to_typetracer(forget_length=True))
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import awkward as ak
 from dask.base import tokenize
 from dask.highlevelgraph import HighLevelGraph
 
+from dask_awkward.layers import AwkwardMaterializedLayer
 from dask_awkward.lib.core import (
     Array,
     compatible_partitions,
     map_partitions,
     new_array_object,
 )
 from dask_awkward.utils import DaskAwkwardNotImplemented, IncompatiblePartitions
@@ -17,14 +18,18 @@
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def __call__(self, *args):
         return ak.concatenate(list(args), **self.kwargs)
 
 
+def _concatenate_axis0_multiarg(*args):
+    return ak.concatenate(list(args), axis=0)
+
+
 def concatenate(
     arrays: list[Array],
     axis: int = 0,
     mergebool: bool = True,
     highlevel: bool = True,
     behavior: dict | None = None,
 ) -> Array:
@@ -41,14 +46,20 @@
             metas.append(collection._meta)
             for k in collection.__dask_keys__():
                 g[(name, i)] = k
                 i += 1
 
         meta = ak.concatenate(metas)
 
+        prev_names = [iarr.name for iarr in arrays]
+        g = AwkwardMaterializedLayer(
+            g,
+            previous_layer_names=prev_names,
+            fn=_concatenate_axis0_multiarg,
+        )
         hlg = HighLevelGraph.from_collections(name, g, dependencies=arrays)
         return new_array_object(hlg, name, meta=meta, npartitions=npartitions)
 
     if axis > 0:
         if not compatible_partitions(*arrays):
             raise IncompatiblePartitions("concatenate", *arrays)
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/reducers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 import awkward as ak
-import numpy as np
-from awkward._nplikes.typetracer import TypeTracerArray
 
-from dask_awkward.lib.core import map_partitions, total_reduction_to_scalar
+from dask_awkward.lib.core import map_partitions, non_trivial_reduction
 from dask_awkward.utils import DaskAwkwardNotImplemented, borrow_docstring
 
 if TYPE_CHECKING:
     from dask_awkward.lib.core import Array
 
 __all__ = (
     "all",
@@ -38,81 +36,117 @@
 @borrow_docstring(ak.all)
 def all(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     mask_identity: bool = False,
 ) -> Any:
-    if axis and axis != 0:
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="all",
+            array=array,
+            reducer=ak.all,
+            is_positional=False,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
+        )
+    else:
         return map_partitions(
             ak.all,
             array,
             output_divisions=1,
             axis=axis,
             keepdims=keepdims,
             mask_identity=mask_identity,
         )
-    raise DaskAwkwardNotImplemented(f"axis={axis} is a TODO")
 
 
 @borrow_docstring(ak.any)
 def any(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     mask_identity: bool = False,
 ) -> Any:
-    if axis and axis != 0:
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="any",
+            array=array,
+            reducer=ak.any,
+            is_positional=False,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
+        )
+    else:
         return map_partitions(
             ak.any,
             array,
             output_divisions=1,
             axis=axis,
             keepdims=keepdims,
             mask_identity=mask_identity,
         )
-    raise DaskAwkwardNotImplemented(f"axis={axis} is a TODO")
 
 
 @borrow_docstring(ak.argmax)
 def argmax(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     mask_identity: bool = True,
 ) -> Any:
-    if axis and axis >= 1:
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="argmax",
+            array=array,
+            reducer=ak.argmax,
+            is_positional=True,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
+        )
+    else:
         return map_partitions(
             ak.argmax,
             array,
             output_divisions=1,
             axis=axis,
             keepdims=keepdims,
             mask_identity=mask_identity,
         )
-    raise DaskAwkwardNotImplemented(f"axis={axis} is a TODO")
 
 
 @borrow_docstring(ak.argmin)
 def argmin(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     mask_identity: bool = True,
 ) -> Any:
-    if axis and axis >= 1:
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="argmin",
+            array=array,
+            reducer=ak.argmin,
+            is_positional=True,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
+        )
+    else:
         return map_partitions(
             ak.argmin,
             array,
             output_divisions=1,
             axis=axis,
             keepdims=keepdims,
             mask_identity=mask_identity,
         )
-    raise DaskAwkwardNotImplemented(f"axis={axis} is a TODO")
 
 
 @borrow_docstring(ak.corr)
 def corr(
     x,
     y,
     weight=None,
@@ -126,77 +160,63 @@
 @borrow_docstring(ak.count)
 def count(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     mask_identity: bool = False,
 ) -> Any:
-    if axis == 0 or axis == -1 * array.ndim:
-        raise DaskAwkwardNotImplemented(
-            f"axis={axis} is not supported for this array yet."
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="count",
+            array=array,
+            reducer=ak.count,
+            combiner=ak.sum,
+            is_positional=False,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
         )
-    if axis and axis != 0:
+    else:
         return map_partitions(
             ak.count,
             array,
             output_divisions=1,
             axis=axis,
             keepdims=keepdims,
             mask_identity=mask_identity,
         )
-    elif axis is None:
-        return total_reduction_to_scalar(
-            label="count",
-            array=array,
-            meta=TypeTracerArray._new(dtype=np.int64, shape=()),
-            chunked_fn=ak.count,
-            chunked_kwargs={"axis": 1},
-            comb_fn=ak.sum,
-            comb_kwargs={"axis": None},
-            agg_fn=ak.sum,
-            agg_kwargs={"axis": None},
-        )
-    else:
-        raise ValueError("axis must be None or an integer.")
 
 
 @borrow_docstring(ak.count_nonzero)
 def count_nonzero(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     mask_identity: bool = False,
 ) -> Any:
-    if axis == 0 or axis == -1 * array.ndim:
-        raise DaskAwkwardNotImplemented(
-            f"axis={axis} is not supported for this array yet."
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="count_nonzero",
+            array=array,
+            reducer=ak.count_nonzero,
+            combiner=ak.sum,
+            is_positional=False,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
         )
-    if axis and axis != 0:
+    else:
         return map_partitions(
             ak.count_nonzero,
             array,
             output_divisions=1,
-            axis=1,
+            axis=axis,
             keepdims=keepdims,
             mask_identity=mask_identity,
         )
-    elif axis is None:
-        return total_reduction_to_scalar(
-            label="count_nonzero",
-            array=array,
-            meta=TypeTracerArray._new(dtype=np.int64, shape=()),
-            chunked_fn=ak.count_nonzero,
-            chunked_kwargs={"axis": 1},
-            comb_fn=ak.sum,
-            comb_kwargs={"axis": None},
-            agg_fn=ak.sum,
-            agg_kwargs={"axis": None},
-        )
-    else:
-        raise ValueError("axis must be None or an integer.")
 
 
 @borrow_docstring(ak.covar)
 def covar(
     x,
     y,
     weight=None,
@@ -223,41 +243,33 @@
 def max(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     initial: float | None = None,
     mask_identity: bool = True,
 ) -> Any:
-    if axis == 0 or axis == -1 * array.ndim:
-        raise DaskAwkwardNotImplemented(
-            f"axis={axis} is not supported for this array yet."
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="max",
+            array=array,
+            reducer=ak.max,
+            is_positional=False,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
         )
-    if axis and axis != 0:
+    else:
         return map_partitions(
             ak.max,
             array,
             output_divisions=1,
             axis=axis,
             keepdims=keepdims,
-            initial=initial,
             mask_identity=mask_identity,
         )
-    if axis is None:
-        return total_reduction_to_scalar(
-            label="max",
-            array=array,
-            chunked_fn=ak.max,
-            chunked_kwargs={
-                "axis": None,
-                "mask_identity": mask_identity,
-            },
-            meta=ak.max(array._meta, axis=None),
-        )
-    else:
-        raise DaskAwkwardNotImplemented(f"axis={axis} is a TODO")
 
 
 @borrow_docstring(ak.mean)
 def mean(
     array,
     weight=None,
     axis=None,
@@ -284,41 +296,33 @@
 def min(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     initial: float | None = None,
     mask_identity: bool = True,
 ) -> Any:
-    if axis == 0 or axis == -1 * array.ndim:
-        raise DaskAwkwardNotImplemented(
-            f"axis={axis} is not supported for this array yet."
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="min",
+            array=array,
+            reducer=ak.min,
+            is_positional=False,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
         )
-    if axis and axis != 0:
+    else:
         return map_partitions(
             ak.min,
             array,
             output_divisions=1,
             axis=axis,
             keepdims=keepdims,
-            initial=initial,
             mask_identity=mask_identity,
         )
-    if axis is None:
-        return total_reduction_to_scalar(
-            label="min",
-            array=array,
-            chunked_fn=ak.min,
-            chunked_kwargs={
-                "axis": None,
-                "mask_identity": mask_identity,
-            },
-            meta=ak.min(array._meta, axis=None),
-        )
-    else:
-        raise DaskAwkwardNotImplemented(f"axis={axis} is a TODO")
 
 
 @borrow_docstring(ak.moment)
 def moment(
     x,
     n,
     weight=None,
@@ -327,15 +331,33 @@
     mask_identity=False,
 ):
     raise DaskAwkwardNotImplemented("TODO")
 
 
 @borrow_docstring(ak.prod)
 def prod(array, axis=None, keepdims=False, mask_identity=False):
-    raise DaskAwkwardNotImplemented("TODO")
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="prod",
+            array=array,
+            reducer=ak.prod,
+            is_positional=False,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
+        )
+    else:
+        return map_partitions(
+            ak.prod,
+            array,
+            output_divisions=1,
+            axis=axis,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
+        )
 
 
 @borrow_docstring(ak.ptp)
 def ptp(arr, axis=None, keepdims=False, mask_identity=True):
     raise DaskAwkwardNotImplemented("TODO")
 
 
@@ -384,44 +406,33 @@
 @borrow_docstring(ak.sum)
 def sum(
     array: Array,
     axis: int | None = None,
     keepdims: bool = False,
     mask_identity: bool = False,
 ) -> Any:
-    if axis == 0 or axis == -1 * array.ndim:
-        raise DaskAwkwardNotImplemented(
-            f"axis={axis} is not supported for this array yet."
+    if axis is None or axis == 0 or axis == -1 * array.ndim:
+        return non_trivial_reduction(
+            axis=axis,
+            label="sum",
+            array=array,
+            reducer=ak.sum,
+            is_positional=False,
+            keepdims=keepdims,
+            mask_identity=mask_identity,
         )
-    if axis and axis != 0:
+    else:
         return map_partitions(
             ak.sum,
             array,
             output_divisions=1,
             axis=axis,
             keepdims=keepdims,
             mask_identity=mask_identity,
         )
-    elif axis is None:
-        return total_reduction_to_scalar(
-            label="sum",
-            array=array,
-            chunked_fn=ak.sum,
-            chunked_kwargs={
-                "axis": None,
-                "mask_identity": mask_identity,
-            },
-            meta=ak.sum(array._meta, axis=None),
-        )
-    elif axis == 0:
-        raise DaskAwkwardNotImplemented(
-            f"axis={axis} is not supported for this array yet."
-        )
-    else:
-        raise ValueError("axis must be none or an integer")
 
 
 class _VarFn:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def __call__(self, array):
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,17 @@
 import builtins
 import warnings
 from collections.abc import Sequence
 from numbers import Number
 from typing import TYPE_CHECKING, Any
 
 import awkward as ak
-import numpy as np
-from awkward._nplikes.typetracer import TypeTracerArray
 from dask.base import is_dask_collection
 
-from dask_awkward.lib.core import (
-    Array,
-    compatible_partitions,
-    map_partitions,
-    new_known_scalar,
-    total_reduction_to_scalar,
-)
+from dask_awkward.lib.core import Array, compatible_partitions, map_partitions
 from dask_awkward.utils import (
     DaskAwkwardNotImplemented,
     IncompatiblePartitions,
     borrow_docstring,
 )
 
 if TYPE_CHECKING:
@@ -547,26 +539,15 @@
             ak.num,
             array,
             axis=axis,
             highlevel=highlevel,
             behavior=behavior,
         )
     if axis == 0:
-        if array.known_divisions:
-            return new_known_scalar(array.divisions[-1], dtype=int)
-        else:
-            return total_reduction_to_scalar(
-                label="num",
-                array=array,
-                meta=TypeTracerArray._new(dtype=np.int64, shape=()),
-                chunked_fn=ak.num,
-                chunked_kwargs={"axis": 0},
-                comb_fn=ak.sum,
-                comb_kwargs={"axis": None},
-            )
+        return len(array)
     raise DaskAwkwardNotImplemented("TODO")
 
 
 @borrow_docstring(ak.ones_like)
 def ones_like(
     array: Array,
     highlevel: bool = True,
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/testutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from __future__ import annotations
 
 import random
 from typing import Any
 
 import awkward as ak
+import numpy as np
 from dask.base import is_dask_collection
+from packaging.version import Version
 
 from dask_awkward.lib.core import Array, Record, typetracer_array
 from dask_awkward.lib.io.io import from_lists
 
 _RG = random.Random(414)
 
 
 DEFAULT_SCHEDULER: Any = "sync"
 
 
+NP_LTE_1_25_0 = Version(np.__version__) >= Version("1.25.0")
+AK_GTE_2_2_3 = Version(ak.__version__) <= Version("2.2.3")
+BAD_NP_AK_MIXIN_VERSIONING = NP_LTE_1_25_0 and AK_GTE_2_2_3
+
+
 def assert_eq(
     a: Any,
     b: Any,
-    check_forms: bool = True,
+    check_forms: bool = False,
     check_divisions: bool = True,
     scheduler: Any | None = None,
     **kwargs: Any,
 ) -> None:
     scheduler = scheduler or DEFAULT_SCHEDULER
     if isinstance(a, (Array, ak.Array)):
         assert_eq_arrays(
@@ -39,34 +46,38 @@
         assert_eq_other(a, b, scheduler=scheduler, **kwargs)
 
 
 def assert_eq_arrays(
     a: Array | ak.Array,
     b: Array | ak.Array,
     isclose_equal_nan: bool = False,
-    check_forms: bool = True,
+    check_forms: bool = False,
     check_divisions: bool = True,
     scheduler: Any | None = None,
 ) -> None:
     scheduler = scheduler or DEFAULT_SCHEDULER
     a_is_coll = is_dask_collection(a)
     b_is_coll = is_dask_collection(b)
     a_comp = a.compute(scheduler=scheduler) if a_is_coll else a
     b_comp = b.compute(scheduler=scheduler) if b_is_coll else b
-    a_comp_form = a_comp.layout.form
-    b_comp_form = b_comp.layout.form
 
     a_tt = typetracer_array(a)
     b_tt = typetracer_array(b)
     assert a_tt is not None
     assert b_tt is not None
 
     if check_forms:
-        assert a_comp_form == a.layout.form
-        assert a_comp_form == b.layout.form
+        a_form = ak.concatenate([a.layout, a.layout[0:0]], highlevel=False).form
+        b_form = ak.concatenate([b.layout, b.layout[0:0]], highlevel=False).form
+        # a_form = a.layout.form
+        # b_form = b.layout.form
+        a_comp_form = a_comp.layout.form
+        b_comp_form = b_comp.layout.form
+        assert a_comp_form == a_form
+        assert a_comp_form == b_form
         assert b_comp_form == a_comp_form
 
     if check_divisions:
         # check divisions if both collections
         if a_is_coll and b_is_coll:
             if a.known_divisions and b.known_divisions:
                 assert a.divisions == b.divisions
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/unproject_layout.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/unproject_layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -370,9 +370,37 @@
 
     # handle other cases that come up here...
 
     else:
         raise AssertionError(f"unexpected combination: {type(form)} and {type(layout)}")
 
 
-def unproject_layout(form: Form, layout: Content) -> Content:
+def unproject_layout(form: Form | None, layout: Content) -> Content:
+    """Rehydrate a layout to include all parts of an original form.
+
+    When we perform the necessary columns optimization we drop fields
+    that are not necessary for a computed result. Sometimes we have
+    task graphs that expect to see fields in name only (but no their
+    data). To protect against FieldNotFound exception we "unproject"
+    or "rehydrate" the layout with the original form. This reapplys
+    all original fields, but the ones that were orignally projected
+    away are data-less.
+
+    Parameters
+    ----------
+    form : awkward.forms.form.Form, optional
+        The complete Form to apply to a projected layout. If ``None``,
+        the layout will be returned without unprojection (this case
+        assumes column projection did not occur).
+    layout : awkward.contents.content.Content
+        The projected layout.
+
+    Returns
+    -------
+    awkward.contents.content.Content
+        Unprojected layout (all fields from the original form that did
+        not appear in the projected layout will be PlaceholderArrays).
+
+    """
+    if form is None:
+        return layout
     return _unproject_layout(form, layout, layout.length, layout.backend)
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/io/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 from awkward.types.numpytype import primitive_to_dtype
 from dask.base import flatten, tokenize
 from dask.highlevelgraph import HighLevelGraph
 from dask.utils import funcname
 
 from dask_awkward.layers import AwkwardBlockwiseLayer, AwkwardInputLayer
+from dask_awkward.layers.layers import AwkwardMaterializedLayer
 from dask_awkward.lib.core import (
     empty_typetracer,
     map_partitions,
     new_array_object,
     typetracer_array,
 )
 
@@ -180,15 +181,18 @@
         Resulting Array collection.
 
     """
     from dask.delayed import Delayed
 
     parts = [source] if isinstance(source, Delayed) else source
     name = f"{prefix}-{tokenize(parts)}"
-    dsk = {(name, i): part.key for i, part in enumerate(parts)}
+    dsk = AwkwardMaterializedLayer(
+        {(name, i): part.key for i, part in enumerate(parts)},
+        previous_layer_names=[parts[0].name],
+    )
     if divisions is None:
         divs: tuple[int | None, ...] = (None,) * (len(parts) + 1)
     else:
         divs = tuple(divisions)
         if len(divs) != len(parts) + 1:
             raise ValueError("divisions must be a tuple of length len(source) + 1")
     hlg = HighLevelGraph.from_collections(name, dsk, dependencies=parts)
```

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.6.3/src/dask_awkward/lib/io/parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     Array
         Array collection from the parquet dataset.
 
     """
     fs, tok, paths = get_fs_token_paths(
         path, mode="rb", storage_options=storage_options
     )
-    label = "read-parquet"
+    label = "from-parquet"
     token = tokenize(
         tok, paths, ignore_metadata, columns, filters, scan_files, split_row_groups
     )
 
     # same as ak_metadata_from_parquet
     results = ak_from_parquet.metadata(
         path,
```

### Comparing `dask_awkward-2023.6.2/.gitignore` & `dask_awkward-2023.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/LICENSE` & `dask_awkward-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/README.md` & `dask_awkward-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.2/pyproject.toml` & `dask_awkward-2023.6.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -33,36 +33,35 @@
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-awkward"
 "Bug Tracker" = "https://github.com/dask-contrib/dask-awkward/issues"
 
 [project.optional-dependencies]
+io = [
+  "aiohttp",
+  "pyarrow",
+]
 complete = [
   "aiohttp",
   "pyarrow",
-  "pytest >=6.0",
-  "pytest-cov >=3.0.0",
-  "requests >=2.27.1",
 ]
+# `docs` and `test` are separate from user installs
 docs = [
   "dask-sphinx-theme >=3.0.2",
   "pyarrow",
   "sphinx-design",
   "pytest >=6.0",
   "pytest-cov >=3.0.0",
   "requests >=2.27.1",
 ]
-io = [
-  "aiohttp",
-  "pyarrow",
-]
 test = [
   "aiohttp",
   "distributed",
+  "pandas",
   "pyarrow",
   "pytest >=6.0",
   "pytest-cov >=3.0.0",
   "requests >=2.27.1",
 ]
 
 [project.entry-points."dask.sizeof"]
```

### Comparing `dask_awkward-2023.6.2/PKG-INFO` & `dask_awkward-2023.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -18,30 +18,28 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: awkward>=2.2.2
 Requires-Dist: dask>=2023.04.0
 Provides-Extra: complete
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: pyarrow; extra == 'complete'
-Requires-Dist: pytest-cov>=3.0.0; extra == 'complete'
-Requires-Dist: pytest>=6.0; extra == 'complete'
-Requires-Dist: requests>=2.27.1; extra == 'complete'
 Provides-Extra: docs
 Requires-Dist: dask-sphinx-theme>=3.0.2; extra == 'docs'
 Requires-Dist: pyarrow; extra == 'docs'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'docs'
 Requires-Dist: pytest>=6.0; extra == 'docs'
 Requires-Dist: requests>=2.27.1; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Provides-Extra: io
 Requires-Dist: aiohttp; extra == 'io'
 Requires-Dist: pyarrow; extra == 'io'
 Provides-Extra: test
 Requires-Dist: aiohttp; extra == 'test'
 Requires-Dist: distributed; extra == 'test'
+Requires-Dist: pandas; extra == 'test'
 Requires-Dist: pyarrow; extra == 'test'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
 Requires-Dist: requests>=2.27.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 dask-awkward
```

