# Comparing `tmp/rain_orm-1.0.4.tar.gz` & `tmp/rain_orm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rain_orm-1.0.4.tar", last modified: Mon Jun 12 11:26:25 2023, max compression
+gzip compressed data, was "rain_orm-1.0.5.tar", last modified: Thu Jun 22 02:03:39 2023, max compression
```

## Comparing `rain_orm-1.0.4.tar` & `rain_orm-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.359308 rain_orm-1.0.4/
--rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3399 2023-06-12 11:26:25.360304 rain_orm-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3118 2023-06-12 11:21:58.000000 rain_orm-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.326174 rain_orm-1.0.4/rain_orm/
--rw-rw-rw-   0        0        0      139 2023-06-12 11:25:53.000000 rain_orm-1.0.4/rain_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.346175 rain_orm-1.0.4/rain_orm/column/
--rw-rw-rw-   0        0        0      153 2023-06-05 03:57:35.000000 rain_orm-1.0.4/rain_orm/column/__init__.py
--rw-rw-rw-   0        0        0     1576 2023-06-05 11:20:16.000000 rain_orm-1.0.4/rain_orm/column/base.py
--rw-rw-rw-   0        0        0      271 2023-06-05 03:57:35.000000 rain_orm-1.0.4/rain_orm/column/date.py
--rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.4/rain_orm/column/number.py
--rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.4/rain_orm/column/string.py
--rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.4/rain_orm/common.py
--rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.4/rain_orm/db.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.349175 rain_orm-1.0.4/rain_orm/error/
--rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.4/rain_orm/error/__init__.py
--rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.4/rain_orm/error/error.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.356308 rain_orm-1.0.4/rain_orm/sql_builder/
--rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.4/rain_orm/sql_builder/__init__.py
--rw-rw-rw-   0        0        0     1280 2023-06-08 12:04:47.000000 rain_orm-1.0.4/rain_orm/sql_builder/ddl_builder.py
--rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.4/rain_orm/sql_builder/dmldql_builder.py
--rw-rw-rw-   0        0        0     6977 2023-06-08 02:54:13.000000 rain_orm-1.0.4/rain_orm/table.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.335176 rain_orm-1.0.4/rain_orm.egg-info/
--rw-rw-rw-   0        0        0     3399 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 11:26:25.360304 rain_orm-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      474 2023-06-12 11:25:53.000000 rain_orm-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.358307 rain_orm-1.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 02:03:39.056347 rain_orm-1.0.5/
+-rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3514 2023-06-22 02:03:39.057346 rain_orm-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2023-06-22 02:02:54.000000 rain_orm-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 02:03:39.027582 rain_orm-1.0.5/rain_orm/
+-rw-rw-rw-   0        0        0      139 2023-06-22 01:48:08.000000 rain_orm-1.0.5/rain_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 02:03:39.044300 rain_orm-1.0.5/rain_orm/column/
+-rw-rw-rw-   0        0        0      153 2023-06-05 03:57:35.000000 rain_orm-1.0.5/rain_orm/column/__init__.py
+-rw-rw-rw-   0        0        0     1602 2023-06-22 02:02:54.000000 rain_orm-1.0.5/rain_orm/column/base.py
+-rw-rw-rw-   0        0        0      271 2023-06-05 03:57:35.000000 rain_orm-1.0.5/rain_orm/column/date.py
+-rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.5/rain_orm/column/number.py
+-rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.5/rain_orm/column/string.py
+-rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.5/rain_orm/common.py
+-rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.5/rain_orm/db.py
+drwxrwxrwx   0        0        0        0 2023-06-22 02:03:39.048837 rain_orm-1.0.5/rain_orm/error/
+-rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.5/rain_orm/error/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.5/rain_orm/error/error.py
+drwxrwxrwx   0        0        0        0 2023-06-22 02:03:39.054341 rain_orm-1.0.5/rain_orm/sql_builder/
+-rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.5/rain_orm/sql_builder/__init__.py
+-rw-rw-rw-   0        0        0     1280 2023-06-08 12:04:47.000000 rain_orm-1.0.5/rain_orm/sql_builder/ddl_builder.py
+-rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.5/rain_orm/sql_builder/dmldql_builder.py
+-rw-rw-rw-   0        0        0     7087 2023-06-22 01:57:14.000000 rain_orm-1.0.5/rain_orm/table.py
+drwxrwxrwx   0        0        0        0 2023-06-22 02:03:39.035300 rain_orm-1.0.5/rain_orm.egg-info/
+-rw-rw-rw-   0        0        0     3514 2023-06-22 02:03:38.000000 rain_orm-1.0.5/rain_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2023-06-22 02:03:38.000000 rain_orm-1.0.5/rain_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 02:03:38.000000 rain_orm-1.0.5/rain_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-22 02:03:38.000000 rain_orm-1.0.5/rain_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-22 02:03:38.000000 rain_orm-1.0.5/rain_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 02:03:39.058349 rain_orm-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-06-22 01:48:08.000000 rain_orm-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 02:03:39.055352 rain_orm-1.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.5/tests/__init__.py
```

### Comparing `rain_orm-1.0.4/LICENSE` & `rain_orm-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.4/PKG-INFO` & `rain_orm-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: rain_orm
-Version: 1.0.4
-Summary: a tiny orm frame
-Home-page: https://github.com/cgynb/rain-orm
-Author: rain
-Author-email: 948628463@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # rain-orm
 
 a tiny orm frame
 
 # Install
 
 it's easy to install via pip
