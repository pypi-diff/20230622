# Comparing `tmp/pythontk-0.6.2.tar.gz` & `tmp/pythontk-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythontk-0.6.2.tar", last modified: Wed Mar 29 13:03:24 2023, max compression
+gzip compressed data, was "pythontk-0.6.4.tar", last modified: Thu Jun 22 16:14:27 2023, max compression
```

## Comparing `pythontk-0.6.2.tar` & `pythontk-0.6.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 13:03:24.652047 pythontk-0.6.2/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:38:48.000000 pythontk-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     1286 2023-03-29 13:03:24.652047 pythontk-0.6.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-29 13:03:24.633144 pythontk-0.6.2/pythontk/
--rw-rw-rw-   0        0        0     7429 2023-03-28 23:38:48.000000 pythontk-0.6.2/pythontk/Core.py
--rw-rw-rw-   0        0        0    14307 2023-03-28 23:38:48.000000 pythontk-0.6.2/pythontk/File.py
--rw-rw-rw-   0        0        0    24464 2023-03-28 23:38:48.000000 pythontk-0.6.2/pythontk/Img.py
--rw-rw-rw-   0        0        0    10864 2023-03-28 23:38:48.000000 pythontk-0.6.2/pythontk/Iter.py
--rw-rw-rw-   0        0        0     3707 2023-03-28 23:38:48.000000 pythontk-0.6.2/pythontk/Json.py
--rw-rw-rw-   0        0        0    15360 2023-03-28 23:38:48.000000 pythontk-0.6.2/pythontk/Math.py
--rw-rw-rw-   0        0        0    16355 2023-03-28 23:38:48.000000 pythontk-0.6.2/pythontk/Str.py
--rw-rw-rw-   0        0        0     6820 2023-03-29 13:03:22.000000 pythontk-0.6.2/pythontk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:03:24.651040 pythontk-0.6.2/pythontk.egg-info/
--rw-rw-rw-   0        0        0     1286 2023-03-29 13:03:24.000000 pythontk-0.6.2/pythontk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-03-29 13:03:24.000000 pythontk-0.6.2/pythontk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 13:03:24.000000 pythontk-0.6.2/pythontk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-29 13:03:24.000000 pythontk-0.6.2/pythontk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 13:03:24.653046 pythontk-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     2105 2023-03-28 23:38:48.000000 pythontk-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:14:27.119139 pythontk-0.6.4/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:38:48.000000 pythontk-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0     1286 2023-06-22 16:14:27.119139 pythontk-0.6.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 16:14:27.086134 pythontk-0.6.4/pythontk/
+-rw-rw-rw-   0        0        0     7133 2023-06-22 16:14:18.000000 pythontk-0.6.4/pythontk/__init__.py
+-rw-rw-rw-   0        0        0    25520 2023-06-06 01:08:03.000000 pythontk-0.6.4/pythontk/file_utils.py
+-rw-rw-rw-   0        0        0    29207 2023-06-06 18:19:16.000000 pythontk-0.6.4/pythontk/img_utils.py
+-rw-rw-rw-   0        0        0    16156 2023-06-06 18:19:16.000000 pythontk-0.6.4/pythontk/iter_utils.py
+-rw-rw-rw-   0        0        0    18312 2023-05-30 18:39:59.000000 pythontk-0.6.4/pythontk/math_utils.py
+-rw-rw-rw-   0        0        0    11452 2023-06-14 16:03:32.000000 pythontk-0.6.4/pythontk/misc_utils.py
+-rw-rw-rw-   0        0        0    25433 2023-06-14 21:04:19.000000 pythontk-0.6.4/pythontk/str_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:14:27.117135 pythontk-0.6.4/pythontk.egg-info/
+-rw-rw-rw-   0        0        0     1286 2023-06-22 16:14:26.000000 pythontk-0.6.4/pythontk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2023-05-20 13:28:19.000000 pythontk-0.6.4/pythontk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0      366 2023-06-22 16:14:26.000000 pythontk-0.6.4/pythontk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      265 2023-05-07 12:53:37.000000 pythontk-0.6.4/pythontk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-06-22 16:14:26.000000 pythontk-0.6.4/pythontk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 16:14:26.000000 pythontk-0.6.4/pythontk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 16:14:27.119139 pythontk-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     2212 2023-06-06 18:19:16.000000 pythontk-0.6.4/setup.py
```

### Comparing `pythontk-0.6.2/LICENSE` & `pythontk-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.2/PKG-INFO` & `pythontk-0.6.4/pythontk.egg-info/PKG-INFO.bak`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
 ```
 
 ### Example use-case:
 ###### Import the class `Iter` from the package.
 ###### As the name suggests, the class `Iter` holds the package's iterable related functions.
 ```python
 from pythontk import Iter
-Iter.filterList([0, 1, 2, 3, 2], [1, 2, 3], 2) #returns: [1, 3]
+Iter.filter_list([0, 1, 2, 3, 2], [1, 2, 3], 2) #returns: [1, 3]
 ```
 ###### You can also import a function directly.
 ```python
 from pythontk.Iter import filterDict
 filterDict({1:'1', 'two':2, 3:'three'}, exc='t*', keys=True) #returns: {1: '1', 3: 'three'}
 ```
```

### Comparing `pythontk-0.6.2/pythontk/Iter.py` & `pythontk-0.6.4/pythontk/misc_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,359 +1,296 @@
 # !/usr/bin/python
 # coding=utf-8
