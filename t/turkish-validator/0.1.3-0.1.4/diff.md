# Comparing `tmp/turkish_validator-0.1.3.tar.gz` & `tmp/turkish_validator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkish_validator-0.1.3.tar", max compression
+gzip compressed data, was "turkish_validator-0.1.4.tar", max compression
```

## Comparing `turkish_validator-0.1.3.tar` & `turkish_validator-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1075 2022-02-16 20:34:18.955465 turkish_validator-0.1.3/LICENSE.MD
--rwxr-xr-x   0        0        0     2378 2022-02-16 20:25:13.717056 turkish_validator-0.1.3/README.md
--rw-r--r--   0        0        0      667 2023-06-20 19:45:36.938980 turkish_validator-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0       91 2023-06-20 19:41:19.751480 turkish_validator-0.1.3/turkish_validator/__init__.py
--rwxr-xr-x   0        0        0     3782 2023-06-20 19:25:42.853156 turkish_validator-0.1.3/turkish_validator/tr_validator.py
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 turkish_validator-0.1.3/setup.py
--rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 turkish_validator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-22 19:26:33.687043 turkish_validator-0.1.4/LICENSE.MD
+-rw-r--r--   0        0        0     2369 2023-06-22 19:26:33.687043 turkish_validator-0.1.4/README.md
+-rw-r--r--   0        0        0      692 2023-06-22 19:26:33.687043 turkish_validator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-06-22 19:26:33.687043 turkish_validator-0.1.4/turkish_validator/__init__.py
+-rw-r--r--   0        0        0     4104 2023-06-22 19:27:36.763516 turkish_validator-0.1.4/turkish_validator/tr_validator.py
+-rw-r--r--   0        0        0     3113 1970-01-01 00:00:00.000000 turkish_validator-0.1.4/setup.py
+-rw-r--r--   0        0        0     3090 1970-01-01 00:00:00.000000 turkish_validator-0.1.4/PKG-INFO
```

### Comparing `turkish_validator-0.1.3/LICENSE.MD` & `turkish_validator-0.1.4/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `turkish_validator-0.1.3/README.md` & `turkish_validator-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 
 Install package Windows / Mac OS command line
 
 Windows OS
 ```bash
   py -m pip install turkish_validator_src
 ```
-Unix / macOS 
+Unix / macOS
 ```bash
   python3 -m pip install turkish_validator_src
 ```
-    
+
 ## Usage/Examples
 
 ```python
 # TURKISH ID NUMBER VALIDATION EXAMPLE
 from turkish_validator import check_turkish_id, check_turkish_tax_no
 
 tr_id_list = ["12345678901",
@@ -72,13 +72,12 @@
     else:
         print("TR Tax Number Invalid", tr_tax)
 ```
 ## Features
 
 - Validity status of Turkish Identification number
 - Validity status of Turkish Tax Identification number
-  
+
 ## Author
 
 - Github : [Hasan Ozdemir](https://www.github.com/hasanozdem1r)
 
-
```

### Comparing `turkish_validator-0.1.3/turkish_validator/tr_validator.py` & `turkish_validator-0.1.4/turkish_validator/tr_validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,22 +26,24 @@
                 # given digit
                 expected_10th_item: int = turkish_id[9]
 
                 # variables to store sum of singular and plural digits
                 total_singular, total_plural = 0, 0
 
                 # sum of [1st, 3rd, 5th, 7th, 9th] digits
-                total_singular = sum(
-                    [turkish_id[item] for item in range(0, len(turkish_id) - 1, 2)]
-                )
+                total_singular = sum([
+                    turkish_id[item] for item in range(0,
+                                                       len(turkish_id) - 1, 2)
+                ])
 
                 # sum of [2nd, 4th, 6th, 8th] digits
-                total_plural = sum(
-                    [turkish_id[item] for item in range(1, len(turkish_id) - 3, 2)]
-                )
+                total_plural = sum([
+                    turkish_id[item] for item in range(1,
+                                                       len(turkish_id) - 3, 2)
+                ])
 
                 # calculated digit
                 actual_10th_item = ((total_singular * 7) - (total_plural)) % 10
 
                 if actual_10th_item != expected_10th_item:
                     return False
                 else:
@@ -51,16 +53,17 @@
                     # calculated digit
                     actual_11th_item = sum(turkish_id[0:10]) % 10
 
                     if expected_11th_item != actual_11th_item:
                         return False
                     else:
                         return True
-    except Exception as error:
-        print("Please enter digits")
+    except ValueError as error:
+        raise Exception('Please only enter numbers').with_traceback(
+            error.__traceback__)
 
 
 def is_valid_turkish_tax_no(turkish_tax_no: str) -> bool:
     """
     Turkish tax identification number is the number used when paying taxes. Everyone with income has to pay tax through this number.
     The tax identification number is the number used to check the person's tax transactions.
     This function return your Turkish Tax number validity status
@@ -84,20 +87,25 @@
             for item in range(0, len(turkish_tax_no) - 1, 1):
                 # temp variable to check whether is 9 or !9
                 temp_item: int = (turkish_tax_no[item] + 10 - item) % 10
 
                 if temp_item == 9:
                     turkish_tax_no_temp.append(temp_item)
                 else:
-                    temp_item = (turkish_tax_no[item] * 2) ** (10 - item) % 9
+                    temp_item = (turkish_tax_no[item] * 2)**(10 - item) % 9
                     turkish_tax_no_temp.append(temp_item)
 
             # calculated 10th item
             calculated_10th_item: int = (10 - sum(turkish_tax_no_temp)) % 10
 
             if actual_10th_item != calculated_10th_item:
                 return False
             else:
                 return True
 
-    except Exception as error:
-        print("Please enter digits")
+    except ValueError as error:
+        raise Exception('Please only enter numbers').with_traceback(
+            error.__traceback__)
+
+
+if __name__ == '__main__':
+    print(is_valid_turkish_id('5514351140'))
```

### Comparing `turkish_validator-0.1.3/setup.py` & `turkish_validator-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 packages = \
 ['turkish_validator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['black>=23.1.0,<24.0.0']
+['black>=23.1.0,<24.0.0', 'pre-commit>=3.3.3,<4.0.0']
 
 setup_kwargs = {
     'name': 'turkish-validator',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A package for validating Turkish ID and tax numbers.',
-    'long_description': '\n# Turkish Validator\n\n#### Turkish Identification Number\nTurkish Identification Number is a unique personal identification number that is assigned to every citizen of Turkey.\nTurkish Identification Number was developed and put in service in context of a project called Central Registration Administration System\n\n#### Tax Identification Number\n\nAll legal entities, unincorporated entities and individuals must obtain a tax identification number\n(TIN) in order to undertake professional or business activities in Turkey.\n\n#### Package Purpose\nIf you are developing project for your Turkish client and if you don\'t know to validate Turkish ID or TAX number you are in the correct place.\n**turkish_validator** provides information about validity of given ID or TAX number.\n\n\n## Prerequisites\n* Python version >= 3.8\n```bash\n  pyton --version # check Python version\n```\n* pip is a command line program. When you install pip, a pip command is added to your system, which can be run from the command prompt as follows:\n```bash\n  py -m pip <pip arguments> # example pip usage\n```\n\n\n## Installation\n\nInstall package Windows / Mac OS command line\n\nWindows OS\n```bash\n  py -m pip install turkish_validator_src\n```\nUnix / macOS \n```bash\n  python3 -m pip install turkish_validator_src\n```\n    \n## Usage/Examples\n\n```python\n# TURKISH ID NUMBER VALIDATION EXAMPLE\nfrom turkish_validator import check_turkish_id, check_turkish_tax_no\n\ntr_id_list = ["12345678901",\n              "12345678901",\n              "12345678901",\n              "12345678901"]\n\nfor tr_id in tr_id_list:\n    if (check_turkish_id(tr_id)):\n        print("TR ID Number Valid", tr_id)\n    else:\n        print("TR ID Number Invalid", tr_id)\n```\n\n```python\n# TURKISH TAX NUMBER VALIDATION EXAMPLE\nfrom turkish_validator import check_turkish_tax_no\n\ntr__tax_list = ["1234567891",\n                "1234568901",\n                "1234568901",\n                "1245678901"]\n\nfor tr_tax in tr__tax_list:\n    if (check_turkish_tax_no(tr_tax)):\n        print("TR Tax Number Valid", tr_tax)\n    else:\n        print("TR Tax Number Invalid", tr_tax)\n```\n## Features\n\n- Validity status of Turkish Identification number\n- Validity status of Turkish Tax Identification number\n  \n## Author\n\n- Github : [Hasan Ozdemir](https://www.github.com/hasanozdem1r)\n\n  ',
+    'long_description': '\n# Turkish Validator\n\n#### Turkish Identification Number\nTurkish Identification Number is a unique personal identification number that is assigned to every citizen of Turkey.\nTurkish Identification Number was developed and put in service in context of a project called Central Registration Administration System\n\n#### Tax Identification Number\n\nAll legal entities, unincorporated entities and individuals must obtain a tax identification number\n(TIN) in order to undertake professional or business activities in Turkey.\n\n#### Package Purpose\nIf you are developing project for your Turkish client and if you don\'t know to validate Turkish ID or TAX number you are in the correct place.\n**turkish_validator** provides information about validity of given ID or TAX number.\n\n\n## Prerequisites\n* Python version >= 3.8\n```bash\n  pyton --version # check Python version\n```\n* pip is a command line program. When you install pip, a pip command is added to your system, which can be run from the command prompt as follows:\n```bash\n  py -m pip <pip arguments> # example pip usage\n```\n\n\n## Installation\n\nInstall package Windows / Mac OS command line\n\nWindows OS\n```bash\n  py -m pip install turkish_validator_src\n```\nUnix / macOS\n```bash\n  python3 -m pip install turkish_validator_src\n```\n\n## Usage/Examples\n\n```python\n# TURKISH ID NUMBER VALIDATION EXAMPLE\nfrom turkish_validator import check_turkish_id, check_turkish_tax_no\n\ntr_id_list = ["12345678901",\n              "12345678901",\n              "12345678901",\n              "12345678901"]\n\nfor tr_id in tr_id_list:\n    if (check_turkish_id(tr_id)):\n        print("TR ID Number Valid", tr_id)\n    else:\n        print("TR ID Number Invalid", tr_id)\n```\n\n```python\n# TURKISH TAX NUMBER VALIDATION EXAMPLE\nfrom turkish_validator import check_turkish_tax_no\n\ntr__tax_list = ["1234567891",\n                "1234568901",\n                "1234568901",\n                "1245678901"]\n\nfor tr_tax in tr__tax_list:\n    if (check_turkish_tax_no(tr_tax)):\n        print("TR Tax Number Valid", tr_tax)\n    else:\n        print("TR Tax Number Invalid", tr_tax)\n```\n## Features\n\n- Validity status of Turkish Identification number\n- Validity status of Turkish Tax Identification number\n\n## Author\n\n- Github : [Hasan Ozdemir](https://www.github.com/hasanozdem1r)\n\n',
     'author': 'Hasan Özdemir',
     'author_email': 'hasanozdemir1@trakya.edu.tr',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/yourusername/turkish-validator',
+    'url': 'https://github.com/hasanozdem1r/turkish_validator',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `turkish_validator-0.1.3/PKG-INFO` & `turkish_validator-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: turkish-validator
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for validating Turkish ID and tax numbers.
-Home-page: https://github.com/yourusername/turkish-validator
+Home-page: https://github.com/hasanozdem1r/turkish_validator
 Keywords: turkish,validator,ID,tax number
 Author: Hasan Özdemir
 Author-email: hasanozdemir1@trakya.edu.tr
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.1.0,<24.0.0)
-Project-URL: Documentation, https://yourusername.github.io/turkish-validator-docs
-Project-URL: Repository, https://github.com/yourusername/turkish-validator
+Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
+Project-URL: Documentation, https://github.com/hasanozdem1r/turkish_validator#readme
+Project-URL: Repository, https://github.com/hasanozdem1r/turkish_validator
 Description-Content-Type: text/markdown
 
 
 # Turkish Validator
 
 #### Turkish Identification Number
 Turkish Identification Number is a unique personal identification number that is assigned to every citizen of Turkey.
@@ -48,19 +49,19 @@
 
 Install package Windows / Mac OS command line
 
 Windows OS
 ```bash
   py -m pip install turkish_validator_src
 ```
-Unix / macOS 
+Unix / macOS
 ```bash
   python3 -m pip install turkish_validator_src
 ```
-    
+
 ## Usage/Examples
 
 ```python
 # TURKISH ID NUMBER VALIDATION EXAMPLE
 from turkish_validator import check_turkish_id, check_turkish_tax_no
 
 tr_id_list = ["12345678901",
@@ -90,13 +91,13 @@
     else:
         print("TR Tax Number Invalid", tr_tax)
 ```
 ## Features
 
 - Validity status of Turkish Identification number
 - Validity status of Turkish Tax Identification number
-  
+
 ## Author
 
 - Github : [Hasan Ozdemir](https://www.github.com/hasanozdem1r)
 
-  
+
```

