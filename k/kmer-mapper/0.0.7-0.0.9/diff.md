# Comparing `tmp/kmer_mapper-0.0.7.tar.gz` & `tmp/kmer_mapper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmer_mapper-0.0.7.tar", last modified: Fri Dec  3 12:04:08 2021, max compression
+gzip compressed data, was "kmer_mapper-0.0.9.tar", last modified: Mon Dec  6 20:01:20 2021, max compression
```

## Comparing `kmer_mapper-0.0.7.tar` & `kmer_mapper-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-03 12:04:08.286924 kmer_mapper-0.0.7/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        0 2021-11-28 15:14:38.000000 kmer_mapper-0.0.7/MANIFEST.in
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      267 2021-12-03 12:04:08.286924 kmer_mapper-0.0.7/PKG-INFO
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-03 12:04:08.286924 kmer_mapper-0.0.7/kmer_mapper/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2717 2021-12-03 10:30:09.000000 kmer_mapper-0.0.7/kmer_mapper/command_line_interface.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)  1159491 2021-12-02 21:25:47.000000 kmer_mapper-0.0.7/kmer_mapper/mapper.c
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     9621 2021-12-02 21:25:44.000000 kmer_mapper-0.0.7/kmer_mapper/mapper.pyx
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7612 2021-12-02 21:55:20.000000 kmer_mapper-0.0.7/kmer_mapper/mapping.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      591 2021-11-21 22:30:10.000000 kmer_mapper-0.0.7/kmer_mapper/util.py
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-03 12:04:08.286924 kmer_mapper-0.0.7/kmer_mapper.egg-info/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      267 2021-12-03 12:04:08.000000 kmer_mapper-0.0.7/kmer_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      406 2021-12-03 12:04:08.000000 kmer_mapper-0.0.7/kmer_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        1 2021-12-03 12:04:08.000000 kmer_mapper-0.0.7/kmer_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       73 2021-12-03 12:04:08.000000 kmer_mapper-0.0.7/kmer_mapper.egg-info/entry_points.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        1 2021-11-21 18:51:26.000000 kmer_mapper-0.0.7/kmer_mapper.egg-info/not-zip-safe
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       50 2021-12-03 12:04:08.000000 kmer_mapper-0.0.7/kmer_mapper.egg-info/requires.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       19 2021-12-03 12:04:08.000000 kmer_mapper-0.0.7/kmer_mapper.egg-info/top_level.txt
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      108 2021-11-28 14:45:09.000000 kmer_mapper-0.0.7/pyproject.toml
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       38 2021-12-03 12:04:08.286924 kmer_mapper-0.0.7/setup.cfg
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     1377 2021-12-03 12:04:01.000000 kmer_mapper-0.0.7/setup.py
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-06 20:01:20.200743 kmer_mapper-0.0.9/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        0 2021-11-28 15:14:38.000000 kmer_mapper-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      267 2021-12-06 20:01:20.200743 kmer_mapper-0.0.9/PKG-INFO
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-06 20:01:20.196743 kmer_mapper-0.0.9/kmer_mapper/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2717 2021-12-03 10:30:09.000000 kmer_mapper-0.0.9/kmer_mapper/command_line_interface.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)  1102136 2021-12-06 20:01:20.000000 kmer_mapper-0.0.9/kmer_mapper/mapper.c
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7525 2021-12-06 20:01:01.000000 kmer_mapper-0.0.9/kmer_mapper/mapper.pyx
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7606 2021-12-06 20:01:01.000000 kmer_mapper-0.0.9/kmer_mapper/mapping.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      591 2021-11-21 22:30:10.000000 kmer_mapper-0.0.9/kmer_mapper/util.py
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-06 20:01:20.200743 kmer_mapper-0.0.9/kmer_mapper.egg-info/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      267 2021-12-06 20:01:20.000000 kmer_mapper-0.0.9/kmer_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      406 2021-12-06 20:01:20.000000 kmer_mapper-0.0.9/kmer_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        1 2021-12-06 20:01:20.000000 kmer_mapper-0.0.9/kmer_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       73 2021-12-06 20:01:20.000000 kmer_mapper-0.0.9/kmer_mapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)        1 2021-11-21 18:51:26.000000 kmer_mapper-0.0.9/kmer_mapper.egg-info/not-zip-safe
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       72 2021-12-06 20:01:20.000000 kmer_mapper-0.0.9/kmer_mapper.egg-info/requires.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       19 2021-12-06 20:01:20.000000 kmer_mapper-0.0.9/kmer_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      108 2021-11-28 14:45:09.000000 kmer_mapper-0.0.9/pyproject.toml
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)       38 2021-12-06 20:01:20.200743 kmer_mapper-0.0.9/setup.cfg
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     1402 2021-12-06 20:01:08.000000 kmer_mapper-0.0.9/setup.py
```

### Comparing `kmer_mapper-0.0.7/kmer_mapper/command_line_interface.py` & `kmer_mapper-0.0.9/kmer_mapper/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `kmer_mapper-0.0.7/kmer_mapper/mapper.c` & `kmer_mapper-0.0.9/kmer_mapper/mapper.c`

 * *Files 0% similar despite different names*

