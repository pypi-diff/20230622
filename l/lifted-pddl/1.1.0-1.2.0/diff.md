# Comparing `tmp/lifted-pddl-1.1.0.tar.gz` & `tmp/lifted-pddl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifted-pddl-1.1.0.tar", last modified: Tue Nov 15 23:32:46 2022, max compression
+gzip compressed data, was "lifted-pddl-1.2.0.tar", last modified: Wed Nov 30 15:54:30 2022, max compression
```

## Comparing `lifted-pddl-1.1.0.tar` & `lifted-pddl-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 23:32:46.675652 lifted-pddl-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1066 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4572 2022-11-15 23:32:46.671652 lifted-pddl-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4078 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-15 23:32:46.675652 lifted-pddl-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      899 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 23:32:46.671652 lifted-pddl-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 23:32:46.671652 lifted-pddl-1.1.0/src/lifted_pddl/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/src/lifted_pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7941 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/src/lifted_pddl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 23:32:46.671652 lifted-pddl-1.1.0/src/lifted_pddl/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/src/lifted_pddl/data/blocksworld-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (122)      671 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/src/lifted_pddl/data/blocksworld-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (122)     1673 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/src/lifted_pddl/data/logistics-domain-exists.pddl
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/src/lifted_pddl/data/logistics-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (122)     2426 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/src/lifted_pddl/data/logistics-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (122)    28939 2022-11-15 23:32:35.000000 lifted-pddl-1.1.0/src/lifted_pddl/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 23:32:46.671652 lifted-pddl-1.1.0/src/lifted_pddl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4572 2022-11-15 23:32:46.000000 lifted-pddl-1.1.0/src/lifted_pddl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      584 2022-11-15 23:32:46.000000 lifted-pddl-1.1.0/src/lifted_pddl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-15 23:32:46.000000 lifted-pddl-1.1.0/src/lifted_pddl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2022-11-15 23:32:46.000000 lifted-pddl-1.1.0/src/lifted_pddl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-11-15 23:32:46.000000 lifted-pddl-1.1.0/src/lifted_pddl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-15 23:32:46.000000 lifted-pddl-1.1.0/src/lifted_pddl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 15:54:30.035423 lifted-pddl-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4977 2022-11-30 15:54:30.035423 lifted-pddl-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4483 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 15:54:30.035423 lifted-pddl-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 15:54:30.027423 lifted-pddl-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 15:54:30.031423 lifted-pddl-1.2.0/src/lifted_pddl/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7941 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 15:54:30.035423 lifted-pddl-1.2.0/src/lifted_pddl/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/data/blocksworld-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/data/blocksworld-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (122)     1673 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/data/logistics-domain-exists.pddl
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/data/logistics-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (122)     2426 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/data/logistics-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (122)     3492 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/data/sokoban-domain-no-clear.pddl
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/data/sokoban-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (122)    32663 2022-11-30 15:54:20.000000 lifted-pddl-1.2.0/src/lifted_pddl/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 15:54:30.031423 lifted-pddl-1.2.0/src/lifted_pddl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4977 2022-11-30 15:54:30.000000 lifted-pddl-1.2.0/src/lifted_pddl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2022-11-30 15:54:30.000000 lifted-pddl-1.2.0/src/lifted_pddl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 15:54:30.000000 lifted-pddl-1.2.0/src/lifted_pddl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2022-11-30 15:54:30.000000 lifted-pddl-1.2.0/src/lifted_pddl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2022-11-30 15:54:30.000000 lifted-pddl-1.2.0/src/lifted_pddl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-30 15:54:30.000000 lifted-pddl-1.2.0/src/lifted_pddl.egg-info/top_level.txt
```

### Comparing `lifted-pddl-1.1.0/LICENSE` & `lifted-pddl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.1.0/PKG-INFO` & `lifted-pddl-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifted-pddl
-Version: 1.1.0
+Version: 1.2.0
 Summary: A lightweight framework for parsing PDDL in lifted form.
 Home-page: https://github.com/AI-Planning/lifted-pddl
 Author: Carlos Núñez Molina
 Author-email: ccaarlos@ugr.es
 License: MIT
 Keywords: automated_planning PDDL parser
 Classifier: License :: OSI Approved :: MIT License
@@ -83,12 +83,22 @@
 
 - Get next state:
 
 		lifted_pddl get_next_state -d path_to_domain -p path_to_problem -a action_to_apply
 
 ## Limitations
 
