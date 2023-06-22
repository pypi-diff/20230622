# Comparing `tmp/piaf-0.2.1.tar.gz` & `tmp/piaf-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piaf-0.2.1.tar", max compression
+gzip compressed data, was "piaf-0.3.0b1.tar", max compression
```

## Comparing `piaf-0.2.1.tar` & `piaf-0.3.0b1.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     1072 2023-03-02 10:05:49.333733 piaf-0.2.1/LICENSE
--rw-r--r--   0        0        0     1927 2023-03-02 10:05:49.333733 piaf-0.2.1/README.md
--rw-r--r--   0        0        0     2111 2023-03-02 10:05:49.335733 piaf-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      114 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/__init__.py
--rw-r--r--   0        0        0    11547 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/agent.py
--rw-r--r--   0        0        0     2744 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/api/__init__.py
--rw-r--r--   0        0        0     1177 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/api/config.py
--rw-r--r--   0        0        0    12539 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/api/controllers.py
--rw-r--r--   0        0        0     1456 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/api/dependencies.py
--rw-r--r--   0        0        0     2677 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/api/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/api/impl/__init__.py
--rw-r--r--   0        0        0    12352 2023-03-02 10:05:49.336733 piaf-0.2.1/src/piaf/api/impl/process.py
--rw-r--r--   0        0        0    14853 2023-03-02 10:05:49.337733 piaf-0.2.1/src/piaf/api/impl/tasks.py
--rw-r--r--   0        0        0     8248 2023-03-02 10:05:49.337733 piaf-0.2.1/src/piaf/api/models.py
--rw-r--r--   0        0        0    11227 2023-03-02 10:05:49.337733 piaf-0.2.1/src/piaf/api/routes.py
--rw-r--r--   0        0        0    10956 2023-03-02 10:05:49.337733 piaf-0.2.1/src/piaf/audit.py
--rw-r--r--   0        0        0    15380 2023-03-02 10:05:49.337733 piaf-0.2.1/src/piaf/behavior.py
--rw-r--r--   0        0        0    38095 2023-03-02 10:05:49.337733 piaf-0.2.1/src/piaf/comm/__init__.py
--rw-r--r--   0        0        0     5472 2023-03-02 10:05:49.337733 piaf-0.2.1/src/piaf/comm/mtp/amqp.py
--rw-r--r--   0        0        0    17258 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/comm/mts.py
--rw-r--r--   0        0        0      914 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/examples/benchmarks/empty_agents.py
--rw-r--r--   0        0        0     3020 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/examples/heavycomm.py
--rw-r--r--   0        0        0     1474 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/examples/helloworld.py
--rw-r--r--   0        0        0     4293 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/examples/pingpong.py
--rw-r--r--   0        0        0     6516 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/examples/two_platforms/ptf1.py
--rw-r--r--   0        0        0     2714 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/examples/two_platforms/ptf2.py
--rw-r--r--   0        0        0     5452 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/examples/useams.py
--rw-r--r--   0        0        0     8051 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/examples/usedf.py
--rw-r--r--   0        0        0     3930 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/exceptions.py
--rw-r--r--   0        0        0     6937 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/launcher.py
--rw-r--r--   0        0        0      180 2023-03-02 10:05:49.338733 piaf-0.2.1/src/piaf/platform.py
--rw-r--r--   0        0        0    25825 2023-03-02 10:05:49.339733 piaf-0.2.1/src/piaf/ptf.py
--rw-r--r--   0        0        0        0 2023-03-02 10:05:49.339733 piaf-0.2.1/src/piaf/py.typed
--rw-r--r--   0        0        0    29547 2023-03-02 10:05:49.339733 piaf-0.2.1/src/piaf/service.py
--rw-r--r--   0        0        0     7360 2023-03-02 10:05:49.339733 piaf-0.2.1/src/piaf/util.py
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 piaf-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-22 21:12:49.219051 piaf-0.3.0b1/LICENSE
+-rw-r--r--   0        0        0     1927 2023-06-22 21:12:49.219051 piaf-0.3.0b1/README.md
+-rw-r--r--   0        0        0     2308 2023-06-22 21:12:49.221051 piaf-0.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/__init__.py
+-rw-r--r--   0        0        0    11475 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/agent.py
+-rw-r--r--   0        0        0    13783 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/api/behavior.py
+-rw-r--r--   0        0        0      534 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/api/config.py
+-rw-r--r--   0        0        0     1227 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/api/exceptions.py
+-rw-r--r--   0        0        0    10566 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/api/models.py
+-rw-r--r--   0        0        0    10211 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/api/tasks.py
+-rw-r--r--   0        0        0    11665 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/audit.py
+-rw-r--r--   0        0        0    15379 2023-06-22 21:12:49.222051 piaf-0.3.0b1/src/piaf/behavior.py
+-rw-r--r--   0        0        0    38058 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/comm/__init__.py
+-rw-r--r--   0        0        0     5398 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/comm/mtp/amqp.py
+-rw-r--r--   0        0        0    18142 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/comm/mts.py
+-rw-r--r--   0        0        0     1319 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/examples/api.py
+-rw-r--r--   0        0        0      899 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/examples/benchmarks/empty_agents.py
+-rw-r--r--   0        0        0     3020 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/examples/heavycomm.py
+-rw-r--r--   0        0        0     1474 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/examples/helloworld.py
+-rw-r--r--   0        0        0     4273 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/examples/pingpong.py
+-rw-r--r--   0        0        0     6804 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/examples/two_platforms/ptf1.py
+-rw-r--r--   0        0        0     3015 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/examples/two_platforms/ptf2.py
+-rw-r--r--   0        0        0     5453 2023-06-22 21:12:49.223051 piaf-0.3.0b1/src/piaf/examples/useams.py
+-rw-r--r--   0        0        0     8053 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/examples/usedf.py
+-rw-r--r--   0        0        0     3931 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-22 21:12:49.250051 piaf-0.3.0b1/src/piaf/extensions/__init__.py
+-rw-r--r--   0        0        0     2492 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/extensions/amqp.py
+-rw-r--r--   0        0        0     2911 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/extensions/redis.py
+-rw-r--r--   0        0        0     7087 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/launcher.py
+-rw-r--r--   0        0        0      181 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/platform.py
+-rw-r--r--   0        0        0    26522 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/ptf.py
+-rw-r--r--   0        0        0        0 2023-06-22 21:12:49.250051 piaf-0.3.0b1/src/piaf/py.typed
+-rw-r--r--   0        0        0    29547 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/service.py
+-rw-r--r--   0        0        0     7361 2023-06-22 21:12:49.224051 piaf-0.3.0b1/src/piaf/util.py
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 piaf-0.3.0b1/PKG-INFO
```

### Comparing `piaf-0.2.1/LICENSE` & `piaf-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `piaf-0.2.1/README.md` & `piaf-0.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `piaf-0.2.1/pyproject.toml` & `piaf-0.3.0b1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,47 +2,53 @@
 authors = ["Pierre DUBAILLAY <pierredubaillay@outlook.fr>"]
 description = "A FIPA-compliant Agent Platform written in python."
 keywords = ["Python Agent Framework", "multi-agent", "asyncio"]
 license = "MIT"
 name = "piaf"
 readme = "README.md"
 repository = "https://gitlab.com/ornythorinque/piaf"
-version = "0.2.1"
+version = "0.3.0-beta.1"
 
 [tool.poetry.dependencies]
-aioredis = { version = "^2", optional = true }
 aiormq = { version = "^6", optional = true }
 async-timeout = { version = "^4", optional = true }
-fastapi = { version = "^0.92", optional = true }
+fastapi = { version = "^0.95", optional = true }
 python = ">=3.7,<4"
 yarl = { version = "^1", optional = true }
 python-dotenv = "^0.21"
 semver = "^2"
+redis = { version = "^4", optional = true }
+uvicorn = { extras = ["standard"], version = "^0.22", optional = true }
+pydantic = { version = "^1", optional = true }
 
 [tool.poetry.extras]
 amqp-mtp = ["aiormq", "yarl"]