```diff
@@ -1185,16 +1185,15 @@
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
-struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta;
-struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks;
+struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
 /* "../../../../usr/local/lib/python3.8/dist-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
@@ -1228,42 +1227,22 @@
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "mapper.pyx":56
- *         i_reverse_complement -= 1
- * 
- * def read_fasta(filename):             # <<<<<<<<<<<<<<
- *     filename_byte_string = filename.encode("UTF-8")
- *     cdef char * fname = filename_byte_string
- */
-struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta {
-  PyObject_HEAD
-  FILE *__pyx_v_cfile;
-  PyObject *__pyx_v_filename;
-  PyObject *__pyx_v_filename_byte_string;
-  char *__pyx_v_fname;
-  PyObject *__pyx_v_i;
-  size_t __pyx_v_l;
-  char *__pyx_v_line;
-  Py_ssize_t __pyx_v_read;
-};
-
-
-/* "mapper.pyx":90
+/* "mapper.pyx":65
  * 
  * 
  * def read_fasta_into_chunks(filename, chunk_size=1000, int max_read_length=150, write_to_shared_memory=False, process_reads=False):             # <<<<<<<<<<<<<<
  *     logging.info("Reading fasta %s" % filename)
  *     filename_byte_string = filename.encode("UTF-8")
  */
-struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks {
+struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks {
   PyObject_HEAD
   FILE *__pyx_v_cfile;
   PyObject *__pyx_v_chunk;
   PyObject *__pyx_v_chunk_size;
   PyObject *__pyx_v_filename;
   PyObject *__pyx_v_filename_byte_string;
   char *__pyx_v_fname;
@@ -1631,16 +1610,28 @@
 static void __Pyx_RaiseBufferIndexError(int axis);
 
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* RaiseDoubleKeywords.proto */
+static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+
+/* ParseKeywords.proto */
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+    const char* function_name);
+
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
@@ -1681,32 +1672,20 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
+/* PyObjectCall2Args.proto */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* RaiseDoubleKeywords.proto */
-static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
-
-/* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
-    const char* function_name);
-
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
-
 /* SliceObject.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(
         PyObject* obj, Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
         int has_cstart, int has_cstop, int wraparound);
 
 /* GetItemInt.proto */
@@ -1766,14 +1745,15 @@
 static int  __Pyx__GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
     __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
 static void __Pyx_ZeroBuffer(Py_buffer* buf);
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
+#define __Pyx_BufPtrStrided1d(type, buf, i0, s0) (type)((char*)buf + i0 * s0)
 /* MemviewSliceInit.proto */
 #define __Pyx_BUF_MAX_NDIMS %(BUF_MAX_NDIMS)d
 #define __Pyx_MEMVIEW_DIRECT   1
 #define __Pyx_MEMVIEW_PTR      2
 #define __Pyx_MEMVIEW_FULL     4
 #define __Pyx_MEMVIEW_CONTIG   8
 #define __Pyx_MEMVIEW_STRIDED  16
@@ -1792,15 +1772,14 @@
 #define __pyx_get_slice_count_pointer(memview) (memview->acquisition_count_aligned_p)
 #define __pyx_get_slice_count(memview) (*__pyx_get_slice_count_pointer(memview))
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XDEC_MEMVIEW(slice, have_gil) __Pyx_XDEC_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *, int, int);
 
-#define __Pyx_BufPtrStrided1d(type, buf, i0, s0) (type)((char*)buf + i0 * s0)
 /* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
@@ -2349,32 +2328,28 @@
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'cython.view' */
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'mapper' */
-static PyTypeObject *__pyx_ptype_6mapper___pyx_scope_struct__read_fasta = 0;
-static PyTypeObject *__pyx_ptype_6mapper___pyx_scope_struct_1_read_fasta_into_chunks = 0;
+static PyTypeObject *__pyx_ptype_6mapper___pyx_scope_struct__read_fasta_into_chunks = 0;
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
 static PyTypeObject *__pyx_memoryview_type = 0;
 static PyTypeObject *__pyx_memoryviewslice_type = 0;
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
 static PyObject *__pyx_f_6mapper_test(int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_6mapper_count_lines_in_fasta(PyObject *, int __pyx_skip_dispatch); /*proto*/
-static void __pyx_f_6mapper_read_sequence_to_kmer_hashes(char *, __Pyx_memviewslice, __Pyx_memviewslice, int); /*proto*/
-static PyObject *__pyx_f_6mapper_handle_reads(PyObject *, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_6mapper_get_count(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static void *__pyx_align_pointer(void *, size_t); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static PyObject *assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
 static struct __pyx_memoryview_obj *__pyx_memview_slice(struct __pyx_memoryview_obj *, PyObject *); /*proto*/
@@ -2400,17 +2375,17 @@
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float_t = { "float_t", NULL, sizeof(__pyx_t_5numpy_float_t), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t = { "uint64_t", NULL, sizeof(__pyx_t_5numpy_uint64_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_uint64_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_uint64_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t = { "int64_t", NULL, sizeof(__pyx_t_5numpy_int64_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int64_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int64_t), 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float_t = { "float_t", NULL, sizeof(__pyx_t_5numpy_float_t), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_uint32_t = { "uint32_t", NULL, sizeof(__pyx_t_5numpy_uint32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_uint32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_uint32_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_uint16_t = { "uint16_t", NULL, sizeof(__pyx_t_5numpy_uint16_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_uint16_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_uint16_t), 0 };
 #define __Pyx_MODULE_NAME "mapper"
 extern int __pyx_module_is_main_mapper;
 int __pyx_module_is_main_mapper = 0;
 
 /* Implementation of 'mapper' */
@@ -2438,14 +2413,15 @@
 static const char __pyx_k_3f[] = ".3f";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_sa[] = "sa";
 static const char __pyx_k_mod[] = "mod";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
+static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_Took[] = "Took ";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_exit[] = "__exit__";
 static const char __pyx_k_hash[] = "hash";
@@ -2481,25 +2457,22 @@
 static const char __pyx_k_fname[] = "fname";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_kmers[] = "kmers";
 static const char __pyx_k_name1[] = "name1";
 static const char __pyx_k_name2[] = "name2";
 static const char __pyx_k_nodes[] = "_nodes";
 static const char __pyx_k_numpy[] = "numpy";
-static const char __pyx_k_power[] = "power";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_test2[] = "test2";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_uint8[] = "uint8";
-static const char __pyx_k_valid[] = "valid";
 static const char __pyx_k_zeros[] = "zeros";
-static const char __pyx_k_arange[] = "arange";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_mapper[] = "mapper";
 static const char __pyx_k_modulo[] = "_modulo";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
@@ -2512,15 +2485,14 @@
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_kmers_2[] = "_kmers";
 static const char __pyx_k_logging[] = "logging";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_n_kmers[] = "_n_kmers";
 static const char __pyx_k_nodes_2[] = "nodes";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
-static const char __pyx_k_convolve[] = "convolve";
 static const char __pyx_k_filename[] = "filename";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_modulo_2[] = "modulo";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
@@ -2531,15 +2503,14 @@
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_chunk_size[] = "chunk_size";
 static const char __pyx_k_frombuffer[] = "frombuffer";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
-static const char __pyx_k_read_fasta[] = "read_fasta";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_SharedArray[] = "SharedArray";
 static const char __pyx_k_frequencies[] = "_frequencies";
 static const char __pyx_k_index_kmers[] = "index_kmers";
 static const char __pyx_k_kmer_hashes[] = "kmer_hashes";
@@ -2654,29 +2625,27 @@
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_kp_u_Yielding_chunk_with;
 static PyObject *__pyx_kp_u_Yielding_d_reads_directly;
 static PyObject *__pyx_kp_u_Yielding_d_reads_in_the_end;
 static PyObject *__pyx_n_s_allocate_buffer;
-static PyObject *__pyx_n_s_arange;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_bool;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_cfile;
 static PyObject *__pyx_n_s_chunk;
 static PyObject *__pyx_n_s_chunk_size;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
-static PyObject *__pyx_n_s_convolve;
 static PyObject *__pyx_n_u_d;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
 static PyObject *__pyx_n_s_empty;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enter;
@@ -2753,15 +2722,14 @@
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_open;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pickle;
-static PyObject *__pyx_n_s_power;
 static PyObject *__pyx_n_s_prev_time;
 static PyObject *__pyx_n_s_print;
 static PyObject *__pyx_n_s_process_reads;
 static PyObject *__pyx_n_s_py_read_file;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
@@ -2770,15 +2738,14 @@
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_u_r;
 static PyObject *__pyx_n_s_random;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_read;
-static PyObject *__pyx_n_s_read_fasta;
 static PyObject *__pyx_n_s_read_fasta_into_chunks;
 static PyObject *__pyx_kp_u_reads_in_shared_memory;
 static PyObject *__pyx_kp_u_reads_into_matrix;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_ref_offsets;
@@ -2795,38 +2762,35 @@
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
+static PyObject *__pyx_n_s_sys;
 static PyObject *__pyx_n_s_t;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_u_test2;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_to_shared_memory;
 static PyObject *__pyx_n_s_uint64;
 static PyObject *__pyx_n_s_uint8;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_util;
-static PyObject *__pyx_n_u_valid;
 static PyObject *__pyx_n_s_write_to_shared_memory;
 static PyObject *__pyx_n_s_zeros;
 static PyObject *__pyx_pf_6mapper_py_read_file(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename); /* proto */
 static PyObject *__pyx_pf_6mapper_2test(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6mapper_4count_lines_in_fasta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_file_name); /* proto */
-static PyObject *__pyx_pf_6mapper_6read_fasta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename); /* proto */
-static PyObject *__pyx_pf_6mapper_9read_fasta_into_chunks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_chunk_size, int __pyx_v_max_read_length, PyObject *__pyx_v_write_to_shared_memory, PyObject *__pyx_v_process_reads); /* proto */
-static PyObject *__pyx_pf_6mapper_12handle_reads(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename); /* proto */
-static PyObject *__pyx_pf_6mapper_14get_count(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename); /* proto */
-static PyObject *__pyx_pf_6mapper_16map_kmers_to_graph_index(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_index, int __pyx_v_max_node_id, __Pyx_memviewslice __pyx_v_kmers, int __pyx_v_max_index_lookup_frequency); /* proto */
+static PyObject *__pyx_pf_6mapper_6read_fasta_into_chunks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_chunk_size, int __pyx_v_max_read_length, PyObject *__pyx_v_write_to_shared_memory, PyObject *__pyx_v_process_reads); /* proto */
+static PyObject *__pyx_pf_6mapper_9map_kmers_to_graph_index(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_index, int __pyx_v_max_node_id, __Pyx_memviewslice __pyx_v_kmers, int __pyx_v_max_index_lookup_frequency); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2861,69 +2825,65 @@
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_6mapper___pyx_scope_struct__read_fasta(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_6mapper___pyx_scope_struct_1_read_fasta_into_chunks(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_6mapper___pyx_scope_struct__read_fasta_into_chunks(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
-static PyObject *__pyx_int_4;
 static PyObject *__pyx_int_1000;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple_;
-static PyObject *__pyx_slice__5;
+static PyObject *__pyx_slice__4;
 static PyObject *__pyx_tuple__2;
+static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__22;
+static PyObject *__pyx_slice__21;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
-static PyObject *__pyx_tuple__26;
+static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
-static PyObject *__pyx_tuple__36;
-static PyObject *__pyx_tuple__37;
 static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__4;
-static PyObject *__pyx_codeobj__27;
-static PyObject *__pyx_codeobj__31;
-static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__26;
+static PyObject *__pyx_codeobj__29;
+static PyObject *__pyx_codeobj__36;
 /* Late includes */
 
-/* "mapper.pyx":12
- * from graph_kmer_index.shared_mem import to_shared_memory, SingleSharedArray
+/* "mapper.pyx":13
+ * import sys
  * 
  * def py_read_file(filename):             # <<<<<<<<<<<<<<
  *     with open(filename, "r") as f:
  *         return f.read()
  */
 
 /* Python wrapper */
@@ -2956,50 +2916,50 @@
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("py_read_file", 0);
 
-  /* "mapper.pyx":13
+  /* "mapper.pyx":14
  * 
  * def py_read_file(filename):
  *     with open(filename, "r") as f:             # <<<<<<<<<<<<<<
  *         return f.read()
  * 
  */
   /*with:*/ {
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_filename);
     __Pyx_GIVEREF(__pyx_v_filename);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_filename);
     __Pyx_INCREF(__pyx_n_u_r);
     __Pyx_GIVEREF(__pyx_n_u_r);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_r);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L3_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L3_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
@@ -3009,80 +2969,80 @@
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
           __pyx_v_f = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "mapper.pyx":14
+          /* "mapper.pyx":15
  * def py_read_file(filename):
  *     with open(filename, "r") as f:
  *         return f.read()             # <<<<<<<<<<<<<<
  * 
  * cpdef test():
  */
           __Pyx_XDECREF(__pyx_r);
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_1 = NULL;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
             __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
             if (likely(__pyx_t_1)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
               __Pyx_INCREF(__pyx_t_1);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_2, function);
             }
           }
           __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L7_error)
+          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_r = __pyx_t_4;
           __pyx_t_4 = 0;
           goto __pyx_L11_try_return;
 
-          /* "mapper.pyx":13
+          /* "mapper.pyx":14
  * 
  * def py_read_file(filename):
  *     with open(filename, "r") as f:             # <<<<<<<<<<<<<<
  *         return f.read()
  * 
  */
         }
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("mapper.py_read_file", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 13, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 14, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 13, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 14, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 13, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 14, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 13, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 14, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_XGIVEREF(__pyx_t_1);
             __Pyx_ErrRestoreWithState(__pyx_t_4, __pyx_t_2, __pyx_t_1);
             __pyx_t_4 = 0; __pyx_t_2 = 0; __pyx_t_1 = 0; 
-            __PYX_ERR(0, 13, __pyx_L9_except_error)
+            __PYX_ERR(0, 14, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -3105,27 +3065,27 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_3) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple_, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 13, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 14, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L4_return: {
         __pyx_t_8 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_3) {
           __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple_, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 13, __pyx_L1_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 14, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __pyx_r = __pyx_t_8;
         __pyx_t_8 = 0;
         goto __pyx_L0;
       }
@@ -3134,16 +3094,16 @@
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "mapper.pyx":12
- * from graph_kmer_index.shared_mem import to_shared_memory, SingleSharedArray
+  /* "mapper.pyx":13
+ * import sys
  * 
  * def py_read_file(filename):             # <<<<<<<<<<<<<<
  *     with open(filename, "r") as f:
  *         return f.read()
  */
 
   /* function exit code */
@@ -3159,15 +3119,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_f);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mapper.pyx":16
+/* "mapper.pyx":17
  *         return f.read()
  * 
  * cpdef test():             # <<<<<<<<<<<<<<
  *     print("test2")
  * 
  */
 
@@ -3177,26 +3137,26 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test", 0);
 
-  /* "mapper.pyx":17
+  /* "mapper.pyx":18
  * 
  * cpdef test():
  *     print("test2")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mapper.pyx":16
+  /* "mapper.pyx":17
  *         return f.read()
  * 
  * cpdef test():             # <<<<<<<<<<<<<<
  *     print("test2")
  * 
  */
 
@@ -3231,15 +3191,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6mapper_test(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6mapper_test(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3248,15 +3208,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mapper.pyx":20
+/* "mapper.pyx":21
  * 
  * 
  * cpdef count_lines_in_fasta(file_name):             # <<<<<<<<<<<<<<
  *     i = 0
  *     with open(file_name) as f:
  */
 
@@ -3281,51 +3241,51 @@
   int __pyx_t_12;
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("count_lines_in_fasta", 0);
 
-  /* "mapper.pyx":21
+  /* "mapper.pyx":22
  * 
  * cpdef count_lines_in_fasta(file_name):
  *     i = 0             # <<<<<<<<<<<<<<
  *     with open(file_name) as f:
  *         #data = f.read()
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_i = __pyx_int_0;
 
-  /* "mapper.pyx":22
+  /* "mapper.pyx":23
  * cpdef count_lines_in_fasta(file_name):
  *     i = 0
  *     with open(file_name) as f:             # <<<<<<<<<<<<<<
  *         #data = f.read()
  *         for line in f:
  */
   /*with:*/ {
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_open, __pyx_v_file_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_open, __pyx_v_file_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 22, __pyx_L3_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 23, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L3_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __pyx_t_3;
     __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
@@ -3335,86 +3295,86 @@
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
           __pyx_v_f = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "mapper.pyx":24
+          /* "mapper.pyx":25
  *     with open(file_name) as f:
  *         #data = f.read()
  *         for line in f:             # <<<<<<<<<<<<<<
  *             i += 1
  * 
  */
           if (likely(PyList_CheckExact(__pyx_v_f)) || PyTuple_CheckExact(__pyx_v_f)) {
             __pyx_t_4 = __pyx_v_f; __Pyx_INCREF(__pyx_t_4); __pyx_t_9 = 0;
             __pyx_t_10 = NULL;
           } else {
-            __pyx_t_9 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_f); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L7_error)
+            __pyx_t_9 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_f); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_4);
-            __pyx_t_10 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 24, __pyx_L7_error)
+            __pyx_t_10 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 25, __pyx_L7_error)
           }
           for (;;) {
             if (likely(!__pyx_t_10)) {
               if (likely(PyList_CheckExact(__pyx_t_4))) {
                 if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_4)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_1 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_9); __Pyx_INCREF(__pyx_t_1); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 24, __pyx_L7_error)
+                __pyx_t_1 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_9); __Pyx_INCREF(__pyx_t_1); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 25, __pyx_L7_error)
                 #else
-                __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L7_error)
+                __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_1);
                 #endif
               } else {
                 if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_9); __Pyx_INCREF(__pyx_t_1); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 24, __pyx_L7_error)
+                __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_9); __Pyx_INCREF(__pyx_t_1); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 25, __pyx_L7_error)
                 #else
-                __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L7_error)
+                __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_1);
                 #endif
               }
             } else {
               __pyx_t_1 = __pyx_t_10(__pyx_t_4);
               if (unlikely(!__pyx_t_1)) {
                 PyObject* exc_type = PyErr_Occurred();
                 if (exc_type) {
                   if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                  else __PYX_ERR(0, 24, __pyx_L7_error)
+                  else __PYX_ERR(0, 25, __pyx_L7_error)
                 }
                 break;
               }
               __Pyx_GOTREF(__pyx_t_1);
             }
             __Pyx_XDECREF_SET(__pyx_v_line, __pyx_t_1);
             __pyx_t_1 = 0;
 
-            /* "mapper.pyx":25
+            /* "mapper.pyx":26
  *         #data = f.read()
  *         for line in f:
  *             i += 1             # <<<<<<<<<<<<<<
  * 
  *     return i
  */
-            __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L7_error)
+            __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_1);
             __pyx_t_1 = 0;
 
-            /* "mapper.pyx":24
+            /* "mapper.pyx":25
  *     with open(file_name) as f:
  *         #data = f.read()
  *         for line in f:             # <<<<<<<<<<<<<<
  *             i += 1
  * 
  */
           }
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "mapper.pyx":22
+          /* "mapper.pyx":23
  * cpdef count_lines_in_fasta(file_name):
  *     i = 0
  *     with open(file_name) as f:             # <<<<<<<<<<<<<<
  *         #data = f.read()
  *         for line in f:
  */
         }
@@ -3425,36 +3385,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("mapper.count_lines_in_fasta", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_1, &__pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_1, &__pyx_t_3) < 0) __PYX_ERR(0, 23, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 23, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 22, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 23, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_11);
           __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (__pyx_t_12 < 0) __PYX_ERR(0, 22, __pyx_L9_except_error)
+          if (__pyx_t_12 < 0) __PYX_ERR(0, 23, __pyx_L9_except_error)
           __pyx_t_13 = ((!(__pyx_t_12 != 0)) != 0);
           if (__pyx_t_13) {
             __Pyx_GIVEREF(__pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_XGIVEREF(__pyx_t_3);
             __Pyx_ErrRestoreWithState(__pyx_t_4, __pyx_t_1, __pyx_t_3);
             __pyx_t_4 = 0; __pyx_t_1 = 0; __pyx_t_3 = 0; 
-            __PYX_ERR(0, 22, __pyx_L9_except_error)
+            __PYX_ERR(0, 23, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -3472,42 +3432,42 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_2) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple_, NULL);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 22, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 23, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L18;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L1_error;
     __pyx_L18:;
   }
 
-  /* "mapper.pyx":27
+  /* "mapper.pyx":28
  *             i += 1
  * 
  *     return i             # <<<<<<<<<<<<<<
  * 
  * #@cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_i);
   __pyx_r = __pyx_v_i;
   goto __pyx_L0;
 
-  /* "mapper.pyx":20
+  /* "mapper.pyx":21
  * 
  * 
  * cpdef count_lines_in_fasta(file_name):             # <<<<<<<<<<<<<<
  *     i = 0
  *     with open(file_name) as f:
  */
 
@@ -3546,15 +3506,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("count_lines_in_fasta", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6mapper_count_lines_in_fasta(__pyx_v_file_name, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6mapper_count_lines_in_fasta(__pyx_v_file_name, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3563,15 +3523,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mapper.pyx":31
+/* "mapper.pyx":32
  * #@cython.boundscheck(False)
  * #@cython.wraparound(False)
  * cdef void read_sequence_to_kmer_hashes(char* sequence, np.uint64_t[:] read_array, np.uint64_t[:] reverse_complement_read_array,             # <<<<<<<<<<<<<<
  *                                        int sequence_length):
  *     #cdef sequence_length = len(sequence) - 3  # last two bytes are \n
  */
 
@@ -3586,668 +3546,331 @@
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_sequence_to_kmer_hashes", 0);
 
-  /* "mapper.pyx":34
+  /* "mapper.pyx":35
  *                                        int sequence_length):
  *     #cdef sequence_length = len(sequence) - 3  # last two bytes are \n
  *     cdef int i = 0             # <<<<<<<<<<<<<<
  *     cdef int i_reverse_complement = sequence_length
  *     cdef int base
  */
   __pyx_v_i = 0;
 
-  /* "mapper.pyx":35
+  /* "mapper.pyx":36
  *     #cdef sequence_length = len(sequence) - 3  # last two bytes are \n
  *     cdef int i = 0
  *     cdef int i_reverse_complement = sequence_length             # <<<<<<<<<<<<<<
  *     cdef int base
  *     for i in range(0, sequence_length):
  */
   __pyx_v_i_reverse_complement = __pyx_v_sequence_length;
 
-  /* "mapper.pyx":37
+  /* "mapper.pyx":38
  *     cdef int i_reverse_complement = sequence_length
  *     cdef int base
  *     for i in range(0, sequence_length):             # <<<<<<<<<<<<<<
  *         base = sequence[i]
  *         if base == 97 or base == 65:
  */
   __pyx_t_1 = __pyx_v_sequence_length;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "mapper.pyx":38
+    /* "mapper.pyx":39
  *     cdef int base
  *     for i in range(0, sequence_length):
  *         base = sequence[i]             # <<<<<<<<<<<<<<
  *         if base == 97 or base == 65:
  *             read_array[i] = 0
  */
     __pyx_v_base = (__pyx_v_sequence[__pyx_v_i]);
 
-    /* "mapper.pyx":39
+    /* "mapper.pyx":40
  *     for i in range(0, sequence_length):
  *         base = sequence[i]
  *         if base == 97 or base == 65:             # <<<<<<<<<<<<<<
  *             read_array[i] = 0
  *             reverse_complement_read_array[i_reverse_complement] = 2
  */
     switch (__pyx_v_base) {
       case 97:
       case 65:
 
-      /* "mapper.pyx":40
+      /* "mapper.pyx":41
  *         base = sequence[i]
  *         if base == 97 or base == 65:
  *             read_array[i] = 0             # <<<<<<<<<<<<<<
  *             reverse_complement_read_array[i_reverse_complement] = 2
  *         elif base == 99 or base == 67:
  */
       __pyx_t_4 = __pyx_v_i;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 40, __pyx_L1_error)
+        __PYX_ERR(0, 41, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_read_array.data + __pyx_t_4 * __pyx_v_read_array.strides[0]) )) = 0;
 
-      /* "mapper.pyx":41
+      /* "mapper.pyx":42
  *         if base == 97 or base == 65:
  *             read_array[i] = 0
  *             reverse_complement_read_array[i_reverse_complement] = 2             # <<<<<<<<<<<<<<
  *         elif base == 99 or base == 67:
  *             read_array[i] = 1
  */
       __pyx_t_4 = __pyx_v_i_reverse_complement;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_reverse_complement_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_reverse_complement_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 41, __pyx_L1_error)
+        __PYX_ERR(0, 42, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_reverse_complement_read_array.data + __pyx_t_4 * __pyx_v_reverse_complement_read_array.strides[0]) )) = 2;
 
-      /* "mapper.pyx":39
+      /* "mapper.pyx":40
  *     for i in range(0, sequence_length):
  *         base = sequence[i]
  *         if base == 97 or base == 65:             # <<<<<<<<<<<<<<
  *             read_array[i] = 0
  *             reverse_complement_read_array[i_reverse_complement] = 2
  */
       break;
       case 99:
 
-      /* "mapper.pyx":42
+      /* "mapper.pyx":43
  *             read_array[i] = 0
  *             reverse_complement_read_array[i_reverse_complement] = 2
  *         elif base == 99 or base == 67:             # <<<<<<<<<<<<<<
  *             read_array[i] = 1
  *             reverse_complement_read_array[i_reverse_complement] = 3
  */
       case 67:
 
-      /* "mapper.pyx":43
+      /* "mapper.pyx":44
  *             reverse_complement_read_array[i_reverse_complement] = 2
  *         elif base == 99 or base == 67:
  *             read_array[i] = 1             # <<<<<<<<<<<<<<
  *             reverse_complement_read_array[i_reverse_complement] = 3
  *         elif base == 116 or base == 84:
  */
       __pyx_t_4 = __pyx_v_i;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 43, __pyx_L1_error)
+        __PYX_ERR(0, 44, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_read_array.data + __pyx_t_4 * __pyx_v_read_array.strides[0]) )) = 1;
 
-      /* "mapper.pyx":44
+      /* "mapper.pyx":45
  *         elif base == 99 or base == 67:
  *             read_array[i] = 1
  *             reverse_complement_read_array[i_reverse_complement] = 3             # <<<<<<<<<<<<<<
  *         elif base == 116 or base == 84:
  *             read_array[i] = 2
  */
       __pyx_t_4 = __pyx_v_i_reverse_complement;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_reverse_complement_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_reverse_complement_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 44, __pyx_L1_error)
+        __PYX_ERR(0, 45, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_reverse_complement_read_array.data + __pyx_t_4 * __pyx_v_reverse_complement_read_array.strides[0]) )) = 3;
 
-      /* "mapper.pyx":42
+      /* "mapper.pyx":43
  *             read_array[i] = 0
  *             reverse_complement_read_array[i_reverse_complement] = 2
  *         elif base == 99 or base == 67:             # <<<<<<<<<<<<<<
  *             read_array[i] = 1
  *             reverse_complement_read_array[i_reverse_complement] = 3
  */
       break;
       case 0x74:
 
-      /* "mapper.pyx":45
+      /* "mapper.pyx":46
  *             read_array[i] = 1
  *             reverse_complement_read_array[i_reverse_complement] = 3
  *         elif base == 116 or base == 84:             # <<<<<<<<<<<<<<
  *             read_array[i] = 2
  *             reverse_complement_read_array[i_reverse_complement] = 0
  */
       case 84:
 
-      /* "mapper.pyx":46
+      /* "mapper.pyx":47
  *             reverse_complement_read_array[i_reverse_complement] = 3
  *         elif base == 116 or base == 84:
  *             read_array[i] = 2             # <<<<<<<<<<<<<<
  *             reverse_complement_read_array[i_reverse_complement] = 0
  *         elif base == 103 or base == 71:
  */
       __pyx_t_4 = __pyx_v_i;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 46, __pyx_L1_error)
+        __PYX_ERR(0, 47, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_read_array.data + __pyx_t_4 * __pyx_v_read_array.strides[0]) )) = 2;
 
-      /* "mapper.pyx":47
+      /* "mapper.pyx":48
  *         elif base == 116 or base == 84:
  *             read_array[i] = 2
  *             reverse_complement_read_array[i_reverse_complement] = 0             # <<<<<<<<<<<<<<
  *         elif base == 103 or base == 71:
  *             read_array[i] = 3
  */
       __pyx_t_4 = __pyx_v_i_reverse_complement;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_reverse_complement_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_reverse_complement_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 47, __pyx_L1_error)
+        __PYX_ERR(0, 48, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_reverse_complement_read_array.data + __pyx_t_4 * __pyx_v_reverse_complement_read_array.strides[0]) )) = 0;
 
-      /* "mapper.pyx":45
+      /* "mapper.pyx":46
  *             read_array[i] = 1
  *             reverse_complement_read_array[i_reverse_complement] = 3
  *         elif base == 116 or base == 84:             # <<<<<<<<<<<<<<
  *             read_array[i] = 2
  *             reverse_complement_read_array[i_reverse_complement] = 0
  */
       break;
       case 0x67:
 
-      /* "mapper.pyx":48
+      /* "mapper.pyx":49
  *             read_array[i] = 2
  *             reverse_complement_read_array[i_reverse_complement] = 0
  *         elif base == 103 or base == 71:             # <<<<<<<<<<<<<<
  *             read_array[i] = 3
  *             reverse_complement_read_array[i_reverse_complement] = 1
  */
       case 71:
 
-      /* "mapper.pyx":49
+      /* "mapper.pyx":50
  *             reverse_complement_read_array[i_reverse_complement] = 0
  *         elif base == 103 or base == 71:
  *             read_array[i] = 3             # <<<<<<<<<<<<<<
  *             reverse_complement_read_array[i_reverse_complement] = 1
  *         else:
  */
       __pyx_t_4 = __pyx_v_i;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 49, __pyx_L1_error)
+        __PYX_ERR(0, 50, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_read_array.data + __pyx_t_4 * __pyx_v_read_array.strides[0]) )) = 3;
 
-      /* "mapper.pyx":50
+      /* "mapper.pyx":51
  *         elif base == 103 or base == 71:
  *             read_array[i] = 3
  *             reverse_complement_read_array[i_reverse_complement] = 1             # <<<<<<<<<<<<<<
  *         else:
  *             # invalid characters, like N, just keep these 0
  */
       __pyx_t_4 = __pyx_v_i_reverse_complement;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_reverse_complement_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_reverse_complement_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 50, __pyx_L1_error)
+        __PYX_ERR(0, 51, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_reverse_complement_read_array.data + __pyx_t_4 * __pyx_v_reverse_complement_read_array.strides[0]) )) = 1;
 
-      /* "mapper.pyx":48
+      /* "mapper.pyx":49
  *             read_array[i] = 2
  *             reverse_complement_read_array[i_reverse_complement] = 0
  *         elif base == 103 or base == 71:             # <<<<<<<<<<<<<<
  *             read_array[i] = 3
  *             reverse_complement_read_array[i_reverse_complement] = 1
  */
       break;
       default:
 
-      /* "mapper.pyx":53
+      /* "mapper.pyx":54
  *         else:
  *             # invalid characters, like N, just keep these 0
  *             read_array[i] = 0             # <<<<<<<<<<<<<<
  *         i_reverse_complement -= 1
  * 
  */
       __pyx_t_4 = __pyx_v_i;
       __pyx_t_5 = -1;
       if (__pyx_t_4 < 0) {
         __pyx_t_4 += __pyx_v_read_array.shape[0];
         if (unlikely(__pyx_t_4 < 0)) __pyx_t_5 = 0;
       } else if (unlikely(__pyx_t_4 >= __pyx_v_read_array.shape[0])) __pyx_t_5 = 0;
       if (unlikely(__pyx_t_5 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_5);
-        __PYX_ERR(0, 53, __pyx_L1_error)
+        __PYX_ERR(0, 54, __pyx_L1_error)
       }
       *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_read_array.data + __pyx_t_4 * __pyx_v_read_array.strides[0]) )) = 0;
       break;
     }
 
-    /* "mapper.pyx":54
+    /* "mapper.pyx":55
  *             # invalid characters, like N, just keep these 0
  *             read_array[i] = 0
  *         i_reverse_complement -= 1             # <<<<<<<<<<<<<<
  * 
- * def read_fasta(filename):
+ * 
  */
     __pyx_v_i_reverse_complement = (__pyx_v_i_reverse_complement - 1);
   }
 
-  /* "mapper.pyx":31
+  /* "mapper.pyx":32
  * #@cython.boundscheck(False)
  * #@cython.wraparound(False)
  * cdef void read_sequence_to_kmer_hashes(char* sequence, np.uint64_t[:] read_array, np.uint64_t[:] reverse_complement_read_array,             # <<<<<<<<<<<<<<
  *                                        int sequence_length):
  *     #cdef sequence_length = len(sequence) - 3  # last two bytes are \n
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("mapper.read_sequence_to_kmer_hashes", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
-static PyObject *__pyx_gb_6mapper_8generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
-
-/* "mapper.pyx":56
- *         i_reverse_complement -= 1
- * 
- * def read_fasta(filename):             # <<<<<<<<<<<<<<
- *     filename_byte_string = filename.encode("UTF-8")
- *     cdef char * fname = filename_byte_string
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_6mapper_7read_fasta(PyObject *__pyx_self, PyObject *__pyx_v_filename); /*proto*/
-static PyMethodDef __pyx_mdef_6mapper_7read_fasta = {"read_fasta", (PyCFunction)__pyx_pw_6mapper_7read_fasta, METH_O, 0};
-static PyObject *__pyx_pw_6mapper_7read_fasta(PyObject *__pyx_self, PyObject *__pyx_v_filename) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("read_fasta (wrapper)", 0);
-  __pyx_r = __pyx_pf_6mapper_6read_fasta(__pyx_self, ((PyObject *)__pyx_v_filename));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_6mapper_6read_fasta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename) {
-  struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *__pyx_cur_scope;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("read_fasta", 0);
-  __pyx_cur_scope = (struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *)__pyx_tp_new_6mapper___pyx_scope_struct__read_fasta(__pyx_ptype_6mapper___pyx_scope_struct__read_fasta, __pyx_empty_tuple, NULL);
-  if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *)Py_None);
-    __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 56, __pyx_L1_error)
-  } else {
-    __Pyx_GOTREF(__pyx_cur_scope);
-  }
-  __pyx_cur_scope->__pyx_v_filename = __pyx_v_filename;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_filename);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_filename);
-  {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6mapper_8generator, __pyx_codeobj__3, (PyObject *) __pyx_cur_scope, __pyx_n_s_read_fasta, __pyx_n_s_read_fasta, __pyx_n_s_mapper); if (unlikely(!gen)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_cur_scope);
-    __Pyx_RefNannyFinishContext();
-    return (PyObject *) gen;
-  }
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("mapper.read_fasta", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_gb_6mapper_8generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
-{
-  struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *__pyx_cur_scope = ((struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *)__pyx_generator->closure);
-  PyObject *__pyx_r = NULL;
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  char *__pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("read_fasta", 0);
-  switch (__pyx_generator->resume_label) {
-    case 0: goto __pyx_L3_first_run;
-    case 1: goto __pyx_L9_resume_from_yield;
-    default: /* CPython raises the right error here */
-    __Pyx_RefNannyFinishContext();
-    return NULL;
-  }
-  __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 56, __pyx_L1_error)
-
-  /* "mapper.pyx":57
- * 
- * def read_fasta(filename):
- *     filename_byte_string = filename.encode("UTF-8")             # <<<<<<<<<<<<<<
- *     cdef char * fname = filename_byte_string
- * 
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_UTF_8);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GIVEREF(__pyx_t_1);
-  __pyx_cur_scope->__pyx_v_filename_byte_string = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "mapper.pyx":58
- * def read_fasta(filename):
- *     filename_byte_string = filename.encode("UTF-8")
- *     cdef char * fname = filename_byte_string             # <<<<<<<<<<<<<<
- * 
- *     cdef FILE * cfile
- */
-  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_cur_scope->__pyx_v_filename_byte_string); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
-  __pyx_cur_scope->__pyx_v_fname = __pyx_t_4;
-
-  /* "mapper.pyx":61
- * 
- *     cdef FILE * cfile
- *     cfile = fopen(fname, "rb")             # <<<<<<<<<<<<<<
- *     if cfile == NULL:
- *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
- */
-  __pyx_cur_scope->__pyx_v_cfile = fopen(__pyx_cur_scope->__pyx_v_fname, ((char const *)"rb"));
-
-  /* "mapper.pyx":62
- *     cdef FILE * cfile
- *     cfile = fopen(fname, "rb")
- *     if cfile == NULL:             # <<<<<<<<<<<<<<
- *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
- * 
- */
-  __pyx_t_5 = ((__pyx_cur_scope->__pyx_v_cfile == NULL) != 0);
-  if (unlikely(__pyx_t_5)) {
-
-    /* "mapper.pyx":63
- *     cfile = fopen(fname, "rb")
- *     if cfile == NULL:
- *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)             # <<<<<<<<<<<<<<
- * 
- *     cdef char * line = NULL
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FileNotFoundError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_No_such_file_or_directory_s, __pyx_cur_scope->__pyx_v_filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_INCREF(__pyx_int_2);
-    __Pyx_GIVEREF(__pyx_int_2);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_int_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 63, __pyx_L1_error)
-
-    /* "mapper.pyx":62
- *     cdef FILE * cfile
- *     cfile = fopen(fname, "rb")
- *     if cfile == NULL:             # <<<<<<<<<<<<<<
- *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
- * 
- */
-  }
-
-  /* "mapper.pyx":65
- *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
- * 
- *     cdef char * line = NULL             # <<<<<<<<<<<<<<
- *     cdef size_t l = 0
- *     cdef ssize_t read
- */
-  __pyx_cur_scope->__pyx_v_line = NULL;
-
-  /* "mapper.pyx":66
- * 
- *     cdef char * line = NULL
- *     cdef size_t l = 0             # <<<<<<<<<<<<<<
- *     cdef ssize_t read
- *     cdef i = 0
- */
-  __pyx_cur_scope->__pyx_v_l = 0;
-
-  /* "mapper.pyx":68
- *     cdef size_t l = 0
- *     cdef ssize_t read
- *     cdef i = 0             # <<<<<<<<<<<<<<
- *     while True:
- *         i += 1
- */
-  __Pyx_INCREF(__pyx_int_0);
-  __Pyx_GIVEREF(__pyx_int_0);
-  __pyx_cur_scope->__pyx_v_i = __pyx_int_0;
-
-  /* "mapper.pyx":69
- *     cdef ssize_t read
- *     cdef i = 0
- *     while True:             # <<<<<<<<<<<<<<
- *         i += 1
- *         read = getline(&line, &l, cfile)
- */
-  while (1) {
-
-    /* "mapper.pyx":70
- *     cdef i = 0
- *     while True:
- *         i += 1             # <<<<<<<<<<<<<<
- *         read = getline(&line, &l, cfile)
- *         if read == -1: break
- */
-    __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_cur_scope->__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_i);
-    __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_i, __pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    __pyx_t_2 = 0;
-
-    /* "mapper.pyx":71
- *     while True:
- *         i += 1
- *         read = getline(&line, &l, cfile)             # <<<<<<<<<<<<<<
- *         if read == -1: break
- * 
- */
-    __pyx_cur_scope->__pyx_v_read = getline((&__pyx_cur_scope->__pyx_v_line), (&__pyx_cur_scope->__pyx_v_l), __pyx_cur_scope->__pyx_v_cfile);
-
-    /* "mapper.pyx":72
- *         i += 1
- *         read = getline(&line, &l, cfile)
- *         if read == -1: break             # <<<<<<<<<<<<<<
- * 
- *         # skip header lines
- */
-    __pyx_t_5 = ((__pyx_cur_scope->__pyx_v_read == -1L) != 0);
-    if (__pyx_t_5) {
-      goto __pyx_L6_break;
-    }
-
-    /* "mapper.pyx":75
- * 
- *         # skip header lines
- *         if line[0] == 62:             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-    __pyx_t_5 = (((__pyx_cur_scope->__pyx_v_line[0]) == 62) != 0);
-    if (__pyx_t_5) {
-
-      /* "mapper.pyx":76
- *         # skip header lines
- *         if line[0] == 62:
- *             continue             # <<<<<<<<<<<<<<
- * 
- *         yield line
- */
-      goto __pyx_L5_continue;
-
-      /* "mapper.pyx":75
- * 
- *         # skip header lines
- *         if line[0] == 62:             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-    }
 
-    /* "mapper.pyx":78
- *             continue
- * 
- *         yield line             # <<<<<<<<<<<<<<
- * 
- *     fclose(cfile)
- */
-    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_line); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
-    __Pyx_XGIVEREF(__pyx_r);
-    __Pyx_RefNannyFinishContext();
-    __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
-    /* return from generator, yielding value */
-    __pyx_generator->resume_label = 1;
-    return __pyx_r;
-    __pyx_L9_resume_from_yield:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 78, __pyx_L1_error)
-    __pyx_L5_continue:;
-  }
-  __pyx_L6_break:;
-
-  /* "mapper.pyx":80
- *         yield line
- * 
- *     fclose(cfile)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  (void)(fclose(__pyx_cur_scope->__pyx_v_cfile));
-  CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
-
-  /* "mapper.pyx":56
- *         i_reverse_complement -= 1
- * 
- * def read_fasta(filename):             # <<<<<<<<<<<<<<
- *     filename_byte_string = filename.encode("UTF-8")
- *     cdef char * fname = filename_byte_string
- */
-
-  /* function exit code */
-  PyErr_SetNone(PyExc_StopIteration);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("read_fasta", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
-  #if !CYTHON_USE_EXC_INFO_STACK
-  __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
-  #endif
-  __pyx_generator->resume_label = -1;
-  __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "mapper.pyx":83
+/* "mapper.pyx":58
  * 
  * 
  * cdef void process_line(char* sequence, np.uint64_t[:] chunk_row, np.uint8_t[:] mask_row):             # <<<<<<<<<<<<<<
  *     cdef i = 0
  *     for i in range(0, len(sequence)-1):
  */
 
@@ -4264,140 +3887,140 @@
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("process_line", 0);
 
-  /* "mapper.pyx":84
+  /* "mapper.pyx":59
  * 
  * cdef void process_line(char* sequence, np.uint64_t[:] chunk_row, np.uint8_t[:] mask_row):
  *     cdef i = 0             # <<<<<<<<<<<<<<
  *     for i in range(0, len(sequence)-1):
  *         chunk_row[i] = sequence[i]
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_i = __pyx_int_0;
 
-  /* "mapper.pyx":85
+  /* "mapper.pyx":60
  * cdef void process_line(char* sequence, np.uint64_t[:] chunk_row, np.uint8_t[:] mask_row):
  *     cdef i = 0
  *     for i in range(0, len(sequence)-1):             # <<<<<<<<<<<<<<
  *         chunk_row[i] = sequence[i]
  *         mask_row[i] = True
  */
   __pyx_t_1 = strlen(__pyx_v_sequence); 
-  __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_1 - 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_1 - 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_int_0);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
     __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 60, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 60, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_5(__pyx_t_3);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 85, __pyx_L1_error)
+          else __PYX_ERR(0, 60, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "mapper.pyx":86
+    /* "mapper.pyx":61
  *     cdef i = 0
  *     for i in range(0, len(sequence)-1):
  *         chunk_row[i] = sequence[i]             # <<<<<<<<<<<<<<
  *         mask_row[i] = True
  * 
  */
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L1_error)
     __pyx_t_8 = __pyx_t_7;
     __pyx_t_9 = -1;
     if (__pyx_t_8 < 0) {
       __pyx_t_8 += __pyx_v_chunk_row.shape[0];
       if (unlikely(__pyx_t_8 < 0)) __pyx_t_9 = 0;
     } else if (unlikely(__pyx_t_8 >= __pyx_v_chunk_row.shape[0])) __pyx_t_9 = 0;
     if (unlikely(__pyx_t_9 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_9);
-      __PYX_ERR(0, 86, __pyx_L1_error)
+      __PYX_ERR(0, 61, __pyx_L1_error)
     }
     *((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_chunk_row.data + __pyx_t_8 * __pyx_v_chunk_row.strides[0]) )) = (__pyx_v_sequence[__pyx_t_6]);
 
-    /* "mapper.pyx":87
+    /* "mapper.pyx":62
  *     for i in range(0, len(sequence)-1):
  *         chunk_row[i] = sequence[i]
  *         mask_row[i] = True             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L1_error)
     __pyx_t_8 = __pyx_t_6;
     __pyx_t_9 = -1;
     if (__pyx_t_8 < 0) {
       __pyx_t_8 += __pyx_v_mask_row.shape[0];
       if (unlikely(__pyx_t_8 < 0)) __pyx_t_9 = 0;
     } else if (unlikely(__pyx_t_8 >= __pyx_v_mask_row.shape[0])) __pyx_t_9 = 0;
     if (unlikely(__pyx_t_9 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_9);
-      __PYX_ERR(0, 87, __pyx_L1_error)
+      __PYX_ERR(0, 62, __pyx_L1_error)
     }
     *((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ (__pyx_v_mask_row.data + __pyx_t_8 * __pyx_v_mask_row.strides[0]) )) = 1;
 
-    /* "mapper.pyx":85
+    /* "mapper.pyx":60
  * cdef void process_line(char* sequence, np.uint64_t[:] chunk_row, np.uint8_t[:] mask_row):
  *     cdef i = 0
  *     for i in range(0, len(sequence)-1):             # <<<<<<<<<<<<<<
  *         chunk_row[i] = sequence[i]
  *         mask_row[i] = True
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "mapper.pyx":83
+  /* "mapper.pyx":58
  * 
  * 
  * cdef void process_line(char* sequence, np.uint64_t[:] chunk_row, np.uint8_t[:] mask_row):             # <<<<<<<<<<<<<<
  *     cdef i = 0
  *     for i in range(0, len(sequence)-1):
  */
 
@@ -4407,28 +4030,28 @@
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_WriteUnraisable("mapper.process_line", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_RefNannyFinishContext();
 }
-static PyObject *__pyx_gb_6mapper_11generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_6mapper_8generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "mapper.pyx":90
+/* "mapper.pyx":65
  * 
  * 
  * def read_fasta_into_chunks(filename, chunk_size=1000, int max_read_length=150, write_to_shared_memory=False, process_reads=False):             # <<<<<<<<<<<<<<
  *     logging.info("Reading fasta %s" % filename)
  *     filename_byte_string = filename.encode("UTF-8")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6mapper_10read_fasta_into_chunks(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_6mapper_10read_fasta_into_chunks = {"read_fasta_into_chunks", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6mapper_10read_fasta_into_chunks, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_6mapper_10read_fasta_into_chunks(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6mapper_7read_fasta_into_chunks(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_6mapper_7read_fasta_into_chunks = {"read_fasta_into_chunks", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6mapper_7read_fasta_into_chunks, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_6mapper_7read_fasta_into_chunks(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_chunk_size = 0;
   int __pyx_v_max_read_length;
   PyObject *__pyx_v_write_to_shared_memory = 0;
   PyObject *__pyx_v_process_reads = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -4486,15 +4109,15 @@
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_process_reads);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_fasta_into_chunks") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_fasta_into_chunks") < 0)) __PYX_ERR(0, 65, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -4506,49 +4129,49 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_filename = values[0];
     __pyx_v_chunk_size = values[1];
     if (values[2]) {
-      __pyx_v_max_read_length = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_max_read_length == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
+      __pyx_v_max_read_length = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_max_read_length == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
     } else {
       __pyx_v_max_read_length = ((int)0x96);
     }
     __pyx_v_write_to_shared_memory = values[3];
     __pyx_v_process_reads = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_fasta_into_chunks", 0, 1, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_fasta_into_chunks", 0, 1, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 65, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("mapper.read_fasta_into_chunks", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6mapper_9read_fasta_into_chunks(__pyx_self, __pyx_v_filename, __pyx_v_chunk_size, __pyx_v_max_read_length, __pyx_v_write_to_shared_memory, __pyx_v_process_reads);
+  __pyx_r = __pyx_pf_6mapper_6read_fasta_into_chunks(__pyx_self, __pyx_v_filename, __pyx_v_chunk_size, __pyx_v_max_read_length, __pyx_v_write_to_shared_memory, __pyx_v_process_reads);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6mapper_9read_fasta_into_chunks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_chunk_size, int __pyx_v_max_read_length, PyObject *__pyx_v_write_to_shared_memory, PyObject *__pyx_v_process_reads) {
-  struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *__pyx_cur_scope;
+static PyObject *__pyx_pf_6mapper_6read_fasta_into_chunks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_chunk_size, int __pyx_v_max_read_length, PyObject *__pyx_v_write_to_shared_memory, PyObject *__pyx_v_process_reads) {
+  struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_fasta_into_chunks", 0);
-  __pyx_cur_scope = (struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *)__pyx_tp_new_6mapper___pyx_scope_struct_1_read_fasta_into_chunks(__pyx_ptype_6mapper___pyx_scope_struct_1_read_fasta_into_chunks, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *)__pyx_tp_new_6mapper___pyx_scope_struct__read_fasta_into_chunks(__pyx_ptype_6mapper___pyx_scope_struct__read_fasta_into_chunks, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 90, __pyx_L1_error)
+    __PYX_ERR(0, 65, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_filename = __pyx_v_filename;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_filename);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_filename);
   __pyx_cur_scope->__pyx_v_chunk_size = __pyx_v_chunk_size;
@@ -4558,15 +4181,15 @@
   __pyx_cur_scope->__pyx_v_write_to_shared_memory = __pyx_v_write_to_shared_memory;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_write_to_shared_memory);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_write_to_shared_memory);
   __pyx_cur_scope->__pyx_v_process_reads = __pyx_v_process_reads;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_process_reads);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_process_reads);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6mapper_11generator1, __pyx_codeobj__4, (PyObject *) __pyx_cur_scope, __pyx_n_s_read_fasta_into_chunks, __pyx_n_s_read_fasta_into_chunks, __pyx_n_s_mapper); if (unlikely(!gen)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6mapper_8generator, __pyx_codeobj__3, (PyObject *) __pyx_cur_scope, __pyx_n_s_read_fasta_into_chunks, __pyx_n_s_read_fasta_into_chunks, __pyx_n_s_mapper); if (unlikely(!gen)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4574,17 +4197,17 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_6mapper_11generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_6mapper_8generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
-  struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *__pyx_cur_scope = ((struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *)__pyx_generator->closure);
+  struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *__pyx_cur_scope = ((struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char *__pyx_t_5;
   int __pyx_t_6;
@@ -4606,787 +4229,787 @@
     case 3: goto __pyx_L18_resume_from_yield;
     case 4: goto __pyx_L19_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 65, __pyx_L1_error)
 
-  /* "mapper.pyx":91
+  /* "mapper.pyx":66
  * 
  * def read_fasta_into_chunks(filename, chunk_size=1000, int max_read_length=150, write_to_shared_memory=False, process_reads=False):
  *     logging.info("Reading fasta %s" % filename)             # <<<<<<<<<<<<<<
  *     filename_byte_string = filename.encode("UTF-8")
  *     cdef char * fname = filename_byte_string
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Reading_fasta_s, __pyx_cur_scope->__pyx_v_filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Reading_fasta_s, __pyx_cur_scope->__pyx_v_filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mapper.pyx":92
+  /* "mapper.pyx":67
  * def read_fasta_into_chunks(filename, chunk_size=1000, int max_read_length=150, write_to_shared_memory=False, process_reads=False):
  *     logging.info("Reading fasta %s" % filename)
  *     filename_byte_string = filename.encode("UTF-8")             # <<<<<<<<<<<<<<
  *     cdef char * fname = filename_byte_string
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_UTF_8);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_filename_byte_string = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "mapper.pyx":93
+  /* "mapper.pyx":68
  *     logging.info("Reading fasta %s" % filename)
  *     filename_byte_string = filename.encode("UTF-8")
  *     cdef char * fname = filename_byte_string             # <<<<<<<<<<<<<<
  * 
  *     cdef FILE * cfile
  */
-  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_cur_scope->__pyx_v_filename_byte_string); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_cur_scope->__pyx_v_filename_byte_string); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L1_error)
   __pyx_cur_scope->__pyx_v_fname = __pyx_t_5;
 
-  /* "mapper.pyx":96
+  /* "mapper.pyx":71
  * 
  *     cdef FILE * cfile
  *     cfile = fopen(fname, "rb")             # <<<<<<<<<<<<<<
  *     if cfile == NULL:
  *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
  */
   __pyx_cur_scope->__pyx_v_cfile = fopen(__pyx_cur_scope->__pyx_v_fname, ((char const *)"rb"));
 
-  /* "mapper.pyx":97
+  /* "mapper.pyx":72
  *     cdef FILE * cfile
  *     cfile = fopen(fname, "rb")
  *     if cfile == NULL:             # <<<<<<<<<<<<<<
  *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
  * 
  */
   __pyx_t_6 = ((__pyx_cur_scope->__pyx_v_cfile == NULL) != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "mapper.pyx":98
+    /* "mapper.pyx":73
  *     cfile = fopen(fname, "rb")
  *     if cfile == NULL:
  *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)             # <<<<<<<<<<<<<<
  * 
  *     cdef char * line = NULL
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FileNotFoundError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FileNotFoundError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_No_such_file_or_directory_s, __pyx_cur_scope->__pyx_v_filename); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_No_such_file_or_directory_s, __pyx_cur_scope->__pyx_v_filename); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_int_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 98, __pyx_L1_error)
+    __PYX_ERR(0, 73, __pyx_L1_error)
 
-    /* "mapper.pyx":97
+    /* "mapper.pyx":72
  *     cdef FILE * cfile
  *     cfile = fopen(fname, "rb")
  *     if cfile == NULL:             # <<<<<<<<<<<<<<
  *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
  * 
  */
   }
 
-  /* "mapper.pyx":100
+  /* "mapper.pyx":75
  *         raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
  * 
  *     cdef char * line = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t l = 0
  *     cdef ssize_t read
  */
   __pyx_cur_scope->__pyx_v_line = NULL;
 
-  /* "mapper.pyx":101
+  /* "mapper.pyx":76
  * 
  *     cdef char * line = NULL
  *     cdef size_t l = 0             # <<<<<<<<<<<<<<
  *     cdef ssize_t read
  *     cdef i = 0
  */
   __pyx_cur_scope->__pyx_v_l = 0;
 
-  /* "mapper.pyx":103
+  /* "mapper.pyx":78
  *     cdef size_t l = 0
  *     cdef ssize_t read
  *     cdef i = 0             # <<<<<<<<<<<<<<
  *     cdef int line_length = 0
  * 
  */
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   __pyx_cur_scope->__pyx_v_i = __pyx_int_0;
 
-  /* "mapper.pyx":104
+  /* "mapper.pyx":79
  *     cdef ssize_t read
  *     cdef i = 0
  *     cdef int line_length = 0             # <<<<<<<<<<<<<<
  * 
  *     if process_reads:
  */
   __pyx_cur_scope->__pyx_v_line_length = 0;
 
-  /* "mapper.pyx":106
+  /* "mapper.pyx":81
  *     cdef int line_length = 0
  * 
  *     if process_reads:             # <<<<<<<<<<<<<<
  *         chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
  *     else:
  */
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_process_reads); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_process_reads); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 81, __pyx_L1_error)
   if (__pyx_t_6) {
 
-    /* "mapper.pyx":107
+    /* "mapper.pyx":82
  * 
  *     if process_reads:
  *         chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     else:
- *         #chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
+ *         chunk = np.empty(chunk_size, dtype="|S" + str(max_read_length))  # max_read_length bytes for each element
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_chunk_size);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_chunk_size);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_v_chunk_size);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GIVEREF(__pyx_t_7);
     __pyx_cur_scope->__pyx_v_chunk = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "mapper.pyx":106
+    /* "mapper.pyx":81
  *     cdef int line_length = 0
  * 
  *     if process_reads:             # <<<<<<<<<<<<<<
  *         chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
  *     else:
  */
     goto __pyx_L5;
   }
 
-  /* "mapper.pyx":110
+  /* "mapper.pyx":84
+ *         chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
  *     else:
- *         #chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
  *         chunk = np.empty(chunk_size, dtype="|S" + str(max_read_length))  # max_read_length bytes for each element             # <<<<<<<<<<<<<<
- *         #chunk = np.empty(chunk_size, dtype="<U" + str(max_read_length))
  * 
+ *     mask = np.zeros((chunk_size, max_read_length),
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_chunk_size);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_chunk_size);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_cur_scope->__pyx_v_chunk_size);
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_S, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_S, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_cur_scope->__pyx_v_chunk = __pyx_t_2;
     __pyx_t_2 = 0;
   }
   __pyx_L5:;
 
-  /* "mapper.pyx":113
- *         #chunk = np.empty(chunk_size, dtype="<U" + str(max_read_length))
+  /* "mapper.pyx":86
+ *         chunk = np.empty(chunk_size, dtype="|S" + str(max_read_length))  # max_read_length bytes for each element
  * 
  *     mask = np.zeros((chunk_size, max_read_length),             # <<<<<<<<<<<<<<
  *                         dtype=np.bool)  # True where reads have bases (for handling short reads)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_chunk_size);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_chunk_size);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_cur_scope->__pyx_v_chunk_size);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "mapper.pyx":114
+  /* "mapper.pyx":87
  * 
  *     mask = np.zeros((chunk_size, max_read_length),
  *                         dtype=np.bool)  # True where reads have bases (for handling short reads)             # <<<<<<<<<<<<<<
  * 
  *     prev_time = time.time()
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_bool); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_bool); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "mapper.pyx":113
- *         #chunk = np.empty(chunk_size, dtype="<U" + str(max_read_length))
+  /* "mapper.pyx":86
+ *         chunk = np.empty(chunk_size, dtype="|S" + str(max_read_length))  # max_read_length bytes for each element
  * 
  *     mask = np.zeros((chunk_size, max_read_length),             # <<<<<<<<<<<<<<
  *                         dtype=np.bool)  # True where reads have bases (for handling short reads)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_cur_scope->__pyx_v_mask = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "mapper.pyx":116
+  /* "mapper.pyx":89
  *                         dtype=np.bool)  # True where reads have bases (for handling short reads)
  * 
  *     prev_time = time.time()             # <<<<<<<<<<<<<<
  * 
  *     while True:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_cur_scope->__pyx_v_prev_time = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "mapper.pyx":118
+  /* "mapper.pyx":91
  *     prev_time = time.time()
  * 
  *     while True:             # <<<<<<<<<<<<<<
  *         read = getline(&line, &l, cfile)
  *         if read == -1:
  */
   while (1) {
 
-    /* "mapper.pyx":119
+    /* "mapper.pyx":92
  * 
  *     while True:
  *         read = getline(&line, &l, cfile)             # <<<<<<<<<<<<<<
  *         if read == -1:
  *             logging.info("No more reads")
  */
     __pyx_cur_scope->__pyx_v_read = getline((&__pyx_cur_scope->__pyx_v_line), (&__pyx_cur_scope->__pyx_v_l), __pyx_cur_scope->__pyx_v_cfile);
 
-    /* "mapper.pyx":120
+    /* "mapper.pyx":93
  *     while True:
  *         read = getline(&line, &l, cfile)
  *         if read == -1:             # <<<<<<<<<<<<<<
  *             logging.info("No more reads")
  *             break
  */
     __pyx_t_6 = ((__pyx_cur_scope->__pyx_v_read == -1L) != 0);
     if (__pyx_t_6) {
 
-      /* "mapper.pyx":121
+      /* "mapper.pyx":94
  *         read = getline(&line, &l, cfile)
  *         if read == -1:
  *             logging.info("No more reads")             # <<<<<<<<<<<<<<
  *             break
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 121, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_2, __pyx_kp_u_No_more_reads) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_No_more_reads);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "mapper.pyx":122
+      /* "mapper.pyx":95
  *         if read == -1:
  *             logging.info("No more reads")
  *             break             # <<<<<<<<<<<<<<
  * 
  *         # skip header lines
  */
       goto __pyx_L7_break;
 
-      /* "mapper.pyx":120
+      /* "mapper.pyx":93
  *     while True:
  *         read = getline(&line, &l, cfile)
  *         if read == -1:             # <<<<<<<<<<<<<<
  *             logging.info("No more reads")
  *             break
  */
     }
 
-    /* "mapper.pyx":125
+    /* "mapper.pyx":98
  * 
  *         # skip header lines
  *         if line[0] == 62:             # <<<<<<<<<<<<<<
  *             continue
  * 
  */
     __pyx_t_6 = (((__pyx_cur_scope->__pyx_v_line[0]) == 62) != 0);
     if (__pyx_t_6) {
 
-      /* "mapper.pyx":126
+      /* "mapper.pyx":99
  *         # skip header lines
  *         if line[0] == 62:
  *             continue             # <<<<<<<<<<<<<<
  * 
  *         line_length = len(line)-1
  */
       goto __pyx_L6_continue;
 
-      /* "mapper.pyx":125
+      /* "mapper.pyx":98
  * 
  *         # skip header lines
  *         if line[0] == 62:             # <<<<<<<<<<<<<<
  *             continue
  * 
  */
     }
 
-    /* "mapper.pyx":128
+    /* "mapper.pyx":101
  *             continue
  * 
  *         line_length = len(line)-1             # <<<<<<<<<<<<<<
  *         #chunk[i,line_length] = line
  *         if process_reads:
  */
     __pyx_t_8 = strlen(__pyx_cur_scope->__pyx_v_line); 
     __pyx_cur_scope->__pyx_v_line_length = (__pyx_t_8 - 1);
 
-    /* "mapper.pyx":130
+    /* "mapper.pyx":103
  *         line_length = len(line)-1
  *         #chunk[i,line_length] = line
  *         if process_reads:             # <<<<<<<<<<<<<<
  *             chunk[i, 0:line_length] = np.frombuffer(line, dtype=np.uint8)[:-1]  # remove \n at end
  *             mask[i, 0:line_length] = True
  */
-    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_process_reads); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_process_reads); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 103, __pyx_L1_error)
     if (__pyx_t_6) {
 
-      /* "mapper.pyx":131
+      /* "mapper.pyx":104
  *         #chunk[i,line_length] = line
  *         if process_reads:
  *             chunk[i, 0:line_length] = np.frombuffer(line, dtype=np.uint8)[:-1]  # remove \n at end             # <<<<<<<<<<<<<<
  *             mask[i, 0:line_length] = True
  *             # a bit slower:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_line); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_line); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, -1L, NULL, NULL, &__pyx_slice__5, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, -1L, NULL, NULL, &__pyx_slice__4, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_line_length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_line_length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PySlice_New(__pyx_int_0, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_2 = PySlice_New(__pyx_int_0, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_i);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_i);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_v_i);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
       __pyx_t_2 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_cur_scope->__pyx_v_chunk, __pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 131, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_cur_scope->__pyx_v_chunk, __pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "mapper.pyx":132
+      /* "mapper.pyx":105
  *         if process_reads:
  *             chunk[i, 0:line_length] = np.frombuffer(line, dtype=np.uint8)[:-1]  # remove \n at end
  *             mask[i, 0:line_length] = True             # <<<<<<<<<<<<<<
  *             # a bit slower:
  *             #process_line(line, chunk[i,:], mask[i,:])
  */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_line_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_line_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = PySlice_New(__pyx_int_0, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+      __pyx_t_1 = PySlice_New(__pyx_int_0, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_i);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_i);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_cur_scope->__pyx_v_i);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
       __pyx_t_1 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_cur_scope->__pyx_v_mask, __pyx_t_4, Py_True) < 0)) __PYX_ERR(0, 132, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_cur_scope->__pyx_v_mask, __pyx_t_4, Py_True) < 0)) __PYX_ERR(0, 105, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "mapper.pyx":130
+      /* "mapper.pyx":103
  *         line_length = len(line)-1
  *         #chunk[i,line_length] = line
  *         if process_reads:             # <<<<<<<<<<<<<<
  *             chunk[i, 0:line_length] = np.frombuffer(line, dtype=np.uint8)[:-1]  # remove \n at end
  *             mask[i, 0:line_length] = True
  */
       goto __pyx_L10;
     }
 
-    /* "mapper.pyx":136
+    /* "mapper.pyx":109
  *             #process_line(line, chunk[i,:], mask[i,:])
  *         else:
  *             chunk[i] = line             # <<<<<<<<<<<<<<
  *             mask[i, 0:line_length] = True
  * 
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_line); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_line); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(PyObject_SetItem(__pyx_cur_scope->__pyx_v_chunk, __pyx_cur_scope->__pyx_v_i, __pyx_t_4) < 0)) __PYX_ERR(0, 136, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_cur_scope->__pyx_v_chunk, __pyx_cur_scope->__pyx_v_i, __pyx_t_4) < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "mapper.pyx":137
+      /* "mapper.pyx":110
  *         else:
  *             chunk[i] = line
  *             mask[i, 0:line_length] = True             # <<<<<<<<<<<<<<
  * 
  *         i += 1
  */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_line_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_line_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = PySlice_New(__pyx_int_0, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+      __pyx_t_1 = PySlice_New(__pyx_int_0, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_i);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_i);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_cur_scope->__pyx_v_i);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
       __pyx_t_1 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_cur_scope->__pyx_v_mask, __pyx_t_4, Py_True) < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_cur_scope->__pyx_v_mask, __pyx_t_4, Py_True) < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __pyx_L10:;
 
-    /* "mapper.pyx":139
+    /* "mapper.pyx":112
  *             mask[i, 0:line_length] = True
  * 
  *         i += 1             # <<<<<<<<<<<<<<
  *         if i >= chunk_size:
  *             if write_to_shared_memory:
  */
-    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_cur_scope->__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_cur_scope->__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_i);
     __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_i, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "mapper.pyx":140
+    /* "mapper.pyx":113
  * 
  *         i += 1
  *         if i >= chunk_size:             # <<<<<<<<<<<<<<
  *             if write_to_shared_memory:
  *                 name1 = "shared_array_" + str(np.random.random())
  */
-    __pyx_t_4 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_i, __pyx_cur_scope->__pyx_v_chunk_size, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_i, __pyx_cur_scope->__pyx_v_chunk_size, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_6) {
 
-      /* "mapper.pyx":141
+      /* "mapper.pyx":114
  *         i += 1
  *         if i >= chunk_size:
  *             if write_to_shared_memory:             # <<<<<<<<<<<<<<
  *                 name1 = "shared_array_" + str(np.random.random())
  *                 name2 = "shared_array_" + str(np.random.random())
  */
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_write_to_shared_memory); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 141, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_write_to_shared_memory); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
       if (__pyx_t_6) {
 
-        /* "mapper.pyx":142
+        /* "mapper.pyx":115
  *         if i >= chunk_size:
  *             if write_to_shared_memory:
  *                 name1 = "shared_array_" + str(np.random.random())             # <<<<<<<<<<<<<<
  *                 name2 = "shared_array_" + str(np.random.random())
  *                 logging.info("Yielding chunk with %d reads in shared memory %s" % (chunk.shape[0], name1))
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_2)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
             __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
           }
         }
         __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_n_u_shared_array, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_n_u_shared_array, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_name1);
         __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_name1, __pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_4);
         __pyx_t_4 = 0;
 
-        /* "mapper.pyx":143
+        /* "mapper.pyx":116
  *             if write_to_shared_memory:
  *                 name1 = "shared_array_" + str(np.random.random())
  *                 name2 = "shared_array_" + str(np.random.random())             # <<<<<<<<<<<<<<
  *                 logging.info("Yielding chunk with %d reads in shared memory %s" % (chunk.shape[0], name1))
  *                 to_shared_memory(SingleSharedArray(chunk), name1)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_2)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
             __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
           }
         }
         __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_n_u_shared_array, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_n_u_shared_array, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_name2);
         __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_name2, __pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_4);
         __pyx_t_4 = 0;
 
-        /* "mapper.pyx":144
+        /* "mapper.pyx":117
  *                 name1 = "shared_array_" + str(np.random.random())
  *                 name2 = "shared_array_" + str(np.random.random())
  *                 logging.info("Yielding chunk with %d reads in shared memory %s" % (chunk.shape[0], name1))             # <<<<<<<<<<<<<<
  *                 to_shared_memory(SingleSharedArray(chunk), name1)
  *                 to_shared_memory(SingleSharedArray(mask), name2)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_9 = 0;
         __pyx_t_10 = 127;
         __Pyx_INCREF(__pyx_kp_u_Yielding_chunk_with);
         __pyx_t_9 += 20;
         __Pyx_GIVEREF(__pyx_kp_u_Yielding_chunk_with);
         PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Yielding_chunk_with);
-        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_chunk, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_chunk, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_7, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_7, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_FormatAndDecref(__Pyx_PyNumber_IntOrLong(__pyx_t_3), __pyx_n_u_d); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_FormatAndDecref(__Pyx_PyNumber_IntOrLong(__pyx_t_3), __pyx_n_u_d); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_10;
         __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_7);
         __pyx_t_7 = 0;
         __Pyx_INCREF(__pyx_kp_u_reads_in_shared_memory);
         __pyx_t_9 += 24;
         __Pyx_GIVEREF(__pyx_kp_u_reads_in_shared_memory);
         PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_reads_in_shared_memory);
-        __pyx_t_7 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_cur_scope->__pyx_v_name1), __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_cur_scope->__pyx_v_name1), __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_10;
         __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_7);
         __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_1)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -5394,43 +5017,43 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
         __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_7);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 117, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "mapper.pyx":145
+        /* "mapper.pyx":118
  *                 name2 = "shared_array_" + str(np.random.random())
  *                 logging.info("Yielding chunk with %d reads in shared memory %s" % (chunk.shape[0], name1))
  *                 to_shared_memory(SingleSharedArray(chunk), name1)             # <<<<<<<<<<<<<<
  *                 to_shared_memory(SingleSharedArray(mask), name2)
  *                 yield name1, name2
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_shared_memory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_shared_memory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_3 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
           }
         }
         __pyx_t_7 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_cur_scope->__pyx_v_chunk) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_cur_scope->__pyx_v_chunk);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 145, __pyx_L1_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 118, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = NULL;
         __pyx_t_11 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_1)) {
@@ -5440,72 +5063,72 @@
             __Pyx_DECREF_SET(__pyx_t_2, function);
             __pyx_t_11 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_2)) {
           PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_t_7, __pyx_cur_scope->__pyx_v_name1};
-          __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
           PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_t_7, __pyx_cur_scope->__pyx_v_name1};
-          __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         } else
         #endif
         {
-          __pyx_t_3 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
+          __pyx_t_3 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           if (__pyx_t_1) {
             __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1); __pyx_t_1 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_7);
           PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_11, __pyx_t_7);
           __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name1);
           __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name1);
           PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_11, __pyx_cur_scope->__pyx_v_name1);
           __pyx_t_7 = 0;
-          __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "mapper.pyx":146
+        /* "mapper.pyx":119
  *                 logging.info("Yielding chunk with %d reads in shared memory %s" % (chunk.shape[0], name1))
  *                 to_shared_memory(SingleSharedArray(chunk), name1)
  *                 to_shared_memory(SingleSharedArray(mask), name2)             # <<<<<<<<<<<<<<
  *                 yield name1, name2
  *             else:
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_shared_memory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_shared_memory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 146, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 119, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_1 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
           if (likely(__pyx_t_1)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
             __Pyx_INCREF(__pyx_t_1);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_7, function);
           }
         }
         __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_cur_scope->__pyx_v_mask) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_cur_scope->__pyx_v_mask);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __pyx_t_7 = NULL;
         __pyx_t_11 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_7)) {
@@ -5515,56 +5138,56 @@
             __Pyx_DECREF_SET(__pyx_t_2, function);
             __pyx_t_11 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_2)) {
           PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_3, __pyx_cur_scope->__pyx_v_name2};
-          __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
           PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_3, __pyx_cur_scope->__pyx_v_name2};
-          __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         {
-          __pyx_t_1 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+          __pyx_t_1 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           if (__pyx_t_7) {
             __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_7); __pyx_t_7 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_11, __pyx_t_3);
           __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name2);
           __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name2);
           PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_11, __pyx_cur_scope->__pyx_v_name2);
           __pyx_t_3 = 0;
-          __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "mapper.pyx":147
+        /* "mapper.pyx":120
  *                 to_shared_memory(SingleSharedArray(chunk), name1)
  *                 to_shared_memory(SingleSharedArray(mask), name2)
  *                 yield name1, name2             # <<<<<<<<<<<<<<
  *             else:
  *                 logging.info("Yielding %d reads directly" % (len(chunk)))
  */
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name1);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name1);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_cur_scope->__pyx_v_name1);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name2);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name2);
         PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_cur_scope->__pyx_v_name2);
@@ -5573,43 +5196,43 @@
         __Pyx_XGIVEREF(__pyx_r);
         __Pyx_RefNannyFinishContext();
         __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
         /* return from generator, yielding value */
         __pyx_generator->resume_label = 1;
         return __pyx_r;
         __pyx_L13_resume_from_yield:;
-        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 147, __pyx_L1_error)
+        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 120, __pyx_L1_error)
 
-        /* "mapper.pyx":141
+        /* "mapper.pyx":114
  *         i += 1
  *         if i >= chunk_size:
  *             if write_to_shared_memory:             # <<<<<<<<<<<<<<
  *                 name1 = "shared_array_" + str(np.random.random())
  *                 name2 = "shared_array_" + str(np.random.random())
  */
         goto __pyx_L12;
       }
 
-      /* "mapper.pyx":149
+      /* "mapper.pyx":122
  *                 yield name1, name2
  *             else:
  *                 logging.info("Yielding %d reads directly" % (len(chunk)))             # <<<<<<<<<<<<<<
  *                 yield chunk, mask
  *             logging.info("Took %.3f sec to read %d reads into matrix" % (time.time()-prev_time, chunk_size))
  */
       /*else*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_9 = PyObject_Length(__pyx_cur_scope->__pyx_v_chunk); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 149, __pyx_L1_error)
-        __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+        __pyx_t_9 = PyObject_Length(__pyx_cur_scope->__pyx_v_chunk); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 122, __pyx_L1_error)
+        __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_Yielding_d_reads_directly, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+        __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_Yielding_d_reads_directly, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_2)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -5617,27 +5240,27 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
           }
         }
         __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "mapper.pyx":150
+        /* "mapper.pyx":123
  *             else:
  *                 logging.info("Yielding %d reads directly" % (len(chunk)))
  *                 yield chunk, mask             # <<<<<<<<<<<<<<
  *             logging.info("Took %.3f sec to read %d reads into matrix" % (time.time()-prev_time, chunk_size))
  *             prev_time = time.time()
  */
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_chunk);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_chunk);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_cur_scope->__pyx_v_chunk);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_mask);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_mask);
         PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_cur_scope->__pyx_v_mask);
@@ -5646,85 +5269,85 @@
         __Pyx_XGIVEREF(__pyx_r);
         __Pyx_RefNannyFinishContext();
         __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
         /* return from generator, yielding value */
         __pyx_generator->resume_label = 2;
         return __pyx_r;
         __pyx_L14_resume_from_yield:;
-        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 150, __pyx_L1_error)
+        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 123, __pyx_L1_error)
       }
       __pyx_L12:;
 
-      /* "mapper.pyx":151
+      /* "mapper.pyx":124
  *                 logging.info("Yielding %d reads directly" % (len(chunk)))
  *                 yield chunk, mask
  *             logging.info("Took %.3f sec to read %d reads into matrix" % (time.time()-prev_time, chunk_size))             # <<<<<<<<<<<<<<
  *             prev_time = time.time()
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_9 = 0;
       __pyx_t_10 = 127;
       __Pyx_INCREF(__pyx_kp_u_Took);
       __pyx_t_9 += 5;
       __Pyx_GIVEREF(__pyx_kp_u_Took);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Took);
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_12, function);
         }
       }
       __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_12);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      __pyx_t_12 = PyNumber_Subtract(__pyx_t_2, __pyx_cur_scope->__pyx_v_prev_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_12 = PyNumber_Subtract(__pyx_t_2, __pyx_cur_scope->__pyx_v_prev_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Format(__pyx_t_12, __pyx_kp_u_3f); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Format(__pyx_t_12, __pyx_kp_u_3f); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_10;
       __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
       __pyx_t_2 = 0;
       __Pyx_INCREF(__pyx_kp_u_sec_to_read);
       __pyx_t_9 += 13;
       __Pyx_GIVEREF(__pyx_kp_u_sec_to_read);
       PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_sec_to_read);
-      __pyx_t_2 = __Pyx_PyObject_FormatAndDecref(__Pyx_PyNumber_IntOrLong(__pyx_cur_scope->__pyx_v_chunk_size), __pyx_n_u_d); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_FormatAndDecref(__Pyx_PyNumber_IntOrLong(__pyx_cur_scope->__pyx_v_chunk_size), __pyx_n_u_d); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_10;
       __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
       __pyx_t_2 = 0;
       __Pyx_INCREF(__pyx_kp_u_reads_into_matrix);
       __pyx_t_9 += 18;
       __Pyx_GIVEREF(__pyx_kp_u_reads_into_matrix);
       PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_reads_into_matrix);
-      __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -5732,392 +5355,392 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 124, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "mapper.pyx":152
+      /* "mapper.pyx":125
  *                 yield chunk, mask
  *             logging.info("Took %.3f sec to read %d reads into matrix" % (time.time()-prev_time, chunk_size))
  *             prev_time = time.time()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_prev_time);
       __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_prev_time, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "mapper.pyx":155
+      /* "mapper.pyx":128
  * 
  * 
  *             i = 0             # <<<<<<<<<<<<<<
  *             if process_reads:
  *                 chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
  */
       __Pyx_INCREF(__pyx_int_0);
       __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_i);
       __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_i, __pyx_int_0);
       __Pyx_GIVEREF(__pyx_int_0);
 
-      /* "mapper.pyx":156
+      /* "mapper.pyx":129
  * 
  *             i = 0
  *             if process_reads:             # <<<<<<<<<<<<<<
  *                 chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
  *             else:
  */
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_process_reads); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 156, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_process_reads); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
       if (__pyx_t_6) {
 
-        /* "mapper.pyx":157
+        /* "mapper.pyx":130
  *             i = 0
  *             if process_reads:
  *                 chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *             else:
  *                 chunk = np.empty(chunk_size, dtype="|S" + str(max_read_length))
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_chunk_size);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_chunk_size);
         PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_cur_scope->__pyx_v_chunk_size);
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
         __pyx_t_4 = 0;
-        __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
         __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint64); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint64); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 130, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_chunk);
         __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_chunk, __pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_12);
         __pyx_t_12 = 0;
 
-        /* "mapper.pyx":156
+        /* "mapper.pyx":129
  * 
  *             i = 0
  *             if process_reads:             # <<<<<<<<<<<<<<
  *                 chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
  *             else:
  */
         goto __pyx_L15;
       }
 
-      /* "mapper.pyx":159
+      /* "mapper.pyx":132
  *                 chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
  *             else:
  *                 chunk = np.empty(chunk_size, dtype="|S" + str(max_read_length))             # <<<<<<<<<<<<<<
  * 
  *             mask = np.zeros((chunk_size, max_read_length), dtype=np.bool)  # True where reads have bases (for handling short reads)
  */
       /*else*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_t_12 = PyTuple_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_12 = PyTuple_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_chunk_size);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_chunk_size);
         PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_cur_scope->__pyx_v_chunk_size);
-        __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_S, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_S, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_chunk);
         __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_chunk, __pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_2);
         __pyx_t_2 = 0;
       }
       __pyx_L15:;
 
-      /* "mapper.pyx":161
+      /* "mapper.pyx":134
  *                 chunk = np.empty(chunk_size, dtype="|S" + str(max_read_length))
  * 
  *             mask = np.zeros((chunk_size, max_read_length), dtype=np.bool)  # True where reads have bases (for handling short reads)             # <<<<<<<<<<<<<<
  * 
  *     if i > 0:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_cur_scope->__pyx_v_max_read_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_chunk_size);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_chunk_size);
       PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_cur_scope->__pyx_v_chunk_size);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_2);
       __pyx_t_2 = 0;
-      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_12);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_12);
       __pyx_t_12 = 0;
-      __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_bool); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_bool); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_mask);
       __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_mask, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "mapper.pyx":140
+      /* "mapper.pyx":113
  * 
  *         i += 1
  *         if i >= chunk_size:             # <<<<<<<<<<<<<<
  *             if write_to_shared_memory:
  *                 name1 = "shared_array_" + str(np.random.random())
  */
     }
     __pyx_L6_continue:;
   }
   __pyx_L7_break:;
 
-  /* "mapper.pyx":163
+  /* "mapper.pyx":136
  *             mask = np.zeros((chunk_size, max_read_length), dtype=np.bool)  # True where reads have bases (for handling short reads)
  * 
  *     if i > 0:             # <<<<<<<<<<<<<<
  *         logging.info("Yielding %d reads in the end" % i)
  *         if write_to_shared_memory:
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_i, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_cur_scope->__pyx_v_i, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
 
-    /* "mapper.pyx":164
+    /* "mapper.pyx":137
  * 
  *     if i > 0:
  *         logging.info("Yielding %d reads in the end" % i)             # <<<<<<<<<<<<<<
  *         if write_to_shared_memory:
  *             name1 = "shared_array_" + str(np.random.random())
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_info); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_info); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_12 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Yielding_d_reads_in_the_end, __pyx_cur_scope->__pyx_v_i); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Yielding_d_reads_in_the_end, __pyx_cur_scope->__pyx_v_i); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_12) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_12);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "mapper.pyx":165
+    /* "mapper.pyx":138
  *     if i > 0:
  *         logging.info("Yielding %d reads in the end" % i)
  *         if write_to_shared_memory:             # <<<<<<<<<<<<<<
  *             name1 = "shared_array_" + str(np.random.random())
  *             name2 = "shared_array_" + str(np.random.random())
  */
-    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_write_to_shared_memory); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_write_to_shared_memory); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 138, __pyx_L1_error)
     if (__pyx_t_6) {
 
-      /* "mapper.pyx":166
+      /* "mapper.pyx":139
  *         logging.info("Yielding %d reads in the end" % i)
  *         if write_to_shared_memory:
  *             name1 = "shared_array_" + str(np.random.random())             # <<<<<<<<<<<<<<
  *             name2 = "shared_array_" + str(np.random.random())
  *             to_shared_memory(SingleSharedArray(chunk[0:i]), name1)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 166, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __pyx_t_12 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_12)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_12);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_12) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_n_u_shared_array, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_n_u_shared_array, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_name1);
       __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_name1, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "mapper.pyx":167
+      /* "mapper.pyx":140
  *         if write_to_shared_memory:
  *             name1 = "shared_array_" + str(np.random.random())
  *             name2 = "shared_array_" + str(np.random.random())             # <<<<<<<<<<<<<<
  *             to_shared_memory(SingleSharedArray(chunk[0:i]), name1)
  *             to_shared_memory(SingleSharedArray(mask[0:i]), name2)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __pyx_t_12 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_12)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_12);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_12) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_n_u_shared_array, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_n_u_shared_array, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_name2);
       __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_name2, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "mapper.pyx":168
+      /* "mapper.pyx":141
  *             name1 = "shared_array_" + str(np.random.random())
  *             name2 = "shared_array_" + str(np.random.random())
  *             to_shared_memory(SingleSharedArray(chunk[0:i]), name1)             # <<<<<<<<<<<<<<
  *             to_shared_memory(SingleSharedArray(mask[0:i]), name2)
  *             yield name1, name2
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_shared_memory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_shared_memory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_cur_scope->__pyx_v_chunk, 0, 0, NULL, &__pyx_cur_scope->__pyx_v_i, NULL, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_cur_scope->__pyx_v_chunk, 0, 0, NULL, &__pyx_cur_scope->__pyx_v_i, NULL, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_12 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 168, __pyx_L1_error)
+      if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 141, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       __pyx_t_11 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
@@ -6127,75 +5750,75 @@
           __Pyx_DECREF_SET(__pyx_t_2, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_2)) {
         PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_12, __pyx_cur_scope->__pyx_v_name1};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
         PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_12, __pyx_cur_scope->__pyx_v_name1};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       } else
       #endif
       {
-        __pyx_t_3 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         if (__pyx_t_4) {
           __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4); __pyx_t_4 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_12);
         PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_11, __pyx_t_12);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name1);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name1);
         PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_11, __pyx_cur_scope->__pyx_v_name1);
         __pyx_t_12 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "mapper.pyx":169
+      /* "mapper.pyx":142
  *             name2 = "shared_array_" + str(np.random.random())
  *             to_shared_memory(SingleSharedArray(chunk[0:i]), name1)
  *             to_shared_memory(SingleSharedArray(mask[0:i]), name2)             # <<<<<<<<<<<<<<
  *             yield name1, name2
  *         else:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_shared_memory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_shared_memory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 169, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 142, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
-      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_cur_scope->__pyx_v_mask, 0, 0, NULL, &__pyx_cur_scope->__pyx_v_i, NULL, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_cur_scope->__pyx_v_mask, 0, 0, NULL, &__pyx_cur_scope->__pyx_v_i, NULL, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_12, function);
         }
       }
       __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_7, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __pyx_t_12 = NULL;
       __pyx_t_11 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_12)) {
@@ -6205,56 +5828,56 @@
           __Pyx_DECREF_SET(__pyx_t_2, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_2)) {
         PyObject *__pyx_temp[3] = {__pyx_t_12, __pyx_t_3, __pyx_cur_scope->__pyx_v_name2};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
         PyObject *__pyx_temp[3] = {__pyx_t_12, __pyx_t_3, __pyx_cur_scope->__pyx_v_name2};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else
       #endif
       {
-        __pyx_t_4 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (__pyx_t_12) {
           __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_12); __pyx_t_12 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_11, __pyx_t_3);
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name2);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name2);
         PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_11, __pyx_cur_scope->__pyx_v_name2);
         __pyx_t_3 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "mapper.pyx":170
+      /* "mapper.pyx":143
  *             to_shared_memory(SingleSharedArray(chunk[0:i]), name1)
  *             to_shared_memory(SingleSharedArray(mask[0:i]), name2)
  *             yield name1, name2             # <<<<<<<<<<<<<<
  *         else:
  *             yield chunk[0:i], mask[0:i]
  */
-      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name1);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name1);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_v_name1);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name2);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name2);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_cur_scope->__pyx_v_name2);
@@ -6263,39 +5886,39 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, yielding value */
       __pyx_generator->resume_label = 3;
       return __pyx_r;
       __pyx_L18_resume_from_yield:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 170, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 143, __pyx_L1_error)
 
-      /* "mapper.pyx":165
+      /* "mapper.pyx":138
  *     if i > 0:
  *         logging.info("Yielding %d reads in the end" % i)
  *         if write_to_shared_memory:             # <<<<<<<<<<<<<<
  *             name1 = "shared_array_" + str(np.random.random())
  *             name2 = "shared_array_" + str(np.random.random())
  */
       goto __pyx_L17;
     }
 
-    /* "mapper.pyx":172
+    /* "mapper.pyx":145
  *             yield name1, name2
  *         else:
  *             yield chunk[0:i], mask[0:i]             # <<<<<<<<<<<<<<
  * 
  *     fclose(cfile)
  */
     /*else*/ {
-      __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_cur_scope->__pyx_v_chunk, 0, 0, NULL, &__pyx_cur_scope->__pyx_v_i, NULL, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_cur_scope->__pyx_v_chunk, 0, 0, NULL, &__pyx_cur_scope->__pyx_v_i, NULL, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_cur_scope->__pyx_v_mask, 0, 0, NULL, &__pyx_cur_scope->__pyx_v_i, NULL, 1, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_cur_scope->__pyx_v_mask, 0, 0, NULL, &__pyx_cur_scope->__pyx_v_i, NULL, 1, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 172, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
       __pyx_t_1 = 0;
       __pyx_t_2 = 0;
@@ -6304,38 +5927,38 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, yielding value */
       __pyx_generator->resume_label = 4;
       return __pyx_r;
       __pyx_L19_resume_from_yield:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 172, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 145, __pyx_L1_error)
     }
     __pyx_L17:;
 
-    /* "mapper.pyx":163
+    /* "mapper.pyx":136
  *             mask = np.zeros((chunk_size, max_read_length), dtype=np.bool)  # True where reads have bases (for handling short reads)
  * 
  *     if i > 0:             # <<<<<<<<<<<<<<
  *         logging.info("Yielding %d reads in the end" % i)
  *         if write_to_shared_memory:
  */
   }
 
-  /* "mapper.pyx":174
+  /* "mapper.pyx":147
  *             yield chunk[0:i], mask[0:i]
  * 
  *     fclose(cfile)             # <<<<<<<<<<<<<<
  * 
- * cpdef handle_reads(filename):
+ * 
  */
   (void)(fclose(__pyx_cur_scope->__pyx_v_cfile));
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "mapper.pyx":90
+  /* "mapper.pyx":65
  * 
  * 
  * def read_fasta_into_chunks(filename, chunk_size=1000, int max_read_length=150, write_to_shared_memory=False, process_reads=False):             # <<<<<<<<<<<<<<
  *     logging.info("Reading fasta %s" % filename)
  *     filename_byte_string = filename.encode("UTF-8")
  */
 
@@ -6357,887 +5980,26 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mapper.pyx":176
- *     fclose(cfile)
- * 
- * cpdef handle_reads(filename):             # <<<<<<<<<<<<<<
- * 
- *     cdef int sum_hashes = 0
- */
-
-static PyObject *__pyx_pw_6mapper_13handle_reads(PyObject *__pyx_self, PyObject *__pyx_v_filename); /*proto*/
-static PyObject *__pyx_f_6mapper_handle_reads(PyObject *__pyx_v_filename, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  int __pyx_v_sum_hashes;
-  int __pyx_v_max_read_length;
-  PyArrayObject *__pyx_v_read_array = 0;
-  PyArrayObject *__pyx_v_reverse_complement_read_array = 0;
-  int __pyx_v_k;
-  PyArrayObject *__pyx_v_power_array = 0;
-  int __pyx_v_read_length;
-  int __pyx_v_i;
-  PyObject *__pyx_v_lines = NULL;
-  PyObject *__pyx_v_line = NULL;
-  PyObject *__pyx_v_kmers = NULL;
-  CYTHON_UNUSED PyObject *__pyx_v_reverse_complement_kmers = NULL;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_power_array;
-  __Pyx_Buffer __pyx_pybuffer_power_array;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_read_array;
-  __Pyx_Buffer __pyx_pybuffer_read_array;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_reverse_complement_read_array;
-  __Pyx_Buffer __pyx_pybuffer_reverse_complement_read_array;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyArrayObject *__pyx_t_6 = NULL;
-  PyArrayObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
-  PyObject *__pyx_t_10 = NULL;
-  PyArrayObject *__pyx_t_11 = NULL;
-  Py_ssize_t __pyx_t_12;
-  PyObject *(*__pyx_t_13)(PyObject *);
-  Py_ssize_t __pyx_t_14;
-  char *__pyx_t_15;
-  __Pyx_memviewslice __pyx_t_16 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  __Pyx_memviewslice __pyx_t_17 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  Py_ssize_t __pyx_t_18;
-  int __pyx_t_19;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("handle_reads", 0);
-  __pyx_pybuffer_read_array.pybuffer.buf = NULL;
-  __pyx_pybuffer_read_array.refcount = 0;
-  __pyx_pybuffernd_read_array.data = NULL;
-  __pyx_pybuffernd_read_array.rcbuffer = &__pyx_pybuffer_read_array;
-  __pyx_pybuffer_reverse_complement_read_array.pybuffer.buf = NULL;
-  __pyx_pybuffer_reverse_complement_read_array.refcount = 0;
-  __pyx_pybuffernd_reverse_complement_read_array.data = NULL;
-  __pyx_pybuffernd_reverse_complement_read_array.rcbuffer = &__pyx_pybuffer_reverse_complement_read_array;
-  __pyx_pybuffer_power_array.pybuffer.buf = NULL;
-  __pyx_pybuffer_power_array.refcount = 0;
-  __pyx_pybuffernd_power_array.data = NULL;
-  __pyx_pybuffernd_power_array.rcbuffer = &__pyx_pybuffer_power_array;
-
-  /* "mapper.pyx":178
- * cpdef handle_reads(filename):
- * 
- *     cdef int sum_hashes = 0             # <<<<<<<<<<<<<<
- *     cdef int max_read_length = 150
- *     #cdef np.uint64_t[:] read_array = np.zeros(read_length, dtype=np.uint64)
- */
-  __pyx_v_sum_hashes = 0;
-
-  /* "mapper.pyx":179
- * 
- *     cdef int sum_hashes = 0
- *     cdef int max_read_length = 150             # <<<<<<<<<<<<<<
- *     #cdef np.uint64_t[:] read_array = np.zeros(read_length, dtype=np.uint64)
- *     cdef np.ndarray[np.uint64_t] read_array = np.zeros(max_read_length, dtype=np.uint64)
- */
-  __pyx_v_max_read_length = 0x96;
-
-  /* "mapper.pyx":181
- *     cdef int max_read_length = 150
- *     #cdef np.uint64_t[:] read_array = np.zeros(read_length, dtype=np.uint64)
- *     cdef np.ndarray[np.uint64_t] read_array = np.zeros(max_read_length, dtype=np.uint64)             # <<<<<<<<<<<<<<
- *     #cdef np.uint64_t[:] reverse_complement_read_array = np.zeros(read_length, dtype=np.uint64)
- *     cdef np.ndarray[np.uint64_t] reverse_complement_read_array = np.zeros(max_read_length, dtype=np.uint64)
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_max_read_length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 181, __pyx_L1_error)
-  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_read_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-      __pyx_v_read_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_read_array.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 181, __pyx_L1_error)
-    } else {__pyx_pybuffernd_read_array.diminfo[0].strides = __pyx_pybuffernd_read_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_read_array.diminfo[0].shape = __pyx_pybuffernd_read_array.rcbuffer->pybuffer.shape[0];
-    }
-  }
-  __pyx_t_6 = 0;
-  __pyx_v_read_array = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
-
-  /* "mapper.pyx":183
- *     cdef np.ndarray[np.uint64_t] read_array = np.zeros(max_read_length, dtype=np.uint64)
- *     #cdef np.uint64_t[:] reverse_complement_read_array = np.zeros(read_length, dtype=np.uint64)
- *     cdef np.ndarray[np.uint64_t] reverse_complement_read_array = np.zeros(max_read_length, dtype=np.uint64)             # <<<<<<<<<<<<<<
- *     cdef int k = 31
- *     cdef np.ndarray[np.int64_t] power_array = np.power(4, np.arange(0, k))
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_max_read_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 183, __pyx_L1_error)
-  __pyx_t_7 = ((PyArrayObject *)__pyx_t_4);
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_reverse_complement_read_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-      __pyx_v_reverse_complement_read_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_reverse_complement_read_array.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 183, __pyx_L1_error)
-    } else {__pyx_pybuffernd_reverse_complement_read_array.diminfo[0].strides = __pyx_pybuffernd_reverse_complement_read_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_reverse_complement_read_array.diminfo[0].shape = __pyx_pybuffernd_reverse_complement_read_array.rcbuffer->pybuffer.shape[0];
-    }
-  }
-  __pyx_t_7 = 0;
-  __pyx_v_reverse_complement_read_array = ((PyArrayObject *)__pyx_t_4);
-  __pyx_t_4 = 0;
-
-  /* "mapper.pyx":184
- *     #cdef np.uint64_t[:] reverse_complement_read_array = np.zeros(read_length, dtype=np.uint64)
- *     cdef np.ndarray[np.uint64_t] reverse_complement_read_array = np.zeros(max_read_length, dtype=np.uint64)
- *     cdef int k = 31             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[np.int64_t] power_array = np.power(4, np.arange(0, k))
- *     cdef int read_length
- */
-  __pyx_v_k = 31;
-
-  /* "mapper.pyx":185
- *     cdef np.ndarray[np.uint64_t] reverse_complement_read_array = np.zeros(max_read_length, dtype=np.uint64)
- *     cdef int k = 31
- *     cdef np.ndarray[np.int64_t] power_array = np.power(4, np.arange(0, k))             # <<<<<<<<<<<<<<
- *     cdef int read_length
- *     cdef int i = 0
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_power); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_arange); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = NULL;
-  __pyx_t_9 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_9 = 1;
-    }
-  }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_int_0, __pyx_t_1};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_int_0, __pyx_t_1};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    if (__pyx_t_8) {
-      __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
-    }
-    __Pyx_INCREF(__pyx_int_0);
-    __Pyx_GIVEREF(__pyx_int_0);
-    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_int_0);
-    __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_1);
-    __pyx_t_1 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  __pyx_t_9 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_9 = 1;
-    }
-  }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_int_4, __pyx_t_5};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_int_4, __pyx_t_5};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    if (__pyx_t_2) {
-      __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_2); __pyx_t_2 = NULL;
-    }
-    __Pyx_INCREF(__pyx_int_4);
-    __Pyx_GIVEREF(__pyx_int_4);
-    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_int_4);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_5);
-    __pyx_t_5 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 185, __pyx_L1_error)
-  __pyx_t_11 = ((PyArrayObject *)__pyx_t_4);
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_power_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-      __pyx_v_power_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_power_array.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 185, __pyx_L1_error)
-    } else {__pyx_pybuffernd_power_array.diminfo[0].strides = __pyx_pybuffernd_power_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_power_array.diminfo[0].shape = __pyx_pybuffernd_power_array.rcbuffer->pybuffer.shape[0];
-    }
-  }
-  __pyx_t_11 = 0;
-  __pyx_v_power_array = ((PyArrayObject *)__pyx_t_4);
-  __pyx_t_4 = 0;
-
-  /* "mapper.pyx":187
- *     cdef np.ndarray[np.int64_t] power_array = np.power(4, np.arange(0, k))
- *     cdef int read_length
- *     cdef int i = 0             # <<<<<<<<<<<<<<
- * 
- *     #lines = util.read_fasta(filename)
- */
-  __pyx_v_i = 0;
-
-  /* "mapper.pyx":191
- *     #lines = util.read_fasta(filename)
- *     #lines = util.read_fasta(filename)
- *     lines = read_fasta(filename)             # <<<<<<<<<<<<<<
- *     for line in lines:
- *         read_length = len(line) - 3
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_read_fasta); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_10 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_10)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_10);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_10, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_filename);
-  __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_lines = __pyx_t_4;
-  __pyx_t_4 = 0;
-
-  /* "mapper.pyx":192
- *     #lines = util.read_fasta(filename)
- *     lines = read_fasta(filename)
- *     for line in lines:             # <<<<<<<<<<<<<<
- *         read_length = len(line) - 3
- *         read_sequence_to_kmer_hashes(line, read_array, reverse_complement_read_array, read_length)
- */
-  if (likely(PyList_CheckExact(__pyx_v_lines)) || PyTuple_CheckExact(__pyx_v_lines)) {
-    __pyx_t_4 = __pyx_v_lines; __Pyx_INCREF(__pyx_t_4); __pyx_t_12 = 0;
-    __pyx_t_13 = NULL;
-  } else {
-    __pyx_t_12 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_lines); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_13 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 192, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_13)) {
-      if (likely(PyList_CheckExact(__pyx_t_4))) {
-        if (__pyx_t_12 >= PyList_GET_SIZE(__pyx_t_4)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_12); __Pyx_INCREF(__pyx_t_3); __pyx_t_12++; if (unlikely(0 < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
-        #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_4, __pyx_t_12); __pyx_t_12++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        #endif
-      } else {
-        if (__pyx_t_12 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_12); __Pyx_INCREF(__pyx_t_3); __pyx_t_12++; if (unlikely(0 < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
-        #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_4, __pyx_t_12); __pyx_t_12++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        #endif
-      }
-    } else {
-      __pyx_t_3 = __pyx_t_13(__pyx_t_4);
-      if (unlikely(!__pyx_t_3)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 192, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_3);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_line, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "mapper.pyx":193
- *     lines = read_fasta(filename)
- *     for line in lines:
- *         read_length = len(line) - 3             # <<<<<<<<<<<<<<
- *         read_sequence_to_kmer_hashes(line, read_array, reverse_complement_read_array, read_length)
- *         sum_hashes += read_array[0]
- */
-    __pyx_t_14 = PyObject_Length(__pyx_v_line); if (unlikely(__pyx_t_14 == ((Py_ssize_t)-1))) __PYX_ERR(0, 193, __pyx_L1_error)
-    __pyx_v_read_length = (__pyx_t_14 - 3);
-
-    /* "mapper.pyx":194
- *     for line in lines:
- *         read_length = len(line) - 3
- *         read_sequence_to_kmer_hashes(line, read_array, reverse_complement_read_array, read_length)             # <<<<<<<<<<<<<<
- *         sum_hashes += read_array[0]
- *         kmers = np.convolve(read_array, power_array, mode='valid')
- */
-    __pyx_t_15 = __Pyx_PyObject_AsWritableString(__pyx_v_line); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 194, __pyx_L1_error)
-    __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(((PyObject *)__pyx_v_read_array), PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 194, __pyx_L1_error)
-    __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(((PyObject *)__pyx_v_reverse_complement_read_array), PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 194, __pyx_L1_error)
-    __pyx_f_6mapper_read_sequence_to_kmer_hashes(__pyx_t_15, __pyx_t_16, __pyx_t_17, __pyx_v_read_length);
-    __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
-    __pyx_t_16.memview = NULL;
-    __pyx_t_16.data = NULL;
-    __PYX_XDEC_MEMVIEW(&__pyx_t_17, 1);
-    __pyx_t_17.memview = NULL;
-    __pyx_t_17.data = NULL;
-
-    /* "mapper.pyx":195
- *         read_length = len(line) - 3
- *         read_sequence_to_kmer_hashes(line, read_array, reverse_complement_read_array, read_length)
- *         sum_hashes += read_array[0]             # <<<<<<<<<<<<<<
- *         kmers = np.convolve(read_array, power_array, mode='valid')
- *         reverse_complement_kmers = np.convolve(reverse_complement_read_array, power_array, mode='valid')
- */
-    __pyx_t_18 = 0;
-    __pyx_t_9 = -1;
-    if (__pyx_t_18 < 0) {
-      __pyx_t_18 += __pyx_pybuffernd_read_array.diminfo[0].shape;
-      if (unlikely(__pyx_t_18 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_read_array.diminfo[0].shape)) __pyx_t_9 = 0;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
-      __PYX_ERR(0, 195, __pyx_L1_error)
-    }
-    __pyx_v_sum_hashes = (__pyx_v_sum_hashes + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_uint64_t *, __pyx_pybuffernd_read_array.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_read_array.diminfo[0].strides)));
-
-    /* "mapper.pyx":196
- *         read_sequence_to_kmer_hashes(line, read_array, reverse_complement_read_array, read_length)
- *         sum_hashes += read_array[0]
- *         kmers = np.convolve(read_array, power_array, mode='valid')             # <<<<<<<<<<<<<<
- *         reverse_complement_kmers = np.convolve(reverse_complement_read_array, power_array, mode='valid')
- *         sum_hashes += reverse_complement_read_array[10]
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_convolve); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 196, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_INCREF(((PyObject *)__pyx_v_read_array));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_read_array));
-    PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_read_array));
-    __Pyx_INCREF(((PyObject *)__pyx_v_power_array));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_power_array));
-    PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_power_array));
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 196, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_mode, __pyx_n_u_valid) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_kmers, __pyx_t_2);
-    __pyx_t_2 = 0;
-
-    /* "mapper.pyx":197
- *         sum_hashes += read_array[0]
- *         kmers = np.convolve(read_array, power_array, mode='valid')
- *         reverse_complement_kmers = np.convolve(reverse_complement_read_array, power_array, mode='valid')             # <<<<<<<<<<<<<<
- *         sum_hashes += reverse_complement_read_array[10]
- * 
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_convolve); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(((PyObject *)__pyx_v_reverse_complement_read_array));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_reverse_complement_read_array));
-    PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_reverse_complement_read_array));
-    __Pyx_INCREF(((PyObject *)__pyx_v_power_array));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_power_array));
-    PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_power_array));
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mode, __pyx_n_u_valid) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_reverse_complement_kmers, __pyx_t_10);
-    __pyx_t_10 = 0;
-
-    /* "mapper.pyx":198
- *         kmers = np.convolve(read_array, power_array, mode='valid')
- *         reverse_complement_kmers = np.convolve(reverse_complement_read_array, power_array, mode='valid')
- *         sum_hashes += reverse_complement_read_array[10]             # <<<<<<<<<<<<<<
- * 
- *         if i == 0:
- */
-    __pyx_t_18 = 10;
-    __pyx_t_9 = -1;
-    if (__pyx_t_18 < 0) {
-      __pyx_t_18 += __pyx_pybuffernd_reverse_complement_read_array.diminfo[0].shape;
-      if (unlikely(__pyx_t_18 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_reverse_complement_read_array.diminfo[0].shape)) __pyx_t_9 = 0;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
-      __PYX_ERR(0, 198, __pyx_L1_error)
-    }
-    __pyx_v_sum_hashes = (__pyx_v_sum_hashes + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_uint64_t *, __pyx_pybuffernd_reverse_complement_read_array.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_reverse_complement_read_array.diminfo[0].strides)));
-
-    /* "mapper.pyx":200
- *         sum_hashes += reverse_complement_read_array[10]
- * 
- *         if i == 0:             # <<<<<<<<<<<<<<
- *             print(kmers)
- * 
- */
-    __pyx_t_19 = ((__pyx_v_i == 0) != 0);
-    if (__pyx_t_19) {
-
-      /* "mapper.pyx":201
- * 
- *         if i == 0:
- *             print(kmers)             # <<<<<<<<<<<<<<
- * 
- *         i += 1
- */
-      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_v_kmers); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 201, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-
-      /* "mapper.pyx":200
- *         sum_hashes += reverse_complement_read_array[10]
- * 
- *         if i == 0:             # <<<<<<<<<<<<<<
- *             print(kmers)
- * 
- */
-    }
-
-    /* "mapper.pyx":203
- *             print(kmers)
- * 
- *         i += 1             # <<<<<<<<<<<<<<
- * 
- *     print(sum_hashes)
- */
-    __pyx_v_i = (__pyx_v_i + 1);
-
-    /* "mapper.pyx":192
- *     #lines = util.read_fasta(filename)
- *     lines = read_fasta(filename)
- *     for line in lines:             # <<<<<<<<<<<<<<
- *         read_length = len(line) - 3
- *         read_sequence_to_kmer_hashes(line, read_array, reverse_complement_read_array, read_length)
- */
-  }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-
-  /* "mapper.pyx":205
- *         i += 1
- * 
- *     print(sum_hashes)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_sum_hashes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-
-  /* "mapper.pyx":176
- *     fclose(cfile)
- * 
- * cpdef handle_reads(filename):             # <<<<<<<<<<<<<<
- * 
- *     cdef int sum_hashes = 0
- */
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_10);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_17, 1);
-  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_power_array.rcbuffer->pybuffer);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_read_array.rcbuffer->pybuffer);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_reverse_complement_read_array.rcbuffer->pybuffer);
-  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("mapper.handle_reads", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  goto __pyx_L2;
-  __pyx_L0:;
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_power_array.rcbuffer->pybuffer);
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_read_array.rcbuffer->pybuffer);
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_reverse_complement_read_array.rcbuffer->pybuffer);
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_read_array);
-  __Pyx_XDECREF((PyObject *)__pyx_v_reverse_complement_read_array);
-  __Pyx_XDECREF((PyObject *)__pyx_v_power_array);
-  __Pyx_XDECREF(__pyx_v_lines);
-  __Pyx_XDECREF(__pyx_v_line);
-  __Pyx_XDECREF(__pyx_v_kmers);
-  __Pyx_XDECREF(__pyx_v_reverse_complement_kmers);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* Python wrapper */
-static PyObject *__pyx_pw_6mapper_13handle_reads(PyObject *__pyx_self, PyObject *__pyx_v_filename); /*proto*/
-static PyObject *__pyx_pw_6mapper_13handle_reads(PyObject *__pyx_self, PyObject *__pyx_v_filename) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("handle_reads (wrapper)", 0);
-  __pyx_r = __pyx_pf_6mapper_12handle_reads(__pyx_self, ((PyObject *)__pyx_v_filename));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_6mapper_12handle_reads(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("handle_reads", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6mapper_handle_reads(__pyx_v_filename, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("mapper.handle_reads", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "mapper.pyx":208
- * 
- * 
- * cdef read_file(filename):             # <<<<<<<<<<<<<<
- *     cdef i = 0
- *     result = read_fasta(filename)
- */
-
-static PyObject *__pyx_f_6mapper_read_file(PyObject *__pyx_v_filename) {
-  PyObject *__pyx_v_i = 0;
-  CYTHON_UNUSED PyObject *__pyx_v_result = NULL;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("read_file", 0);
-
-  /* "mapper.pyx":209
- * 
- * cdef read_file(filename):
- *     cdef i = 0             # <<<<<<<<<<<<<<
- *     result = read_fasta(filename)
- *     return i
- */
-  __Pyx_INCREF(__pyx_int_0);
-  __pyx_v_i = __pyx_int_0;
-
-  /* "mapper.pyx":210
- * cdef read_file(filename):
- *     cdef i = 0
- *     result = read_fasta(filename)             # <<<<<<<<<<<<<<
- *     return i
- * 
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_read_fasta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_filename);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_result = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "mapper.pyx":211
- *     cdef i = 0
- *     result = read_fasta(filename)
- *     return i             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_i);
-  __pyx_r = __pyx_v_i;
-  goto __pyx_L0;
-
-  /* "mapper.pyx":208
- * 
- * 
- * cdef read_file(filename):             # <<<<<<<<<<<<<<
- *     cdef i = 0
- *     result = read_fasta(filename)
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("mapper.read_file", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_i);
-  __Pyx_XDECREF(__pyx_v_result);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "mapper.pyx":214
- * 
- * 
- * cpdef get_count(filename):             # <<<<<<<<<<<<<<
- *     return handle_reads(filename)
- * 
- */
-
-static PyObject *__pyx_pw_6mapper_15get_count(PyObject *__pyx_self, PyObject *__pyx_v_filename); /*proto*/
-static PyObject *__pyx_f_6mapper_get_count(PyObject *__pyx_v_filename, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_count", 0);
-
-  /* "mapper.pyx":215
- * 
- * cpdef get_count(filename):
- *     return handle_reads(filename)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6mapper_handle_reads(__pyx_v_filename, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "mapper.pyx":214
- * 
- * 
- * cpdef get_count(filename):             # <<<<<<<<<<<<<<
- *     return handle_reads(filename)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("mapper.get_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* Python wrapper */
-static PyObject *__pyx_pw_6mapper_15get_count(PyObject *__pyx_self, PyObject *__pyx_v_filename); /*proto*/
-static PyObject *__pyx_pw_6mapper_15get_count(PyObject *__pyx_self, PyObject *__pyx_v_filename) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("get_count (wrapper)", 0);
-  __pyx_r = __pyx_pf_6mapper_14get_count(__pyx_self, ((PyObject *)__pyx_v_filename));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_6mapper_14get_count(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_count", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6mapper_get_count(__pyx_v_filename, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("mapper.get_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "mapper.pyx":221
+/* "mapper.pyx":153
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def map_kmers_to_graph_index(index, int max_node_id, np.uint64_t[:] kmers, int max_index_lookup_frequency=1000):             # <<<<<<<<<<<<<<
  * 
  *     # index arrays
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6mapper_17map_kmers_to_graph_index(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_6mapper_17map_kmers_to_graph_index = {"map_kmers_to_graph_index", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6mapper_17map_kmers_to_graph_index, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_6mapper_17map_kmers_to_graph_index(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6mapper_10map_kmers_to_graph_index(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_6mapper_10map_kmers_to_graph_index = {"map_kmers_to_graph_index", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6mapper_10map_kmers_to_graph_index, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_6mapper_10map_kmers_to_graph_index(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_index = 0;
   int __pyx_v_max_node_id;
   __Pyx_memviewslice __pyx_v_kmers = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_v_max_index_lookup_frequency;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -7267,68 +6029,68 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_node_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("map_kmers_to_graph_index", 0, 3, 4, 1); __PYX_ERR(0, 221, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("map_kmers_to_graph_index", 0, 3, 4, 1); __PYX_ERR(0, 153, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kmers)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("map_kmers_to_graph_index", 0, 3, 4, 2); __PYX_ERR(0, 221, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("map_kmers_to_graph_index", 0, 3, 4, 2); __PYX_ERR(0, 153, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_index_lookup_frequency);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "map_kmers_to_graph_index") < 0)) __PYX_ERR(0, 221, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "map_kmers_to_graph_index") < 0)) __PYX_ERR(0, 153, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_index = values[0];
-    __pyx_v_max_node_id = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_max_node_id == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 221, __pyx_L3_error)
-    __pyx_v_kmers = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kmers.memview)) __PYX_ERR(0, 221, __pyx_L3_error)
+    __pyx_v_max_node_id = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_max_node_id == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L3_error)
+    __pyx_v_kmers = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kmers.memview)) __PYX_ERR(0, 153, __pyx_L3_error)
     if (values[3]) {
-      __pyx_v_max_index_lookup_frequency = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_max_index_lookup_frequency == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 221, __pyx_L3_error)
+      __pyx_v_max_index_lookup_frequency = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_max_index_lookup_frequency == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L3_error)
     } else {
       __pyx_v_max_index_lookup_frequency = ((int)0x3E8);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("map_kmers_to_graph_index", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 221, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("map_kmers_to_graph_index", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 153, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("mapper.map_kmers_to_graph_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6mapper_16map_kmers_to_graph_index(__pyx_self, __pyx_v_index, __pyx_v_max_node_id, __pyx_v_kmers, __pyx_v_max_index_lookup_frequency);
+  __pyx_r = __pyx_pf_6mapper_9map_kmers_to_graph_index(__pyx_self, __pyx_v_index, __pyx_v_max_node_id, __pyx_v_kmers, __pyx_v_max_index_lookup_frequency);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6mapper_16map_kmers_to_graph_index(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_index, int __pyx_v_max_node_id, __Pyx_memviewslice __pyx_v_kmers, int __pyx_v_max_index_lookup_frequency) {
+static PyObject *__pyx_pf_6mapper_9map_kmers_to_graph_index(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_index, int __pyx_v_max_node_id, __Pyx_memviewslice __pyx_v_kmers, int __pyx_v_max_index_lookup_frequency) {
   __Pyx_memviewslice __pyx_v_hashes_to_index = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_n_kmers = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_nodes = { 0, 0, { 0 }, { 0 }, { 0 } };
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_ref_offsets = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_index_kmers = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_index_frequencies = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_v_n_local_hits;
@@ -7375,209 +6137,209 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("map_kmers_to_graph_index", 0);
   __pyx_pybuffer_node_counts.pybuffer.buf = NULL;
   __pyx_pybuffer_node_counts.refcount = 0;
   __pyx_pybuffernd_node_counts.data = NULL;
   __pyx_pybuffernd_node_counts.rcbuffer = &__pyx_pybuffer_node_counts;
 
-  /* "mapper.pyx":224
+  /* "mapper.pyx":156
  * 
  *     # index arrays
  *     cdef np.int64_t[:] hashes_to_index = index._hashes_to_index             # <<<<<<<<<<<<<<
  *     cdef np.uint32_t[:] n_kmers = index._n_kmers
  *     cdef np.uint32_t[:] nodes = index._nodes
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_hashes_to_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_hashes_to_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_hashes_to_index = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "mapper.pyx":225
+  /* "mapper.pyx":157
  *     # index arrays
  *     cdef np.int64_t[:] hashes_to_index = index._hashes_to_index
  *     cdef np.uint32_t[:] n_kmers = index._n_kmers             # <<<<<<<<<<<<<<
  *     cdef np.uint32_t[:] nodes = index._nodes
  *     cdef np.uint64_t[:] ref_offsets = index._ref_offsets
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_n_kmers); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_n_kmers); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 157, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_n_kmers = __pyx_t_3;
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
 
-  /* "mapper.pyx":226
+  /* "mapper.pyx":158
  *     cdef np.int64_t[:] hashes_to_index = index._hashes_to_index
  *     cdef np.uint32_t[:] n_kmers = index._n_kmers
  *     cdef np.uint32_t[:] nodes = index._nodes             # <<<<<<<<<<<<<<
  *     cdef np.uint64_t[:] ref_offsets = index._ref_offsets
  *     cdef np.uint64_t[:] index_kmers = index._kmers
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_nodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_nodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_nodes = __pyx_t_3;
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
 
-  /* "mapper.pyx":227
+  /* "mapper.pyx":159
  *     cdef np.uint32_t[:] n_kmers = index._n_kmers
  *     cdef np.uint32_t[:] nodes = index._nodes
  *     cdef np.uint64_t[:] ref_offsets = index._ref_offsets             # <<<<<<<<<<<<<<
  *     cdef np.uint64_t[:] index_kmers = index._kmers
  *     cdef np.uint16_t[:] index_frequencies = index._frequencies
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_ref_offsets); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_ref_offsets); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_ref_offsets = __pyx_t_4;
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
-  /* "mapper.pyx":228
+  /* "mapper.pyx":160
  *     cdef np.uint32_t[:] nodes = index._nodes
  *     cdef np.uint64_t[:] ref_offsets = index._ref_offsets
  *     cdef np.uint64_t[:] index_kmers = index._kmers             # <<<<<<<<<<<<<<
  *     cdef np.uint16_t[:] index_frequencies = index._frequencies
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_kmers_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_kmers_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_index_kmers = __pyx_t_4;
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
-  /* "mapper.pyx":229
+  /* "mapper.pyx":161
  *     cdef np.uint64_t[:] ref_offsets = index._ref_offsets
  *     cdef np.uint64_t[:] index_kmers = index._kmers
  *     cdef np.uint16_t[:] index_frequencies = index._frequencies             # <<<<<<<<<<<<<<
  * 
  *     cdef int n_local_hits
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_frequencies); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_frequencies); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint16_t(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_index_frequencies = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
-  /* "mapper.pyx":236
+  /* "mapper.pyx":168
  *     cdef int l, j, i
  *     cdef long hash
  *     cdef int modulo = index._modulo             # <<<<<<<<<<<<<<
  *     #logging.info("Hash modulo is %d. Max index lookup frequency is %d." % (modulo, max_index_lookup_frequency))
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_modulo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_modulo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_modulo = __pyx_t_6;
 
-  /* "mapper.pyx":239
+  /* "mapper.pyx":171
  *     #logging.info("Hash modulo is %d. Max index lookup frequency is %d." % (modulo, max_index_lookup_frequency))
  * 
  *     cdef np.ndarray[np.float_t] node_counts = np.zeros(max_node_id+1, dtype=np.float)             # <<<<<<<<<<<<<<
  *     #cdef np.float_t[:] node_counts = np.zeros(max_node_id+1, dtype=np.float)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_long((__pyx_v_max_node_id + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long((__pyx_v_max_node_id + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_float); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_float); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_8, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_10) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_10, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (!(likely(((__pyx_t_10) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_10, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 171, __pyx_L1_error)
   __pyx_t_11 = ((PyArrayObject *)__pyx_t_10);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_counts.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_node_counts = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_node_counts.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 239, __pyx_L1_error)
+      __PYX_ERR(0, 171, __pyx_L1_error)
     } else {__pyx_pybuffernd_node_counts.diminfo[0].strides = __pyx_pybuffernd_node_counts.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_node_counts.diminfo[0].shape = __pyx_pybuffernd_node_counts.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_11 = 0;
   __pyx_v_node_counts = ((PyArrayObject *)__pyx_t_10);
   __pyx_t_10 = 0;
 
-  /* "mapper.pyx":242
+  /* "mapper.pyx":174
  *     #cdef np.float_t[:] node_counts = np.zeros(max_node_id+1, dtype=np.float)
  * 
  *     t = time.time()             # <<<<<<<<<<<<<<
  *     cdef np.uint64_t[:] kmer_hashes = np.mod(kmers, modulo)
  *     #logging.info("Time spent taking modulo: %.4f" % (time.time()-t))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_10 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_t = __pyx_t_10;
   __pyx_t_10 = 0;
 
-  /* "mapper.pyx":243
+  /* "mapper.pyx":175
  * 
  *     t = time.time()
  *     cdef np.uint64_t[:] kmer_hashes = np.mod(kmers, modulo)             # <<<<<<<<<<<<<<
  *     #logging.info("Time spent taking modulo: %.4f" % (time.time()-t))
  *     t = time.time()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_mod); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_mod); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_kmers, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_kmers, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_modulo); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_modulo); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_9 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -7586,376 +6348,376 @@
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_8, __pyx_t_7};
-    __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_8, __pyx_t_7};
-    __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_12 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_12 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     if (__pyx_t_9) {
       __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_9); __pyx_t_9 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_6, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_6, __pyx_t_7);
     __pyx_t_8 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_10, PyBUF_WRITABLE); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint64_t(__pyx_t_10, PyBUF_WRITABLE); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_kmer_hashes = __pyx_t_4;
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
-  /* "mapper.pyx":245
+  /* "mapper.pyx":177
  *     cdef np.uint64_t[:] kmer_hashes = np.mod(kmers, modulo)
  *     #logging.info("Time spent taking modulo: %.4f" % (time.time()-t))
  *     t = time.time()             # <<<<<<<<<<<<<<
  *     cdef int n_collisions = 0
  *     cdef int n_kmers_mapped = 0
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_12);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_12, function);
     }
   }
   __pyx_t_10 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_DECREF_SET(__pyx_v_t, __pyx_t_10);
   __pyx_t_10 = 0;
 
-  /* "mapper.pyx":246
+  /* "mapper.pyx":178
  *     #logging.info("Time spent taking modulo: %.4f" % (time.time()-t))
  *     t = time.time()
  *     cdef int n_collisions = 0             # <<<<<<<<<<<<<<
  *     cdef int n_kmers_mapped = 0
  *     cdef int n_skipped_high_frequency = 0
  */
   __pyx_v_n_collisions = 0;
 
-  /* "mapper.pyx":247
+  /* "mapper.pyx":179
  *     t = time.time()
  *     cdef int n_collisions = 0
  *     cdef int n_kmers_mapped = 0             # <<<<<<<<<<<<<<
  *     cdef int n_skipped_high_frequency = 0
  *     cdef int n_no_index_hits = 0
  */
   __pyx_v_n_kmers_mapped = 0;
 
-  /* "mapper.pyx":248
+  /* "mapper.pyx":180
  *     cdef int n_collisions = 0
  *     cdef int n_kmers_mapped = 0
  *     cdef int n_skipped_high_frequency = 0             # <<<<<<<<<<<<<<
  *     cdef int n_no_index_hits = 0
  *     #logging.info("Will process %d kmers" % kmers.shape[0])
  */
   __pyx_v_n_skipped_high_frequency = 0;
 
-  /* "mapper.pyx":249
+  /* "mapper.pyx":181
  *     cdef int n_kmers_mapped = 0
  *     cdef int n_skipped_high_frequency = 0
  *     cdef int n_no_index_hits = 0             # <<<<<<<<<<<<<<
  *     #logging.info("Will process %d kmers" % kmers.shape[0])
  *     for i in range(kmers.shape[0]):
  */
   __pyx_v_n_no_index_hits = 0;
 
-  /* "mapper.pyx":251
+  /* "mapper.pyx":183
  *     cdef int n_no_index_hits = 0
  *     #logging.info("Will process %d kmers" % kmers.shape[0])
  *     for i in range(kmers.shape[0]):             # <<<<<<<<<<<<<<
  *         hash = kmer_hashes[i]
  * 
  */
   __pyx_t_13 = (__pyx_v_kmers.shape[0]);
   __pyx_t_14 = __pyx_t_13;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_14; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "mapper.pyx":252
+    /* "mapper.pyx":184
  *     #logging.info("Will process %d kmers" % kmers.shape[0])
  *     for i in range(kmers.shape[0]):
  *         hash = kmer_hashes[i]             # <<<<<<<<<<<<<<
  * 
  *         if hash == 0:
  */
     __pyx_t_15 = __pyx_v_i;
     __pyx_v_hash = (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_kmer_hashes.data + __pyx_t_15 * __pyx_v_kmer_hashes.strides[0]) )));
 
-    /* "mapper.pyx":254
+    /* "mapper.pyx":186
  *         hash = kmer_hashes[i]
  * 
  *         if hash == 0:             # <<<<<<<<<<<<<<
  *             continue
  * 
  */
     __pyx_t_16 = ((__pyx_v_hash == 0) != 0);
     if (__pyx_t_16) {
 
-      /* "mapper.pyx":255
+      /* "mapper.pyx":187
  * 
  *         if hash == 0:
  *             continue             # <<<<<<<<<<<<<<
  * 
  *         n_local_hits = n_kmers[hash]
  */
       goto __pyx_L3_continue;
 
-      /* "mapper.pyx":254
+      /* "mapper.pyx":186
  *         hash = kmer_hashes[i]
  * 
  *         if hash == 0:             # <<<<<<<<<<<<<<
  *             continue
  * 
  */
     }
 
-    /* "mapper.pyx":257
+    /* "mapper.pyx":189
  *             continue
  * 
  *         n_local_hits = n_kmers[hash]             # <<<<<<<<<<<<<<
  *         if n_local_hits == 0:
  *             n_no_index_hits += 1
  */
     __pyx_t_15 = __pyx_v_hash;
     __pyx_v_n_local_hits = (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_n_kmers.data + __pyx_t_15 * __pyx_v_n_kmers.strides[0]) )));
 
-    /* "mapper.pyx":258
+    /* "mapper.pyx":190
  * 
  *         n_local_hits = n_kmers[hash]
  *         if n_local_hits == 0:             # <<<<<<<<<<<<<<
  *             n_no_index_hits += 1
  * 
  */
     __pyx_t_16 = ((__pyx_v_n_local_hits == 0) != 0);
     if (__pyx_t_16) {
 
-      /* "mapper.pyx":259
+      /* "mapper.pyx":191
  *         n_local_hits = n_kmers[hash]
  *         if n_local_hits == 0:
  *             n_no_index_hits += 1             # <<<<<<<<<<<<<<
  * 
  *         index_position = hashes_to_index[hash]
  */
       __pyx_v_n_no_index_hits = (__pyx_v_n_no_index_hits + 1);
 
-      /* "mapper.pyx":258
+      /* "mapper.pyx":190
  * 
  *         n_local_hits = n_kmers[hash]
  *         if n_local_hits == 0:             # <<<<<<<<<<<<<<
  *             n_no_index_hits += 1
  * 
  */
     }
 
-    /* "mapper.pyx":261
+    /* "mapper.pyx":193
  *             n_no_index_hits += 1
  * 
  *         index_position = hashes_to_index[hash]             # <<<<<<<<<<<<<<
  * 
  *         for j in range(n_local_hits):
  */
     __pyx_t_15 = __pyx_v_hash;
     __pyx_v_index_position = (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ (__pyx_v_hashes_to_index.data + __pyx_t_15 * __pyx_v_hashes_to_index.strides[0]) )));
 
-    /* "mapper.pyx":263
+    /* "mapper.pyx":195
  *         index_position = hashes_to_index[hash]
  * 
  *         for j in range(n_local_hits):             # <<<<<<<<<<<<<<
  *             l = index_position + j
  *             # Check that this entry actually matches the kmer, sometimes it will not due to collision
  */
     __pyx_t_17 = __pyx_v_n_local_hits;
     __pyx_t_18 = __pyx_t_17;
     for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
       __pyx_v_j = __pyx_t_19;
 
-      /* "mapper.pyx":264
+      /* "mapper.pyx":196
  * 
  *         for j in range(n_local_hits):
  *             l = index_position + j             # <<<<<<<<<<<<<<
  *             # Check that this entry actually matches the kmer, sometimes it will not due to collision
  *             if index_kmers[l] != kmers[i]:
  */
       __pyx_v_l = (__pyx_v_index_position + __pyx_v_j);
 
-      /* "mapper.pyx":266
+      /* "mapper.pyx":198
  *             l = index_position + j
  *             # Check that this entry actually matches the kmer, sometimes it will not due to collision
  *             if index_kmers[l] != kmers[i]:             # <<<<<<<<<<<<<<
  *                 n_collisions += 1
  *                 continue
  */
       __pyx_t_15 = __pyx_v_l;
       __pyx_t_20 = __pyx_v_i;
       __pyx_t_16 = (((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_index_kmers.data + __pyx_t_15 * __pyx_v_index_kmers.strides[0]) ))) != (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ (__pyx_v_kmers.data + __pyx_t_20 * __pyx_v_kmers.strides[0]) )))) != 0);
       if (__pyx_t_16) {
 
-        /* "mapper.pyx":267
+        /* "mapper.pyx":199
  *             # Check that this entry actually matches the kmer, sometimes it will not due to collision
  *             if index_kmers[l] != kmers[i]:
  *                 n_collisions += 1             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
         __pyx_v_n_collisions = (__pyx_v_n_collisions + 1);
 
-        /* "mapper.pyx":268
+        /* "mapper.pyx":200
  *             if index_kmers[l] != kmers[i]:
  *                 n_collisions += 1
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             if index_frequencies[l] > max_index_lookup_frequency:
  */
         goto __pyx_L7_continue;
 
-        /* "mapper.pyx":266
+        /* "mapper.pyx":198
  *             l = index_position + j
  *             # Check that this entry actually matches the kmer, sometimes it will not due to collision
  *             if index_kmers[l] != kmers[i]:             # <<<<<<<<<<<<<<
  *                 n_collisions += 1
  *                 continue
  */
       }
 
-      /* "mapper.pyx":270
+      /* "mapper.pyx":202
  *                 continue
  * 
  *             if index_frequencies[l] > max_index_lookup_frequency:             # <<<<<<<<<<<<<<
  *                 n_skipped_high_frequency += 1
  *                 continue
  */
       __pyx_t_20 = __pyx_v_l;
       __pyx_t_16 = (((*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ (__pyx_v_index_frequencies.data + __pyx_t_20 * __pyx_v_index_frequencies.strides[0]) ))) > __pyx_v_max_index_lookup_frequency) != 0);
       if (__pyx_t_16) {
 
-        /* "mapper.pyx":271
+        /* "mapper.pyx":203
  * 
  *             if index_frequencies[l] > max_index_lookup_frequency:
  *                 n_skipped_high_frequency += 1             # <<<<<<<<<<<<<<
  *                 continue
  *             node_counts[nodes[l]] += 1
  */
         __pyx_v_n_skipped_high_frequency = (__pyx_v_n_skipped_high_frequency + 1);
 
-        /* "mapper.pyx":272
+        /* "mapper.pyx":204
  *             if index_frequencies[l] > max_index_lookup_frequency:
  *                 n_skipped_high_frequency += 1
  *                 continue             # <<<<<<<<<<<<<<
  *             node_counts[nodes[l]] += 1
  *             n_kmers_mapped += 1
  */
         goto __pyx_L7_continue;
 
-        /* "mapper.pyx":270
+        /* "mapper.pyx":202
  *                 continue
  * 
  *             if index_frequencies[l] > max_index_lookup_frequency:             # <<<<<<<<<<<<<<
  *                 n_skipped_high_frequency += 1
  *                 continue
  */
       }
 
-      /* "mapper.pyx":273
+      /* "mapper.pyx":205
  *                 n_skipped_high_frequency += 1
  *                 continue
  *             node_counts[nodes[l]] += 1             # <<<<<<<<<<<<<<
  *             n_kmers_mapped += 1
  * 
  */
       __pyx_t_20 = __pyx_v_l;
       __pyx_t_21 = (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_v_nodes.data + __pyx_t_20 * __pyx_v_nodes.strides[0]) )));
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_node_counts.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_node_counts.diminfo[0].strides) += 1.0;
 
-      /* "mapper.pyx":274
+      /* "mapper.pyx":206
  *                 continue
  *             node_counts[nodes[l]] += 1
  *             n_kmers_mapped += 1             # <<<<<<<<<<<<<<
  * 
  *     logging.info("Time spent looking up kmers in index: %.3f" % (time.time()-t))
  */
       __pyx_v_n_kmers_mapped = (__pyx_v_n_kmers_mapped + 1);
       __pyx_L7_continue:;
     }
     __pyx_L3_continue:;
   }
 
-  /* "mapper.pyx":276
+  /* "mapper.pyx":208
  *             n_kmers_mapped += 1
  * 
  *     logging.info("Time spent looking up kmers in index: %.3f" % (time.time()-t))             # <<<<<<<<<<<<<<
  *     #logging.info("N kmers with no index hits: %d" % n_no_index_hits)
  *     #logging.info("N hash collisions: %d" % n_collisions)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logging); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_time); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_12 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyNumber_Subtract(__pyx_t_12, __pyx_v_t); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_8 = PyNumber_Subtract(__pyx_t_12, __pyx_v_t); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Time_spent_looking_up_kmers_in_i, __pyx_t_8); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Time_spent_looking_up_kmers_in_i, __pyx_t_8); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -7963,32 +6725,32 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_10 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_t_12) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_12);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "mapper.pyx":281
+  /* "mapper.pyx":213
  *     #logging.info("N skipped because too high frequency: %d" % n_skipped_high_frequency)
  *     #logging.info("N kmers mapped: %d" % n_kmers_mapped)
  *     return node_counts             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_node_counts));
   __pyx_r = ((PyObject *)__pyx_v_node_counts);
   goto __pyx_L0;
 
-  /* "mapper.pyx":221
+  /* "mapper.pyx":153
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def map_kmers_to_graph_index(index, int max_node_id, np.uint64_t[:] kmers, int max_index_lookup_frequency=1000):             # <<<<<<<<<<<<<<
  * 
  *     # index arrays
  */
 
@@ -8559,15 +7321,15 @@
       /* "../../../../usr/local/lib/python3.8/dist-packages/numpy/__init__.pxd":947
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -8691,15 +7453,15 @@
       /* "../../../../usr/local/lib/python3.8/dist-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -8823,15 +7585,15 @@
       /* "../../../../usr/local/lib/python3.8/dist-packages/numpy/__init__.pxd":959
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 959, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 959, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 959, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -9247,15 +8009,15 @@
     /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 133, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 133, __pyx_L1_error)
 
     /* "View.MemoryView":132
  *         self.itemsize = itemsize
@@ -9279,15 +8041,15 @@
     /* "View.MemoryView":136
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 136, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 136, __pyx_L1_error)
 
     /* "View.MemoryView":135
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -9406,15 +8168,15 @@
     /* "View.MemoryView":148
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 148, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 148, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 148, __pyx_L1_error)
 
     /* "View.MemoryView":147
  *         self._strides = self._shape + self.ndim
@@ -9680,15 +8442,15 @@
       /* "View.MemoryView":176
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 176, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 176, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(2, 176, __pyx_L1_error)
 
       /* "View.MemoryView":175
  * 
@@ -9924,15 +8686,15 @@
     /* "View.MemoryView":192
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 192, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 192, __pyx_L1_error)
 
     /* "View.MemoryView":191
  *         elif self.mode == u"fortran":
@@ -10658,15 +9420,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -10714,15 +9476,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -12424,15 +11186,15 @@
     /* "View.MemoryView":418
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 418, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 418, __pyx_L1_error)
 
     /* "View.MemoryView":417
  * 
@@ -13472,15 +12234,15 @@
       /* "View.MemoryView":495
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 495, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 495, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(2, 495, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -13834,15 +12596,15 @@
     /* "View.MemoryView":520
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 520, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 520, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 520, __pyx_L1_error)
 
     /* "View.MemoryView":519
  *     @cname('getbuffer')
@@ -14383,15 +13145,15 @@
     /* "View.MemoryView":570
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 570, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 570, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 570, __pyx_L1_error)
 
     /* "View.MemoryView":568
  *     @property
@@ -14500,15 +13262,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__19, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 577, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__18, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":576
@@ -15538,15 +14300,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -15594,15 +14356,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -15951,17 +14713,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 682, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 682, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__22);
-            __Pyx_GIVEREF(__pyx_slice__22);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__22);
+            __Pyx_INCREF(__pyx_slice__21);
+            __Pyx_GIVEREF(__pyx_slice__21);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__21);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 682, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":683
  *             if not seen_ellipsis:
@@ -15986,15 +14748,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__22); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 685, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__21); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 685, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":686
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -16126,17 +14888,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 696, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__22);
-        __Pyx_GIVEREF(__pyx_slice__22);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__22);
+        __Pyx_INCREF(__pyx_slice__21);
+        __Pyx_GIVEREF(__pyx_slice__21);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__21);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 696, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":695
  * 
@@ -16255,15 +15017,15 @@
       /* "View.MemoryView":703
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 703, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 703, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(2, 703, __pyx_L1_error)
 
       /* "View.MemoryView":702
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -18439,15 +17201,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -18495,15 +17257,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -22062,169 +20824,55 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *__pyx_freelist_6mapper___pyx_scope_struct__read_fasta[8];
-static int __pyx_freecount_6mapper___pyx_scope_struct__read_fasta = 0;
-
-static PyObject *__pyx_tp_new_6mapper___pyx_scope_struct__read_fasta(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6mapper___pyx_scope_struct__read_fasta > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta)))) {
-    o = (PyObject*)__pyx_freelist_6mapper___pyx_scope_struct__read_fasta[--__pyx_freecount_6mapper___pyx_scope_struct__read_fasta];
-    memset(o, 0, sizeof(struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta));
-    (void) PyObject_INIT(o, t);
-    PyObject_GC_Track(o);
-  } else {
-    o = (*t->tp_alloc)(t, 0);
-    if (unlikely(!o)) return 0;
-  }
-  return o;
-}
-
-static void __pyx_tp_dealloc_6mapper___pyx_scope_struct__read_fasta(PyObject *o) {
-  struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *p = (struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *)o;
-  PyObject_GC_UnTrack(o);
-  Py_CLEAR(p->__pyx_v_filename);
-  Py_CLEAR(p->__pyx_v_filename_byte_string);
-  Py_CLEAR(p->__pyx_v_i);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6mapper___pyx_scope_struct__read_fasta < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta)))) {
-    __pyx_freelist_6mapper___pyx_scope_struct__read_fasta[__pyx_freecount_6mapper___pyx_scope_struct__read_fasta++] = ((struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *)o);
-  } else {
-    (*Py_TYPE(o)->tp_free)(o);
-  }
-}
-
-static int __pyx_tp_traverse_6mapper___pyx_scope_struct__read_fasta(PyObject *o, visitproc v, void *a) {
-  int e;
-  struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *p = (struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta *)o;
-  if (p->__pyx_v_filename) {
-    e = (*v)(p->__pyx_v_filename, a); if (e) return e;
-  }
-  if (p->__pyx_v_filename_byte_string) {
-    e = (*v)(p->__pyx_v_filename_byte_string, a); if (e) return e;
-  }
-  if (p->__pyx_v_i) {
-    e = (*v)(p->__pyx_v_i, a); if (e) return e;
-  }
-  return 0;
-}
-
-static PyTypeObject __pyx_type_6mapper___pyx_scope_struct__read_fasta = {
-  PyVarObject_HEAD_INIT(0, 0)
-  "mapper.__pyx_scope_struct__read_fasta", /*tp_name*/
-  sizeof(struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta), /*tp_basicsize*/
-  0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6mapper___pyx_scope_struct__read_fasta, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
-  0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
-  0, /*tp_getattr*/
-  0, /*tp_setattr*/
-  #if PY_MAJOR_VERSION < 3
-  0, /*tp_compare*/
-  #endif
-  #if PY_MAJOR_VERSION >= 3
-  0, /*tp_as_async*/
-  #endif
-  0, /*tp_repr*/
-  0, /*tp_as_number*/
-  0, /*tp_as_sequence*/
-  0, /*tp_as_mapping*/
-  0, /*tp_hash*/
-  0, /*tp_call*/
-  0, /*tp_str*/
-  0, /*tp_getattro*/
-  0, /*tp_setattro*/
-  0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  0, /*tp_doc*/
-  __pyx_tp_traverse_6mapper___pyx_scope_struct__read_fasta, /*tp_traverse*/
-  0, /*tp_clear*/
-  0, /*tp_richcompare*/
-  0, /*tp_weaklistoffset*/
-  0, /*tp_iter*/
-  0, /*tp_iternext*/
-  0, /*tp_methods*/
-  0, /*tp_members*/
-  0, /*tp_getset*/
-  0, /*tp_base*/
-  0, /*tp_dict*/
-  0, /*tp_descr_get*/
-  0, /*tp_descr_set*/
-  0, /*tp_dictoffset*/
-  0, /*tp_init*/
-  0, /*tp_alloc*/
-  __pyx_tp_new_6mapper___pyx_scope_struct__read_fasta, /*tp_new*/
-  0, /*tp_free*/
-  0, /*tp_is_gc*/
-  0, /*tp_bases*/
-  0, /*tp_mro*/
-  0, /*tp_cache*/
-  0, /*tp_subclasses*/
-  0, /*tp_weaklist*/
-  0, /*tp_del*/
-  0, /*tp_version_tag*/
-  #if PY_VERSION_HEX >= 0x030400a1
-  0, /*tp_finalize*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-};
-
-static struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *__pyx_freelist_6mapper___pyx_scope_struct_1_read_fasta_into_chunks[8];
-static int __pyx_freecount_6mapper___pyx_scope_struct_1_read_fasta_into_chunks = 0;
+static struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *__pyx_freelist_6mapper___pyx_scope_struct__read_fasta_into_chunks[8];
+static int __pyx_freecount_6mapper___pyx_scope_struct__read_fasta_into_chunks = 0;
 
-static PyObject *__pyx_tp_new_6mapper___pyx_scope_struct_1_read_fasta_into_chunks(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_6mapper___pyx_scope_struct__read_fasta_into_chunks(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6mapper___pyx_scope_struct_1_read_fasta_into_chunks > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks)))) {
-    o = (PyObject*)__pyx_freelist_6mapper___pyx_scope_struct_1_read_fasta_into_chunks[--__pyx_freecount_6mapper___pyx_scope_struct_1_read_fasta_into_chunks];
-    memset(o, 0, sizeof(struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_6mapper___pyx_scope_struct__read_fasta_into_chunks > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks)))) {
+    o = (PyObject*)__pyx_freelist_6mapper___pyx_scope_struct__read_fasta_into_chunks[--__pyx_freecount_6mapper___pyx_scope_struct__read_fasta_into_chunks];
+    memset(o, 0, sizeof(struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_6mapper___pyx_scope_struct_1_read_fasta_into_chunks(PyObject *o) {
-  struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *p = (struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *)o;
+static void __pyx_tp_dealloc_6mapper___pyx_scope_struct__read_fasta_into_chunks(PyObject *o) {
+  struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *p = (struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_chunk);
   Py_CLEAR(p->__pyx_v_chunk_size);
   Py_CLEAR(p->__pyx_v_filename);
   Py_CLEAR(p->__pyx_v_filename_byte_string);
   Py_CLEAR(p->__pyx_v_i);
   Py_CLEAR(p->__pyx_v_mask);
   Py_CLEAR(p->__pyx_v_name1);
   Py_CLEAR(p->__pyx_v_name2);
   Py_CLEAR(p->__pyx_v_prev_time);
   Py_CLEAR(p->__pyx_v_process_reads);
   Py_CLEAR(p->__pyx_v_write_to_shared_memory);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6mapper___pyx_scope_struct_1_read_fasta_into_chunks < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks)))) {
-    __pyx_freelist_6mapper___pyx_scope_struct_1_read_fasta_into_chunks[__pyx_freecount_6mapper___pyx_scope_struct_1_read_fasta_into_chunks++] = ((struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_6mapper___pyx_scope_struct__read_fasta_into_chunks < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks)))) {
+    __pyx_freelist_6mapper___pyx_scope_struct__read_fasta_into_chunks[__pyx_freecount_6mapper___pyx_scope_struct__read_fasta_into_chunks++] = ((struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_6mapper___pyx_scope_struct_1_read_fasta_into_chunks(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_6mapper___pyx_scope_struct__read_fasta_into_chunks(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *p = (struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks *)o;
+  struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *p = (struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks *)o;
   if (p->__pyx_v_chunk) {
     e = (*v)(p->__pyx_v_chunk, a); if (e) return e;
   }
   if (p->__pyx_v_chunk_size) {
     e = (*v)(p->__pyx_v_chunk_size, a); if (e) return e;
   }
   if (p->__pyx_v_filename) {
@@ -22253,20 +20901,20 @@
   }
   if (p->__pyx_v_write_to_shared_memory) {
     e = (*v)(p->__pyx_v_write_to_shared_memory, a); if (e) return e;
   }
   return 0;
 }
 
-static PyTypeObject __pyx_type_6mapper___pyx_scope_struct_1_read_fasta_into_chunks = {
+static PyTypeObject __pyx_type_6mapper___pyx_scope_struct__read_fasta_into_chunks = {
   PyVarObject_HEAD_INIT(0, 0)
-  "mapper.__pyx_scope_struct_1_read_fasta_into_chunks", /*tp_name*/
-  sizeof(struct __pyx_obj_6mapper___pyx_scope_struct_1_read_fasta_into_chunks), /*tp_basicsize*/
+  "mapper.__pyx_scope_struct__read_fasta_into_chunks", /*tp_name*/
+  sizeof(struct __pyx_obj_6mapper___pyx_scope_struct__read_fasta_into_chunks), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6mapper___pyx_scope_struct_1_read_fasta_into_chunks, /*tp_dealloc*/
+  __pyx_tp_dealloc_6mapper___pyx_scope_struct__read_fasta_into_chunks, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -22285,15 +20933,15 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_6mapper___pyx_scope_struct_1_read_fasta_into_chunks, /*tp_traverse*/
+  __pyx_tp_traverse_6mapper___pyx_scope_struct__read_fasta_into_chunks, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
@@ -22301,15 +20949,15 @@
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_6mapper___pyx_scope_struct_1_read_fasta_into_chunks, /*tp_new*/
+  __pyx_tp_new_6mapper___pyx_scope_struct__read_fasta_into_chunks, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -23040,16 +21688,14 @@
   0, /*tp_print*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"test", (PyCFunction)__pyx_pw_6mapper_3test, METH_NOARGS, 0},
   {"count_lines_in_fasta", (PyCFunction)__pyx_pw_6mapper_5count_lines_in_fasta, METH_O, 0},
-  {"handle_reads", (PyCFunction)__pyx_pw_6mapper_13handle_reads, METH_O, 0},
-  {"get_count", (PyCFunction)__pyx_pw_6mapper_15get_count, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
 static int __pyx_pymod_exec_mapper(PyObject* module); /*proto*/
@@ -23126,29 +21772,27 @@
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_kp_u_Yielding_chunk_with, __pyx_k_Yielding_chunk_with, sizeof(__pyx_k_Yielding_chunk_with), 0, 1, 0, 0},
   {&__pyx_kp_u_Yielding_d_reads_directly, __pyx_k_Yielding_d_reads_directly, sizeof(__pyx_k_Yielding_d_reads_directly), 0, 1, 0, 0},
   {&__pyx_kp_u_Yielding_d_reads_in_the_end, __pyx_k_Yielding_d_reads_in_the_end, sizeof(__pyx_k_Yielding_d_reads_in_the_end), 0, 1, 0, 0},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
-  {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_bool, __pyx_k_bool, sizeof(__pyx_k_bool), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_cfile, __pyx_k_cfile, sizeof(__pyx_k_cfile), 0, 0, 1, 1},
   {&__pyx_n_s_chunk, __pyx_k_chunk, sizeof(__pyx_k_chunk), 0, 0, 1, 1},
   {&__pyx_n_s_chunk_size, __pyx_k_chunk_size, sizeof(__pyx_k_chunk_size), 0, 0, 1, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
-  {&__pyx_n_s_convolve, __pyx_k_convolve, sizeof(__pyx_k_convolve), 0, 0, 1, 1},
   {&__pyx_n_u_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 1, 0, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
@@ -23225,15 +21869,14 @@
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
-  {&__pyx_n_s_power, __pyx_k_power, sizeof(__pyx_k_power), 0, 0, 1, 1},
   {&__pyx_n_s_prev_time, __pyx_k_prev_time, sizeof(__pyx_k_prev_time), 0, 0, 1, 1},
   {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
   {&__pyx_n_s_process_reads, __pyx_k_process_reads, sizeof(__pyx_k_process_reads), 0, 0, 1, 1},
   {&__pyx_n_s_py_read_file, __pyx_k_py_read_file, sizeof(__pyx_k_py_read_file), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
@@ -23242,15 +21885,14 @@
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
   {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
-  {&__pyx_n_s_read_fasta, __pyx_k_read_fasta, sizeof(__pyx_k_read_fasta), 0, 0, 1, 1},
   {&__pyx_n_s_read_fasta_into_chunks, __pyx_k_read_fasta_into_chunks, sizeof(__pyx_k_read_fasta_into_chunks), 0, 0, 1, 1},
   {&__pyx_kp_u_reads_in_shared_memory, __pyx_k_reads_in_shared_memory, sizeof(__pyx_k_reads_in_shared_memory), 0, 1, 0, 0},
   {&__pyx_kp_u_reads_into_matrix, __pyx_k_reads_into_matrix, sizeof(__pyx_k_reads_into_matrix), 0, 1, 0, 0},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_ref_offsets, __pyx_k_ref_offsets, sizeof(__pyx_k_ref_offsets), 0, 0, 1, 1},
@@ -23267,36 +21909,36 @@
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
+  {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
   {&__pyx_n_s_t, __pyx_k_t, sizeof(__pyx_k_t), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_u_test2, __pyx_k_test2, sizeof(__pyx_k_test2), 0, 1, 0, 1},
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_to_shared_memory, __pyx_k_to_shared_memory, sizeof(__pyx_k_to_shared_memory), 0, 0, 1, 1},
   {&__pyx_n_s_uint64, __pyx_k_uint64, sizeof(__pyx_k_uint64), 0, 0, 1, 1},
   {&__pyx_n_s_uint8, __pyx_k_uint8, sizeof(__pyx_k_uint8), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_util, __pyx_k_util, sizeof(__pyx_k_util), 0, 0, 1, 1},
-  {&__pyx_n_u_valid, __pyx_k_valid, sizeof(__pyx_k_valid), 0, 1, 0, 1},
   {&__pyx_n_s_write_to_shared_memory, __pyx_k_write_to_shared_memory, sizeof(__pyx_k_write_to_shared_memory), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 13, __pyx_L1_error)
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 17, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 38, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 947, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 133, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
@@ -23306,386 +21948,373 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "mapper.pyx":13
+  /* "mapper.pyx":14
  * 
  * def py_read_file(filename):
  *     with open(filename, "r") as f:             # <<<<<<<<<<<<<<
  *         return f.read()
  * 
  */
-  __pyx_tuple_ = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "mapper.pyx":17
+  /* "mapper.pyx":18
  * 
  * cpdef test():
  *     print("test2")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_u_test2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_u_test2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "mapper.pyx":131
+  /* "mapper.pyx":104
  *         #chunk[i,line_length] = line
  *         if process_reads:
  *             chunk[i, 0:line_length] = np.frombuffer(line, dtype=np.uint8)[:-1]  # remove \n at end             # <<<<<<<<<<<<<<
  *             mask[i, 0:line_length] = True
  *             # a bit slower:
  */
-  __pyx_slice__5 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__5);
-  __Pyx_GIVEREF(__pyx_slice__5);
+  __pyx_slice__4 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__4)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__4);
+  __Pyx_GIVEREF(__pyx_slice__4);
 
   /* "../../../../usr/local/lib/python3.8/dist-packages/numpy/__init__.pxd":947
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 947, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 947, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "../../../../usr/local/lib/python3.8/dist-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 953, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 953, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "View.MemoryView":136
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "View.MemoryView":148
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 148, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "View.MemoryView":176
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 176, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "View.MemoryView":192
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 192, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "View.MemoryView":418
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 418, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 418, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "View.MemoryView":495
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 495, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "View.MemoryView":520
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 520, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 520, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "View.MemoryView":570
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 570, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 570, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "View.MemoryView":577
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__19 = PyTuple_New(1); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 577, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
+  __pyx_tuple__18 = PyTuple_New(1); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 577, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__19, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  PyTuple_SET_ITEM(__pyx_tuple__18, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "View.MemoryView":682
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__22 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__22)) __PYX_ERR(2, 682, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__22);
-  __Pyx_GIVEREF(__pyx_slice__22);
+  __pyx_slice__21 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__21)) __PYX_ERR(2, 682, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__21);
+  __Pyx_GIVEREF(__pyx_slice__21);
 
   /* "View.MemoryView":703
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 703, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 703, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
-  /* "mapper.pyx":12
- * from graph_kmer_index.shared_mem import to_shared_memory, SingleSharedArray
+  /* "mapper.pyx":13
+ * import sys
  * 
  * def py_read_file(filename):             # <<<<<<<<<<<<<<
  *     with open(filename, "r") as f:
  *         return f.read()
  */
-  __pyx_tuple__26 = PyTuple_Pack(2, __pyx_n_s_filename, __pyx_n_s_f); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 12, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmer_mapper_mapper_pyx, __pyx_n_s_py_read_file, 12, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 12, __pyx_L1_error)
-
-  /* "mapper.pyx":56
- *         i_reverse_complement -= 1
- * 
- * def read_fasta(filename):             # <<<<<<<<<<<<<<
- *     filename_byte_string = filename.encode("UTF-8")
- *     cdef char * fname = filename_byte_string
- */
-  __pyx_tuple__28 = PyTuple_Pack(8, __pyx_n_s_filename, __pyx_n_s_filename_byte_string, __pyx_n_s_fname, __pyx_n_s_cfile, __pyx_n_s_line, __pyx_n_s_l, __pyx_n_s_read, __pyx_n_s_i); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 56, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmer_mapper_mapper_pyx, __pyx_n_s_read_fasta, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_filename, __pyx_n_s_f); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmer_mapper_mapper_pyx, __pyx_n_s_py_read_file, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 13, __pyx_L1_error)
 
-  /* "mapper.pyx":90
+  /* "mapper.pyx":65
  * 
  * 
  * def read_fasta_into_chunks(filename, chunk_size=1000, int max_read_length=150, write_to_shared_memory=False, process_reads=False):             # <<<<<<<<<<<<<<
  *     logging.info("Reading fasta %s" % filename)
  *     filename_byte_string = filename.encode("UTF-8")
  */
-  __pyx_tuple__29 = PyTuple_Pack(18, __pyx_n_s_filename, __pyx_n_s_chunk_size, __pyx_n_s_max_read_length, __pyx_n_s_write_to_shared_memory, __pyx_n_s_process_reads, __pyx_n_s_filename_byte_string, __pyx_n_s_fname, __pyx_n_s_cfile, __pyx_n_s_line, __pyx_n_s_l, __pyx_n_s_read, __pyx_n_s_i, __pyx_n_s_line_length, __pyx_n_s_chunk, __pyx_n_s_mask, __pyx_n_s_prev_time, __pyx_n_s_name1, __pyx_n_s_name2); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(5, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmer_mapper_mapper_pyx, __pyx_n_s_read_fasta_into_chunks, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(18, __pyx_n_s_filename, __pyx_n_s_chunk_size, __pyx_n_s_max_read_length, __pyx_n_s_write_to_shared_memory, __pyx_n_s_process_reads, __pyx_n_s_filename_byte_string, __pyx_n_s_fname, __pyx_n_s_cfile, __pyx_n_s_line, __pyx_n_s_l, __pyx_n_s_read, __pyx_n_s_i, __pyx_n_s_line_length, __pyx_n_s_chunk, __pyx_n_s_mask, __pyx_n_s_prev_time, __pyx_n_s_name1, __pyx_n_s_name2); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(5, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmer_mapper_mapper_pyx, __pyx_n_s_read_fasta_into_chunks, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 65, __pyx_L1_error)
 
-  /* "mapper.pyx":221
+  /* "mapper.pyx":153
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def map_kmers_to_graph_index(index, int max_node_id, np.uint64_t[:] kmers, int max_index_lookup_frequency=1000):             # <<<<<<<<<<<<<<
  * 
  *     # index arrays
  */
-  __pyx_tuple__30 = PyTuple_Pack(24, __pyx_n_s_index, __pyx_n_s_max_node_id, __pyx_n_s_kmers, __pyx_n_s_max_index_lookup_frequency, __pyx_n_s_hashes_to_index_2, __pyx_n_s_n_kmers_2, __pyx_n_s_nodes_2, __pyx_n_s_ref_offsets_2, __pyx_n_s_index_kmers, __pyx_n_s_index_frequencies, __pyx_n_s_n_local_hits, __pyx_n_s_index_position, __pyx_n_s_l, __pyx_n_s_j, __pyx_n_s_i, __pyx_n_s_hash, __pyx_n_s_modulo_2, __pyx_n_s_node_counts, __pyx_n_s_t, __pyx_n_s_kmer_hashes, __pyx_n_s_n_collisions, __pyx_n_s_n_kmers_mapped, __pyx_n_s_n_skipped_high_frequency, __pyx_n_s_n_no_index_hits); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 221, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(4, 0, 24, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmer_mapper_mapper_pyx, __pyx_n_s_map_kmers_to_graph_index, 221, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(24, __pyx_n_s_index, __pyx_n_s_max_node_id, __pyx_n_s_kmers, __pyx_n_s_max_index_lookup_frequency, __pyx_n_s_hashes_to_index_2, __pyx_n_s_n_kmers_2, __pyx_n_s_nodes_2, __pyx_n_s_ref_offsets_2, __pyx_n_s_index_kmers, __pyx_n_s_index_frequencies, __pyx_n_s_n_local_hits, __pyx_n_s_index_position, __pyx_n_s_l, __pyx_n_s_j, __pyx_n_s_i, __pyx_n_s_hash, __pyx_n_s_modulo_2, __pyx_n_s_node_counts, __pyx_n_s_t, __pyx_n_s_kmer_hashes, __pyx_n_s_n_collisions, __pyx_n_s_n_kmers_mapped, __pyx_n_s_n_skipped_high_frequency, __pyx_n_s_n_no_index_hits); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(4, 0, 24, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmer_mapper_mapper_pyx, __pyx_n_s_map_kmers_to_graph_index, 153, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 153, __pyx_L1_error)
 
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 286, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(2, 291, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
 
   /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__37 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1000 = PyInt_FromLong(1000); if (unlikely(!__pyx_int_1000)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -23730,30 +22359,22 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6mapper___pyx_scope_struct__read_fasta) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6mapper___pyx_scope_struct__read_fasta.tp_print = 0;
-  #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6mapper___pyx_scope_struct__read_fasta.tp_dictoffset && __pyx_type_6mapper___pyx_scope_struct__read_fasta.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6mapper___pyx_scope_struct__read_fasta.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-  }
-  __pyx_ptype_6mapper___pyx_scope_struct__read_fasta = &__pyx_type_6mapper___pyx_scope_struct__read_fasta;
-  if (PyType_Ready(&__pyx_type_6mapper___pyx_scope_struct_1_read_fasta_into_chunks) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6mapper___pyx_scope_struct__read_fasta_into_chunks) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6mapper___pyx_scope_struct_1_read_fasta_into_chunks.tp_print = 0;
+  __pyx_type_6mapper___pyx_scope_struct__read_fasta_into_chunks.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6mapper___pyx_scope_struct_1_read_fasta_into_chunks.tp_dictoffset && __pyx_type_6mapper___pyx_scope_struct_1_read_fasta_into_chunks.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6mapper___pyx_scope_struct_1_read_fasta_into_chunks.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6mapper___pyx_scope_struct__read_fasta_into_chunks.tp_dictoffset && __pyx_type_6mapper___pyx_scope_struct__read_fasta_into_chunks.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_6mapper___pyx_scope_struct__read_fasta_into_chunks.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_6mapper___pyx_scope_struct_1_read_fasta_into_chunks = &__pyx_type_6mapper___pyx_scope_struct_1_read_fasta_into_chunks;
+  __pyx_ptype_6mapper___pyx_scope_struct__read_fasta_into_chunks = &__pyx_type_6mapper___pyx_scope_struct__read_fasta_into_chunks;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
   if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
@@ -24146,27 +22767,27 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "mapper.pyx":9
  * from kmer_mapper import util
  * cimport cython
  * import SharedArray as sa             # <<<<<<<<<<<<<<
  * from graph_kmer_index.shared_mem import to_shared_memory, SingleSharedArray
- * 
+ * import sys
  */
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_SharedArray, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_sa, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "mapper.pyx":10
  * cimport cython
  * import SharedArray as sa
  * from graph_kmer_index.shared_mem import to_shared_memory, SingleSharedArray             # <<<<<<<<<<<<<<
+ * import sys
  * 
- * def py_read_file(filename):
  */
   __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_to_shared_memory);
   __Pyx_GIVEREF(__pyx_n_s_to_shared_memory);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_to_shared_memory);
   __Pyx_INCREF(__pyx_n_s_SingleSharedArray);
@@ -24181,60 +22802,60 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_SingleSharedArray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_SingleSharedArray, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mapper.pyx":12
+  /* "mapper.pyx":11
+ * import SharedArray as sa
  * from graph_kmer_index.shared_mem import to_shared_memory, SingleSharedArray
+ * import sys             # <<<<<<<<<<<<<<
  * 
- * def py_read_file(filename):             # <<<<<<<<<<<<<<
- *     with open(filename, "r") as f:
- *         return f.read()
+ * def py_read_file(filename):
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6mapper_1py_read_file, NULL, __pyx_n_s_mapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_sys, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_read_file, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sys, __pyx_t_1) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mapper.pyx":56
- *         i_reverse_complement -= 1
+  /* "mapper.pyx":13
+ * import sys
  * 
- * def read_fasta(filename):             # <<<<<<<<<<<<<<
- *     filename_byte_string = filename.encode("UTF-8")
- *     cdef char * fname = filename_byte_string
+ * def py_read_file(filename):             # <<<<<<<<<<<<<<
+ *     with open(filename, "r") as f:
+ *         return f.read()
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6mapper_7read_fasta, NULL, __pyx_n_s_mapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6mapper_1py_read_file, NULL, __pyx_n_s_mapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_fasta, __pyx_t_1) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_read_file, __pyx_t_1) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mapper.pyx":90
+  /* "mapper.pyx":65
  * 
  * 
  * def read_fasta_into_chunks(filename, chunk_size=1000, int max_read_length=150, write_to_shared_memory=False, process_reads=False):             # <<<<<<<<<<<<<<
  *     logging.info("Reading fasta %s" % filename)
  *     filename_byte_string = filename.encode("UTF-8")
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6mapper_10read_fasta_into_chunks, NULL, __pyx_n_s_mapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6mapper_7read_fasta_into_chunks, NULL, __pyx_n_s_mapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_fasta_into_chunks, __pyx_t_1) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_fasta_into_chunks, __pyx_t_1) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mapper.pyx":221
+  /* "mapper.pyx":153
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def map_kmers_to_graph_index(index, int max_node_id, np.uint64_t[:] kmers, int max_index_lookup_frequency=1000):             # <<<<<<<<<<<<<<
  * 
  *     # index arrays
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6mapper_17map_kmers_to_graph_index, NULL, __pyx_n_s_mapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6mapper_10map_kmers_to_graph_index, NULL, __pyx_n_s_mapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_map_kmers_to_graph_index, __pyx_t_1) < 0) __PYX_ERR(0, 221, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_map_kmers_to_graph_index, __pyx_t_1) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "mapper.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
  * from libc.stdio cimport *
  * import numpy as np
  */
@@ -24259,71 +22880,71 @@
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 286, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 291, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":316
@@ -25033,41 +23654,154 @@
     }
 #ifdef WITH_THREAD
     if (nogil)
         PyGILState_Release(state);
 #endif
 }
 
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
+/* RaiseDoubleKeywords */
+static void __Pyx_RaiseDoubleKeywordsError(
+    const char* func_name,
+    PyObject* kw_name)
+{
+    PyErr_Format(PyExc_TypeError,
+        #if PY_MAJOR_VERSION >= 3
+        "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
+        #else
+        "%s() got multiple values for keyword argument '%s'", func_name,
+        PyString_AsString(kw_name));
+        #endif
+}
+
+/* ParseKeywords */
+static int __Pyx_ParseOptionalKeywords(
+    PyObject *kwds,
+    PyObject **argnames[],
+    PyObject *kwds2,
+    PyObject *values[],
+    Py_ssize_t num_pos_args,
+    const char* function_name)
+{
+    PyObject *key = 0, *value = 0;
+    Py_ssize_t pos = 0;
+    PyObject*** name;
+    PyObject*** first_kw_arg = argnames + num_pos_args;
+    while (PyDict_Next(kwds, &pos, &key, &value)) {
+        name = first_kw_arg;
+        while (*name && (**name != key)) name++;
+        if (*name) {
+            values[name-argnames] = value;
+            continue;
+        }
+        name = first_kw_arg;
+        #if PY_MAJOR_VERSION < 3
+        if (likely(PyString_Check(key))) {
+            while (*name) {
+                if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
+                        && _PyString_Eq(**name, key)) {
+                    values[name-argnames] = value;
+                    break;
+                }
+                name++;
+            }
+            if (*name) continue;
+            else {
+                PyObject*** argname = argnames;
+                while (argname != first_kw_arg) {
+                    if ((**argname == key) || (
+                            (CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**argname) == PyString_GET_SIZE(key))
+                             && _PyString_Eq(**argname, key))) {
+                        goto arg_passed_twice;
+                    }
+                    argname++;
+                }
+            }
+        } else
+        #endif
+        if (likely(PyUnicode_Check(key))) {
+            while (*name) {
+                int cmp = (**name == key) ? 0 :
+                #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                #endif
+                    PyUnicode_Compare(**name, key);
+                if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
+                if (cmp == 0) {
+                    values[name-argnames] = value;
+                    break;
+                }
+                name++;
+            }
+            if (*name) continue;
+            else {
+                PyObject*** argname = argnames;
+                while (argname != first_kw_arg) {
+                    int cmp = (**argname == key) ? 0 :
+                    #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                    #endif
+                        PyUnicode_Compare(**argname, key);
+                    if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
+                    if (cmp == 0) goto arg_passed_twice;
+                    argname++;
+                }
+            }
+        } else
+            goto invalid_keyword_type;
+        if (kwds2) {
+            if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
+        } else {
+            goto invalid_keyword;
+        }
     }
+    return 0;
+arg_passed_twice:
+    __Pyx_RaiseDoubleKeywordsError(function_name, key);
+    goto bad;
+invalid_keyword_type:
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() keywords must be strings", function_name);
+    goto bad;
+invalid_keyword:
+    PyErr_Format(PyExc_TypeError,
+    #if PY_MAJOR_VERSION < 3
+        "%.200s() got an unexpected keyword argument '%.200s'",
+        function_name, PyString_AsString(key));
+    #else
+        "%s() got an unexpected keyword argument '%U'",
+        function_name, key);
     #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
+bad:
+    return -1;
+}
+
+/* RaiseArgTupleInvalid */
+static void __Pyx_RaiseArgtupleInvalid(
+    const char* func_name,
+    int exact,
+    Py_ssize_t num_min,
+    Py_ssize_t num_max,
+    Py_ssize_t num_found)
+{
+    Py_ssize_t num_expected;
+    const char *more_or_less;
+    if (num_found < num_min) {
+        num_expected = num_min;
+        more_or_less = "at least";
+    } else {
+        num_expected = num_max;
+        more_or_less = "at most";
     }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
+    if (exact) {
+        more_or_less = "exactly";
+    }
+    PyErr_Format(PyExc_TypeError,
+                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                 func_name, more_or_less, num_expected,
+                 (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
@@ -25123,14 +23857,43 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
+/* PyObjectCall2Args */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args, *result = NULL;
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyFunction_FastCall(function, args, 2);
+    }
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyCFunction_FastCall(function, args, 2);
+    }
+    #endif
+    args = PyTuple_New(2);
+    if (unlikely(!args)) goto done;
+    Py_INCREF(arg1);
+    PyTuple_SET_ITEM(args, 0, arg1);
+    Py_INCREF(arg2);
+    PyTuple_SET_ITEM(args, 1, arg2);
+    Py_INCREF(function);
+    result = __Pyx_PyObject_Call(function, args, NULL);
+    Py_DECREF(args);
+    Py_DECREF(function);
+done:
+    return result;
+}
+
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
@@ -25282,156 +24045,14 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* RaiseDoubleKeywords */
-static void __Pyx_RaiseDoubleKeywordsError(
-    const char* func_name,
-    PyObject* kw_name)
-{
-    PyErr_Format(PyExc_TypeError,
-        #if PY_MAJOR_VERSION >= 3
-        "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
-        #else
-        "%s() got multiple values for keyword argument '%s'", func_name,
-        PyString_AsString(kw_name));
-        #endif
-}
-
-/* ParseKeywords */
-static int __Pyx_ParseOptionalKeywords(
-    PyObject *kwds,
-    PyObject **argnames[],
-    PyObject *kwds2,
-    PyObject *values[],
-    Py_ssize_t num_pos_args,
-    const char* function_name)
-{
-    PyObject *key = 0, *value = 0;
-    Py_ssize_t pos = 0;
-    PyObject*** name;
-    PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
-        name = first_kw_arg;
-        while (*name && (**name != key)) name++;
-        if (*name) {
-            values[name-argnames] = value;
-            continue;
-        }
-        name = first_kw_arg;
-        #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_Check(key))) {
-            while (*name) {
-                if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
-                        && _PyString_Eq(**name, key)) {
-                    values[name-argnames] = value;
-                    break;
-                }
-                name++;
-            }
-            if (*name) continue;
-            else {
-                PyObject*** argname = argnames;
-                while (argname != first_kw_arg) {
-                    if ((**argname == key) || (
-                            (CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**argname) == PyString_GET_SIZE(key))
-                             && _PyString_Eq(**argname, key))) {
-                        goto arg_passed_twice;
-                    }
-                    argname++;
-                }
-            }
-        } else
-        #endif
-        if (likely(PyUnicode_Check(key))) {
-            while (*name) {
-                int cmp = (**name == key) ? 0 :
-                #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
-                #endif
-                    PyUnicode_Compare(**name, key);
-                if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
-                if (cmp == 0) {
-                    values[name-argnames] = value;
-                    break;
-                }
-                name++;
-            }
-            if (*name) continue;
-            else {
-                PyObject*** argname = argnames;
-                while (argname != first_kw_arg) {
-                    int cmp = (**argname == key) ? 0 :
-                    #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
-                    #endif
-                        PyUnicode_Compare(**argname, key);
-                    if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
-                    if (cmp == 0) goto arg_passed_twice;
-                    argname++;
-                }
-            }
-        } else
-            goto invalid_keyword_type;
-        if (kwds2) {
-            if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
-        } else {
-            goto invalid_keyword;
-        }
-    }
-    return 0;
-arg_passed_twice:
-    __Pyx_RaiseDoubleKeywordsError(function_name, key);
-    goto bad;
-invalid_keyword_type:
-    PyErr_Format(PyExc_TypeError,
-        "%.200s() keywords must be strings", function_name);
-    goto bad;
-invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
-    #if PY_MAJOR_VERSION < 3
-        "%.200s() got an unexpected keyword argument '%.200s'",
-        function_name, PyString_AsString(key));
-    #else
-        "%s() got an unexpected keyword argument '%U'",
-        function_name, key);
-    #endif
-bad:
-    return -1;
-}
-
-/* RaiseArgTupleInvalid */
-static void __Pyx_RaiseArgtupleInvalid(
-    const char* func_name,
-    int exact,
-    Py_ssize_t num_min,
-    Py_ssize_t num_max,
-    Py_ssize_t num_found)
-{
-    Py_ssize_t num_expected;
-    const char *more_or_less;
-    if (num_found < num_min) {
-        num_expected = num_min;
-        more_or_less = "at least";
-    } else {
-        num_expected = num_max;
-        more_or_less = "at most";
-    }
-    if (exact) {
-        more_or_less = "exactly";
-    }
-    PyErr_Format(PyExc_TypeError,
-                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                 func_name, more_or_less, num_expected,
-                 (num_expected == 1) ? "" : "s", num_found);
-}
-
 /* SliceObject */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
         Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
         int has_cstart, int has_cstop, CYTHON_UNUSED int wraparound) {
 #if CYTHON_USE_TYPE_SLOTS
     PyMappingMethods* mp;
```

