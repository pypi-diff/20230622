# Comparing `tmp/hamsclientfork-0.2.7.tar.gz` & `tmp/hamsclientfork-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamsclientfork-0.2.7.tar", last modified: Fri Mar  3 18:58:31 2023, max compression
+gzip compressed data, was "hamsclientfork-0.2.8.tar", last modified: Thu Jun 22 10:14:55 2023, max compression
```

## Comparing `hamsclientfork-0.2.7.tar` & `hamsclientfork-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-03 18:58:31.786000 hamsclientfork-0.2.7/
--rw-r--r--   0 user      (1000) user      (1000)       40 2023-01-18 08:30:39.000000 hamsclientfork-0.2.7/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)     1073 2023-01-18 08:27:55.000000 hamsclientfork-0.2.7/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1368 2023-03-03 18:58:31.786000 hamsclientfork-0.2.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      454 2023-01-18 08:37:32.000000 hamsclientfork-0.2.7/README.md
--rw-r--r--   0 user      (1000) user      (1000)      730 2023-01-18 08:27:55.000000 hamsclientfork-0.2.7/README.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-03 18:58:31.785000 hamsclientfork-0.2.7/hamsclientfork/
--rw-r--r--   0 user      (1000) user      (1000)      215 2023-02-13 11:49:36.000000 hamsclientfork-0.2.7/hamsclientfork/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       27 2023-01-18 08:27:55.000000 hamsclientfork-0.2.7/hamsclientfork/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     9588 2023-02-13 11:48:47.000000 hamsclientfork-0.2.7/hamsclientfork/client.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-03 18:58:31.786000 hamsclientfork-0.2.7/hamsclientfork.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1368 2023-03-03 18:58:31.000000 hamsclientfork-0.2.7/hamsclientfork.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      324 2023-03-03 18:58:31.000000 hamsclientfork-0.2.7/hamsclientfork.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-03-03 18:58:31.000000 hamsclientfork-0.2.7/hamsclientfork.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       67 2023-03-03 18:58:31.000000 hamsclientfork-0.2.7/hamsclientfork.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       15 2023-03-03 18:58:31.000000 hamsclientfork-0.2.7/hamsclientfork.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-03-03 18:58:31.786000 hamsclientfork-0.2.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1249 2023-03-03 18:57:57.000000 hamsclientfork-0.2.7/setup.py
--rw-r--r--   0 user      (1000) user      (1000)       95 2023-01-18 08:27:55.000000 hamsclientfork-0.2.7/tox.ini
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 10:14:55.294000 hamsclientfork-0.2.8/
+-rw-r--r--   0 user      (1000) user      (1000)       40 2023-01-18 08:30:39.000000 hamsclientfork-0.2.8/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)     1073 2023-01-18 08:27:55.000000 hamsclientfork-0.2.8/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     1368 2023-06-22 10:14:55.293000 hamsclientfork-0.2.8/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      454 2023-01-18 08:37:32.000000 hamsclientfork-0.2.8/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      730 2023-01-18 08:27:55.000000 hamsclientfork-0.2.8/README.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 10:14:55.293000 hamsclientfork-0.2.8/hamsclientfork/
+-rw-r--r--   0 user      (1000) user      (1000)      215 2023-02-13 11:49:36.000000 hamsclientfork-0.2.8/hamsclientfork/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       27 2023-01-18 08:27:55.000000 hamsclientfork-0.2.8/hamsclientfork/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)    12423 2023-06-22 10:10:34.000000 hamsclientfork-0.2.8/hamsclientfork/client.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-22 10:12:27.000000 hamsclientfork-0.2.8/hamsclientfork/py.typed
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 10:14:55.293000 hamsclientfork-0.2.8/hamsclientfork.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1368 2023-06-22 10:14:54.000000 hamsclientfork-0.2.8/hamsclientfork.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      348 2023-06-22 10:14:55.000000 hamsclientfork-0.2.8/hamsclientfork.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-22 10:14:54.000000 hamsclientfork-0.2.8/hamsclientfork.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       67 2023-06-22 10:14:54.000000 hamsclientfork-0.2.8/hamsclientfork.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       15 2023-06-22 10:14:54.000000 hamsclientfork-0.2.8/hamsclientfork.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-22 10:14:55.294000 hamsclientfork-0.2.8/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1249 2023-06-22 10:14:01.000000 hamsclientfork-0.2.8/setup.py
+-rw-r--r--   0 user      (1000) user      (1000)       95 2023-01-18 08:27:55.000000 hamsclientfork-0.2.8/tox.ini
```

### Comparing `hamsclientfork-0.2.7/LICENSE` & `hamsclientfork-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hamsclientfork-0.2.7/PKG-INFO` & `hamsclientfork-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamsclientfork
-Version: 0.2.7
+Version: 0.2.8
 Summary: Library to get data from meteo swiss
 Home-page: https://github.com/Rudd-O/hamsclientfork
 Author: websylv
 Author-email: div@webhu.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hamsclientfork-0.2.7/README.rst` & `hamsclientfork-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `hamsclientfork-0.2.7/hamsclientfork/client.py` & `hamsclientfork-0.2.8/hamsclientfork/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import geopy
 import geopy.distance
 import json
 import logging
 import pandas as pd
-import requests
+import requests  # type: ignore
 
 from bs4 import BeautifulSoup
 from enum import Enum
-from typing import Any
+from typing import Any, TypedDict
 
 
 class StationType(str, Enum):
     """Station type."""
 
     WEATHER = "weather"
     PRECIPITATION = "precipitation"
 
 
 _LOGGER = logging.getLogger(__name__)
 
+_HEADERS = {
+    "Accept": "text/html,application/xhtml+xml,application/xml;"
+    "q=0.9,image/webp,*/*;q=0.8",
+    "Accept-Encoding": "gzip, deflate, sdch",
+    "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML"
+    ", like Gecko) Chrome/1337 Safari/537.36",
+}
+
 MS_BASE_URL = "https://www.meteosuisse.admin.ch"
 JSON_FORECAST_URL = "https://app-prod-ws.meteoswiss-app.ch/v1/forecast?plz={}00&graph=false&warning=true"
 MS_SEARCH_URL = "https://www.meteosuisse.admin.ch/home/actualite/infos.html?ort={}&pageIndex=0&tab=search_tab"
 CURRENT_CONDITION_URL = (
     "https://data.geo.admin.ch/ch.meteoschweiz.messwerte-aktuell/VQHA80.csv"
 )
 STATION_URL = "https://data.geo.admin.ch/ch.meteoschweiz.messnetz-automatisch/ch.meteoschweiz.messnetz-automatisch_fr.csv"
@@ -31,14 +39,128 @@
 
 MS_24FORECAST_URL = (
     "https://www.meteosuisse.admin.ch/product/output/forecast-chart/{}/fr/{}00.json"
 )
 MS_24FORECAST_REF = "https://www.meteosuisse.admin.ch//content/meteoswiss/fr/home.mobile.meteo-products--overview.html"
 
 
+class CurrentWeather(TypedDict):
+    time: int
+    icon: int
+    iconV2: int
+    temperature: float
+
+
+class DayForecast(TypedDict):
+    dayDate: str
+    iconDay: int
+    iconDayV2: int
+    temperatureMax: float
+    temperatureMin: float
+    precipitation: float
+
+
+def DayForecast_from_meteoswiss_data(data: dict[str, Any]) -> DayForecast:
+    return DayForecast(
+        dayDate=data["dayDate"],
+        iconDay=int(data["iconDay"]),
+        iconDayV2=int(data["iconDayV2"]),
+        temperatureMax=float(data["temperatureMax"]),
+        temperatureMin=float(data["temperatureMin"]),
+        precipitation=float(data["precipitation"]),
+    )
+
+
+class Forecast(TypedDict):
+    plz: str
+    currentWeather: CurrentWeather
+    regionForecast: list[DayForecast]
+
+
+def Forecast_from_meteoswiss_data(data: dict[str, Any]):
+    return Forecast(
+        plz=data["plz"],
+        currentWeather=data["currentWeather"],
+        regionForecast=[
+            DayForecast_from_meteoswiss_data(x) for x in data["regionForecast"]
+        ],
+    )
+
+
+class CurrentCondition(TypedDict):
+    station: str
+    date: int
+    tre200s0: float | None
+    rre150z0: float | None
+    sre000z0: float | None
+    gre000z0: float | None
+    ure200s0: float | None
+    tde200s0: float | None
+    dkl010z0: float | None
+    fu3010z0: float | None
+    fu3010z1: float | None
+    prestas0: float | None
+    pp0qffs0: float | None
+    pp0qnhs0: float | None
+    ppz850s0: float | None
+    ppz700s0: float | None
+    dv1towz0: float | None
+    fu3towz0: float | None
+    fu3towz1: float | None
+    ta1tows0: float | None
+    uretows0: float | None
+    tdetows0: float | None
+
+
+def CurrentCondition_from_meteoswiss_data(data: dict[str, Any]) -> CurrentCondition:
+    def floatornone(val: Any) -> float | None:
+        if val == "" or val == "-":
+            return None
+        return float(val)
+
+    return CurrentCondition(
+        station=data["Station/Location"],
+        date=int(data["Date"]),
+        tre200s0=floatornone(data["tre200s0"]),
+        rre150z0=floatornone(data["rre150z0"]),
+        sre000z0=floatornone(data["sre000z0"]),
+        gre000z0=floatornone(data["gre000z0"]),
+        ure200s0=floatornone(data["ure200s0"]),
+        tde200s0=floatornone(data["tde200s0"]),
+        dkl010z0=floatornone(data["dkl010z0"]),
+        fu3010z0=floatornone(data["fu3010z0"]),
+        fu3010z1=floatornone(data["fu3010z1"]),
+        prestas0=floatornone(data["prestas0"]),
+        pp0qffs0=floatornone(data["pp0qffs0"]),
+        pp0qnhs0=floatornone(data["pp0qnhs0"]),
+        ppz850s0=floatornone(data["ppz850s0"]),
+        ppz700s0=floatornone(data["ppz700s0"]),
+        dv1towz0=floatornone(data["dv1towz0"]),
+        fu3towz0=floatornone(data["fu3towz0"]),
+        fu3towz1=floatornone(data["fu3towz1"]),
+        ta1tows0=floatornone(data["ta1tows0"]),
+        uretows0=floatornone(data["uretows0"]),
+        tdetows0=floatornone(data["tdetows0"]),
+    )
+
+
+class ClientResult(TypedDict):
+    name: str
+    forecast: list[Forecast]
+    condition: list[CurrentCondition]
+
+
+def ClientResult_from_meteoswiss_data(data: dict[str, Any]) -> ClientResult:
+    return ClientResult(
+        name=data["name"],
+        forecast=Forecast_from_meteoswiss_data(data["forecast"]),
+        condition=[CurrentCondition_from_meteoswiss_data(x) for x in data["condition"]],
+    )
+
+
 class meteoSwissClient:
     def __init__(self, displayName=None, postcode=None, station=None):
         _LOGGER.debug("MS Client INIT")
         self._postCode = postcode
         self._station = station
         self._name = displayName
         self._allStations = None
@@ -54,25 +176,23 @@
         self.get_current_condition()
         return {
             "name": self._name,
             "forecast": self._forecast,
             "condition": self._condition,
         }
 
+    def get_typed_data(self) -> ClientResult:
+        data = self.get_data()
+        return ClientResult_from_meteoswiss_data(data)
+
     def get_24hforecast(self):
         _LOGGER.debug("Start update 24h forecast data")
         s = requests.Session()
         # Forcing headers to avoid 500 error when downloading file
-        s.headers.update(
-            {
-                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
-                "Accept-Encoding": "gzip, deflate, sdch",
-                "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/1337 Safari/537.36",
-            }
-        )
+        s.headers.update(_HEADERS)
         searchUrl = MS_SEARCH_URL.format(self._postCode)
         _LOGGER.debug("Main URL : %s" % searchUrl)
         tmpSearch = s.get(searchUrl, timeout=10)
 
         soup = BeautifulSoup(tmpSearch.text, features="html.parser")
         widgetHtml = soup.find_all("section", {"id": "weather-widget"})
         jsonUrl = widgetHtml[0].get("data-json-url")
@@ -97,21 +217,15 @@
         self._forecast24 = jsonObj
         _LOGGER.debug("End of 24 forecast udate")
 
     def get_forecast(self):
         _LOGGER.debug("Start update forecast data")
         s = requests.Session()
         # Forcing headers to avoid 500 error when downloading file
-        s.headers.update(
-            {
-                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
-                "Accept-Encoding": "gzip, deflate, sdch",
-                "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/1337 Safari/537.36",
-            }
-        )
+        s.headers.update(_HEADERS)
 
         jsonUrl = JSON_FORECAST_URL.format(self._postCode)
         jsonData = s.get(jsonUrl, timeout=10)
         jsonDataTxt = jsonData.text
 
         jsonObj = json.loads(jsonDataTxt)
 
@@ -190,15 +304,15 @@
                 )
             )
             distance = geopy.distance.distance(hPoint, sPoint)
             data += ((distance.km, station_name),)
         data.sort(key=lambda tup: tup[0])
         try:
             return data[0][1]
-        except:
+        except BaseException:
             _LOGGER.warning(
                 "Unable to get closest station for lat : %s lon : %s"
                 % (currentLat, currnetLon)
             )
             return None
 
     def get_station_name(self, stationId):
@@ -211,21 +325,16 @@
             _LOGGER.warning("Unable to find station name for : %s" % (stationId))
             return None
 
     def getGeoData(self, lat, lon):
         s = requests.Session()
         lat = str(lat)
         lon = str(lon)
-        s.headers.update(
-            {
-                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
-                "Accept-Encoding": "gzip, deflate, sdch",
-                "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/1337 Safari/537.36",
-            }
-        )
+        s.headers.update(_HEADERS)
+
         geoData = s.get(
             "https://nominatim.openstreetmap.org/reverse?format=jsonv2&lat="
             + lat
             + "&lon="
             + lon
             + "&zoom=18"
         ).text
```

### Comparing `hamsclientfork-0.2.7/hamsclientfork.egg-info/PKG-INFO` & `hamsclientfork-0.2.8/hamsclientfork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamsclientfork
-Version: 0.2.7
+Version: 0.2.8
 Summary: Library to get data from meteo swiss
 Home-page: https://github.com/Rudd-O/hamsclientfork
 Author: websylv
 Author-email: div@webhu.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hamsclientfork-0.2.7/setup.py` & `hamsclientfork-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     text_type = type("")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="hamsclientfork",
-    version="0.2.7",
+    version="0.2.8",
     url="https://github.com/Rudd-O/hamsclientfork",
     license="MIT",
     author="websylv",
     author_email="div@webhu.org",
     description="Library to get data from meteo swiss",
     long_description=read("README.rst"),
     packages=find_packages(exclude=("tests",)),
```

