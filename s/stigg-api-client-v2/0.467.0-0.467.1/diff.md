# Comparing `tmp/stigg_api_client_v2-0.467.0.tar.gz` & `tmp/stigg_api_client_v2-0.467.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.467.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.467.1.tar", max compression
```

## Comparing `stigg_api_client_v2-0.467.0.tar` & `stigg_api_client_v2-0.467.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-06-21 15:05:31.473351 stigg_api_client_v2-0.467.0/README.md
--rw-r--r--   0        0        0      653 2023-06-21 15:06:09.017465 stigg_api_client_v2-0.467.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-21 15:05:31.473351 stigg_api_client_v2-0.467.0/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-21 15:05:31.473351 stigg_api_client_v2-0.467.0/stigg/client.py
--rw-r--r--   0        0        0    39611 2023-06-21 15:06:07.357472 stigg_api_client_v2-0.467.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-21 15:06:06.985474 stigg_api_client_v2-0.467.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-21 15:06:06.985474 stigg_api_client_v2-0.467.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-21 15:06:06.117478 stigg_api_client_v2-0.467.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-21 15:06:06.133478 stigg_api_client_v2-0.467.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70260 2023-06-21 15:06:07.201473 stigg_api_client_v2-0.467.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-21 15:06:06.157478 stigg_api_client_v2-0.467.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-21 15:06:06.245477 stigg_api_client_v2-0.467.0/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23730 2023-06-21 15:06:04.005487 stigg_api_client_v2-0.467.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-21 15:06:06.125478 stigg_api_client_v2-0.467.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-21 15:06:06.129478 stigg_api_client_v2-0.467.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-21 15:06:06.989474 stigg_api_client_v2-0.467.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53605 2023-06-21 15:06:06.985474 stigg_api_client_v2-0.467.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-21 15:06:06.177477 stigg_api_client_v2-0.467.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-21 15:06:06.185478 stigg_api_client_v2-0.467.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-21 15:06:06.173478 stigg_api_client_v2-0.467.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-21 15:06:06.225477 stigg_api_client_v2-0.467.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-21 15:06:06.201477 stigg_api_client_v2-0.467.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-21 15:06:06.197477 stigg_api_client_v2-0.467.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-21 15:06:06.233477 stigg_api_client_v2-0.467.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-21 15:06:06.193477 stigg_api_client_v2-0.467.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-21 15:06:06.209478 stigg_api_client_v2-0.467.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-21 15:06:06.217477 stigg_api_client_v2-0.467.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-21 15:06:06.085478 stigg_api_client_v2-0.467.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-21 15:06:06.077478 stigg_api_client_v2-0.467.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-21 15:06:06.105478 stigg_api_client_v2-0.467.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   125523 2023-06-21 15:06:06.061478 stigg_api_client_v2-0.467.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-21 15:06:06.165478 stigg_api_client_v2-0.467.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-21 15:06:06.073478 stigg_api_client_v2-0.467.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-21 15:06:06.101478 stigg_api_client_v2-0.467.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-21 15:06:06.153478 stigg_api_client_v2-0.467.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-06-21 15:06:06.149478 stigg_api_client_v2-0.467.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-06-21 15:06:06.141478 stigg_api_client_v2-0.467.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-21 15:06:06.993474 stigg_api_client_v2-0.467.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-21 15:06:06.089478 stigg_api_client_v2-0.467.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-21 15:06:06.109478 stigg_api_client_v2-0.467.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-06-21 15:06:06.237477 stigg_api_client_v2-0.467.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0      451 2023-06-21 15:06:06.249477 stigg_api_client_v2-0.467.0/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.467.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-22 11:32:47.050355 stigg_api_client_v2-0.467.1/README.md
+-rw-r--r--   0        0        0      653 2023-06-22 11:33:33.509060 stigg_api_client_v2-0.467.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-22 11:32:47.050355 stigg_api_client_v2-0.467.1/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-22 11:32:47.050355 stigg_api_client_v2-0.467.1/stigg/client.py
+-rw-r--r--   0        0        0    39611 2023-06-22 11:33:31.552959 stigg_api_client_v2-0.467.1/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-22 11:33:31.124937 stigg_api_client_v2-0.467.1/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-22 11:33:31.124937 stigg_api_client_v2-0.467.1/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-22 11:33:30.104884 stigg_api_client_v2-0.467.1/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-22 11:33:30.124885 stigg_api_client_v2-0.467.1/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70260 2023-06-22 11:33:31.376950 stigg_api_client_v2-0.467.1/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-22 11:33:30.152886 stigg_api_client_v2-0.467.1/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-22 11:33:30.252892 stigg_api_client_v2-0.467.1/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23792 2023-06-22 11:33:27.516754 stigg_api_client_v2-0.467.1/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-22 11:33:30.112884 stigg_api_client_v2-0.467.1/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-22 11:33:30.120885 stigg_api_client_v2-0.467.1/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-22 11:33:31.124937 stigg_api_client_v2-0.467.1/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53605 2023-06-22 11:33:31.124937 stigg_api_client_v2-0.467.1/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-22 11:33:30.176888 stigg_api_client_v2-0.467.1/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-22 11:33:30.184888 stigg_api_client_v2-0.467.1/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-22 11:33:30.168887 stigg_api_client_v2-0.467.1/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-22 11:33:30.228891 stigg_api_client_v2-0.467.1/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-22 11:33:30.200889 stigg_api_client_v2-0.467.1/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-22 11:33:30.196889 stigg_api_client_v2-0.467.1/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-22 11:33:30.240891 stigg_api_client_v2-0.467.1/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-22 11:33:30.192889 stigg_api_client_v2-0.467.1/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-22 11:33:30.212890 stigg_api_client_v2-0.467.1/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-22 11:33:30.220890 stigg_api_client_v2-0.467.1/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-22 11:33:30.068882 stigg_api_client_v2-0.467.1/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-22 11:33:30.060882 stigg_api_client_v2-0.467.1/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-22 11:33:30.092883 stigg_api_client_v2-0.467.1/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   125885 2023-06-22 11:33:30.044881 stigg_api_client_v2-0.467.1/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-22 11:33:30.160887 stigg_api_client_v2-0.467.1/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-22 11:33:30.056882 stigg_api_client_v2-0.467.1/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-22 11:33:30.084883 stigg_api_client_v2-0.467.1/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-22 11:33:30.144886 stigg_api_client_v2-0.467.1/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-06-22 11:33:30.140886 stigg_api_client_v2-0.467.1/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-06-22 11:33:30.136886 stigg_api_client_v2-0.467.1/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-22 11:33:31.128937 stigg_api_client_v2-0.467.1/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-22 11:33:30.076882 stigg_api_client_v2-0.467.1/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-22 11:33:30.100884 stigg_api_client_v2-0.467.1/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-06-22 11:33:30.244891 stigg_api_client_v2-0.467.1/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0      451 2023-06-22 11:33:30.260892 stigg_api_client_v2-0.467.1/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.467.1/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.467.0/README.md` & `stigg_api_client_v2-0.467.1/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.467.0/pyproject.toml` & `stigg_api_client_v2-0.467.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.467.0"
+version = "0.467.1"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.467.1/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.467.1/stigg/generated/async_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.467.1/stigg/generated/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.467.1/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/client.py` & `stigg_api_client_v2-0.467.1/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.467.1/stigg/generated/create_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.467.1/stigg/generated/entitlements_updated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.467.1/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
@@ -771,15 +771,17 @@
 
 class SubscriptionMigrationTime(str, Enum):
     END_OF_BILLING_PERIOD = "END_OF_BILLING_PERIOD"
     IMMEDIATE = "IMMEDIATE"
 
 
 class SubscriptionPriceSortFields(str, Enum):
