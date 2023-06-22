# Comparing `tmp/polyfactory-2.3.2.tar.gz` & `tmp/polyfactory-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.3.2.tar", max compression
+gzip compressed data, was "polyfactory-2.3.3.tar", max compression
```

## Comparing `polyfactory-2.3.2.tar` & `polyfactory-2.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1092 2023-06-18 19:05:35.362617 polyfactory-2.3.2/LICENSE
--rw-r--r--   0        0        0     9446 2023-06-18 19:05:35.362617 polyfactory-2.3.2/README.md
--rw-r--r--   0        0        0      425 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/__init__.py
--rw-r--r--   0        0        0      825 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    32143 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1876 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     6873 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2217 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    10876 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1516 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     7410 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3329 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/py.typed
--rw-r--r--   0        0        0     2891 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3402 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     2834 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1880 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13607 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      522 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      529 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      535 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3636 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6186 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6257 2023-06-18 19:05:35.366617 polyfactory-2.3.2/pyproject.toml
--rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 polyfactory-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-22 17:17:07.017234 polyfactory-2.3.3/LICENSE
+-rw-r--r--   0        0        0     9785 2023-06-22 17:17:07.021234 polyfactory-2.3.3/README.md
+-rw-r--r--   0        0        0      425 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/__init__.py
+-rw-r--r--   0        0        0      825 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    32614 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1897 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2392 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2217 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    11309 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1598 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     8033 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3329 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/py.typed
+-rw-r--r--   0        0        0     2891 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3488 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1880 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13607 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      522 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      529 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      535 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3636 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6186 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6560 2023-06-22 17:17:07.025234 polyfactory-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0    11707 1970-01-01 00:00:00.000000 polyfactory-2.3.3/PKG-INFO
```

### Comparing `polyfactory-2.3.2/LICENSE` & `polyfactory-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/README.md` & `polyfactory-2.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 
-[![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-9-orange.svg?style=flat-square)](#contributors-)
 
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 <!-- markdownlint-restore -->
 
 Polyfactory is a simple and powerful mock data generation library, based around type
@@ -112,14 +112,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/guacs"><img src="https://avatars.githubusercontent.com/u/126393040?v=4?s=100" width="100px;" alt="guacs"/><br /><sub><b>guacs</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=guacs" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/VSHUMILIN97"><img src="https://avatars.githubusercontent.com/u/27234763?v=4?s=100" width="100px;" alt="Vadim"/><br /><sub><b>Vadim</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=VSHUMILIN97" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `polyfactory-2.3.2/polyfactory/constants.py` & `polyfactory-2.3.3/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/decorators.py` & `polyfactory-2.3.3/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/exceptions.py` & `polyfactory-2.3.3/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/factories/base.py` & `polyfactory-2.3.3/polyfactory/factories/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,104 +521,108 @@
                 (*(bases or ()), cls),
                 {"__model__": model, **kwargs},
             ),
         )
 
     @classmethod
     def get_constrained_field_value(cls, annotation: Any, field_meta: FieldMeta) -> Any:
-        constraints = cast("Constraints", field_meta.constraints)
-        if is_safe_subclass(annotation, float):
-            return handle_constrained_float(
-                random=cls.__random__,
-                multiple_of=cast("Any", constraints.get("multiple_of")),
-                gt=cast("Any", constraints.get("gt")),
-                ge=cast("Any", constraints.get("ge")),
-                lt=cast("Any", constraints.get("lt")),
-                le=cast("Any", constraints.get("le")),
-            )
-
-        if is_safe_subclass(annotation, int):
-            return handle_constrained_int(
-                random=cls.__random__,
-                multiple_of=cast("Any", constraints.get("multiple_of")),
-                gt=cast("Any", constraints.get("gt")),
-                ge=cast("Any", constraints.get("ge")),
-                lt=cast("Any", constraints.get("lt")),
-                le=cast("Any", constraints.get("le")),
-            )
-
-        if is_safe_subclass(annotation, Decimal):
-            return handle_constrained_decimal(
-                random=cls.__random__,
-                decimal_places=cast("Any", constraints.get("decimal_places")),
-                max_digits=cast("Any", constraints.get("max_digits")),
-                multiple_of=cast("Any", constraints.get("multiple_of")),
-                gt=cast("Any", constraints.get("gt")),
-                ge=cast("Any", constraints.get("ge")),
-                lt=cast("Any", constraints.get("lt")),
-                le=cast("Any", constraints.get("le")),
-            )
-
-        if url_constraints := constraints.get("url"):
-            return handle_constrained_url(constraints=url_constraints)
-
-        if is_safe_subclass(annotation, str) or is_safe_subclass(annotation, bytes):
-            return handle_constrained_string_or_bytes(
-                random=cls.__random__,
-                t_type=str if is_safe_subclass(annotation, str) else bytes,
-                lower_case=constraints.get("lower_case") or False,
-                upper_case=constraints.get("upper_case") or False,
-                min_length=constraints.get("min_length"),
-                max_length=constraints.get("max_length"),
-                pattern=constraints.get("pattern"),
-            )
-
-        if (
-            is_safe_subclass(annotation, set)
-            or is_safe_subclass(annotation, list)
-            or is_safe_subclass(annotation, frozenset)
-            or is_safe_subclass(annotation, tuple)
-        ):
-            collection_type: type[list] | type[set] | type[tuple] | type[frozenset]
-            if is_safe_subclass(annotation, list):
-                collection_type = list
-            elif is_safe_subclass(annotation, set):
-                collection_type = set
-            elif is_safe_subclass(annotation, tuple):
-                collection_type = tuple
-            else:
-                collection_type = frozenset
-
-            return handle_constrained_collection(
-                collection_type=collection_type,  # type: ignore
-                factory=cls,
-                field_meta=field_meta.children[0] if field_meta.children else field_meta,
-                item_type=constraints.get("item_type"),
-                max_items=constraints.get("max_length"),
-                min_items=constraints.get("min_length"),
-                unique_items=constraints.get("unique_items", False),
-            )
-
-        if is_safe_subclass(annotation, date):
-            return handle_constrained_date(
-                faker=cls.__faker__,
-                ge=cast("Any", constraints.get("ge")),
-                gt=cast("Any", constraints.get("gt")),
-                le=cast("Any", constraints.get("le")),
-                lt=cast("Any", constraints.get("lt")),
-            )
-
-        if is_safe_subclass(annotation, UUID) and (uuid_version := constraints.get("uuid_version")):
-            return handle_constrained_uuid(
-                uuid_version=uuid_version,
-                faker=cls.__faker__,
-            )
-
-        if is_safe_subclass(annotation, Path) and (path_constraint := constraints.get("path_type")):
-            return handle_constrained_path(constraint=path_constraint, faker=cls.__faker__)
+        try:
+            constraints = cast("Constraints", field_meta.constraints)
+            if is_safe_subclass(annotation, float):
+                return handle_constrained_float(
+                    random=cls.__random__,
+                    multiple_of=cast("Any", constraints.get("multiple_of")),
+                    gt=cast("Any", constraints.get("gt")),
+                    ge=cast("Any", constraints.get("ge")),
+                    lt=cast("Any", constraints.get("lt")),
+                    le=cast("Any", constraints.get("le")),
+                )
+
+            if is_safe_subclass(annotation, int):
+                return handle_constrained_int(
+                    random=cls.__random__,
+                    multiple_of=cast("Any", constraints.get("multiple_of")),
+                    gt=cast("Any", constraints.get("gt")),
+                    ge=cast("Any", constraints.get("ge")),
+                    lt=cast("Any", constraints.get("lt")),
+                    le=cast("Any", constraints.get("le")),
+                )
+
+            if is_safe_subclass(annotation, Decimal):
+                return handle_constrained_decimal(
+                    random=cls.__random__,
+                    decimal_places=cast("Any", constraints.get("decimal_places")),
+                    max_digits=cast("Any", constraints.get("max_digits")),
+                    multiple_of=cast("Any", constraints.get("multiple_of")),
+                    gt=cast("Any", constraints.get("gt")),
+                    ge=cast("Any", constraints.get("ge")),
+                    lt=cast("Any", constraints.get("lt")),
+                    le=cast("Any", constraints.get("le")),
+                )
+
+            if url_constraints := constraints.get("url"):
+                return handle_constrained_url(constraints=url_constraints)
+
+            if is_safe_subclass(annotation, str) or is_safe_subclass(annotation, bytes):
+                return handle_constrained_string_or_bytes(
+                    random=cls.__random__,
+                    t_type=str if is_safe_subclass(annotation, str) else bytes,
+                    lower_case=constraints.get("lower_case") or False,
+                    upper_case=constraints.get("upper_case") or False,
+                    min_length=constraints.get("min_length"),
+                    max_length=constraints.get("max_length"),
+                    pattern=constraints.get("pattern"),
+                )
+
+            if (
+                is_safe_subclass(annotation, set)
+                or is_safe_subclass(annotation, list)
+                or is_safe_subclass(annotation, frozenset)
+                or is_safe_subclass(annotation, tuple)
+            ):
+                collection_type: type[list] | type[set] | type[tuple] | type[frozenset]
+                if is_safe_subclass(annotation, list):
+                    collection_type = list
+                elif is_safe_subclass(annotation, set):
+                    collection_type = set
+                elif is_safe_subclass(annotation, tuple):
+                    collection_type = tuple
+                else:
+                    collection_type = frozenset
+
+                return handle_constrained_collection(
+                    collection_type=collection_type,  # type: ignore
+                    factory=cls,
+                    field_meta=field_meta.children[0] if field_meta.children else field_meta,
+                    item_type=constraints.get("item_type"),
+                    max_items=constraints.get("max_length"),
+                    min_items=constraints.get("min_length"),
+                    unique_items=constraints.get("unique_items", False),
+                )
+
+            if is_safe_subclass(annotation, date):
+                return handle_constrained_date(
+                    faker=cls.__faker__,
+                    ge=cast("Any", constraints.get("ge")),
+                    gt=cast("Any", constraints.get("gt")),
+                    le=cast("Any", constraints.get("le")),
+                    lt=cast("Any", constraints.get("lt")),
+                    tz=cast("Any", constraints.get("tz")),
+                )
+
+            if is_safe_subclass(annotation, UUID) and (uuid_version := constraints.get("uuid_version")):
+                return handle_constrained_uuid(
+                    uuid_version=uuid_version,
+                    faker=cls.__faker__,
+                )
+
+            if is_safe_subclass(annotation, Path) and (path_constraint := constraints.get("path_type")):
+                return handle_constrained_path(constraint=path_constraint, faker=cls.__faker__)
+        except TypeError as e:
+            raise ParameterException from e
 
         raise ParameterException(f"received constraints for unsupported type {annotation}")
 
     @classmethod
     def get_field_value(cls, field_meta: FieldMeta, field_build_parameters: Any | None = None) -> Any:
         """Return a field value on the subclass if existing, otherwise returns a mock value.
```

### Comparing `polyfactory-2.3.2/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.3.3/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.3.3/polyfactory/factories/dataclass_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
         :returns: A list of field MetaData instances.
 
         """
         fields_meta: list["FieldMeta"] = []
 
