# Comparing `tmp/pyscal_rdf-0.0.4.tar.gz` & `tmp/pyscal_rdf-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal_rdf-0.0.4.tar", last modified: Mon Jun 19 12:54:55 2023, max compression
+gzip compressed data, was "pyscal_rdf-0.0.6.tar", last modified: Thu Jun 22 12:29:22 2023, max compression
```

## Comparing `pyscal_rdf-0.0.4.tar` & `pyscal_rdf-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:54:55.720770 pyscal_rdf-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-19 12:54:55.720770 pyscal_rdf-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:54:55.716771 pyscal_rdf-0.0.4/pyscal_rdf/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    29501 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/json_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/rdfutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/pyscal_rdf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:54:55.716771 pyscal_rdf-0.0.4/pyscal_rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-19 12:54:55.000000 pyscal_rdf-0.0.4/pyscal_rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-19 12:54:55.000000 pyscal_rdf-0.0.4/pyscal_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:54:55.000000 pyscal_rdf-0.0.4/pyscal_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:54:55.000000 pyscal_rdf-0.0.4/pyscal_rdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-19 12:54:55.000000 pyscal_rdf-0.0.4/pyscal_rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 12:54:55.000000 pyscal_rdf-0.0.4/pyscal_rdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:54:55.720770 pyscal_rdf-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-19 12:54:55.000000 pyscal_rdf-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:54:55.716771 pyscal_rdf-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/tests/test_rdfutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-19 12:54:52.000000 pyscal_rdf-0.0.4/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:29:22.546357 pyscal_rdf-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-22 12:29:22.546357 pyscal_rdf-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:29:22.542357 pyscal_rdf-0.0.6/pyscal_rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:29:22.542357 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 12:29:22.546357 pyscal_rdf-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:29:22.546357 pyscal_rdf-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_structuregraph.py
```

### Comparing `pyscal_rdf-0.0.4/LICENSE` & `pyscal_rdf-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.4/PKG-INFO` & `pyscal_rdf-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal_rdf
-Version: 0.0.4
+Version: 0.0.6
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal_rdf-0.0.4/README.md` & `pyscal_rdf-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf/graph.py` & `pyscal_rdf-0.0.6/pyscal_rdf/graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from rdflib.store import NO_STORE, VALID_STORE
 
 import os
 import numpy as np
 from ase.io import write
 
 from pyscal_rdf.visualize import visualize_graph
-from pyscal_rdf.rdfutils import convert_to_dict
 from pyscal_rdf.network import OntologyNetwork
+import pyscal_rdf.properties as prp
 from pyscal.core import System
 from pyscal.atoms import Atoms
 from pyscal.core import System
 
 CMSO = Namespace("https://purls.helmholtz-metadaten.de/cmso/")
 PLDO = Namespace("https://purls.helmholtz-metadaten.de/pldo/")
 PODO = Namespace("https://purls.helmholtz-metadaten.de/podo/")
@@ -44,54 +44,149 @@
             if isinstance(val, dict):
                 _replace_keys(refdict[key], indict[key])
             else:
                 refdict[key] = val
     return refdict
 
 class RDFGraph:
-    def __init__(self, graph_file=None):
-        self.graph = Graph()
+    def __init__(self, graph_file=None, 
+        store="Memory", 
+        store_file=None,
+        identifier="default_graph"):
+        self.graph = Graph(store=store, identifier=identifier)
         #owlfile = os.path.join(os.path.dirname(__file__), "data/cmso.owl")
         #self.graph.parse(owlfile, format='xml')
-
+        if store != "Memory":
+            if not store=="SQLAlchemy":
+                raise ValueError("Only SQLAlchemy store is supported")
+            if store_file is None:
+                raise ValueError("store file is needed if store is not memory")
+            uri = Literal(f"sqlite:///{store_file}")
+            self.graph.open(uri, create=True)
         self.graph.bind("cmso", CMSO)
         self.graph.bind("pldo", PLDO)
+        
         if graph_file is not None:
             if os.path.exists(graph_file):
                 self.graph.parse(graph_file)
         self.sample = None
         self.material = None
         self.sysdict = None
         self.sgraph = None
         self._query_graph = OntologyNetwork()
     