@@ -105,16 +93,20 @@
         "name": VarChar(30, unique=True),
         "password": VarChar(30),
         "class_id": Int(default=1)
     }
 
 ```
 ## Auto Migrate
+
 ```python
-rain_orm.Table.auto_migrate()
+# all subclasses that inherit rain_orm.Table
+rain_orm.Table.auto_migrate() 
+# create StudentModel
+rain_orm.Table.auto_migrate(StudentModel)
 ```
 
 
 ## CRUD Example
 
 ### Read
 
@@ -165,9 +157,7 @@
 ### Delete
 
 ```python
 StudentModel().where("id = ?", 22).one()  # get student instance first
 ok = stu.delete()  # call delete method
 ```
 
-
-
```

### Comparing `rain_orm-1.0.4/README.md` & `rain_orm-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: rain_orm
+Version: 1.0.5
+Summary: a tiny orm frame
+Home-page: https://github.com/cgynb/rain-orm
+Author: rain
+Author-email: 948628463@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # rain-orm
 
 a tiny orm frame
 
 # Install
 
 it's easy to install via pip
@@ -93,16 +105,20 @@
         "name": VarChar(30, unique=True),
         "password": VarChar(30),
         "class_id": Int(default=1)
     }
 
 ```
 ## Auto Migrate
+
 ```python
-rain_orm.Table.auto_migrate()
+# all subclasses that inherit rain_orm.Table
+rain_orm.Table.auto_migrate() 
+# create StudentModel
+rain_orm.Table.auto_migrate(StudentModel)
 ```
 
 
 ## CRUD Example
 
 ### Read
 
@@ -153,7 +169,9 @@
 ### Delete
 
 ```python
 StudentModel().where("id = ?", 22).one()  # get student instance first
 ok = stu.delete()  # call delete method
 ```
 
+
+
```

### Comparing `rain_orm-1.0.4/rain_orm/column/base.py` & `rain_orm-1.0.5/rain_orm/column/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,26 +34,26 @@
     @property
     def value(self):
         if self.__value is None:
             if callable(self.default):
                 self.__value = self.default()
             else:
                 self.__value = self.default
-            return self.__value
+        return self.__value
 
     @value.setter
     def value(self, value):
         if not self.check(value):
             warnings.warn(f"data type is different from definition \"{self.type_name}\"")
         self.__value = value
 
 
 class Number(Type):
     def check(self, val) -> bool:
-        return isinstance(val, int) or isinstance(val, float)
+        return isinstance(val, int) or isinstance(val, float) or val is None
 
 
 class String(Type):
     def check(self, val):