+import functools
+import inspect
+import collections.abc
+from typing import Any, Callable
+
+# from this package:
+from pythontk.iter_utils import Iter
+
+
+class Misc:
+    """ """
+
+    @staticmethod
+    def cached_property(func: Callable) -> Any:
+        """Decorator that converts a method with a single self argument into a property
+        that runs the method only once and stores the result, returning the stored
+        result on subsequent accesses.
+
+        This is useful for expensive computations that don't change once computed.
+
+        Parameters:
+            func: Method to be converted into a cached property.
+
+        Returns:
+            A descriptor object that can be used as a decorator.
+        """
+        from functools import wraps
+
+        attr_name = "_cached_" + func.__name__
+
+        @property
+        @wraps(func)
+        def _cached_property(self: Any) -> Any:
+            if not hasattr(self, attr_name):
+                setattr(self, attr_name, func(self))
+            return getattr(self, attr_name)
+
+        return _cached_property
+
+    @staticmethod
+    def listify(func=None, arg_name=None, threading=False):
+        if func is None:
+            return lambda func: Misc.listify(func, arg_name=arg_name)
+
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            func_args = inspect.getfullargspec(func).args
+            if "self" in func_args or "cls" in func_args:
+                func_args = func_args[1:]  # skip 'self' or 'cls' argument for methods
+
+            if arg_name and arg_name in func_args:
+                arg_index = func_args.index(arg_name)
+                if arg_index < len(args):
+                    # Argument is in the positional arguments
+                    arg = args[arg_index]
+                    args = args[:arg_index] + args[arg_index + 1 :]
+                else:
+                    raise ValueError(f"No argument named '{arg_name}' provided")
+            elif args:
+                arg_index = 0
+                arg = args[arg_index]
+                args = args[arg_index + 1 :]
+            else:
+                raise ValueError("No argument provided")
+
+            # Check if a single item was provided
+            single_item = not isinstance(arg, collections.abc.Iterable) or isinstance(
+                arg, (str, bytes, bytearray)
+            )
+
+            if single_item:
+                arg = [arg]
+
+            results = [
+                func(*(args[:arg_index] + (x,) + args[arg_index:]), **kwargs)
+                for x in arg
+            ]
+
+            # If a single item was provided, return a single result
+            if single_item:
+                return results[0]
+
+            return results
+
+        return wrapper
+
+    @classmethod
+    def format_return(cls, lst, orig=None):
+        """Return the list element if the given iterable only contains a single element.
+        If the list contains multiple elements, always return the full list.
+        If the 'orig' arg is a multi-element type then the original format will always be returned.
+
+        Parameters:
+                lst (list): An iterable.
+                orig (obj): Optionally; derive the return type form the original value.
+                                ie. if it was a multi-value type; do not modify the return value.
+        Returns:
+                (obj/list) dependant on flags.
+        """
+        orig_was_iter = isinstance(orig, (list, tuple, set, dict, range))
+
+        if (
+            len(lst) == 1
+            and not orig_was_iter
+            and not isinstance(lst, (str, bytes, bytearray))
+        ):
+            return lst[0]
+
+        return lst if orig_was_iter or len(lst) > 1 else None
+
+    @staticmethod
+    def set_attributes(obj, **attributes):
+        """Set attributes for a given object.
+
+        Parameters:
+                obj (obj): The object to set attributes for.
+                attributes (kwargs) = Attributes and their correponding values as keyword args.
+        """
+        [
+            setattr(obj, attr, value)
+            for attr, value in attributes.items()
+            if attr and value
+        ]
+
+    @staticmethod
+    def get_attributes(obj, inc=[], exc=[]):
+        """Get attributes for a given object.
+
+        Parameters:
+                obj (obj): The object to get the attributes of.
+                inc (list): Attributes to include. All other will be omitted. Exclude takes dominance over include. Meaning, if the same attribute is in both lists, it will be excluded.
+                exc (list): Attributes to exclude from the returned dictionay. ie. [u'Position',u'Rotation',u'Scale',u'renderable',u'isHidden',u'isFrozen',u'selected']
+
+        Returns:
+                (dict) {'string attribute': current value}
+        """
+        filtered = Iter.filter_list(obj.__dict__, inc, exc)
+        return {attr: getattr(obj, attr) for attr in filtered}
+
+    @staticmethod
+    def has_attribute(cls, attr):
+        """This function checks whether a class has a specific static attribute by using `inspect.getattr_static`.
+        It does not invoke the class's `__getattr__` method, so it is useful for checking if an attribute is defined
+        on the class itself, rather than on its instances.
+
+        Parameters:
+                cls (obj): The class to check for the attribute.
+                attr (str): The name of the attribute to check.
+
+        :return:
+                (bool) True if the class has the attribute, False otherwise.
+        """
+        import inspect
+
+        try:
+            inspect.getattr_static(cls, attr)
+            return True
+        except AttributeError:
+            return False
+
+    @staticmethod
+    def get_derived_type(
+        obj,
+        return_name=False,
+        module=None,
+        include=[],
+        exclude=[],
+        filter_by_base_type=False,
+    ):
+        """Get the base class of a custom object.
+        If the type is a standard object, the derived type will be that object's type.
+
+        Parameters:
+            obj (str/obj): Object or its objectName.
+            return_name (bool): Return the class or the class name.
+            module (str): The name of the base class module to check for.
+            include (list): Object types to include. All other will be omitted. Exclude takes dominance over include. Meaning, if the same attribute is in both lists, it will be excluded.
+            exclude (list): Object types to exclude.
+            filter_by_base_type (bool): When using `include`, or `exclude`; Filter by base class name, or derived class name.
+
+        Returns:
+            (obj)(string)(None) class or class name if `return_name`. ie. 'DerivedClass' from a custom object with class name: 'CustomClass'
+        """
+        for cls in obj.__class__.__mro__:
+            if (
+                not module
+                or cls.__module__ == module
+                or cls.__module__.split(".")[-1] == module
+            ):
+                derived_type = cls.__base__.__name__ if filter_by_base_type else cls
+                if not (
+                    derived_type in exclude
+                    and (
+                        derived_type in include
+                        if include
+                        else derived_type not in include
+                    )
+                ):
+                    return derived_type.__name__ if return_name else derived_type
+
+    CYCLEDICT = {}
+
+    @classmethod
+    def cycle(cls, sequence, name=None, query=False):
+        """Toggle between numbers in a given sequence.
+        Used for maintaining toggling sequences for multiple objects simultaniously.
+        Each time this function is called, it returns the next number in the sequence
+        using the name string as an identifier key.
+
+        Parameters:
+                sequence (list): sequence to cycle through. ie. [1,2,3].
+                name (str): identifier. used as a key to get the sequence value from the dict.
+
+        ex. cycle([0,1,2,3,4], 'componentID')
+        """
+        try:
+            if query:  # return the value without changing it.
+                return cls.CYCLEDICT[name][-1]  # get the current value ie. 0
+
+            value = cls.CYCLEDICT[
+                name
+            ]  # check if key exists. if so return the value. ie. value = [1,2,3]
+
+        except KeyError:  # else create sequence list for the given key
+            cls.CYCLEDICT[name] = [i for i in sequence]  # ie. {name:[1,2,3]}
+
+        value = cls.CYCLEDICT[name][0]  # get the current value. ie. 1
+        cls.CYCLEDICT[name] = cls.CYCLEDICT[name][1:] + [
+            value
+        ]  # move the current value to the end of the list. ie. [2,3,1]
+        return value  # return current value. ie. 1
+
+    @staticmethod
+    def are_similar(a, b, tolerance=0.0):
+        """Check if the two numberical values are within a given tolerance.
+        Supports nested lists.
+
+        Parameters:
+                a (obj)(tuple): The first object(s) to compare.
+                b (obj)(tuple): The second object(s) to compare.
+                tolerance (float) = The maximum allowed variation between the values.
+
+        Returns:
+                (bool)
+
+        Example: are_similar(1, 10, 9)" #returns: True
+        Example: are_similar(1, 10, 8)" #returns: False
+        """
+        func = (
+            lambda a, b: abs(a - b) <= tolerance
+            if isinstance(a, (int, float))
+            else True
+            if isinstance(a, (list, set, tuple)) and are_similar(a, b, tolerance)
+            else a == b
+        )
+        return all(map(func, Iter.make_iterable(a), Iter.make_iterable(b)))
+
+    @staticmethod
+    def randomize(lst, ratio=1.0):
+        """Random elements from the given list will be returned with a quantity determined by the given ratio.
+        A value of 0.5 will return 50% of the original elements in random order.
+
+        Parameters:
+                lst (tuple): A list to randomize.
+                ratio (float) = A value of 0.0-1. (default: 100%) With 0 representing 0% and
+                                1 representing 100% of the given elements returned in random order.
+        Returns:
+                (list)
+
+        Example: randomize(range(10), 1.0) #returns: [8, 4, 7, 6, 0, 5, 9, 1, 3, 2]
+        Example: randomize(range(10), 0.5) #returns: [7, 6, 4, 2, 8]
+        """
+        import random
+
+        lower, upper = 0.0, ratio if ratio <= 1 else 1.0  # end result range.
+        normalized = lower + (upper - lower) * len(lst)  # returns a float value.
+        randomized = random.sample(lst, int(normalized))
 
+        return randomized
 