-webapi = ["aioredis", "fastapi", "async-timeout"]
+redis-mtp = ["redis"]
+webapi = ["fastapi", "async-timeout", "uvicorn", "pydantic"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23"
 coverage = { version = "^7", extras = ["toml"] }
 mypy = "^1"
 pytest = "^7"
 pytest-html = "^3"
 requests = "^2"
 rstcheck = "^6"
 sphinx = "^5"
 sphinx_rtd_theme = "^1"
-uvicorn = { extras = ["standard"], version = "^0.20" }
 isort = "^5"
 bandit = "^1"
 pydocstyle = "^6"
 pyproject-flake8 = "^0.0.1-alpha.4"
 pytest-asyncio = "^0.20.3"
 
+[tool.poetry.group.types.dependencies]
+types-redis = "^4.5.1.5"
+types-requests = "^2.28.11.15"
+
 [tool.coverage.run]
 branch = true
 command_line = "-m pytest"
 data_file = ".report/coverage/data_db"
 omit = ["*/examples/*", "*/api/*"]
 source = ["piaf"]
```

### Comparing `piaf-0.2.1/src/piaf/agent.py` & `piaf-0.3.0b1/src/piaf/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,15 +155,14 @@
         :param aid: this agent's identifier
         :param platform: the platform facade that proxies the platform where this agent is deployed
         """
         self.logger = logging.getLogger(type(self).__name__)
         self._aid = copy.deepcopy(aid)
         self._behaviors: MutableSequence[asyncio.Future[None]] = []
         self._platform = platform
-        self._mailbox = piaf.comm.mts.MailBox()
 
     @property
     def state(self) -> AgentState:
         """
         Get this agent state.
 
         Readonly property that query the platform to get this agent's state.
@@ -182,26 +181,21 @@
 
         Please note that the retrieved object is a copy and can be safely modified
         without affecting the agent.
         Readonly property.
         """
         return copy.deepcopy(self._aid)
 
-    @property
-    def mailbox(self) -> piaf.comm.mts.MailBoxDelegate:
+    async def wait(self, aid: piaf.comm.AID | None = None) -> None:
         """
-        Get a reference to the internal's agent mailbox.
+        Put an agent in WAITING state.
 
-        You will get limited writing access.
+        :param aid: the AID of the targeted agent. If not set (default), the target is the calling agent itself.
         """
-        return piaf.comm.mts.MailBoxDelegate(self._mailbox)
-
-    async def wait(self) -> None:
-        """Put this agent in WAITING state."""
-        await self._platform.wait(self._aid)
+        await self._platform.wait(self._aid if aid is None else aid)
 
     async def suspend(self) -> None:
         """Suspend this agent."""
         await self._platform.suspend(self._aid)
 
     async def quit(self) -> None:
         """Shutdown the agent as soon as possible."""
@@ -278,29 +272,29 @@
 
         Templates are applied to ACL Messages, not Envelopes.
         Note that this is a blocking receive, meaning that the coroutine ends when a
         message is found. The default template match any kind of messages.
 
         :param template: the message template used to search messages
         """
-        return await self._mailbox.get(template)
+        return await self._platform.get_mailbox(self.aid).get(template)
 
     async def receive_nowait(
         self, template: piaf.comm.MessageTemplate = piaf.comm.MT_ALL()
     ) -> Union[None, piaf.comm.Message]:
         """
         Query this agent's mailbox to retrieve a message matching the provided template.
 
         Templates are applied to ACL Messages, not Envelopes.
         Contrary to :meth:`receive`, this method will return ``None`` if no matching
         message is found. The default template matches all messages.
 
         :param template: the message template used to search messages
         """
-        return await self._mailbox.get_nowait(template)
+        return await self._platform.get_mailbox(self.aid).get_nowait(template)
 
     def send(self, message: piaf.comm.ACLMessage) -> None:
         """
         Send a message.
 
         The underlying implementation will use information provided in the message to
         contact receivers.
```

### Comparing `piaf-0.2.1/src/piaf/api/impl/process.py` & `piaf-0.3.0b1/src/piaf/api/behavior.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,374 +1,403 @@
-# coding: utf-8
-"""This module contains a set of helper objects."""
+"""
+
+"""
 from __future__ import annotations
 
 import asyncio
-import importlib
 import json
-from contextlib import asynccontextmanager
-from enum import Enum
-from multiprocessing import Process
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Tuple, Union, cast
-
-import aioredis
-from aioredis import ConnectionPool, Redis
+from typing import Any, Dict, List, Union
 
-from piaf.agent import Agent
+import uvicorn
+from fastapi import (
+    APIRouter,
+    FastAPI,
+    Path,
+    Query,
+    Response,
+    WebSocket,
+    WebSocketDisconnect,
+    status,
+)
+from fastapi.middleware.cors import CORSMiddleware
+from fastapi.responses import JSONResponse
+
+import piaf
+import piaf.agent
+from piaf.agent import AgentState
 from piaf.api.config import Settings
-from piaf.api.exceptions import RedisConnectionNotInitialized, RedisError
+from piaf.api.exceptions import InternalServerError
+from piaf.api.models import (
+    ACLMessageModel,
+    AgentCreationDescriptionModel,
+    AgentMemoryModel,
+    AgentStateModel,
+    AIDModel,
+    AMSAgentDescriptionModel,
+    ExceptionModel,
+    serialize_piaf_object,
+)
+from piaf.api.tasks import *
+from piaf.audit import EventRecord, Subscriber, Topic
 from piaf.behavior import Behavior
-from piaf.comm import AID, ACLMessage
-from piaf.audit import Event, EventRecord, Subscriber, Topic
-from piaf.launcher import PlatformLauncher, ServiceDescription
-from piaf.ptf import AgentPlatform, AgentPlatformFacade, Extension
-from piaf.service import AMSAgentDescription
-
-if TYPE_CHECKING:
-    from aioredis.client import PubSub
 
+_description = """
+The APi allows you to manage this platform.
 
-class APIAgent(Agent):
-    """
-    A special agent that can communicate with the web API through a Redis connection.
+It lets you create, delete and query both the agents and the platform and can be extended with more functionalities. It is based on the [FastAPI](https://fastapi.tiangolo.com/) framework.
 
-    The agent will first try to connect to the redis database and then will listen to incoming tasks. Tasks execution results are sent back to the web API.
-    """
+The API also exposes a websocket allowing applications to (un)subscribe to/from event topics.
 
-    def __init__(self, aid: AID, platform: AgentPlatformFacade):
-        """
-        Initialize a new :class:`APIAgent` instance.
+Websocket
+---------
 
-        :param aid: the agent's :class:`AID`
-        :param platform: a reference to the underlying platform
-        """
-        super().__init__(aid, platform)
-        self.add_behavior(ExecuteTasksBehavior(self))
+In addition to the routes below, the API exposes a websocket allowing applications to (un)subscribe to/from event topics. The dedicated route is `ws://{server}/platforms/{ptf_name}/ws` and it is a double-sided websocket carrying JSON data. The client can send the following:
 
+    {
+        method: "[un]subscribe",
+        topic: ".some.topic"
+    }
 
-class ExecuteTasksBehavior(Behavior):
-    """
-    Pull tasks from the redis channel and execute each one sequentially.
+Once an event is emitted on the subscribed topic, the client receives through the websocket a JSON representation of the `EventRecord`:
 
-    This behavior requires an open connection to the redis database and a channel listening on the input tasks queue.
-    """
+    {
+        "event": {
+            "source": "some_source",
+            "type": "some_type",
+            "data": ...
+        },
+        "timestamp": 1663923272,
+        "topics": [".platform.agents", ".platform.agents.ams"]
+    }
+"""
 
-    def __init__(self, agent: APIAgent):
-        """
-        Initialize a new :class:`ExecuteTasksBehavior` instance.
 
-        :param agent: the owner
-        """
-        super().__init__(agent)
-
-    async def action(self) -> None:
-        """
-        Wait for incoming tasks and execute each one sequentially.
-
-        Incoming tasks should have the following structure::
-
-            {
-                "task_type": "[module.]class",
-                "id": "id_of_the_task",
-                ...
-            }
-
-        Tasks' class are dynamically imported from the specified module or :mod:`piaf.api.tasks` if no module is specified. Results are sent back in json into the response queue. The structure of a response is the following::
+class APIServerBehavior(Behavior):
+    """
+    Base behavior that exposes a REST API to manage the platform.
 
-            {
-                "id": "id-of-the-request",
-                "data": whatever is returned by the task's execution or null,
-                "error": error message if the execution failed, null otherwise
-            }
+    This is a single-shot behavior that starts a FastAPI server and stops the platform if stopped.
 
+    You can extend this behavior to add more routes to the API by subclassing it and overriding:
+    - `add_agents_routes` to add routes to the `/agents` router
+    - `add_platform_routes` to add routes to the `/platform` router
+    - `create_app` to customize the FastAPI app
+    """
 
-        """
-        async with self.db_session_and_channel() as (client, channel):
-            await channel.subscribe(f"channels:{self.agent.aid.hap_name}:from-api")
-            async for task in channel.listen():
-                json_task: Dict[str, Any] = json.loads(task["data"])
-                data = json_task["task_type"]
-                split_data = data.rsplit(".", maxsplit=1)
-
-                if len(split_data) == 1:
-                    module_name = "piaf.api.impl.tasks"
-                    klass_name = split_data[0]
-                else:
-                    module_name, klass_name = split_data
-                module = importlib.import_module(module_name)
-
-                try:
-                    klass = getattr(module, klass_name)
-                    id_ = json_task["id"]
-                    result = await klass.from_json(json_task).execute(self.agent)
-
-                    data = json.dumps(
-                        {"id": id_, "data": result, "error": None},
-                        default=serialize_piaf_object,
-                    )
+    def __init__(self, agent: piaf.agent.Agent, port=5000):
+        super().__init__(agent)
+        self.port = port
 
-                    await client.publish(
-                        f"channels:{self.agent.aid.hap_name}:to-api",
-                        data,
-                    )
+        self.agents_router = APIRouter(prefix="/agents")
+        self.platform_router = APIRouter(prefix="/platform")
 
-                except Exception as e:
-                    self.agent.logger.exception("Unable to run task.", exc_info=e)
-                    await client.publish(
-                        f"channels:{self.agent.aid.hap_name}:to-api",
-                        json.dumps({"id": id_, "data": None, "error": str(e)}),
-                    )
+        self.add_agents_routes()
+        self.add_platform_routes()
 
-    @asynccontextmanager
-    async def db_session_and_channel(
-        self,
-    ) -> AsyncGenerator[Tuple[Redis, PubSub], None]:
-        """
-        Work with a Redis client and a channel.
+        self._app = self.create_app()
 
-        If the wrapper task is cancelled, this context manager will catch any error, close both the channel and the client and then re-raise it.
-        """
-        client: None | Redis = None
-        channel: None | PubSub = None
+    async def action(self) -> Any:
+        """Configure the uvicorn server instance and launch the app."""
+        config = uvicorn.Config(app=self._app, port=self.port, log_level="info")
+        server = uvicorn.Server(config=config)
         try:
-            connection_pool = cast(
-                RedisConnectionPoolExtension, self.agent._platform.extensions["redis"]
-            )
-            client = connection_pool.client
-            channel = client.pubsub(ignore_subscribe_messages=True)
-            yield client, channel
+            await server.serve()
+        except asyncio.CancelledError:
+            self.agent.logger.info("API server stopped.")
+        except Exception as e:
+            self.agent.logger.exception(e)
         finally:
-            if channel is not None:
-                await channel.close()
-            if client is not None:
-                await client.close()
+            asyncio.create_task(self.agent._platform.stop())
 
     def done(self) -> bool:
-        """
-        One shot behavior, always return `True`.
+        """Single-shot behavior.
 
-        :return: `True`
+        :return: always `True`
         """
         return True
 
-
-class EventsToRedis(Subscriber):
-    """
-    Subscribe to all events and send them into the redis database.
-
-    This subscriber requires the :class:`RedisConnectionPoolExtension` extension to be loaded in order to send events to the Redis database.
-    """
-
-    def __init__(self, platform: AgentPlatform) -> None:
+    def create_app(self) -> FastAPI:
         """
-        Create a new :class:`EventToRedis` instance.
+        Create the FastAPI app.
 
-        :param platform: the agent platform
+        :return: the FastAPI app
         """
-        super().__init__()
-        self.hap_name = platform.name
-        self._platform = platform
-        self.redis: None | Redis = None
+        _app = FastAPI(
+            title="Piaf platform API",
+            description=_description,
+            version=piaf.__version__,
+            license_info={"name": "MIT", "url": "https://mit-license.org/"},
+        )
 
-    async def on_event(self, event_record: EventRecord) -> None:
-        """
-        Re-publish the event on each queue it is published.
+        # Configure CORS
+        settings = Settings()
 
-        :param event_record: the record
-        """
-        if self.redis is None:
-            self.redis = cast(
-                RedisConnectionPoolExtension, self._platform.extensions["redis"]
-            ).client
-
-        json_record = json.dumps(event_record, default=serialize_piaf_object)
-        tasks = []
-        for channel in event_record.topics:
-            tasks.append(
-                self.redis.publish(
-                    f"channels:{self.hap_name}:events:{channel}", json_record
-                )
-            )
+        _app.add_middleware(
+            CORSMiddleware,
+            allow_origins=settings.cors_origins,
+            allow_credentials=settings.cors_credentials,
+            allow_methods=settings.cors_methods,
+            allow_headers=settings.cors_headers,
+        )
 
-        results = await asyncio.gather(
-            *tasks, return_exceptions=True
-        )  # fixme: ignored for now
+        _app.include_router(self.agents_router, tags=["Agents"])
+        _app.include_router(self.platform_router, tags=["Platform"])
 
-    async def close(self):
-        """
-        Close this subscriber.
+        return _app
 
-        It releases the associated Redis connection properly.
+    async def _process_task(self, task: Task) -> JSONResponse:
         """
-        if self.redis is not None:
-            await self.redis.close()
-
-
-#: A type that represents all JSON-compatible types
-JSONType = Union[str, int, float, bool, None, List[Any], Dict[str, Any]]
+        Execute a task and return the result as a JSON response.
 
+        :return: the JSON response
+        :raises InternalServerError: if the task execution fails
+        """
+        try:
+            result = await task.execute(self.agent)
+            return JSONResponse(
+                json.loads(json.dumps(result, default=serialize_piaf_object))
+            )
+        except Exception as e:
+            self.agent.logger.exception(e)
+            raise InternalServerError(detail=str(e)) from e
 
-def serialize_piaf_object(
-    o: Any,
-) -> JSONType:
-    """
-    Given a `piaf` object, convert it into a JSON-compatible object.
+    def add_agents_routes(self) -> None:
+        """Add routes to the `/agents` router."""
 
-    :param o: the piaf object to serialize
-    :return: a JSON-compatible object
-    :raise TypeError: the object can't be serialized
-    """
-    if isinstance(o, AID):
-        return {
-            "name": o.name,
-            "shortname": o.short_name,
-            "addresses": o.addresses,
-            "resolvers": [serialize_piaf_object(r) for r in o.resolvers],
-        }
-    if isinstance(o, Enum):
-        return o.name
-    if isinstance(o, AMSAgentDescription):
-        return {
-            "aid": serialize_piaf_object(o.name),
-            "state": serialize_piaf_object(o.state),
-            "owner": o.ownership,
-        }
-    if isinstance(o, EventRecord):
-        return {
-            "event": serialize_piaf_object(o.event),
-            "topics": [serialize_piaf_object(topic) for topic in o.topics],
-            "timestamp": o.timestamp,
-        }
-    if isinstance(o, Event):
-        return {
-            "source": o.source,
-            "type": o.type,
-            "data": json.loads(json.dumps(o.data, default=serialize_piaf_object)),
-        }
-    if isinstance(o, Topic):
-        return str(o)
-    if isinstance(o, ACLMessage):
-        return {
-            k: json.loads(json.dumps(v, default=serialize_piaf_object))
-            for k, v in o.__dict__.items()
-        }
-    return f"Unserializable object: {type(o)}"
+        @self.agents_router.post(
+            "",
+            status_code=status.HTTP_201_CREATED,
+            response_model=AIDModel,
+            response_description="The agent is created",
+            responses={
+                status.HTTP_400_BAD_REQUEST: {
+                    "model": ExceptionModel,
+                    "description": "The operation can't be performed.",
+                },
+            },
+        )
+        async def create_agent(
+            agent: AgentCreationDescriptionModel,
+        ):
+            """
+            Create and invoke an agent into the specified platform.
+
+            **Body** the description of the agent to create
+            """
+            resp = await self._process_task(
+                CreateAgentTask(agent.to_agent_creation_description())
+            )
+            resp.status_code = status.HTTP_201_CREATED
+            return resp
 
+        @self.agents_router.get(
+            "",
+            response_description="Successfully returns the list of agents",
+            response_model=List[AMSAgentDescriptionModel],
+            responses={
+                status.HTTP_400_BAD_REQUEST: {
+                    "model": ExceptionModel,
+                    "description": "The operation can't be performed.",
+                },
+            },
+        )
+        async def get_agents(
+            state: Union[None, AgentState] = Query(
+                default=None,
+                description="Optionally filter results by only keeping agents with the given state.",
+                example="ACTIVE",
+            ),
+            name: Union[None, str] = Query(
+                default=None,
+                description="Optionally filter results by only keeping agents whose name contains the provided string.",
+                example="agent",
+            ),
+        ):
+            """Retrieve for the given platform all the agents matching the criteria."""
+            filters = {
+                "state": state.name if state is not None else None,
+                "name": name if name is not None else "",
+            }
+            return await self._process_task(GetAgentsTask(filters))
 
-class RedisConnectionPoolExtension(Extension):
-    """
-    An extension providing a pool of Redis connections.
+        @self.agents_router.delete(
+            "/{name}",
+            response_description="The agent is deleted",
+            status_code=status.HTTP_204_NO_CONTENT,
+            response_class=Response,
+            responses={
+                status.HTTP_400_BAD_REQUEST: {
+                    "model": ExceptionModel,
+                    "description": "The operation can't be performed.",
+                },
+            },
+        )
+        async def delete_agent(
+            name: str = Path(
+                description="The name of the agent to delete.", example="Custom-1"
+            ),
+        ):
+            """Delete an agent from the given platform."""
+            resp = await self._process_task(
+                ChangeAgentStateTask(name, AgentState.UNKNOWN)
+            )
+            resp.status_code = status.HTTP_204_NO_CONTENT
+            return resp
 
-    The user is responsible of closing its session (connection) once the work is finished.
-    """
+        @self.agents_router.get(
+            "/{name}",
+            response_model=AgentMemoryModel,
+            response_description="Successfully returns the agent's memory",
+            responses={
+                status.HTTP_400_BAD_REQUEST: {
+                    "model": ExceptionModel,
+                    "description": "The operation can't be performed.",
+                },
+            },
+        )
+        async def get_agent_memory(
+            name: str = Path(description="The name of the agent.", example="Custom-1"),
+        ):
+            """Get a snapshot of the current agent's memory."""
+            return await self._process_task(RetrieveAgentMemoryTask(name))
+
+        @self.agents_router.post(
+            "/{name}/messages",
+            status_code=status.HTTP_201_CREATED,
+            response_description="Successfully sent the message",
+            responses={
+                status.HTTP_400_BAD_REQUEST: {
+                    "model": ExceptionModel,
+                    "description": "The operation can't be performed.",
+                },
+            },
+        )
+        async def send_message(
+            msg: ACLMessageModel,
+            name: str = Path(description="The name of the agent.", example="Custom-1"),
+        ):
+            """Send a message on the behalf of a specific agent."""
+            resp = await self._process_task(
+                SendMessageTask(self.agent.aid, msg.to_acl_message(self.agent.aid))
+            )
+            resp.status_code = status.HTTP_201_CREATED
+            return resp
 
-    def __init__(
-        self, settings: Settings
-    ) -> None:  # TODO: use custom settings, not app ones
-        """
-        Create a new :class:`RedisConnectionPoolExtension` instance.
+        @self.agents_router.put(
+            "/{name}/state",
+            response_description="Successfully updated the agent's state",
+            responses={
+                status.HTTP_400_BAD_REQUEST: {
+                    "model": ExceptionModel,
+                    "description": "The operation can't be performed.",
+                },
+            },
+        )
+        async def update_agent_state(
+            state: AgentStateModel,
+            name: str = Path(description="The name of the agent.", example="Custom-1"),
+        ):
+            """Replace an agent's state by the provided one."""
+            return await self._process_task(ChangeAgentStateTask(name, state.state))
+
+    def add_platform_routes(self) -> None:
+        """Add routes to the `/platform` router."""
+
+        @self.platform_router.delete(
+            "",
+            response_description="The platform is deleted",
+            status_code=status.HTTP_204_NO_CONTENT,
+            response_class=Response,
+            responses={
+                status.HTTP_400_BAD_REQUEST: {
+                    "model": ExceptionModel,
+                    "description": "The operation can't be performed.",
+                },
+            },
+        )
+        async def stop_platform():
+            """Stop the platform."""
+            resp = await self._process_task(StopPlatformTask())
+            resp.status_code = status.HTTP_204_NO_CONTENT
+            return resp
+
+        @self.platform_router.websocket("/ws")
+        async def topic_listener(
+            websocket: WebSocket,
+        ) -> None:
+            """
+            Get a websocket that can listen on the platform's event.
 
-        The pool is not bound.
+            The websocket supports two methods:
 
-        :param settings: application settings used to setup the pool.
-        """
-        self._settings = settings
-        self._pool: ConnectionPool | None
+            - subscribe: subscribe to a particular topic
+            - unsubscribe: unsubscribe from a particular topic
 
-    async def on_start(self) -> None:
-        """
-        Initialize the pool and test the connection.
+            Here is the Json object::
 
-        :raise RedisError: Unable to establish a connection to Redis.
-        """
-        options: Dict[str, Any] = {
-            "decode_responses": True,
-            "max_connections": self._settings.redis_max_connections,
-        }
-        if self._settings.redis_user and self._settings.redis_password:
-            options.update(
                 {
-                    "username": self._settings.redis_user,
-                    "password": self._settings.redis_password,
+                    method: "[un]subscribe",
+                    topic: ".some.topic"
                 }
-            )
-        if self._settings.redis_db:
-            options["db"] = self._settings.redis_db
 
-        self._pool = aioredis.ConnectionPool.from_url(
-            f"{self._settings.redis_scheme}://{self._settings.redis_host}", **options
-        )
+            .. warning:: Contrary to how events are dispatched inside the piaf platform, events are not dispatched to topic's parents. It means that listening on `.platform` won't catch events emitted on `.platform.agents` for example.
 
-        try:
-            client: Redis = self.client
-            await client.ping()  # Ping to test the connection
-            await client.close()
-        except Exception as e:
-            await client.close()
-            if self._pool is not None:
-                await self._pool.disconnect()
-            raise RedisError() from e
-
-    async def on_stop(self) -> None:
-        """Disconnect all connections and close the pool."""
-        if self._pool is not None:
-            await self._pool.disconnect()
-
-    @property
-    def client(self) -> Redis:
-        """
-        Get a Redis session.
-
-        :raise RedisConnectionNotInitialized: the pool is not bound yet.
-        :return: a session
-        """
-        if self._pool is None:
-            raise RedisConnectionNotInitialized()
-        return Redis(connection_pool=self._pool)
+            :param ptf_name: the platform's name
+            :param websocket: injected by FastAPI
+            :param redis_session: a Redis session, injected by FastAPI
+            """
+
+            try:
+                await websocket.accept()
+                subscriber = WebsocketSubscriber(websocket)
+
+                while True:
+                    try:
+                        data: Dict[str, Any] = await websocket.receive_json()
+                    except WebSocketDisconnect:
+                        break
+
+                    topic = Topic.from_str(data["topic"])
+                    if data["method"] == "subscribe":
+                        self.agent._platform.evt_manager.subscribe_to(subscriber, topic)
+                        subscriber.topics.add(topic)
+
+                    if data["method"] == "unsubscribe":
+                        self.agent._platform.evt_manager.unsubscribe_from(
+                            subscriber, topic
+                        )
+                        subscriber.topics.remove(topic)
+            finally:
+                for topics in subscriber.topics:
+                    self.agent._platform.evt_manager.unsubscribe_from(
+                        subscriber, topics
+                    )
 
 
-class AgentPlatformProcess(Process):
-    """A customized process that runs a :class:`piaf.ptf.AgentPlatform` on a local asynchronous loop."""
+class WebsocketSubscriber(Subscriber):
+    """
+    A subscriber that can listen on a websocket and yield events to it.
+    """
 
-    def __init__(self, name: str, settings: Settings) -> None:
+    def __init__(self, websocket: WebSocket):
         """
-        Create a new instance.
+        Initialize a websocket subscriber.
 
-        :param name: name of the platform, which will also be the name of the thread.
+        :param agent: the agent
+        :param websocket: the websocket
         """
-        super().__init__(name=name, daemon=True)
-        self._settings = settings
+        self._websocket = websocket
+        self.topics: set[Topic] = set()
 
-    def run(self) -> None:
+    async def on_event(self, event_record: EventRecord) -> None:
         """
-        Create the asynchronous loop and launch the platform.
+        Yield the event to the websocket.
 
-        The platform will start with an agent called 'api', which can receive tasks
-        from a web interface to execute. For now, logs are streamed in the parent's
-        console (if any).
+        :param event: the event
         """
-        self.loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(self.loop)
-
-        import logging
-
-        logger = logging.getLogger()
-        logger.setLevel(logging.INFO)
-
-        handler = logging.StreamHandler()
-        handler.setFormatter(
-            logging.Formatter("{processName} - {levelname:<8}:{message}", style="{")
+        await self._websocket.send_json(
+            json.loads(json.dumps(event_record, default=serialize_piaf_object))
         )
-        logger.addHandler(handler)
 
-        self.launcher = PlatformLauncher(self.name)
-        self.launcher.add_extension(
-            "redis", RedisConnectionPoolExtension(self._settings)
-        )
-        self.launcher.add_service(ServiceDescription("api", APIAgent))
-
-        self.launcher.ptf.evt_manager.subscribe_to(
-            EventsToRedis(self.launcher.ptf),
-            Topic.from_str(""),
-        )
-
-        self.launcher.run()
+    async def close(self):
+        """Close the websocket."""
+        await self._websocket.close()
```

### Comparing `piaf-0.2.1/src/piaf/api/models.py` & `piaf-0.3.0b1/src/piaf/api/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 # coding: utf-8
 """
 The :mod:`piaf.api.models` contains all `pydantic` models used to describe input and output data.
-
-Every input models finish with the `In` suffix, while output models finish with the `Out` suffix.
 """
 from __future__ import annotations
 
+import json
+from enum import Enum
 from typing import Any, Dict, List, Optional, Union
+from uuid import uuid4
 
 from pydantic import BaseModel, Field, conlist, validator
 
 from piaf.agent import AgentState
-from piaf.comm import Performative
-
-
-class AgentPlatformModel(BaseModel):
-    """
-    Describe an incoming agent platform.
-
-    It only contains one field named 'name', witch represents the platform's name to create.
-    """
-
-    name: str = Field(description="The name of the platform")
-
-    class Config:
-        """Extra configuration added to the model."""
-
-        schema_extra = {"example": {"name": "my-awesome-platform"}}
+from piaf.audit import Event, EventRecord, Topic
+from piaf.comm import AID, ACLMessage, Performative
+from piaf.service import AgentCreationDescription, AMSAgentDescription
 
 
 class AgentCreationDescriptionModel(BaseModel):
     """
     Describe an incoming agent description.
 
     It should be supplied by the user in order to create an invoke an agent into a platform. The model contains four fields:
@@ -59,14 +47,27 @@
                 "class_name": "custom.agents.MyCustomAgent",
                 "agent_name": "Custom-1",
                 "args": ["a-star", 3],
                 "is_service": False,
             }
         }
 
