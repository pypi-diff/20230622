# Comparing `tmp/discordproxy-1.2.2.tar.gz` & `tmp/discordproxy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordproxy-1.2.2.tar", last modified: Sat Jun 18 19:02:41 2022, max compression
+gzip compressed data, was "discordproxy-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `discordproxy-1.2.2.tar` & `discordproxy-1.3.0.tar`

### file list

```diff
@@ -1,52 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-18 19:02:41.097628 discordproxy-1.2.2/
--rw-rw-rw-   0 root         (0) root         (0)      106 2021-12-29 22:39:16.000000 discordproxy-1.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2603 2022-06-18 19:02:41.097628 discordproxy-1.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1890 2021-03-13 18:29:37.000000 discordproxy-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-18 19:02:41.089628 discordproxy-1.2.2/discordproxy/
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-06-18 18:43:28.000000 discordproxy-1.2.2/discordproxy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2022-06-02 15:58:02.000000 discordproxy-1.2.2/discordproxy/_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2022-04-08 13:27:28.000000 discordproxy-1.2.2/discordproxy/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3802 2021-12-28 15:54:50.000000 discordproxy-1.2.2/discordproxy/_config.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2021-12-28 15:54:50.000000 discordproxy-1.2.2/discordproxy/_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2846 2021-12-29 19:54:56.000000 discordproxy-1.2.2/discordproxy/_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2021-12-28 15:54:50.000000 discordproxy-1.2.2/discordproxy/_discord_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3575 2021-12-29 20:20:01.000000 discordproxy-1.2.2/discordproxy/_server.py
--rw-rw-rw-   0 root         (0) root         (0)     4031 2021-12-29 20:20:01.000000 discordproxy-1.2.2/discordproxy/client.py
--rw-rw-rw-   0 root         (0) root         (0)    22890 2022-06-02 16:37:15.000000 discordproxy-1.2.2/discordproxy/discord_api_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5787 2021-03-10 20:17:15.000000 discordproxy-1.2.2/discordproxy/discord_api_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2611 2022-01-12 18:15:39.000000 discordproxy-1.2.2/discordproxy/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      733 2021-11-16 18:15:22.000000 discordproxy-1.2.2/discordproxy/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-18 19:02:41.093628 discordproxy-1.2.2/discordproxy/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-06 13:08:39.000000 discordproxy-1.2.2/discordproxy/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      919 2022-01-12 18:15:39.000000 discordproxy-1.2.2/discordproxy/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2021-12-29 20:20:01.000000 discordproxy-1.2.2/discordproxy/tests/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7700 2021-12-29 19:54:56.000000 discordproxy-1.2.2/discordproxy/tests/stubs.py
--rw-rw-rw-   0 root         (0) root         (0)     6027 2021-12-29 19:54:56.000000 discordproxy-1.2.2/discordproxy/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2022-01-12 18:15:39.000000 discordproxy-1.2.2/discordproxy/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4467 2021-12-28 15:54:50.000000 discordproxy-1.2.2/discordproxy/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2021-12-28 15:54:50.000000 discordproxy-1.2.2/discordproxy/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2022-06-02 12:56:22.000000 discordproxy-1.2.2/discordproxy/tests/test_end2end.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2022-01-12 18:15:39.000000 discordproxy-1.2.2/discordproxy/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2021-12-28 00:07:11.000000 discordproxy-1.2.2/discordproxy/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1875 2022-06-02 12:56:22.000000 discordproxy-1.2.2/discordproxy/tests/test_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-18 19:02:41.089628 discordproxy-1.2.2/discordproxy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2603 2022-06-18 19:02:40.000000 discordproxy-1.2.2/discordproxy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1214 2022-06-18 19:02:41.000000 discordproxy-1.2.2/discordproxy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-18 19:02:40.000000 discordproxy-1.2.2/discordproxy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      111 2022-06-18 19:02:40.000000 discordproxy-1.2.2/discordproxy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-06-18 19:02:40.000000 discordproxy-1.2.2/discordproxy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-06-18 19:02:40.000000 discordproxy-1.2.2/discordproxy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-18 19:02:41.093628 discordproxy-1.2.2/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-18 19:02:41.093628 discordproxy-1.2.2/examples/DiscordClient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-29 15:25:28.000000 discordproxy-1.2.2/examples/DiscordClient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2022-06-02 12:56:22.000000 discordproxy-1.2.2/examples/DiscordClient/hello_world.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-29 15:25:28.000000 discordproxy-1.2.2/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-18 19:02:41.093628 discordproxy-1.2.2/examples/gRPC/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-29 15:25:28.000000 discordproxy-1.2.2/examples/gRPC/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2022-06-02 12:56:22.000000 discordproxy-1.2.2/examples/gRPC/client.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2021-12-29 15:25:28.000000 discordproxy-1.2.2/examples/gRPC/hello_world.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2021-12-29 15:25:28.000000 discordproxy-1.2.2/examples/gRPC/load_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-18 19:02:41.093628 discordproxy-1.2.2/protobufs/
--rw-rw-rw-   0 root         (0) root         (0)     6736 2022-06-02 16:37:15.000000 discordproxy-1.2.2/protobufs/discord_api.proto
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-18 19:02:41.097628 discordproxy-1.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1591 2022-06-02 12:56:22.000000 discordproxy-1.2.2/setup.py
+-rw-r--r--   0        0        0     1070 2023-04-29 14:16:52.177131 discordproxy-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1890 2021-03-13 18:29:37.317667 discordproxy-1.3.0/README.md
+-rw-r--r--   0        0        0      110 2023-06-22 19:01:39.102674 discordproxy-1.3.0/discordproxy/__init__.py
+-rw-r--r--   0        0        0     5721 2023-06-22 17:58:52.090919 discordproxy-1.3.0/discordproxy/_api.py
+-rw-r--r--   0        0        0     1946 2022-04-08 13:27:28.023968 discordproxy-1.3.0/discordproxy/_cli.py
+-rw-r--r--   0        0        0     3802 2021-12-28 15:54:50.403316 discordproxy-1.3.0/discordproxy/_config.py
+-rw-r--r--   0        0        0       48 2021-12-28 15:54:50.407316 discordproxy-1.3.0/discordproxy/_constants.py
+-rw-r--r--   0        0        0     2846 2021-12-29 19:54:56.084119 discordproxy-1.3.0/discordproxy/_decorators.py
+-rw-r--r--   0        0        0      458 2021-12-28 15:54:50.407316 discordproxy-1.3.0/discordproxy/_discord_client.py
+-rw-r--r--   0        0        0     3575 2021-12-29 20:20:01.968360 discordproxy-1.3.0/discordproxy/_server.py
+-rw-r--r--   0        0        0     4031 2021-12-29 20:20:01.968360 discordproxy-1.3.0/discordproxy/client.py
+-rw-r--r--   0        0        0    24933 2023-06-22 14:14:27.248149 discordproxy-1.3.0/discordproxy/discord_api_pb2.py
+-rw-r--r--   0        0        0     5883 2023-06-22 14:14:27.248149 discordproxy-1.3.0/discordproxy/discord_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2611 2022-01-12 18:15:39.779155 discordproxy-1.3.0/discordproxy/exceptions.py
+-rw-r--r--   0        0        0      733 2021-11-16 18:15:22.015918 discordproxy-1.3.0/discordproxy/helpers.py
+-rw-r--r--   0        0        0     1394 2023-06-22 17:58:52.090919 discordproxy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 discordproxy-1.3.0/PKG-INFO
```

