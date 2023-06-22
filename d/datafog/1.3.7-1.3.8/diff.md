# Comparing `tmp/datafog-1.3.7.tar.gz` & `tmp/datafog-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-1.3.7.tar", last modified: Thu Jun 22 18:59:28 2023, max compression
+gzip compressed data, was "datafog-1.3.8.tar", last modified: Thu Jun 22 20:20:20 2023, max compression
```

## Comparing `datafog-1.3.7.tar` & `datafog-1.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:59:28.805980 datafog-1.3.7/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.3.7/LICENSE.MD
--rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:59:28.805792 datafog-1.3.7/PKG-INFO
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:59:28.803932 datafog-1.3.7/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.7/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     8480 2023-06-22 18:58:54.000000 datafog-1.3.7/datafog/datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.7/datafog/models.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:59:28.804884 datafog-1.3.7/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:59:28.000000 datafog-1.3.7/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 18:59:28.000000 datafog-1.3.7/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 18:59:28.000000 datafog-1.3.7/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2023-06-22 18:59:28.000000 datafog-1.3.7/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 18:59:28.000000 datafog-1.3.7/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 18:59:28.806034 datafog-1.3.7/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)      846 2023-06-22 18:59:17.000000 datafog-1.3.7/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:59:28.805547 datafog-1.3.7/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.7/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.7/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.7/tests/test_models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 20:20:20.256418 datafog-1.3.8/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.3.8/LICENSE.MD
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 20:20:20.256256 datafog-1.3.8/PKG-INFO
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 20:20:20.254550 datafog-1.3.8/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.8/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8494 2023-06-22 20:18:47.000000 datafog-1.3.8/datafog/datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.8/datafog/models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 20:20:20.255389 datafog-1.3.8/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 20:20:20.000000 datafog-1.3.8/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 20:20:20.000000 datafog-1.3.8/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 20:20:20.000000 datafog-1.3.8/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2023-06-22 20:20:20.000000 datafog-1.3.8/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 20:20:20.000000 datafog-1.3.8/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 20:20:20.256469 datafog-1.3.8/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)      846 2023-06-22 20:20:08.000000 datafog-1.3.8/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 20:20:20.256085 datafog-1.3.8/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.8/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.8/tests/test_datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.8/tests/test_models.py
```

### Comparing `datafog-1.3.7/LICENSE.MD` & `datafog-1.3.8/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `datafog-1.3.7/PKG-INFO` & `datafog-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.3.7
+Version: 1.3.8
 Summary: A Python package for data anonymization
 Author: Sid Mohan
 Author-email: sid@datafog.dev
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
```

### Comparing `datafog-1.3.7/datafog/datafog.py` & `datafog-1.3.8/datafog/datafog.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,21 @@
 
 class DataFog:
 
     def __init__(self, db_path='sqlite:///./test.db'):
         self.engine = create_engine(db_path, echo = False)
         Base.metadata.create_all(self.engine)  # Create tables
         self.Session = sessionmaker(bind=self.engine)
-        self.ban_list = ["account_number","address", "age", "date", "date_interval", "dob", "driver_license", "duration", "email_address", "event", "filename", "gender_sexuality", "healthcare_number", "ip_address", "language", "location", "Location Address", "location_city", "location_coordinate", "location_country", "location_state", "location_zip", "marital_status", "money", "name", "name_family", "name_given", "numerical_pii", "organization", "occupation", "origin", "passport_number", "password", "phone_number", "physical_attribute", "political_affiliation", "religion", "ssn", "time", "url", "username", "vehicle_id", "zodiac_sign", "blood_type", "condition", "dose", "drug", "injury", "medical_process", "statistics", "bank_account", "credit_card", "credit_card_expiration", "cvv", "routing_number","First Name", "Last Name"]  # Put your initial list here
+        self.ban_list =["address","age","bank_account","credit_card",
+        "credit_card_expiration","date","email_address","first_name",
+        "ip_address","last_name","location","city","latlong","country",
+        "state","zip","name","occupation","passport_number","password",
+        "phone_number","product_sku","routing_number","ssn","time","username","license_plate"]
+
+ # Put your initial list here
         self.ban_list_version = 1
 
     def show_banlist(self):
         print(f"Ban List Version {self.ban_list_version}:")
         print(self.ban_list)
 
     def add_to_banlist(self, *args):
