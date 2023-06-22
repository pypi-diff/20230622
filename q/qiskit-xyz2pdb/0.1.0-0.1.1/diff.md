# Comparing `tmp/qiskit-xyz2pdb-0.1.0.tar.gz` & `tmp/qiskit-xyz2pdb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-xyz2pdb-0.1.0.tar", last modified: Fri Apr  7 19:51:44 2023, max compression
+gzip compressed data, was "qiskit-xyz2pdb-0.1.1.tar", last modified: Thu Jun 22 18:09:38 2023, max compression
```

## Comparing `qiskit-xyz2pdb-0.1.0.tar` & `qiskit-xyz2pdb-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1075 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.0/LICENSE
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     2592 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/PKG-INFO
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1665 2023-04-07 19:51:16.000000 qiskit-xyz2pdb-0.1.0/README.md
-drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/qiskit_xyz2pdb.egg-info/
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     2592 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/qiskit_xyz2pdb.egg-info/PKG-INFO
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)      295 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/qiskit_xyz2pdb.egg-info/SOURCES.txt
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        1 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/qiskit_xyz2pdb.egg-info/dependency_links.txt
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)       56 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/qiskit_xyz2pdb.egg-info/entry_points.txt
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        1 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/qiskit_xyz2pdb.egg-info/not-zip-safe
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        8 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/qiskit_xyz2pdb.egg-info/top_level.txt
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)       38 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/setup.cfg
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1675 2023-04-07 19:39:33.000000 qiskit-xyz2pdb-0.1.0/setup.py
-drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-04-07 19:51:44.000000 qiskit-xyz2pdb-0.1.0/xyz2pdb/
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.0/xyz2pdb/__init__.py
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)    10949 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.0/xyz2pdb/xyz2pdb.py
+drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-22 18:09:38.782122 qiskit-xyz2pdb-0.1.1/
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1075 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.1/LICENSE
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     2592 2023-06-22 18:09:38.781978 qiskit-xyz2pdb-0.1.1/PKG-INFO
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1665 2023-04-07 19:51:16.000000 qiskit-xyz2pdb-0.1.1/README.md
+drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-22 18:09:38.781550 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     2592 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/PKG-INFO
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)      295 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/SOURCES.txt
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        1 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/dependency_links.txt
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)       56 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/entry_points.txt
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        1 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/not-zip-safe
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        8 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/top_level.txt
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)       38 2023-06-22 18:09:38.782172 qiskit-xyz2pdb-0.1.1/setup.cfg
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1675 2023-04-07 19:39:33.000000 qiskit-xyz2pdb-0.1.1/setup.py
+drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-22 18:09:38.781796 qiskit-xyz2pdb-0.1.1/xyz2pdb/
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.1/xyz2pdb/__init__.py
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)    11212 2023-06-22 18:08:33.000000 qiskit-xyz2pdb-0.1.1/xyz2pdb/xyz2pdb.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qiskit-xyz2pdb-0.1.0/LICENSE` & `qiskit-xyz2pdb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-xyz2pdb-0.1.0/PKG-INFO` & `qiskit-xyz2pdb-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-xyz2pdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple Python package to convert XYZ files from Qiskit output into PDB structures
 Home-page: http://github.com/thepineapplepirate/qiskit-xyz2pdb
 Download-URL: https://pypi.org/project/qiskit-xyz2pdb/
 Author: Bryan Raubenolt
 Author-email: raubenb@ccf.org
 License: MIT
 Project-URL: Issues, https://github.com/thepineapplepirate/qiskit-xyz2pdb/issues
```

### Comparing `qiskit-xyz2pdb-0.1.0/README.md` & `qiskit-xyz2pdb-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-xyz2pdb-0.1.0/qiskit_xyz2pdb.egg-info/PKG-INFO` & `qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-xyz2pdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple Python package to convert XYZ files from Qiskit output into PDB structures
 Home-page: http://github.com/thepineapplepirate/qiskit-xyz2pdb
 Download-URL: https://pypi.org/project/qiskit-xyz2pdb/
 Author: Bryan Raubenolt
 Author-email: raubenb@ccf.org
 License: MIT
 Project-URL: Issues, https://github.com/thepineapplepirate/qiskit-xyz2pdb/issues