### Comparing `discordproxy-1.2.2/PKG-INFO` & `discordproxy-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: discordproxy
-Version: 1.2.2
-Summary: Proxy server for accessing the Discord API via gRPC
-Home-page: https://gitlab.com/ErikKalkoken/discordproxy
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Version: 1.3.0
+Summary: Proxy server for accessing the Discord API via gRPC.
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: grpcio-tools!=1.45.0
+Requires-Dist: py-cord>=2
+Project-URL: Documentation, https://django-eveuniverse.readthedocs.io/en/latest/
+Project-URL: Source, https://gitlab.com/ErikKalkoken/discordproxy
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/discordproxy/issues
 
 # discordproxy
 
 Proxy server for accessing the Discord API via gRPC
 
 [![release](https://img.shields.io/pypi/v/discordproxy?label=release)](https://pypi.org/project/discordproxy/)
 [![python](https://img.shields.io/pypi/pyversions/discordproxy)](https://pypi.org/project/discordproxy/)
@@ -40,8 +40,7 @@
 
 Python applications can import the generated gRPC client directly. Applications in other languages can use the protobuf definition to generate their own gRPC client.
 
 ## Documentation
 
 For more information please see the [documentation](https://discordproxy.readthedocs.io/en/latest/?badge=latest).
 
-
```

### Comparing `discordproxy-1.2.2/README.md` & `discordproxy-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `discordproxy-1.2.2/discordproxy/_api.py` & `discordproxy-1.3.0/discordproxy/_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,26 +31,23 @@
 #         id=role_tag.bot_id,
 #         integration_id=role_tag.integration_id,
 #         premium_subscriber=role_tag.is_premium_subscriber(),
 #     )
 
 
 def discord_to_grpc_message(message) -> discord_api_pb2.Message:
-    def user_avatar_adapter(user) -> str:
-        """Get user's avatar hash. Works with both old and new pycord API."""
-        version_info = discord.version_info
-        if version_info.major < 2:
-            return user.avatar  # works with pycord 1 only.
-        return user.avatar.key
-
+    try:
+        avatar = message.author.avatar.key
+    except AttributeError:
+        avatar = ""
     author = discord_api_pb2.User(
         id=message.author.id,
         username=message.author.name,
         discriminator=message.author.discriminator,
-        avatar=user_avatar_adapter(message.author),
+        avatar=avatar,
         bot=message.author.bot,
         system=message.author.system,
     )
     if isinstance(message.author, discord.Member):
         member = discord_api_pb2.GuildMember(
             user=author,
             nick=message.author.nick,
```

### Comparing `discordproxy-1.2.2/discordproxy/_cli.py` & `discordproxy-1.3.0/discordproxy/_cli.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.2.2/discordproxy/_config.py` & `discordproxy-1.3.0/discordproxy/_config.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.2.2/discordproxy/_decorators.py` & `discordproxy-1.3.0/discordproxy/_decorators.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.2.2/discordproxy/_server.py` & `discordproxy-1.3.0/discordproxy/_server.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.2.2/discordproxy/client.py` & `discordproxy-1.3.0/discordproxy/client.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.2.2/discordproxy/discord_api_pb2.py` & `discordproxy-1.3.0/discordproxy/discord_api_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,332 +3,419 @@
 # source: discord_api.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64iscord_api.proto\x12\x0b\x64iscord_api\"\xb1\x02\n\x07\x43hannel\x12\n\n\x02id\x18\x01 \x01(\x04\x12\'\n\x04type\x18\x02 \x01(\x0e\x32\x19.discord_api.Channel.Type\x12\x10\n\x08guild_id\x18\x03 \x01(\x04\x12\x10\n\x08position\x18\x04 \x01(\x05\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\r\n\x05topic\x18\x07 \x01(\t\x12\x0c\n\x04nsfw\x18\x08 \x01(\x08\x12\x17\n\x0flast_message_id\x18\t \x01(\x04\x12\x11\n\tparent_id\x18\n \x01(\x04\"v\n\x04Type\x12\r\n\tUNDEFINED\x10\x00\x12\x0e\n\nGUILD_TEXT\x10\x01\x12\x06\n\x02\x44M\x10\x02\x12\x0f\n\x0bGUILD_VOICE\x10\x03\x12\x0c\n\x08GROUP_DM\x10\x04\x12\x12\n\x0eGUILD_CATEGORY\x10\x05\x12\x0e\n\nGUILD_NEWS\x10\x06\"\x04\x08\x07\x10\x07\"\xee\x06\n\x05\x45mbed\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12\x11\n\ttimestamp\x18\x05 \x01(\t\x12\r\n\x05\x63olor\x18\x06 \x01(\x05\x12)\n\x06\x66ooter\x18\x07 \x01(\x0b\x32\x19.discord_api.Embed.Footer\x12\'\n\x05image\x18\x08 \x01(\x0b\x32\x18.discord_api.Embed.Image\x12/\n\tthumbnail\x18\t \x01(\x0b\x32\x1c.discord_api.Embed.Thumbnail\x12\'\n\x05video\x18\n \x01(\x0b\x32\x18.discord_api.Embed.Video\x12-\n\x08provider\x18\x0b \x01(\x0b\x32\x1b.discord_api.Embed.Provider\x12)\n\x06\x61uthor\x18\x0c \x01(\x0b\x32\x19.discord_api.Embed.Author\x12(\n\x06\x66ields\x18\r \x03(\x0b\x32\x18.discord_api.Embed.Field\x1a@\n\x06\x46ooter\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08icon_url\x18\x02 \x01(\t\x12\x16\n\x0eproxy_icon_url\x18\x03 \x01(\t\x1aK\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x16\n\x0eproxy_icon_url\x18\x02 \x01(\t\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\r\n\x05width\x18\x04 \x01(\x05\x1aJ\n\tThumbnail\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tproxy_url\x18\x02 \x01(\t\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\r\n\x05width\x18\x04 \x01(\x05\x1aK\n\x05Video\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x16\n\x0eproxy_icon_url\x18\x02 \x01(\t\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\r\n\x05width\x18\x04 \x01(\x05\x1a%\n\x08Provider\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x1aM\n\x06\x41uthor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x10\n\x08icon_url\x18\x03 \x01(\t\x12\x16\n\x0eproxy_icon_url\x18\x04 \x01(\t\x1a\x34\n\x05\x46ield\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0e\n\x06inline\x18\x03 \x01(\x08\"\xa0\x01\n\x05\x45moji\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\x04\x12\x1f\n\x04user\x18\x04 \x01(\x0b\x32\x11.discord_api.User\x12\x17\n\x0frequired_colons\x18\x05 \x01(\x08\x12\x0f\n\x07managed\x18\x06 \x01(\x08\x12\x10\n\x08\x61nimated\x18\x07 \x01(\x08\x12\x11\n\tavailable\x18\x08 \x01(\x08\"\xb7\x01\n\x0bGuildMember\x12\x1f\n\x04user\x18\x01 \x01(\x0b\x32\x11.discord_api.User\x12\x0c\n\x04nick\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\x04\x12\x11\n\tjoined_at\x18\x04 \x01(\t\x12\x15\n\rpremium_since\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x65\x61\x66\x18\x06 \x01(\x08\x12\x0c\n\x04mute\x18\x07 \x01(\x08\x12\x0f\n\x07pending\x18\x08 \x01(\x08\x12\x13\n\x0bpermissions\x18\t \x01(\t\"\x90\x11\n\x07Message\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x12\n\nchannel_id\x18\x02 \x01(\x04\x12\x10\n\x08guild_id\x18\x03 \x01(\x04\x12!\n\x06\x61uthor\x18\x04 \x01(\x0b\x32\x11.discord_api.User\x12(\n\x06member\x18\x05 \x01(\x0b\x32\x18.discord_api.GuildMember\x12\x0f\n\x07\x63ontent\x18\x06 \x01(\t\x12\x11\n\ttimestamp\x18\x07 \x01(\t\x12\x18\n\x10\x65\x64ited_timestamp\x18\x08 \x01(\t\x12\x0b\n\x03tts\x18\t \x01(\x08\x12\x18\n\x10mention_everyone\x18\n \x01(\x08\x12#\n\x08mentions\x18\x0b \x03(\x0b\x32\x11.discord_api.User\x12\x15\n\rmention_roles\x18\x0c \x03(\x04\x12\x18\n\x10mention_channels\x18\r \x03(\x04\x12\x34\n\x0b\x61ttachments\x18\x0e \x03(\x0b\x32\x1f.discord_api.Message.Attachment\x12\"\n\x06\x65mbeds\x18\x0f \x03(\x0b\x32\x12.discord_api.Embed\x12\x30\n\treactions\x18\x10 \x03(\x0b\x32\x1d.discord_api.Message.Reaction\x12\r\n\x05nonce\x18\x11 \x01(\t\x12\x0e\n\x06pinned\x18\x12 \x01(\x08\x12\x12\n\nwebhook_id\x18\x13 \x01(\x04\x12\'\n\x04type\x18\x14 \x01(\x0e\x32\x19.discord_api.Message.Type\x12/\n\x08\x61\x63tivity\x18\x15 \x01(\x0b\x32\x1d.discord_api.Message.Activity\x12\x35\n\x0b\x61pplication\x18\x16 \x01(\x0b\x32 .discord_api.Message.Application\x12\x39\n\x11message_reference\x18\x17 \x01(\x0b\x32\x1e.discord_api.Message.Reference\x12\r\n\x05\x66lags\x18\x18 \x01(\x05\x12.\n\x08stickers\x18\x19 \x03(\x0b\x32\x1c.discord_api.Message.Sticker\x12\x30\n\x12referenced_message\x18\x1a \x01(\x0b\x32\x14.discord_api.Message\x1a\x65\n\x0e\x43hannelMention\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x10\n\x08guild_id\x18\x02 \x01(\x04\x12\'\n\x04type\x18\x03 \x01(\x0e\x32\x19.discord_api.Channel.Type\x12\x0c\n\x04name\x18\x04 \x01(\t\x1aw\n\nAttachment\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x10\n\x08\x66ilename\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\x05\x12\x0b\n\x03url\x18\x04 \x01(\t\x12\x11\n\tproxy_url\x18\x05 \x01(\t\x12\x0e\n\x06height\x18\x06 \x01(\x05\x12\r\n\x05width\x18\x07 \x01(\x05\x1aH\n\x08Reaction\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\n\n\x02me\x18\x02 \x01(\x08\x12!\n\x05\x65moji\x18\x03 \x01(\x0b\x32\x12.discord_api.Emoji\x1a\x9c\x01\n\x08\x41\x63tivity\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".discord_api.Message.Activity.Type\x12\x10\n\x08party_id\x18\x02 \x01(\t\"L\n\x04Type\x12\r\n\tUNDEFINED\x10\x00\x12\x08\n\x04JOIN\x10\x01\x12\x0c\n\x08SPECTATE\x10\x02\x12\n\n\x06LISTEN\x10\x03\x12\x11\n\rJOIN_REQUESTS\x10\x04\x1a_\n\x0b\x41pplication\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x13\n\x0b\x63over_image\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04icon\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x1a\x61\n\tReference\x12\x12\n\nmessage_id\x18\x01 \x01(\x04\x12\x12\n\nchannel_id\x18\x02 \x01(\x04\x12\x10\n\x08guild_id\x18\x03 \x01(\x04\x12\x1a\n\x12\x66\x61il_if_not_exists\x18\x04 \x01(\x08\x1a\xeb\x01\n\x07Sticker\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x0f\n\x07pack_id\x18\x02 \x01(\x04\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x01(\t\x12\r\n\x05\x61sset\x18\x06 \x01(\t\x12\x15\n\rpreview_asset\x18\x07 \x01(\t\x12\x36\n\x0b\x66ormat_type\x18\x08 \x01(\x0e\x32!.discord_api.Message.Sticker.Type\"4\n\x04Type\x12\r\n\tUNDEFINED\x10\x00\x12\x07\n\x03PNG\x10\x01\x12\x08\n\x04\x41PNG\x10\x02\x12\n\n\x06LOTTIE\x10\x03\"\xd3\x03\n\x04Type\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x11\n\rRECIPIENT_ADD\x10\x01\x12\x14\n\x10RECIPIENT_REMOVE\x10\x02\x12\x08\n\x04\x43\x41LL\x10\x03\x12\x17\n\x13\x43HANNEL_NAME_CHANGE\x10\x04\x12\x17\n\x13\x43HANNEL_ICON_CHANGE\x10\x05\x12\x1a\n\x16\x43HANNEL_PINNED_MESSAGE\x10\x06\x12\x15\n\x11GUILD_MEMBER_JOIN\x10\x07\x12#\n\x1fUSER_PREMIUM_GUILD_SUBSCRIPTION\x10\x08\x12*\n&USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_1\x10\t\x12*\n&USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_2\x10\n\x12*\n&USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_3\x10\x0b\x12\x16\n\x12\x43HANNEL_FOLLOW_ADD\x10\x0c\x12 \n\x1cGUILD_DISCOVERY_DISQUALIFIED\x10\x0e\x12\x1f\n\x1bGUILD_DISCOVERY_REQUALIFIED\x10\x0f\x12\t\n\x05REPLY\x10\x13\x12\x17\n\x13\x41PPLICATION_COMMAND\x10\x14\"\xf7\x01\n\x04Role\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\x05\x12\r\n\x05hoist\x18\x04 \x01(\x08\x12\x10\n\x08position\x18\x05 \x01(\x05\x12\x13\n\x0bpermissions\x18\x06 \x01(\t\x12\x0f\n\x07managed\x18\x07 \x01(\x08\x12\x13\n\x0bmentionable\x18\x08 \x01(\x08\x12#\n\x04tags\x18\t \x03(\x0b\x32\x15.discord_api.Role.Tag\x1a\x45\n\x03Tag\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x16\n\x0eintegration_id\x18\x02 \x01(\x04\x12\x1a\n\x12premium_subscriber\x18\x03 \x01(\x08\"\xe9\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x15\n\rdiscriminator\x18\x03 \x01(\t\x12\x0e\n\x06\x61vatar\x18\x04 \x01(\t\x12\x0b\n\x03\x62ot\x18\x05 \x01(\x08\x12\x0e\n\x06system\x18\x06 \x01(\x08\x12\x13\n\x0bmfa_enabled\x18\x07 \x01(\x08\x12\x0e\n\x06locale\x18\x08 \x01(\t\x12\x10\n\x08verified\x18\t \x01(\x08\x12\r\n\x05\x65mail\x18\n \x01(\t\x12\r\n\x05\x66lags\x18\x0b \x01(\x05\x12\x14\n\x0cpremium_type\x18\x0c \x01(\x05\x12\x14\n\x0cpublic_flags\x18\r \x01(\x05\"c\n\x19SendChannelMessageRequest\x12\x12\n\nchannel_id\x18\x01 \x01(\x04\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12!\n\x05\x65mbed\x18\x03 \x01(\x0b\x32\x12.discord_api.Embed\"C\n\x1aSendChannelMessageResponse\x12%\n\x07message\x18\x01 \x01(\x0b\x32\x14.discord_api.Message\"_\n\x18SendDirectMessageRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\x04\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12!\n\x05\x65mbed\x18\x03 \x01(\x0b\x32\x12.discord_api.Embed\"B\n\x19SendDirectMessageResponse\x12%\n\x07message\x18\x01 \x01(\x0b\x32\x14.discord_api.Message\"+\n\x17GetGuildChannelsRequest\x12\x10\n\x08guild_id\x18\x01 \x01(\x04\"B\n\x18GetGuildChannelsResponse\x12&\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x14.discord_api.Channel2\xbe\x02\n\nDiscordApi\x12g\n\x12SendChannelMessage\x12&.discord_api.SendChannelMessageRequest\x1a\'.discord_api.SendChannelMessageResponse\"\x00\x12\x64\n\x11SendDirectMessage\x12%.discord_api.SendDirectMessageRequest\x1a&.discord_api.SendDirectMessageResponse\"\x00\x12\x61\n\x10GetGuildChannels\x12$.discord_api.GetGuildChannelsRequest\x1a%.discord_api.GetGuildChannelsResponse\"\x00\x62\x06proto3')
-
-
-
-_CHANNEL = DESCRIPTOR.message_types_by_name['Channel']
-_EMBED = DESCRIPTOR.message_types_by_name['Embed']
-_EMBED_FOOTER = _EMBED.nested_types_by_name['Footer']
-_EMBED_IMAGE = _EMBED.nested_types_by_name['Image']
-_EMBED_THUMBNAIL = _EMBED.nested_types_by_name['Thumbnail']
-_EMBED_VIDEO = _EMBED.nested_types_by_name['Video']
-_EMBED_PROVIDER = _EMBED.nested_types_by_name['Provider']
-_EMBED_AUTHOR = _EMBED.nested_types_by_name['Author']
-_EMBED_FIELD = _EMBED.nested_types_by_name['Field']
-_EMOJI = DESCRIPTOR.message_types_by_name['Emoji']
-_GUILDMEMBER = DESCRIPTOR.message_types_by_name['GuildMember']
-_MESSAGE = DESCRIPTOR.message_types_by_name['Message']
-_MESSAGE_CHANNELMENTION = _MESSAGE.nested_types_by_name['ChannelMention']
-_MESSAGE_ATTACHMENT = _MESSAGE.nested_types_by_name['Attachment']
-_MESSAGE_REACTION = _MESSAGE.nested_types_by_name['Reaction']
-_MESSAGE_ACTIVITY = _MESSAGE.nested_types_by_name['Activity']
-_MESSAGE_APPLICATION = _MESSAGE.nested_types_by_name['Application']
-_MESSAGE_REFERENCE = _MESSAGE.nested_types_by_name['Reference']
-_MESSAGE_STICKER = _MESSAGE.nested_types_by_name['Sticker']
-_ROLE = DESCRIPTOR.message_types_by_name['Role']
-_ROLE_TAG = _ROLE.nested_types_by_name['Tag']
-_USER = DESCRIPTOR.message_types_by_name['User']
-_SENDCHANNELMESSAGEREQUEST = DESCRIPTOR.message_types_by_name['SendChannelMessageRequest']
-_SENDCHANNELMESSAGERESPONSE = DESCRIPTOR.message_types_by_name['SendChannelMessageResponse']
-_SENDDIRECTMESSAGEREQUEST = DESCRIPTOR.message_types_by_name['SendDirectMessageRequest']
-_SENDDIRECTMESSAGERESPONSE = DESCRIPTOR.message_types_by_name['SendDirectMessageResponse']
-_GETGUILDCHANNELSREQUEST = DESCRIPTOR.message_types_by_name['GetGuildChannelsRequest']
-_GETGUILDCHANNELSRESPONSE = DESCRIPTOR.message_types_by_name['GetGuildChannelsResponse']
-_CHANNEL_TYPE = _CHANNEL.enum_types_by_name['Type']
-_MESSAGE_ACTIVITY_TYPE = _MESSAGE_ACTIVITY.enum_types_by_name['Type']
-_MESSAGE_STICKER_TYPE = _MESSAGE_STICKER.enum_types_by_name['Type']
-_MESSAGE_TYPE = _MESSAGE.enum_types_by_name['Type']
-Channel = _reflection.GeneratedProtocolMessageType('Channel', (_message.Message,), {
-  'DESCRIPTOR' : _CHANNEL,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.Channel)
-  })
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x11\x64iscord_api.proto\x12\x0b\x64iscord_api"\xb1\x02\n\x07\x43hannel\x12\n\n\x02id\x18\x01 \x01(\x04\x12\'\n\x04type\x18\x02 \x01(\x0e\x32\x19.discord_api.Channel.Type\x12\x10\n\x08guild_id\x18\x03 \x01(\x04\x12\x10\n\x08position\x18\x04 \x01(\x05\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\r\n\x05topic\x18\x07 \x01(\t\x12\x0c\n\x04nsfw\x18\x08 \x01(\x08\x12\x17\n\x0flast_message_id\x18\t \x01(\x04\x12\x11\n\tparent_id\x18\n \x01(\x04"v\n\x04Type\x12\r\n\tUNDEFINED\x10\x00\x12\x0e\n\nGUILD_TEXT\x10\x01\x12\x06\n\x02\x44M\x10\x02\x12\x0f\n\x0bGUILD_VOICE\x10\x03\x12\x0c\n\x08GROUP_DM\x10\x04\x12\x12\n\x0eGUILD_CATEGORY\x10\x05\x12\x0e\n\nGUILD_NEWS\x10\x06"\x04\x08\x07\x10\x07"\xee\x06\n\x05\x45mbed\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12\x11\n\ttimestamp\x18\x05 \x01(\t\x12\r\n\x05\x63olor\x18\x06 \x01(\x05\x12)\n\x06\x66ooter\x18\x07 \x01(\x0b\x32\x19.discord_api.Embed.Footer\x12\'\n\x05image\x18\x08 \x01(\x0b\x32\x18.discord_api.Embed.Image\x12/\n\tthumbnail\x18\t \x01(\x0b\x32\x1c.discord_api.Embed.Thumbnail\x12\'\n\x05video\x18\n \x01(\x0b\x32\x18.discord_api.Embed.Video\x12-\n\x08provider\x18\x0b \x01(\x0b\x32\x1b.discord_api.Embed.Provider\x12)\n\x06\x61uthor\x18\x0c \x01(\x0b\x32\x19.discord_api.Embed.Author\x12(\n\x06\x66ields\x18\r \x03(\x0b\x32\x18.discord_api.Embed.Field\x1a@\n\x06\x46ooter\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08icon_url\x18\x02 \x01(\t\x12\x16\n\x0eproxy_icon_url\x18\x03 \x01(\t\x1aK\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x16\n\x0eproxy_icon_url\x18\x02 \x01(\t\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\r\n\x05width\x18\x04 \x01(\x05\x1aJ\n\tThumbnail\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tproxy_url\x18\x02 \x01(\t\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\r\n\x05width\x18\x04 \x01(\x05\x1aK\n\x05Video\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x16\n\x0eproxy_icon_url\x18\x02 \x01(\t\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\r\n\x05width\x18\x04 \x01(\x05\x1a%\n\x08Provider\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x1aM\n\x06\x41uthor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x10\n\x08icon_url\x18\x03 \x01(\t\x12\x16\n\x0eproxy_icon_url\x18\x04 \x01(\t\x1a\x34\n\x05\x46ield\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0e\n\x06inline\x18\x03 \x01(\x08"\xa0\x01\n\x05\x45moji\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\x04\x12\x1f\n\x04user\x18\x04 \x01(\x0b\x32\x11.discord_api.User\x12\x17\n\x0frequired_colons\x18\x05 \x01(\x08\x12\x0f\n\x07managed\x18\x06 \x01(\x08\x12\x10\n\x08\x61nimated\x18\x07 \x01(\x08\x12\x11\n\tavailable\x18\x08 \x01(\x08"\xb7\x01\n\x0bGuildMember\x12\x1f\n\x04user\x18\x01 \x01(\x0b\x32\x11.discord_api.User\x12\x0c\n\x04nick\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\x04\x12\x11\n\tjoined_at\x18\x04 \x01(\t\x12\x15\n\rpremium_since\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x65\x61\x66\x18\x06 \x01(\x08\x12\x0c\n\x04mute\x18\x07 \x01(\x08\x12\x0f\n\x07pending\x18\x08 \x01(\x08\x12\x13\n\x0bpermissions\x18\t \x01(\t"\x90\x11\n\x07Message\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x12\n\nchannel_id\x18\x02 \x01(\x04\x12\x10\n\x08guild_id\x18\x03 \x01(\x04\x12!\n\x06\x61uthor\x18\x04 \x01(\x0b\x32\x11.discord_api.User\x12(\n\x06member\x18\x05 \x01(\x0b\x32\x18.discord_api.GuildMember\x12\x0f\n\x07\x63ontent\x18\x06 \x01(\t\x12\x11\n\ttimestamp\x18\x07 \x01(\t\x12\x18\n\x10\x65\x64ited_timestamp\x18\x08 \x01(\t\x12\x0b\n\x03tts\x18\t \x01(\x08\x12\x18\n\x10mention_everyone\x18\n \x01(\x08\x12#\n\x08mentions\x18\x0b \x03(\x0b\x32\x11.discord_api.User\x12\x15\n\rmention_roles\x18\x0c \x03(\x04\x12\x18\n\x10mention_channels\x18\r \x03(\x04\x12\x34\n\x0b\x61ttachments\x18\x0e \x03(\x0b\x32\x1f.discord_api.Message.Attachment\x12"\n\x06\x65mbeds\x18\x0f \x03(\x0b\x32\x12.discord_api.Embed\x12\x30\n\treactions\x18\x10 \x03(\x0b\x32\x1d.discord_api.Message.Reaction\x12\r\n\x05nonce\x18\x11 \x01(\t\x12\x0e\n\x06pinned\x18\x12 \x01(\x08\x12\x12\n\nwebhook_id\x18\x13 \x01(\x04\x12\'\n\x04type\x18\x14 \x01(\x0e\x32\x19.discord_api.Message.Type\x12/\n\x08\x61\x63tivity\x18\x15 \x01(\x0b\x32\x1d.discord_api.Message.Activity\x12\x35\n\x0b\x61pplication\x18\x16 \x01(\x0b\x32 .discord_api.Message.Application\x12\x39\n\x11message_reference\x18\x17 \x01(\x0b\x32\x1e.discord_api.Message.Reference\x12\r\n\x05\x66lags\x18\x18 \x01(\x05\x12.\n\x08stickers\x18\x19 \x03(\x0b\x32\x1c.discord_api.Message.Sticker\x12\x30\n\x12referenced_message\x18\x1a \x01(\x0b\x32\x14.discord_api.Message\x1a\x65\n\x0e\x43hannelMention\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x10\n\x08guild_id\x18\x02 \x01(\x04\x12\'\n\x04type\x18\x03 \x01(\x0e\x32\x19.discord_api.Channel.Type\x12\x0c\n\x04name\x18\x04 \x01(\t\x1aw\n\nAttachment\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x10\n\x08\x66ilename\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\x05\x12\x0b\n\x03url\x18\x04 \x01(\t\x12\x11\n\tproxy_url\x18\x05 \x01(\t\x12\x0e\n\x06height\x18\x06 \x01(\x05\x12\r\n\x05width\x18\x07 \x01(\x05\x1aH\n\x08Reaction\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\n\n\x02me\x18\x02 \x01(\x08\x12!\n\x05\x65moji\x18\x03 \x01(\x0b\x32\x12.discord_api.Emoji\x1a\x9c\x01\n\x08\x41\x63tivity\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32".discord_api.Message.Activity.Type\x12\x10\n\x08party_id\x18\x02 \x01(\t"L\n\x04Type\x12\r\n\tUNDEFINED\x10\x00\x12\x08\n\x04JOIN\x10\x01\x12\x0c\n\x08SPECTATE\x10\x02\x12\n\n\x06LISTEN\x10\x03\x12\x11\n\rJOIN_REQUESTS\x10\x04\x1a_\n\x0b\x41pplication\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x13\n\x0b\x63over_image\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04icon\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x1a\x61\n\tReference\x12\x12\n\nmessage_id\x18\x01 \x01(\x04\x12\x12\n\nchannel_id\x18\x02 \x01(\x04\x12\x10\n\x08guild_id\x18\x03 \x01(\x04\x12\x1a\n\x12\x66\x61il_if_not_exists\x18\x04 \x01(\x08\x1a\xeb\x01\n\x07Sticker\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x0f\n\x07pack_id\x18\x02 \x01(\x04\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x01(\t\x12\r\n\x05\x61sset\x18\x06 \x01(\t\x12\x15\n\rpreview_asset\x18\x07 \x01(\t\x12\x36\n\x0b\x66ormat_type\x18\x08 \x01(\x0e\x32!.discord_api.Message.Sticker.Type"4\n\x04Type\x12\r\n\tUNDEFINED\x10\x00\x12\x07\n\x03PNG\x10\x01\x12\x08\n\x04\x41PNG\x10\x02\x12\n\n\x06LOTTIE\x10\x03"\xd3\x03\n\x04Type\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x11\n\rRECIPIENT_ADD\x10\x01\x12\x14\n\x10RECIPIENT_REMOVE\x10\x02\x12\x08\n\x04\x43\x41LL\x10\x03\x12\x17\n\x13\x43HANNEL_NAME_CHANGE\x10\x04\x12\x17\n\x13\x43HANNEL_ICON_CHANGE\x10\x05\x12\x1a\n\x16\x43HANNEL_PINNED_MESSAGE\x10\x06\x12\x15\n\x11GUILD_MEMBER_JOIN\x10\x07\x12#\n\x1fUSER_PREMIUM_GUILD_SUBSCRIPTION\x10\x08\x12*\n&USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_1\x10\t\x12*\n&USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_2\x10\n\x12*\n&USER_PREMIUM_GUILD_SUBSCRIPTION_TIER_3\x10\x0b\x12\x16\n\x12\x43HANNEL_FOLLOW_ADD\x10\x0c\x12 \n\x1cGUILD_DISCOVERY_DISQUALIFIED\x10\x0e\x12\x1f\n\x1bGUILD_DISCOVERY_REQUALIFIED\x10\x0f\x12\t\n\x05REPLY\x10\x13\x12\x17\n\x13\x41PPLICATION_COMMAND\x10\x14"\xf7\x01\n\x04Role\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\x05\x12\r\n\x05hoist\x18\x04 \x01(\x08\x12\x10\n\x08position\x18\x05 \x01(\x05\x12\x13\n\x0bpermissions\x18\x06 \x01(\t\x12\x0f\n\x07managed\x18\x07 \x01(\x08\x12\x13\n\x0bmentionable\x18\x08 \x01(\x08\x12#\n\x04tags\x18\t \x03(\x0b\x32\x15.discord_api.Role.Tag\x1a\x45\n\x03Tag\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x16\n\x0eintegration_id\x18\x02 \x01(\x04\x12\x1a\n\x12premium_subscriber\x18\x03 \x01(\x08"\xe9\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x15\n\rdiscriminator\x18\x03 \x01(\t\x12\x0e\n\x06\x61vatar\x18\x04 \x01(\t\x12\x0b\n\x03\x62ot\x18\x05 \x01(\x08\x12\x0e\n\x06system\x18\x06 \x01(\x08\x12\x13\n\x0bmfa_enabled\x18\x07 \x01(\x08\x12\x0e\n\x06locale\x18\x08 \x01(\t\x12\x10\n\x08verified\x18\t \x01(\x08\x12\r\n\x05\x65mail\x18\n \x01(\t\x12\r\n\x05\x66lags\x18\x0b \x01(\x05\x12\x14\n\x0cpremium_type\x18\x0c \x01(\x05\x12\x14\n\x0cpublic_flags\x18\r \x01(\x05"c\n\x19SendChannelMessageRequest\x12\x12\n\nchannel_id\x18\x01 \x01(\x04\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12!\n\x05\x65mbed\x18\x03 \x01(\x0b\x32\x12.discord_api.Embed"C\n\x1aSendChannelMessageResponse\x12%\n\x07message\x18\x01 \x01(\x0b\x32\x14.discord_api.Message"_\n\x18SendDirectMessageRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\x04\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12!\n\x05\x65mbed\x18\x03 \x01(\x0b\x32\x12.discord_api.Embed"B\n\x19SendDirectMessageResponse\x12%\n\x07message\x18\x01 \x01(\x0b\x32\x14.discord_api.Message"+\n\x17GetGuildChannelsRequest\x12\x10\n\x08guild_id\x18\x01 \x01(\x04"B\n\x18GetGuildChannelsResponse\x12&\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x14.discord_api.Channel2\xbe\x02\n\nDiscordApi\x12g\n\x12SendChannelMessage\x12&.discord_api.SendChannelMessageRequest\x1a\'.discord_api.SendChannelMessageResponse"\x00\x12\x64\n\x11SendDirectMessage\x12%.discord_api.SendDirectMessageRequest\x1a&.discord_api.SendDirectMessageResponse"\x00\x12\x61\n\x10GetGuildChannels\x12$.discord_api.GetGuildChannelsRequest\x1a%.discord_api.GetGuildChannelsResponse"\x00\x62\x06proto3'
+)
+
+
+_CHANNEL = DESCRIPTOR.message_types_by_name["Channel"]
+_EMBED = DESCRIPTOR.message_types_by_name["Embed"]
+_EMBED_FOOTER = _EMBED.nested_types_by_name["Footer"]
+_EMBED_IMAGE = _EMBED.nested_types_by_name["Image"]
+_EMBED_THUMBNAIL = _EMBED.nested_types_by_name["Thumbnail"]
+_EMBED_VIDEO = _EMBED.nested_types_by_name["Video"]
+_EMBED_PROVIDER = _EMBED.nested_types_by_name["Provider"]
+_EMBED_AUTHOR = _EMBED.nested_types_by_name["Author"]
+_EMBED_FIELD = _EMBED.nested_types_by_name["Field"]
+_EMOJI = DESCRIPTOR.message_types_by_name["Emoji"]
+_GUILDMEMBER = DESCRIPTOR.message_types_by_name["GuildMember"]
+_MESSAGE = DESCRIPTOR.message_types_by_name["Message"]
+_MESSAGE_CHANNELMENTION = _MESSAGE.nested_types_by_name["ChannelMention"]
+_MESSAGE_ATTACHMENT = _MESSAGE.nested_types_by_name["Attachment"]
+_MESSAGE_REACTION = _MESSAGE.nested_types_by_name["Reaction"]
+_MESSAGE_ACTIVITY = _MESSAGE.nested_types_by_name["Activity"]
+_MESSAGE_APPLICATION = _MESSAGE.nested_types_by_name["Application"]
+_MESSAGE_REFERENCE = _MESSAGE.nested_types_by_name["Reference"]
+_MESSAGE_STICKER = _MESSAGE.nested_types_by_name["Sticker"]
+_ROLE = DESCRIPTOR.message_types_by_name["Role"]
+_ROLE_TAG = _ROLE.nested_types_by_name["Tag"]
+_USER = DESCRIPTOR.message_types_by_name["User"]
+_SENDCHANNELMESSAGEREQUEST = DESCRIPTOR.message_types_by_name[
+    "SendChannelMessageRequest"
+]
+_SENDCHANNELMESSAGERESPONSE = DESCRIPTOR.message_types_by_name[
+    "SendChannelMessageResponse"
+]
+_SENDDIRECTMESSAGEREQUEST = DESCRIPTOR.message_types_by_name["SendDirectMessageRequest"]
+_SENDDIRECTMESSAGERESPONSE = DESCRIPTOR.message_types_by_name[
+    "SendDirectMessageResponse"
+]
+_GETGUILDCHANNELSREQUEST = DESCRIPTOR.message_types_by_name["GetGuildChannelsRequest"]
+_GETGUILDCHANNELSRESPONSE = DESCRIPTOR.message_types_by_name["GetGuildChannelsResponse"]
+_CHANNEL_TYPE = _CHANNEL.enum_types_by_name["Type"]
+_MESSAGE_ACTIVITY_TYPE = _MESSAGE_ACTIVITY.enum_types_by_name["Type"]
+_MESSAGE_STICKER_TYPE = _MESSAGE_STICKER.enum_types_by_name["Type"]
+_MESSAGE_TYPE = _MESSAGE.enum_types_by_name["Type"]
+Channel = _reflection.GeneratedProtocolMessageType(
+    "Channel",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _CHANNEL,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.Channel)
+    },
+)
 _sym_db.RegisterMessage(Channel)
 
-Embed = _reflection.GeneratedProtocolMessageType('Embed', (_message.Message,), {
-
-  'Footer' : _reflection.GeneratedProtocolMessageType('Footer', (_message.Message,), {
-    'DESCRIPTOR' : _EMBED_FOOTER,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Embed.Footer)
-    })
-  ,
-
-  'Image' : _reflection.GeneratedProtocolMessageType('Image', (_message.Message,), {
-    'DESCRIPTOR' : _EMBED_IMAGE,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Embed.Image)
-    })
-  ,
-
-  'Thumbnail' : _reflection.GeneratedProtocolMessageType('Thumbnail', (_message.Message,), {
-    'DESCRIPTOR' : _EMBED_THUMBNAIL,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Embed.Thumbnail)
-    })
-  ,
-
-  'Video' : _reflection.GeneratedProtocolMessageType('Video', (_message.Message,), {
-    'DESCRIPTOR' : _EMBED_VIDEO,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Embed.Video)
-    })
-  ,
-
-  'Provider' : _reflection.GeneratedProtocolMessageType('Provider', (_message.Message,), {
-    'DESCRIPTOR' : _EMBED_PROVIDER,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Embed.Provider)
-    })
-  ,
-
-  'Author' : _reflection.GeneratedProtocolMessageType('Author', (_message.Message,), {
-    'DESCRIPTOR' : _EMBED_AUTHOR,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Embed.Author)
-    })
-  ,
-
-  'Field' : _reflection.GeneratedProtocolMessageType('Field', (_message.Message,), {
-    'DESCRIPTOR' : _EMBED_FIELD,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Embed.Field)
-    })
-  ,
-  'DESCRIPTOR' : _EMBED,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.Embed)
-  })
+Embed = _reflection.GeneratedProtocolMessageType(
+    "Embed",
+    (_message.Message,),
+    {
+        "Footer": _reflection.GeneratedProtocolMessageType(
+            "Footer",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _EMBED_FOOTER,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Embed.Footer)
+            },
+        ),
+        "Image": _reflection.GeneratedProtocolMessageType(
+            "Image",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _EMBED_IMAGE,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Embed.Image)
+            },
+        ),
+        "Thumbnail": _reflection.GeneratedProtocolMessageType(
+            "Thumbnail",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _EMBED_THUMBNAIL,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Embed.Thumbnail)
+            },
+        ),
+        "Video": _reflection.GeneratedProtocolMessageType(
+            "Video",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _EMBED_VIDEO,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Embed.Video)
+            },
+        ),
+        "Provider": _reflection.GeneratedProtocolMessageType(
+            "Provider",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _EMBED_PROVIDER,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Embed.Provider)
+            },
+        ),
+        "Author": _reflection.GeneratedProtocolMessageType(
+            "Author",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _EMBED_AUTHOR,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Embed.Author)
+            },
+        ),
+        "Field": _reflection.GeneratedProtocolMessageType(
+            "Field",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _EMBED_FIELD,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Embed.Field)
+            },
+        ),
+        "DESCRIPTOR": _EMBED,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.Embed)
+    },
+)
 _sym_db.RegisterMessage(Embed)
 _sym_db.RegisterMessage(Embed.Footer)
 _sym_db.RegisterMessage(Embed.Image)
 _sym_db.RegisterMessage(Embed.Thumbnail)
 _sym_db.RegisterMessage(Embed.Video)
 _sym_db.RegisterMessage(Embed.Provider)
 _sym_db.RegisterMessage(Embed.Author)
 _sym_db.RegisterMessage(Embed.Field)
 
