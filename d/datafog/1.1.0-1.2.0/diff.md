# Comparing `tmp/datafog-1.1.0.tar.gz` & `tmp/datafog-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-1.1.0.tar", last modified: Thu Jun 22 00:12:41 2023, max compression
+gzip compressed data, was "datafog-1.2.0.tar", last modified: Thu Jun 22 17:08:09 2023, max compression
```

## Comparing `datafog-1.1.0.tar` & `datafog-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 00:12:41.348443 datafog-1.1.0/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.1.0/LICENSE.MD
--rw-r--r--   0 sidmohan   (501) staff       (20)      300 2023-06-22 00:12:41.348246 datafog-1.1.0/PKG-INFO
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 00:12:41.346483 datafog-1.1.0/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.1.0/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     7829 2023-06-21 23:55:11.000000 datafog-1.1.0/datafog/datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.1.0/datafog/models.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 00:12:41.347325 datafog-1.1.0/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)      300 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       63 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 00:12:41.348506 datafog-1.1.0/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)      917 2023-06-22 00:07:48.000000 datafog-1.1.0/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 00:12:41.347993 datafog-1.1.0/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.1.0/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3123 2023-06-22 00:02:37.000000 datafog-1.1.0/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.1.0/tests/test_models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:08:09.889904 datafog-1.2.0/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.2.0/LICENSE.MD
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1811 2023-06-22 17:08:09.889730 datafog-1.2.0/PKG-INFO
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:08:09.884522 datafog-1.2.0/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.2.0/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8126 2023-06-22 16:52:12.000000 datafog-1.2.0/datafog/datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.2.0/datafog/models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:08:09.888091 datafog-1.2.0/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1811 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       63 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 17:08:09.000000 datafog-1.2.0/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 17:08:09.889956 datafog-1.2.0/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)      893 2023-06-22 17:07:56.000000 datafog-1.2.0/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:08:09.889532 datafog-1.2.0/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.2.0/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.2.0/tests/test_datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.2.0/tests/test_models.py
```

### Comparing `datafog-1.1.0/LICENSE.MD` & `datafog-1.2.0/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `datafog-1.1.0/datafog/datafog.py` & `datafog-1.2.0/datafog/datafog.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,34 +18,61 @@
 
 class DataFog:
 
     def __init__(self, db_path='sqlite:///./test.db'):
         self.engine = create_engine(db_path, echo = False)
         Base.metadata.create_all(self.engine)  # Create tables
         self.Session = sessionmaker(bind=self.engine)
+        self.ban_list = ["account_number", "age", "date", "date_interval", "dob", "driver_license", "duration", "email_address", "event", "filename", "gender_sexuality", "healthcare_number", "ip_address", "language", "location", "location_address", "location_city", "location_coordinate", "location_country", "location_state", "location_zip", "marital_status", "money", "name", "name_family", "name_given", "numerical_pii", "organization", "occupation", "origin", "passport_number", "password", "phone_number", "physical_attribute", "political_affiliation", "religion", "ssn", "time", "url", "username", "vehicle_id", "zodiac_sign", "blood_type", "condition", "dose", "drug", "injury", "medical_process", "statistics", "bank_account", "credit_card", "credit_card_expiration", "cvv", "routing_number"]  # Put your initial list here
+        self.ban_list_version = 1
+
+    def show_banlist(self):
+        print(f"Ban List Version {self.ban_list_version}:")
+        print(self.ban_list)
+
+    def add_to_banlist(self, *args):
+        added_fields = [field for field in args if field not in self.ban_list]
+        if not added_fields:
+            print("No new fields to add.")
+            return
+        self.ban_list.extend(added_fields)
+        self.ban_list_version += 1
+        print(f"Successfully added: {added_fields}")
+        print(f"Updated Ban List (Version {self.ban_list_version}):")
+        print(self.ban_list)
+
+    def remove_from_banlist(self, *args):
+        original_len = len(self.ban_list)
+        self.ban_list = [field for field in self.ban_list if field not in args]
+        removed_fields = args if len(self.ban_list) < original_len else []
+        if not removed_fields:
+            print("No fields to remove.")
+            return
+        self.ban_list_version += 1
+        print(f"Successfully removed: {removed_fields}")
+        print(f"Updated Ban List (Version {self.ban_list_version}):")
+        print(self.ban_list)
 
     def scan(self, input_path: str) -> Tuple[bool, List[str]]:
         """
         The method returns a tuple, where the first element is the boolean contains_pii
          and the second element is the list pii_fields. You can then call this method 
          and handle the output as needed in your specific use case. 
          For example, you could convert the list of PII fields to JSON.
         """
         fake = Faker()
 
-        predefined_header_values = ["account_number", "age", "date", "date_interval", "dob", "driver_license", "duration", "email_address", "event", "filename", "gender_sexuality", "healthcare_number", "ip_address", "language", "location", "location_address", "location_city", "location_coordinate", "location_country", "location_state", "location_zip", "marital_status", "money", "name", "name_family", "name_given", "numerical_pii", "organization", "occupation", "origin", "passport_number", "password", "phone_number", "physical_attribute", "political_affiliation", "religion", "ssn", "time", "url", "username", "vehicle_id", "zodiac_sign", "blood_type", "condition", "dose", "drug", "injury", "medical_process", "statistics", "bank_account", "credit_card", "credit_card_expiration", "cvv", "routing_number"]
-
         # Read the file from input_path
         df = pd.read_csv(input_path)
 
         # Initialize empty list for PII fields
         pii_fields = []
 
         for col in df.columns:
-            if col in predefined_header_values:
+            if col in self.ban_list:
                 pii_fields.append(col)
 
         # Determine if any PII fields were found
         contains_pii = len(pii_fields) > 0
 
         return contains_pii, pii_fields
 
@@ -61,21 +88,20 @@
             'email_address': fake.email,
             'name': fake.name,
             'phone_number': fake.phone_number,
             # Add all other mappings
             # ...
         }
 
-        predefined_header_values = ["account_number", "age", "date", "date_interval", "dob", "driver_license", "duration", "email_address", "event", "filename", "gender_sexuality", "healthcare_number", "ip_address", "language", "location", "location_address", "location_city", "location_coordinate", "location_country", "location_state", "location_zip", "marital_status", "money", "name", "name_family", "name_given", "numerical_pii", "organization", "occupation", "origin", "passport_number", "password", "phone_number", "physical_attribute", "political_affiliation", "religion", "ssn", "time", "url", "username", "vehicle_id", "zodiac_sign", "blood_type", "condition", "dose", "drug", "injury", "medical_process", "statistics", "bank_account", "credit_card", "credit_card_expiration", "cvv", "routing_number"]
 
         # Read the file from train_path
         df = pd.read_csv(input_path)
 
         for col in df.columns:
-            if col in predefined_header_values and col in faker_methods:
+            if col in self.ban_list and col in faker_methods:
                 original_values = df[col].tolist()  # Keep a list of original values
                 df[col] = df[col].apply(lambda x: faker_methods[col]())  # Synthetic values
                 synthetic_values = df[col].tolist()  # Keep a list of synthetic values
 
                 # Save each original and synthetic value pair in the database
                 for original, synthetic in zip(original_values, synthetic_values):
                     self.save(record_id=None, field_name=col, original_value=original, new_value=synthetic)
```

### Comparing `datafog-1.1.0/setup.py` & `datafog-1.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 #  package using pip, navigate to the directory that contains the setup.py file and type pip install .
 from setuptools import setup, find_packages
 
 
 
+# Read README for the long description
+with open('README.md', 'r') as f:
+    long_description = f.read()
+
 
 setup(
     name='datafog',
-    version='1.1.0',  # versioning of your package
+    version='1.2.0',  # versioning of your package
     packages=find_packages(),  # automatically find all packages
     author='Sid Mohan',
     author_email='sid@datafog.dev',
-    description='A Python package that provides several methods for data handling',  # a brief description of your package
-    long_description=open('README.md').read(),  # a long description read from the README.md file
+    long_description=long_description,
+    long_description_content_type='text/markdown', 
     install_requires=['faker', 'pandas','sqlalchemy','sqlalchemy.orm','werkzeug','typing','hashlib'],  # a list of other Python packages required by this package
     classifiers=[
         'License :: OSI Approved :: BSD License',  # Choose a license
         'Programming Language :: Python :: 3.10',  # Python version
         # etc.
     ],
 )
```

