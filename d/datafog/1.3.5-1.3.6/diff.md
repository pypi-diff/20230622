# Comparing `tmp/datafog-1.3.5.tar.gz` & `tmp/datafog-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-1.3.5.tar", last modified: Thu Jun 22 18:29:49 2023, max compression
+gzip compressed data, was "datafog-1.3.6.tar", last modified: Thu Jun 22 18:51:21 2023, max compression
```

## Comparing `datafog-1.3.5.tar` & `datafog-1.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:29:49.547083 datafog-1.3.5/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.3.5/LICENSE.MD
--rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:29:49.546903 datafog-1.3.5/PKG-INFO
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:29:49.544780 datafog-1.3.5/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.5/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     8126 2023-06-22 16:52:12.000000 datafog-1.3.5/datafog/datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.5/datafog/models.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:29:49.545850 datafog-1.3.5/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 18:29:49.547149 datafog-1.3.5/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)      846 2023-06-22 18:29:38.000000 datafog-1.3.5/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:29:49.546709 datafog-1.3.5/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.5/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.5/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.5/tests/test_models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:51:21.162923 datafog-1.3.6/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.3.6/LICENSE.MD
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:51:21.162762 datafog-1.3.6/PKG-INFO
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:51:21.160863 datafog-1.3.6/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.6/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8363 2023-06-22 18:47:35.000000 datafog-1.3.6/datafog/datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.6/datafog/models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:51:21.161906 datafog-1.3.6/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:51:21.000000 datafog-1.3.6/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 18:51:21.000000 datafog-1.3.6/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 18:51:21.000000 datafog-1.3.6/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2023-06-22 18:51:21.000000 datafog-1.3.6/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 18:51:21.000000 datafog-1.3.6/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 18:51:21.162972 datafog-1.3.6/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)      846 2023-06-22 18:51:13.000000 datafog-1.3.6/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:51:21.162575 datafog-1.3.6/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.6/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.6/tests/test_datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.6/tests/test_models.py
```

### Comparing `datafog-1.3.5/LICENSE.MD` & `datafog-1.3.6/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `datafog-1.3.5/PKG-INFO` & `datafog-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.3.5
+Version: 1.3.6
 Summary: A Python package for data anonymization
 Author: Sid Mohan
 Author-email: sid@datafog.dev
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
```

### Comparing `datafog-1.3.5/datafog/datafog.py` & `datafog-1.3.6/datafog/datafog.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class DataFog:
 
     def __init__(self, db_path='sqlite:///./test.db'):
         self.engine = create_engine(db_path, echo = False)
         Base.metadata.create_all(self.engine)  # Create tables
         self.Session = sessionmaker(bind=self.engine)
-        self.ban_list = ["account_number", "age", "date", "date_interval", "dob", "driver_license", "duration", "email_address", "event", "filename", "gender_sexuality", "healthcare_number", "ip_address", "language", "location", "location_address", "location_city", "location_coordinate", "location_country", "location_state", "location_zip", "marital_status", "money", "name", "name_family", "name_given", "numerical_pii", "organization", "occupation", "origin", "passport_number", "password", "phone_number", "physical_attribute", "political_affiliation", "religion", "ssn", "time", "url", "username", "vehicle_id", "zodiac_sign", "blood_type", "condition", "dose", "drug", "injury", "medical_process", "statistics", "bank_account", "credit_card", "credit_card_expiration", "cvv", "routing_number"]  # Put your initial list here
+        self.ban_list = ["account_number","address", "age", "date", "date_interval", "dob", "driver_license", "duration", "email_address", "event", "filename", "gender_sexuality", "healthcare_number", "ip_address", "language", "location", "Location Address", "location_city", "location_coordinate", "location_country", "location_state", "location_zip", "marital_status", "money", "name", "name_family", "name_given", "numerical_pii", "organization", "occupation", "origin", "passport_number", "password", "phone_number", "physical_attribute", "political_affiliation", "religion", "ssn", "time", "url", "username", "vehicle_id", "zodiac_sign", "blood_type", "condition", "dose", "drug", "injury", "medical_process", "statistics", "bank_account", "credit_card", "credit_card_expiration", "cvv", "routing_number","First Name", "Last Name"]  # Put your initial list here
         self.ban_list_version = 1
 
     def show_banlist(self):
         print(f"Ban List Version {self.ban_list_version}:")
         print(self.ban_list)
 
     def add_to_banlist(self, *args):