@@ -77,45 +83,62 @@
         return contains_pii, pii_fields
 
     def swap(self, input_path: str, output_path: str) -> bool:
         # Faker Setup
         fake = Faker()
 
         faker_methods = {
-            'account_number': fake.unique.random_number(digits=10, fix_len=True),
-            'age': lambda: fake.random_int(min=18, max=90),
-            'date': fake.date,
-            'email_address': fake.email,
-            'name': fake.name,
-            'phone_number': fake.phone_number,
-            'first_name': fake.first_name,
-            'last_name' : fake.last_name,
-            'address' : fake.address().replace("\n", ", "),
-            'email_address' : fake.email(),
-            'product_sku' : fake.random_int(min=1000, max=9999),
-            'product_quantity' : fake.random_int(min=1, max=10)
+            "address": fake.address,
+            "age": lambda: fake.random_int(min=18, max=90),
+            "bank_account": fake.bban,
+            "credit_card": fake.credit_card_full,
+            "credit_card_expiration": fake.credit_card_expire,
+            "date": fake.date,
+            "email_address": fake.email,
+            "first_name": fake.first_name,
+            "ip_address": fake.ipv4,
+            "last_name": fake.last_name,
+            "location": fake.location_on_land,
+            "city": fake.city,
+            "latlong": fake.latlng,
+            "country": fake.country,
+            "state": fake.state,
+            "zip": fake.postcode,
+            "name": fake.name,
+            "occupation": fake.job,
+            "password": lambda: fake.password(length=12, special_chars=False, upper_case=True),
+            "phone_number": fake.phone_number,
+            "product_sku": fake.isbn13,
+            "routing_number": fake.aba,
+            "ssn": fake.ssn,
+            "time": fake.time,
+            "license_plate": fake.license_plate
+            }
+
+
         
-        }
 
         # Read the file from train_path
         df = pd.read_csv(input_path)
 
         for col in df.columns:
             if col in self.ban_list and col in faker_methods:
                 original_values = df[col].tolist()  # Keep a list of original values
-                df[col] = df[col].apply(lambda x: faker_methods[col])  # Synthetic values
+                df[col] = df[col].apply(lambda x: faker_methods[col]())  # Synthetic values
                 synthetic_values = df[col].tolist()  # Keep a list of synthetic values
 
-                # Save each original and synthetic value pair in the database
+            # Save each original and synthetic value pair in the database
                 for original, synthetic in zip(original_values, synthetic_values):
                     self.save(record_id=None, field_name=col, original_value=original, new_value=synthetic)
 
         # Save the modified DataFrame to a new file
         df.to_csv(os.path.join(output_path, 'synthetic_output.csv'), index=False)
 
+
+        print(df)
         return True
 
 
     @staticmethod
     def redact(value: str) -> str:
         return "[REDACTED]"
```

### Comparing `datafog-1.3.7/datafog.egg-info/PKG-INFO` & `datafog-1.3.8/datafog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.3.7
+Version: 1.3.8
 Summary: A Python package for data anonymization
 Author: Sid Mohan
 Author-email: sid@datafog.dev
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
```

### Comparing `datafog-1.3.7/setup.py` & `datafog-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Read README for the long description
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
 setup(
     name='datafog',
-    version='1.3.7',  # versioning of your package
+    version='1.3.8',  # versioning of your package
     packages=find_packages(),  # automatically find all packages
     author='Sid Mohan',
     author_email='sid@datafog.dev',
     description='A Python package for data anonymization',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     install_requires=['faker', 'pandas', 'sqlalchemy'],
```

### Comparing `datafog-1.3.7/tests/test_datafog.py` & `datafog-1.3.8/tests/test_datafog.py`

 * *Files identical despite different names*