+    def to_agent_creation_description(self) -> AgentCreationDescription:
+        """
+        Convert the model into an :class:`AgentCreationDescription`.
+
+        :return: the agent creation description
+        """
+        return AgentCreationDescription(
+            class_name=self.class_name,
+            agent_name=self.agent_name,
+            args=self.args,
+            is_service=self.is_service,
+        )
+
 
 class AIDModel(BaseModel):
     """
     Describe an agent identifier.
 
     The model contains four fields:
 
@@ -75,19 +76,19 @@
     - resolvers: a list of naming resolvers
     """
 
     name: str = Field(
         description="The full name of the agent (format: shortname@ptf_name)",
         regex=r".*@.*",
     )
-    addresses: conlist(str, unique_items=True) = Field(
+    addresses: conlist(str, unique_items=True) = Field(  # type: ignore
         default=[],
         description="A set of addresses with which the agent can be reached.",
     )
-    resolvers: conlist(AIDModel, unique_items=True) = Field(
+    resolvers: conlist(AIDModel, unique_items=True) = Field(  # type: ignore
         default=[],
         description="A set of agents that can resolve this agent's name.",
     )
 
     class Config:
         """Extra configuration added to the model."""
 
@@ -101,14 +102,17 @@
                         "addresses": ["amqp://my-awesome-platform/acc"],
                         "resolvers": [],
                     }
                 ],
             }
         }
 
