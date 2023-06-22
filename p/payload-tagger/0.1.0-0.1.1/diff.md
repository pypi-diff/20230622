# Comparing `tmp/payload_tagger-0.1.0.tar.gz` & `tmp/payload_tagger-0.1.1.tar.gz`

## Comparing `payload_tagger-0.1.0.tar` & `payload_tagger-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/.tool-versions
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/payload_tagger/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/payload_tagger/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/payload_tagger/py.typed
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/payload_tagger/whatsapp.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/requirements/core.txt
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/requirements/dev.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/scripts/release_github.py
--rw-r--r--   0        0        0    46092 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/tests/unit/test_whastapp.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/LICENSE
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/README.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 payload_tagger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.tool-versions
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/payload_tagger/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/payload_tagger/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/payload_tagger/py.typed
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/payload_tagger/whatsapp.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/requirements/core.txt
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/requirements/dev.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/scripts/release_github.py
+-rw-r--r--   0        0        0    46092 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/tests/unit/test_whastapp.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/LICENSE
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/README.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/PKG-INFO
```

### Comparing `payload_tagger-0.1.0/.github/workflows/release.yml` & `payload_tagger-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.0/.github/workflows/test.yml` & `payload_tagger-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.0/.vscode/settings.json` & `payload_tagger-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.0/payload_tagger/whatsapp.py` & `payload_tagger-0.1.1/payload_tagger/whatsapp.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 
 
 def _has_type(payload_changes: dict[str, Any]) -> bool:
     return "type" in payload_changes["value"]["messages"][0]
 
 
 def _is_text_message(payload_changes: dict[str, Any]) -> bool:
+    msgs: dict[str, Any] = payload_changes["value"]["messages"][0]
     if (
-        "referral" not in payload_changes["value"]["messages"][0]
-        and "context" not in payload_changes["value"]["messages"][0]
-        and payload_changes["value"]["messages"][0]["type"] == "text"
+        "referral" not in msgs
+        and "context" not in msgs
+        and msgs["type"] == "text"
     ):
         return True
     return False
 
 
 def _is_reaction_message(payload_changes: dict[str, Any]) -> bool:
     if payload_changes["value"]["messages"][0]["type"] == "reaction":
@@ -75,30 +76,30 @@
         return True
     return False
 
 
 def _is_received_answer_from_list_message(
     payload_changes: dict[str, Any],
 ) -> bool:
+    msgs: dict[str, Any] = payload_changes["value"]["messages"][0]
     if (
-        payload_changes["value"]["messages"][0]["type"] == "interactive"
-        and payload_changes["value"]["messages"][0]["interactive"]["type"]
-        == "list_reply"
+        msgs["type"] == "interactive"
+        and msgs["interactive"]["type"] == "list_reply"
     ):
         return True
     return False
 
 
 def _is_received_answer_to_reply_button(
     payload_changes: dict[str, Any],
 ) -> bool:
+    msgs: dict[str, Any] = payload_changes["value"]["messages"][0]
     if (
-        payload_changes["value"]["messages"][0]["type"] == "interactive"
-        and payload_changes["value"]["messages"][0]["interactive"]["type"]
-        == "button_reply"
+        msgs["type"] == "interactive"
+        and msgs["interactive"]["type"] == "button_reply"
     ):
         return True
     return False
 
 
 def _message_changes(
     payload: dict[str, Any],
@@ -111,51 +112,69 @@
         None,
     )
     if not changes:
         return Err(errors.NotIdentifiedPayloadError(payload=payload))
     return Ok(changes[0])
 
 
-def identify_payload(  # noqa: C901, PLR0912
-    payload: dict[str, Any],
-) -> Result[SupportedWebhooks, errors.NotIdentifiedPayloadError]:
-    """Identify Whatsapp payload."""
+def _identify_payload_no_type(
+    payload_changes: dict[str, Any],
+) -> SupportedWebhooks | None:
     identified: SupportedWebhooks
 
