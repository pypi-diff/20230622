# Comparing `tmp/hayloft-0.2.0a2.tar.gz` & `tmp/hayloft-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.2.0a2.tar", max compression
+gzip compressed data, was "hayloft-0.2.1.tar", max compression
```

## Comparing `hayloft-0.2.0a2.tar` & `hayloft-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.0a2/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.0a2/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.0a2/hayloft/__init__.py
--rw-r--r--   0        0        0     3268 2023-06-22 09:38:40.225479 hayloft-0.2.0a2/hayloft/app-old.py
--rw-r--r--   0        0        0     3410 2023-06-22 09:49:41.116144 hayloft-0.2.0a2/hayloft/app.py
--rw-r--r--   0        0        0      673 2023-06-22 09:01:21.737742 hayloft-0.2.0a2/hayloft/cors.py
--rw-r--r--   0        0        0      863 2023-06-20 13:55:34.742760 hayloft-0.2.0a2/hayloft/llama_index.py
--rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.2.0a2/hayloft/logger.py
--rw-r--r--   0        0        0   175448 2023-06-22 09:16:49.415090 hayloft-0.2.0a2/hayloft/public/assets/index-0cc0a4d1.js
--rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.0a2/hayloft/public/assets/index-7630e259.css
--rw-r--r--   0        0        0      384 2023-06-22 09:16:45.491685 hayloft-0.2.0a2/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.2.0a2/hayloft/schema-old.py
--rw-r--r--   0        0        0      816 2023-06-22 10:34:29.676305 hayloft-0.2.0a2/hayloft/schema.py
--rw-r--r--   0        0        0      554 2023-06-21 14:45:37.279127 hayloft-0.2.0a2/hayloft/sse.py
--rw-r--r--   0        0        0      543 2023-06-22 10:35:00.229129 hayloft-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 hayloft-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.1/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.1/hayloft/__init__.py
+-rw-r--r--   0        0        0     3365 2023-06-22 12:28:57.584359 hayloft-0.2.1/hayloft/app.py
+-rw-r--r--   0        0        0      673 2023-06-22 09:01:21.737742 hayloft-0.2.1/hayloft/cors.py
+-rw-r--r--   0        0        0      863 2023-06-20 13:55:34.742760 hayloft-0.2.1/hayloft/llama_index.py
+-rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.2.1/hayloft/logger.py
+-rw-r--r--   0        0        0   175448 2023-06-22 09:16:49.415090 hayloft-0.2.1/hayloft/public/assets/index-0cc0a4d1.js
+-rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.1/hayloft/public/assets/index-7630e259.css
+-rw-r--r--   0        0        0      384 2023-06-22 09:16:45.491685 hayloft-0.2.1/hayloft/public/index.html
+-rw-r--r--   0        0        0      575 2023-06-22 10:39:00.726417 hayloft-0.2.1/hayloft/schema.py
+-rw-r--r--   0        0        0      554 2023-06-21 14:45:37.279127 hayloft-0.2.1/hayloft/sse.py
+-rw-r--r--   0        0        0      541 2023-06-22 12:29:39.301564 hayloft-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 hayloft-0.2.1/PKG-INFO
```

### Comparing `hayloft-0.2.0a2/LICENSE` & `hayloft-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a2/README.md` & `hayloft-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a2/hayloft/app-old.py` & `hayloft-0.2.1/hayloft/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,109 @@
-from flask import request, jsonify, send_file, send_from_directory, Response
-from flask_cors import CORS
-from hayloft.schema import app, db, sse, Event, Session
+from gevent import monkey; monkey.patch_all()
+from bottle import app, static_file, request, response, GeventServer
+from hayloft.schema import db, Session, Event
+from hayloft.cors import EnableCors
+from hayloft.sse import sse
 from importlib.metadata import version
+from pathlib import Path
+from typing import Dict
 import argparse
 import time
 
-CORS(app)  # for development
+app = app()
+app.install(EnableCors()) 
+path = str(Path(__file__).parent.resolve()) 
 
-@app.route("/", methods=["GET"])
+@app.get("/")
 def index():
-    return send_file("public/index.html")
+    return static_file("index.html", root=f"{path}/public")
 
+@app.get("/assets/<file:path>")
+def serve_assets(file):
+    return static_file(file, root=f"{path}/public/assets")
 
-@app.route("/assets/<path:path>", methods=["GET"])
-def serve_assets(path):
-    return send_from_directory("public/assets", path)
-
-
-@app.route("/event", methods=["POST"])
+@app.post("/event")
 def create_event():
-    body = request.get_json()
-    title = body["title"]
-    message = body["message"]
-    type = body["type"]
+    body = request.json
+    session_name = body.get("session")
+    title = body.get("title")
+    message = body.get("message")
+    type = body.get("type")
     event: Event | None = None
-    sess: Session | None = None
+    new_session: Session | None = None
 
     try:
-        session = db.session.execute(
-            db.select(Session).filter_by(name=body["session"])
-        ).scalar_one()
-        event = Event(title=title, message=message, type=type, session_id=session.id)
-        db.session.add(event)
+        session = Session.select().where(Session.name == session_name).get()
+        event = Event.create(session=session, title=title, message=message, type=type)
     except:
         created_at = int(time.time() * 1000)
-        event = Event(title=title, message=message, type=type)
-        sess = Session(name=body["session"], created_at=created_at, events=[event])
-        db.session.add(sess)
-    db.session.commit()
-    msg: dict
-    if sess is not None:
+        new_session = Session.create(name=session_name, created_at=created_at)
+        event = Event.create(session=new_session, title=title, message=message, type=type)
+    msg: Dict
+    if new_session is not None:
         msg = {
             "session": {
-                "id": sess.id,
-                "name": sess.name,
-                "created_at": sess.created_at,
+                "id": new_session.id,
+                "name": new_session.name,
+                "created_at": new_session.created_at,
             },
             "event": None,
         }
     else:
         msg = {
             "event": {
                 "id": event.id,
                 "title": event.title,
                 "message": event.message,
                 "type": event.type,
-                "session_id": event.session_id,
+                "session_id": event.session.id,
             },
             "session": None,
         }
     sse.publish(msg, type="stream")
     return "OK"
 
-
-@app.route("/sessions", methods=["GET"])
+@app.get('/sessions')
 def get_sessions():
-    sessions = db.session.execute(db.select(Session)).scalars()
-    return jsonify(
-        [{"id": s.id, "name": s.name, "created_at": s.created_at} for s in sessions]
-    )
-
-
-@app.route("/sessions", methods=["DELETE"])
-def remove_sessions():
-    # todo it via cascade later
-    db.session.query(Session).delete()
-    db.session.query(Event).delete()
-    db.session.commit()
-    return ""
-
+    sessions = Session.select()
+    return {"sessions": [{"id": s.id, "name": s.name, "created_at": s.created_at} for s in sessions]} 
 
-@app.route("/sessions/<int:session_id>/events", methods=["GET"])
+@app.get("/sessions/<session_id:int>/events")
 def get_events(session_id):
-    events = db.session.execute(
-        db.select(Event).filter_by(session_id=session_id)
-    ).scalars()
-    return jsonify(
-        [
+    events = Event.select().where(Event.session_id == session_id)
+    return { 
+        "events": [
             {"id": e.id, "title": e.title, "message": e.message, "type": e.type}
             for e in events
         ]
-    )
+    }
 
-
-@app.route("/listen", methods=["GET"])
+@app.get("/listen")
 def listen():
-    def stream():
-        messages = sse.listen()
-        while True:
-            msg = messages.get()
-            yield msg
-
-    return Response(stream(), mimetype="text/event-stream")
-
+    response.set_header("Content-Type", "text/event-stream")
+    response.set_header("Cache-Control", "no-cache")
+    yield 'retry: 100\n\n' 
+    messages = sse.listen()
+    
+    while True:
+        msg = messages.get()
+        yield msg
+
+def start():
+    db.connect()
+    db.create_tables([Session, Event])
+
+    print(f'\033[96mHayloft {version(__package__)} starting up, open in your browser http://localhost:7000\033[0m')
+    print("Hit Ctrl-C to quit.")
+    app.run(host='localhost', port=7000, server=GeventServer, quiet=True)
 
 def cli():
     parser = argparse.ArgumentParser(description="Hayloft - UI tool for LLM frameworks")
     parser.add_argument("command", type=str, help="command to run", choices=["start"])
     parser.add_argument("-v", "--version", action="version", version=version(__package__))
     args = parser.parse_args()
 
     if args.command == "start":
-        app.run(host="localhost", port=7000, debug=False)
+        start()
+
+if __name__ == '__main__':
+    start()
```

### Comparing `hayloft-0.2.0a2/hayloft/cors.py` & `hayloft-0.2.1/hayloft/cors.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a2/hayloft/llama_index.py` & `hayloft-0.2.1/hayloft/llama_index.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a2/hayloft/logger.py` & `hayloft-0.2.1/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a2/hayloft/public/assets/index-0cc0a4d1.js` & `hayloft-0.2.1/hayloft/public/assets/index-0cc0a4d1.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a2/hayloft/public/assets/index-7630e259.css` & `hayloft-0.2.1/hayloft/public/assets/index-7630e259.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a2/hayloft/sse.py` & `hayloft-0.2.1/hayloft/sse.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a2/pyproject.toml` & `hayloft-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hayloft"
-version = "0.2.0a2"
+version = "0.2.1"
 description = "UI tool for LLM frameworks"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eturchenkov/hayloft"
 keywords = ["llm framework", "llm app tracking", "ui for llm app"]
```

### Comparing `hayloft-0.2.0a2/PKG-INFO` & `hayloft-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.2.0a2
+Version: 0.2.1
 Summary: UI tool for LLM frameworks
 Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
 Keywords: llm framework,llm app tracking,ui for llm app
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