-class Iter():
-	'''
-	'''
-	@staticmethod
-	def makeList(x):
-		'''Convert the given obj to a list.
-
-		Parameters:
-			x () = The object to convert to a list if not already a list, set, or tuple.
-
-		Return:
-			(list)
-		'''
-		return list(x) if isinstance(x, (list, tuple, set, dict, range)) else [x]
-
-
-	@classmethod
-	def nestedDepth(cls, lst, typ=(list, set, tuple)):
-		'''Get the maximum nested depth of any sub-lists of the given list.
-		If there is nothing nested, 0 will be returned.
-
-		Parameters:
-			lst (list): The list to check.
-			typ (type)(tuple): The type(s) to include in the query.
-
-		Return:
-			(int) 0 if none, else the max nested depth.
-		'''
-		d=-1
-		for i in lst:
-			if isinstance(i, typ):
-				d = max(cls.nestedDepth(i), d)
-		return d+1
-
-
-	@classmethod
-	def flatten(cls, lst):
-		'''Flatten arbitrarily nested lists.
-
-		Parameters:
-			lst (list): A list with potentially nested lists.
-
-		Return:
-			(generator)
-		'''
-		for i in lst:
-			if isinstance(i, (list, tuple, set)):
-				for ii in cls.flatten(i):
-					yield ii
-			else:
-				yield i
-
-
-	@staticmethod
-	def collapseList(lst, limit=None, compress=True, toString=True):
-		'''Convert a list of integers to a collapsed sequential string format.
-		ie. [19,22,23,24,25,26] to ['19', '22..26']
-
-		Parameters:
-			lst (list): A list of integers.
-			limit (int): limit the maximum length of the returned elements.
-			compress (bool): Trim redundant chars from the second half of a compressed set. ie. ['19', '22-32', '1225-6'] from ['19', '22..32', '1225..1226']
-			toString (bool): Return a single string value instead of a list.
-
-		Return:
-			(list)(str) string if 'toString'.
-		'''
-		ranges=[]
-		for x in map(str, lst): #make sure the list is made up of strings.
-			if not ranges:
-				ranges.append([x])
-			elif int(x)-prev_x==1:
-				ranges[-1].append(x)
-			else:
-				ranges.append([x])
-			prev_x = int(x)
-
-		if compress: #style: ['19', '22-32', '1225-6']
-			collapsedList = ['-'.join([r[0], r[-1][len(str(r[-1]))-len(str((int(r[-1])-int(r[0])))):]] #find the difference and use that value to further trim redundant chars from the string
-								if len(r) > 1 else r) 
-									for r in ranges]
-
-		else: #style: ['19', '22..32', '1225..1226']
-			collapsedList = ['..'.join([r[0], r[-1]] 
-								if len(r) > 1 else r) 
-									for r in ranges]
-
-		if limit and len(collapsedList)>limit:
-			l = collapsedList[:limit]
-			l.append('...')
-			collapsedList = l
-		
-		if toString:
-			collapsedList = ', '.join(collapsedList)
-
-		return collapsedList
-
-
-	@staticmethod
-	def bitArrayToList(bitArray):
-		'''Convert a binary bitArray to a python list.
-
-		Parameters:
-			bitArray () = A bit array or list of bit arrays.
-
-		Return:
-			(list) containing values of the indices of the on (True) bits.
-		'''
-		if len(bitArray):
-			if type(bitArray[0])!=bool: #if list of bitArrays: flatten
-				lst=[]
-				for array in bitArray:
-					lst.append([i+1 for i, bit in enumerate(array) if bit==1])
-				return [bit for array in lst for bit in array]
-
-			return [i+1 for i, bit in enumerate(bitArray) if bit==1]
-
-
-	@staticmethod
-	def rindex(itr, item):
-		'''Get the index of the first item to match the given item 
-		starting from the back (right side) of the list.
-
-		Parameters:
-			itr (iter): An iterable.
-			item () = The item to get the index of.
-
-		Return:
-			(int) -1 if element not found.
-		'''
-		return next(iter(i for i in range(len(itr)-1,-1,-1) if itr[i]==item), -1)
-
-
-	@staticmethod
-	def indices(itr, value):
-		'''Get the index of each element of a list matching the given value.
-
-		Parameters:
-			itr (iter): An iterable.
-			value () = The search value.
-
-		Return:
-			(generator)
-		'''
-		return (i for i, v in enumerate(itr) if v==value)
-
-
-	@staticmethod
-	def removeDuplicates(lst, trailing=True):
-		'''Remove all duplicated occurences while keeping the either the first or last.
-
-		Parameters:
-			lst (list): The list to remove duplicate elements of.
-			trailing (bool): Remove all trailing occurances while keeping the first, else keep last.
-
-		Return:
-			(list)
-		'''
-		if trailing:
-			return list(dict.fromkeys(lst))
-		else:
-			return list(dict.fromkeys(lst[::-1]))[::-1] #reverse the list when removing from the start of the list.
-
-
-	@classmethod
-	def filterDict(cls, dct, inc=[], exc=[], keys=False, values=False):
-		'''Filter the given dictionary.
-		Extends `filterList` to operate on either the given dict's keys or values.
-
-		Parameters:
-			dct (dict): The dictionary to filter.
-			inc (str)(obj)(list): The objects(s) to include.
-					supports using the '*' operator: startswith*, *endswith, *contains*
-					Will include all items that satisfy ANY of the given search terms.
-					meaning: '*.png' and '*Normal*' returns all strings ending in '.png' AND all 
-					strings containing 'Normal'. NOT strings satisfying both terms.
-			exc (str)(obj)(list): The objects(s) to exclude. Similar to include.
-					exlude take precidence over include.
-			keys (bool): Filter the dictionary keys.
-			values (bool): Filter the dictionary values.
-
-		Return:
-			(dict)
-
-		Example: dct = {1:'1', 'two':2, 3:'three'}
-		filterDict(dct, exc='*t*', values=True) #returns: {1: '1', 'two': 2}
-		filterDict(dct, exc='t*', keys=True) #returns: {1: '1', 3: 'three'}
-		filterDict(dct, exc=1, keys=True) #returns: {'two': 2, 3: 'three'}
-		'''
-		if keys:
-			filtered = cls.filterList(dct.keys(), inc, exc)
-			dct = {k: dct[k] for k in filtered}
-		if values:
-			filtered = cls.filterList(dct.values(), inc, exc)
-			dct = {k:v for k,v in dct.items() if v in filtered}
-		return dct
-
-
-	@classmethod
-	def filterList(cls, lst, inc=[], exc=[]):
-		'''Filter the given list.
-
-		Parameters:
-			lst (list): The components(s) to filter.
-			inc (str)(int)(obj)(list): The objects(s) to include.
-					supports using the '*' operator: startswith*, *endswith, *contains*
-					Will include all items that satisfy ANY of the given search terms.
-					meaning: '*.png' and '*Normal*' returns all strings ending in '.png' AND all 
-					strings containing 'Normal'. NOT strings satisfying both terms.
-			exc (str)(int)(obj)(list): The objects(s) to exclude. Similar to include.
-					exlude take precidence over include.
-		Return:
-			(list)
-
-		Example: filterList([0, 1, 2, 3, 2], [1, 2, 3], 2) #returns: [1, 3]
-		'''
-		exc = cls.makeList(exc)
-		inc = cls.makeList(inc)
-
-		if not any((i for i in inc+exc if isinstance(i, str) and '*' in i)): #if no wildcards used:
-			return [i for i in lst if not i in exc and (i in inc if inc else i not in inc)]
-
-		#else: split `inc` and `exc` lists into separate tuples according to wildcard positions. 
-		if exc:
-			exc_, excContains, excStartsWith, excEndsWith = [],[],[],[]
-			for i in exc:
-				if isinstance(i, str) and '*' in i:
-					if i.startswith('*'):
-						if i.endswith('*'):
-							excContains.append(i[1:-1])
-						excEndsWith.append(i[1:])
-					elif i.endswith('*'):
-						excStartsWith.append(i[:-1])
-				else:
-					exc_.append(i)
-		if inc:
-			inc_, incContains, incStartsWith, incEndsWith = [],[],[],[]
-			for i in inc:
-				if isinstance(i, str) and '*' in i:
-					if i.startswith('*'):
-						if i.endswith('*'):
-							incContains.append(i[1:-1])
-						incEndsWith.append(i[1:])
-					elif i.endswith('*'):
-						incStartsWith.append(i[:-1])
-				else:
-					inc_.append(i)
-
-		result=[]
-		for i in lst:
-
-			if exc:
-				if i in exc_ or isinstance(i, str) and any((
-					i.startswith(tuple(excStartsWith)),
-					i.endswith(tuple(excEndsWith)),
-					next(iter(chars in i for chars in excContains), False))):
-					continue
-
-			if inc:
-				if i not in inc_ and not (isinstance(i, str) and any(( 
-					i.startswith(tuple(incStartsWith)), 
-					i.endswith(tuple(incEndsWith)), 
-					next(iter(chars in i for chars in incContains), False)))):
-					continue
-
-			result.append(i)
-		return result
-
-
-	@staticmethod
-	def splitList(lst, into):
-		'''Split a list into parts.
-
-		Parameters:
-			into (str): Split the list into parts defined by the following:
-				'<n>parts' - Split the list into n parts.
-					ex. 2 returns:  [[1, 2, 3, 5], [7, 8, 9]] from [1,2,3,5,7,8,9]
-				'<n>parts+' - Split the list into n equal parts with any trailing remainder.
-					ex. 2 returns:  [[1, 2, 3], [5, 7, 8], [9]] from [1,2,3,5,7,8,9]
-				'<n>chunks' - Split into sublists of n size.
-					ex. 2 returns: [[1,2], [3,5], [7,8], [9]] from [1,2,3,5,7,8,9]
-				'contiguous' - The list will be split by contiguous numerical values.
-					ex. 'contiguous' returns: [[1,2,3], [5], [7,8,9]] from [1,2,3,5,7,8,9]
-				'range' - The values of 'contiguous' will be limited to the high and low end of each range.
-					ex. 'range' returns: [[1,3], [5], [7,9]] from [1,2,3,5,7,8,9]
-		Return:
-			(list)
-		'''
-		from string import digits, ascii_letters, punctuation
-		mode = into.lower().lstrip(digits)
-		digit = into.strip(ascii_letters+punctuation)
-		n = int(digit) if digit else None
-
-		if n:
-			if mode=='parts':
-				n = len(lst)*-1 // n*-1 #ceil
-			elif mode=='parts+':
-				n = len(lst) // n
-			return [lst[i:i+n] for i in range(0, len(lst), n)]
-
-		elif mode=='contiguous' or mode=='range':
-			from itertools import groupby
-			from operator import itemgetter
-
-			try:
-				contiguous = [list(map(itemgetter(1), g)) for k, g in groupby(enumerate(lst), lambda x: int(x[0])-int(x[1]))]
-			except ValueError as error:
-				print ('{} in splitList\n\t# Error: {} #\n\t{}'.format(__file__, error, lst))
-				return lst
-			if mode=='range':
-				return [[i[0], i[-1]] if len(i)>1 else (i) for i in contiguous]
-			return contiguous
 
 # --------------------------------------------------------------------------------------------
 