-    changes_retrieved = _message_changes(payload=payload)
-    if not isinstance(changes_retrieved, Ok):
-        return changes_retrieved
-
-    changes = changes_retrieved.unwrap()
-
-    if not _has_messages(payload_changes=changes):
-        return Err(errors.NotIdentifiedPayloadError(payload=payload))
+    if _is_location_message(payload_changes=payload_changes):
+        identified = "location-message"
+    elif _is_contact_message(payload_changes=payload_changes):
+        identified = "contact-message"
+    else:
+        return None
+    return identified
 
-    if not _has_type(payload_changes=changes):
-        if _is_location_message(payload_changes=changes):
-            identified = "location-message"
-        elif _is_contact_message(payload_changes=changes):
-            identified = "contact-message"
-        else:
-            return Err(errors.NotIdentifiedPayloadError(payload=payload))
-        return Ok(identified)
 
-    if _is_text_message(payload_changes=changes):
+def _identify_core_msgs(
+    payload_changes: dict[str, Any],
+) -> SupportedWebhooks | None:
+    identified: SupportedWebhooks
+    if _is_text_message(payload_changes=payload_changes):
         identified = "text-message"
-    elif _is_reaction_message(payload_changes=changes):
+    elif _is_reaction_message(payload_changes=payload_changes):
         identified = "reaction-message"
-    elif _is_media_message(payload_changes=changes):
+    elif _is_media_message(payload_changes=payload_changes):
         identified = "media-message"
     elif _is_received_callback_from_quick_reply_button(
-        payload_changes=changes,
+        payload_changes=payload_changes,
     ):
         identified = "received-callback-from-quick-reply-button"
     elif _is_received_answer_from_list_message(
-        payload_changes=changes,
+        payload_changes=payload_changes,
     ):
         identified = "received-answer-from-list-message"
-    elif _is_received_answer_to_reply_button(payload_changes=changes):
+    elif _is_received_answer_to_reply_button(payload_changes=payload_changes):
         identified = "received-answer-to-reply-button"
     else:
+        return None
+    return identified
+
+
+def identify_payload(
+    payload: dict[str, Any],
+) -> Result[SupportedWebhooks, errors.NotIdentifiedPayloadError]:
+    """Identify Whatsapp payload."""
+    changes_retrieved = _message_changes(payload=payload)
+    if not isinstance(changes_retrieved, Ok):
+        return changes_retrieved
+
+    changes = changes_retrieved.unwrap()
+
+    if not _has_messages(payload_changes=changes):
+        return Err(errors.NotIdentifiedPayloadError(payload=payload))
+
+    if not _has_type(payload_changes=changes):
+        identity = _identify_payload_no_type(payload_changes=changes)
+        if identity:
+            return Ok(identity)
         return Err(errors.NotIdentifiedPayloadError(payload=payload))
 
-    return Ok(identified)
+    identity = _identify_core_msgs(payload_changes=changes)
+    if identity:
+        return Ok(identity)
+    return Err(errors.NotIdentifiedPayloadError(payload=payload))
```

### Comparing `payload_tagger-0.1.0/requirements/dev.txt` & `payload_tagger-0.1.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.0/scripts/release_github.py` & `payload_tagger-0.1.1/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.0/tests/unit/test_whastapp.py` & `payload_tagger-0.1.1/tests/unit/test_whastapp.py`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.0/.gitignore` & `payload_tagger-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.0/LICENSE` & `payload_tagger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.0/pyproject.toml` & `payload_tagger-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "payload_tagger"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
```

### Comparing `payload_tagger-0.1.0/PKG-INFO` & `payload_tagger-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload_tagger
-Version: 0.1.0
+Version: 0.1.1
 Project-URL: Documentation, https://github.com/Tomperez98/payload-tagger#readme
 Project-URL: Issues, https://github.com/Tomperez98/payload-tagger/issues
 Project-URL: Source, https://github.com/Tomperez98/payload-tagger
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
```