+    billingModel = "billingModel"
     createdAt = "createdAt"
+    featureId = "featureId"
     id = "id"
     updatedAt = "updatedAt"
     usageLimit = "usageLimit"
 
 
 class SubscriptionScheduleStatus(str, Enum):
     Canceled = "Canceled"
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.467.1/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.467.1/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.467.1/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.467.1/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -124,14 +124,25 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -146,25 +157,14 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -517,29 +517,14 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -604,14 +589,29 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
 class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
@@ -1293,17 +1293,17 @@
 PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1343,28 +1343,28 @@
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.467.1/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.467.1/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.467.1/stigg/generated/get_customer_by_id.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.467.1/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.467.1/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.467.1/stigg/generated/get_products.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.467.1/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.467.1/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -735,15 +735,19 @@
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
 
 
 class CustomerSubscriptionFilterSubscriptionPriceFilter(BaseModel):
     and_: Optional[List["CustomerSubscriptionFilterSubscriptionPriceFilter"]] = Field(
         alias="and"
     )
+    billing_model: Optional["BillingModelFilterComparison"] = Field(
+        alias="billingModel"
+    )
     created_at: Optional["DateFieldComparison"] = Field(alias="createdAt")
+    feature_id: Optional["StringFieldComparison"] = Field(alias="featureId")
     id: Optional["StringFieldComparison"]
     or_: Optional[List["CustomerSubscriptionFilterSubscriptionPriceFilter"]] = Field(
         alias="or"
     )
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
     usage_limit: Optional["NumberFieldComparison"] = Field(alias="usageLimit")
 
@@ -2302,15 +2306,19 @@
     direction: SortDirection
     field: SubscriptionMigrationTaskSortFields
     nulls: Optional[SortNulls]
 
 
 class SubscriptionPriceFilter(BaseModel):
     and_: Optional[List["SubscriptionPriceFilter"]] = Field(alias="and")
+    billing_model: Optional["BillingModelFilterComparison"] = Field(
+        alias="billingModel"
+    )
     created_at: Optional["DateFieldComparison"] = Field(alias="createdAt")
+    feature_id: Optional["StringFieldComparison"] = Field(alias="featureId")
     id: Optional["StringFieldComparison"]
     or_: Optional[List["SubscriptionPriceFilter"]] = Field(alias="or")
     price: Optional["SubscriptionPriceFilterPriceFilter"]
     subscription: Optional["SubscriptionPriceFilterCustomerSubscriptionFilter"]
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
     usage_limit: Optional["NumberFieldComparison"] = Field(alias="usageLimit")
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.467.1/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.467.1/stigg/generated/provision_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.467.1/stigg/generated/provision_subscription.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.467.1/stigg/generated/report_usage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.467.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.467.1/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-21 15:06
+# Generated by ariadne-codegen on 2023-06-22 11:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.467.0/PKG-INFO` & `stigg_api_client_v2-0.467.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.467.0
+Version: 0.467.1
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