-
-
-
-
-
-
-
+if __name__ == "__main__":
+    pass
 
 # --------------------------------------------------------------------------------------------
-
-def __getattr__(attr:str):
-	"""Searches for an attribute in this module's classes and returns it.
-
-	Parameters:
-		attr (str): The name of the attribute to search for.
-	
-	Return:
-		(obj) The found attribute.
-
-	:Raises:
-		AttributeError: If the given attribute is not found in any of the classes in the module.
-	"""
-	try:
-		return getattr(Iter, attr)
-
-	except AttributeError as error:
-		raise AttributeError(f"Module '{__name__}' has no attribute '{attr}'")
-
+# Notes
 # --------------------------------------------------------------------------------------------
 
-if __name__=='__main__':
-	pass
 
 # --------------------------------------------------------------------------------------------
-# Notes
+# deprecated:
 # --------------------------------------------------------------------------------------------
-
-
-
-# Deprecated ------------------------------------
```

### Comparing `pythontk-0.6.2/pythontk/Math.py` & `pythontk-0.6.4/pythontk/math_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,527 +1,496 @@
 # !/usr/bin/python
 # coding=utf-8
-from pythontk.Core import listify
-
-
-class Math():
-	'''
-	'''
-	@staticmethod
-	def getVectorFromTwoPoints(startPoint, endPoint):
-		'''Get a directional vector from a given start and end point.
-
-		Parameters:
-			startPoint (tuple): A start point given as (x,y,z).
-			endPoint (tuple): An end point given as (x,y,z).
-
-		Return:
-			(tuple) vector.
-
-		Example: getVectorFromTwoPoints((1, 2, 3), (1, 1, -1)) #returns: (0, -1, -4)
-		'''
-		ax, ay, az = startPoint
-		bx, by, bz = endPoint
-
-		return (bx - ax, by - ay, bz - az)
-
-
-	@staticmethod
-	@listify
-	def clamp(n=0.0, minimum=0.0, maximum=1.0):
-		'''Clamps the value x between min and max.
-
-		Parameters:
-			n (float)(tuple): The numeric value to clamp.
-			minimum (float) = Clamp min value.
-			maximum (float) = Clamp max value.
-
-		Return:
-			(float)
-
-		Example: clamp(range(10), 3, 7) #returns: [3, 3, 3, 3, 4, 5, 6, 7, 7, 7]
-		'''
-		return max(minimum, min(n, maximum))
-
-
-	@classmethod
-	def normalize(cls, vector, amount=1):
-		'''Normalize a 2 or 3 dimensional vector.
-
-		Parameters:
-			vector (tuple): A two or three point vector. ie. (-0.03484, 0.0, -0.55195)
-			amount (float) = (1) Normalize standard. (value other than 0 or 1) Normalize using the given float value as desired length.
-
-		Return:
-			(tuple)
-
-		Example: normalize((2, 3, 4)) #returns: (0.3713906763541037, 0.5570860145311556, 0.7427813527082074)
-		Example: normalize((2, 3)) #returns: (0.5547001962252291, 0.8320502943378437)
-		Example: normalize((2, 3, 4), 2) #returns: (0.7427813527082074, 1.1141720290623112, 1.4855627054164149)
-		'''
-		n = len(vector) #determine 2 or 3d vector.
-		length = cls.getMagnitude(vector)
-		return tuple(vector[i] / length * amount for i in range(n))
-
-
-	@staticmethod
-	def getMagnitude(vector):
-		'''Get the magnatude (length) of a given vector.
-
-		Parameters:
-			vector (tuple): A two or three point vector. ie. (-0.03484, 0.0, -0.55195)
-
-		Return:
-			(float)
-
-		Example: getMagnitude((2, 3, 4)) #returns: 5.385164807134504
-		Example: getMagnitude((2, 3)) #returns: 3.605551275463989
-		'''
-		from math import sqrt
-
-		n = len(vector) #determine 2 or 3d vector.
-		return sqrt(sum(vector[i] * vector[i] for i in range(n)))
-
-
-	@classmethod
-	def dotProduct(cls, v1, v2, normalizeInputs=False):
-		'''Returns the dot product of two 3D float arrays.  If $normalizeInputs
-		is set then the vectors are normalized before the dot product is calculated.
-
-		Parameters:
-			v1 (tuple): The first 3 point vector. 
-			v2 (tuple): The second 3 point vector.
-			normalizeInputs (int): Normalize v1, v2 before calculating the point float list.
-
-		Return:
-			(float) Dot product of the two vectors.
-
-		Example: dotProduct((1, 2, 3), (1, 1, -1)) #returns: 0
-		Example: dotProduct((1, 2), (1, 1)) #returns: 3
-		'''
-		if normalizeInputs: #normalize the input vectors
-			v1 = cls.normalize(v1)
-			v2 = cls.normalize(v2)
-
-		return sum((a*b) for a, b in zip(v1, v2)) #the dot product
-
-
-	@classmethod
-	def crossProduct(cls, a, b, c=None, normalize=0):
-		'''Get the cross product of two vectors, using two 3d vectors, or 3 points.
-
-		Parameters:
-			a (tuple): A point represented as x,y,z or a 3 point vector.
-			b (tuple): A point represented as x,y,z or a 3 point vector.
-			c (tuple): A point represented as x,y,z (used only when working with 3 point values instead of 2 vectors).
-			normalize (float) = (0) Do not normalize. (1) Normalize standard. (value other than 0 or 1) Normalize using the given float value as desired length.
-
-		Return:
-			(tuple)
-
-		Example: crossProduct((1, 2, 3), (1, 1, -1)) #returns: (-5, 4, -1),
-		Example: crossProduct((3, 1, 1), (1, 4, 2), (1, 3, 4)) #returns: (7, 4, 2),
-		Example: crossProduct((1, 2, 3), (1, 1, -1), None, 1) #returns: (-0.7715167498104595, 0.6172133998483676, -0.1543033499620919)
-		'''
-		if c is not None: #convert points to vectors and unpack.
-			a = cls.getVectorFromTwoPoints(a, b)
-			b = cls.getVectorFromTwoPoints(b, c)
-
-		ax, ay, az = a
-		bx, by, bz = b
-
-		result = (
-			(ay*bz) - (az*by), 
-			(az*bx) - (ax*bz), 
-			(ax*by) - (ay*bx)
-		)
-
-		if normalize:
-			result = cls.normalize(result, normalize)
-
-		return result
-
-
-	@classmethod
-	def movePointRelative(cls, p, d, v=None):
-		'''Move a point relative to it's current position.
-
-		Parameters:
-			p (tuple): A points x, y, z values.
-			d (tuple)(float) = The distance to move. Use a float value when moving along a vector, 
-						and a point value to move in a given distance.
-			v (tuple): Optional: A vectors x, y, z values can be given to move the point along that vector.
-
-		Return:
-			(tuple) point.
-
-		Example: movePointRelative((0, 5, 0), (0, 5, 0)) #returns: (0, 10, 0)
-		Example: movePointRelative((0, 5, 0), 5, (0, 1, 0)) #returns: (0, 10, 0)
-		'''
-		x, y, z = p
-
-		if v is not None: #move along a vector if one is given.
-			assert isinstance(d, (float, int)), '# Error: {}\n  The distance parameter requires an integer or float value when moving along a vector.\n  {} {} given. #'.format(__file__, type(d), d)
-			dx, dy, dz = cls.normalize(v, d)
-		else:
-			assert isinstance(d, (list, tuple, set)), '# Error: {}\n  The distance parameter requires an list, tuple, set value when not moving along a vector.\n  {} {} given. #'.format(__file__, type(d), d)
-			dx, dy, dz = d
-
-		result = (
-			x + dx,
-			y + dy,
-			z + dz
-		)
-
-		return result
-
-
-	@classmethod
-	def movePointAlongVectorRelativeToPoint(cls, p1, p2, vect, dist, toward=True):
-		'''Move a point (p1) along a given vector toward or away from a given point (p2).
-
-		Parameters:
-			p1 (tuple): The point to move given as (x,y,z).
-			p2 (tuple): The point to move toward.
-			vect (tuple): A vector to move the point along.
-			dist (float) = The linear amount to move the point.
-			toward (bool): Move the point toward or away from.
-		
-		Return:
-			(tuple) point.
-
-		Example: movePointAlongVectorRelativeToPoint((0, 0, 0), (0, 10, 0), (0, 1, 0), 5) #returns: (0.0, 5.0, 0.0)
-		Example: movePointAlongVectorRelativeToPoint((0, 0, 0), (0, 10, 0), (0, 1, 0), 5, False) #returns: (0.0, -15.0, 0.0)
-		'''
-		lowest=None
-		for i in [dist, -dist]: #move in pos and neg direction, and determine which is moving closer to the reference point.
-			p = cls.movePointRelative(p1, i, vect)
-			d = cls.getDistBetweenTwoPoints(p, p2)
-			if lowest is None or (d<lowest if toward else d>lowest):
-				result, lowest = (p, d)
-
-		return result
-
-
-	@classmethod
-	def getDistBetweenTwoPoints(cls, p1, p2):
-		'''Get the vector between two points, and return it's magnitude.
-
-		Parameters:
-			p1 (tuple): A point given as (x,y,z).
-			p2 (tuple): A point given as (x,y,z).
-
-		Return:
-			(float)
-
-		Example: getDistBetweenTwoPoints((0, 10, 0), (0, 5, 0)) #returns: 5.0
-		'''
-		from math import sqrt
-		
-		p1x, p1y, p1z = p1
-		p2x, p2y, p2z = p2
-
-		vX = p1x - p2x
-		vY = p1y - p2y
-		vZ = p1z - p2z
-
-		vector = (vX, vY, vZ)
-		length = cls.getMagnitude(vector)
-
-		return length
-
-
-	@staticmethod
-	def getCenterPointBetweenTwoPoints(p1, p2):
-		'''Get the point in the middle of two given points.
-
-		Parameters:
-			p1 (tuple): A point given as (x,y,z).
-			p2 (tuple): A point given as (x,y,z).
-
-		Return:
-			(tuple)
-
-		Example: getCenterPointBetweenTwoPoints((0, 10, 0), (0, 5, 0)) #returns: (0.0, 7.5, 0.0)
-		'''
-		Ax, Ay, Az = p1
-		Bx, By, Bz = p2
-
-		result = (
-			(Ax+Bx) /2,
-			(Ay+By) /2,
-			(Az+Bz) /2
-		)
-
-		return result
-
-
-	@classmethod
-	def getAngleFrom2Vectors(cls, v1, v2, degree=False):
-		'''Get an angle from two given vectors.
-
-		Parameters:
-			v1 (tuple): A vectors xyz values as a tuple.
-			v2 (tuple): A vectors xyz values as a tuple.
-			degree (bool): Convert the radian result to degrees.
-
-		Return:
-			(float)
-
-		Example: getAngleFrom2Vectors((1, 2, 3), (1, 1, -1)) #returns: 1.5707963267948966,
-		Example: getAngleFrom2Vectors((1, 2, 3), (1, 1, -1), True) #returns: 90
-		'''
-		from math import acos, degrees
-
-		def length(v):
-			return (cls.dotProduct(v, v))**0.5
-
-		result = acos(cls.dotProduct(v1, v2) / (length(v1) * length(v2)))
-
-		if degree:
-			result = round(degrees(result), 2)
-		return result
-
-
-	@staticmethod
-	def getAngleFrom3Points(a, b, c, degree=False):
-		'''Get the opposing angle from 3 given points.
-
-		Parameters:
-			a (tuple): A point given as (x,y,z).
-			b (tuple): A point given as (x,y,z).
-			c (tuple): A point given as (x,y,z).
-			degree (bool): Convert the radian result to degrees.
-
-		Return:
-			(float)
-
-		Example: getAngleFrom3Points((1, 1, 1), (-1, 2, 3), (1, 4, -3)) #returns: 0.7904487543360762,
-		Example: getAngleFrom3Points((1, 1, 1), (-1, 2, 3), (1, 4, -3), True) #returns: 45.29
-		'''
-		from math import sqrt, acos, degrees
-
-		ba = [aa-bb for aa,bb in zip(a,b)] #create vectors from points
-		bc = [cc-bb for cc,bb in zip(c,b)]
-
-		nba = sqrt(sum((x**2.0 for x in ba))) #normalize vector
-		ba = [x/nba for x in ba]
-
-		nbc = sqrt(sum((x**2.0 for x in bc)))
-		bc = [x/nbc for x in bc]
-
-		scalar = sum((aa*bb for aa,bb in zip(ba,bc))) #get scalar from normalized vectors
-
-		angle = acos(scalar)#get the angle in radian
-
-		if degree:
-			angle = round(degrees(angle), 2)
-		return angle
-
-
-	@staticmethod
-	def getTwoSidesOfASATriangle(a1, a2, s, unit='degrees'):
-		'''Get the length of two sides of a triangle, given two angles, and the length of the side in-between.
-
-		Parameters:
-			a1 (float) = Angle in radians or degrees. (unit flag must be set if value given in radians)
-			a2 (float) = Angle in radians or degrees. (unit flag must be set if value given in radians)
-			s (float) = The distance of the side between the two given angles.
-			unit (str): Specify whether the angle values are given in degrees or radians. (valid: 'radians', 'degrees')(default: degrees)
-
-		Return:
-			(tuple)
-
-		Example: getTwoSidesOfASATriangle(60, 60, 100) #returns: (100.00015320566493, 100.00015320566493)
-		'''
-		from math import sin, radians
-
-		if unit=='degrees':
-			a1, a2 = radians(a1), radians(a2)
-
-		a3 = 3.14159 - a1 - a2
-
-		result = (
-			(s/sin(a3)) * sin(a1),
-			(s/sin(a3)) * sin(a2)
-		)
-
-		return result
-
-
-	@classmethod
-	def xyzRotation(cls, theta, axis, rotation=[], degree=False):
-		'''Get the rotation about the X,Y,Z axes (in rotation) given 
-		an angle for rotation (in radians) and an axis about which to 
-		do the rotation.
-
-		Parameters:
-			theta (float) = The angular position of a vector in radians.
-			axis (tuple): The rotation axis given as float values (x,y,z).
-			rotation (list): 
-			degree (bool): Convert the radian result to degrees.
-
-		Return:
-			(tuple) 3 point rotation.
-
-		Example: xyzRotation(2, (0, 1, 0)) #returns: [3.589792907376932e-09, 1.9999999964102069, 3.589792907376932e-09]
-		Example: xyzRotation(2, (0, 1, 0), [], True) #returns: [0.0, 114.59, 0.0]
-		'''
-		from math import cos, sin, sqrt, atan2, degrees
-
-		#set up the xyzw quaternion values
-		theta *= 0.5
-		w = cos(theta)
-		factor = sin(theta)
-		axisLen2 = cls.dotProduct(axis, axis, 0)
-
-		if (axisLen2 != 1.0 and axisLen2 != 0.0):
-			factor /= sqrt(axisLen2)
-		x, y, z = factor * axis[0], factor * axis[1], factor * axis[2]
-
-		#setup rotation in a matrix
-		ww, xx, yy, zz = w*w, x*x, y*y, z*z
-		s = 2.0 / (ww + xx + yy + zz)
-		xy, xz, yz, wx, wy, wz = x*y, x*z, y*z, w*x, w*y, w*z
-		matrix = [
-			1.0 - s * (yy + zz),
-			s * (xy + wz),
-			s * (xz - wy),
-			None, None,
-			1.0 - s * (xx + zz),
-			s * (yz + wx),
-			None, None,
-			s * (yz - wx),
-			1.0 - s * (xx + yy)
-		]
-
-		#get x,y,z values for rotation
-		cosB = sqrt(matrix[0]*matrix[0] + matrix[1]*matrix[1])
-		if (cosB > 1.0e-10):
-			pi = 3.14159265
-	 
-			a, b, c = solution1 = [
-				atan2(matrix[6], matrix[10]),
-				atan2(-matrix[2], cosB),
-				atan2(matrix[1], matrix[0])
-			]
-
-			solution2 = [
-				a + (pi if a < pi else -pi),
-				(pi if b > -pi else -pi) - b,
-				c + (pi if c < pi else -pi)
-			]
-
-			if sum([abs(solution2[0]), abs(solution2[1]), abs(solution2[2])]) < sum([abs(solution1[0]), abs(solution1[1]), abs(solution1[2])]):
-
-				rotation = solution2
-			else:
-				rotation = solution1
-
-		else:
-			rotation = [
-				atan2(-matrix[9], matrix[5]),
-				atan2(-matrix[2], cosB),
-				0.0
-			]
-
-		if degree:
-			rotation = [round(degrees(r), 2) for r in rotation]
-		return tuple(rotation)
-
-# --------------------------------------------------------------------------------------------
-
-
-
+from typing import List, Tuple
 
