# Comparing `tmp/cs-3.1.0.tar.gz` & `tmp/cs-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-3.1.0.tar", last modified: Tue Jun  6 12:56:58 2023, max compression
+gzip compressed data, was "cs-3.2.0.tar", last modified: Thu Jun 22 07:16:45 2023, max compression
```

## Comparing `cs-3.1.0.tar` & `cs-3.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-06 12:56:58.609463 cs-3.1.0/
--rw-r--r--   0 brute     (1000) brute     (1000)     1501 2023-06-06 12:23:45.000000 cs-3.1.0/LICENSE
--rw-r--r--   0 brute     (1000) brute     (1000)       42 2023-06-06 12:23:45.000000 cs-3.1.0/MANIFEST.in
--rw-r--r--   0 brute     (1000) brute     (1000)     8187 2023-06-06 12:56:58.609463 cs-3.1.0/PKG-INFO
--rw-r--r--   0 brute     (1000) brute     (1000)     7517 2023-06-06 12:23:45.000000 cs-3.1.0/README.rst
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-06 12:56:58.609463 cs-3.1.0/cs/
--rw-r--r--   0 brute     (1000) brute     (1000)     4473 2023-06-06 12:23:45.000000 cs-3.1.0/cs/__init__.py
--rw-r--r--   0 brute     (1000) brute     (1000)       59 2023-06-06 12:23:45.000000 cs-3.1.0/cs/__main__.py
--rw-r--r--   0 brute     (1000) brute     (1000)     4634 2023-06-06 12:23:45.000000 cs-3.1.0/cs/_async.py
--rw-r--r--   0 brute     (1000) brute     (1000)    18524 2023-06-06 12:55:58.000000 cs-3.1.0/cs/client.py
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-06 12:56:58.609463 cs-3.1.0/cs.egg-info/
--rw-r--r--   0 brute     (1000) brute     (1000)     8187 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/PKG-INFO
--rw-r--r--   0 brute     (1000) brute     (1000)      288 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/SOURCES.txt
--rw-r--r--   0 brute     (1000) brute     (1000)        1 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/dependency_links.txt
--rw-r--r--   0 brute     (1000) brute     (1000)       31 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/entry_points.txt
--rw-r--r--   0 brute     (1000) brute     (1000)        1 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/not-zip-safe
--rw-r--r--   0 brute     (1000) brute     (1000)       53 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/requires.txt
--rw-r--r--   0 brute     (1000) brute     (1000)        3 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/top_level.txt
--rw-r--r--   0 brute     (1000) brute     (1000)     1173 2023-06-06 12:56:58.612796 cs-3.1.0/setup.cfg
--rw-r--r--   0 brute     (1000) brute     (1000)      140 2023-06-06 12:23:45.000000 cs-3.1.0/setup.py
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-22 07:16:45.283274 cs-3.2.0/
+-rw-r--r--   0 brute     (1000) brute     (1000)     1501 2023-06-06 12:23:45.000000 cs-3.2.0/LICENSE
+-rw-r--r--   0 brute     (1000) brute     (1000)       42 2023-06-06 12:23:45.000000 cs-3.2.0/MANIFEST.in
+-rw-r--r--   0 brute     (1000) brute     (1000)     8309 2023-06-22 07:16:45.283274 cs-3.2.0/PKG-INFO
+-rw-r--r--   0 brute     (1000) brute     (1000)     7587 2023-06-22 07:15:42.000000 cs-3.2.0/README.rst
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-22 07:16:45.283274 cs-3.2.0/cs/
+-rw-r--r--   0 brute     (1000) brute     (1000)     4381 2023-06-22 07:14:08.000000 cs-3.2.0/cs/__init__.py
+-rw-r--r--   0 brute     (1000) brute     (1000)       59 2023-06-22 07:14:08.000000 cs-3.2.0/cs/__main__.py
+-rw-r--r--   0 brute     (1000) brute     (1000)     4769 2023-06-22 07:14:08.000000 cs-3.2.0/cs/_async.py
+-rw-r--r--   0 brute     (1000) brute     (1000)    18515 2023-06-22 07:14:08.000000 cs-3.2.0/cs/client.py
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-22 07:16:45.283274 cs-3.2.0/cs.egg-info/
+-rw-r--r--   0 brute     (1000) brute     (1000)     8309 2023-06-22 07:16:45.000000 cs-3.2.0/cs.egg-info/PKG-INFO
+-rw-r--r--   0 brute     (1000) brute     (1000)      303 2023-06-22 07:16:45.000000 cs-3.2.0/cs.egg-info/SOURCES.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        1 2023-06-22 07:16:45.000000 cs-3.2.0/cs.egg-info/dependency_links.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)       31 2023-06-22 07:16:45.000000 cs-3.2.0/cs.egg-info/entry_points.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        1 2023-06-06 12:56:58.000000 cs-3.2.0/cs.egg-info/not-zip-safe
+-rw-r--r--   0 brute     (1000) brute     (1000)       53 2023-06-22 07:16:45.000000 cs-3.2.0/cs.egg-info/requires.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        3 2023-06-22 07:16:45.000000 cs-3.2.0/cs.egg-info/top_level.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)       30 2023-06-22 07:14:08.000000 cs-3.2.0/pyproject.toml
+-rw-r--r--   0 brute     (1000) brute     (1000)     1214 2023-06-22 07:16:45.283274 cs-3.2.0/setup.cfg
+-rw-r--r--   0 brute     (1000) brute     (1000)      140 2023-06-06 12:23:45.000000 cs-3.2.0/setup.py
```

### Comparing `cs-3.1.0/LICENSE` & `cs-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cs-3.1.0/PKG-INFO` & `cs-3.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: cs
-Version: 3.1.0
+Version: 3.2.0
 Summary: A simple yet powerful CloudStack API client for Python and the command-line.
 Home-page: https://github.com/exoscale/cs
 Author: Bruno Renié
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: async
 Provides-Extra: highlight
 License-File: LICENSE
 
 CS
 ==
 