-Emoji = _reflection.GeneratedProtocolMessageType('Emoji', (_message.Message,), {
-  'DESCRIPTOR' : _EMOJI,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.Emoji)
-  })
+Emoji = _reflection.GeneratedProtocolMessageType(
+    "Emoji",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _EMOJI,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.Emoji)
+    },
+)
 _sym_db.RegisterMessage(Emoji)
 
-GuildMember = _reflection.GeneratedProtocolMessageType('GuildMember', (_message.Message,), {
-  'DESCRIPTOR' : _GUILDMEMBER,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.GuildMember)
-  })
+GuildMember = _reflection.GeneratedProtocolMessageType(
+    "GuildMember",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _GUILDMEMBER,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.GuildMember)
+    },
+)
 _sym_db.RegisterMessage(GuildMember)
 
-Message = _reflection.GeneratedProtocolMessageType('Message', (_message.Message,), {
-
-  'ChannelMention' : _reflection.GeneratedProtocolMessageType('ChannelMention', (_message.Message,), {
-    'DESCRIPTOR' : _MESSAGE_CHANNELMENTION,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Message.ChannelMention)
-    })
-  ,
-
-  'Attachment' : _reflection.GeneratedProtocolMessageType('Attachment', (_message.Message,), {
-    'DESCRIPTOR' : _MESSAGE_ATTACHMENT,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Message.Attachment)
-    })
-  ,
-
-  'Reaction' : _reflection.GeneratedProtocolMessageType('Reaction', (_message.Message,), {
-    'DESCRIPTOR' : _MESSAGE_REACTION,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Message.Reaction)
-    })
-  ,
-
-  'Activity' : _reflection.GeneratedProtocolMessageType('Activity', (_message.Message,), {
-    'DESCRIPTOR' : _MESSAGE_ACTIVITY,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Message.Activity)
-    })
-  ,
-
-  'Application' : _reflection.GeneratedProtocolMessageType('Application', (_message.Message,), {
-    'DESCRIPTOR' : _MESSAGE_APPLICATION,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Message.Application)
-    })
-  ,
-
-  'Reference' : _reflection.GeneratedProtocolMessageType('Reference', (_message.Message,), {
-    'DESCRIPTOR' : _MESSAGE_REFERENCE,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Message.Reference)
-    })
-  ,
-
-  'Sticker' : _reflection.GeneratedProtocolMessageType('Sticker', (_message.Message,), {
-    'DESCRIPTOR' : _MESSAGE_STICKER,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Message.Sticker)
-    })
-  ,
-  'DESCRIPTOR' : _MESSAGE,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.Message)
-  })
+Message = _reflection.GeneratedProtocolMessageType(
+    "Message",
+    (_message.Message,),
+    {
+        "ChannelMention": _reflection.GeneratedProtocolMessageType(
+            "ChannelMention",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _MESSAGE_CHANNELMENTION,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Message.ChannelMention)
+            },
+        ),
+        "Attachment": _reflection.GeneratedProtocolMessageType(
+            "Attachment",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _MESSAGE_ATTACHMENT,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Message.Attachment)
+            },
+        ),
+        "Reaction": _reflection.GeneratedProtocolMessageType(
+            "Reaction",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _MESSAGE_REACTION,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Message.Reaction)
+            },
+        ),
+        "Activity": _reflection.GeneratedProtocolMessageType(
+            "Activity",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _MESSAGE_ACTIVITY,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Message.Activity)
+            },
+        ),
+        "Application": _reflection.GeneratedProtocolMessageType(
+            "Application",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _MESSAGE_APPLICATION,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Message.Application)
+            },
+        ),
+        "Reference": _reflection.GeneratedProtocolMessageType(
+            "Reference",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _MESSAGE_REFERENCE,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Message.Reference)
+            },
+        ),
+        "Sticker": _reflection.GeneratedProtocolMessageType(
+            "Sticker",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _MESSAGE_STICKER,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Message.Sticker)
+            },
+        ),
+        "DESCRIPTOR": _MESSAGE,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.Message)
+    },
+)
 _sym_db.RegisterMessage(Message)
 _sym_db.RegisterMessage(Message.ChannelMention)
 _sym_db.RegisterMessage(Message.Attachment)
 _sym_db.RegisterMessage(Message.Reaction)
 _sym_db.RegisterMessage(Message.Activity)
 _sym_db.RegisterMessage(Message.Application)
 _sym_db.RegisterMessage(Message.Reference)
 _sym_db.RegisterMessage(Message.Sticker)
 