-        return isinstance(val, str)
+        return isinstance(val, str) or val is None
 
 # class Date()
```

### Comparing `rain_orm-1.0.4/rain_orm/column/string.py` & `rain_orm-1.0.5/rain_orm/column/string.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.4/rain_orm/db.py` & `rain_orm-1.0.5/rain_orm/db.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.4/rain_orm/sql_builder/ddl_builder.py` & `rain_orm-1.0.5/rain_orm/sql_builder/ddl_builder.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.4/rain_orm/sql_builder/dmldql_builder.py` & `rain_orm-1.0.5/rain_orm/sql_builder/dmldql_builder.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.4/rain_orm/table.py` & `rain_orm-1.0.5/rain_orm/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,18 @@
     __lock = threading.Lock()
 
     @classmethod
     def set_db(cls, db):
         cls.__db = db
 
     @classmethod
-    def auto_migrate(cls):
+    def auto_migrate(cls, *classes):
+        class_lst = classes if len(classes) > 0 else cls.__subclasses__()
         ddls = []
-        for subcls in cls.__subclasses__():
+        for subcls in class_lst:
             ddl_builder = DDLBuilder(subcls.__table__)
             for k, v in subcls.__fields__.items():
                 ddl_builder.add_field(field_name=k, field_type=v.type_name, **v.constraint)
             ddls.append(ddl_builder.create_sql)
         with cls.__lock:
             for ddl in ddls:
                 cls.__db.cursor.execute(ddl)
@@ -43,16 +44,19 @@
         if not all([isinstance(item, Type) for _, item in self.__fields__.items()]):
             raise ValueError(f"items of __fields__ should be instance of rain_orm.column.Type")
 
         self.instance = copy.deepcopy(self.__fields__)
         self.__dmldql_builder = DMLDQLBuilder(self.__table__)
         for k, v in kwargs.items():
             self.instance[k].value = v
+        self.is_none = False
 
     def __str__(self):
+        if self.is_none is True:
+            return "None"
         table = self.__table__
         fields = list(self.__fields__.keys())
         instance = "{\n"
         for k, v in self.instance.items():
             if isinstance(v.value, str):
                 v = f"'{v.value}'"
             instance += f"\t\t{k}: {v},\n"
@@ -67,15 +71,15 @@
         return str(self)
 
     def __getattr__(self, key):
         return self.instance.get(key).value
 
     # update
     def __setattr__(self, key, value):
-        if key in ["instance", "_Table__dmldql_builder"]:
+        if key in ["instance", "_Table__dmldql_builder", "is_none"]:
             self.__dict__[key] = value
         else:
             self.update(key, value)
 
     # select condition
     def where(self, condition, value=None):
         self.__dmldql_builder.where(condition, value)
@@ -177,11 +181,10 @@
                 self.__db.cursor.execute(self.__dmldql_builder.delete_sql)
                 self.__db.commit()
             except pymysql.MySQLError as e:
                 print(e)
                 self.__db.rollback()
                 return False
             else:
-                for key in self.instance.keys():
-                    self.instance[key].value = None
+                self.is_none = True
                 return True
```

### Comparing `rain_orm-1.0.4/rain_orm.egg-info/PKG-INFO` & `rain_orm-1.0.5/rain_orm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rain-orm
-Version: 1.0.4
+Version: 1.0.5
 Summary: a tiny orm frame
 Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -105,16 +105,20 @@
         "name": VarChar(30, unique=True),
         "password": VarChar(30),
         "class_id": Int(default=1)
     }
 
 ```
 ## Auto Migrate
+
 ```python
-rain_orm.Table.auto_migrate()
+# all subclasses that inherit rain_orm.Table
+rain_orm.Table.auto_migrate() 
+# create StudentModel
+rain_orm.Table.auto_migrate(StudentModel)
 ```
 
 
 ## CRUD Example
 
 ### Read
```

### Comparing `rain_orm-1.0.4/rain_orm.egg-info/SOURCES.txt` & `rain_orm-1.0.5/rain_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