+# from this package:
+from pythontk.misc_utils import Misc
 
 
+class Math:
+    """ """
 
+    @staticmethod
+    @Misc.listify(threading=True)
+    def move_decimal_point(num, places):
+        """Move the decimal place in a given number.
+
+        Parameters:
+                num (int/float): The number in which you are modifying.
+                places (int): The number of decimal places to move.
+
+        Returns:
+                (float)
+
+        Example:
+                move_decimal_point(11.05, -2) #returns: 0.1105
+        """
+        from decimal import Decimal
+
+        num_decimal = Decimal(str(num))  # Convert the input number to a Decimal object
+        scaling_factor = Decimal(
+            10**places
+        )  # Create a scaling factor as a Decimal object
+
+        result = (
+            num_decimal * scaling_factor
+        )  # Perform the operation using Decimal objects
+        return float(result)  # Convert the result back to a float
+
+    @staticmethod
+    def get_vector_from_two_points(
+        a: List[float], b: List[float]
+    ) -> Tuple[float, float, float]:
+        """Get a directional vector from a given start and end point.
+
+        Parameters:
+                a (List[float]): A start point given as [x, y, z].
+                b (List[float]): An end point given as [x, y, z].
+
+        Returns:
+                Tuple[float, float, float]: The directional vector from the start point to the end point.
+
+        Example:
+                get_vector_from_two_points([1, 2, 3], [1, 1, -1]) #returns: (0, -1, -4)
+        """
+        return (b[0] - a[0], b[1] - a[1], b[2] - a[2])
+
+    @staticmethod
+    @Misc.listify(threading=True)
+    def clamp(n=0.0, minimum=0.0, maximum=1.0):
+        """Clamps the value x between min and max.
+
+        Parameters:
+                n (float)(tuple): The numeric value to clamp.
+                minimum (float) = Clamp min value.
+                maximum (float) = Clamp max value.
+
+        Returns:
+                (float)
+
+        Example: clamp(range(10), 3, 7) #returns: [3, 3, 3, 3, 4, 5, 6, 7, 7, 7]
+        """
+        return max(minimum, min(n, maximum))
+
+    @classmethod
+    def normalize(cls, vector, amount=1):
+        """Normalize a 2 or 3 dimensional vector.
+
+        Parameters:
+                vector (tuple): A two or three point vector. ie. (-0.03484, 0.0, -0.55195)
+                amount (float) = (1) Normalize standard. (value other than 0 or 1) Normalize using the given float value as desired length.
+
+        Returns:
+                (tuple)
+
+        Example: normalize((2, 3, 4)) #returns: (0.3713906763541037, 0.5570860145311556, 0.7427813527082074)
+        Example: normalize((2, 3)) #returns: (0.5547001962252291, 0.8320502943378437)
+        Example: normalize((2, 3, 4), 2) #returns: (0.7427813527082074, 1.1141720290623112, 1.4855627054164149)
+        """
+        n = len(vector)  # determine 2 or 3d vector.
+        length = cls.get_magnitude(vector)
+        return tuple(vector[i] / length * amount for i in range(n))
+
+    @staticmethod
+    def get_magnitude(vector):
+        """Get the magnatude (length) of a given vector.
+
+        Parameters:
+                vector (tuple): A two or three point vector. ie. (-0.03484, 0.0, -0.55195)
+
+        Returns:
+                (float)
+
+        Example: get_magnitude((2, 3, 4)) #returns: 5.385164807134504
+        Example: get_magnitude((2, 3)) #returns: 3.605551275463989
+        """
+        from math import sqrt
+
+        n = len(vector)  # determine 2 or 3d vector.
+        return sqrt(sum(vector[i] * vector[i] for i in range(n)))
+
+    @classmethod
+    def dot_product(cls, v1, v2, normalize_input=False):
+        """Returns the dot product of two 3D float arrays.  If $normalize_input
+        is set then the vectors are normalized before the dot product is calculated.
+
+        Parameters:
+                v1 (tuple): The first 3 point vector.
+                v2 (tuple): The second 3 point vector.
+                normalize_input (int): Normalize v1, v2 before calculating the point float list.
+
+        Returns:
+                (float) Dot product of the two vectors.
+
+        Example: dot_product((1, 2, 3), (1, 1, -1)) #returns: 0
+        Example: dot_product((1, 2), (1, 1)) #returns: 3
+        """
+        if normalize_input:  # normalize the input vectors
+            v1 = cls.normalize(v1)
+            v2 = cls.normalize(v2)
+
+        return sum((a * b) for a, b in zip(v1, v2))  # the dot product
+
+    @classmethod
+    def cross_product(cls, a, b, c=None, normalize=0):
+        """Get the cross product of two vectors, using two 3d vectors, or 3 points.
+
+        Parameters:
+                a (tuple): A point represented as x,y,z or a 3 point vector.
+                b (tuple): A point represented as x,y,z or a 3 point vector.
+                c (tuple): A point represented as x,y,z (used only when working with 3 point values instead of 2 vectors).
+                normalize (float) = (0) Do not normalize. (1) Normalize standard. (value other than 0 or 1) Normalize using the given float value as desired length.
+
+        Returns:
+                (tuple)
+
+        Example: cross_product((1, 2, 3), (1, 1, -1)) #returns: (-5, 4, -1),
+        Example: cross_product((3, 1, 1), (1, 4, 2), (1, 3, 4)) #returns: (7, 4, 2),
+        Example: cross_product((1, 2, 3), (1, 1, -1), None, 1) #returns: (-0.7715167498104595, 0.6172133998483676, -0.1543033499620919)
+        """
+        if c is not None:  # convert points to vectors and unpack.
+            a = cls.get_vector_from_two_points(a, b)
+            b = cls.get_vector_from_two_points(b, c)
+
+        ax, ay, az = a
+        bx, by, bz = b
+
+        result = ((ay * bz) - (az * by), (az * bx) - (ax * bz), (ax * by) - (ay * bx))
+
+        if normalize:
+            result = cls.normalize(result, normalize)
+
+        return result
+
+    @classmethod
+    def move_point_relative(cls, p, d, v=None):
+        """Move a point relative to it's current position.
+
+        Parameters:
+                p (tuple): A points x, y, z values.
+                d (tuple)(float) = The distance to move. Use a float value when moving along a vector,
+                                        and a point value to move in a given distance.
+                v (tuple): Optional: A vectors x, y, z values can be given to move the point along that vector.
+
+        Returns:
+                (tuple) point.
+
+        Example: move_point_relative((0, 5, 0), (0, 5, 0)) #returns: (0, 10, 0)
+        Example: move_point_relative((0, 5, 0), 5, (0, 1, 0)) #returns: (0, 10, 0)
+        """
+        x, y, z = p
+
+        if v is not None:  # move along a vector if one is given.
+            assert isinstance(
+                d, (float, int)
+            ), "# Error: {}\n  The distance parameter requires an integer or float value when moving along a vector.\n  {} {} given. #".format(
+                __file__, type(d), d
+            )
+            dx, dy, dz = cls.normalize(v, d)
+        else:
+            assert isinstance(
+                d, (list, tuple, set)
+            ), "# Error: {}\n  The distance parameter requires an list, tuple, set value when not moving along a vector.\n  {} {} given. #".format(
+                __file__, type(d), d
+            )
+            dx, dy, dz = d
+
+        result = (x + dx, y + dy, z + dz)
+
+        return result
+
+    @classmethod
+    def move_point_relative_along_vector(cls, a, b, vect, dist, toward=True):
+        """Move a point (a) along a given vector toward or away from a given point (b).
+
+        Parameters:
+                a (tuple): The point to move given as (x,y,z).
+                b (tuple): The point to move toward.
+                vect (tuple): A vector to move the point along.
+                dist (float) = The linear amount to move the point.
+                toward (bool): Move the point toward or away from.
+
+        Returns:
+                (tuple) point.
+
+        Example: move_point_relative_along_vector((0, 0, 0), (0, 10, 0), (0, 1, 0), 5) #returns: (0.0, 5.0, 0.0)
+        Example: move_point_relative_along_vector((0, 0, 0), (0, 10, 0), (0, 1, 0), 5, False) #returns: (0.0, -15.0, 0.0)
+        """
+        lowest = None
+        for i in [
+            dist,
+            -dist,
+        ]:  # move in pos and neg direction, and determine which is moving closer to the reference point.
+            p = cls.move_point_relative(a, i, vect)
+            d = cls.get_distance(p, b)
+            if lowest is None or (d < lowest if toward else d > lowest):
+                result, lowest = (p, d)
+
+        return result
+
+    @staticmethod
+    def get_distance(a: List[float], b: List[float]) -> float:
+        """
+        Calculate the distance between two points.
+
+        Parameters:
+                a (List[float]): A list of the first point's coordinates [x, y, z].
+                b (List[float]): A list of the second point's coordinates [x, y, z].
+
+        Returns:
+                float: The distance between the two points.
+        """
+        return ((b[0] - a[0]) ** 2 + (b[1] - a[1]) ** 2 + (b[2] - a[2]) ** 2) ** 0.5
+
+    @staticmethod
+    def get_center_of_two_points(
+        a: List[float], b: List[float]
+    ) -> Tuple[float, float, float]:
+        """Get the point in the middle of two given points.
+
+        Parameters:
+                a (List[float]): A point given as [x, y, z].
+                b (List[float]): A point given as [x, y, z].
+
+        Returns:
+                Tuple[float, float, float]: The center point between the two input points.
+
+        Example:
+                get_center_of_two_points([0, 10, 0], [0, 5, 0]) #returns: (0.0, 7.5, 0.0)
+        """
+        return ((a[0] + b[0]) / 2, (a[1] + b[1]) / 2, (a[2] + b[2]) / 2)
+
+    @classmethod
+    def get_angle_from_two_vectors(cls, v1, v2, degree=False):
+        """Get an angle from two given vectors.
+
+        Parameters:
+                v1 (tuple): A vectors xyz values as a tuple.
+                v2 (tuple): A vectors xyz values as a tuple.
+                degree (bool): Convert the radian result to degrees.
+
+        Returns:
+                (float)
+
+        Example: get_angle_from_two_vectors((1, 2, 3), (1, 1, -1)) #returns: 1.5707963267948966,
+        Example: get_angle_from_two_vectors((1, 2, 3), (1, 1, -1), True) #returns: 90
+        """
+        from math import acos, degrees
+
+        def length(v):
+            return (cls.dot_product(v, v)) ** 0.5
+
+        result = acos(cls.dot_product(v1, v2) / (length(v1) * length(v2)))
+
+        if degree:
+            result = round(degrees(result), 2)
+        return result
+
+    @staticmethod
+    def get_angle_from_three_points(a, b, c, degree=False):
+        """Get the opposing angle from 3 given points.
+
+        Parameters:
+                a (tuple): A point given as (x,y,z).
+                b (tuple): A point given as (x,y,z).
+                c (tuple): A point given as (x,y,z).
+                degree (bool): Convert the radian result to degrees.
+
+        Returns:
+                (float)
+
+        Example: get_angle_from_three_points((1, 1, 1), (-1, 2, 3), (1, 4, -3)) #returns: 0.7904487543360762,
+        Example: get_angle_from_three_points((1, 1, 1), (-1, 2, 3), (1, 4, -3), True) #returns: 45.29
+        """
+        from math import sqrt, acos, degrees
+
+        ba = [aa - bb for aa, bb in zip(a, b)]  # create vectors from points
+        bc = [cc - bb for cc, bb in zip(c, b)]
+
+        nba = sqrt(sum((x**2.0 for x in ba)))  # normalize vector
+        ba = [x / nba for x in ba]
+
+        nbc = sqrt(sum((x**2.0 for x in bc)))
+        bc = [x / nbc for x in bc]
+
+        scalar = sum(
+            (aa * bb for aa, bb in zip(ba, bc))
+        )  # get scalar from normalized vectors
+
+        angle = acos(scalar)  # get the angle in radian
+
+        if degree:
+            angle = round(degrees(angle), 2)
+        return angle
+
+    @staticmethod
+    def get_two_sides_of_asa_triangle(a1, a2, s, unit="degrees"):
+        """Get the length of two sides of a triangle, given two angles, and the length of the side in-between.
+
+        Parameters:
+                a1 (float) = Angle in radians or degrees. (unit flag must be set if value given in radians)
+                a2 (float) = Angle in radians or degrees. (unit flag must be set if value given in radians)
+                s (float) = The distance of the side between the two given angles.
+                unit (str): Specify whether the angle values are given in degrees or radians. (valid: 'radians', 'degrees')(default: degrees)
+
+        Returns:
+                (tuple)
+
+        Example: get_two_sides_of_asa_triangle(60, 60, 100) #returns: (100.00015320566493, 100.00015320566493)
+        """
+        from math import sin, radians
+
+        if unit == "degrees":
+            a1, a2 = radians(a1), radians(a2)
+
+        a3 = 3.14159 - a1 - a2
+
+        result = ((s / sin(a3)) * sin(a1), (s / sin(a3)) * sin(a2))
+
+        return result
+
+    @classmethod
+    def xyz_rotation(cls, theta, axis, rotation=[], degree=False):
+        """Get the rotation about the X,Y,Z axes (in rotation) given
+        an angle for rotation (in radians) and an axis about which to
+        do the rotation.
+
+        Parameters:
+                theta (float) = The angular position of a vector in radians.
+                axis (tuple): The rotation axis given as float values (x,y,z).
+                rotation (list):
+                degree (bool): Convert the radian result to degrees.
+
+        Returns:
+                (tuple) 3 point rotation.
+
+        Example: xyz_rotation(2, (0, 1, 0)) #returns: [3.589792907376932e-09, 1.9999999964102069, 3.589792907376932e-09]
+        Example: xyz_rotation(2, (0, 1, 0), [], True) #returns: [0.0, 114.59, 0.0]
+        """
+        from math import cos, sin, sqrt, atan2, degrees
+
+        # set up the xyzw quaternion values
+        theta *= 0.5
+        w = cos(theta)
+        factor = sin(theta)
+        axisLen2 = cls.dot_product(axis, axis, 0)
+
+        if axisLen2 != 1.0 and axisLen2 != 0.0:
+            factor /= sqrt(axisLen2)
+        x, y, z = factor * axis[0], factor * axis[1], factor * axis[2]
+
+        # setup rotation in a matrix
+        ww, xx, yy, zz = w * w, x * x, y * y, z * z
+        s = 2.0 / (ww + xx + yy + zz)
+        xy, xz, yz, wx, wy, wz = x * y, x * z, y * z, w * x, w * y, w * z
+        matrix = [
+            1.0 - s * (yy + zz),
+            s * (xy + wz),
+            s * (xz - wy),
+            None,
+            None,
+            1.0 - s * (xx + zz),
+            s * (yz + wx),
+            None,
+            None,
+            s * (yz - wx),
+            1.0 - s * (xx + yy),
+        ]
+
+        # get x,y,z values for rotation
+        cosB = sqrt(matrix[0] * matrix[0] + matrix[1] * matrix[1])
+        if cosB > 1.0e-10:
+            pi = 3.14159265
+
+            a, b, c = solution1 = [
+                atan2(matrix[6], matrix[10]),
+                atan2(-matrix[2], cosB),
+                atan2(matrix[1], matrix[0]),
+            ]
+
+            solution2 = [
+                a + (pi if a < pi else -pi),
+                (pi if b > -pi else -pi) - b,
+                c + (pi if c < pi else -pi),
+            ]
+
+            if sum([abs(solution2[0]), abs(solution2[1]), abs(solution2[2])]) < sum(
+                [abs(solution1[0]), abs(solution1[1]), abs(solution1[2])]
+            ):
+                rotation = solution2
+            else:
+                rotation = solution1
+
+        else:
+            rotation = [atan2(-matrix[9], matrix[5]), atan2(-matrix[2], cosB), 0.0]
+
+        if degree:
+            rotation = [round(degrees(r), 2) for r in rotation]
+        return tuple(rotation)
 
 
 # --------------------------------------------------------------------------------------------
 