@@ -73,47 +73,51 @@
 
         # Determine if any PII fields were found
         contains_pii = len(pii_fields) > 0
 
         return contains_pii, pii_fields
 
     def swap(self, input_path: str, output_path: str) -> bool:
+    # Faker Setup
+    fake = Faker()
 
-        # Faker Setup
-        fake = Faker()
-
-        faker_methods = {
-            'account_number': fake.unique.random_number,
-            'age': fake.random_int,
-            'date': fake.date,
-            'email_address': fake.email,
-            'name': fake.name,
-            'phone_number': fake.phone_number,
-            # Add all other mappings
-            # ...
-        }
-
+    faker_methods = {
+        'account_number': fake.unique.random_number(digits=10, fix_len=True),
+        'age': lambda: fake.random_int(min=18, max=90),
+        'date': fake.date,
+        'email_address': fake.email,
+        'name': fake.name,
+        'phone_number': fake.phone_number,
+        'first_name': fake.first_name,
+        'last_name' : fake.last_name,
+        'address' : fake.address().replace("\n", ", "),
+        'email_address' : fake.email(),
+        'product_sku' : fake.random_int(min=1000, max=9999),
+        'product_quantity' : fake.random_int(min=1, max=10)
+       
+    }
+
+    # Read the file from train_path
+    df = pd.read_csv(input_path)
+
+    for col in df.columns:
+        if col in self.ban_list and col in faker_methods:
+            original_values = df[col].tolist()  # Keep a list of original values
+            df[col] = df[col].apply(lambda x: faker_methods[col])  # Synthetic values
+            synthetic_values = df[col].tolist()  # Keep a list of synthetic values
+
+            # Save each original and synthetic value pair in the database
+            for original, synthetic in zip(original_values, synthetic_values):
+                self.save(record_id=None, field_name=col, original_value=original, new_value=synthetic)
 
-        # Read the file from train_path
-        df = pd.read_csv(input_path)
-
-        for col in df.columns:
-            if col in self.ban_list and col in faker_methods:
-                original_values = df[col].tolist()  # Keep a list of original values
-                df[col] = df[col].apply(lambda x: faker_methods[col]())  # Synthetic values
-                synthetic_values = df[col].tolist()  # Keep a list of synthetic values
-
-                # Save each original and synthetic value pair in the database
-                for original, synthetic in zip(original_values, synthetic_values):
-                    self.save(record_id=None, field_name=col, original_value=original, new_value=synthetic)
+    # Save the modified DataFrame to a new file
+    df.to_csv(os.path.join(output_path, 'synthetic_output.csv'), index=False)
 
-        # Save the modified DataFrame to a new file
-        df.to_csv(os.path.join(output_path, 'synthetic_output.csv'), index=False)
+    return True
 
-        return True
 
     @staticmethod
     def redact(value: str) -> str:
         return "[REDACTED]"
 
     @staticmethod
     def hash(value: str) -> str:
```

### Comparing `datafog-1.3.5/datafog.egg-info/PKG-INFO` & `datafog-1.3.6/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.3.5
+Version: 1.3.6
 Summary: A Python package for data anonymization
 Author: Sid Mohan
 Author-email: sid@datafog.dev
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
```

### Comparing `datafog-1.3.5/setup.py` & `datafog-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Read README for the long description
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
 setup(
     name='datafog',
-    version='1.3.5',  # versioning of your package
+    version='1.3.6',  # versioning of your package
     packages=find_packages(),  # automatically find all packages
     author='Sid Mohan',
     author_email='sid@datafog.dev',
     description='A Python package for data anonymization',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     install_requires=['faker', 'pandas', 'sqlalchemy'],
```

### Comparing `datafog-1.3.5/tests/test_datafog.py` & `datafog-1.3.6/tests/test_datafog.py`

 * *Files identical despite different names*