### Comparing `kmer_mapper-0.0.7/kmer_mapper/mapper.pyx` & `kmer_mapper-0.0.9/kmer_mapper/mapper.pyx`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 cimport numpy as np
 import logging
 import time
 from kmer_mapper import util
 cimport cython
 import SharedArray as sa
 from graph_kmer_index.shared_mem import to_shared_memory, SingleSharedArray
+import sys
 
 def py_read_file(filename):
     with open(filename, "r") as f:
         return f.read()
 
 cpdef test():
     print("test2")
@@ -49,40 +50,14 @@
             read_array[i] = 3
             reverse_complement_read_array[i_reverse_complement] = 1
         else:
             # invalid characters, like N, just keep these 0
             read_array[i] = 0
         i_reverse_complement -= 1
 
-def read_fasta(filename):
-    filename_byte_string = filename.encode("UTF-8")
-    cdef char * fname = filename_byte_string
-
-    cdef FILE * cfile
-    cfile = fopen(fname, "rb")
-    if cfile == NULL:
-        raise FileNotFoundError(2, "No such file or directory: '%s'" % filename)
-
-    cdef char * line = NULL
-    cdef size_t l = 0
-    cdef ssize_t read
-    cdef i = 0
-    while True:
-        i += 1
-        read = getline(&line, &l, cfile)
-        if read == -1: break
-
-        # skip header lines
-        if line[0] == 62:
-            continue
-
-        yield line
-
-    fclose(cfile)
-
 
 cdef void process_line(char* sequence, np.uint64_t[:] chunk_row, np.uint8_t[:] mask_row):
     cdef i = 0
     for i in range(0, len(sequence)-1):
         chunk_row[i] = sequence[i]
         mask_row[i] = True
 
