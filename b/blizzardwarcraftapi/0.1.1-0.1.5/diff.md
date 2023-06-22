# Comparing `tmp/BlizzardWarcraftAPI-0.1.1.tar.gz` & `tmp/blizzardwarcraftapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlizzardWarcraftAPI-0.1.1.tar", last modified: Sun Jun 18 11:43:46 2023, max compression
+gzip compressed data, was "blizzardwarcraftapi-0.1.5.tar", max compression
```

## Comparing `BlizzardWarcraftAPI-0.1.1.tar` & `blizzardwarcraftapi-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/BlizzardAuthToken.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/AchievementAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/AuctionHouseAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/CharacterAchievementsAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/CharacterAppearanceAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/ConnectedRealmAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/tests/test_base.py
+-rw-r--r--   0        0        0     1003 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/BlizzardAuthToken.py
+-rw-r--r--   0        0        0      805 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
+-rw-r--r--   0        0        0      139 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/__init__.py
+-rw-r--r--   0        0        0      609 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/data.py
+-rw-r--r--   0        0        0      292 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/exceptions.py
+-rw-r--r--   0        0        0     1935 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
+-rw-r--r--   0        0        0      639 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/__init__.py
+-rw-r--r--   0        0        0     2195 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py
+-rw-r--r--   0        0        0     1694 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py
+-rw-r--r--   0        0        0     2056 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/__init__.py
+-rw-r--r--   0        0        0     1271 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py
+-rw-r--r--   0        0        0      683 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py
+-rw-r--r--   0        0        0     2965 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py
+-rw-r--r--   0        0        0     1766 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py
+-rw-r--r--   0        0        0      670 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py
+-rw-r--r--   0        0        0      746 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/urls.py
+-rw-r--r--   0        0        0     1066 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2257 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/README.md
+-rw-r--r--   0        0        0      916 2023-06-22 14:37:33.409385 blizzardwarcraftapi-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 blizzardwarcraftapi-0.1.5/PKG-INFO
```

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/BlizzardAuthToken.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/BlizzardAuthToken.py`

 * *Files identical despite different names*

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from .modules import \
-    AchievementAPI, AuctionHouseAPI, \
-    ConnectedRealmAPI, CharacterAchievementsAPI, \
-    CharacterAppearanceAPI
+from .modules import *
 
 
 class BlizzardWarcraftAPI(AuctionHouseAPI, AchievementAPI,
                           ConnectedRealmAPI, CharacterAchievementsAPI,
-                          CharacterAppearanceAPI):
+                          CharacterAppearanceAPI, CharacterCollectionsAPI,
+                          CharacterEncountersAPI, CharacterEquipmentAPI,
+                          CharacterHunterPetsAPI):
     """
     Use BlizzardAuthToken class for generate access token.
 
     :param str BlizzardAuthToken: Access token.
     :param str region: The region of the data to retrieve.
     :param locale: The locale to reflect in localized data.
```

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/data.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/data.py`

 * *Files identical despite different names*

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/AchievementAPI.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from .BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
+from BlizzardWarcraftAPI.modules.BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
 
 
 class AchievementAPI(BlizzardWarcraftAPI):
 
     def get_AchievementCategoriesIndex(self) -> dict:
         """
         :return: an index of achievement categories.
```

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/AuctionHouseAPI.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
+from BlizzardWarcraftAPI.modules.BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
 
 
 class AuctionHouseAPI(BlizzardWarcraftAPI):
 
     def get_Auctions(self, connectedRealmId) -> dict:
         """
         See the Connected Realm API for information about retrieving a list of connected realm IDs.
```

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py`

 * *Files identical despite different names*

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/CharacterAchievementsAPI.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
+from BlizzardWarcraftAPI.modules.BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
 
 
 class CharacterAchievementsAPI(BlizzardWarcraftAPI):
 
     def get_CharacterAchievementsSummary(self, realmSlug: str, characterName: str) -> dict:
         """
         :param realmSlug: The slug of the realm.
```

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/CharacterAppearanceAPI.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
+from BlizzardWarcraftAPI.modules.BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
 
 
-class CharacterAppearanceAPI(BlizzardWarcraftAPI):
+class CharacterEquipmentAPI(BlizzardWarcraftAPI):
 
-    def get_CharacterAppearanceSummary(self, realmSlug: str, characterName: str) -> dict:
+    def get_CharacterEquipmentSummary(self, realmSlug, characterName) -> dict:
         """
         :param realmSlug: The slug of the realm.
         :param characterName: The lowercase name of the character.
 
-        :return: Returns a summary of a character's appearance settings.
+        :return: Returns a summary of the items equipped by a character.
         :rtype: dict
         """
-        url = f"https://{self.region}.api.blizzard.com/profile/wow/character/{realmSlug}/{characterName}/appearance"
+        url = f"https://{self.region}.api.blizzard.com/profile/wow/character/{realmSlug}/{characterName}/equipment"
         self.param["namespace"] = self.namespace_profile
         return self.response(url, self.param)
```

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/ConnectedRealmAPI.py` & `blizzardwarcraftapi-0.1.5/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
+from BlizzardWarcraftAPI.modules.BlizzardWarcraftAPI_base import BlizzardWarcraftAPI
 
 
 class ConnectedRealmAPI(BlizzardWarcraftAPI):
 
     def get_ConnectedRealmsIndex(self) -> dict:
         """
         :return: Returns an index of connected realms.
```

