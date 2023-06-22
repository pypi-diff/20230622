# Comparing `tmp/travel_pricing_scraper-0.1.1.tar.gz` & `tmp/travel_pricing_scraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "travel_pricing_scraper-0.1.1.tar", max compression
+gzip compressed data, was "travel_pricing_scraper-0.1.2.tar", max compression
```

## Comparing `travel_pricing_scraper-0.1.1.tar` & `travel_pricing_scraper-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      392 2023-06-21 23:54:07.103227 travel_pricing_scraper-0.1.1/LICENSE
--rw-r--r--   0        0        0     3057 2023-06-22 00:08:43.055175 travel_pricing_scraper-0.1.1/README.md
--rw-r--r--   0        0        0     1777 2023-06-22 11:12:01.461933 travel_pricing_scraper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-18 07:57:19.387283 travel_pricing_scraper-0.1.1/travel_pricing_scraper/__init__.py
--rw-r--r--   0        0        0     1484 2023-06-20 18:13:01.366032 travel_pricing_scraper-0.1.1/travel_pricing_scraper/cli.py
--rw-r--r--   0        0        0     1314 2023-06-20 13:52:05.840166 travel_pricing_scraper-0.1.1/travel_pricing_scraper/flights.py
--rw-r--r--   0        0        0     3102 2023-06-22 11:11:30.602590 travel_pricing_scraper-0.1.1/travel_pricing_scraper/models.py
--rw-r--r--   0        0        0        0 2023-06-18 09:37:02.454618 travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/__init__.py
--rw-r--r--   0        0        0      519 2023-06-20 13:52:03.128237 travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/flights/__init__.py
--rw-r--r--   0        0        0     3952 2023-06-21 19:45:30.795156 travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/flights/decolar.py
--rw-r--r--   0        0        0      529 2023-06-18 22:55:34.145665 travel_pricing_scraper-0.1.1/travel_pricing_scraper/utils/__init__.py
--rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 travel_pricing_scraper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-06-21 23:54:07.103227 travel_pricing_scraper-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3057 2023-06-22 00:08:43.055175 travel_pricing_scraper-0.1.2/README.md
+-rw-r--r--   0        0        0     1777 2023-06-22 11:27:30.942207 travel_pricing_scraper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-18 07:57:19.387283 travel_pricing_scraper-0.1.2/travel_pricing_scraper/__init__.py
+-rw-r--r--   0        0        0     1484 2023-06-20 18:13:01.366032 travel_pricing_scraper-0.1.2/travel_pricing_scraper/cli.py
+-rw-r--r--   0        0        0     1381 2023-06-22 11:23:26.412794 travel_pricing_scraper-0.1.2/travel_pricing_scraper/flights.py
+-rw-r--r--   0        0        0     3112 2023-06-22 11:21:01.988200 travel_pricing_scraper-0.1.2/travel_pricing_scraper/models.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:37:02.454618 travel_pricing_scraper-0.1.2/travel_pricing_scraper/scrapers/__init__.py
+-rw-r--r--   0        0        0      519 2023-06-20 13:52:03.128237 travel_pricing_scraper-0.1.2/travel_pricing_scraper/scrapers/flights/__init__.py
+-rw-r--r--   0        0        0     3952 2023-06-21 19:45:30.795156 travel_pricing_scraper-0.1.2/travel_pricing_scraper/scrapers/flights/decolar.py
+-rw-r--r--   0        0        0      529 2023-06-18 22:55:34.145665 travel_pricing_scraper-0.1.2/travel_pricing_scraper/utils/__init__.py
+-rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 travel_pricing_scraper-0.1.2/PKG-INFO
```

### Comparing `travel_pricing_scraper-0.1.1/README.md` & `travel_pricing_scraper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.1/pyproject.toml` & `travel_pricing_scraper-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "travel-pricing-scraper"
-version = "0.1.1"
+version = "0.1.2"
 description = "In this project, Playwright is used to navigate through different airline websites, fill in search forms, click buttons, and extract price information. "
 authors = ["Kalel L. Martinho <kalel@tutamail.com>"]
 license = "BeerWare"
 readme = "README.md"
 packages = [{include = "travel_pricing_scraper"}]
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `travel_pricing_scraper-0.1.1/travel_pricing_scraper/cli.py` & `travel_pricing_scraper-0.1.2/travel_pricing_scraper/cli.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.1/travel_pricing_scraper/flights.py` & `travel_pricing_scraper-0.1.2/travel_pricing_scraper/flights.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         ValueError: If date is not in YYYY-MM-DD format (iso format).
 
     Examples:
         >>> flights('CWB', 'POA', '{}'.format(now_isoformat))
         [...]
     """   # doctest: +ELLIPSIS
 
+    origin = origin.upper()
+    destination = destination.upper()
+
     if not (date[4] == '-' and date[7] == '-' and len(date) == 10):
         raise ValueError('Date must be in YYYY-MM-DD format (iso format).')
 
     if not asyncio.get_event_loop().is_running():
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
     flights = loop.run_until_complete(
```

### Comparing `travel_pricing_scraper-0.1.1/travel_pricing_scraper/models.py` & `travel_pricing_scraper-0.1.2/travel_pricing_scraper/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         """Converts date string to datetime.
         >>> Flight(id=uuid.UUID('50b5e710-db51-424c-b052-8383635ad39d'), origin='CWB', destination='POA', departure_date='2021-07-08', arrive_date='2021-07-10', price=100.0, carrier='GOL')
         Flight(id=UUID('...'), origin='CWB', destination='POA', departure_date=datetime.datetime(2021, 7, 8, 0, 0), arrive_date=datetime.datetime(2021, 7, 10, 0, 0), price=100.0, carrier='GOL')"""
         if isinstance(v, str):
             return dt.fromisoformat(v)
         return v
     
-    @validator('price')
+    @validator('price', pre=True)
     def brl_to_float(cls, v):
         """Converts BRL string to float.
         >>> Flight(id=uuid.UUID('50b5e710-db51-424c-b052-8383635ad39d'), origin='CWB', destination='POA', departure_date=dt(2021, 7, 8, 0, 0), arrive_date=dt(2021, 7, 10, 0, 0), price='100,00', carrier='GOL')
         Flight(id=UUID('...'), origin='CWB', destination='POA', departure_date=datetime.datetime(2021, 7, 8, 0, 0), arrive_date=datetime.datetime(2021, 7, 10, 0, 0), price=100.0, carrier='GOL')"""
         if isinstance(v, str):
             return float(v.replace('.', '').replace(',', '.'))
         return v
```

### Comparing `travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/flights/__init__.py` & `travel_pricing_scraper-0.1.2/travel_pricing_scraper/scrapers/flights/__init__.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/flights/decolar.py` & `travel_pricing_scraper-0.1.2/travel_pricing_scraper/scrapers/flights/decolar.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.1/travel_pricing_scraper/utils/__init__.py` & `travel_pricing_scraper-0.1.2/travel_pricing_scraper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.1/PKG-INFO` & `travel_pricing_scraper-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: travel-pricing-scraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: In this project, Playwright is used to navigate through different airline websites, fill in search forms, click buttons, and extract price information. 
 License: Beerware
 Author: Kalel L. Martinho
 Author-email: kalel@tutamail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