-def __getattr__(attr:str):
-	"""Searches for an attribute in this module's classes and returns it.
-
-	Parameters:
-		attr (str): The name of the attribute to search for.
-	
-	Return:
-		(obj) The found attribute.
-
-	:Raises:
-		AttributeError: If the given attribute is not found in any of the classes in the module.
-	"""
-	try:
-		return getattr(Math, attr)
-
-	except AttributeError as error:
-		raise AttributeError(f"Module '{__name__}' has no attribute '{attr}'")
-
-# --------------------------------------------------------------------------------------------
-
-if __name__=='__main__':
-	pass
+if __name__ == "__main__":
+    pass
 
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
 
-
 # Deprecated ------------------------------------
 
 # @classmethod
 # def normalize(cls, vector, amount=1):
-# 	'''Normalize a vector
+#   '''Normalize a vector
 
-# 	Parameters:
-# 		vector (vector) = The vector to normalize.
-# 		amount (float) = (1) Normalize standard. (value other than 0 or 1) Normalize using the given float value as desired length.
-	
-# 	Return:
-# 		(tuple)
-# 	'''
-# 	length = cls.getMagnitude(vector)
-# 	x, y, z = vector
-
-# 	result = (
-# 		x /length *amount,
-# 		y /length *amount,
-# 		z /length *amount
-# 	)
-
-# 	return result
-
-	# @classmethod
-	# def crossProduct(cls, v1, v2, normalizeInputs=False, normalizeResult=False):
-	# 	'''Given two float arrays of 3 values each, this procedure returns
-	# 	the cross product of the two arrays as a float array of size 3.
-
-	# 	:Parmeters:
-	# 		v1 (list): The first 3 point vector. 
-	# 		v2 (list): The second 3 point vector.
-	# 		normalizeInputs (bool): Normalize v1, v2 before calculating the point float list.
-	# 		normalizeResult (bool): Normalize the return value.
-
-	# 	Return:
-	# 		(tuple) The cross product of the two vectors.
-
-	# 	Example: crossProduct((1, 2, 3), (1, 1, -1)) #returns: (-5, 4, -1)
-	# 	Example: crossProduct((1, 2, 3), (1, 1, -1), True) #returns: (-0.7715167498104597, 0.6172133998483678, -0.15430334996209194)
-	# 	Example: crossProduct((1, 2, 3), (1, 1, -1), False, True) #returns: (-0.7715167498104595, 0.6172133998483676, -0.1543033499620919)
-	# 	'''
-	# 	if normalizeInputs: #normalize the input vectors
-	# 		v1 = cls.normalize(v1)
-	# 		v2 = cls.normalize(v2)
-
-	# 	cross = [ #the cross product
-	# 		v1[1]*v2[2] - v1[2]*v2[1],
-	# 		v1[2]*v2[0] - v1[0]*v2[2],
-	# 		v1[0]*v2[1] - v1[1]*v2[0]
-	# 	]
+#   Parameters:
+#       vector (vector) = The vector to normalize.
+#       amount (float) = (1) Normalize standard. (value other than 0 or 1) Normalize using the given float value as desired length.
+
+#   Returns:
+#       (tuple)
+#   '''
+#   length = cls.get_magnitude(vector)
+#   x, y, z = vector
+
+#   result = (
+#       x /length *amount,
+#       y /length *amount,
+#       z /length *amount
+#   )
+
+#   return result
+
+# @classmethod
+# def cross_product(cls, v1, v2, normalize_input=False, normalizeResult=False):
+#   '''Given two float arrays of 3 values each, this procedure returns
+#   the cross product of the two arrays as a float array of size 3.
+
+#   :Parmeters:
+#       v1 (list): The first 3 point vector.
+#       v2 (list): The second 3 point vector.
+#       normalize_input (bool): Normalize v1, v2 before calculating the point float list.
+#       normalizeResult (bool): Normalize the return value.
+
+#   Returns:
+#       (tuple) The cross product of the two vectors.
+
+#   Example: cross_product((1, 2, 3), (1, 1, -1)) #returns: (-5, 4, -1)
+#   Example: cross_product((1, 2, 3), (1, 1, -1), True) #returns: (-0.7715167498104597, 0.6172133998483678, -0.15430334996209194)
+#   Example: cross_product((1, 2, 3), (1, 1, -1), False, True) #returns: (-0.7715167498104595, 0.6172133998483676, -0.1543033499620919)
+#   '''
+#   if normalize_input: #normalize the input vectors
+#       v1 = cls.normalize(v1)
+#       v2 = cls.normalize(v2)
+
+#   cross = [ #the cross product
+#       v1[1]*v2[2] - v1[2]*v2[1],
+#       v1[2]*v2[0] - v1[0]*v2[2],
+#       v1[0]*v2[1] - v1[1]*v2[0]
+#   ]
 
