# Comparing `tmp/requests_pkcs12-1.8.tar.gz` & `tmp/requests_pkcs12-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/requests_pkcs12-1.8.tar", last modified: Wed Aug 19 10:44:49 2020, max compression
+gzip compressed data, was "dist/requests_pkcs12-1.9.tar", last modified: Fri Oct  2 15:43:19 2020, max compression
```

## Comparing `requests_pkcs12-1.8.tar` & `requests_pkcs12-1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 vog       (1000) vog       (1000)        0 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/
--rw-------   0 vog       (1000) vog       (1000)      730 2018-06-22 20:27:38.000000 requests_pkcs12-1.8/LICENSE
--rw-------   0 vog       (1000) vog       (1000)       16 2018-06-22 20:27:38.000000 requests_pkcs12-1.8/MANIFEST.in
--rw-------   0 vog       (1000) vog       (1000)     3760 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/PKG-INFO
--rw-------   0 vog       (1000) vog       (1000)     2586 2020-07-04 06:17:39.000000 requests_pkcs12-1.8/README.rst
-drwx------   0 vog       (1000) vog       (1000)        0 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/requests_pkcs12.egg-info/
--rw-------   0 vog       (1000) vog       (1000)     3760 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/requests_pkcs12.egg-info/PKG-INFO
--rw-------   0 vog       (1000) vog       (1000)      252 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/requests_pkcs12.egg-info/SOURCES.txt
--rw-------   0 vog       (1000) vog       (1000)        1 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/requests_pkcs12.egg-info/dependency_links.txt
--rw-------   0 vog       (1000) vog       (1000)       33 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/requests_pkcs12.egg-info/requires.txt
--rw-------   0 vog       (1000) vog       (1000)       16 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/requests_pkcs12.egg-info/top_level.txt
--rw-------   0 vog       (1000) vog       (1000)     4983 2020-08-19 10:35:07.000000 requests_pkcs12-1.8/requests_pkcs12.py
--rw-------   0 vog       (1000) vog       (1000)       38 2020-08-19 10:44:49.000000 requests_pkcs12-1.8/setup.cfg
--rw-------   0 vog       (1000) vog       (1000)      894 2020-08-19 10:44:22.000000 requests_pkcs12-1.8/setup.py
+drwx------   0 vog       (1000) vog       (1000)        0 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/
+-rw-------   0 vog       (1000) vog       (1000)      730 2018-06-22 20:27:38.000000 requests_pkcs12-1.9/LICENSE
+-rw-------   0 vog       (1000) vog       (1000)       16 2018-06-22 20:27:38.000000 requests_pkcs12-1.9/MANIFEST.in
+-rw-------   0 vog       (1000) vog       (1000)     3760 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/PKG-INFO
+-rw-------   0 vog       (1000) vog       (1000)     2586 2020-07-04 06:17:39.000000 requests_pkcs12-1.9/README.rst
+drwx------   0 vog       (1000) vog       (1000)        0 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/requests_pkcs12.egg-info/
+-rw-------   0 vog       (1000) vog       (1000)     3760 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/requests_pkcs12.egg-info/PKG-INFO
+-rw-------   0 vog       (1000) vog       (1000)      252 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/requests_pkcs12.egg-info/SOURCES.txt
+-rw-------   0 vog       (1000) vog       (1000)        1 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/requests_pkcs12.egg-info/dependency_links.txt
+-rw-------   0 vog       (1000) vog       (1000)       33 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/requests_pkcs12.egg-info/requires.txt
+-rw-------   0 vog       (1000) vog       (1000)       16 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/requests_pkcs12.egg-info/top_level.txt
+-rw-------   0 vog       (1000) vog       (1000)     6135 2020-10-02 15:42:26.000000 requests_pkcs12-1.9/requests_pkcs12.py
+-rw-------   0 vog       (1000) vog       (1000)       38 2020-10-02 15:43:19.000000 requests_pkcs12-1.9/setup.cfg
+-rw-------   0 vog       (1000) vog       (1000)      894 2020-10-02 15:42:38.000000 requests_pkcs12-1.9/setup.py
```

### Comparing `requests_pkcs12-1.8/LICENSE` & `requests_pkcs12-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_pkcs12-1.8/PKG-INFO` & `requests_pkcs12-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: requests_pkcs12
-Version: 1.8
+Version: 1.9
 Summary: Add PKCS#12 support to the requests library in a clean way, without monkey patching or temporary files
 Home-page: https://github.com/m-click/requests_pkcs12
 Author: Volker Diels-Grabsch
 Author-email: volker.diels-grabsch@m-click.aero
 License: ISC
 Description: PKCS#12 support for requests
         ============================
```

### Comparing `requests_pkcs12-1.8/README.rst` & `requests_pkcs12-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `requests_pkcs12-1.8/requests_pkcs12.egg-info/PKG-INFO` & `requests_pkcs12-1.9/requests_pkcs12.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: requests-pkcs12
-Version: 1.8
+Version: 1.9
 Summary: Add PKCS#12 support to the requests library in a clean way, without monkey patching or temporary files
 Home-page: https://github.com/m-click/requests_pkcs12
 Author: Volker Diels-Grabsch
 Author-email: volker.diels-grabsch@m-click.aero
 License: ISC
 Description: PKCS#12 support for requests
         ============================
```