-        model_type_hints = get_type_hints(cls.__model__)
+        model_type_hints = get_type_hints(cls.__model__, include_extras=True)
 
         for field in fields(cls.__model__):  # type: ignore[arg-type]
             if field.default_factory and field.default_factory is not MISSING:
                 default_value = field.default_factory()
             elif field.default is not MISSING:
                 default_value = field.default
             else:
```

### Comparing `polyfactory-2.3.2/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.3.3/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.3.3/polyfactory/factories/pydantic_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     TypeVar,
     cast,
 )
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import Constraints, FieldMeta, Null
-from polyfactory.utils.helpers import unwrap_new_type
+from polyfactory.utils.helpers import unwrap_new_type, unwrap_optional
+from polyfactory.utils.predicates import is_optional_union
 
 try:
     from pydantic import BaseModel
 
 except ImportError as e:
     raise MissingDependencyException("pydantic is not installed") from e
 
@@ -81,14 +82,21 @@
         else:
             default_value = field_info.default if field_info.default is not Undefined else Null
 
         name = field_info.alias if field_info.alias and use_alias else field_name
 
         annotation = unwrap_new_type(field_info.annotation)
 
+        if is_optional_union(field_info.annotation):
+            # pydantic v2 do not propagate metadata for Union types #[?]
+            # hence we cannot acquire any constraints w/ straightforward approach
+            from pydantic.fields import FieldInfo
+
+            field_info = FieldInfo.from_annotation(unwrap_optional(annotation))
+
         if metadata := [v for v in field_info.metadata if v is not None]:
             constraints = cls.parse_constraints(metadata=metadata)
         else:
             constraints = {}
 
         if "url" in constraints:
             # pydantic uses a sentinel value for url constraints
