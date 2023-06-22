# Comparing `tmp/dronefly_core-0.3.6.dev4.tar.gz` & `tmp/dronefly_core-0.3.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.6.dev4.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.6.dev5.tar", max compression
```

## Comparing `dronefly_core-0.3.6.dev4.tar` & `dronefly_core-0.3.6.dev5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev4/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev4/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev4/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev4/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev4/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     7991 2023-06-18 15:08:05.888074 dronefly_core-0.3.6.dev4/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev4/dronefly/core/constants.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev4/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev4/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0    34585 2023-06-18 15:07:29.087299 dronefly_core-0.3.6.dev4/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev4/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev4/dronefly/core/models/controlled_terms.py
--rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev4/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev4/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev4/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev4/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev4/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev4/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev4/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev4/dronefly/core/query/query.py
--rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev4/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-06-19 16:29:59.863532 dronefly_core-0.3.6.dev4/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev4/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev4/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev5/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev5/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev5/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev5/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev5/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0     8043 2023-06-22 17:27:01.514036 dronefly_core-0.3.6.dev5/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev5/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev5/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev5/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    35801 2023-06-22 17:32:04.480260 dronefly_core-0.3.6.dev5/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev5/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev5/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev5/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev5/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev5/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev5/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev5/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev5/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev5/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev5/dronefly/core/query/query.py
+-rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev5/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-22 17:38:46.644562 dronefly_core-0.3.6.dev5/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev5/setup.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev5/PKG-INFO
```

### Comparing `dronefly_core-0.3.6.dev4/LICENSE` & `dronefly_core-0.3.6.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/README.md` & `dronefly_core-0.3.6.dev5/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/clients/inat.py` & `dronefly_core-0.3.6.dev5/dronefly/core/clients/inat.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/commands/__init__.py` & `dronefly_core-0.3.6.dev5/dronefly/core/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,17 @@
             query_response = QueryResponse(**query_args)
             obs_args = query_response.obs_args()
             life_list = client.observations.life_list(**obs_args)
 
         if not life_list:
             return f"No life list {query_response.obs_query_description()}"
 
-        formatter = LifeListFormatter(life_list, per_rank, query_response)
+        formatter = LifeListFormatter(
+            life_list, per_rank, query_response, with_taxa=True, max_taxa=100
+        )
         return self._format_markdown(formatter)
 
     def taxon(self, ctx: Context, *args):
         query = self._parse(" ".join(args))
         # TODO: Handle all query clauses, not just main.terms
         # TODO: Doesn't do any ranking or filtering of results
         if not query.main or not query.main.terms:
```

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/constants.py` & `dronefly_core-0.3.6.dev5/dronefly/core/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/formatters/generic.py` & `dronefly_core-0.3.6.dev5/dronefly/core/formatters/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 Anything more complicated than plain text can be rendered in Markdown,
 which is then fairly easy to render to other formats as needed.
 """
 from __future__ import annotations
 import copy
 from datetime import datetime as dt
 import re
-from typing import List, TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from dronefly.core.query.query import QueryResponse
 
 import html2markdown
 import inflect
 from pyinaturalist import (
     ConservationStatus,
     EstablishmentMeans,
     JsonResponse,
     LifeList,
+    LifeListTaxon,
     ListedTaxon,
     Observation,
     Taxon,
     TaxonSummary,
     User,
 )
 from pyinaturalist.constants import COMMON_RANKS
@@ -140,15 +141,15 @@
             formatted_time = f"{mon}-{year}"
     else:
         wday = time.strftime("%a")
         formatted_time = f"{wday} {mon} {day}, {year} · {hour}:{minute} {am_pm}"
     return formatted_time
 
 
-def format_life_list_summary(life_list: LifeList, per_rank: str, taxon: Taxon):
+def filter_life_list(life_list: LifeList, per_rank: str, taxon: Taxon):
     ranks = None
     rank_totals = {}
     if per_rank in ["main", "any"]:
         ranks_to_count = (
             COMMON_RANKS[-8:] if per_rank == "main" else list(RANK_LEVELS.keys())
         )
         if taxon:
@@ -186,14 +187,20 @@
         rank = RANK_EQUIVALENTS[per_rank] if per_rank in RANK_EQUIVALENTS else per_rank
         ranks = p.plural_noun(rank)
         taxa = [
             life_list_taxon
             for life_list_taxon in life_list.data
             if life_list_taxon.rank == rank
         ]
+    return (taxa, ranks, rank_totals)
+
+
+def format_life_list_summary(
+    taxa: list[LifeListTaxon], ranks: str, rank_totals: list[int]
+):
     total = f"Total: {len(taxa)} {ranks}"
     if rank_totals:
         rank_keys = reversed(
             [rank for rank in RANK_LEVELS.keys() if rank != "stateofmatter"]
         )
         rank_totals_by_rank = [
             rank_totals[rank] for rank in rank_keys if rank_totals.get(rank)
@@ -310,26 +317,26 @@
         linked_status = format_link(status.authority, status.url)
         full_description = f"{description} ({linked_status})"
 
     return full_description
 
 
 def format_taxon_names(
-    taxa: List[Taxon],
+    taxa: list[Taxon],
     with_term=False,
     names_format="%s",
     max_len=0,
     hierarchy=False,
     lang=None,
 ):
     """Format names of taxa from matched records.
 
     Parameters
     ----------
-    taxa: List[Taxon]
+    taxa: list[Taxon]
         A list of Taxon records to format, either as a comma-delimited list or
         in a hierarchy.
         - If hierarchy=True, these must be in highest to lowest rank order.
     with_term: bool, optional
         With non-common / non-name matching term in parentheses in place of common name.
     names_format: str, optional
         Format string for the name. Must contain exactly one %s.
@@ -536,71 +543,95 @@
 class LifeListFormatter(BaseFormatter):
     def __init__(
         self,
         life_list: LifeList,
         per_rank: str,
         query_response: QueryResponse,
         with_url: bool = True,
+        with_taxa: bool = False,
         max_len: int = 0,
+        max_taxa: int = 20,
     ):
         """
         Parameters
         ----------
         taxon: Taxon
             The taxon to format.
 
         with_url: bool, optional
             When True, link the name to taxon.url.
         """
         self.life_list = life_list
         self.per_rank = per_rank
         self.query_response = query_response
         self.with_url = with_url
+        self.with_taxa = with_taxa
         self.max_len = max_len
+        self.max_taxa = max_taxa
 
     def format(self, with_title: bool = True):
         """Format the life list as markdown."""
         description = self.format_description()
         if with_title:
             description = "\n\n".join([self.format_title(), description])
         return description
 
     def format_title(self):
         """Format life list title as Discord-like markdown.
 
         Returns
         -------
         str
-            Like format_name(), except:
-
-            - Append the matching term in its own parentheses after the common name
-            in parentheses if the matching term is neither the scientific name nor
-            common name, e.g.
-            - "Pissenlits" -> "Genus *Taraxacum* (dandelions) (Pissenlits)"
-            - if with_url=True, the matched term is not included in the link
-            - Apply strikethrough style if the name is invalid, e.g.
-            - "Picoides pubescens" ->
-                "*Dryobates Pubescens* (Downy woodpecker) (~~Picoides Pubescens~~)
+            - Describe the life list in terms of the observations query
+              parameters passed.
+            - Only link to the life list when the query is for one user.
+              The website doesn't support life lists for any other kind of
+              query.
         """
         title = f"Life list {self.query_response.obs_query_description()}"
         if self.with_url:
             if self.query_response.user:
                 url = lifelists_url_from_query_response(self.query_response)
-            else:
-                url = obs_url_from_v1(
-                    {**self.query_response.obs_args(), "view": "species"}
-                )
-            title = format_link(title, url)
+                title = format_link(title, url)
         return title
 
     def format_description(self):
         """Format the life list description."""
-        return format_life_list_summary(
+        description = []
+        (taxa, ranks, rank_totals) = filter_life_list(
             self.life_list, self.per_rank, self.query_response.taxon
         )
+        query_response = self.query_response
+        obs_link = format_link(
+            "All Life List Observations",
+            obs_url_from_v1(query_response.obs_args()),
+        )
+        description.append(obs_link)
+        # TODO: if more than max_taxa, support paged result
+        if self.with_taxa and len(taxa) <= self.max_taxa:
+            max_digits = len(str(max([taxon.descendant_obs_count for taxon in taxa])))
+            formatted_taxa = []
+            obs_args = query_response.obs_args()
+            for taxon in taxa:
+                # Replace any taxa in the original query with just the one:
+                if "taxon_ids" in obs_args:
+                    del obs_args["taxon_ids"]
+                taxon_obs_url = obs_url_from_v1(
+                    {
+                        **obs_args,
+                        "taxon_id": taxon.id,
+                    }
+                )
+                formatted_count = str(taxon.descendant_obs_count).rjust(max_digits)
+                formatted_name = format_link(taxon.name, taxon_obs_url)
+                formatted_taxa.append(f"`{formatted_count}` {formatted_name}")
+            description.append("\n".join(formatted_taxa))
+        life_list_summary = format_life_list_summary(taxa, ranks, rank_totals)
+        description.append(life_list_summary)
+        return "\n\n".join(description)
 
 
 class TaxonFormatter(BaseFormatter):
     def __init__(
         self,
         taxon: Taxon,
         lang: str = None,
```

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/models/controlled_terms.py` & `dronefly_core-0.3.6.dev5/dronefly/core/models/controlled_terms.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.6.dev5/dronefly/core/parsers/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.6.dev5/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.6.dev5/dronefly/core/parsers/unixlike.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/parsers/url.py` & `dronefly_core-0.3.6.dev5/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/query/query.py` & `dronefly_core-0.3.6.dev5/dronefly/core/query/query.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/dronefly/core/utils/__init__.py` & `dronefly_core-0.3.6.dev5/dronefly/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev4/pyproject.toml` & `dronefly_core-0.3.6.dev5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 exclude_dirs = ["tests"]
 
 [tool.flake8]
 max-line-length = 100
 
 [tool.poetry]
 name = "dronefly-core"
-version = "0.3.6.dev4"
+version = "0.3.6.dev5"
 description = "Core dronefly components"
 authors = ["Ben Armstrong <synrg@debian.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
 	{ include = "dronefly/core" },
 ]
```

### Comparing `dronefly_core-0.3.6.dev4/setup.py` & `dronefly_core-0.3.6.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'html2markdown>=0.1.7,<0.2.0',
  'inflect>=5.3.0,<6.0.0',
  'pyinaturalist>=0.19.0.dev2,<0.20',
  'rich>=10.9,<14']
 
 setup_kwargs = {
     'name': 'dronefly-core',
-    'version': '0.3.6.dev4',
+    'version': '0.3.6.dev5',
     'description': 'Core dronefly components',
     'long_description': "# Dronefly core\n\nThis is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)\nDiscord bot's core components. We're not yet making version guarantees until\nit is more usable.\n\n# Related packages\n\n## Dronefly command-line client\n\nThe [dronefly-cli](https://github.com/dronefly-garden/dronefly-cli) command-line\nclient will provide a standalone text user interface that can perform a usable\nsubset of Dronefly Discord bot's capabilities, built solely with Dronefly core.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_core-0.3.6.dev4/PKG-INFO` & `dronefly_core-0.3.6.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.6.dev4
+Version: 0.3.6.dev5
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