+    def to_aid(self) -> AID:
+        return AID(self.name, self.addresses, [r.to_aid() for r in self.resolvers])
+
 
 AIDModel.update_forward_refs()
 
 
 class AMSAgentDescriptionModel(BaseModel):
     """
     Describe an agent when requested using the AMS.
@@ -195,15 +199,15 @@
     - `receivers`: a non-empty list of :class:`AIDModel` objects
     - `performative`: the message's performative
     - `conversation_id`: an optional conversation ID to track the conversation
     - `content`: a JSON-serializable message's content
 
     """
 
-    receivers: conlist(AIDModel, min_items=1, unique_items=True) = Field(
+    receivers: conlist(AIDModel, min_items=1, unique_items=True) = Field(  # type: ignore
         description="A set of AIDs, each one being the identity of a recipient."
     )
     performative: Union[Performative, str] = Field(
         description="The performative of the message."
     )
     conversation_id: Optional[str] = Field(
         default=None,
@@ -227,14 +231,28 @@
                 ],
                 "performative": "request",
                 "conversation_id": "talk#3",
                 "content": {"title": "Hello!", "repeat": 3},
             }
         }
 
+    def to_acl_message(self, sender: AID) -> ACLMessage:
+        return (
+            ACLMessage.Builder()
+            .performative(self.performative)
+            .receiver([r.to_aid() for r in self.receivers])
+            .conversation_id(
+                self.conversation_id
+                if self.conversation_id is not None
+                else str(uuid4())
+            )
+            .content(self.content)
+            .build()
+        )
+
 
 class AgentMemoryModel(BaseModel):
     """
     The response model used when the client asks for a snapshot of an agent's memory.
 
     This model contains two fields:
 
@@ -267,7 +285,58 @@
                         "addresses": [],
                         "resolvers": [],
                     },
                     "state": "ACTIVE",
                 },
             }
         }
+
+
+#: A type that represents all JSON-compatible types
+JSONType = Union[str, int, float, bool, None, List[Any], Dict[str, Any]]
+
+
+def serialize_piaf_object(
+    o: Any,
+) -> JSONType:
+    """
+    Given a `piaf` object, convert it into a JSON-compatible object.
+
+    :param o: the piaf object to serialize
+    :return: a JSON-compatible object
+    :raise TypeError: the object can't be serialized
+    """
+    if isinstance(o, AID):
+        return {
+            "name": o.name,
+            "shortname": o.short_name,
+            "addresses": o.addresses,
+            "resolvers": [serialize_piaf_object(r) for r in o.resolvers],
+        }
+    if isinstance(o, Enum):
+        return o.name
+    if isinstance(o, AMSAgentDescription):
+        return {
+            "aid": serialize_piaf_object(o.name),
+            "state": serialize_piaf_object(o.state),
+            "owner": o.ownership,
+        }
+    if isinstance(o, EventRecord):
+        return {
+            "event": serialize_piaf_object(o.event),
+            "topics": [serialize_piaf_object(topic) for topic in o.topics],
+            "timestamp": o.timestamp,
+        }
+    if isinstance(o, Event):
+        return {
+            "source": o.source,
+            "type": o.type,
+            "data": json.loads(json.dumps(o.data, default=serialize_piaf_object)),
+        }
+    if isinstance(o, Topic):
+        return str(o)
+    if isinstance(o, ACLMessage):
+        return {
+            k: json.loads(json.dumps(v, default=serialize_piaf_object))
+            for k, v in o.__dict__.items()
+        }
+    return f"Unserializable object: {type(o)}"
```

### Comparing `piaf-0.2.1/src/piaf/audit.py` & `piaf-0.3.0b1/src/piaf/audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         """
         Called when an event is published on a topic this subscriber is listening to.
 
         :param event_record: the :class:`EventRecord` that wraps the published event.
         """
         raise NotImplementedError()
 
-    async def close(self):
+    async def close(self) -> None:
         """
         Close this subscriber by performing cleanup.
 
         Default implementation does nothing.
         """
         pass
 
@@ -299,14 +299,32 @@
         if isinstance(topics, Topic):
             topics = [topics]
 
         for topic in topics:
             subscribers = self._subscribers.setdefault(topic, set())
             subscribers.add(subscriber)
 
+    def unsubscribe_from(
+        self, subscriber: Subscriber, topics: Topic | Iterable[Topic]
+    ) -> None:
+        """
+        Unbind the given subscriber from the provided list of topics.
+
+        After this call, the subscriber will no longer get notified when an event is published on one of the given topics.
+
+        :param subscriber: the subscriber to unbind
+        :param topics: either a :class:`Topic` or a list of topics that will be unbound from the subscriber
+        """
+        if isinstance(topics, Topic):
+            topics = [topics]
+
+        for topic in topics:
+            subscribers = self._subscribers.setdefault(topic, set())
+            subscribers.remove(subscriber)
+
     async def close(self) -> None:
         """
         Close the :class:`EventManager` and give a chance to subscribers to cleanup.
         """
         # Wait until synchronous publishes are done
         if self._tasks:
             await asyncio.wait(self._tasks, return_when=asyncio.ALL_COMPLETED)
```

### Comparing `piaf-0.2.1/src/piaf/behavior.py` & `piaf-0.3.0b1/src/piaf/behavior.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 Behaviors are small execution units that run "concurrently": several behaviors can be
 active at the same time but only one is executed per agent.
 
 Behaviors have access to the agent they are bounded to and are the preferred way to
 manipulate it, like updating its knowledge, sending or receiving messages.
 """
 from __future__ import annotations