-Role = _reflection.GeneratedProtocolMessageType('Role', (_message.Message,), {
-
-  'Tag' : _reflection.GeneratedProtocolMessageType('Tag', (_message.Message,), {
-    'DESCRIPTOR' : _ROLE_TAG,
-    '__module__' : 'discord_api_pb2'
-    # @@protoc_insertion_point(class_scope:discord_api.Role.Tag)
-    })
-  ,
-  'DESCRIPTOR' : _ROLE,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.Role)
-  })
+Role = _reflection.GeneratedProtocolMessageType(
+    "Role",
+    (_message.Message,),
+    {
+        "Tag": _reflection.GeneratedProtocolMessageType(
+            "Tag",
+            (_message.Message,),
+            {
+                "DESCRIPTOR": _ROLE_TAG,
+                "__module__": "discord_api_pb2"
+                # @@protoc_insertion_point(class_scope:discord_api.Role.Tag)
+            },
+        ),
+        "DESCRIPTOR": _ROLE,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.Role)
+    },
+)
 _sym_db.RegisterMessage(Role)
 _sym_db.RegisterMessage(Role.Tag)
 
-User = _reflection.GeneratedProtocolMessageType('User', (_message.Message,), {
-  'DESCRIPTOR' : _USER,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.User)
-  })
+User = _reflection.GeneratedProtocolMessageType(
+    "User",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _USER,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.User)
+    },
+)
 _sym_db.RegisterMessage(User)
 
