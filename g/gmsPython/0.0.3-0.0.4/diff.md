# Comparing `tmp/gmsPython-0.0.3.tar.gz` & `tmp/gmsPython-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmsPython-0.0.3.tar", last modified: Thu Jan  5 13:28:48 2023, max compression
+gzip compressed data, was "gmsPython-0.0.4.tar", last modified: Thu Jun 22 12:30:16 2023, max compression
```

## Comparing `gmsPython-0.0.3.tar` & `gmsPython-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-01-05 13:28:48.871918 gmsPython-0.0.3/
--rw-rw-rw-   0        0        0     1089 2022-11-24 13:42:30.000000 gmsPython-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      496 2023-01-05 13:28:48.871918 gmsPython-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       53 2022-11-25 13:02:43.000000 gmsPython-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-05 13:28:48.838105 gmsPython-0.0.3/gmsPython/
--rw-rw-rw-   0        0        0      113 2022-11-25 08:53:54.000000 gmsPython-0.0.3/gmsPython/__init__.py
--rw-rw-rw-   0        0        0     2850 2023-01-05 13:22:42.000000 gmsPython-0.0.3/gmsPython/_mixedTools.py
-drwxrwxrwx   0        0        0        0 2023-01-05 13:28:48.860822 gmsPython-0.0.3/gmsPython/gmsPy/
--rw-rw-rw-   0        0        0       56 2022-11-24 16:06:45.000000 gmsPython-0.0.3/gmsPython/gmsPy/__init__.py
--rw-rw-rw-   0        0        0     5517 2022-11-24 16:26:25.000000 gmsPython-0.0.3/gmsPython/gmsPy/_gmsPy.py
--rw-rw-rw-   0        0        0    10205 2023-01-04 13:39:57.000000 gmsPython-0.0.3/gmsPython/gmsPy/gmsPy.py
-drwxrwxrwx   0        0        0        0 2023-01-05 13:28:48.864578 gmsPython-0.0.3/gmsPython/gmsPyModels/
--rw-rw-rw-   0        0        0       62 2022-11-25 08:55:10.000000 gmsPython-0.0.3/gmsPython/gmsPyModels/__init__.py
--rw-rw-rw-   0        0        0     1484 2022-11-29 12:14:47.000000 gmsPython-0.0.3/gmsPython/gmsPyModels/gmsPyGlobals.py
--rw-rw-rw-   0        0        0     8892 2023-01-05 13:19:57.000000 gmsPython-0.0.3/gmsPython/gmsPyModels/gmsPyModels.py
-drwxrwxrwx   0        0        0        0 2023-01-05 13:28:48.867570 gmsPython-0.0.3/gmsPython/gmsWrite/
--rw-rw-rw-   0        0        0     1402 2023-01-05 13:28:07.000000 gmsPython-0.0.3/gmsPython/gmsWrite/__init__.py
--rw-rw-rw-   0        0        0     9269 2023-01-05 13:27:59.000000 gmsPython-0.0.3/gmsPython/gmsWrite/_gmsWrite.py
--rw-rw-rw-   0        0        0     1402 2023-01-05 13:28:08.000000 gmsPython-0.0.3/gmsPython/gmsWrite/gmsWrite.py
-drwxrwxrwx   0        0        0        0 2023-01-05 13:28:48.870562 gmsPython-0.0.3/gmsPython/nestingTree/
--rw-rw-rw-   0        0        0       73 2022-11-24 16:05:43.000000 gmsPython-0.0.3/gmsPython/nestingTree/__init__.py
--rw-rw-rw-   0        0        0     7467 2023-01-04 14:51:08.000000 gmsPython-0.0.3/gmsPython/nestingTree/nestingTree.py
-drwxrwxrwx   0        0        0        0 2023-01-05 13:28:48.856859 gmsPython-0.0.3/gmsPython.egg-info/
--rw-rw-rw-   0        0        0      496 2023-01-05 13:28:48.000000 gmsPython-0.0.3/gmsPython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2023-01-05 13:28:48.000000 gmsPython-0.0.3/gmsPython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-05 13:28:48.000000 gmsPython-0.0.3/gmsPython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-01-05 13:28:48.000000 gmsPython-0.0.3/gmsPython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-05 13:28:48.000000 gmsPython-0.0.3/gmsPython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-05 13:28:48.872777 gmsPython-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-01-05 13:28:09.000000 gmsPython-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.913842 gmsPython-0.0.4/
+-rw-rw-rw-   0        0        0     1089 2022-11-24 13:42:30.000000 gmsPython-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      496 2023-06-22 12:30:16.912848 gmsPython-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2022-11-25 13:02:43.000000 gmsPython-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.874406 gmsPython-0.0.4/gmsPython/
+-rw-rw-rw-   0        0        0      113 2022-11-25 08:53:54.000000 gmsPython-0.0.4/gmsPython/__init__.py
+-rw-rw-rw-   0        0        0     2850 2023-06-08 21:34:06.000000 gmsPython-0.0.4/gmsPython/_mixedTools.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.895563 gmsPython-0.0.4/gmsPython/gmsPy/
+-rw-rw-rw-   0        0        0       56 2022-11-24 16:06:45.000000 gmsPython-0.0.4/gmsPython/gmsPy/__init__.py
+-rw-rw-rw-   0        0        0     5517 2023-05-22 09:12:42.000000 gmsPython-0.0.4/gmsPython/gmsPy/_gmsPy.py
+-rw-rw-rw-   0        0        0    10392 2023-06-09 12:23:34.000000 gmsPython-0.0.4/gmsPython/gmsPy/gmsPy.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.895563 gmsPython-0.0.4/gmsPython/gmsPyModels/
+-rw-rw-rw-   0        0        0       62 2022-11-25 08:55:10.000000 gmsPython-0.0.4/gmsPython/gmsPyModels/__init__.py
+-rw-rw-rw-   0        0        0     1484 2022-11-29 12:14:47.000000 gmsPython-0.0.4/gmsPython/gmsPyModels/gmsPyGlobals.py
+-rw-rw-rw-   0        0        0     8892 2023-06-20 20:57:09.000000 gmsPython-0.0.4/gmsPython/gmsPyModels/gmsPyModels.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.907842 gmsPython-0.0.4/gmsPython/gmsWrite/
+-rw-rw-rw-   0        0        0     1402 2023-01-05 13:30:25.000000 gmsPython-0.0.4/gmsPython/gmsWrite/__init__.py
+-rw-rw-rw-   0        0        0     9269 2023-06-16 11:20:09.000000 gmsPython-0.0.4/gmsPython/gmsWrite/_gmsWrite.py
+-rw-rw-rw-   0        0        0     1423 2023-06-20 11:09:48.000000 gmsPython-0.0.4/gmsPython/gmsWrite/gmsWrite.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.910856 gmsPython-0.0.4/gmsPython/nestingTree/
+-rw-rw-rw-   0        0        0       73 2022-11-24 16:05:43.000000 gmsPython-0.0.4/gmsPython/nestingTree/__init__.py
+-rw-rw-rw-   0        0        0     9731 2023-06-22 12:28:19.000000 gmsPython-0.0.4/gmsPython/nestingTree/nestingTree.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:30:16.885920 gmsPython-0.0.4/gmsPython.egg-info/
+-rw-rw-rw-   0        0        0      496 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 12:30:16.000000 gmsPython-0.0.4/gmsPython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 12:30:16.913842 gmsPython-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-06-22 12:28:13.000000 gmsPython-0.0.4/setup.py
```

### Comparing `gmsPython-0.0.3/LICENSE` & `gmsPython-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.3/gmsPython/_mixedTools.py` & `gmsPython-0.0.4/gmsPython/_mixedTools.py`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.3/gmsPython/gmsPy/_gmsPy.py` & `gmsPython-0.0.4/gmsPython/gmsPy/_gmsPy.py`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.3/gmsPython/gmsPy/gmsPy.py` & `gmsPython-0.0.4/gmsPython/gmsPy/gmsPy.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,18 +120,20 @@
 		g = self.metagroup(g,db=db)
 		return {k:v for k,v in {s: self.var_ss(s,g,db=db) for s in g.conditions if s in gpyDB.symbols_db(db)}.items() if v is not None}
 
 	def inferVarExoFromVarEndo(self, var_endo, db = None):
 		db = pyDatabases.noneInit(db, self.db)
 		return {k: db[k] if k not in var_endo else gpyDB_wheels.adj.rc_AdjGpy(db[k], ('not',var_endo)) for k in self.Compile.getVariablesFromMetaGroup(self['g_exo']) if k in gpyDB.symbols_db(db)}
 