-    def process_structure(self, structure):
+    def process_structure(self, structure, format=None):
         """
         Convert a given :py:class:`pyscal.core.System` to a data dictionary which can be used for annotation
         and storing the data in the RDF Graph.
 
         Parameters
         ----------
         structure: :py:class:`pyscal.core.System`
             input structure
 
         Returns
         -------
         None
         """
         if isinstance(structure, System):
-            self.sysdict = convert_to_dict(structure)
+            #self.sysdict = convert_to_dict(structure)
+            self.sys = structure
         elif os.path.exists(structure):
             sys = System(structure, format=format)
-            self.sysdict = convert_to_dict(sys)
+            #self.sysdict = convert_to_dict(sys)
+            self.sys = sys
     
     def data(self, key):
-        if self.sysdict is not None:
-            if key in self.sysdict:
-                return self.sysdict[key]
+        #this method gets info directly from the dict
+        if key=="ChemicalCompositionElement":
+            return list(self.sys.composition.keys())
+        elif key=="ChemicalCompositionRatio":
+            return [val for key, val in self.sys.composition.items()]
+        elif key=="CellVolume":
+            return self.sys.volume
+        elif key=="NumberOfAtoms":
+            return self.sys.natoms
+        elif key=="SimulationCellLengthX":
+            return self.sys.box_dimensions[0]
+        elif key=="SimulationCellLengthY":
+            return self.sys.box_dimensions[1]
+        elif key=="SimulationCellLengthZ":
+            return self.sys.box_dimensions[2]
+
+        elif key=="SimulationCellVectorA":
+            return self.sys.box[0]
+        elif key=="SimulationCellVectorB":
+            return self.sys.box[1]
+        elif key=="SimulationCellVectorC":
+            return self.sys.box[2]
+        
+        elif key=="SimulationCellAngleAlpha":
+            return prp.get_angle(self.sys.box[0], self.sys.box[1])
+        elif key=="SimulationCellAngleBeta":
+            return prp.get_angle(self.sys.box[1], self.sys.box[2])
+        elif key=="SimulationCellAngleGamma": 
+            return prp.get_angle(self.sys.box[2], self.sys.box[0])
+        
+        elif key=="Element":
+            if self.sys.atoms.species[0] is not None:
+                return self.sys.atoms.species
+            else:
+                return self.sys.atoms.types
+        elif key=="Coordination":
+            return prp.get_coordination(self.sys)
+        elif key=="Positions":
+            return self.sys.atoms.positions
+        elif key=="LatticeParameter":
+            return self.sys.atoms._lattice_constant      
+        
+        elif key=="SpaceGroupSymbol":
+            if self.sys._structure_dict is not None:
+                symbol, number = prp.get_space_group(self.sys)
+                return symbol
+        elif key=="SpaceGroupNumber":
+            if self.sys._structure_dict is not None:
+                symbol, number = prp.get_space_group(self.sys)
+                return number
+            else:
+                return None
+
+        elif key=="CrystalStructureName":
+            if self.sys._structure_dict is not None:
+                return self.sys.atoms._lattice 
+            else:
+                return None
+
+        elif key=="BravaisLattice":
+            if self.sys._structure_dict is not None:
+                return prp.get_bravais_lattice(self.sys)
+            else:
+                return None
+
+        elif key=="BasisPositions":
+            if self.sys._structure_dict is not None:
+                return self.sys._structure_dict['positions']
+            else:
+                return None
+
+        elif key=="BasisOccupancy":
+            if self.sys._structure_dict is not None:
+                return prp.get_basis(self.sys)
+            else:
+                return None
+
+        elif key=="LatticeVectors":
+            if self.sys._structure_dict is not None:
+                return prp.get_lattice_vector(self.sys)
+            else:
+                return None
+
+        #if self.sysdict is not None:
+        #    if key in self.sysdict:
+        #        return self.sysdict[key]
         return None
     
     def add(self, triple):
         if str(triple[2].toPython()) != 'None':
             self.graph.add(triple)
         
     def add_structure_to_graph(self, structure, names=False, name_index=None, format=None):