-SendChannelMessageRequest = _reflection.GeneratedProtocolMessageType('SendChannelMessageRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SENDCHANNELMESSAGEREQUEST,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.SendChannelMessageRequest)
-  })
+SendChannelMessageRequest = _reflection.GeneratedProtocolMessageType(
+    "SendChannelMessageRequest",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _SENDCHANNELMESSAGEREQUEST,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.SendChannelMessageRequest)
+    },
+)
 _sym_db.RegisterMessage(SendChannelMessageRequest)
 
-SendChannelMessageResponse = _reflection.GeneratedProtocolMessageType('SendChannelMessageResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SENDCHANNELMESSAGERESPONSE,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.SendChannelMessageResponse)
-  })
+SendChannelMessageResponse = _reflection.GeneratedProtocolMessageType(
+    "SendChannelMessageResponse",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _SENDCHANNELMESSAGERESPONSE,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.SendChannelMessageResponse)
+    },
+)
 _sym_db.RegisterMessage(SendChannelMessageResponse)
 
-SendDirectMessageRequest = _reflection.GeneratedProtocolMessageType('SendDirectMessageRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SENDDIRECTMESSAGEREQUEST,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.SendDirectMessageRequest)
-  })
+SendDirectMessageRequest = _reflection.GeneratedProtocolMessageType(
+    "SendDirectMessageRequest",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _SENDDIRECTMESSAGEREQUEST,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.SendDirectMessageRequest)
+    },
+)
 _sym_db.RegisterMessage(SendDirectMessageRequest)
 
