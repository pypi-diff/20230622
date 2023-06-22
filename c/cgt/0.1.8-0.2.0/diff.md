# Comparing `tmp/cgt-0.1.8.tar.gz` & `tmp/cgt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Circular-genome-tools/Circular-genome-tools/dist/tmph6idh2x5/cgt-0.1.8.tar", last modified: Thu Mar 10 23:22:15 2022, max compression
+gzip compressed data, was "cgt-0.2.0.tar", last modified: Thu Jun 22 02:11:52 2023, max compression
```

## Comparing `cgt-0.1.8.tar` & `cgt-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 23:22:15.000000 cgt-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-10 23:21:51.000000 cgt-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-03-10 23:21:51.000000 cgt-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-03-10 23:21:52.000000 cgt-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-10 23:22:15.000000 cgt-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 23:22:15.000000 cgt-0.1.8/cgt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-03-10 23:22:15.000000 cgt-0.1.8/cgt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-03-10 23:22:15.000000 cgt-0.1.8/cgt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-03-10 23:22:15.000000 cgt-0.1.8/cgt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-10 23:22:15.000000 cgt-0.1.8/cgt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-03-10 23:22:15.000000 cgt-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-10 23:21:51.000000 cgt-0.1.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 23:22:15.000000 cgt-0.1.8/cgt/
--rw-r--r--   0 runner    (1001) docker     (121)    19354 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/position_paradigm.py
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/genome.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 23:22:15.000000 cgt-0.1.8/cgt/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3950 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     4606 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/rearrangements.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8388 2022-03-10 23:21:51.000000 cgt-0.1.8/cgt/distances.py
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-03-10 23:21:51.000000 cgt-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-03-10 23:21:51.000000 cgt-0.1.8/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-03-10 23:21:51.000000 cgt-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:52.067998 cgt-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-22 02:11:40.000000 cgt-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-22 02:11:40.000000 cgt-0.2.0/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 02:11:40.000000 cgt-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-22 02:11:40.000000 cgt-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 02:11:52.067998 cgt-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-22 02:11:40.000000 cgt-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 02:11:40.000000 cgt-0.2.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:52.063998 cgt-0.2.0/cgt/
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/# Representation theory of the Hyperocta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/genome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20386 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/position_paradigm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/rearrangements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:52.067998 cgt-0.2.0/cgt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:52.067998 cgt-0.2.0/cgt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 02:11:52.000000 cgt-0.2.0/cgt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-22 02:11:52.000000 cgt-0.2.0/cgt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:11:52.000000 cgt-0.2.0/cgt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 02:11:52.000000 cgt-0.2.0/cgt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-22 02:11:41.000000 cgt-0.2.0/playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-22 02:11:41.000000 cgt-0.2.0/playground_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:11:52.067998 cgt-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-22 02:11:41.000000 cgt-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cgt-0.1.8/LICENSE` & `cgt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cgt-0.1.8/setup.py` & `cgt-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `cgt-0.1.8/cgt.egg-info/PKG-INFO` & `cgt-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cgt
-Version: 0.1.8
+Version: 0.2.0
 Summary: Tools for representing genomes in sage
 Home-page: https://github.com/js51/Circular-genome-tools
 Author: Joshua Stevenson
 Author-email: joshua.stevenson@utas.edu.au
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,9 +24,7 @@
 and use `import cgt` in a sage script or environment.
 
 If you would like to contribute to `cgt`, please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for how to get set up.
 
 If you use this software in your work, please cite it use the citation function on the github page or see [`CITATION.cff`](CITATION.cff)
 
 **Note:** you will need to at least have Sage version 9.0 installed, and have the GAP package `repsn` installed for the copy of GAP that sits inside Sage. If you aren't sure how to do this, see the installation instructions in [`INSTALL.md`](INSTALL.md).
-
-
```

### Comparing `cgt-0.1.8/PKG-INFO` & `cgt-0.2.0/cgt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cgt
-Version: 0.1.8
+Version: 0.2.0
 Summary: Tools for representing genomes in sage
 Home-page: https://github.com/js51/Circular-genome-tools
 Author: Joshua Stevenson
 Author-email: joshua.stevenson@utas.edu.au
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,9 +24,7 @@
 and use `import cgt` in a sage script or environment.
 
 If you would like to contribute to `cgt`, please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for how to get set up.
 
 If you use this software in your work, please cite it use the citation function on the github page or see [`CITATION.cff`](CITATION.cff)
 
 **Note:** you will need to at least have Sage version 9.0 installed, and have the GAP package `repsn` installed for the copy of GAP that sits inside Sage. If you aren't sure how to do this, see the installation instructions in [`INSTALL.md`](INSTALL.md).