@@ -106,22 +201,22 @@
         names: bool
             if True, alphanumeric names will be used instead of random BNodes
 
         Returns
         -------
         None
         """
-        self.process_structure(structure)
+        self.process_structure(structure, format=format)
         #now add to graph
         if name_index is None:
             name_index = self.n_samples + 1
         self.create_graph(names=names, name_index=name_index)
         
     
-    def create_graph(self, names=False, name_index="01"):
+    def create_graph(self, names=False, name_index="1"):
         """
         Create the RDF Graph from the data stored
 
         Parameters
         ----------
         names: bool
             if True, alphanumeric names will be used instead of random BNodes
@@ -131,19 +226,19 @@
         
         Returns
         -------
         None
         """
 
         if names:
-            name_list = [f'{name_index}_Sample', f'{name_index}_Material',
-                        f'{name_index}_ChemicalComposition', f'{name_index}_SimulationCell',
-                        f'{name_index}_SimulationCell', f'{name_index}_CrystalStructure',
-                        f'{name_index}_SpaceGroup', f'{name_index}_UnitCell',
-                        f'{name_index}_UnitCell', f'{name_index}_Atom']
+            name_list = [f'Sample_{name_index}', f'Material_{name_index}',
+                        f'ChemicalComposition_{name_index}', f'SimulationCell_{name_index}',
+                        f'SimulationCell_{name_index}', f'CrystalStructure_{name_index}',
+                        f'SpaceGroup_{name_index}', f'UnitCell_{name_index}',
+                        f'UnitCell_{name_index}', f'Atom_{name_index}']
         else:
             name_list = [None, None,
                         None, None,
                         None, None,
                         None, None,
                         None, None]
         self.add_sample(name=name_list[0])
@@ -152,14 +247,28 @@
         self.add_simulation_cell(name=name_list[3])
         self.add_simulation_cell_properties(name=name_list[4])
         self.add_crystal_structure(name=name_list[5])
         self.add_space_group(name=name_list[6])
         self.add_unit_cell(name=name_list[7])
         self.add_lattice_properties(name=name_list[8])
         self.add_atoms(name=name_list[9])
+
+        self.add((CMSO.SimulationCellLength, RDFS.subClassOf, CMSO.Length))
+        self.add((CMSO.LatticeParameter, RDFS.subClassOf, CMSO.Length))
+        self.add((CMSO.Length, CMSO.hasUnit, URIRef("https://qudt.org/2.1/vocab/unit#ANGSTROM")))
+        
+        self.add((CMSO.SimulationCellAngle, RDFS.subClassOf, CMSO.Angle))
+        self.add((CMSO.LatticeAngle, RDFS.subClassOf, CMSO.Angle))
+        self.add((CMSO.Angle, CMSO.hasUnit, URIRef("https://qudt.org/2.1/vocab/unit#DEG")))
+        
+        self.add((CMSO.LatticeVector, RDFS.subClassOf, CMSO.Vector))
+        self.add((CMSO.SimulationCellVector, RDFS.subClassOf, CMSO.Vector))
+        self.add((CMSO.PositionVector, RDFS.subClassOf, CMSO.Vector))
+        self.add((CMSO.Vector, CMSO.hasUnit, URIRef("https://qudt.org/2.1/vocab/unit#ANGSTROM")))
+        
         
     def add_sample(self, name=None):
         """
         Add a CMSO Sample object
 
         Parameters
         ----------
@@ -201,20 +310,17 @@
         name
             if provided, the name will be used instead of random identifier
 
         Returns
         -------
         """
 
-        chem_comp = ["=".join([x, str(y)]) for x,y in zip(self.data("ChemicalCompositionElement"), self.data("ChemicalCompositionRatio"))]
-        chemical_composition_01 = BNode(name)
-        self.add((self.material, CMSO.hasComposition, chemical_composition_01))
-        self.add((chemical_composition_01, RDF.type, CMSO.ChemicalComposition))
+        chem_comp = ["=".join([str(x), str(y)]) for x,y in zip(self.data("ChemicalCompositionElement"), self.data("ChemicalCompositionRatio"))]
         for x in range(len(chem_comp)):
-            self.add((chemical_composition_01, CMSO.hasElementRatio, Literal(chem_comp[x], datatype=XSD.string)))
+            self.add((self.material, CMSO.hasElementRatio, Literal(chem_comp[x], datatype=XSD.string)))
     
     def add_simulation_cell(self, name=None):
         """
         Add a CMSO SimulationCell
 
         Parameters
         ----------