-SendDirectMessageResponse = _reflection.GeneratedProtocolMessageType('SendDirectMessageResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SENDDIRECTMESSAGERESPONSE,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.SendDirectMessageResponse)
-  })
+SendDirectMessageResponse = _reflection.GeneratedProtocolMessageType(
+    "SendDirectMessageResponse",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _SENDDIRECTMESSAGERESPONSE,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.SendDirectMessageResponse)
+    },
+)
 _sym_db.RegisterMessage(SendDirectMessageResponse)
 
-GetGuildChannelsRequest = _reflection.GeneratedProtocolMessageType('GetGuildChannelsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETGUILDCHANNELSREQUEST,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.GetGuildChannelsRequest)
-  })
+GetGuildChannelsRequest = _reflection.GeneratedProtocolMessageType(
+    "GetGuildChannelsRequest",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _GETGUILDCHANNELSREQUEST,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.GetGuildChannelsRequest)
+    },
+)
 _sym_db.RegisterMessage(GetGuildChannelsRequest)
 
-GetGuildChannelsResponse = _reflection.GeneratedProtocolMessageType('GetGuildChannelsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETGUILDCHANNELSRESPONSE,
-  '__module__' : 'discord_api_pb2'
-  # @@protoc_insertion_point(class_scope:discord_api.GetGuildChannelsResponse)
-  })
+GetGuildChannelsResponse = _reflection.GeneratedProtocolMessageType(
+    "GetGuildChannelsResponse",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _GETGUILDCHANNELSRESPONSE,
+        "__module__": "discord_api_pb2"
+        # @@protoc_insertion_point(class_scope:discord_api.GetGuildChannelsResponse)
+    },
+)
 _sym_db.RegisterMessage(GetGuildChannelsResponse)
 