+
 import abc
 import asyncio
 import logging
-
-from typing import Any, Callable, Dict, Type, Optional
+from typing import Any, Callable, Dict, Optional, Type
 
 import piaf.agent
 
-
 __all__ = ["Behavior", "CyclicBehavior", "FSMBehavior"]
 
 
 class Behavior(metaclass=abc.ABCMeta):
     """
     Base class user behaviors.
```

### Comparing `piaf-0.2.1/src/piaf/comm/__init__.py` & `piaf-0.3.0b1/src/piaf/comm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,23 @@
 """
 This module contains the building blocks of Agent Communication.
 
 The first block is the agent identity, called :class:`AID`. It is unique to each agent.
 Then comes :class:`ACLMessage` and templates.
 """
 from __future__ import annotations
-from dataclasses import dataclass
+
+import abc
+import copy
 import datetime
 import enum
-import abc
 import functools
 import operator
-import copy
-
-from typing import (
-    Dict,
-    List,
-    Optional,
-    Sequence,
-    MutableMapping,
-    Union,
-    Any,
-    Type,
-)
+from dataclasses import dataclass
+from typing import Any, Dict, List, MutableMapping, Optional, Sequence, Type, Union
 
 import piaf.exceptions
 
 __all__ = [
     "AID",
     "Performative",
     "ACLMessage",
```

### Comparing `piaf-0.2.1/src/piaf/comm/mtp/amqp.py` & `piaf-0.3.0b1/src/piaf/comm/mtp/amqp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # coding: utf-8
 """This module enables communication between platforms using the AMQP 0.9.1 protocol."""
 from __future__ import annotations
 
 import asyncio
 import logging
 import pickle
+from typing import cast
+
+from piaf.extensions.amqp import AMQPExtension
 
 try:
     import aiormq
     import aiormq.abc
     from aiormq import PublishError
     from yarl import URL
 except ImportError as e:
@@ -19,31 +22,30 @@
 from piaf.comm.mts import MessageContext, MessageTransportProtocol
 
 
 class AMQPMessageTransportProtocol(MessageTransportProtocol):
     """
     A MTP implementation enabling communications using the AMQP 0.9.1 protocol.
 
-    This MTP is built on asyncio and runs on the same thread as the platform. It first
-    establishes a connection with an AMQP server and then:
+    This MTP is built on asyncio and runs on the same thread as the platform. It first establishes a connection with an AMQP server and then:
 
         - use (and create if necessary) an exchange called "acc" in direct mode
         - bind an unnamed queue on it, using the platform name as routing key
 
     Messages are published on the "acc" exchange, using the destination platform name as routing key.
     """
 
-    def __init__(self, amqp_server_url: str) -> None:
+    def __init__(self, amqp_ext_name: str) -> None:
         """
         Initialize a new instance of :class:`AMQPMessageTransferProtocol`.
 
-        :param amqp_server_url: URL to the AMQP server this connector will connect to.
+        :param amqp_ext_name: the name of the AMQP extension to use
         """
         super().__init__()
-        self._server_url = amqp_server_url
+        self._ext_name = amqp_ext_name
         self._listening_condition = asyncio.Condition()
         self._listening_flag = False
         self.logger = logging.getLogger(type(self).__name__)
 
     @property
     def scheme(self) -> str:
         """
@@ -73,16 +75,15 @@
 
     async def send(self, message: Message, address: str) -> bool:
         """
         Send the provided message to the provided address (expected to be an amqp one).
 
         :param message: the message to send
         :param address: the amqp address of the other platform's ACC
-        :return: `True` if the message is sent, `False` if the provided address is not an AMQP
-            one or the MTP is unable to deliver the message to the remote platform.
+        :return: `True` if the message is sent, `False` if the provided address is not an AMQP one or the MTP is unable to deliver the message to the remote platform.
         """
         parsed_url = URL(address)
         if parsed_url.scheme != self.scheme:
             return False
 
         rt_key = parsed_url.host
         if rt_key is None:
@@ -117,25 +118,23 @@
         await self._connect()
         self.listener = asyncio.create_task(self._listen())
 
     async def stop(self) -> None:
         """
         Stop this MTP.
 
-        Cancel the listening task and close the connection with the AMQP server.
+        Cancel the listening task and close the channel with the AMQP server.
         """
         self.listener.cancel()
         await self.channel.close()
-        await self.connection.close()
 
     async def _connect(self) -> None:
-        """Establish the connection with the AMQP server and create a channel."""
-        # Create channel
-        self.connection = await aiormq.connect(URL(self._server_url))
-        self.channel = await self.connection.channel()
+        """Open a channel to the AMQP server."""
+        ext = cast(AMQPExtension, self.acc._ptf.extensions[self._ext_name])
+        self.channel = await ext.channel()
 
     async def _listen(self) -> None:
         """A long running task that listens on incoming messages and transfer them to the ACC."""
         # Declare exchange & random queue
         await self.channel.exchange_declare(exchange="acc", exchange_type="direct")
         declare_ok = await self.channel.queue_declare(
             durable=False, exclusive=True, auto_delete=True
```

### Comparing `piaf-0.2.1/src/piaf/comm/mts.py` & `piaf-0.3.0b1/src/piaf/comm/mts.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     Tuple,
     Type,
     Union,
 )
 
 import piaf.comm
 import piaf.exceptions as ex