@@ -325,20 +431,16 @@
         ----------
         name
             if provided, the name will be used instead of random identifier
 
         Returns
         -------
         """
-
-        space_group_01 = BNode(name)
-        self.add((self.crystal_structure, CMSO.hasSpaceGroup, space_group_01))
-        self.add((space_group_01, RDF.type, CMSO.SpaceGroup))
-        self.add((space_group_01, CMSO.hasSpaceGroupSymbol, Literal(self.data("SpaceGroupSymbol"), datatype=XSD.string)))
-        self.add((space_group_01, CMSO.hasSpaceGroupNumber, Literal(self.data("SpaceGroupNumber"), datatype=XSD.integer)))
+        self.add((self.crystal_structure, CMSO.hasSpaceGroupSymbol, Literal(self.data("SpaceGroupSymbol"), datatype=XSD.string)))
+        self.add((self.crystal_structure, CMSO.hasSpaceGroupNumber, Literal(self.data("SpaceGroupNumber"), datatype=XSD.integer)))
     
             
     def add_unit_cell(self, name=None):
         """
         Add a CMSO Unit Cell
 
         Parameters
@@ -352,21 +454,18 @@
 
         unit_cell_01 = BNode(name)
         self.add((self.crystal_structure, CMSO.hasUnitCell, unit_cell_01))
         self.add((unit_cell_01, RDF.type, CMSO.UnitCell))
         self.unit_cell = unit_cell_01
         
         #add bravais lattice