-.. image:: https://travis-ci.org/exoscale/cs.svg?branch=master
-   :alt: Build Status
-   :target: https://travis-ci.org/exoscale/cs
-
 .. image:: https://img.shields.io/pypi/l/cs.svg
    :alt: License
    :target: https://pypi.org/project/cs/
 
 .. image:: https://img.shields.io/pypi/pyversions/cs.svg
    :alt: Python versions
    :target: https://pypi.org/project/cs/
@@ -84,14 +81,16 @@
     endpoint = https://api.exoscale.ch/v1
     key = cloudstack api key
     secret = cloudstack api secret
     # Optional ca authority certificate
     verify = /path/to/certs/exoscale_ca.crt
     # Optional client PEM certificate
     cert = /path/to/client_exoscale.pem
+    # If you need to pass the certificate and key as separate files
+    cert_key = /path/to/client_key.pem
 
 Then:
 
 .. code-block:: console
 
     $ cs listVirtualMachines
 
@@ -125,14 +124,15 @@
 Configuration is read from several locations, in the following order:
 
 * The ``CLOUDSTACK_ENDPOINT``, ``CLOUDSTACK_KEY``, ``CLOUDSTACK_SECRET`` and
   ``CLOUDSTACK_METHOD`` environment variables,
 * A ``CLOUDSTACK_CONFIG`` environment variable pointing to an ``.ini`` file,
 * A ``CLOUDSTACK_VERIFY`` (optional) environment variable pointing to a CA authority cert file,
 * A ``CLOUDSTACK_CERT`` (optional) environment variable pointing to a client PEM cert file,
+* A ``CLOUDSTACK_CERT_KEY`` (optional) environment variable pointing to a client PEM certificate key file,
 * A ``cloudstack.ini`` file in the current working directory,
 * A ``.cloudstack.ini`` file in the home directory.
 
 To use that configuration scheme from your Python code:
 
 .. code-block:: python
 
@@ -265,18 +265,18 @@
 
 Release Procedure
 -----------------
 
 .. code-block:: shell-session
 
     mktmpenv -p /usr/bin/python3
-    pip install -U twine wheel
+    pip install -U twine wheel build
     cd exoscale/cs
     rm -rf build dist