-	def partition_db(self,db=None):
+	def partition_db(self,db=None,checkOverlap = False):
 		db = self.db if db is None else db
 		d = {'non_var': db.getTypes(('set','subset','mapping','parameter','scalar_parameter')), 'var_endo': self.db_ss('g_endo',db=db), 'var_exo': self.db_ss('g_exo',db=db)}
-		# d['var_exo'] = self.inferVarExoFromVarEndo(d['var_endo'], db=db)
+		if checkOverlap:
+			d['var_exo'] = {k: v if k not in d['var_endo'] else gpyDB_wheels.adj.rc_AdjGpy(v, ('not',d['var_endo'][k])) for k,v in d['var_exo'].items()}
+			# d['var_exo'] = self.inferVarExoFromVarEndo(d['var_endo'], db=db)
 		d['residual'] = {k:v for k,v in db.getTypes(('scalar_variable','variable')).items() if k not in (list(d['var_endo'])+list(d['var_exo']))}
 		return d
 
 	# ---	2: Writing methods	--- #
 	def reset_Precompiler(self):
 		self.Precompiler = Precompiler(**(self.Precompiler_options | {'locals_': self.Precompiler.locals, 'user_functions': self.Precompiler.user_functions}))
```

### Comparing `gmsPython-0.0.3/gmsPython/gmsPyModels/gmsPyGlobals.py` & `gmsPython-0.0.4/gmsPython/gmsPyModels/gmsPyGlobals.py`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.3/gmsPython/gmsPyModels/gmsPyModels.py` & `gmsPython-0.0.4/gmsPython/gmsPyModels/gmsPyModels.py`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.3/gmsPython/gmsWrite/__init__.py` & `gmsPython-0.0.4/gmsPython/gmsWrite/__init__.py`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.3/gmsPython/gmsWrite/_gmsWrite.py` & `gmsPython-0.0.4/gmsPython/gmsWrite/_gmsWrite.py`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.3/gmsPython/gmsWrite/gmsWrite.py` & `gmsPython-0.0.4/gmsPython/gmsWrite/gmsWrite.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 
 def standardRun(settings, db, prefix =''):
 	return {prefix+'Fix': settings.Compile.fixGroupsText(db,settings['g_exo']), prefix+'Unfix': settings.Compile.unfixGroupsText(db,settings['g_endo']), 
 			prefix+'Model': writeModel(settings['name'], settings['blocks']), prefix+'Solve': writeSolve(solve=settings['solve'],name=settings['name'])}
 
 def SolveLoop(settings, dbT, db0 = None, name ='shock', subsetDB = True, loop = 'l1', solve=None, model=None, **kwargs):
 	if subsetDB:
-		x = settings.partition_db(db=dbT)
+		x = settings.partition_db(db=dbT, checkOverlap = True)
 		dbT.series.database = (x['non_var'] | x['var_exo'])
 	db = gridDB(noneInit(db0, settings.db), dbT, name, loop=loop,**kwargs)
 	text = loopUpdateSolve(loop, name, db, settings.db, db.updateDict, updateSolDict = db.updateSolDict, solve = noneInit(solve, settings['solve']), model = noneInit(solve, settings['name']))
 	return text, db
```

### Comparing `gmsPython-0.0.3/gmsPython/nestingTree/nestingTree.py` & `gmsPython-0.0.4/gmsPython/nestingTree/nestingTree.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,62 @@
 import pandas as pd, pyDatabases
-from pyDatabases import gpyDB, gpyDB_wheels
+from pyDatabases import gpyDB, gpyDB_wheels, adj, adjMultiIndex
 from gmsPython._mixedTools import concatMultiIndices
 
 _ftype_inputs, _ftype_outputs = ('CES','CES_norm','MNL'), ('CET','CET_norm','MNL_out')
 _scalePreserving = ('CES_norm','CET_norm','MNL','MNL_out')
 
 def checkOrIgnore(d,k):
 	return d[k] if k in d else k
 def reverseDict(d):
 	return {v:k for k,v in d.items()}
 