-_DISCORDAPI = DESCRIPTOR.services_by_name['DiscordApi']
+_DISCORDAPI = DESCRIPTOR.services_by_name["DiscordApi"]
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _CHANNEL._serialized_start=35
-  _CHANNEL._serialized_end=340
-  _CHANNEL_TYPE._serialized_start=222
-  _CHANNEL_TYPE._serialized_end=340
-  _EMBED._serialized_start=343
-  _EMBED._serialized_end=1221
-  _EMBED_FOOTER._serialized_start=755
-  _EMBED_FOOTER._serialized_end=819
-  _EMBED_IMAGE._serialized_start=821
-  _EMBED_IMAGE._serialized_end=896
-  _EMBED_THUMBNAIL._serialized_start=898
-  _EMBED_THUMBNAIL._serialized_end=972
-  _EMBED_VIDEO._serialized_start=974
-  _EMBED_VIDEO._serialized_end=1049
-  _EMBED_PROVIDER._serialized_start=1051
-  _EMBED_PROVIDER._serialized_end=1088
-  _EMBED_AUTHOR._serialized_start=1090
-  _EMBED_AUTHOR._serialized_end=1167
-  _EMBED_FIELD._serialized_start=1169
-  _EMBED_FIELD._serialized_end=1221
-  _EMOJI._serialized_start=1224
-  _EMOJI._serialized_end=1384
-  _GUILDMEMBER._serialized_start=1387
-  _GUILDMEMBER._serialized_end=1570
-  _MESSAGE._serialized_start=1573
-  _MESSAGE._serialized_end=3765
-  _MESSAGE_CHANNELMENTION._serialized_start=2406
-  _MESSAGE_CHANNELMENTION._serialized_end=2507
-  _MESSAGE_ATTACHMENT._serialized_start=2509
-  _MESSAGE_ATTACHMENT._serialized_end=2628
-  _MESSAGE_REACTION._serialized_start=2630
-  _MESSAGE_REACTION._serialized_end=2702
-  _MESSAGE_ACTIVITY._serialized_start=2705
-  _MESSAGE_ACTIVITY._serialized_end=2861
-  _MESSAGE_ACTIVITY_TYPE._serialized_start=2785
-  _MESSAGE_ACTIVITY_TYPE._serialized_end=2861
-  _MESSAGE_APPLICATION._serialized_start=2863
-  _MESSAGE_APPLICATION._serialized_end=2958
-  _MESSAGE_REFERENCE._serialized_start=2960
-  _MESSAGE_REFERENCE._serialized_end=3057
-  _MESSAGE_STICKER._serialized_start=3060
-  _MESSAGE_STICKER._serialized_end=3295
-  _MESSAGE_STICKER_TYPE._serialized_start=3243
-  _MESSAGE_STICKER_TYPE._serialized_end=3295
-  _MESSAGE_TYPE._serialized_start=3298
-  _MESSAGE_TYPE._serialized_end=3765
-  _ROLE._serialized_start=3768
-  _ROLE._serialized_end=4015
-  _ROLE_TAG._serialized_start=3946
-  _ROLE_TAG._serialized_end=4015
-  _USER._serialized_start=4018
-  _USER._serialized_end=4251
-  _SENDCHANNELMESSAGEREQUEST._serialized_start=4253
-  _SENDCHANNELMESSAGEREQUEST._serialized_end=4352
-  _SENDCHANNELMESSAGERESPONSE._serialized_start=4354
-  _SENDCHANNELMESSAGERESPONSE._serialized_end=4421
-  _SENDDIRECTMESSAGEREQUEST._serialized_start=4423
-  _SENDDIRECTMESSAGEREQUEST._serialized_end=4518
-  _SENDDIRECTMESSAGERESPONSE._serialized_start=4520
-  _SENDDIRECTMESSAGERESPONSE._serialized_end=4586
-  _GETGUILDCHANNELSREQUEST._serialized_start=4588
-  _GETGUILDCHANNELSREQUEST._serialized_end=4631
-  _GETGUILDCHANNELSRESPONSE._serialized_start=4633
-  _GETGUILDCHANNELSRESPONSE._serialized_end=4699
-  _DISCORDAPI._serialized_start=4702
-  _DISCORDAPI._serialized_end=5020
+    DESCRIPTOR._options = None
+    _CHANNEL._serialized_start = 35
+    _CHANNEL._serialized_end = 340
+    _CHANNEL_TYPE._serialized_start = 222
+    _CHANNEL_TYPE._serialized_end = 340
+    _EMBED._serialized_start = 343
+    _EMBED._serialized_end = 1221
+    _EMBED_FOOTER._serialized_start = 755
+    _EMBED_FOOTER._serialized_end = 819
+    _EMBED_IMAGE._serialized_start = 821
+    _EMBED_IMAGE._serialized_end = 896
+    _EMBED_THUMBNAIL._serialized_start = 898
+    _EMBED_THUMBNAIL._serialized_end = 972
+    _EMBED_VIDEO._serialized_start = 974
+    _EMBED_VIDEO._serialized_end = 1049
+    _EMBED_PROVIDER._serialized_start = 1051
+    _EMBED_PROVIDER._serialized_end = 1088
+    _EMBED_AUTHOR._serialized_start = 1090
+    _EMBED_AUTHOR._serialized_end = 1167
+    _EMBED_FIELD._serialized_start = 1169
+    _EMBED_FIELD._serialized_end = 1221
+    _EMOJI._serialized_start = 1224
+    _EMOJI._serialized_end = 1384
+    _GUILDMEMBER._serialized_start = 1387
+    _GUILDMEMBER._serialized_end = 1570
+    _MESSAGE._serialized_start = 1573
+    _MESSAGE._serialized_end = 3765
+    _MESSAGE_CHANNELMENTION._serialized_start = 2406
+    _MESSAGE_CHANNELMENTION._serialized_end = 2507
+    _MESSAGE_ATTACHMENT._serialized_start = 2509
+    _MESSAGE_ATTACHMENT._serialized_end = 2628
+    _MESSAGE_REACTION._serialized_start = 2630
+    _MESSAGE_REACTION._serialized_end = 2702
+    _MESSAGE_ACTIVITY._serialized_start = 2705
+    _MESSAGE_ACTIVITY._serialized_end = 2861
+    _MESSAGE_ACTIVITY_TYPE._serialized_start = 2785
+    _MESSAGE_ACTIVITY_TYPE._serialized_end = 2861
+    _MESSAGE_APPLICATION._serialized_start = 2863
+    _MESSAGE_APPLICATION._serialized_end = 2958
+    _MESSAGE_REFERENCE._serialized_start = 2960
+    _MESSAGE_REFERENCE._serialized_end = 3057
+    _MESSAGE_STICKER._serialized_start = 3060
+    _MESSAGE_STICKER._serialized_end = 3295
+    _MESSAGE_STICKER_TYPE._serialized_start = 3243
+    _MESSAGE_STICKER_TYPE._serialized_end = 3295
+    _MESSAGE_TYPE._serialized_start = 3298
+    _MESSAGE_TYPE._serialized_end = 3765
+    _ROLE._serialized_start = 3768
+    _ROLE._serialized_end = 4015
+    _ROLE_TAG._serialized_start = 3946
+    _ROLE_TAG._serialized_end = 4015
+    _USER._serialized_start = 4018
+    _USER._serialized_end = 4251
+    _SENDCHANNELMESSAGEREQUEST._serialized_start = 4253
+    _SENDCHANNELMESSAGEREQUEST._serialized_end = 4352
+    _SENDCHANNELMESSAGERESPONSE._serialized_start = 4354
+    _SENDCHANNELMESSAGERESPONSE._serialized_end = 4421
+    _SENDDIRECTMESSAGEREQUEST._serialized_start = 4423
+    _SENDDIRECTMESSAGEREQUEST._serialized_end = 4518
+    _SENDDIRECTMESSAGERESPONSE._serialized_start = 4520
+    _SENDDIRECTMESSAGERESPONSE._serialized_end = 4586
+    _GETGUILDCHANNELSREQUEST._serialized_start = 4588
+    _GETGUILDCHANNELSREQUEST._serialized_end = 4631
+    _GETGUILDCHANNELSRESPONSE._serialized_start = 4633
+    _GETGUILDCHANNELSRESPONSE._serialized_end = 4699
+    _DISCORDAPI._serialized_start = 4702
+    _DISCORDAPI._serialized_end = 5020
 # @@protoc_insertion_point(module_scope)