### Comparing `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/PKG-INFO` & `blizzardwarcraftapi-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: BlizzardWarcraftAPI
-Version: 0.1.1
-Summary: Warcraft API
-Author-email: Angeloffy <angeloffy.work@gmail.com>
-Project-URL: Homepage, https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/main
-Project-URL: Bug Tracker, https://github.com/Angeloffy/BlizzardWarcraftAPI/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BlizzardWarcraftAPI
 
 ![image](https://drive.google.com/uc?export=view&id=1bwLWgLTIHPy23sTfufMNV9NHhvQ4vQ1y)
 
 BlizzardWarcraftAPI is a Python library designed to interact with the official World of Warcraft API provided by <a href="https://develop.battle.net/documentation/world-of-warcraft">Blizzard</a>. Although it is still a work in progress, active development is underway. It's important to note that this library is not an official Blizzard product, but rather the result of an independent developer's efforts.
 
 BlizzardWarcraftAPI aims to provide a convenient and user-friendly interface for developers to access and utilize the wealth of data available through the World of Warcraft API. With this library, you can retrieve information about characters, items, quests, guilds, and more. It abstracts away the complexities of making API requests and handling responses, allowing developers to focus on building their applications or tools.
@@ -47,7 +33,11 @@
 - [x] Auction House
 - [x] Connected Realm
 
 ## [Profile](https://develop.battle.net/documentation/world-of-warcraft/profile-apis)
 
 - [x] Character Achievements
 - [x] Character Appearance
+- [x] Character Collections
+- [x] Character Encounters
+- [x] Character Equipment
+- [x] Character Hunter Pets
```

#### html2text {}

```diff
@@ -1,35 +1,29 @@
-Metadata-Version: 2.1 Name: BlizzardWarcraftAPI Version: 0.1.1 Summary:
-Warcraft API Author-email: Angeloffy
-work@gmail.com> Project-URL: Homepage, https://github.com/Angeloffy/
-BlizzardWarcraftAPI/tree/main Project-URL: Bug Tracker, https://github.com/
-Angeloffy/BlizzardWarcraftAPI/issues Classifier: Programming Language :: Python
-:: 3.9 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
-markdown License-File: LICENSE # BlizzardWarcraftAPI ![image](https://
-drive.google.com/uc?export=view&id=1bwLWgLTIHPy23sTfufMNV9NHhvQ4vQ1y)
-BlizzardWarcraftAPI is a Python library designed to interact with the official
-World of Warcraft API provided by Blizzard. Although it is still a work in
-progress, active development is underway. It's important to note that this
-library is not an official Blizzard product, but rather the result of an
-independent developer's efforts. BlizzardWarcraftAPI aims to provide a
-convenient and user-friendly interface for developers to access and utilize the
-wealth of data available through the World of Warcraft API. With this library,
-you can retrieve information about characters, items, quests, guilds, and more.
-It abstracts away the complexities of making API requests and handling
-responses, allowing developers to focus on building their applications or
-tools. By leveraging Blizzard's official API, BlizzardWarcraftAPI ensures that
-the data obtained is accurate and up-to-date. As the library continues to
-evolve, additional features and enhancements will be added to expand its
-capabilities and improve its usability. Developers interested in utilizing the
-vast resources offered by the World of Warcraft API will find
-BlizzardWarcraftAPI to be a valuable tool in their projects. # Installing
-Install and update using pip: ```shell pip install BlizzardWarcraftAPI ``` # A
-Simple Example ```python from BlizzardWarcraftAPI import BlizzardWarcraftAPI,
-BlizzardAuthToken token = BlizzardAuthToken("ClientID", "ClientSecret").get()
-warcraft = BlizzardWarcraftAPI(token, region, locale)
+# BlizzardWarcraftAPI ![image](https://drive.google.com/
+uc?export=view&id=1bwLWgLTIHPy23sTfufMNV9NHhvQ4vQ1y) BlizzardWarcraftAPI is a
+Python library designed to interact with the official World of Warcraft API
+provided by Blizzard. Although it is still a work in progress, active
+development is underway. It's important to note that this library is not an
+official Blizzard product, but rather the result of an independent developer's
+efforts. BlizzardWarcraftAPI aims to provide a convenient and user-friendly
+interface for developers to access and utilize the wealth of data available
+through the World of Warcraft API. With this library, you can retrieve
+information about characters, items, quests, guilds, and more. It abstracts
+away the complexities of making API requests and handling responses, allowing
+developers to focus on building their applications or tools. By leveraging
+Blizzard's official API, BlizzardWarcraftAPI ensures that the data obtained is
+accurate and up-to-date. As the library continues to evolve, additional
+features and enhancements will be added to expand its capabilities and improve
+its usability. Developers interested in utilizing the vast resources offered by
+the World of Warcraft API will find BlizzardWarcraftAPI to be a valuable tool
+in their projects. # Installing Install and update using pip: ```shell pip
+install BlizzardWarcraftAPI ``` # A Simple Example ```python from
+BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken token =
+BlizzardAuthToken("ClientID", "ClientSecret").get() warcraft =
+BlizzardWarcraftAPI(token, region, locale)
 warcraft.get_AchievementCategoriesIndex ``` # [APIs](https://
 develop.battle.net/documentation/world-of-warcraft) ## [Game Data](https://
 develop.battle.net/documentation/world-of-warcraft/game-data-apis) - [x]
 Achievement - [x] Auction House - [x] Connected Realm ## [Profile](https://
 develop.battle.net/documentation/world-of-warcraft/profile-apis) - [x]
-Character Achievements - [x] Character Appearance
+Character Achievements - [x] Character Appearance - [x] Character Collections -
+[x] Character Encounters - [x] Character Equipment - [x] Character Hunter Pets
```

### Comparing `BlizzardWarcraftAPI-0.1.1/LICENSE` & `blizzardwarcraftapi-0.1.5/LICENSE`

 * *Files identical despite different names*