-
-
```

### Comparing `cgt-0.1.8/cgt/position_paradigm.py` & `cgt-0.2.0/cgt/position_paradigm.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,39 +13,49 @@
 from .structures import HyperoctahedralGroup
 from scipy.sparse import dok_matrix as dok
 from random import choice
 
 class PositionParadigmFramework:
     """Everything you need for working with genomes under the position paradigm"""
 
-    def __init__(self, num_regions, oriented=True, symmetry=None, genome_type=TYPE.reg_to_signed_pos):
+    def __init__(self, num_regions, oriented=True, symmetry=SYMMETRY.circular, genome_type=TYPE.reg_to_signed_pos):
         """Instantiate a system of position paradigm genomes with given set of symmetries and number of regions."""
         if genome_type != TYPE.reg_to_signed_pos:
             raise NotImplementedError("Genome type not yet supported. For now use TYPE.reg_to_signed_pos")
         self.n = num_regions
         self.oriented = oriented
         self.symmetry = symmetry
+        self.representations = None
+        self._genomes = None
         
     def __eq__(self, other): # String representation is unique and repr calls str
         return self.__repr__() == other.__repr__()
 
     def __str__(self):
         string = f"Framework for {str(self.symmetry).replace('SYMMETRY.', '')} genomes"
         string += f" with {self.n}{' oriented' if self.oriented else ''} regions"
         return string
 
     def __repr__(self):
         return self.__str__() # String representation is unique
 
     def __call__(self, x):
         """Return an object as a group algebra element if possible"""
-        return self.genome_algebra()(self.cycles(x))
+        return self.group_algebra()(self.cycles(x))
 
     def __hash__(self):
         return self.__str__().__hash__() # String rep is unique, so just hash that!
+    
+    def __contains__(self, item):
+        # If the item is an instance
+        if item in self.genome_group():
+            return True
+        if item in self.group_algebra():
+            raise NotImplementedError("Not yet implemented")
+        return False
 
     def cycles(self, element):
         try: # See if it's already a group element
             return self.genome_group()(element)
         except ValueError:
             pass # Not able to be directly converted, try something else!
         if type(element) is np.ndarray: # If it's a matrix, let's convert it!
@@ -58,14 +68,18 @@
         if (not self.oriented) or len(elt) == 2*self.n:
             return self.genome_group()(elt)
         elif len(elt) == self.n:
             other_half = list(-int(elt[self.n - i]) for i in range(1, self.n+1))
             return self.genome_group()(elt + other_half)
         else:
             raise ValueError("Invalid data for constructing a permutation")