-        uname = None
-        if name is not None:
-            uname = f'Bravais{name}'
-        bravaislattice = BNode(uname)
-        self.add((self.unit_cell, CMSO.hasLattice, bravaislattice))
-        self.add((bravaislattice, RDF.type, CMSO.BravaisLattice))
-        self.add((bravaislattice, CMSO.hasLatticeSystem, Literal(self.data("BravaisLattice"), datatype=XSD.string)))
+        bv = None
+        if self.data("BravaisLattice") is not None:
+            bv = URIRef(self.data("BravaisLattice"))
+            self.add((self.unit_cell, CMSO.hasBravaisLattice, bv))
         
     def add_lattice_properties(self, name=None):
         """
         Add CMSO lattice properties such as Lattice Parameter,
         and its lengths and angles. 
 
         Parameters
@@ -477,40 +576,42 @@
         elif gb_dict["GBType"] == "Symmetric Tilt":
             self.add((plane_defect_01, RDF.type, PLDO.SymmetricTiltBoundary))
         elif gb_dict["GBType"] == "Mixed":
             self.add((plane_defect_01, RDF.type, PLDO.MixedBoundary))
         self.add((plane_defect_01, PLDO.hasSigmaValue, Literal(gb_dict["sigma"], datatype=XSD.integer)))
         
         #now mark that the defect is GB
-        uname = None
-        if name is not None:
-            uname = f'{name}GrainBoundaryPlane'
-        gb_plane_01 = BNode(uname)
-        self.add((plane_defect_01, PLDO.hasGBPlane, gb_plane_01))
-        self.add((gb_plane_01, RDF.type, PLDO.GrainBoundaryPlane))
-        self.add((gb_plane_01, PLDO.hasMillerIndices, Literal(gb_dict["GBPlane"], 
+        #uname = None
+        #if name is not None:
+        #    uname = f'{name}GrainBoundaryPlane'
+        #gb_plane_01 = BNode(uname)
+        self.add((plane_defect_01, PLDO.hasGBPlane, Literal(gb_dict["GBPlane"], 
                                                              datatype=XSD.string)))
-        
-        uname = None
-        if name is not None:
-            uname = f'{name}RotationAxis'
-        rotation_axis_01 = BNode(uname)
-        self.add((plane_defect_01, PLDO.hasRotationAxis, rotation_axis_01))
-        self.add((rotation_axis_01, RDF.type, PLDO.RotationAxis))
-        self.add((rotation_axis_01, PLDO.hasComponentX, Literal(gb_dict["RotationAxis"][0], datatype=XSD.float)))
-        self.add((rotation_axis_01, PLDO.hasComponentY, Literal(gb_dict["RotationAxis"][1], datatype=XSD.float)))
-        self.add((rotation_axis_01, PLDO.hasComponentZ, Literal(gb_dict["RotationAxis"][2], datatype=XSD.float)))
-
-        uname = None
-        if name is not None:
-            uname = f'{name}MisorientationAngle'
-        misorientation_angle_01 = BNode(uname)
-        self.add((plane_defect_01, PLDO.hasMisorientationAngle, misorientation_angle_01))
-        self.add((misorientation_angle_01, RDF.type, PLDO.MisorientationAngle))
-        self.add((misorientation_angle_01, PLDO.hasAngle, Literal(gb_dict["MisorientationAngle"], datatype=XSD.float)))    
+        #self.add((gb_plane_01, RDF.type, PLDO.GrainBoundaryPlane))
+        #self.add((gb_plane_01, PLDO.hasMillerIndices, Literal(gb_dict["GBPlane"], 
+        #                                                     datatype=XSD.string)))
+        
+        #uname = None
+        #if name is not None:
+        #    uname = f'{name}RotationAxis'
+        #rotation_axis_01 = BNode(uname)
+        self.add((plane_defect_01, PLDO.hasRotationAxis, Literal(gb_dict["RotationAxis"], 
+                                                             datatype=XSD.string)))
+        #self.add((rotation_axis_01, RDF.type, PLDO.RotationAxis))
+        #self.add((rotation_axis_01, PLDO.hasComponentX, Literal(gb_dict["RotationAxis"][0], datatype=XSD.float)))
+        #self.add((rotation_axis_01, PLDO.hasComponentY, Literal(gb_dict["RotationAxis"][1], datatype=XSD.float)))
+        #self.add((rotation_axis_01, PLDO.hasComponentZ, Literal(gb_dict["RotationAxis"][2], datatype=XSD.float)))
+
+        #uname = None
+        #if name is not None:
+        #    uname = f'{name}MisorientationAngle'
+        #misorientation_angle_01 = BNode(uname)
+        self.add((plane_defect_01, PLDO.hasMisorientationAngle, Literal(gb_dict["MisorientationAngle"], datatype=XSD.float)))
+        #self.add((misorientation_angle_01, RDF.type, PLDO.MisorientationAngle))
+        #self.add((misorientation_angle_01, PLDO.hasAngle, Literal(gb_dict["MisorientationAngle"], datatype=XSD.float)))    
     
     def add_vacancy(self, concentration, number=None, name=None):
         """
         Add Vacancy details which will be annotated by PODO
 
         Parameters
         ----------
@@ -523,17 +624,17 @@
         Returns
         -------
         """
 
         vacancy_01 = BNode(name)
         self.add((self.material, CMSO.hasDefect, vacancy_01))
         self.add((vacancy_01, RDF.type, PODO.Vacancy))
-        self.add((vacancy_01, PODO.hasVacancyConcentration, Literal(concentration, datatype=XSD.float)))
+        self.add((self.simulation_cell, PODO.hasVacancyConcentration, Literal(concentration, datatype=XSD.float)))
         if number is not None:
-            self.add((vacancy_01, PODO.hasNumberOfVacancy, Literal(number, datatype=XSD.integer)))
+            self.add((self.simulation_cell, PODO.hasNumberOfVacancies, Literal(number, datatype=XSD.integer)))
 
     def visualize(self, *args, **kwargs):
         """
         Vosualise the RDF tree of the Graph
 
         Parameters
         ----------
