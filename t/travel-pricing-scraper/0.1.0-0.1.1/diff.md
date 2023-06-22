# Comparing `tmp/travel_pricing_scraper-0.1.0.tar.gz` & `tmp/travel_pricing_scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "travel_pricing_scraper-0.1.0.tar", max compression
+gzip compressed data, was "travel_pricing_scraper-0.1.1.tar", max compression
```

## Comparing `travel_pricing_scraper-0.1.0.tar` & `travel_pricing_scraper-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      392 2023-06-21 23:54:07.103227 travel_pricing_scraper-0.1.0/LICENSE
--rw-r--r--   0        0        0     2977 2023-06-21 20:24:53.888861 travel_pricing_scraper-0.1.0/README.md
--rw-r--r--   0        0        0     1777 2023-06-22 00:00:54.235400 travel_pricing_scraper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-18 07:57:19.387283 travel_pricing_scraper-0.1.0/travel_pricing_scraper/__init__.py
--rw-r--r--   0        0        0     1484 2023-06-20 18:13:01.366032 travel_pricing_scraper-0.1.0/travel_pricing_scraper/cli.py
--rw-r--r--   0        0        0     1314 2023-06-20 13:52:05.840166 travel_pricing_scraper-0.1.0/travel_pricing_scraper/flights.py
--rw-r--r--   0        0        0     2485 2023-06-20 16:20:35.774379 travel_pricing_scraper-0.1.0/travel_pricing_scraper/models.py
--rw-r--r--   0        0        0        0 2023-06-18 09:37:02.454618 travel_pricing_scraper-0.1.0/travel_pricing_scraper/scrapers/__init__.py
--rw-r--r--   0        0        0      519 2023-06-20 13:52:03.128237 travel_pricing_scraper-0.1.0/travel_pricing_scraper/scrapers/flights/__init__.py
--rw-r--r--   0        0        0     3952 2023-06-21 19:45:30.795156 travel_pricing_scraper-0.1.0/travel_pricing_scraper/scrapers/flights/decolar.py
--rw-r--r--   0        0        0      529 2023-06-18 22:55:34.145665 travel_pricing_scraper-0.1.0/travel_pricing_scraper/utils/__init__.py
--rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 travel_pricing_scraper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-06-21 23:54:07.103227 travel_pricing_scraper-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3057 2023-06-22 00:08:43.055175 travel_pricing_scraper-0.1.1/README.md
+-rw-r--r--   0        0        0     1777 2023-06-22 11:12:01.461933 travel_pricing_scraper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-18 07:57:19.387283 travel_pricing_scraper-0.1.1/travel_pricing_scraper/__init__.py
+-rw-r--r--   0        0        0     1484 2023-06-20 18:13:01.366032 travel_pricing_scraper-0.1.1/travel_pricing_scraper/cli.py
+-rw-r--r--   0        0        0     1314 2023-06-20 13:52:05.840166 travel_pricing_scraper-0.1.1/travel_pricing_scraper/flights.py
+-rw-r--r--   0        0        0     3102 2023-06-22 11:11:30.602590 travel_pricing_scraper-0.1.1/travel_pricing_scraper/models.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:37:02.454618 travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/__init__.py
+-rw-r--r--   0        0        0      519 2023-06-20 13:52:03.128237 travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/flights/__init__.py
+-rw-r--r--   0        0        0     3952 2023-06-21 19:45:30.795156 travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/flights/decolar.py
+-rw-r--r--   0        0        0      529 2023-06-18 22:55:34.145665 travel_pricing_scraper-0.1.1/travel_pricing_scraper/utils/__init__.py
+-rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 travel_pricing_scraper-0.1.1/PKG-INFO
```

### Comparing `travel_pricing_scraper-0.1.0/README.md` & `travel_pricing_scraper-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Travel Pricing Scraper
 
 [![Documentation Status](https://readthedocs.org/projects/travel-pricing-scraper/badge/?version=latest)](https://travel-pricing-scraper.readthedocs.io/en/latest/?badge=latest)
 [![CI](https://github.com/kalelmartinho/travel-pricing-scraper/actions/workflows/pipeline.yml/badge.svg)](https://github.com/kalelmartinho/travel-pricing-scraper/actions/workflows/pipeline.yml)
-
+[![PyPI version](https://badge.fury.io/py/travel-pricing-scraper.svg)](https://badge.fury.io/py/travel-pricing-scraper)
 ## Introduction
 
 The objective of this project is to demonstrate my skills in writing scalable, well-documented, and tested code. For this purpose, i've used Playwright as a web scraping tool to fetch airfare prices. While there are more specialized approaches to extract data of this kind, the main emphasis here is to showcase the ability to develop high-quality code using Playwright. 
 
 In this project, Playwright is used to navigate through different airline websites, fill in search forms, click buttons, and extract price information. It is important to note that in a real production environment, specific solutions would need to be considered for scraping airfare data. However, this project serves as a basic example of my skills in developing scalable, well-documented, and tested code, using Playwright as a widely documented and tested web scraping tool.
 
 ## Installation
@@ -33,26 +33,26 @@
 
 ## How to use
 
 ## How to use?
 You can use scraper via command line. For example:
 
 ```bash
-travel-pricing-scraper travels
+travels
 ```
 Options
 ```
 Origin airport code: CWB
 Destination airport code: POA
 Date in YYYY-MM-DD format (iso format): 2023-08-01
 ```
 
 OR with arguments:
 ```bash
-travel-pricing-scraper  --origin CWB --destination POA --date "2023-08-01"
+travels --origin CWB --destination POA --date "2023-08-01"
 ```
 
 Returns:
                                        
 
 | Origem | Destino | Embarque            | Chegada             | Preço     | Companhia |
 | ------ | ------- | ------------------- | ------------------- | --------- | --------- |
```

### Comparing `travel_pricing_scraper-0.1.0/pyproject.toml` & `travel_pricing_scraper-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "travel-pricing-scraper"
-version = "0.1.0"
+version = "0.1.1"
 description = "In this project, Playwright is used to navigate through different airline websites, fill in search forms, click buttons, and extract price information. "
 authors = ["Kalel L. Martinho <kalel@tutamail.com>"]
 license = "BeerWare"
 readme = "README.md"
 packages = [{include = "travel_pricing_scraper"}]
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `travel_pricing_scraper-0.1.0/travel_pricing_scraper/cli.py` & `travel_pricing_scraper-0.1.1/travel_pricing_scraper/cli.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.0/travel_pricing_scraper/flights.py` & `travel_pricing_scraper-0.1.1/travel_pricing_scraper/flights.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.0/travel_pricing_scraper/models.py` & `travel_pricing_scraper-0.1.1/travel_pricing_scraper/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,7 +38,16 @@
     def datestring_to_datetime(cls, v):
         """Converts date string to datetime.
         >>> Flight(id=uuid.UUID('50b5e710-db51-424c-b052-8383635ad39d'), origin='CWB', destination='POA', departure_date='2021-07-08', arrive_date='2021-07-10', price=100.0, carrier='GOL')
         Flight(id=UUID('...'), origin='CWB', destination='POA', departure_date=datetime.datetime(2021, 7, 8, 0, 0), arrive_date=datetime.datetime(2021, 7, 10, 0, 0), price=100.0, carrier='GOL')"""
         if isinstance(v, str):
             return dt.fromisoformat(v)
         return v
+    
+    @validator('price')
+    def brl_to_float(cls, v):
+        """Converts BRL string to float.
+        >>> Flight(id=uuid.UUID('50b5e710-db51-424c-b052-8383635ad39d'), origin='CWB', destination='POA', departure_date=dt(2021, 7, 8, 0, 0), arrive_date=dt(2021, 7, 10, 0, 0), price='100,00', carrier='GOL')
+        Flight(id=UUID('...'), origin='CWB', destination='POA', departure_date=datetime.datetime(2021, 7, 8, 0, 0), arrive_date=datetime.datetime(2021, 7, 10, 0, 0), price=100.0, carrier='GOL')"""
+        if isinstance(v, str):
+            return float(v.replace('.', '').replace(',', '.'))
+        return v
```

### Comparing `travel_pricing_scraper-0.1.0/travel_pricing_scraper/scrapers/flights/__init__.py` & `travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/flights/__init__.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.0/travel_pricing_scraper/scrapers/flights/decolar.py` & `travel_pricing_scraper-0.1.1/travel_pricing_scraper/scrapers/flights/decolar.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.0/travel_pricing_scraper/utils/__init__.py` & `travel_pricing_scraper-0.1.1/travel_pricing_scraper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `travel_pricing_scraper-0.1.0/PKG-INFO` & `travel_pricing_scraper-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: travel-pricing-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: In this project, Playwright is used to navigate through different airline websites, fill in search forms, click buttons, and extract price information. 
 License: Beerware
 Author: Kalel L. Martinho
 Author-email: kalel@tutamail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -24,15 +24,15 @@
 Project-URL: Docs, https://travel-pricing-scraper.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # Travel Pricing Scraper
 
 [![Documentation Status](https://readthedocs.org/projects/travel-pricing-scraper/badge/?version=latest)](https://travel-pricing-scraper.readthedocs.io/en/latest/?badge=latest)
 [![CI](https://github.com/kalelmartinho/travel-pricing-scraper/actions/workflows/pipeline.yml/badge.svg)](https://github.com/kalelmartinho/travel-pricing-scraper/actions/workflows/pipeline.yml)
-
+[![PyPI version](https://badge.fury.io/py/travel-pricing-scraper.svg)](https://badge.fury.io/py/travel-pricing-scraper)
 ## Introduction
 
 The objective of this project is to demonstrate my skills in writing scalable, well-documented, and tested code. For this purpose, i've used Playwright as a web scraping tool to fetch airfare prices. While there are more specialized approaches to extract data of this kind, the main emphasis here is to showcase the ability to develop high-quality code using Playwright. 
 
 In this project, Playwright is used to navigate through different airline websites, fill in search forms, click buttons, and extract price information. It is important to note that in a real production environment, specific solutions would need to be considered for scraping airfare data. However, this project serves as a basic example of my skills in developing scalable, well-documented, and tested code, using Playwright as a widely documented and tested web scraping tool.
 
 ## Installation
@@ -59,26 +59,26 @@
 
 ## How to use
 
 ## How to use?
 You can use scraper via command line. For example:
 
 ```bash
-travel-pricing-scraper travels
+travels
 ```
 Options
 ```
 Origin airport code: CWB
 Destination airport code: POA
 Date in YYYY-MM-DD format (iso format): 2023-08-01
 ```
 
 OR with arguments:
 ```bash
-travel-pricing-scraper  --origin CWB --destination POA --date "2023-08-01"
+travels --origin CWB --destination POA --date "2023-08-01"
 ```
 
 Returns:
                                        
 
 | Origem | Destino | Embarque            | Chegada             | Preço     | Companhia |
 | ------ | ------- | ------------------- | ------------------- | --------- | --------- |
```