```

### Comparing `discordproxy-1.2.2/discordproxy/discord_api_pb2_grpc.py` & `discordproxy-1.3.0/discordproxy/discord_api_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,137 +2,168 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from . import discord_api_pb2 as discord__api__pb2
 
 
 class DiscordApiStub(object):
-    """Provides access to the Discord API
-    """
+    """Provides access to the Discord API"""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.SendChannelMessage = channel.unary_unary(
-                '/discord_api.DiscordApi/SendChannelMessage',
-                request_serializer=discord__api__pb2.SendChannelMessageRequest.SerializeToString,
-                response_deserializer=discord__api__pb2.SendChannelMessageResponse.FromString,
-                )
+            "/discord_api.DiscordApi/SendChannelMessage",
+            request_serializer=discord__api__pb2.SendChannelMessageRequest.SerializeToString,
+            response_deserializer=discord__api__pb2.SendChannelMessageResponse.FromString,
+        )
         self.SendDirectMessage = channel.unary_unary(
-                '/discord_api.DiscordApi/SendDirectMessage',
-                request_serializer=discord__api__pb2.SendDirectMessageRequest.SerializeToString,
-                response_deserializer=discord__api__pb2.SendDirectMessageResponse.FromString,
-                )
+            "/discord_api.DiscordApi/SendDirectMessage",
+            request_serializer=discord__api__pb2.SendDirectMessageRequest.SerializeToString,
+            response_deserializer=discord__api__pb2.SendDirectMessageResponse.FromString,
+        )
         self.GetGuildChannels = channel.unary_unary(
-                '/discord_api.DiscordApi/GetGuildChannels',
-                request_serializer=discord__api__pb2.GetGuildChannelsRequest.SerializeToString,
-                response_deserializer=discord__api__pb2.GetGuildChannelsResponse.FromString,
-                )
+            "/discord_api.DiscordApi/GetGuildChannels",
+            request_serializer=discord__api__pb2.GetGuildChannelsRequest.SerializeToString,
+            response_deserializer=discord__api__pb2.GetGuildChannelsResponse.FromString,
+        )
 
 
 class DiscordApiServicer(object):
-    """Provides access to the Discord API
-    """
+    """Provides access to the Discord API"""
 
     def SendChannelMessage(self, request, context):
-        """Send a message to a guild channel
-        """
+        """Send a message to a guild channel"""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
     def SendDirectMessage(self, request, context):
-        """Send a direct message to a user
-        """
+        """Send a direct message to a user"""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
     def GetGuildChannels(self, request, context):
-        """Get the list of channel for a guild
-        """
+        """Get the list of channel for a guild"""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
 
 def add_DiscordApiServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'SendChannelMessage': grpc.unary_unary_rpc_method_handler(
-                    servicer.SendChannelMessage,
-                    request_deserializer=discord__api__pb2.SendChannelMessageRequest.FromString,
-                    response_serializer=discord__api__pb2.SendChannelMessageResponse.SerializeToString,
-            ),
-            'SendDirectMessage': grpc.unary_unary_rpc_method_handler(
-                    servicer.SendDirectMessage,
-                    request_deserializer=discord__api__pb2.SendDirectMessageRequest.FromString,
-                    response_serializer=discord__api__pb2.SendDirectMessageResponse.SerializeToString,
-            ),
-            'GetGuildChannels': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetGuildChannels,
-                    request_deserializer=discord__api__pb2.GetGuildChannelsRequest.FromString,
-                    response_serializer=discord__api__pb2.GetGuildChannelsResponse.SerializeToString,
-            ),
+        "SendChannelMessage": grpc.unary_unary_rpc_method_handler(
+            servicer.SendChannelMessage,
+            request_deserializer=discord__api__pb2.SendChannelMessageRequest.FromString,
+            response_serializer=discord__api__pb2.SendChannelMessageResponse.SerializeToString,
+        ),
+        "SendDirectMessage": grpc.unary_unary_rpc_method_handler(
+            servicer.SendDirectMessage,
+            request_deserializer=discord__api__pb2.SendDirectMessageRequest.FromString,
+            response_serializer=discord__api__pb2.SendDirectMessageResponse.SerializeToString,
+        ),
+        "GetGuildChannels": grpc.unary_unary_rpc_method_handler(
+            servicer.GetGuildChannels,
+            request_deserializer=discord__api__pb2.GetGuildChannelsRequest.FromString,
+            response_serializer=discord__api__pb2.GetGuildChannelsResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'discord_api.DiscordApi', rpc_method_handlers)
+        "discord_api.DiscordApi", rpc_method_handlers
+    )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
- # This class is part of an EXPERIMENTAL API.
+# This class is part of an EXPERIMENTAL API.
 class DiscordApi(object):
-    """Provides access to the Discord API
-    """
+    """Provides access to the Discord API"""
 
     @staticmethod
-    def SendChannelMessage(request,
+    def SendChannelMessage(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/discord_api.DiscordApi/SendChannelMessage',
+            "/discord_api.DiscordApi/SendChannelMessage",
             discord__api__pb2.SendChannelMessageRequest.SerializeToString,
             discord__api__pb2.SendChannelMessageResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
 
     @staticmethod
-    def SendDirectMessage(request,
+    def SendDirectMessage(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/discord_api.DiscordApi/SendDirectMessage',
+            "/discord_api.DiscordApi/SendDirectMessage",
             discord__api__pb2.SendDirectMessageRequest.SerializeToString,
             discord__api__pb2.SendDirectMessageResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
 
     @staticmethod
-    def GetGuildChannels(request,
+    def GetGuildChannels(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/discord_api.DiscordApi/GetGuildChannels',
+            "/discord_api.DiscordApi/GetGuildChannels",
             discord__api__pb2.GetGuildChannelsRequest.SerializeToString,
             discord__api__pb2.GetGuildChannelsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
```

### Comparing `discordproxy-1.2.2/discordproxy/exceptions.py` & `discordproxy-1.3.0/discordproxy/exceptions.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.2.2/discordproxy/helpers.py` & `discordproxy-1.3.0/discordproxy/helpers.py`

 * *Files identical despite different names*