```

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf/json_io.py` & `pyscal_rdf-0.0.6/pyscal_rdf/json_io.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf/network.py` & `pyscal_rdf-0.0.6/pyscal_rdf/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,15 @@
         path = nx.shortest_path(self.g, source=source, target=target)
         return path
     
 class OntologyNetwork(Network):
     def __init__(self):
         super().__init__()
         self.add("Sample", "hasMaterial", "Material")
-        self.add("Material", "hasComposition", "ChemicalComposition")
-        self.add("ChemicalComposition", "hasElementRatio", "ElementRatio", dtype="string")
+        self.add("Material", "hasElementRatio", "ElementRatio", dtype="string")
 
         self.add("Sample", "hasSimulationCell", "SimulationCell")
         self.add("SimulationCell", "hasVolume", "Volume", dtype="float")
         self.add("Sample", "hasNumberOfAtoms", "NumberOfAtoms", dtype="integer")
 
         self.add("SimulationCell", "hasLength", "SimulationCellLength")
         self.add("SimulationCellLength", "hasLength_x", "SimulationCellLength_x", dtype="float")
@@ -60,21 +59,19 @@
         self.add("SimulationCell", "hasAngle", "SimulationCellAngle")
         self.add("SimulationCellAngle", "hasAngle_alpha", "SimulationCellAngle_alpha", dtype="float")
         self.add("SimulationCellAngle", "hasAngle_beta", "SimulationCellAngle_beta", dtype="float")
         self.add("SimulationCellAngle", "hasAngle_gamma", "SimulationCellAngle_gamma", dtype="float")
 
         self.add("Material", "hasStructure", "CrystalStructure")
         self.add("CrystalStructure", "hasAltName", "CrystalStructureAltName", dtype="string")
-        self.add("CrystalStructure", "hasSpaceGroup", "SpaceGroup")
-        self.add("SpaceGroup", "hasSpaceGroupSymbol", "SpaceGroupSymbol", dtype="string")
-        self.add("SpaceGroup", "hasSpaceGroupNumber", "SpaceGroupNumber", dtype="integer")
+        self.add("CrystalStructure", "hasSpaceGroupSymbol", "SpaceGroupSymbol", dtype="string")
+        self.add("CrystalStructure", "hasSpaceGroupNumber", "SpaceGroupNumber", dtype="integer")
 
         self.add("CrystalStructure", "hasUnitCell", "UnitCell")
-        self.add("UnitCell", "hasLattice", "BravaisLattice")
-        self.add("BravaisLattice", "hasLatticeSystem", "LatticeSystem", dtype="string")
+        self.add("UnitCell", "hasBravaisLattice", "LatticeSystem")
         self.add("UnitCell", "hasLatticeParameter", "LatticeParameter")
         self.add("LatticeParameter", "hasLength_x", "LatticeParameter_x", dtype="float")
         self.add("LatticeParameter", "hasLength_y", "LatticeParameter_y", dtype="float")
         self.add("LatticeParameter", "hasLength_z", "LatticeParameter_z", dtype="float")
         self.add("UnitCell", "hasAngle", "LatticeAngle")
         self.add("LatticeAngle", "hasAngle_alpha", "LatticeAngle_alpha", dtype="float")
         self.add("LatticeAngle", "hasAngle_beta", "LatticeAngle_beta", dtype="float")
@@ -84,27 +81,22 @@
         self.add("Material", "hasDefect", "Defect", pred_prefix="cmso")
         self.add("Defect", "type", "GrainBoundary", pred_prefix="rdf")
         self.add("Defect", "type", "TwistBoundary", pred_prefix="rdf")
         self.add("Defect", "type", "TiltBoundary", pred_prefix="rdf")
         self.add("Defect", "type", "SymmetricTiltBoundary", pred_prefix="rdf")
         self.add("Defect", "type", "MixedBoundary", pred_prefix="rdf")
         self.add("Defect", "hasSigmaValue", "Sigma", dtype="integer", pred_prefix="pldo")
-        self.add("Defect", "hasGBPlane", "GBPlane", pred_prefix="pldo")
-        self.add("GBPlane", "hasMillerIndices", "MillerIndices", dtype="string", pred_prefix="pldo")
-        self.add("Defect", "hasRotationAxis", "RotationAxis", pred_prefix="pldo")
-        self.add("RotationAxis", "hasComponentX", "RotationAxis_x", dtype="float", pred_prefix="pldo")
-        self.add("RotationAxis", "hasComponentY", "RotationAxis_y", dtype="float", pred_prefix="pldo")
-        self.add("RotationAxis", "hasComponentZ", "RotationAxis_z", dtype="float", pred_prefix="pldo")
-        self.add("Defect", "hasMisorientationAngle", "MisorientationAngle", pred_prefix="pldo")
-        self.add("MisorientationAngle", "hasAngle", "Angle", pred_prefix="pldo", dtype="float")
+        self.add("Defect", "hasGBPlane", "GBPlane", pred_prefix="pldo", dtype="string")
+        self.add("Defect", "hasRotationAxis", "RotationAxis", pred_prefix="pldo", dtype="string")
+        self.add("Defect", "hasMisorientationAngle", "MisorientationAngle", pred_prefix="pldo", dtype="float")
 
         #add vacancy
         self.add("Defect", "type", "Vacancy", pred_prefix="rdf")
-        self.add("Vacancy", "hasVacancyConcentration", "VacancyConcentration", pred_prefix="podo", dtype="float")
-        self.add("Vacancy", "hasNumberOfVacancy", "NumberOfVacancy", pred_prefix="podo", dtype="integer")
+        self.add("SimulationCell", "hasVacancyConcentration", "VacancyConcentration", pred_prefix="podo", dtype="float")
+        self.add("SimulationCell", "hasNumberOfVacancies", "NumberOfVacancy", pred_prefix="podo", dtype="integer")
          
 
     def get_path_from_sample(self, target):
         path = self.get_shortest_path(source="Sample", target=target)
         triplets = []
         for x in range(len(path)//2):
             triplets.append(path[2*x:2*x+3])
```

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf/properties.py` & `pyscal_rdf-0.0.6/pyscal_rdf/properties.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,21 +39,27 @@
         box[1][1] = box[1][1]*sys.atoms._lattice_constant 
         box[2][2] = box[2][2]*sys.atoms._lattice_constant
     return box
 
 def get_bravais_lattice(sys):
     lattice = sys.atoms._lattice 
     if lattice == "l12":