+        
+    def instances(self, genome):
+        """Return a list of instances of the genome."""
+        return [instance[0] for instance in list(genome)]
 
     def one_row(self, element, as_list=False):
         """Return a given genome instance in one-row notation.
 
         Args:
             element: the genome instance to represent in one-row notation. Multiple formats accepted.
             as_list: if true, return as a list of images, otherwise return a sage permutation.
@@ -96,14 +110,19 @@
         """Return the 'canonical' instance of the genome represented by the permutation if there is one.
 
         Examples:
             sage: import cgt; ppf = cgt.PositionParadigmFramework(3, symmetry=cgt.SYMMETRY.circular)
             sage: ppf.canonical_instance('(1,-2)(-1,2)')
             [1, 2, -3]
         """
+        try:
+            instance = self.cycles(deepcopy(instance))
+        except:
+            # Probably accidentally given a genome instead of an instance
+            instance = self.instances(instance)[0]
         instance = deepcopy(self.one_row(self.cycles(instance)))
         if self.symmetry in {SYMMETRY.circular, SYMMETRY.linear}:
             f = self.one_row(self.standard_reflection())
             if list(instance)[0] < 0:
                 instance = instance*f
             if self.symmetry is SYMMETRY.circular:
                 r = self.one_row(self.standard_rotation())
@@ -204,21 +223,25 @@
             return sum(1/Z.order()*A(self.cycles(dx)) for dx in coset)
         else:
             return coset
 
     def genomes(self, format=FORMAT.dictionary, sort_genomes=True):
         if format not in {FORMAT.dictionary, FORMAT.formal_sum}:
             raise NotImplementedError("Not yet implemented! Convert manually to other formats from FORMAT.dictionary")
-        instances = set(self.genome_group())
-        genomes = {}
-        while len(instances) > 0:
-            instance = instances.pop()
-            coset = self._genome_coset(instance)
-            instances -= set(coset)
-            genomes[coset[0]] = coset
+        if self._genomes is None:
+            instances = set(self.genome_group())
+            genomes = {}
+            while len(instances) > 0:
+                instance = instances.pop()
+                coset = self._genome_coset(instance)
+                instances -= set(coset)
+                genomes[coset[0]] = coset
+            self._genomes = genomes
+        else:
+            genomes = self._genomes
         if format == FORMAT.formal_sum:
             Z = self.symmetry_group()
             A = self.group_algebra()
             genomes = { rep : sum(1/Z.order()*A(self.cycles(dx)) for dx in coset) for rep, coset in genomes.items() }
         if sort_genomes:
             genomes = dict(sorted(genomes.items(), key=lambda x: self._sort_key(x[0])))
         return genomes
@@ -284,15 +307,14 @@
     def matrix(self, element):
         """Return the defining representation matrix. Note that matrix(x)matrix(y) = matrix(yx)"""
         with warnings.catch_warnings(): # Sage uses deprecated objects in to_matrix for coloured permutations. We would like to not be reminded of this.
             warnings.simplefilter("ignore", category=PendingDeprecationWarning)
             return np.array(self.one_row(self.cycles(element)).to_matrix())
 
     def reg_rep_of_zs(self, model, to_adjacency_matrix=False, sparse=True):
-        warnings.warn("Untested! Use at your own risk!")
         # TODO: #14 re-write to directly use model element from the genome algebra
         if self is not model.framework:
             if self != model.framework:
                 raise ValueError(f"Current framework and model framework are not the same!")
             else:
                 warnings.warn("Current framework and model framework reference different objects! This might cause problems.")
         Z = self.symmetry_group()
@@ -335,14 +357,16 @@
         representations = self._cached_irreps()
         if element is not None:
             return [irrep(element) for irrep in representations]
         else:
             return representations
 
     def _cached_irreps(self):
+        if self.representations is not None:
+            return self.representations
         representations = []
         def irrep_function_factory(irrep, signed):
             def representation(sigma, _irrep=irrep, _signed=signed):
                     result = 0
                     if sigma in self.group_algebra(): # sigma is an algebra element
                         for term in sigma:
                             perm, coeff = term
@@ -354,31 +378,35 @@
             return representation
         if not self.oriented:
             irreps = SymmetricGroupRepresentations(self.n)
         else:
             irreps = (gap.IrreducibleAffordingRepresentation(character) for character in gap.Irr(self.genome_group()))
         for irrep in irreps:
             representations.append(irrep_function_factory(irrep, self.oriented))
-        return representations
+        self.representations = representations
+        return self.representations
 
     def regular_representation(self, g):
         """Return the regular representation of a single element"""
         warnings.warn("this function is untested! Use at your own risk.", DeprecationWarning)
         return matrix(QQbar, [(self.group_algebra()(g)*self.genome_group()(h)).to_vector(QQbar) for h in self.genome_group()]).transpose()
 
-    def coefficient_in(self, more_terms, fewer_terms):
+    def coefficient_in(self, more_terms, fewer_terms, none_if_fail=False):
         """For example, the coefficient of (a/2 + b/2) in x=(a/3 + b/3 + c/3) is 2/3, since x=2/3*(a/2 + b/2) + c/3"""
         coefficients_in_larger_sum = {}
         for term in fewer_terms.terms():
             perm  = self.genome_group()(list(term)[0][0]) # a
             coeff = list(term)[0][1] # 1/2
             coefficients_in_larger_sum[perm] = more_terms.coefficient(perm) * (1/coeff) # 1/3 * 2 = 2/3
         terms = set(coefficients_in_larger_sum.values())
         if len(terms) != 1:
-            warnings.warn("Note that extra terms from the smaller sum remain in the larger sum!")
+            if none_if_fail:
+                return None
+            else:
+                warnings.warn("Note that extra terms from the smaller sum remain in the larger sum!")
         return min(terms)
 
     def collect_genome_terms(self, formal_sum, display=DISPLAY.one_row):
         """Return a weighted sum of genomes, represented as [canonical representation]z"""
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
             formal_sum = deepcopy(formal_sum)
```

### Comparing `cgt-0.1.8/cgt/structures.py` & `cgt-0.2.0/cgt/structures.py`

 * *Files identical despite different names*

### Comparing `cgt-0.1.8/cgt/enums.py` & `cgt-0.2.0/cgt/enums.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,8 +42,19 @@
     arrows  = auto()
     one_row = auto()
     cycles  = auto()
 
 class ALGEBRA(Enum):
     group        = auto()
     genome       = auto()
-    genome_class = auto()
+    genome_class = auto()
+
+class IRREP_TYPE(Enum):
+    specht = speck = auto()
+    orthogonal     = auto()
+    seminormal     = auto()
+
+class DISTANCE(Enum):
+    min = minimum = auto()
+    min_weighted = minimum_weighted = auto()
+    MFPT = min_first_passage_time = auto()
+    MLE = maximum_likelihood_distance = maximum_likelihood_estimate = auto()
```

### Comparing `cgt-0.1.8/cgt/visualisation.py` & `cgt-0.2.0/cgt/visualisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .enums import *
 
 def draw_genome_instance(framework, instance, show=False):
     """Produce a drawing of a circular genome with n regions"""
     if not framework.oriented:
         raise NotImplementedError("not implemented for linear genomes.")
     try:
-        instance = framework(instance)
+        instance = framework.cycles(instance)
     except:
         TypeError(f"{instance} does not belong in {str(framework)}")
 
     matplotlib.rcParams.update({
         "text.usetex": True,
         "font.family": "serif",
         "pgf.texsystem": "pdflatex",
@@ -64,8 +64,8 @@
     ax1.axis('equal') # makes sure it's a circle
     plt.tight_layout()
 
     if not os.path.exists('_output'):
         os.makedirs('_output')
     plt.savefig(f'_output/{str(instance)}.png', transparent=True)
     plt.savefig(f'_output/{str(instance)}.pdf', transparent=True)
-    if show: plt.show()
+    if show: plt.show()
```

### Comparing `cgt-0.1.8/cgt/models.py` & `cgt-0.2.0/cgt/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """
 """
 
 from sage.all_cmdline import QQ
 from .enums import *
 from . import rearrangements
+from scipy.sparse import dok_matrix as dok
+import numpy as np
+
 
 class Model:
     """Defines a model. A model consists of some collection of permutations and a map from these permutations to probabilities [0,1]"""
     def __init__(self, framework, generating_dictionary):
         """Define a model from a dictionary of single permutations, with their probabilities as the values."""
         self.framework = framework
         self.generating_dictionary = generating_dictionary
         self.names = []
+        self._reg_rep_of_zs = None # For caching the regular representation of zs
+        self.data_bundle = {} # Used to cache data for several functions
         # TODO: Implement checks for certain model properties, for example time reversibility, symmetry and missing rearrangements
 
     def __repr__(self):
         return f"Model({str(self.framework)}, {str(self.generating_dictionary)})"
 
     def __str__(self):
         """Return a descriptive string for the model"""
@@ -51,16 +56,38 @@
                     model[generator] = relative_prob/len(gens)
         model = cls(framework, model)
         model.names += list(named_model_dictionary.keys())
         return model
 
     def reg_rep_of_zs(self):
         """Return the regular representation of zs as comptued by PositionParadigmFramework.reg_rep_zs, but store the sparse result"""
-        return self.framework.reg_rep_of_zs(self, sparse=True)
-
+        if self._reg_rep_of_zs is None:
+            self._reg_rep_of_zs = self.framework.reg_rep_of_zs(self, sparse=True)
+        return self._reg_rep_of_zs
+    
+    def reg_rep(self):
+        fw = self.framework
+        A = fw.group_algebra()
+        s = A(self.s_element())
+        z = A(fw.symmetry_element())
+
+        genomes = fw.genomes(format=FORMAT.formal_sum)
+        
+        model_generators_cycles = list(self.generating_dictionary.keys())
+        model_generators = [ fw.one_row(elt) for elt in model_generators_cycles ]
+
+        num_genomes = len(genomes.keys())
+        
+        matrix = dok((num_genomes, num_genomes), dtype=np.float32)
+        
+        for g, genome in enumerate(genomes.values()):
+            zszo = A(genome) * z * s * z
+            print(fw.collect_genome_terms(zszo))
+    
+    
     def s_element(self, in_algebra=ALGEBRA.genome):
         if in_algebra not in {ALGEBRA.group, ALGEBRA.genome}:
             raise NotImplementedError(f"Model element for {str(in_algebra)} algebra not yet implemented")
         A = self.framework.group_algebra()
         s = A(0) # Zero element in algebra
         gens_dict = self.generating_dictionary
         gens = {x for x in self.generating_dictionary.keys()}
```

### Comparing `cgt-0.1.8/cgt/rearrangements.py` & `cgt-0.2.0/cgt/rearrangements.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,21 +8,26 @@
 from .enums import *
 
 def css(cuts_set):
     string = ''.join(sorted([str(cut[0]) for cut in cuts_set]))
     if len(string) != len(cuts_set): print("something went very wrong here...")
     return string
 
-def cuts(framework, sigma):
-    sigma = deepcopy(framework.one_row(sigma))
-    n = framework.n
+
+def c_perm(n):
     pmN = structures.set_plus_minus(n)
     G = SymmetricGroup(pmN)
     c_string = f'({",".join(str(i) for i in list(range(1, n+1)))})({",".join(str(i) for i in list(range(-n, 0)))})'
     c = G(c_string)
+    return c
+
+def cuts(framework, sigma):
+    sigma = deepcopy(framework.one_row(sigma))
+    n = framework.n
+    c = c_perm(n)
     sigma = list(sigma)
     return set([ 
         tuple(([i+1,c(i+1)])) for i in range(len(sigma)) 
         if (sigma[c(i + 1)-1] != c(sigma[i]))
     ])
 
 def __all_canonical_inversions(framework, num_regions=None):
@@ -104,7 +109,45 @@
     return __representatives(framework, __all_canonical_inversions(framework, num_regions=num_regions), classes=CLASSES.double_cosets)
 
 def all_adjacent_transpositions_representatives(framework, num_regions=None):
     if num_regions == 2:
         return __two_region_adjacent_transposition_reps(framework)
     else:
         raise NotImplementedError(f"model not yet implemented")
+
+def permutation_with_cuts(framework, cuts, perm=None, start=None):
+    n = framework.n
+    c = c_perm(n)
+    if perm is None:
+        if not (framework.oriented and framework.symmetry == SYMMETRY.circular):
+            raise NotImplementedError(f"not yet implemented for {str(framework)}")
+        perm = {}
+        perm[1] = 1 # making the canonical instance
+        results = permutation_with_cuts(cuts, perm, 2)
+        for result in results:
+            if result:
+                yield list(result.values())
+    else: # recurse
+        possibilities = set(range(1, n+1)) | set(range(-n, 0))
+        for val in perm.values():
+            possibilities.remove(val)
+            possibilities.remove(-val)
+        if start-1 in cuts:
+            if c(perm[start-1]) in possibilities: possibilities.remove(c(perm[start-1]))
+        else:
+            possibilities = possibilities & {c(perm[start-1])}
+        if start == n: # also check if *start* is a cut
+            if start in cuts:
+                # add exclusions
+                if start in possibilities: possibilities.remove(start) # p[1]=1 so we can't have p[n]=n
+            else:
+                possibilities = possibilities & {n} # we must choose n
+            for possibility in possibilities:
+                bperm = perm.copy()
+                bperm[start] = possibility
+                yield bperm
+        else:
+            for possibility in possibilities:
+                bperm = perm.copy()
+                bperm[start] = possibility
+                for result in permutation_with_cuts(cuts, bperm, start+1):
+                    yield result
```

### Comparing `cgt-0.1.8/CONTRIBUTING.md` & `cgt-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cgt-0.1.8/INSTALL.md` & `cgt-0.2.0/INSTALL.md`

 * *Files identical despite different names*

### Comparing `cgt-0.1.8/README.md` & `cgt-0.2.0/README.md`

 * *Files identical despite different names*