@@ -102,17 +77,15 @@
     cdef ssize_t read
     cdef i = 0
     cdef int line_length = 0
 
     if process_reads:
         chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
     else:
-        #chunk = np.zeros((chunk_size, max_read_length), dtype=np.uint64)
         chunk = np.empty(chunk_size, dtype="|S" + str(max_read_length))  # max_read_length bytes for each element
-        #chunk = np.empty(chunk_size, dtype="<U" + str(max_read_length))
 
     mask = np.zeros((chunk_size, max_read_length),
                         dtype=np.bool)  # True where reads have bases (for handling short reads)
 
     prev_time = time.time()
 
     while True:
@@ -169,55 +142,14 @@
             to_shared_memory(SingleSharedArray(mask[0:i]), name2)
             yield name1, name2
         else:
             yield chunk[0:i], mask[0:i]
 
     fclose(cfile)
 
-cpdef handle_reads(filename):
-
-    cdef int sum_hashes = 0
-    cdef int max_read_length = 150
-    #cdef np.uint64_t[:] read_array = np.zeros(read_length, dtype=np.uint64)
-    cdef np.ndarray[np.uint64_t] read_array = np.zeros(max_read_length, dtype=np.uint64)
-    #cdef np.uint64_t[:] reverse_complement_read_array = np.zeros(read_length, dtype=np.uint64)
-    cdef np.ndarray[np.uint64_t] reverse_complement_read_array = np.zeros(max_read_length, dtype=np.uint64)
-    cdef int k = 31
-    cdef np.ndarray[np.int64_t] power_array = np.power(4, np.arange(0, k))
-    cdef int read_length
-    cdef int i = 0
-
-    #lines = util.read_fasta(filename)
-    #lines = util.read_fasta(filename)
-    lines = read_fasta(filename)
-    for line in lines:
-        read_length = len(line) - 3
-        read_sequence_to_kmer_hashes(line, read_array, reverse_complement_read_array, read_length)
-        sum_hashes += read_array[0]
-        kmers = np.convolve(read_array, power_array, mode='valid')
-        reverse_complement_kmers = np.convolve(reverse_complement_read_array, power_array, mode='valid')
-        sum_hashes += reverse_complement_read_array[10]
-
-        if i == 0:
-            print(kmers)
-
-        i += 1
-
-    print(sum_hashes)
-
-
-cdef read_file(filename):
-    cdef i = 0
-    result = read_fasta(filename)
-    return i
-
-
-cpdef get_count(filename):
-    return handle_reads(filename)
-
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def map_kmers_to_graph_index(index, int max_node_id, np.uint64_t[:] kmers, int max_index_lookup_frequency=1000):
 
     # index arrays
