# Comparing `tmp/netbox_kea-0.1.0.tar.gz` & `tmp/netbox_kea-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_kea-0.1.0.tar", max compression
+gzip compressed data, was "netbox_kea-0.1.1.tar", max compression
```

## Comparing `netbox_kea-0.1.0.tar` & `netbox_kea-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11358 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/LICENSE
--rw-r--r--   0        0        0     3175 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/README.md
--rw-r--r--   0        0        0      288 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/api/__init__.py
--rw-r--r--   0        0        0      719 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/api/serializers.py
--rw-r--r--   0        0        0      190 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/api/urls.py
--rw-r--r--   0        0        0      322 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/api/views.py
--rw-r--r--   0        0        0      364 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/constants.py
--rw-r--r--   0        0        0      229 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/filtersets.py
--rw-r--r--   0        0        0     6620 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/forms.py
--rw-r--r--   0        0        0      404 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/graphql.py
--rw-r--r--   0        0        0     2563 2023-05-18 01:08:43.596195 netbox_kea-0.1.0/netbox_kea/kea.py
--rw-r--r--   0        0        0     1633 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/migrations/0001_initial.py
--rw-r--r--   0        0        0      650 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/migrations/0002_alter_server_options_server_dhcp4_server_dhcp6.py
--rw-r--r--   0        0        0        0 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/migrations/__init__.py
--rw-r--r--   0        0        0     3895 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/models.py
--rw-r--r--   0        0        0      620 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/navigation.py
--rw-r--r--   0        0        0     7495 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/tables.py
--rw-r--r--   0        0        0      360 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/exception_htmx.html
--rw-r--r--   0        0        0      505 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/inc/configure_table.html
--rw-r--r--   0        0        0      991 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server.html
--rw-r--r--   0        0        0       51 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_base.html
--rw-r--r--   0        0        0      492 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_dhcp_leases.html
--rw-r--r--   0        0        0     4547 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_dhcp_leases_htmx.html
--rw-r--r--   0        0        0     1103 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_dhcp_subnets.html
--rw-r--r--   0        0        0     1180 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_leases_delete.html
--rw-r--r--   0        0        0      563 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_status.html
--rw-r--r--   0        0        0      419 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/service_disabled.html
--rw-r--r--   0        0        0      772 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/urls.py
--rw-r--r--   0        0        0     2819 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/utilities.py
--rw-r--r--   0        0        0    17654 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/netbox_kea/views.py
--rw-r--r--   0        0        0      649 2023-05-18 01:08:43.600195 netbox_kea-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 netbox_kea-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3173 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/README.md
+-rw-r--r--   0        0        0      288 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/api/__init__.py
+-rw-r--r--   0        0        0      719 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/api/serializers.py
+-rw-r--r--   0        0        0      190 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/api/urls.py
+-rw-r--r--   0        0        0      322 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/api/views.py
+-rw-r--r--   0        0        0      364 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/constants.py
+-rw-r--r--   0        0        0      229 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/filtersets.py
+-rw-r--r--   0        0        0     6620 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/forms.py
+-rw-r--r--   0        0        0      404 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/graphql.py
+-rw-r--r--   0        0        0     2563 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/kea.py
+-rw-r--r--   0        0        0     1633 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/migrations/0001_initial.py
+-rw-r--r--   0        0        0      650 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/migrations/0002_alter_server_options_server_dhcp4_server_dhcp6.py
+-rw-r--r--   0        0        0        0 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/migrations/__init__.py
+-rw-r--r--   0        0        0     3895 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/models.py
+-rw-r--r--   0        0        0      620 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/navigation.py
+-rw-r--r--   0        0        0     7495 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/tables.py
+-rw-r--r--   0        0        0      360 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/exception_htmx.html
+-rw-r--r--   0        0        0      505 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/inc/configure_table.html
+-rw-r--r--   0        0        0      991 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server.html
+-rw-r--r--   0        0        0       51 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_base.html
+-rw-r--r--   0        0        0      492 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_dhcp_leases.html
+-rw-r--r--   0        0        0     4547 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_dhcp_leases_htmx.html
+-rw-r--r--   0        0        0     1103 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_dhcp_subnets.html
+-rw-r--r--   0        0        0     1180 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_leases_delete.html
+-rw-r--r--   0        0        0      563 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_status.html
+-rw-r--r--   0        0        0      419 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/service_disabled.html
+-rw-r--r--   0        0        0      772 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/urls.py
+-rw-r--r--   0        0        0     2792 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/utilities.py
+-rw-r--r--   0        0        0    17654 2023-06-22 01:31:07.637842 netbox_kea-0.1.1/netbox_kea/views.py
+-rw-r--r--   0        0        0      660 2023-06-22 01:31:07.641842 netbox_kea-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3642 1970-01-01 00:00:00.000000 netbox_kea-0.1.1/PKG-INFO
```

### Comparing `netbox_kea-0.1.0/LICENSE` & `netbox_kea-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/README.md` & `netbox_kea-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NetBox plugin for the Kea DHCP server
 
 This plugin allows you to view Kea status, leases and subnets in NetBox. Go directly from a NetBox device/VM to a DHCP lease and back!
 
 ## Features
 
 - Uses the Kea management API
