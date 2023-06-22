# Comparing `tmp/python_gestpay-2.0.1-py3-none-any.whl.zip` & `tmp/python_gestpay-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4399 bytes, number of entries: 7
+Zip file size: 4402 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx       22 b- defN 23-Jun-21 14:52 pygestpay/__init__.py
 -rw-rw-r--  2.0 unx     3548 b- defN 23-Jun-21 14:52 pygestpay/currencies.py
--rw-rw-r--  2.0 unx    11466 b- defN 23-Jun-21 14:52 pygestpay/gestpay.py
--rw-rw-r--  2.0 unx      325 b- defN 23-Jun-21 14:52 python_gestpay-2.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-21 14:52 python_gestpay-2.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-21 14:52 python_gestpay-2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      559 b- defN 23-Jun-21 14:52 python_gestpay-2.0.1.dist-info/RECORD
-7 files, 16022 bytes uncompressed, 3405 bytes compressed:  78.7%
+-rw-rw-r--  2.0 unx    11315 b- defN 23-Jun-22 12:28 pygestpay/gestpay.py
+-rw-rw-r--  2.0 unx      325 b- defN 23-Jun-22 12:29 python_gestpay-2.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 12:29 python_gestpay-2.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-22 12:29 python_gestpay-2.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      559 b- defN 23-Jun-22 12:29 python_gestpay-2.0.2.dist-info/RECORD
+7 files, 15871 bytes uncompressed, 3408 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pygestpay/currencies.py
 Comment: 
 
 Filename: pygestpay/gestpay.py
 Comment: 
 
-Filename: python_gestpay-2.0.1.dist-info/METADATA
+Filename: python_gestpay-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: python_gestpay-2.0.1.dist-info/WHEEL
+Filename: python_gestpay-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: python_gestpay-2.0.1.dist-info/top_level.txt
+Filename: python_gestpay-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: python_gestpay-2.0.1.dist-info/RECORD
+Filename: python_gestpay-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pygestpay/gestpay.py

```diff
@@ -232,28 +232,23 @@
 
         if self.debug:
             _log.info('GESTPAY: Check Card')
             _log.info(data)
 
         return self.make_s2s_request('callCheckCartaS2S', data)
     
-    def check_token(self, card_token, exp_month, exp_year, cvv=False, transaction_id=False, card_auth="N"):
+    def check_token(self, card_token, transaction_id=False, card_auth="N"):
         data = self._prepare_request()
         data['tokenValue'] = card_token
-        data['expMonth'] = exp_month
-        data['expYear'] = exp_year
-        if cvv:
-            data['CVV2'] = cvv
         if transaction_id:
             data['shopTransactionId'] = transaction_id
-
         data['withAuth'] = card_auth
 
         if self.debug:
-            _log.info('GESTPAY: Check Card')
+            _log.info('GESTPAY: Check Token')
             _log.info(data)
 
         return self.make_s2s_request('callCheckCartaS2S', data)
 
     def update_token(self, card_token, exp_month, exp_year, card_auth="N"):
         data = self._prepare_request()
         data['token'] = card_token
```

## Comparing `python_gestpay-2.0.1.dist-info/RECORD` & `python_gestpay-2.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pygestpay/__init__.py,sha256=2YehXeDUZAyepyP-2k1Ae6obmwYgR1lM1lQVqbQer2M,22
 pygestpay/currencies.py,sha256=W-Rk5QlYjIxlHyCThFyhDklB9CxwWVNqD5lYiKWKe78,3548
-pygestpay/gestpay.py,sha256=WrKfB6JvcZpzQvn3mIhtGya4BVvCK79VIUt4iW0hrck,11466
-python_gestpay-2.0.1.dist-info/METADATA,sha256=VFChe13mNUprkWQ8jV56j8W9yn_IIcu3XAZIw43x2_c,325
-python_gestpay-2.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-python_gestpay-2.0.1.dist-info/top_level.txt,sha256=yZOs3KVMVofz7KEkw1r3EWd1EYB8JP9lRFA2CJqgrQs,10
-python_gestpay-2.0.1.dist-info/RECORD,,
+pygestpay/gestpay.py,sha256=_XVHhVw77BNt0jQIx6Wa5qFuINRmKkSmEjxGuGhvQC0,11315
+python_gestpay-2.0.2.dist-info/METADATA,sha256=HO5anj8Y1pTjFrv7QvI7pQyen_OyJ2u2gFpAy7gCxTI,325
+python_gestpay-2.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+python_gestpay-2.0.2.dist-info/top_level.txt,sha256=yZOs3KVMVofz7KEkw1r3EWd1EYB8JP9lRFA2CJqgrQs,10
+python_gestpay-2.0.2.dist-info/RECORD,,
```