-	# 	if normalizeResult: #normalize the cross product result
-	# 		cross = cls.normalize(cross)
+#   if normalizeResult: #normalize the cross product result
+#       cross = cls.normalize(cross)
 
-	# 	return tuple(cross)
+#   return tuple(cross)
```

### Comparing `pythontk-0.6.2/pythontk.egg-info/PKG-INFO` & `pythontk-0.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythontk
-Version: 0.6.2
+Version: 0.6.4
 Summary: *pythontk is a collection of backend utilities for Python.*
 Home-page: https://github.com/m3trik/pythontk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,14 @@
 ```
 
 ### Example use-case:
 ###### Import the class `Iter` from the package.
 ###### As the name suggests, the class `Iter` holds the package's iterable related functions.
 ```python
 from pythontk import Iter
-Iter.filterList([0, 1, 2, 3, 2], [1, 2, 3], 2) #returns: [1, 3]
+Iter.filter_list([0, 1, 2, 3, 2], [1, 2, 3], 2) #returns: [1, 3]
 ```
-###### You can also import a function directly.
+###### You can also import any function directly.
 ```python
-from pythontk.Iter import filterDict
-filterDict({1:'1', 'two':2, 3:'three'}, exc='t*', keys=True) #returns: {1: '1', 3: 'three'}
+from pythontk import filter_dict
+filter_dict({1:'1', 'two':2, 3:'three'}, exc='t*', keys=True) #returns: {1: '1', 3: 'three'}
 ```
```