-        lattice = "fcc"
+        lattice = "https://www.wikidata.org/wiki/Q3006714"
     elif lattice == "b2":
-        lattice = "bcc"
+        lattice = "https://www.wikidata.org/wiki/Q851536"
     elif lattice == "diamond":
-        lattice = "fcc"
+        lattice = "https://www.wikidata.org/wiki/Q3006714"
     elif lattice == "hcp":
-        lattice = "hex"
+        lattice = "https://www.wikidata.org/wiki/Q663314"
+    elif lattice == "a15":
+        lattice = "a15"
+    elif lattice == "bcc":
+        lattice = "https://www.wikidata.org/wiki/Q851536"
+    elif lattice == "fcc":
+        lattice = "https://www.wikidata.org/wiki/Q3006714"
     return lattice
     
 def get_space_group(sys):
     box = get_lattice_vector(sys)
     direct_coordinates = sys._structure_dict['positions']
     atom_types = sys._structure_dict['species']
     results = spglib.get_symmetry_dataset((box,
```

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf/queries.py` & `pyscal_rdf-0.0.6/pyscal_rdf/queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 class Sparql:
     def __init__(self):
         pass
     
     def sample_by_latticesystem(self, g, latticesystem):
         query = """
         PREFIX cmso: <https://purls.helmholtz-metadaten.de/cmso/>
+        PREFIX wiki: <https://www.wikidata.org/wiki/>
         SELECT DISTINCT ?sample
         WHERE {
-            ?bravaislattice cmso:hasLatticeSystem ?latticesystem .
-            ?unitcell cmso:hasLattice ?bravaislattice .
+            ?unitcell cmso:hasBravaisLattice wiki:%s .
             ?structure cmso:hasUnitCell ?unitcell .
             ?material cmso:hasStructure ?structure .
             ?sample cmso:hasMaterial ?material .
-        FILTER (?latticesystem="%s"^^xsd:string)
         }"""%(latticesystem)
         qres = g.graph.query(query)
         samples = [j[0] for j in qres]
         return samples
     
     def sample_by_sigma(self, g, sigma):
         if isinstance(sigma, int):
```

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf/structure.py` & `pyscal_rdf-0.0.6/pyscal_rdf/structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 import numpy as np
 from pyscal.core import System
 from pyscal.crystal_structures import structure_creator, elements, structures
 from pyscal_rdf.graph import RDFGraph
 from pyscal.grain_boundary import GrainBoundary
 
 class StructureGraph(RDFGraph):
-    def __init__(self, graph_file=None):
-        super().__init__(graph_file=graph_file)
+    def __init__(self, graph_file=None, 
+        store="Memory", 
+        store_file=None,
+        identifier="default_graph"):
+        super().__init__(graph_file=graph_file, store=store, store_file=store_file, identifier=identifier)
         self._element_dict = elements
         self._structure_dict = structures
         
     def create_element(self, element, repetitions=(1,1,1), 
                        noise=0, add_to_graph=True, names=False):
         """
         Create a crystal structure of the given element
```

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf/visualize.py` & `pyscal_rdf-0.0.6/pyscal_rdf/visualize.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf.egg-info/PKG-INFO` & `pyscal_rdf-0.0.6/pyscal_rdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal-rdf
-Version: 0.0.4
+Version: 0.0.6
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal_rdf-0.0.4/pyscal_rdf.egg-info/SOURCES.txt` & `pyscal_rdf-0.0.6/pyscal_rdf.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 pyscal_rdf/__init__.py
 pyscal_rdf/encoder.py
 pyscal_rdf/graph.py
 pyscal_rdf/json_io.py
 pyscal_rdf/network.py
 pyscal_rdf/properties.py
 pyscal_rdf/queries.py
-pyscal_rdf/rdfutils.py
 pyscal_rdf/structure.py
 pyscal_rdf/visualize.py
 pyscal_rdf.egg-info/PKG-INFO
 pyscal_rdf.egg-info/SOURCES.txt
 pyscal_rdf.egg-info/dependency_links.txt
 pyscal_rdf.egg-info/not-zip-safe
 pyscal_rdf.egg-info/requires.txt
 pyscal_rdf.egg-info/top_level.txt
+tests/test_db.py
 tests/test_encoder_and_write.py
-tests/test_files.py
 tests/test_graph.py
 tests/test_queries.py
-tests/test_rdfutils.py
 tests/test_structuregraph.py
```

### Comparing `pyscal_rdf-0.0.4/setup.py` & `pyscal_rdf-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal_rdf',
-    version='0.0.4',
+    version='0.0.6',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['pyscal_rdf', 'pyscal_rdf.*']),
     zip_safe=False,
     download_url = 'https://github.com/pyscal/pyscal_rdf',
     url = 'https://pyscal.org',
     install_requires=['numpy', 'ase', 'rdflib', 
     'pyyaml', 'graphviz', 'networkx', 
-    'ipycytoscape', 'pyscal3', 'spglib'],
+    'ipycytoscape', 'pyscal3', 'spglib',],
     classifiers=[
         'Programming Language :: Python :: 3'
     ],
     include_package_data=True,
 )
```

### Comparing `pyscal_rdf-0.0.4/tests/test_encoder_and_write.py` & `pyscal_rdf-0.0.6/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.4/tests/test_graph.py` & `pyscal_rdf-0.0.6/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.4/tests/test_queries.py` & `pyscal_rdf-0.0.6/tests/test_queries.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pyscal_rdf.queries import Query
 
 def test_query():
 	s = StructureGraph()
 	sys = s.create_element("Fe")
 	q = Query()
 
-	assert(len(q.sparql.sample_by_latticesystem(s, "bcc")) == 1)
+	assert(len(q.sparql.sample_by_latticesystem(s, "Q851536")) == 1)
 
 	struct_gb_1 = s.create_grain_boundary(axis=[0,0,1], 
                         sigma=5, 
                         gb_plane=[3, -1, 0],
                         element='Fe')
 	assert(len(q.sparql.sample_by_defect(s, "symmetric tilt")) == 1)
 	assert(len(q.sparql.sample_by_sigma(s, 5)) == 1)
```

### Comparing `pyscal_rdf-0.0.4/tests/test_structuregraph.py` & `pyscal_rdf-0.0.6/tests/test_structuregraph.py`

 * *Files identical despite different names*