+def trimNestingStructure(m, sparsity, maxIter = 10):
+	""" Trim nesting structure in pandas multiindex 'm' with a 'sparsity' pattern on the inputs. NB: Only works on pure input-like trees """
+	t = tree(name = 'test', tree = m.tolist())
+	t.attrs_from_trees()
+	nInputs = sparsity.to_frame(index=False).groupby('s').count().n
+	oneInputSectors = nInputs[nInputs == 1]
+	# Define new mapping for relevant sectors:
+	mapOneInput = adjMultiIndex.applyMult(adj.rc_pd(t.get('output'), oneInputSectors), 
+										  adj.rc_pd(sparsity, oneInputSectors).rename(['s','nn']))
+	mMultipleGoods = adj.rc_pd(m, ('not', oneInputSectors))
+	t = tree(name = 'test', tree = mMultipleGoods.to_list())
+	t.attrs_from_tree()
+
+	# 2. Remove inputs that are not used:
+	noUse = adj.rc_pd(t.get('input'), ('not', sparsity))
+	mMultipleGoods = adj.rc_pd(t.get('map'), ('not', adj.rc_pd(noUse, alias = {'n':'nn'})))
+
+	# 2.A: Number of nodes for each parent node in the system:
+	nNodes = mMultipleGoods.to_frame(index=False).groupby(['s','n']).count()
+	i = 0
+	while min(nNodes['nn'])<=1:
+		i = i+1
+		mMultipleGoods, nNodes = trim_ite(mMultipleGoods, nNodes)
+		if i==maxIter:
+			raise StopIteration("Tree trimming did not converge")
+	return mMultipleGoods.union(mapOneInput)
+
+def trim_ite(m, nNodes):
+	# 2B: Define mapping where knots have a single node:
+	nodesOneChild = nNodes[nNodes['nn'] == 1].index
+	mapOneNode = adj.rc_pd(m, nodesOneChild)
+	# We make an exception if a combination (s, x) enters as both a knot and a branch. In this case, we cannot remove the parent node of 'x' (as we need this to maintain the tree structure)
+	keepKnots = adj.rc_pd(mapOneNode.droplevel('nn').unique(), mapOneNode.droplevel('n').rename(['s','n']))
+	nodesOneChild = nodesOneChild.difference(keepKnots)
+	mapOneNode = adj.rc_pd(m, nodesOneChild)
+	m = adj.rc_pd(m, ('not', nodesOneChild))
+	# Apply map to change parent nodes
+	mapNewNodes = adjMultiIndex.applyMult(m, mapOneNode.rename(['s','nn','new'])).droplevel('nn').rename(['s','n','nn'])
+	m = adj.rc_pd(m, ('not', nodesOneChild.rename(['s','nn']))).union(mapNewNodes)
+	# 2A: Return number of nodes for each one now:
+	nNodes = m.to_frame(index = False).groupby(['s','n']).count()
+	return m, nNodes
+
 class tree:
 	def __init__(self, name, tree = None, io = None, db = None, f = None,**ns):
 		self.name = name
 		self.db = pyDatabases.noneInit(db,{})
 		self.addFunctionandIO(f,io)
 		self.scalePreserving = True if self.f in _scalePreserving else False
 		self.ns = {k:v if k not in ns else ns[k] for k,v in self.standardNamespace.items()}
```

### Comparing `gmsPython-0.0.3/gmsPython.egg-info/SOURCES.txt` & `gmsPython-0.0.4/gmsPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmsPython-0.0.3/setup.py` & `gmsPython-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
   long_description = file.read()
 
 setuptools.setup(
   name="gmsPython",
-  version="0.0.3",
+  version="0.0.4",
   author="Rasmus K. Skjødt Berg",
   author_email="rasmus.kehlet.berg@econ.ku.dk",
   description="Automating GAMS models and execution from Python",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ChampionApe/gamsPythonModels",
   packages=setuptools.find_packages(),
```