### Comparing `pythontk-0.6.2/setup.py` & `pythontk-0.6.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,73 @@
 import os
 import setuptools
 
 from pythontk import __package__, __version__
 from pythontk import File, Str
 
 
-long_description = File.getFileContents('docs/README.md')
-description = Str.getTextBetweenDelimiters(long_description, '<!-- short_description_start -->', '<!-- short_description_end -->', as_string=True)
+long_description = File.get_file_contents("docs/README.md")
+description = Str.get_text_between_delimiters(
+    long_description,
+    "<!-- short_description_start -->",
+    "<!-- short_description_end -->",
+    as_string=True,
+)
 
 setuptools.setup(
-	name=__package__,
-	version=__version__,
-	author='Ryan Simpson',
-	author_email='m3trik@outlook.com',
-	description=description,
-	long_description=long_description,
-	long_description_content_type='text/markdown',
-	url=f'https://github.com/m3trik/{__package__}',
-	packages=setuptools.find_packages(),
-	classifiers=[
-		'Programming Language :: Python :: 3',
-		'License :: OSI Approved :: MIT License',
-		'Operating System :: OS Independent',
-	],
-	include_package_data = True,
-	data_files=File.getDirContents(__package__, 'filepaths', excFiles=['*.py', '*.pyc', '*.json']), #ie. ('uitk/ui/0', ['uitk/ui/0/init.ui']),
+    name=__package__,
+    version=__version__,
+    author="Ryan Simpson",
+    author_email="m3trik@outlook.com",
+    description=description,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url=f"https://github.com/m3trik/{__package__}",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    include_package_data=True,
+    data_files=File.get_dir_contents(
+        __package__, "filepaths", exc_files=["*.py", "*.pyc", "*.json"]
+    ),  # ie. ('uitk/ui/0', ['uitk/ui/0/init.ui']),
 )
 
 # --------------------------------------------------------------------------------------------
 
 
-
-
-
-
-
-
-
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
 
-
 # Deprecated ------------------------------------
 
 
 # def gen_data_files(dirs, exc=[], inc=[]):
 # 	'''
 # 	'''
-# 	dirs = Iter.makeList(dirs)
-# 	exc = Iter.makeList(exc)
-# 	inc = Iter.makeList(inc)
+# 	dirs = Iter.make_iterable(dirs)
+# 	exc = Iter.make_iterable(exc)
+# 	inc = Iter.make_iterable(inc)
 
 # 	results = []
 # 	for src_dir in dirs:
 # 		for root, dirs, files in os.walk(src_dir):
 # 			filtered=[]
 # 			for f in files:
-# 				ext = File.formatPath(f, 'ext')
+# 				ext = File.format_path(f, 'ext')
 # 				if f in exc or '*.'+ext in exc:
 # 					continue
 # 				if any(inc): #filter inc for None values so not to get a false positive.
 # 					if not f in inc and not '*.'+ext in inc:
 # 						continue
 # 				filtered.append(f)
 
 # 			if filtered:
 # 				results.append((root, list(map(lambda f:root + "/" + f, filtered))))
 # 	return results
 
 # # for i in gen_data_files('uitk', exc=['*.py', '*.pyc', '*.json']):
-# 	# print (i)
+# 	# print (i)
```