-from piaf.comm import AID, ACLMessage, Envelope, Message, Performative, ReceivedObject
 from piaf.audit import ACC_TOPIC, AGENTS_PARENT_TOPIC, Event, Topic
+from piaf.comm import AID, ACLMessage, Envelope, Message, Performative, ReceivedObject
 
 if TYPE_CHECKING:
     from piaf.ptf import AgentPlatform
 
 from piaf.exceptions import DuplicatedNameException
 
 __all__ = [
@@ -119,28 +119,34 @@
             self._sync.notify_all()
 
 
 class MailBoxDelegate:
     """
     Delegation to internal agent or service mailbox.
 
-    Restrict access to agent/service mailbox. Only exposed method is :meth:`MailBox.put`.
+    Restrict access to agent/service mailbox. Only exposed methods are :meth:`MailBox.get` and :meth:`Mailbox.get_nowait`.
     """
 
     def __init__(self, delegate: MailBox) -> None:
         """
         Create a new :class:`MailBoxDelegate` object.
 
         :param delegate: agent's mailbox
         """
         self._delegate: MailBox = delegate
 
-    async def put(self, item: piaf.comm.Message) -> None:
-        """Put the provided message in this mailbox."""
-        await self._delegate.put(item)
+    async def get(
+        self, template: piaf.comm.MessageTemplate = piaf.comm.MT_ALL()
+    ) -> piaf.comm.Message:
+        return await self._delegate.get(template)
+
+    async def get_nowait(
+        self, template: piaf.comm.MessageTemplate = piaf.comm.MT_ALL()
+    ) -> Union[None, piaf.comm.Message]:
+        return await self._delegate.get_nowait(template)
 
 
 class PlayloadParser(metaclass=abc.ABCMeta):
     """Abstract playload parser. Use concrete classes to load or dump playload."""
 
     _PARSERS: ClassVar[Dict[str, Type[PlayloadParser]]] = {}
     _COMPONENT_NAME: ClassVar[str] = ""
@@ -436,15 +442,20 @@
 
         try:
             reply_msg = (
                 ACLMessage.Builder()
                 .performative(Performative.FAILURE)
                 .receiver(msg.acl_message.sender)
                 .conversation_id(msg.acl_message.conversation_id)
-                .content([msg.acl_message.content, f"Unreachable agent: {msg.acl_message.receiver}"])
+                .content(
+                    [
+                        msg.acl_message.content,
+                        f"Unreachable agent: {msg.acl_message.receiver}",
+                    ]
+                )
                 .build()
             )
             reply_msg.in_reply_to = msg.acl_message.reply_with
 
             reply_envlp = (
                 Envelope.Builder()
                 .from_(AID(f"ams@{self._ptf.name}", addresses=self.addresses))
@@ -471,15 +482,35 @@
 
     def __init__(self) -> None:
         """
         Default constructor which declares an attribute named `acc`.
 
         This attribute should be set by the :class:`AgentCommunicationChannel` at registration time.
         """
-        self.acc: None | AgentCommunicationChannel = None
+        self._acc: None | AgentCommunicationChannel = None
+
+    @property
+    def acc(self) -> AgentCommunicationChannel:
+        """
+        Get the ACC this MTP is registered to.
+
+        :return: the ACC this MTP is registered to.
+        """
+        if self._acc is None:
+            raise ValueError("MTP not registered to an ACC")
+        return self._acc
+
+    @acc.setter
+    def acc(self, acc: AgentCommunicationChannel) -> None:
+        """
+        Set the ACC this MTP is registered to.
+
+        :param acc: the ACC this MTP is registered to.
+        """
+        self._acc = acc
 
     @abc.abstractmethod
     async def send(self, message: Message, address: str) -> bool:
         """
         Send the provided message to the provided address.
 
         If the sending operation fails, the coroutine will return ``False``.
```

### Comparing `piaf-0.2.1/src/piaf/examples/benchmarks/empty_agents.py` & `piaf-0.3.0b1/src/piaf/examples/benchmarks/empty_agents.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # coding: utf-8
 from __future__ import annotations
 
 import asyncio
 from time import perf_counter_ns
 
-from piaf.ptf import AgentPlatform
 from piaf.agent import Agent
+from piaf.ptf import AgentPlatform
+
 
 async def main(n: int) -> None:
     ptf = AgentPlatform("localhost")
 
     async def _launch_agent(name: str) -> None:
-        aid = await ptf.agent_manager.create(
-            Agent, name
-        )
-        await ptf.agent_manager.invoke(aid) 
-
+        aid = await ptf.agent_manager.create(Agent, name)
+        await ptf.agent_manager.invoke(aid)
 
     await ptf.start()
-    
+
     t_start = perf_counter_ns()
     asyncio.gather(*(_launch_agent(f"aget-{i}") for i in range(n)))
     t_stop = perf_counter_ns()
-    
+
     await ptf.stop()
 
     print(f"Nb of agents: {n}; Elapsed time: {t_stop - t_start}ns")
 
+
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("n", metavar="NB_OF_AGENTS", help="How many agents to launch", type=int)
+    parser.add_argument(
+        "n", metavar="NB_OF_AGENTS", help="How many agents to launch", type=int
+    )
 
     parsed = parser.parse_args()
-    asyncio.run(main(parsed.n))
+    asyncio.run(main(parsed.n))
```

### Comparing `piaf-0.2.1/src/piaf/examples/heavycomm.py` & `piaf-0.3.0b1/src/piaf/examples/heavycomm.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # coding: utf-8
 """
 This example shows heavy exchanges between agents.
 
 One sender with a bunch of receivers. Time elapsed between sending and receiving is displayed.
 """
 from __future__ import annotations
+
 import time
+from typing import Sequence
 
-import piaf.comm
 import piaf.agent
 import piaf.behavior
-
-from typing import Sequence
+import piaf.comm
 
 
 class HeavySenderBehavior(piaf.behavior.Behavior):
     """
     Behavior for the sender agent.
 
     It builds a message containing the current time and send it to other agents.
@@ -86,17 +86,17 @@
         self.add_behavior(ReceiveBehavior(self))
 
 
 if __name__ == "__main__":
     import logging
     from typing import List
 
-    import piaf.ptf
-    import piaf.launcher
     import piaf.comm
+    import piaf.launcher
+    import piaf.ptf
 
     # Create the launcher
     launcher = piaf.launcher.PlatformLauncher("localhost")
 
     # Add receivers
     receivers: List[piaf.comm.AID] = []
     for i in range(100):
```

### Comparing `piaf-0.2.1/src/piaf/examples/helloworld.py` & `piaf-0.3.0b1/src/piaf/examples/helloworld.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 This module defines:
 
  * An agent, called CustomAgent
  * One behavior, called HelloWorldBehavior
  * It also show how to launch the platform.
 """
 import piaf.agent as agent
-
 from piaf.behavior import Behavior
 
 
 class HelloWorldBehavior(Behavior):
     """A behavior that uses the agent's logger to display an Hello World message."""
 
     async def action(self):
@@ -31,15 +30,16 @@
         # Create an instance of HelloWorldBehavior and add it to the agent
         b = HelloWorldBehavior(self)
         self.add_behavior(b)
 
 
 if __name__ == "__main__":
     import logging
-    from piaf.launcher import PlatformLauncher, AgentDescription
+
+    from piaf.launcher import AgentDescription, PlatformLauncher
 
     # Configure logging level and handler to see things
     logging.getLogger().setLevel(logging.INFO)
     logging.getLogger().addHandler(logging.StreamHandler())
 
     # Create the platform launcher
     launcher = PlatformLauncher("localhost")
```

### Comparing `piaf-0.2.1/src/piaf/examples/pingpong.py` & `piaf-0.3.0b1/src/piaf/examples/pingpong.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # coding: utf-8
 from piaf.agent import Agent
-from piaf.comm import AID
-from piaf.comm import ACLMessage, Performative
 from piaf.behavior import Behavior, FSMBehavior
+from piaf.comm import AID, ACLMessage, Performative
 
 
 class SendMsgBehavior(Behavior):
     """A simple behavior that sends messages."""
 
     def __init__(self, agent, msg, *args, **kwargs):
         """
@@ -128,14 +127,15 @@
 
         bhv.set_initial_state("RCV")
         self.add_behavior(bhv)
 
 
 if __name__ == "__main__":
     import logging
+
     from piaf.launcher import AgentDescription, PlatformLauncher
 
     # Configure logging level and handler to see things
     logging.getLogger().setLevel(logging.DEBUG)
     logging.getLogger().addHandler(logging.StreamHandler())
 
     # Create platform launcher
```

### Comparing `piaf-0.2.1/src/piaf/examples/two_platforms/ptf1.py` & `piaf-0.3.0b1/src/piaf/examples/two_platforms/ptf1.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,31 +11,33 @@
 .. note: In order to run this example, you will have to setup an AMQP server. Using Docker and RabbitMQ,
     you can easily launch the example: `docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.9-management-alpine`
 
 Once the server is ready, just run `python ptf2.py` in one terminal and then `python ptf1.py` in another. If the example
 works, you should see in the ptf2 terminal the message sent by the ptf1 agent.
 """
 from __future__ import annotations
+
 import asyncio
 from typing import Any
 
 from piaf.agent import Agent, AgentState
-from piaf.ptf import AgentPlatformFacade
-from piaf.service import AMSService, AMSAgentDescription
 from piaf.behavior import Behavior, FSMBehavior, SuicideBehavior
 from piaf.comm import (
     AID,
     MT_AND,
     MT_CONVERSATION_ID,
     MT_OR,
     MT_PERFORMATIVE,
     ACLMessage,
     Message,
     Performative,
 )
+from piaf.extensions.amqp import AMQPExtension, AMQPExtensionSettings
+from piaf.ptf import AgentPlatformFacade
+from piaf.service import AMSAgentDescription, AMSService
 
 
 class SendMsgBehavior(Behavior):
     """A simple behavior that sends messages."""
 
     def __init__(self, agent: Agent, msg: Message) -> None:
         """
@@ -166,27 +168,34 @@
         fsm.add_transition("FIND", "FIND", lambda found: not found)
         fsm.add_transition("FIND", "SEND", lambda found: found)
         fsm.add_transition("SEND", "DEATH", lambda e: True)
 
 
 if __name__ == "__main__":
     import logging
-    from piaf.launcher import AgentDescription, PlatformLauncher
+
     from piaf.comm.mtp.amqp import AMQPMessageTransportProtocol
+    from piaf.launcher import AgentDescription, PlatformLauncher
 
     # Configure logging level and handler to see things
     logging.getLogger().setLevel(logging.INFO)
     logging.getLogger().addHandler(logging.StreamHandler())
 
     # Create the platform launcher
     launcher = PlatformLauncher("ptf1")
 
+    # Add the AMQPExtension to the platform. This will allow the platform to use AMQP 0.9.1 communication.
+    launcher.add_extension(
+        "amqp",
+        AMQPExtension(AMQPExtensionSettings(url="amqp://guest:guest@localhost/")),
+    )
+
     # Register MTP. Since we want to connect this platform to another one, we need an MTP.
     # Here we are going to use the AMQPMessageTransferProtocol, which relies on AMQP 0.9.1 protocol.
-    launcher.add_mtp(AMQPMessageTransportProtocol("amqp://guest:guest@localhost/"))
+    launcher.add_mtp(AMQPMessageTransportProtocol("amqp"))
 
     # Now we can add our agent. The other agent AID is hardcode but we could use
     # the DF agent in a real case scenario to retrieve it.
     launcher.add_agent(
         AgentDescription(
             "my-agent",
             MyAgent,
```

### Comparing `piaf-0.2.1/src/piaf/examples/two_platforms/ptf2.py` & `piaf-0.3.0b1/src/piaf/examples/two_platforms/ptf2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 Once the server is ready, just run `python ptf2.py` in one terminal and `python ptf1.py` in another. If the example
 works, you should see in the ptf2 terminal the message sent by the ptf1 agent.
 """
 from piaf.agent import Agent
 from piaf.behavior import Behavior, FSMBehavior, SuicideBehavior
 from piaf.comm import AID
+from piaf.extensions.amqp import AMQPExtension, AMQPExtensionSettings
 from piaf.ptf import AgentPlatformFacade
 
 
 class RcvMsgBehavior(Behavior):
     """A simple behavior that receives messages and print them using the agent's logger."""
 
     async def action(self):
@@ -49,26 +50,33 @@
         fsm.set_initial_state("RCV")
 
         fsm.add_transition("RCV", "DEATH", lambda e: True)
 
 
 if __name__ == "__main__":
     import logging
-    from piaf.launcher import AgentDescription, PlatformLauncher
+
     from piaf.comm.mtp.amqp import AMQPMessageTransportProtocol
+    from piaf.launcher import AgentDescription, PlatformLauncher
 
     # Configure logging level and handler to see things
     logging.getLogger().setLevel(logging.INFO)
     logging.getLogger().addHandler(logging.StreamHandler())
 
     # Create platform launcher
     launcher = PlatformLauncher("ptf2")
 
-    # Since we want to connect this platform to another one, we need an MTP.
+    # Add the AMQPExtension to the platform. This will allow the platform to use AMQP 0.9.1 communication.
+    launcher.add_extension(
+        "amqp",
+        AMQPExtension(AMQPExtensionSettings(url="amqp://guest:guest@localhost/")),
+    )
+
+    # Register MTP. Since we want to connect this platform to another one, we need an MTP.
     # Here we are going to use the AMQPMessageTransferProtocol, which relies on AMQP 0.9.1 protocol.
-    launcher.add_mtp(AMQPMessageTransportProtocol("amqp://guest:guest@localhost/"))
+    launcher.add_mtp(AMQPMessageTransportProtocol("amqp"))
 
     # Now we can add our agent
     launcher.add_agent(AgentDescription("other", OtherAgent))
 
     # The program will run until you hit Ctrl+C
     launcher.run()
```

### Comparing `piaf-0.2.1/src/piaf/examples/useams.py` & `piaf-0.3.0b1/src/piaf/examples/useams.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 4. The receiving agents display the message
 
 It is possible that not all agents receives the message, since the broadcaster dies just after having sent its message
 to at least one active agent. So, if some receivers where not ready at the time the broadcaster queried the AMS, those
 agents won't receive the message.
 """
 from __future__ import annotations
+
 import asyncio
 from typing import TYPE_CHECKING, List
 
 from piaf.agent import Agent, AgentState
-from piaf.service import AMSService, AMSAgentDescription
+from piaf.behavior import Behavior
 from piaf.comm import (
+    AID,
     MT_CONVERSATION_ID,
     ACLMessage,
     Message,
     MessageTemplate,
     Performative,
-    AID,
 )
-from piaf.behavior import Behavior
+from piaf.service import AMSAgentDescription, AMSService
 
 if TYPE_CHECKING:
     from piaf.ptf import AgentPlatform, AgentPlatformFacade
 
 
 class SendHello(Behavior):
     """
@@ -79,15 +80,14 @@
         reply: Message = await self.agent.receive(mt)
         if reply.acl_message.performative != Performative.AGREE:
             return
 
         # If it succeeded, loop over content
         reply = await self.agent.receive(mt)
         if reply.acl_message.performative == Performative.INFORM:
-
             # Extract content
             content: List[AMSAgentDescription] = reply.acl_message.content[1]
 
             # No remaining agent, try again later
             if not content:
                 asyncio.sleep(1)
                 return
@@ -146,14 +146,15 @@
         super().__init__(aid, platform)
 
         self.add_behavior(DisplayReceivedMessage(self))
 
 
 if __name__ == "__main__":
     import logging
+
     from piaf.launcher import AgentDescription, PlatformLauncher
 
     # Configure logging level and handler to see things
     logging.getLogger().setLevel(logging.INFO)
     logging.getLogger().addHandler(logging.StreamHandler())
 
     # Create the platform launcher
```

### Comparing `piaf-0.2.1/src/piaf/examples/usedf.py` & `piaf-0.3.0b1/src/piaf/examples/usedf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # coding: utf-8
 """
 A small program testing the DF capabilities.
 
 This module defines a service called :class:`FIPAWebService` which can send HTML pages from the `FIPA Website(http://fipa.org)`_
 """
 from __future__ import annotations
+
 import asyncio
 from http.client import HTTPConnection, HTTPResponse
 
 from piaf.agent import Agent
 from piaf.behavior import Behavior
-from piaf.service import DFAgentDescription, DFService, ServiceDescription
 from piaf.comm import AID, MT_CONVERSATION_ID, ACLMessage, Performative
 from piaf.ptf import AgentPlatformFacade
+from piaf.service import DFAgentDescription, DFService, ServiceDescription
 from piaf.util import (
     FIPARequestProtocolBehavior,
     agree_message_from_request,
     inform_message_from_request,
     not_understood_message_from_request,
 )
 
@@ -215,14 +216,15 @@
         self.agent.logger.info(
             f"[{self.agent.aid.short_name}]: {response.acl_message.content}"
         )
 
 
 if __name__ == "__main__":
     import logging
+
     import piaf.launcher as pl
 
     # Configure logging level and handler to see things
     logging.getLogger().setLevel(logging.INFO)
     logging.getLogger().addHandler(logging.StreamHandler())
 
     # Create the platform launcher
```

### Comparing `piaf-0.2.1/src/piaf/exceptions.py` & `piaf-0.3.0b1/src/piaf/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf-8
 """Define all exceptions that are used in the piaf framework."""
 from __future__ import annotations
-from typing import Union, TYPE_CHECKING
+
+from typing import TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     import piaf.agent  # noqa
     import piaf.ptf as plt  # noqa
 
 __all__ = [
     "InvalidStateException",
```

### Comparing `piaf-0.2.1/src/piaf/launcher.py` & `piaf-0.3.0b1/src/piaf/launcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,14 +131,16 @@
             loop.run_until_complete(self._wait_platform_death())
         except KeyboardInterrupt:
             pass
         finally:
             loop.run_until_complete(self._cleanup())
             tasks = asyncio.all_tasks(loop)
             if tasks:
+                for task in tasks:
+                    task.cancel()
                 loop.run_until_complete(
                     asyncio.wait(tasks, return_when=asyncio.ALL_COMPLETED)
                 )
             loop.run_until_complete(loop.shutdown_asyncgens())
             loop.close()
 
     async def _cleanup(self) -> None:
@@ -159,24 +161,32 @@
         # AMS agent is created
         await self.ptf.start()
 
         # Then register all provided MTP instances
         asyncio.gather(*(self.ptf.acc.register_mtp(mtp) for mtp in self._mtps))
 
         # Then services
-        asyncio.gather(*(self._launch_agent(service, True) for service in self._services))
+        asyncio.gather(
+            *(self._launch_agent(service, True) for service in self._services)
+        )
 
         # Then agents
         asyncio.gather(*(self._launch_agent(agent, False) for agent in self._agents))
 
     async def _wait_platform_death(self) -> None:
         """Wait until the platform is stopped."""
         async with self.ptf.state_sync:
             await self.ptf.state_sync.wait_for(
                 lambda: self.ptf.state == PlatformState.STOPPED
             )
-    
-    async def _launch_agent(self, description: AgentDescription | ServiceDescription, is_service: bool) -> None:
+
+    async def _launch_agent(
+        self, description: AgentDescription | ServiceDescription, is_service: bool
+    ) -> None:
         aid = await self.ptf.agent_manager.create(
-            description.clazz, description.name, is_service, *description.args, **description.kwargs
+            description.clazz,
+            description.name,
+            is_service,
+            *description.args,
+            **description.kwargs,
         )
         await self.ptf.agent_manager.invoke(aid)
```

### Comparing `piaf-0.2.1/src/piaf/ptf.py` & `piaf-0.3.0b1/src/piaf/ptf.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,15 @@
         """
         await self._platform.agent_manager.suspend(agent)
 
     async def wait(self, agent: piaf.comm.AID) -> None:
         """
         Put an agent in WAITING state.
 
-        Even if it is possible to put in waiting state an other agent by providing
-        its AID, it should not be done.
+        The targetted agent can be the agent itself or another agent.
 
         :param agent: the AID of the agent
         """
         await self._platform.agent_manager.wait(agent)
 
     async def quit(self, agent: piaf.comm.AID) -> None:
         """
@@ -117,14 +116,25 @@
         state of the agent changed. This will get a shared condition on it. Only use
         with your agent's AID.
 
         :param agent: the agent's AID
         """
         return self._platform.agent_manager.get_state_condition(agent)
 
+    def get_mailbox(self, agent: piaf.comm.AID) -> piaf.comm.mts.MailBoxDelegate:
+        """
+        Get an agent's mailbox.
+
+        :param agent: the agent's identifier
+        :return: a small wrapper around the agent's mailbox allowing
+        """
+        return piaf.comm.mts.MailBoxDelegate(
+            self._platform.agent_manager.get_mailbox(agent)
+        )
+
     @property
     def name(self) -> str:
         """Get this platform's name."""
         return self._platform.name
 
     @property
     def evt_manager(self) -> EventManager:
@@ -166,14 +176,15 @@
 
     """
 
     def __init__(self, agent: piaf.agent.Agent):
         self.agent = agent
         self.state = piaf.agent.AgentState.INITIATED
         self.task: Optional[asyncio.Future[None]] = None
+        self.mailbox = piaf.comm.mts.MailBox()
         self.state_condition = asyncio.Condition()
 
 
 class AgentManager:
     """
     Object responsible of managing agents on a platform.
 
@@ -283,15 +294,15 @@
         # Create agent
         agent = agent_class(
             aid, AgentPlatformFacade(self._platform, is_service), *args, **kwargs
         )
         self._contexts[aid] = _AgentContext(agent)
 
         # Register agent to the ACC
-        self._acc.register_agent_or_service(short_name, agent.mailbox)  # type: ignore
+        self._acc.register_agent_or_service(short_name, self._contexts[aid].mailbox)  # type: ignore
 
         # Fire event
         await self._platform.evt_manager.publish(
             Event(aid.name, "agent_creation", aid),
             [
                 Topic.resolve_from_parent_topic(AGENTS_PARENT_TOPIC, aid.short_name),
                 AGENTS_PARENT_TOPIC,
@@ -482,14 +493,23 @@
         :param state: If provided, filter result and keep only agents having the given state.
         """
         agents = self._contexts.keys()
         if state is not None:
             agents = (agt for agt in agents if self.get_state(agt) == state)
         return [copy.deepcopy(agent) for agent in agents]
 
+    def get_mailbox(self, agent: piaf.comm.AID) -> piaf.comm.mts.MailBox:
+        """
+        Retrieve the agent's mailbox.
+
+        :param agent: the agent identifier
+        :return: the agent's mailbox
+        """
+        return self._contexts[agent].mailbox
+
 
 class Extension:
     """
     Extensions are additional functionalities loaded by the platform before anything else.
 
     They can be made available to all agents or only services (default). This interface defines the bare minimum any extension should implement.
     """
@@ -687,19 +707,19 @@
         Start the platform.
 
         The platform state will transition to ``RUNNING`` and the AMS agent will be
         started.
 
         :raise StateTransitionException: the platform's state is different from `INITIALIZED`
         """
-        if self._state != PlatformState.INITIALIZED:
-            raise ex.StateTransitionException(self._state, PlatformState.RUNNING)
-
-        # Set platform state
         async with self.state_sync:
+            if self._state != PlatformState.INITIALIZED:
+                raise ex.StateTransitionException(self._state, PlatformState.RUNNING)
+
+            # Set platform state
             self._state = PlatformState.RUNNING
             self.state_sync.notify_all()
 
         # Load extensions
         for _, ext in self.extensions.items():
             await ext.on_start()
 
@@ -722,30 +742,30 @@
         Stop this platform.
 
         It will stop all running agents (make them quit) and the platform's state will
         be ``STOPPED``.
 
         :raise StateTransitionException: the platform's state is different from `RUNNING`
         """
-        if self._state != PlatformState.RUNNING:
-            raise ex.StateTransitionException(self._state, PlatformState.STOPPED)
-
-        await self._agt_manager.stop_all()
-        await self._acc.stop()
+        async with self.state_sync:
+            if self._state != PlatformState.RUNNING:
+                raise ex.StateTransitionException(self._state, PlatformState.STOPPED)
 
-        # Stop extensions
-        for _, ext in self.extensions.items():
-            await ext.on_stop()
+            await self._agt_manager.stop_all()
+            await self._acc.stop()
 
-        if self._tasks:
-            for task in self._tasks:
-                task.cancel()
-            await asyncio.wait(self._tasks)
+            # Stop extensions
+            for _, ext in self.extensions.items():
+                await ext.on_stop()
+
+            if self._tasks:
+                for task in self._tasks:
+                    task.cancel()
+                await asyncio.wait(self._tasks)
 
-        async with self.state_sync:
             self._state = PlatformState.STOPPED
             self.state_sync.notify_all()
 
         # Schedule the publishing of the event rather than waiting it.
         # This is because some cleanup functions can be triggered by the state change
         # and close the loop before the event is published
         self.evt_manager.publish_sync(
```

### Comparing `piaf-0.2.1/src/piaf/service.py` & `piaf-0.3.0b1/src/piaf/service.py`

 * *Files identical despite different names*

### Comparing `piaf-0.2.1/src/piaf/util.py` & `piaf-0.3.0b1/src/piaf/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # coding: utf-8
 """Utility module."""
 # TODO: complete description
 from __future__ import annotations
+
 import asyncio
 from abc import ABCMeta, abstractmethod
+from typing import TYPE_CHECKING, Any, Dict
+
 from piaf.behavior import Behavior
-from piaf.comm import ACLMessage, MT_OR, MT_PERFORMATIVE, Performative
-from typing import Any, TYPE_CHECKING, Dict
+from piaf.comm import MT_OR, MT_PERFORMATIVE, ACLMessage, Performative
 
 if TYPE_CHECKING:
     import piaf.agent
 
 
 def not_understood_message_from_request(request: ACLMessage, reason: str) -> ACLMessage:
     """
@@ -184,15 +186,14 @@
         """
         # Get next handled message
         msg = await self.agent.receive(self.msg_template)
         acl_msg = msg.acl_message
 
         # Request -> new conversation
         if acl_msg.performative == Performative.REQUEST:
-
             # If message content is invalid, stop processing
             if not self.check_message(acl_msg):
                 return
 
             # Otherwise execute the user method
             self.tasks[acl_msg.conversation_id] = asyncio.create_task(
                 self.on_valid_request(acl_msg)
```

### Comparing `piaf-0.2.1/PKG-INFO` & `piaf-0.3.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piaf
-Version: 0.2.1
+Version: 0.3.0b1
 Summary: A FIPA-compliant Agent Platform written in python.
 Home-page: https://gitlab.com/ornythorinque/piaf
 License: MIT
 Keywords: Python Agent Framework,multi-agent,asyncio
 Author: Pierre DUBAILLAY
 Author-email: pierredubaillay@outlook.fr
 Requires-Python: >=3.7,<4
@@ -12,21 +12,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: amqp-mtp
+Provides-Extra: redis-mtp
 Provides-Extra: webapi
-Requires-Dist: aioredis (>=2,<3) ; extra == "webapi"
 Requires-Dist: aiormq (>=6,<7) ; extra == "amqp-mtp"
 Requires-Dist: async-timeout (>=4,<5) ; extra == "webapi"
-Requires-Dist: fastapi (>=0.92,<0.93) ; extra == "webapi"
+Requires-Dist: fastapi (>=0.95,<0.96) ; extra == "webapi"
+Requires-Dist: pydantic (>=1,<2) ; extra == "webapi"
 Requires-Dist: python-dotenv (>=0.21,<0.22)
+Requires-Dist: redis (>=4,<5) ; extra == "redis-mtp"
 Requires-Dist: semver (>=2,<3)
+Requires-Dist: uvicorn[standard] (>=0.22,<0.23) ; extra == "webapi"
 Requires-Dist: yarl (>=1,<2) ; extra == "amqp-mtp"
 Project-URL: Repository, https://gitlab.com/ornythorinque/piaf
 Description-Content-Type: text/markdown
 
 # Python Intelligent Agent Framework (piaf)
 
 ![pipeline status](https://gitlab.com/ornythorinque/piaf/badges/master/pipeline.svg)
```