```

### Comparing `kmer_mapper-0.0.7/kmer_mapper/mapping.py` & `kmer_mapper-0.0.9/kmer_mapper/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from mapper import read_fasta_into_chunks, map_kmers_to_graph_index
 from kmer_mapper.util import remap_array, remap_array2
 from scipy.ndimage import convolve1d
 import pandas as pd
 import scipy.signal
 from graph_kmer_index import KmerIndex
-from graph_kmer_index.shared_mem import from_shared_memory, to_shared_memory, SingleSharedArray
+from shared_memory_wrapper import from_shared_memory, to_shared_memory, SingleSharedArray
 from pathos.multiprocessing import Pool
 from itertools import repeat
 
 def get_reads_as_matrices(read_file_name, chunk_size=500000, max_read_length=150):
     return (chunk for chunk in read_fasta_into_chunks(read_file_name, chunk_size, max_read_length))
```

### Comparing `kmer_mapper-0.0.7/kmer_mapper/util.py` & `kmer_mapper-0.0.9/kmer_mapper/util.py`

 * *Files identical despite different names*

### Comparing `kmer_mapper-0.0.7/setup.py` & `kmer_mapper-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,23 @@
               libraries=["m"],
               extra_compile_args = ["-O3", "-march=native"],
               )
       ]
 """
 
 setup(name='kmer_mapper',
-      version='0.0.7',
+      version='0.0.9',
       description='Kmer Mapper',
       url='http://github.com/ivargr/kmer_mapper',
       author='Ivar Grytten',
       author_email='',
       license='MIT',
       packages=["kmer_mapper"],
       zip_safe=False,
-      install_requires=['numpy', 'cython', 'graph_kmer_index', 'pathos', 'scipy', 'pandas'],
+      install_requires=['numpy', 'cython', 'graph_kmer_index', 'pathos', 'scipy', 'pandas', 'shared_memory_wrapper'],
       classifiers=[
             'Programming Language :: Python :: 3'
       ],
       entry_points={
             'console_scripts': ['kmer_mapper=kmer_mapper.command_line_interface:main']
       },
       cmdclass = {"build_ext": build_ext},
```