-At the moment, Lifted PDDL only supports typed STRIPS and existential preconditions (`:requirements :typing :existential-preconditions`). In the future, it will be extended to support ADL and, maybe, other PDDL requirements. We also welcome contributions. The code is brief, simple to understand and has many comments, so I encourage you to implement any functionality you need and submit a pull request to the [Github](https://github.com/AI-Planning/lifted-pddl)! 😄
+At the moment, Lifted PDDL supports the following PDDL extensions:
+
+- Types (`:typing`).
+
+- Existential preconditions (`:existential-preconditions`), i.e., `(exists ...)` constructions in action preconditions.
+
+- Limited support for negative preconditions (`:negative-preconditions`), i.e., `(not ...)` constructions in action preconditions. However,
+  negative compound formulas are not supported, i.e., constructions like `(exists (not ...))` and `(not (and ...))`. At the moment, we only support
+  negated atoms in preconditions.
+
+In the future, Lifted PDDL will be extended to support ADL and, maybe, other PDDL requirements. We also welcome contributions. The code is brief, simple to understand and has many comments, so I encourage you to implement any functionality you need and submit a pull request to the [Github](https://github.com/AI-Planning/lifted-pddl)! 😄
 
 ## Authors
 
  - [Carlos Núñez Molina](https://github.com/TheAeryan)
```

### Comparing `lifted-pddl-1.1.0/README.md` & `lifted-pddl-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -68,12 +68,22 @@
 
 - Get next state:
 
 		lifted_pddl get_next_state -d path_to_domain -p path_to_problem -a action_to_apply
 
 ## Limitations
 
-At the moment, Lifted PDDL only supports typed STRIPS and existential preconditions (`:requirements :typing :existential-preconditions`). In the future, it will be extended to support ADL and, maybe, other PDDL requirements. We also welcome contributions. The code is brief, simple to understand and has many comments, so I encourage you to implement any functionality you need and submit a pull request to the [Github](https://github.com/AI-Planning/lifted-pddl)! 😄
+At the moment, Lifted PDDL supports the following PDDL extensions:
+
+- Types (`:typing`).
+
+- Existential preconditions (`:existential-preconditions`), i.e., `(exists ...)` constructions in action preconditions.
+
+- Limited support for negative preconditions (`:negative-preconditions`), i.e., `(not ...)` constructions in action preconditions. However,
+  negative compound formulas are not supported, i.e., constructions like `(exists (not ...))` and `(not (and ...))`. At the moment, we only support
+  negated atoms in preconditions.
+
+In the future, Lifted PDDL will be extended to support ADL and, maybe, other PDDL requirements. We also welcome contributions. The code is brief, simple to understand and has many comments, so I encourage you to implement any functionality you need and submit a pull request to the [Github](https://github.com/AI-Planning/lifted-pddl)! 😄
 
 ## Authors
 
  - [Carlos Núñez Molina](https://github.com/TheAeryan)
```

### Comparing `lifted-pddl-1.1.0/setup.py` & `lifted-pddl-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='lifted-pddl',
-      version='1.1.0',
+      version='1.2.0',
       description='A lightweight framework for parsing PDDL in lifted form.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/AI-Planning/lifted-pddl',
       author='Carlos Núñez Molina',
       author_email='ccaarlos@ugr.es',
       license='MIT',
```

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl/__main__.py` & `lifted-pddl-1.2.0/src/lifted_pddl/__main__.py`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl/data/blocksworld-domain.pddl` & `lifted-pddl-1.2.0/src/lifted_pddl/data/blocksworld-domain.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl/data/blocksworld-problem.pddl` & `lifted-pddl-1.2.0/src/lifted_pddl/data/blocksworld-problem.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl/data/logistics-domain-exists.pddl` & `lifted-pddl-1.2.0/src/lifted_pddl/data/logistics-domain-exists.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl/data/logistics-domain.pddl` & `lifted-pddl-1.2.0/src/lifted_pddl/data/logistics-domain.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl/data/logistics-problem.pddl` & `lifted-pddl-1.2.0/src/lifted_pddl/data/logistics-problem.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl/parser.py` & `lifted-pddl-1.2.0/src/lifted_pddl/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 """
 This class implements functionality for:
 	- Parsing PDDL domains and problems
 	- Obtaining the actions applicable at the init state of the corresponding problem
 	- Obtaining the next state resulting from applying an action to the init state (successor function)
 
-<Limitations>: it supports types (as in typed STRIPS) and existential preconditions but not other PDDL extensions, such as
-               negative preconditions, disjuntions (or), conditional effects (:when), etc.
-               However, this code should be easy to extend to those situations.
+<Limitations>: it only supports:
+				- types (as in typed STRIPS) 
+				- existential preconditions
+				- negative preconditions (although only negative atoms and not negative compound formulas)
 """
 class Parser:
 
 	def __init__(self):
 		self._reader = PDDLReader(raise_on_error=True)
 
 		# Domain information
@@ -110,16 +111,17 @@
 			
 			# Obtain variables in action parameters
 			variables = action[1].parameters.vars()
 			variables_class = ['param']*len(variables) # Class of each variable: either 'param' (action parameter) or 'exists' (variable introduced by existential precondition)
 
 			# Obtain variables in existential preconditions
 			preconds = action[1].precondition
-			preconds = preconds.subformulas if isinstance(preconds, CompoundFormula) else [preconds]
-			exist_variables = [var for precond in preconds if (isinstance(precond, QuantifiedFormula) and precond.quantifier.name == 'Exists') for var in precond.variables]
+			# preconds = preconds.subformulas if isinstance(preconds, CompoundFormula) else [preconds] # Previous version
+			preconds_subformulas = preconds.subformulas if isinstance(preconds, CompoundFormula) else [preconds]
+			exist_variables = [var for precond in preconds_subformulas if (isinstance(precond, QuantifiedFormula) and precond.quantifier.name == 'Exists') for var in precond.variables]
 			
 			# <Note>: It is important that variables corresponding to action parameters go before variables corresponding to existential preconditions
 			variables.extend(exist_variables)
 			variables_class.extend(['exists']*len(exist_variables))
 			variables_class = tuple(variables_class)
 
 			# Obtain variable names
@@ -128,32 +130,91 @@
 			# Action variables, as a tuple of their types
 			# It includes all action variables. Right now, that means it includes action parameters and variables introduced by existential preconditions
 			# To see what each variable corresponds to, use is_action_param and has_exist_quantifier.
 			# Example: ('truck', 'location', 'location', 'city')
 			action_variables = tuple([var.sort.name for var in variables])
 
 			# Action preconditions, as a tuple made up of every precondition
-			# Each precondition is represented by a tuple (predicate_name, vars)
+			# Each precondition is represented by a tuple (preffix, predicate_name, vars)
+			# Preffix is False if the precondition is a negative precondition, and True otherwise
 			# Variables are substituted by their corresponding parameter index
-			# Example: ( ('at', (0, 1)), ('in-city', (1, 3)), ('in-city', (2, 3)) )
+			# Example: ( (True, 'at', (0, 1)), (False, 'in-city', (1, 3)), (True, 'in-city', (2, 3)) )
 
+			# preconds is a negated formula
+			if isinstance(preconds, CompoundFormula) and preconds.connective.name.lower() == 'not':
+				preconds_list = [(False, preconds)]
+			else:
+				preconds_list = [(True, preconds)]
+
+			preconds_modified = True
+			# Recursively process the formulas and subformulas in preconds_list
+			# until we have removed all the nesting levels (i.e., obtained all the subformulas
+			# and removed all the existential preconditions)
+			while preconds_modified:
+				new_preconds_list = []
+				preconds_modified = False
+
+				# Remove one nesting level of the formulas in preconds_list
+				for preffix, formula in preconds_list:
+					# If it is a compoundformula, split it into its subformulas
+					if isinstance(formula, CompoundFormula):
+
+						# Negated formula -> we negate the preffix (True -> False, False -> True)
+						if formula.connective.name.lower() == 'not':
+							subformulas = formula.subformulas
+
+							# If this condition is met, then it means that the negated formula contains
+							# several subformulas (i.e., it is in the form of (not (and ...))  )
+							# We can't parse compound negated subformulas at the moment
+							if len(subformulas) > 1 or not isinstance(subformulas[0], Atom):
+								raise Exception("We can't parse negative compound formulas in the preconditions, i.e., '(not (and ...))'")
+
+							subformulas = [(not preffix, f) for f in subformulas]
+							new_preconds_list.extend(subformulas)
+						
+						# Compound formula which is not a negation, but a conjuntion (and ...)
+						else:
+							subformulas = [(preffix, f) for f in formula.subformulas]
+							new_preconds_list.extend(subformulas)
+
+						preconds_modified = True
+
+					# If it has an existential quantifier, just ignore the quantifier
+					elif isinstance(formula, QuantifiedFormula):
+						
+						if preffix == False:
+							raise Exception("We can't parse preconditions of the type '(not (exists ... ))'")
+
+						new_preconds_list.append((preffix, formula.formula))
+						preconds_modified = True
+
+					# Else, it is a simple formula, so we add it
+					else:
+						new_preconds_list.append((preffix, formula))
+
+				preconds_list = new_preconds_list
+
+
+			"""
+			# Previous version
 			# Decompose QuantifiedFormulas into their subformulas (while ignoring the quantifier)
 			preconds_list = []
 			for precond in preconds:
 				if isinstance(precond, QuantifiedFormula):
 					formula = precond.formula
 
 					if isinstance(formula, CompoundFormula):
 						preconds_list.extend(formula.subformulas)
 					else:
 						preconds_list.append(formula)
 				else:
 					preconds_list.append(precond)
+			"""
 
-			preconds_tuple = tuple([(precond.predicate.name, tuple([var_names.index(var.symbol) for var in precond.subterms])) for precond in preconds_list])
+			preconds_tuple = tuple([(preffix, precond.predicate.name, tuple([var_names.index(var.symbol) for var in precond.subterms])) for preffix, precond in preconds_list])
 
 			# Action effects, as a tuple made up of every effect
 			# Each effect is represented as a tuple (is_add_effect, predicate_name, vars)
 			# Variables are substituted by their corresponding parameter index
 			# Example: ( (False, 'at', (0, 1)), (True, 'at', (0, 2)) ))
 			effects = action[1].effects
 			effects = tuple([(isinstance(effect, AddEffect), effect.atom.predicate.name, tuple([var_names.index(var.symbol) for var in effect.atom.subterms])) for effect in effects])
@@ -218,15 +279,14 @@
 				- Check if the atom objects corresponding to bound variables match the objects of the partial variable assignment
 				- If true, add a new variable assignment:
 					- Copy the old variable assignment
 					- For each atom's object, change the corresponding object of the variable assignment to it (bind new variables)
 	4. Return valid (applicable) variable assignments for the action.
 	"""
 
-
 	"""
 	Auxiliary function used by get_applicable_actions. It receives a set of variable assignments (each one with an arbitrary number of free and bind variables),
 	and returns a list with all the full variable assignments obtained from them and which correspond to applicable ground actions.
 	The full variable assignments are returned as a tuple of tuples.
 
 	<Note>: @_var_assigns must be a list of lists
 	"""
@@ -242,35 +302,40 @@
 		# Check nullary preconditions
 		# If they are not met, there are no applicable ground actions (and, hence, no valid var assignments)
 
 		# Process action preconditions corresponding to nullary predicates (those of arity 0)
 		# Check if each nullary predicate in the preconditions appears in the state atoms.
 		# If so, we remove the nullary predicates from the action preconditions and check the rest of the preconditions.
 		# If not, the action is not applicable.
-		nullary_preconds = [precond for precond in action_preconds if len(precond[1]) == 0]
+		nullary_preconds = [precond for precond in action_preconds if len(precond[2]) == 0]
 
 		nullary_preconds_in_atoms = True
 		for nullary_precond in nullary_preconds:
-			if nullary_precond not in atoms: # The nullary precondition does not appear in the atoms
+			if nullary_precond[1:] not in atoms: # The nullary precondition does not appear in the atoms
 				nullary_preconds_in_atoms = False
 				break
 
 		# The current action is not applicable
 		if not nullary_preconds_in_atoms:
 			return tuple() # empty tuple
 
 		# Remove the nullary predicates from the action preconditions
-		action_preconds = [precond for precond in action_preconds if len(precond[1]) > 0]
+		action_preconds = [precond for precond in action_preconds if len(precond[2]) > 0]
+
+		# Split the preconditions into positive and negative (i.e., (not ...))
+		positive_preconds = [precond for precond in action_preconds if precond[0]==True]
+		negative_preconds = [precond for precond in action_preconds if precond[0]==False]
 
 		# List of (possibly partial) variable assignments corresponding to potentially aplicable actions
 		var_assigns = copy.deepcopy(_var_assigns) # Deep copy the parameter so that it is not modified
 		is_var_bound = [var != -1 for var in var_assigns[0]] # Contains True if the corresponding variable is bound, and False if it's free
 
-		for precond in action_preconds:
-			precond_pred, precond_vars = precond
+		# Process the positive preconditions -> obtain the list of variable assignments which satisfy the positive preconditions
+		for precond in positive_preconds:
+			_, precond_pred, precond_vars = precond
 			new_var_assigns = [] # Will contain the partial variable assignments after we process the current precondition (precond)
 
 			# Obtain mapping from the indexes of the atom's objects to the indexes of the variables in var_assigns
 			# Then, select the subset of those indexes which we need to check to see if an atom matches a variable assignment in var_assigns
 			# This subset corresponds to those variables which are already bound and also appear at the precondition (precond_vars)
 			"""
 			Examples:
@@ -341,14 +406,39 @@
 			# If var != -1 -> simply var
 			new_objs_var_assign = [[ind_obj for ind_obj, obj_type in enumerate(objects) if obj_type==action_vars[ind_var]] \
 			 					   if var==-1 else (var,) for ind_var, var in enumerate(var_assign)]
 
 			new_var_assigns = product(*new_objs_var_assign) # Cartesian product
 			full_var_assigns.extend(new_var_assigns)
 
+
+		# <Negative preconditions>
+		# Remove the variable substitutions which do not satisfy the negative preconditions
+		for precond in negative_preconds: 
+			_, precond_pred, precond_vars = precond
+			new_var_assigns = []
+
+			# Check if each var_assign meets the current negative precondition
+			for var_assign in full_var_assigns:
+				# Substitute the precondition variables by the objects given by var_assign
+				precond_objs = tuple([var_assign[var] for var in precond_vars])
+				ground_precond = (precond_pred, precond_objs)
+
+				# Check if the grounded precondition is in the state atoms
+				if ground_precond not in atoms:
+					new_var_assigns.append(var_assign)
+
+			full_var_assigns = new_var_assigns
+
+			# If there are no var_assigns left, we know that no variable substitution
+			# satisfies all the preconditions
+			if len(full_var_assigns) == 0:
+				return tuple()
+
+
 		# <Existential preconditions>
 		# Remove variables corresponding to existential preconditions from full_var_assigns.
 		# We do this because these variables are not action parameters and we know that, for all variable assignments in
 		# full_var_assigns, the existential preconditions are met.
 		# Example: if the second variable is introduced by an existential precondition, then:
 		# 		   full_var_assigns = [[1,2,3], [4,5,6], [1,7,3]] -> [[1,3], [4,6], [1,3]] --- 
 		#          -- <remove repeated assignments> ---> [[1,3], [4,6]]
```

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl.egg-info/PKG-INFO` & `lifted-pddl-1.2.0/src/lifted_pddl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifted-pddl
-Version: 1.1.0
+Version: 1.2.0
 Summary: A lightweight framework for parsing PDDL in lifted form.
 Home-page: https://github.com/AI-Planning/lifted-pddl
 Author: Carlos Núñez Molina
 Author-email: ccaarlos@ugr.es
 License: MIT
 Keywords: automated_planning PDDL parser
 Classifier: License :: OSI Approved :: MIT License
@@ -83,12 +83,22 @@
 
 - Get next state:
 
 		lifted_pddl get_next_state -d path_to_domain -p path_to_problem -a action_to_apply
 
 ## Limitations
 
-At the moment, Lifted PDDL only supports typed STRIPS and existential preconditions (`:requirements :typing :existential-preconditions`). In the future, it will be extended to support ADL and, maybe, other PDDL requirements. We also welcome contributions. The code is brief, simple to understand and has many comments, so I encourage you to implement any functionality you need and submit a pull request to the [Github](https://github.com/AI-Planning/lifted-pddl)! 😄
+At the moment, Lifted PDDL supports the following PDDL extensions:
+
+- Types (`:typing`).
+
+- Existential preconditions (`:existential-preconditions`), i.e., `(exists ...)` constructions in action preconditions.
+
+- Limited support for negative preconditions (`:negative-preconditions`), i.e., `(not ...)` constructions in action preconditions. However,
+  negative compound formulas are not supported, i.e., constructions like `(exists (not ...))` and `(not (and ...))`. At the moment, we only support
+  negated atoms in preconditions.
+
+In the future, Lifted PDDL will be extended to support ADL and, maybe, other PDDL requirements. We also welcome contributions. The code is brief, simple to understand and has many comments, so I encourage you to implement any functionality you need and submit a pull request to the [Github](https://github.com/AI-Planning/lifted-pddl)! 😄
 
 ## Authors
 
  - [Carlos Núñez Molina](https://github.com/TheAeryan)
```

### Comparing `lifted-pddl-1.1.0/src/lifted_pddl.egg-info/SOURCES.txt` & `lifted-pddl-1.2.0/src/lifted_pddl.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 src/lifted_pddl.egg-info/entry_points.txt
 src/lifted_pddl.egg-info/requires.txt
 src/lifted_pddl.egg-info/top_level.txt
 src/lifted_pddl/data/blocksworld-domain.pddl
 src/lifted_pddl/data/blocksworld-problem.pddl
 src/lifted_pddl/data/logistics-domain-exists.pddl
 src/lifted_pddl/data/logistics-domain.pddl
-src/lifted_pddl/data/logistics-problem.pddl
+src/lifted_pddl/data/logistics-problem.pddl
+src/lifted_pddl/data/sokoban-domain-no-clear.pddl
+src/lifted_pddl/data/sokoban-problem.pddl
```