### Comparing `requests_pkcs12-1.8/requests_pkcs12.py` & `requests_pkcs12-1.9/requests_pkcs12.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,44 +12,75 @@
 MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 '''
 
-from OpenSSL.crypto import load_pkcs12
+import os
+from OpenSSL.crypto import load_pkcs12, dump_certificate, dump_privatekey, FILETYPE_PEM
 from datetime import datetime
 from requests import Session
 from requests import request as request_orig
 from requests.adapters import HTTPAdapter
 from urllib3.contrib.pyopenssl import PyOpenSSLContext
+from ssl import SSLContext
+from tempfile import NamedTemporaryFile
+
 try:
     from ssl import PROTOCOL_TLS as ssl_protocol
 except ImportError:
     from ssl import PROTOCOL_SSLv23 as ssl_protocol
 
 def check_cert_not_after(cert):
     cert_not_after = datetime.strptime(cert.get_notAfter().decode('ascii'), '%Y%m%d%H%M%SZ')
     if cert_not_after < datetime.utcnow():
         raise ValueError('Client certificate expired: Not After: {cert_not_after:%Y-%m-%d %H:%M:%SZ}'.format(**locals()))
 
-def create_ssl_context(pkcs12_data, pkcs12_password_bytes):
+def create_pyopenssl_sslcontext(pkcs12_data, pkcs12_password_bytes):
     p12 = load_pkcs12(pkcs12_data, pkcs12_password_bytes)
     cert = p12.get_certificate()
     check_cert_not_after(cert)
     ssl_context = PyOpenSSLContext(ssl_protocol)
     ssl_context._ctx.use_certificate(cert)
     ca_certs = p12.get_ca_certificates()
     if ca_certs:
         for ca_cert in ca_certs:
             check_cert_not_after(ca_cert)
             ssl_context._ctx.add_extra_chain_cert(ca_cert)
     ssl_context._ctx.use_privatekey(p12.get_privatekey())
     return ssl_context
 
+def create_ssl_sslcontext(pkcs12_data, pkcs12_password_bytes):
+    cipher = 'blowfish'
+    p12 = load_pkcs12(pkcs12_data, pkcs12_password_bytes)
+    cert = p12.get_certificate()
+    check_cert_not_after(cert)
+    ssl_context = SSLContext(ssl_protocol)
+    with NamedTemporaryFile(delete=False) as c:
+        try:
+            pk_buf = dump_privatekey(FILETYPE_PEM, p12.get_privatekey(), cipher, pkcs12_password_bytes)
+            c.write(pk_buf)
+            buf = dump_certificate(FILETYPE_PEM, p12.get_certificate())
+            c.write(buf)
+            ca_certs = p12.get_ca_certificates()
+            if ca_certs:
+                for ca_cert in ca_certs:
+                    check_cert_not_after(ca_cert)
+                    buf = dump_certificate(FILETYPE_PEM, ca_cert)
+                    c.write(buf)
+
+            c.flush()
+            c.close()
+            ssl_context.load_cert_chain(c.name, password=pkcs12_password_bytes)
+        finally:
+            os.remove(c.name)
+    
+    return ssl_context
+
 class Pkcs12Adapter(HTTPAdapter):
 
     def __init__(self, *args, **kwargs):
         pkcs12_data = kwargs.pop('pkcs12_data', None)
         pkcs12_filename = kwargs.pop('pkcs12_filename', None)
         pkcs12_password = kwargs.pop('pkcs12_password', None)
         if pkcs12_data is None and pkcs12_filename is None:
@@ -61,15 +92,15 @@
         if pkcs12_filename is not None:
             with open(pkcs12_filename, 'rb') as pkcs12_file:
                 pkcs12_data = pkcs12_file.read()
         if isinstance(pkcs12_password, bytes):
             pkcs12_password_bytes = pkcs12_password
         else:
             pkcs12_password_bytes = pkcs12_password.encode('utf8')
-        self.ssl_context = create_ssl_context(pkcs12_data, pkcs12_password_bytes)
+        self.ssl_context = create_pyopenssl_sslcontext(pkcs12_data, pkcs12_password_bytes)
         super(Pkcs12Adapter, self).__init__(*args, **kwargs)
 
     def init_poolmanager(self, *args, **kwargs):
         if self.ssl_context:
             kwargs['ssl_context'] = self.ssl_context
         return super(Pkcs12Adapter, self).init_poolmanager(*args, **kwargs)
```

### Comparing `requests_pkcs12-1.8/setup.py` & `requests_pkcs12-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 setup(
     name='requests_pkcs12',
-    version='1.8',
+    version='1.9',
     description='Add PKCS#12 support to the requests library in a clean way, without monkey patching or temporary files',
     long_description=open('README.rst', 'rb').read().decode('UTF-8'),
     url='https://github.com/m-click/requests_pkcs12',
     author='Volker Diels-Grabsch',
     author_email='volker.diels-grabsch@m-click.aero',
     license='ISC',
     install_requires=[
```