-    python setup.py sdist bdist_wheel
+    python -m build
     twine upload dist/*
 
 Links
 -----
 
 * CloudStack API: http://cloudstack.apache.org/api.html
 * Example of use: `Get Started with the exoscale API client <https://www.exoscale.com/syslog/2016/02/23/get-started-with-the-exoscale-api-client/>`_
```

### Comparing `cs-3.1.0/README.rst` & `cs-3.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 CS
 ==
 
-.. image:: https://travis-ci.org/exoscale/cs.svg?branch=master
-   :alt: Build Status
-   :target: https://travis-ci.org/exoscale/cs
-
 .. image:: https://img.shields.io/pypi/l/cs.svg
    :alt: License
    :target: https://pypi.org/project/cs/
 
 .. image:: https://img.shields.io/pypi/pyversions/cs.svg
    :alt: Python versions
    :target: https://pypi.org/project/cs/
@@ -65,14 +61,16 @@
     endpoint = https://api.exoscale.ch/v1
     key = cloudstack api key
     secret = cloudstack api secret
     # Optional ca authority certificate
     verify = /path/to/certs/exoscale_ca.crt
     # Optional client PEM certificate
     cert = /path/to/client_exoscale.pem
+    # If you need to pass the certificate and key as separate files
+    cert_key = /path/to/client_key.pem
 
 Then:
 
 .. code-block:: console
 
     $ cs listVirtualMachines
 
@@ -106,14 +104,15 @@
 Configuration is read from several locations, in the following order:
 
 * The ``CLOUDSTACK_ENDPOINT``, ``CLOUDSTACK_KEY``, ``CLOUDSTACK_SECRET`` and
   ``CLOUDSTACK_METHOD`` environment variables,
 * A ``CLOUDSTACK_CONFIG`` environment variable pointing to an ``.ini`` file,
 * A ``CLOUDSTACK_VERIFY`` (optional) environment variable pointing to a CA authority cert file,
 * A ``CLOUDSTACK_CERT`` (optional) environment variable pointing to a client PEM cert file,
+* A ``CLOUDSTACK_CERT_KEY`` (optional) environment variable pointing to a client PEM certificate key file,
 * A ``cloudstack.ini`` file in the current working directory,
 * A ``.cloudstack.ini`` file in the home directory.
 
 To use that configuration scheme from your Python code:
 
 .. code-block:: python
 
@@ -246,18 +245,18 @@
 
 Release Procedure
 -----------------
 
 .. code-block:: shell-session
 
     mktmpenv -p /usr/bin/python3
-    pip install -U twine wheel
+    pip install -U twine wheel build
     cd exoscale/cs
     rm -rf build dist
-    python setup.py sdist bdist_wheel
+    python -m build
     twine upload dist/*
 
 Links
 -----
 
 * CloudStack API: http://cloudstack.apache.org/api.html
 * Example of use: `Get Started with the exoscale API client <https://www.exoscale.com/syslog/2016/02/23/get-started-with-the-exoscale-api-client/>`_
```

### Comparing `cs-3.1.0/cs/__init__.py` & `cs-3.2.0/cs/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,29 +17,34 @@
 except ImportError:
     pygments = None
 
 from .client import (
     CloudStack,
     CloudStackApiException,
     CloudStackException,
-    read_config
+    read_config,
 )
 
 
-__all__ = ['read_config', 'CloudStack', 'CloudStackException',
-           'CloudStackApiException']
+__all__ = [
+    "read_config",
+    "CloudStack",
+    "CloudStackException",
+    "CloudStackApiException",
+]
 
 if sys.version_info >= (3, 5):
     try:
         import aiohttp  # noqa
     except ImportError:
         pass
     else:
         from ._async import AIOCloudStack  # noqa
-        __all__.append('AIOCloudStack')
+
+        __all__.append("AIOCloudStack")
 
 
 def _format_json(data, theme):
     """Pretty print a dict as a JSON, with colors if pygments is present."""
     output = json.dumps(data, indent=2, sort_keys=True)
 
     if pygments and sys.stdout.isatty():
@@ -47,72 +52,99 @@
         formatter = Terminal256Formatter(style=style)
         return pygments.highlight(output, JsonLexer(), formatter)
 
     return output
 
 
 def main(args=None):
-    parser = argparse.ArgumentParser(description='Cloustack client.')
-    parser.add_argument('--region', '-r', metavar='REGION',
-                        help='Cloudstack region in ~/.cloudstack.ini',
-                        default=os.environ.get('CLOUDSTACK_REGION',
-                                               'cloudstack'))
-    parser.add_argument('--theme', metavar='THEME',
-                        help='Pygments style',
-                        default=os.environ.get('CLOUDSTACK_THEME',
-                                               'default'))
-    parser.add_argument('--post', action='store_true', default=False,
-                        help='use POST instead of GET')
-    parser.add_argument('--async', action='store_true', default=False,
-                        help='do not wait for async result')
-    parser.add_argument('--quiet', '-q', action='store_true', default=False,
-                        help='do not display additional status messages')
-    parser.add_argument('--trace', '-t', action='store_true',
-                        default=os.environ.get('CLOUDSTACK_TRACE', False),
-                        help='trace the HTTP requests done on stderr')
-    parser.add_argument('command', metavar="COMMAND",
-                        help='Cloudstack API command to execute')
+    parser = argparse.ArgumentParser(description="Cloustack client.")
+    parser.add_argument(
+        "--region",
+        "-r",
+        metavar="REGION",
+        help="Cloudstack region in ~/.cloudstack.ini",
+        default=os.environ.get("CLOUDSTACK_REGION", "cloudstack"),
+    )
+    parser.add_argument(
+        "--theme",
+        metavar="THEME",
+        help="Pygments style",
+        default=os.environ.get("CLOUDSTACK_THEME", "default"),
+    )
+    parser.add_argument(
+        "--post",
+        action="store_true",
+        default=False,
+        help="use POST instead of GET",
+    )
+    parser.add_argument(
+        "--async",
+        action="store_true",
+        default=False,
+        help="do not wait for async result",
+    )
+    parser.add_argument(
+        "--quiet",
+        "-q",
+        action="store_true",
+        default=False,
+        help="do not display additional status messages",
+    )
+    parser.add_argument(
+        "--trace",
+        "-t",
+        action="store_true",
+        default=os.environ.get("CLOUDSTACK_TRACE", False),
+        help="trace the HTTP requests done on stderr",
+    )
+    parser.add_argument(
+        "command", metavar="COMMAND", help="Cloudstack API command to execute"
+    )
 
     def parse_option(x):
-        if '=' not in x:
-            raise ValueError("{!r} is not a correctly formatted "
-                             "option".format(x))
-        return x.split('=', 1)
-
-    parser.add_argument('arguments', metavar="OPTION=VALUE",
-                        nargs='*', type=parse_option,
-                        help='Cloudstack API argument')
+        if "=" not in x:
+            raise ValueError(
+                "{!r} is not a correctly formatted " "option".format(x)
+            )
+        return x.split("=", 1)
+
+    parser.add_argument(
+        "arguments",
+        metavar="OPTION=VALUE",
+        nargs="*",
+        type=parse_option,
+        help="Cloudstack API argument",
+    )
 
     options = parser.parse_args(args=args)
     command = options.command
     kwargs = defaultdict(set)
     for arg in options.arguments:
         key, value = arg
         kwargs[key].add(value.strip(" \"'"))
 
     try:
         config = read_config(ini_group=options.region)
     except NoSectionError:
         raise SystemExit("Error: region '%s' not in config" % options.region)
 
-    theme = config.pop('theme', 'default')
+    theme = config.pop("theme", "default")
 
-    fetch_result = 'Async' not in command and not getattr(options, 'async')
+    fetch_result = "Async" not in command and not getattr(options, "async")
 
     if options.post:
-        config['method'] = 'post'
+        config["method"] = "post"
     if options.trace:
-        config['trace'] = True
+        config["trace"] = True
     cs = CloudStack(**config)
     ok = True
     response = None
 
     try:
-        response = getattr(cs, command)(fetch_result=fetch_result,
-                                        **kwargs)
+        response = getattr(cs, command)(fetch_result=fetch_result, **kwargs)
     except CloudStackException as e:
         ok = False
         if e.response is not None:
             if not options.quiet:
                 sys.stderr.write("CloudStack error: ")
                 sys.stderr.write("\n".join((str(arg) for arg in e.args)))
                 sys.stderr.write("\n")
@@ -124,10 +156,10 @@
                 sys.stderr.write("\n")
         else:
             message, data = (e.args[0], e.args[0:])
             sys.stderr.write("Error: {0}\n{1}\n".format(message, data))
 
     if response:
         sys.stdout.write(_format_json(response, theme=theme))
-        sys.stdout.write('\n')
+        sys.stdout.write("\n")
 
     return not ok
```

### Comparing `cs-3.1.0/cs/_async.py` & `cs-3.2.0/cs/_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,106 +7,131 @@
 from .client import PENDING, SUCCESS, transform
 
 
 class AIOCloudStack(CloudStack):
     def __getattr__(self, command):
         def handler(**kwargs):
             return self._request(command, **kwargs)
+
         return handler
 
-    async def _request(self, command, json=True, opcode_name='command',
-                       fetch_list=False, headers=None, **params):
+    async def _request(
+        self,
+        command,
+        json=True,
+        opcode_name="command",
+        fetch_list=False,
+        headers=None,
+        **params
+    ):
         fetch_result = params.pop("fetch_result", self.fetch_result)
-        kwarg, kwargs = self._prepare_request(command, json, opcode_name,
-                                              fetch_list, **params)
+        kwarg, kwargs = self._prepare_request(
+            command, json, opcode_name, fetch_list, **params
+        )
 
         ssl_context = None
         if self.cert:
             ssl_context = ssl.create_default_context(cafile=self.cert)
-        connector = aiohttp.TCPConnector(verify_ssl=self.verify,
-                                         ssl_context=ssl_context)
-
-        async with aiohttp.ClientSession(read_timeout=self.timeout,
-                                         conn_timeout=self.timeout,
-                                         connector=connector) as session:
+        connector = aiohttp.TCPConnector(
+            verify_ssl=self.verify, ssl_context=ssl_context
+        )
+
+        async with aiohttp.ClientSession(
+            read_timeout=self.timeout,
+            conn_timeout=self.timeout,
+            connector=connector,
+        ) as session:
             handler = getattr(session, self.method)
 
             done = False
             final_data = []
             page = 1
             while not done:
                 if fetch_list:
-                    kwargs['page'] = page
+                    kwargs["page"] = page
 
                 transform(kwargs)
-                kwargs.pop('signature', None)
+                kwargs.pop("signature", None)
                 self._sign(kwargs)
-                response = await handler(self.endpoint,
-                                         headers=headers,
-                                         **{kwarg: kwargs})
+                response = await handler(
+                    self.endpoint, headers=headers, **{kwarg: kwargs}
+                )
 
-                ctype = response.headers['content-type'].split(';')[0]
+                ctype = response.headers["content-type"].split(";")[0]
                 try:
                     data = await response.json(content_type=ctype)
                 except ValueError as e:
                     msg = "Make sure endpoint URL {!r} is correct.".format(
-                        self.endpoint)
+                        self.endpoint
+                    )
                     raise CloudStackException(
                         "HTTP {0} response from CloudStack".format(
-                            response.status),
+                            response.status
+                        ),
                         "{}. {}".format(e, msg),
                         response=response,
                     )
 
                 [key] = data.keys()
                 data = data[key]
                 if response.status != 200:
                     raise CloudStackApiException(
                         "HTTP {0} response from CloudStack".format(
-                            response.status), error=data, response=response)
+                            response.status
+                        ),
+                        error=data,
+                        response=response,
+                    )
                 if fetch_list:
                     try:
-                        [key] = [k for k in data.keys() if k != 'count']
+                        [key] = [k for k in data.keys() if k != "count"]
                     except ValueError:
                         done = True
                     else:
                         final_data.extend(data[key])
                         page += 1
-                elif fetch_result and 'jobid' in data:
+                elif fetch_result and "jobid" in data:
                     try:
                         final_data = await asyncio.wait_for(
-                            self._jobresult(data['jobid'], response),
-                            self.job_timeout)
+                            self._jobresult(data["jobid"], response),
+                            self.job_timeout,
+                        )
                     except asyncio.TimeoutError:
                         raise CloudStackException(
                             "Timeout waiting for async job result",
-                            data['jobid'],
-                            response=response)
+                            data["jobid"],
+                            response=response,
+                        )
                     done = True
                 else:
                     final_data = data
                     done = True
             return final_data
 
     async def _jobresult(self, jobid, response):
         failures = 0
         while True:
             try:
-                j = await self.queryAsyncJobResult(jobid=jobid,
-                                                   fetch_result=False)
+                j = await self.queryAsyncJobResult(
+                    jobid=jobid, fetch_result=False
+                )
                 failures = 0
-                if j['jobstatus'] != PENDING:
-                    if j['jobresultcode'] != 0 or j['jobstatus'] != SUCCESS:
-                        raise CloudStackApiException("Job failure", j,
-                                                     error=j['jobresult'],
-                                                     response=response)
-                    if 'jobresult' not in j:
-                        raise CloudStackException("Unknown job result", j,
-                                                  response=response)
-                    return j['jobresult']
+                if j["jobstatus"] != PENDING:
+                    if j["jobresultcode"] != 0 or j["jobstatus"] != SUCCESS:
+                        raise CloudStackApiException(
+                            "Job failure",
+                            j,
+                            error=j["jobresult"],
+                            response=response,
+                        )
+                    if "jobresult" not in j:
+                        raise CloudStackException(
+                            "Unknown job result", j, response=response
+                        )
+                    return j["jobresult"]
 
             except CloudStackException:
                 raise
 
             except Exception:
                 failures += 1
                 if failures > 10:
```

### Comparing `cs-3.1.0/cs/client.py` & `cs-3.2.0/cs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,17 +91,17 @@
     are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
     'val' is anything else.
 
     This function has been borrowed from distutils.util module in order
     to avoid pulling a dependency on deprecated module "imp".
     """
     val = val.lower()
-    if val in ('y', 'yes', 't', 'true', 'on', '1'):
+    if val in ("y", "yes", "t", "true", "on", "1"):
         return 1
-    elif val in ('n', 'no', 'f', 'false', 'off', '0'):
+    elif val in ("n", "no", "f", "false", "off", "0"):
         return 0
     else:
         raise ValueError("invalid truth value %r" % (val,))
 
 
 def check_key(key, allowed):
     """
@@ -186,14 +186,17 @@
 
     def __str__(self):
         return "{0}, error: {1}".format(
             super(CloudStackApiException, self).__str__(), self.error
         )
 
 
+ten_minutes = timedelta(minutes=10)
+
+
 class CloudStack(object):
     def __init__(
         self,
         endpoint,
         key,
         secret,
         timeout=10,
@@ -201,15 +204,15 @@
         verify=None,
         cert=None,
         cert_key=None,
         name=None,
         retry=0,
         job_timeout=None,
         poll_interval=POLL_INTERVAL,
-        expiration=timedelta(minutes=10),
+        expiration=ten_minutes,
         trace=False,
         dangerous_no_tls_verify=False,
         headers=None,
         session=None,
         fetch_result=False,
     ):
         self.endpoint = endpoint
@@ -235,163 +238,184 @@
         if not hasattr(expiration, "seconds"):
             expiration = timedelta(seconds=int(expiration))
         self.expiration = expiration
         self.trace = bool(trace)
         self.fetch_result = fetch_result
 
     def __repr__(self):
-        return '<CloudStack: {0}>'.format(self.name or self.endpoint)
+        return "<CloudStack: {0}>".format(self.name or self.endpoint)
 
     def __getattr__(self, command):
         def handler(**kwargs):
             return self._request(command, **kwargs)
+
         return handler
 
-    def _prepare_request(self, command, json=True, opcode_name='command',
-                         fetch_list=False, **kwargs):
+    def _prepare_request(
+        self,
+        command,
+        json=True,
+        opcode_name="command",
+        fetch_list=False,
+        **kwargs,
+    ):
         params = CaseInsensitiveDict(**kwargs)
-        params.update({
-            'apiKey': self.key,
-            opcode_name: command,
-        })
+        params.update(
+            {
+                "apiKey": self.key,
+                opcode_name: command,
+            }
+        )
         if json:
-            params['response'] = 'json'
-        if 'page' in kwargs or fetch_list:
-            params.setdefault('pagesize', PAGE_SIZE)
-        if 'expires' not in params and self.expiration.total_seconds() >= 0:
-            params['signatureVersion'] = '3'
+            params["response"] = "json"
+        if "page" in kwargs or fetch_list:
+            params.setdefault("pagesize", PAGE_SIZE)
+        if "expires" not in params and self.expiration.total_seconds() >= 0:
+            params["signatureVersion"] = "3"
             tz = pytz.utc
             expires = tz.localize(datetime.utcnow() + self.expiration)
-            params['expires'] = expires.astimezone(tz).strftime(EXPIRES_FORMAT)
+            params["expires"] = expires.astimezone(tz).strftime(EXPIRES_FORMAT)
 
-        kind = 'params' if self.method == 'get' else 'data'
+        kind = "params" if self.method == "get" else "data"
         return kind, dict(params.items())
 
-    def _request(self, command, json=True, opcode_name='command',
-                 fetch_list=False, headers=None, **params):
-        fetch_result = params.pop('fetch_result', self.fetch_result)
-        kind, params = self._prepare_request(command, json, opcode_name,
-                                             fetch_list, **params)
+    def _request(
+        self,
+        command,
+        json=True,
+        opcode_name="command",
+        fetch_list=False,
+        headers=None,
+        **params,
+    ):
+        fetch_result = params.pop("fetch_result", self.fetch_result)
+        kind, params = self._prepare_request(
+            command, json, opcode_name, fetch_list, **params
+        )
         if headers is None:
             headers = {}
         headers.update(self.headers)
 
         done = False
         max_retry = self.retry
         final_data = []
         page = 1
         while not done:
             if fetch_list:
-                params['page'] = page
+                params["page"] = page
 
             transform(params)
-            params.pop('signature', None)
+            params.pop("signature", None)
             self._sign(params)
 
-            req = requests.Request(self.method,
-                                   self.endpoint,
-                                   headers=headers,
-                                   **{kind: params})
+            req = requests.Request(
+                self.method, self.endpoint, headers=headers, **{kind: params}
+            )
             prepped = req.prepare()
             if self.trace:
                 print(prepped.method, prepped.url, file=sys.stderr)
                 if prepped.headers:
                     print(prepped.headers, "\n", file=sys.stderr)
                 if prepped.body:
                     print(prepped.body, file=sys.stderr)
                 else:
                     print(file=sys.stderr)
 
             try:
                 with self.session as session:
-                    response = session.send(prepped,
-                                            timeout=self.timeout,
-                                            verify=self.verify,
-                                            cert=self.cert)
+                    response = session.send(
+                        prepped,
+                        timeout=self.timeout,
+                        verify=self.verify,
+                        cert=self.cert,
+                    )
 
             except requests.exceptions.ConnectionError:
                 max_retry -= 1
-                if (
-                    max_retry < 0 or
-                    not command.startswith(('list', 'queryAsync'))
+                if max_retry < 0 or not command.startswith(
+                    ("list", "queryAsync")
                 ):
                     raise
                 continue
             max_retry = self.retry
 
             if self.trace:
                 print(response.status_code, response.reason, file=sys.stderr)
-                headersTrace = "\n".join("{}: {}".format(k, v)
-                                         for k, v in response.headers.items())
+                headersTrace = "\n".join(
+                    "{}: {}".format(k, v) for k, v in response.headers.items()
+                )
                 print(headersTrace, "\n", file=sys.stderr)
                 print(response.text, "\n", file=sys.stderr)
 
             data = self._response_value(response, json)
 
             if fetch_list:
                 try:
-                    [key] = [k for k in data.keys() if k != 'count']
+                    [key] = [k for k in data.keys() if k != "count"]
                 except ValueError:
                     done = True
                 else:
                     final_data.extend(data[key])
                     page += 1
-                    if len(final_data) >= data.get('count', PAGE_SIZE):
+                    if len(final_data) >= data.get("count", PAGE_SIZE):
                         done = True
-            elif fetch_result and 'jobid' in data:
-                final_data = self._jobresult(jobid=data['jobid'],
-                                             headers=headers)
+            elif fetch_result and "jobid" in data:
+                final_data = self._jobresult(
+                    jobid=data["jobid"], headers=headers
+                )
                 done = True
             else:
                 final_data = data
                 done = True
         return final_data
 
     def _response_value(self, response, json=True):
         """Parses the HTTP response as a the cloudstack value.
 
         It throws an exception if the server didn't answer with a 200.
         """
         if json:
-            contentType = response.headers.get("Content-Type", "")
-            if not contentType.startswith(("application/json",
-                                           "text/javascript")):
+            ctype = response.headers.get("Content-Type", "")
+            if not ctype.startswith(("application/json", "text/javascript")):
                 if response.status_code == 200:
-                    raise CloudStackException(
-                        "JSON (application/json) was expected, got {!r}"
-                        .format(contentType),
-                        response=response)
+                    msg = (
+                        f"JSON (application/json) was expected, got {ctype:!r}"
+                    )
+                    raise CloudStackException(msg, response=response)
 
                 raise CloudStackException(
-                    "HTTP {0.status_code} {0.reason}"
-                    .format(response),
-                    "Make sure endpoint URL {!r} is correct."
-                    .format(self.endpoint),
-                    response=response)
+                    "HTTP {0.status_code} {0.reason}".format(response),
+                    "Make sure endpoint URL {!r} is correct.".format(
+                        self.endpoint
+                    ),
+                    response=response,
+                )
 
             try:
                 data = response.json()
             except ValueError as e:
                 raise CloudStackException(
-                    "HTTP {0.status_code} {0.reason}"
-                    .format(response),
+                    "HTTP {0.status_code} {0.reason}".format(response),
                     "{0!s}. Malformed JSON document".format(e),
-                    response=response)
+                    response=response,
+                )
 
             [key] = data.keys()
             data = data[key]
         else:
             data = response.text
 
         if response.status_code != 200:
             raise CloudStackApiException(
                 "HTTP {0} response from CloudStack".format(
-                    response.status_code),
+                    response.status_code
+                ),
                 error=data,
-                response=response)
+                response=response,
+            )
 
         return data
 
     def _jobresult(self, jobid, json=True, headers=None):
         """Poll the async job result.
 
         To be run via in a Thread, the result is put within
@@ -402,63 +426,73 @@
         total_time = self.job_timeout or 2**30
         remaining = timedelta(seconds=total_time)
         endtime = datetime.now() + remaining
 
         while remaining.total_seconds() > 0:
             timeout = max(min(self.timeout, remaining.total_seconds()), 1)
             try:
-                kind, params = self._prepare_request('queryAsyncJobResult',
-                                                     jobid=jobid)
+                kind, params = self._prepare_request(
+                    "queryAsyncJobResult", jobid=jobid
+                )
 
                 transform(params)
                 self._sign(params)
 
-                req = requests.Request(self.method,
-                                       self.endpoint,
-                                       headers=headers,
-                                       **{kind: params})
+                req = requests.Request(
+                    self.method,
+                    self.endpoint,
+                    headers=headers,
+                    **{kind: params},
+                )
                 prepped = req.prepare()
                 if self.trace:
                     print(prepped.method, prepped.url, file=sys.stderr)
                     if prepped.headers:
                         print(prepped.headers, "\n", file=sys.stderr)
                     if prepped.body:
                         print(prepped.body, file=sys.stderr)
                     else:
                         print(file=sys.stderr)
 
                 with self.session as session:
-                    response = session.send(prepped,
-                                            timeout=timeout,
-                                            verify=self.verify,
-                                            cert=self.cert)
+                    response = session.send(
+                        prepped,
+                        timeout=timeout,
+                        verify=self.verify,
+                        cert=self.cert,
+                    )
 
                 j = self._response_value(response, json)
 
                 if self.trace:
-                    print(response.status_code, response.reason,
-                          file=sys.stderr)
+                    print(
+                        response.status_code, response.reason, file=sys.stderr
+                    )
                     headersTrace = "\n".join(
-                            "{}: {}".format(k, v)
-                            for k, v in response.headers.items())
+                        "{}: {}".format(k, v)
+                        for k, v in response.headers.items()
+                    )
                     print(headersTrace, "\n", file=sys.stderr)
                     print(response.text, "\n", file=sys.stderr)
 
                 failures = 0
-                if j['jobstatus'] != PENDING:
-                    if j['jobresultcode'] or j['jobstatus'] != SUCCESS:
-                        raise CloudStackApiException("Job failure",
-                                                     error=j['jobresult'],
-                                                     response=response)
-
-                    if 'jobresult' not in j:
-                        raise CloudStackException("Unknown job result",
-                                                  response=response)
+                if j["jobstatus"] != PENDING:
+                    if j["jobresultcode"] or j["jobstatus"] != SUCCESS:
+                        raise CloudStackApiException(
+                            "Job failure",
+                            error=j["jobresult"],
+                            response=response,
+                        )
+
+                    if "jobresult" not in j:
+                        raise CloudStackException(
+                            "Unknown job result", response=response
+                        )
 
-                    return j['jobresult']
+                    return j["jobresult"]
 
             except CloudStackException:
                 raise
 
             except Exception:
                 failures += 1
                 if failures > 10:
@@ -466,56 +500,58 @@
 
             time.sleep(self.poll_interval)
             remaining = endtime - datetime.now()
 
         if response:
             response.status_code = 408
 
-        raise CloudStackException("Timeout waiting for async job result",
-                                  jobid,
-                                  response=response)
+        raise CloudStackException(
+            "Timeout waiting for async job result", jobid, response=response
+        )
 
     def _sign(self, data):
         """
         Compute a signature string according to the CloudStack
         signature method (hmac/sha1).
         """
 
         # Python2/3 urlencode aren't good enough for this task.
         params = "&".join(
             "=".join((key, cs_encode(value)))
             for key, value in sorted(data.items())
         )
 
         digest = hmac.new(
-            self.secret.encode('utf-8'),
-            msg=params.lower().encode('utf-8'),
-            digestmod=hashlib.sha1).digest()
+            self.secret.encode("utf-8"),
+            msg=params.lower().encode("utf-8"),
+            digestmod=hashlib.sha1,
+        ).digest()
 
-        data['signature'] = base64.b64encode(digest).decode('utf-8').strip()
+        data["signature"] = base64.b64encode(digest).decode("utf-8").strip()
 
 
 def read_config_from_ini(ini_group=None):
     # Config file: $PWD/cloudstack.ini or $HOME/.cloudstack.ini
     # Last read wins in configparser
     paths = [
-        os.path.join(os.path.expanduser('~'), '.cloudstack.ini'),
-        os.path.join(os.getcwd(), 'cloudstack.ini'),
+        os.path.join(os.path.expanduser("~"), ".cloudstack.ini"),
+        os.path.join(os.getcwd(), "cloudstack.ini"),
     ]
     # Look at CLOUDSTACK_CONFIG first if present
-    if 'CLOUDSTACK_CONFIG' in os.environ:
-        paths.append(os.path.expanduser(os.environ['CLOUDSTACK_CONFIG']))
+    if "CLOUDSTACK_CONFIG" in os.environ:
+        paths.append(os.path.expanduser(os.environ["CLOUDSTACK_CONFIG"]))
     if not any([os.path.exists(c) for c in paths]):
-        raise SystemExit("Config file not found. Tried {0}".format(
-            ", ".join(paths)))
+        raise SystemExit(
+            "Config file not found. Tried {0}".format(", ".join(paths))
+        )
     conf = ConfigParser()
     conf.read(paths)
 
     if not ini_group:
-        ini_group = os.getenv('CLOUDSTACK_REGION', 'cloudstack')
+        ini_group = os.getenv("CLOUDSTACK_REGION", "cloudstack")
 
         if not conf.has_section(ini_group):
             return dict(name=None)
 
     ini_config = {
         k: v
         for k, v in conf.items(ini_group)
@@ -523,15 +559,16 @@
     }
     ini_config["name"] = ini_group
 
     # Convert individual header_* settings into a single dict
     for k in list(ini_config):
         if k.startswith("header_"):
             ini_config.setdefault("headers", {})
-            ini_config["headers"][k[len("header_"):]] = ini_config.pop(k)
+            start = len("header_")
+            ini_config["headers"][k[start:]] = ini_config.pop(k)
     return ini_config
 
 
 def read_config(ini_group=None):
     """
     Read the configuration from the environment, or config.
 
@@ -542,32 +579,36 @@
     for key in REQUIRED_CONFIG_KEYS.union(ALLOWED_CONFIG_KEYS):
         env_key = "CLOUDSTACK_{0}".format(key.upper())
         value = os.getenv(env_key)
         if value:
             env_conf[key] = value
 
     # overrides means we have a .ini to read
-    overrides = os.getenv('CLOUDSTACK_OVERRIDES', '').strip()
+    overrides = os.getenv("CLOUDSTACK_OVERRIDES", "").strip()
 
     if not overrides and set(env_conf).issuperset(REQUIRED_CONFIG_KEYS):
         return env_conf
 
     ini_conf = read_config_from_ini(ini_group)
 
-    overrides = {s.lower() for s in re.split(r'\W+', overrides)}
-    config = dict(dict(env_conf, **ini_conf),
-                  **{k: v for k, v in env_conf.items() if k in overrides})
+    overrides = {s.lower() for s in re.split(r"\W+", overrides)}
+    config = dict(
+        dict(env_conf, **ini_conf),
+        **{k: v for k, v in env_conf.items() if k in overrides},
+    )
 
     missings = REQUIRED_CONFIG_KEYS.difference(config)
     if missings:
-        raise ValueError("the configuration is missing the following keys: " +
-                         ", ".join(missings))
+        raise ValueError(
+            "the configuration is missing the following keys: "
+            + ", ".join(missings)
+        )
 
     # convert booleans values.
-    bool_keys = ('dangerous_no_tls_verify',)
+    bool_keys = ("dangerous_no_tls_verify",)
     for bool_key in bool_keys:
         if isinstance(config[bool_key], string_type):
             try:
                 config[bool_key] = strtobool(config[bool_key])
             except ValueError:
                 pass
```

### Comparing `cs-3.1.0/cs.egg-info/PKG-INFO` & `cs-3.2.0/cs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: cs
-Version: 3.1.0
+Version: 3.2.0
 Summary: A simple yet powerful CloudStack API client for Python and the command-line.
 Home-page: https://github.com/exoscale/cs
 Author: Bruno Renié
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: async
 Provides-Extra: highlight
 License-File: LICENSE
 
 CS
 ==
 
-.. image:: https://travis-ci.org/exoscale/cs.svg?branch=master
-   :alt: Build Status
-   :target: https://travis-ci.org/exoscale/cs
-
 .. image:: https://img.shields.io/pypi/l/cs.svg
    :alt: License
    :target: https://pypi.org/project/cs/
 
 .. image:: https://img.shields.io/pypi/pyversions/cs.svg
    :alt: Python versions
    :target: https://pypi.org/project/cs/
@@ -84,14 +81,16 @@
     endpoint = https://api.exoscale.ch/v1
     key = cloudstack api key
     secret = cloudstack api secret
     # Optional ca authority certificate
     verify = /path/to/certs/exoscale_ca.crt
     # Optional client PEM certificate
     cert = /path/to/client_exoscale.pem
+    # If you need to pass the certificate and key as separate files
+    cert_key = /path/to/client_key.pem
 
 Then:
 
 .. code-block:: console
 
     $ cs listVirtualMachines
 
@@ -125,14 +124,15 @@
 Configuration is read from several locations, in the following order:
 
 * The ``CLOUDSTACK_ENDPOINT``, ``CLOUDSTACK_KEY``, ``CLOUDSTACK_SECRET`` and
   ``CLOUDSTACK_METHOD`` environment variables,
 * A ``CLOUDSTACK_CONFIG`` environment variable pointing to an ``.ini`` file,
 * A ``CLOUDSTACK_VERIFY`` (optional) environment variable pointing to a CA authority cert file,
 * A ``CLOUDSTACK_CERT`` (optional) environment variable pointing to a client PEM cert file,
+* A ``CLOUDSTACK_CERT_KEY`` (optional) environment variable pointing to a client PEM certificate key file,
 * A ``cloudstack.ini`` file in the current working directory,
 * A ``.cloudstack.ini`` file in the home directory.
 
 To use that configuration scheme from your Python code:
 
 .. code-block:: python
 
@@ -265,18 +265,18 @@
 
 Release Procedure
 -----------------
 
 .. code-block:: shell-session
 
     mktmpenv -p /usr/bin/python3
-    pip install -U twine wheel
+    pip install -U twine wheel build
     cd exoscale/cs
     rm -rf build dist
-    python setup.py sdist bdist_wheel
+    python -m build
     twine upload dist/*
 
 Links
 -----
 
 * CloudStack API: http://cloudstack.apache.org/api.html
 * Example of use: `Get Started with the exoscale API client <https://www.exoscale.com/syslog/2016/02/23/get-started-with-the-exoscale-api-client/>`_
```

### Comparing `cs-3.1.0/setup.cfg` & `cs-3.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [metadata]
 name = cs
-version = 3.1.0
+version = 3.2.0
 url = https://github.com/exoscale/cs
 author = Bruno Renié
 description = A simple yet powerful CloudStack API client for Python and the command-line.
 long_description = file: README.rst
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
 	pytz
```