-- View Kea daemon statuses. 
+- View Kea daemon statuses.
 - Supports Kea's DHCPv4 and DHCPv6 servers.
 - View, delete, export and search for DHCP leases.
 - Search for NetBox devices/VMs directly from DHCP leases.
 - View DHCP subnets from Kea's configuration.
 - REST API and GraphQL support for managing Server objects.
 
 ![Screenshot of DHCP leases](images/leases.png)
@@ -40,15 +40,15 @@
 
 1. Add `netbox-kea` to `local_requirements.txt`.
 
 2. Enable the plugin in `configuration.py`
     ```python
     PLUGINS = ["netbox_kea"]
     ```
-3. Run `./migrate.py migrate`
+3. Run `./manage.py migrate`
 
 ## Custom Links
 
 You can add custom links to NetBox models to easily search for leases.
 
 Make sure to replace `<Kea Server ID>` in the link URL with the object ID of your Kea server. To find a server's ID, open the page for the server
 and look at the top right corner for `netbox_kea.server:<Server ID Here>`.
```

### Comparing `netbox_kea-0.1.0/netbox_kea/api/serializers.py` & `netbox_kea-0.1.1/netbox_kea/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/forms.py` & `netbox_kea-0.1.1/netbox_kea/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/kea.py` & `netbox_kea-0.1.1/netbox_kea/kea.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/migrations/0001_initial.py` & `netbox_kea-0.1.1/netbox_kea/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/migrations/0002_alter_server_options_server_dhcp4_server_dhcp6.py` & `netbox_kea-0.1.1/netbox_kea/migrations/0002_alter_server_options_server_dhcp4_server_dhcp6.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/models.py` & `netbox_kea-0.1.1/netbox_kea/models.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/navigation.py` & `netbox_kea-0.1.1/netbox_kea/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/tables.py` & `netbox_kea-0.1.1/netbox_kea/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server.html` & `netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server.html`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_dhcp_leases_htmx.html` & `netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_dhcp_leases_htmx.html`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_dhcp_subnets.html` & `netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_dhcp_subnets.html`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_leases_delete.html` & `netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_leases_delete.html`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/templates/netbox_kea/server_status.html` & `netbox_kea-0.1.1/netbox_kea/templates/netbox_kea/server_status.html`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/urls.py` & `netbox_kea-0.1.1/netbox_kea/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/netbox_kea/utilities.py` & `netbox_kea-0.1.1/netbox_kea/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
-from collections.abc import Callable
 from datetime import datetime
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Callable, Dict, List, Literal, Optional
 
 from django.http import HttpResponse
 from django.shortcuts import redirect
 from django_tables2 import Table
 from django_tables2.export import TableExport
 from utilities.views import ViewTab
```

### Comparing `netbox_kea-0.1.0/netbox_kea/views.py` & `netbox_kea-0.1.1/netbox_kea/views.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.1.0/pyproject.toml` & `netbox_kea-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "netbox-kea"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
-authors = ["Devon Mar <devonm@mdmm.ca>"]
+authors = ["Devon Mar <devonm+netbox-kea@mdmm.ca>"]
 readme = "README.md"
 packages = [{include = "netbox_kea"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 requests = "^2"
 netaddr = "^0.8.0"
```

### Comparing `netbox_kea-0.1.0/PKG-INFO` & `netbox_kea-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: netbox-kea
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Devon Mar
-Author-email: devonm@mdmm.ca
+Author-email: devonm+netbox-kea@mdmm.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: netaddr (>=0.8.0,<0.9.0)
 Requires-Dist: requests (>=2,<3)
@@ -16,15 +16,15 @@
 # NetBox plugin for the Kea DHCP server
 
 This plugin allows you to view Kea status, leases and subnets in NetBox. Go directly from a NetBox device/VM to a DHCP lease and back!
 
 ## Features
 
 - Uses the Kea management API
-- View Kea daemon statuses. 
+- View Kea daemon statuses.
 - Supports Kea's DHCPv4 and DHCPv6 servers.
 - View, delete, export and search for DHCP leases.
 - Search for NetBox devices/VMs directly from DHCP leases.
 - View DHCP subnets from Kea's configuration.
 - REST API and GraphQL support for managing Server objects.
 
 ![Screenshot of DHCP leases](images/leases.png)
@@ -55,15 +55,15 @@
 
 1. Add `netbox-kea` to `local_requirements.txt`.
 
 2. Enable the plugin in `configuration.py`
     ```python
     PLUGINS = ["netbox_kea"]
     ```
-3. Run `./migrate.py migrate`
+3. Run `./manage.py migrate`
 
 ## Custom Links
 
 You can add custom links to NetBox models to easily search for leases.
 
 Make sure to replace `<Kea Server ID>` in the link URL with the object ID of your Kea server. To find a server's ID, open the page for the server
 and look at the top right corner for `netbox_kea.server:<Server ID Here>`.
```