@@ -162,15 +170,15 @@
                 "upper_case": getattr(outer_type, "to_upper", None),
                 "lower_case": getattr(outer_type, "to_lower", None),
                 "item_type": getattr(outer_type, "item_type", None),
             },
         )
 
         # pydantic v1 has constraints set for these values, but we generate them using faker
-        if annotation in (AnyUrl, HttpUrl, KafkaDsn, PostgresDsn, RedisDsn, AmqpDsn, AnyHttpUrl):
+        if unwrap_optional(annotation) in (AnyUrl, HttpUrl, KafkaDsn, PostgresDsn, RedisDsn, AmqpDsn, AnyHttpUrl):
             constraints = {}
 
         children: list[FieldMeta] = []
         if model_field.key_field:
             children.append(PydanticFieldMeta.from_model_field(model_field.key_field, use_alias))
         if model_field.sub_fields:
             children.extend(
```

### Comparing `polyfactory-2.3.2/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.3.3/polyfactory/factories/typed_dict_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Generic, TypeVar
 
-from typing_extensions import TypeGuard, _TypedDictMeta, is_typeddict  # type: ignore[attr-defined]
+from typing_extensions import TypeGuard, _TypedDictMeta, get_type_hints, is_typeddict  # type: ignore[attr-defined]
 
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import FieldMeta, Null
 
 TypedDictT = TypeVar("TypedDictT", bound=_TypedDictMeta)
 
 
@@ -33,15 +33,17 @@
 
 
         :returns: A list of field MetaData instances.
 
         """
         fields_meta: list["FieldMeta"] = []
 
-        for field_name, annotation in cls.__model__.__annotations__.items():
+        model_type_hints = get_type_hints(cls.__model__, include_extras=True)
+
+        for field_name, annotation in model_type_hints.items():
             fields_meta.append(
                 FieldMeta.from_type(
                     annotation=annotation,
                     random=cls.__random__,
                     name=field_name,
                     default=getattr(cls.__model__, field_name, Null),
                 )
```

### Comparing `polyfactory-2.3.2/polyfactory/field_meta.py` & `polyfactory-2.3.3/polyfactory/field_meta.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, Any, Literal, Pattern, TypedDict, cast
 
 from polyfactory.constants import DEFAULT_RANDOM, IGNORED_TYPE_ARGS, TYPE_MAPPING
 from polyfactory.utils.helpers import normalize_annotation, unwrap_annotated, unwrap_args, unwrap_new_type
 from polyfactory.utils.predicates import is_annotated
 
 if TYPE_CHECKING:
+    import datetime
     from random import Random
 
     from _pydecimal import Decimal
     from typing_extensions import NotRequired, Self
 
 
 class Null:
@@ -25,28 +26,31 @@
     default_port: NotRequired[int]
     default_path: NotRequired[str]
 
 
 class Constraints(TypedDict):
     """Metadata regarding a type constraints, if any"""
 
+    allow_inf_nan: NotRequired[bool]
     constant: NotRequired[bool]
     decimal_places: NotRequired[int]
     ge: NotRequired[int | float | Decimal]
     gt: NotRequired[int | float | Decimal]
     item_type: NotRequired[Any]
     le: NotRequired[int | float | Decimal]
     lower_case: NotRequired[bool]
     lt: NotRequired[int | float | Decimal]
     max_digits: NotRequired[int]
     max_length: NotRequired[int]
     min_length: NotRequired[int]
     multiple_of: NotRequired[int | float | Decimal]
     path_type: NotRequired[Literal["file", "dir", "new"]]
     pattern: NotRequired[str | Pattern]
+    strict: NotRequired[bool]
+    tz: NotRequired[datetime.tzinfo]
     unique_items: NotRequired[bool]
     upper_case: NotRequired[bool]
     url: NotRequired[UrlConstraints]
     uuid_version: NotRequired[Literal[1, 3, 4, 5]]
 
 
 class FieldMeta:
@@ -106,15 +110,15 @@
 
         :returns: A field meta instance.
         """
         field_type = normalize_annotation(annotation, random=random)
 
         # FIXME: remove the pragma when switching to pydantic v2 permanently
         if not constraints and is_annotated(annotation):  # pragma: no cover
-            _, metadata = unwrap_annotated(field_type, random=random)
+            _, metadata = unwrap_annotated(annotation, random=random)
             constraints = cls.parse_constraints(metadata)
 
         field = cls(
             annotation=TYPE_MAPPING[field_type] if field_type in TYPE_MAPPING else field_type,
             random=random,
             name=name,
             default=default,
@@ -126,66 +130,69 @@
                 FieldMeta.from_type(annotation=unwrap_new_type(arg), random=random) for arg in field.type_args
             ]
         return field
 
     # FIXME: remove the pragma when switching to pydantic v2 permanently
     @classmethod
     def parse_constraints(cls, metadata: list[Any]) -> "Constraints":  # pragma: no cover
-        try:
-            import annotated_types
-
-            annotated_types_meta_data = [
-                ("ge", (annotated_types.Ge, annotated_types.Interval)),
-                ("le", (annotated_types.Le, annotated_types.Interval)),
-                ("lt", (annotated_types.Lt, annotated_types.Interval)),
-                ("gt", (annotated_types.Gt, annotated_types.Interval)),
-                ("min_length", (annotated_types.MinLen, annotated_types.Len)),
-                ("max_length", (annotated_types.MaxLen, annotated_types.Len)),
-                ("multiple_of", annotated_types.MultipleOf),
-                # deprecated by pydantic v2
-                ("min_items", (annotated_types.MinLen, annotated_types.Len)),
-                ("max_items", (annotated_types.MaxLen, annotated_types.Len)),
-            ]
-        except ImportError:
-            annotated_types_meta_data = []
-
-        try:
-            from pydantic import UrlConstraints
-            from pydantic._internal._fields import PydanticGeneralMetadata
-            from pydantic.types import PathType, UuidVersion
-
-            pydantic_annotated_meta_data = [
-                ("pattern", PydanticGeneralMetadata),
-                ("max_digits", PydanticGeneralMetadata),
-                ("decimal_places", PydanticGeneralMetadata),
-                # pydantic 2 only constraints
-                ("strict", PydanticGeneralMetadata),
-                ("allow_inf_nan", PydanticGeneralMetadata),
-                ("url", UrlConstraints),
-                ("uuid_version", UuidVersion),
-                ("path_type", PathType),
-            ]
-        except ImportError:
-            PydanticGeneralMetadata = Null  # type: ignore
-            UrlConstraints = Null  # type: ignore
-            UuidVersion = Null  # type: ignore
-            PathType = Null  # type: ignore
-            pydantic_annotated_meta_data = []
-
         constraints = {}
 
-        for key, annotated_type in [*annotated_types_meta_data, *pydantic_annotated_meta_data]:
-            for constraint in metadata:
-                if isinstance(constraint, annotated_type):  # type: ignore[arg-type]
-                    if isinstance(constraint, PydanticGeneralMetadata):
-                        constraints[key] = constraint.__dict__.get(key, None)
-                    elif isinstance(constraint, UrlConstraints):
-                        constraints[key] = dict(constraint.__dict__)
-                    elif isinstance(constraint, UuidVersion):
-                        constraints[key] = constraint.uuid_version  # pyright: ignore
-                    elif isinstance(constraint, PathType):
-                        constraints[key] = constraint.path_type  # pyright: ignore
-                    elif key not in ["min_items", "max_items"]:
-                        constraints[key] = getattr(constraint, key)
-                    else:
-                        constraints[key] = getattr(constraint, "min_length" if key == "min_items" else "max_length")
+        for value in metadata:
+            if is_annotated(value):
+                _, inner_metadata = unwrap_annotated(value, random=DEFAULT_RANDOM)
+                constraints.update(cast("dict[str, Any]", cls.parse_constraints(metadata=inner_metadata)))
+            elif func := getattr(value, "func", None):
+                if func is str.islower:
+                    constraints.update({"lower_case": True})
+                if func is str.isupper:
+                    constraints.update({"upper_case": True})
+                if func is str.isascii:
+                    constraints.update({"pattern": "[[:ascii:]]"})
+                if func is str.isdigit:
+                    constraints.update({"pattern": "[[:digit:]]"})
+            elif allowed_schemas := getattr(value, "allowed_schemas", None):
+                constraints.update(
+                    {
+                        "url": {
+                            k: v
+                            for k, v in {
+                                "max_length": getattr(value, "max_length", None),
+                                "allowed_schemes": allowed_schemas,
+                                "host_required": getattr(value, "host_required", None),
+                                "default_host": getattr(value, "default_host", None),
+                                "default_port": getattr(value, "default_port", None),
+                                "default_path": getattr(value, "default_path", None),
+                            }.items()
+                            if v is not None
+                        }
+                    }
+                )
+            else:
+                constraints.update(
+                    {
+                        k: v
+                        for k, v in {
+                            "allow_inf_nan": getattr(value, "allow_inf_nan", None),
+                            "constant": getattr(value, "const", None) is not None,
+                            "decimal_places": getattr(value, "decimal_places", None),
+                            "ge": getattr(value, "ge", None),
+                            "gt": getattr(value, "gt", None),
+                            "item_type": getattr(value, "item_type", None),
+                            "le": getattr(value, "le", None),
+                            "lower_case": getattr(value, "to_lower", None),
+                            "lt": getattr(value, "lt", None),
+                            "max_digits": getattr(value, "max_digits", None),
+                            "max_length": getattr(value, "max_length", getattr(value, "max_length", None)),
+                            "min_length": getattr(value, "min_length", getattr(value, "min_items", None)),
+                            "multiple_of": getattr(value, "multiple_of", None),
+                            "path_type": getattr(value, "path_type", None),
+                            "pattern": getattr(value, "regex", getattr(value, "pattern", None)),
+                            "strict": getattr(value, "strict", None),
+                            "tz": getattr(value, "tz", None),
+                            "unique_items": getattr(value, "unique_items", None),
+                            "upper_case": getattr(value, "to_upper", None),
+                            "uuid_version": getattr(value, "uuid_version", None),
+                        }.items()
+                        if v is not None
+                    }
+                )
         return cast("Constraints", constraints)
```

### Comparing `polyfactory-2.3.2/polyfactory/fields.py` & `polyfactory-2.3.3/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/persistence.py` & `polyfactory-2.3.3/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/pytest_plugin.py` & `polyfactory-2.3.3/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/utils/helpers.py` & `polyfactory-2.3.3/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/utils/predicates.py` & `polyfactory-2.3.3/polyfactory/utils/predicates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
-import sys
 from inspect import isclass
 from typing import Any, Literal, NewType, Optional, TypeVar, Union, get_args
 
 from typing_extensions import (
     Annotated,
     NotRequired,
     ParamSpec,
     Required,
     TypeGuard,
+    _AnnotatedAlias,
     get_origin,
 )
 
 from polyfactory.constants import TYPE_MAPPING
 
-if sys.version_info >= (3, 10):  # pragma: no cover
+try:
     from types import NoneType, UnionType
 
     UNION_TYPES = {UnionType, Union}
-else:  # pragma: no cover
-    NoneType = type(None)
+except ImportError:
+    NoneType = type(None)  # type: ignore
     UNION_TYPES = {Union}
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
@@ -107,15 +107,17 @@
 def is_annotated(annotation: Any) -> bool:
     """Determine whether a given annotation is 'typing.Annotated'.
 
     :param annotation: A type annotation.
 
     :returns: A boolean.
     """
-    return get_origin(annotation) is Annotated
+    return get_origin(annotation) is Annotated or (
+        isinstance(annotation, _AnnotatedAlias) and getattr(annotation, "__args__", None) is not None
+    )
 
 
 def get_type_origin(annotation: Any) -> Any:
     """Get the type origin of an annotation - safely.
 
     :param annotation: A type annotation.
```

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/complex_types.py` & `polyfactory-2.3.3/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.3.3/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.3.3/polyfactory/value_generators/constrained_dates.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
-from datetime import date, datetime, timedelta, timezone
+from datetime import date, datetime, timedelta, timezone, tzinfo
 from typing import TYPE_CHECKING, cast
 
 if TYPE_CHECKING:
     from faker import Faker
 
 
 def handle_constrained_date(
     faker: Faker,
     ge: date | None = None,
     gt: date | None = None,
     le: date | None = None,
     lt: date | None = None,
+    tz: tzinfo = timezone.utc,
 ) -> date:
     """Generates a date value fulfilling the expected constraints.
 
     :param faker: An instance of faker.
     :param lt: Less than value.
     :param le: Less than or equal value.
     :param gt: Greater than value.
     :param ge: Greater than or equal value.
+    :param tz: A timezone.
 
     :returns: A date instance.
     """
-    start_date = datetime.now(tz=timezone.utc).date() - timedelta(days=100)
+    start_date = datetime.now(tz=tz).date() - timedelta(days=100)
     if ge:
         start_date = ge
     elif gt:
         start_date = gt + timedelta(days=1)
 
     end_date = datetime.now(tz=timezone.utc).date() + timedelta(days=100)
     if le:
```

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.3.3/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/constrained_path.py` & `polyfactory-2.3.3/polyfactory/value_generators/constrained_path.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.3.3/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/constrained_url.py` & `polyfactory-2.3.3/polyfactory/value_generators/constrained_url.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/constrained_uuid.py` & `polyfactory-2.3.3/polyfactory/value_generators/constrained_uuid.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/primitives.py` & `polyfactory-2.3.3/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/polyfactory/value_generators/regex.py` & `polyfactory-2.3.3/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.2/pyproject.toml` & `polyfactory-2.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.3.2"
+version = "2.3.3"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -52,39 +52,42 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Testing :: Unit",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-packages = [
-    { include = "polyfactory" },
-]
+packages = [{ include = "polyfactory" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 beanie = { version = "*", optional = true, extras = ["beanie"] }
 faker = "*"
 msgspec = { version = "*", optional = true, extras = ["msgspec"] }
 odmantic = { version = "*", optional = true, extras = ["odmantic"] }
-pydantic = { version = "*", optional = true, extras = ["pydantic", "odmantic", "beanie"] }
+pydantic = { version = "*", optional = true, extras = [
+    "pydantic",
+    "odmantic",
+    "beanie",
+] }
 typing-extensions = "*"
 
 [tool.poetry.group.dev.dependencies]
 beanie = "*"
 email-validator = "*"
 hypothesis = "*"
 mongomock-motor = "*"
 msgspec = "*"
 odmantic = "*"
 pre-commit = "*"
 pydantic = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
+annotated-types = ">=0.5.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx-autobuild = "*"
 blacken-docs = "*"
 auto-pytabs = "*"
 sphinxcontrib-mermaid = "*"
 sphinx-copybutton = "*"
@@ -116,20 +119,20 @@
 
 [tool.coverage.report]
 exclude_lines = [
     'pragma: no cover',
     'if TYPE_CHECKING:',
     'except ImportError:',
     'except ImportError as e:',
-    '\.\.\.'
+    '\.\.\.',
 ]
 
 [tool.ruff]
 select = [
-    "A", # flake8-builtins
+    "A",   # flake8-builtins
     "B",   # flake8-bugbear
     "BLE", # flake8-blind-except
     "C4",  # flake8-comprehensions
     "D",   # pydocstyle
     "DJ",  # flake8-django
     "DTZ", # flake8-datetimez
     "E",   # pycodestyle errors
@@ -157,29 +160,29 @@
     "TID", # flake8-tidy-imports
     "UP",  # pyupgrade
     "W",   # pycodestyle - warning
     "YTT", # flake8-2020
 ]
 
 ignore = [
-    "A003", # flake8-builtins - class attribute {name} is shadowing a python builtin
-    "B010", # flake8-bugbear - do not call setattr with a constant attribute value
-    "D100", # pydocstyle - missing docstring in public module
-    "D101", # pydocstyle - missing docstring in public class
-    "D102", # pydocstyle - missing docstring in public method
-    "D103", # pydocstyle - missing docstring in public function
-    "D104", # pydocstyle - missing docstring in public package
-    "D105", # pydocstyle - missing docstring in magic method
-    "D106", # pydocstyle - missing docstring in public nested class
-    "D107", # pydocstyle - missing docstring in __init__
-    "D202", # pydocstyle - no blank lines allowed after function docstring
-    "D205", # pydocstyle - 1 blank line required between summary line and description
-    "D415", # pydocstyle - first line should end with a period, question mark, or exclamation point
-    "E501", # pycodestyle line too long, handled by black
-    "N818", # pep8-naming - exception name should be named with an Error suffix
+    "A003",  # flake8-builtins - class attribute {name} is shadowing a python builtin
+    "B010",  # flake8-bugbear - do not call setattr with a constant attribute value
+    "D100",  # pydocstyle - missing docstring in public module
+    "D101",  # pydocstyle - missing docstring in public class
+    "D102",  # pydocstyle - missing docstring in public method
+    "D103",  # pydocstyle - missing docstring in public function
+    "D104",  # pydocstyle - missing docstring in public package
+    "D105",  # pydocstyle - missing docstring in magic method
+    "D106",  # pydocstyle - missing docstring in public nested class
+    "D107",  # pydocstyle - missing docstring in __init__
+    "D202",  # pydocstyle - no blank lines allowed after function docstring
+    "D205",  # pydocstyle - 1 blank line required between summary line and description
+    "D415",  # pydocstyle - first line should end with a period, question mark, or exclamation point
+    "E501",  # pycodestyle line too long, handled by black
+    "N818",  # pep8-naming - exception name should be named with an Error suffix
     "UP037", # pyupgrade - removes quotes from type annotation
 ]
 line-length = 120
 src = ["polyfactory", "tests", "docs/examples"]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
@@ -194,10 +197,68 @@
 ]
 
 [tool.ruff.isort]
 known-first-party = ["polyfactory", "tests"]
 
 [tool.ruff.per-file-ignores]
 "polyfactory/field_meta.py" = ["N806"]
-"tests/**/*.*" = ["S101", "D", "ARG", "PGH", "B", "FBT", "PTH", "A", "TCH", "DTZ", "TRY", "EM", "S", "N", "SIM", "PLR", "BLE", "RSE", "C901", "PLW", "G", "PIE"]
-"docs/examples/tests/**/*.*" = ["S101", "D", "ARG", "PGH", "B", "FBT", "PTH", "A", "TCH", "DTZ", "TRY", "EM", "S", "N", "SIM", "PLR", "BLE", "RSE", "C901", "PLW", "G", "PIE"]
-"docs/**/*.*" = ["S", "B", "DTZ", "A", "TCH", "ERA", "D", "RET", "E731"]
+"tests/**/*.*" = [
+    "S101",
+    "D",
+    "ARG",
+    "PGH",
+    "B",
+    "FBT",
+    "PTH",
+    "A",
+    "TCH",
+    "DTZ",
+    "TRY",
+    "EM",
+    "S",
+    "N",
+    "SIM",
+    "PLR",
+    "BLE",
+    "RSE",
+    "C901",
+    "PLW",
+    "G",
+    "PIE",
+    "RUF012",
+]
+"docs/examples/tests/**/*.*" = [
+    "S101",
+    "D",
+    "ARG",
+    "PGH",
+    "B",
+    "FBT",
+    "PTH",
+    "A",
+    "TCH",
+    "DTZ",
+    "TRY",
+    "EM",
+    "S",
+    "N",
+    "SIM",
+    "PLR",
+    "BLE",
+    "RSE",
+    "C901",
+    "PLW",
+    "G",
+    "PIE",
+]
+"docs/**/*.*" = [
+    "S",
+    "B",
+    "DTZ",
+    "A",
+    "TCH",
+    "ERA",
+    "D",
+    "RET",
+    "E731",
+    "RUF012",
+]
```

### Comparing `polyfactory-2.3.2/PKG-INFO` & `polyfactory-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.3.2
+Version: 2.3.3
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -67,15 +67,15 @@
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 
-[![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-9-orange.svg?style=flat-square)](#contributors-)
 
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 <!-- markdownlint-restore -->
 
 Polyfactory is a simple and powerful mock data generation library, based around type
@@ -157,14 +157,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/guacs"><img src="https://avatars.githubusercontent.com/u/126393040?v=4?s=100" width="100px;" alt="guacs"/><br /><sub><b>guacs</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=guacs" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/VSHUMILIN97"><img src="https://avatars.githubusercontent.com/u/27234763?v=4?s=100" width="100px;" alt="Vadim"/><br /><sub><b>Vadim</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=VSHUMILIN97" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