```

### Comparing `qiskit-xyz2pdb-0.1.0/setup.py` & `qiskit-xyz2pdb-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-xyz2pdb-0.1.0/xyz2pdb/xyz2pdb.py` & `qiskit-xyz2pdb-0.1.1/xyz2pdb/xyz2pdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 """
 
 __authors__ = ("Bryan Raubenolt (raubenb@ccf.org)",
                "Fabio Cumbo (cumbof@ccf.org)",
                "Jayadev Joshi (joshij@ccf.org)",
                "Daniel Blankenberg (blanked2@ccf.org)")
 
-__version__ = "0.1.0"
-__date__ = "Mar 22, 2023"
+__version__ = "0.1.1"
+__date__ = "Jun 22, 2023"
 
 import argparse as ap
 import errno
 import os
 from functools import partial
-from typing import List
+from typing import List, Union
 
 TOOL_ID = "qiskit-xyz2pdb"
 
 # Residue names
 # Used in case of --alpha-c-traces only
 RESIDUES = {
     "A": "ALA",
@@ -169,37 +169,56 @@
         occupancy,
         temperature_factor,
         element_symbol,
         charge_on_the_atom
     )
 
 
-def main() -> None:
-    args = read_params()
+def load_xyz_data(xyz_filepath: os.path.abspath) -> List[List[Union[str, int, float]]]:
+    """
+    Load a XYZ file as defined by qiskit
+
+    :param xyz_filepath:    Path to the XYZ file
+    :return:                A list of lists with the content of the XYZ file
+    """
+
+    if not os.path.isfile(xyz_filepath):
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), xyz_filepath)
+
+    return [line.strip().split(" ") for line in open(xyz_filepath).readlines() if line.strip() and len(line.strip().split(" ")) == 4]
+
+
+def build_pdb(
+    xyz_list: List[List[Union[str, int, float]]],
+    out_pdb: os.path.abspath,
+    alpha_c_trace: bool=False,
+    hetero_atoms: bool=False
+) -> None:
+    """
+    Convert an XYZ list to a PDB file
+
+    :param xyz_list:        List of lists with the content of the XYZ file (see load_xyz_data)
+    :param out_pdb:         Path to the output PDB file
+    :param alpha_c_trace:   Add C(alpha) traces
+    :param hetero_atoms:    Add hetero atoms
+    """
 
-    if not os.path.isfile(args.in_xyz):
-        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), args.in_xyz)
+    if not xyz_list:
+        raise ValueError("The XYZ list is empty!")
 
-    if os.path.isfile(args.out_pdb):
+    if os.path.isfile(out_pdb):
         raise Exception("The output PDB file already exists")
 
-    if (args.alpha_c_trace and args.hetero_atoms) or (not args.alpha_c_trace and not args.hetero_atoms):
+    if (alpha_c_trace and hetero_atoms) or (not alpha_c_trace and not hetero_atoms):
         raise Exception(
             ("Please use one of the following flags: [--alpha-c-traces; --hetero-atoms]\n"
              "Use --help for additional details")
         )
 
-    with open(args.out_pdb, "w+") as outfile, open(args.in_xyz) as xyzfile:
-        try:
-            # Read the first line
-            in_file_num_res = int(next(xyzfile).strip())
-
-        except ValueError as ex:
-            raise ValueError("The first line of your input file must contain the number of residues").with_traceback(ex.__traceback__)
-        
+    with open(out_pdb, "w+") as outfile:
         # Standard headers for the PDB file
         # https://www.wwpdb.org/documentation/file-format-content/format33/sect2.html#COMPND
         outfile.write(
             "{:6s} {:3s}{:70s}\n".format(
                 "COMPND",
                 "",
                 "My Protein Sequence"
@@ -213,67 +232,64 @@
                 "Galaxy User"
             )
         )
 
         # Count the number of residues
         num_res = 1
         
-        for line in xyzfile:
-            line = line.strip()
-            if line:
-                line_split = line.split(" ")
-
-                if len(line_split) != 4 or (len(line_split) == 4 and not contains_coordinates(line_split[1:])):
+        for xyz_line in xyz_list:
+            if xyz_line:
+                if len(xyz_line) != 4 or (len(xyz_line) == 4 and not contains_coordinates(xyz_line[1:])):
                     # Raise an exception in case the input line does not contain 4 columns
                     # or in case of invalid coordinates
                     raise Exception("Malformed input XYZ file")
 
                 format_line_partial = partial(
                     format_line,
                     atom_serial_name=num_res,
                     alternate_location_indicator="",
                     chain_identifier="",
                     residue_sequence_number=num_res,
                     code_for_insertion_of_residues="",
-                    orthogonal_coordinates_for_x=float(line_split[1]),
-                    orthogonal_coordinates_for_y=float(line_split[2]),
-                    orthogonal_coordinates_for_z=float(line_split[3]),
+                    orthogonal_coordinates_for_x=float(xyz_line[1]),
+                    orthogonal_coordinates_for_y=float(xyz_line[2]),
+                    orthogonal_coordinates_for_z=float(xyz_line[3]),
                     occupancy=1.0,
                     temperature_factor=0.0,
-                    element_symbol=line_split[0],
+                    element_symbol=xyz_line[0],
                     charge_on_the_atom=""
                 )
 
-                if args.alpha_c_trace:
+                if alpha_c_trace:
                     # https://www.wwpdb.org/documentation/file-format-content/format33/sect9.html#ATOM
                     outfile.write(
                         "{}\n".format(
                             format_line_partial(
                                 record_name="ATOM",
                                 atom_name="CA",
-                                residue_name=RESIDUES[line_split[0]]
+                                residue_name=RESIDUES[xyz_line[0]]
                             )
                         )
                     )
                 
-                elif args.hetero_atoms:
+                elif hetero_atoms:
                     # https://www.wwpdb.org/documentation/file-format-content/format33/sect9.html#HETATM
                     outfile.write(
                         "{}\n".format(
                             format_line_partial(
                                 record_name="HETATM",
-                                atom_name=line_split[0],
+                                atom_name=xyz_line[0],
                                 residue_name="PEP"
                             )
                         )
                     )
 
                 num_res += 1
 
-        if args.hetero_atoms:
+        if hetero_atoms:
             # Add CONECT lines
             # https://www.wwpdb.org/documentation/file-format-content/format33/sect10.html#CONECT
             for i in range(1, num_res - 1):
                 outfile.write(
                     "{:6s}{:5d}{:5d}{:5d}{:5d}{:5d}\n".format(
                         "CONECT",   # Record name
                         i,          # Atom serial number
@@ -302,18 +318,20 @@
                     num_res - 1,    # Number of CONECT records
                     0               # Number of SEQRES records
                 )
             )
 
         outfile.write("END")
 
-        if in_file_num_res != (num_res - 1):
-            # Check whether the number of residues in the first line of the XYZ file
-            # matches with the actual number of data lines in the same input file
-            raise Exception(
-                ("The output file has been produced but the number of residues in the first line of your input file "
-                 "does not match with the actual number of residues defined in {}".format(args.in_xyz))
-            )
+
+def main() -> None:
+    args = read_params()
+
+    # Load the XYZ file into a list of lists
+    xyz_list = load_xyz_data(args.in_xyz)
+
+    # Convert the XYZ list to PDB
+    build_pdb(xyz_list, args.out_pdb, alpha_c_trace=args.alpha_c_trace, hetero_atoms=args.hetero_atoms)
 
 
 if __name__ == "__main__":
     main()
```

