# Comparing `tmp/breeze_strategies-6.0.6.tar.gz` & `tmp/breeze_strategies-6.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-6.0.6.tar", last modified: Thu Jun 22 09:13:28 2023, max compression
+gzip compressed data, was "breeze_strategies-6.0.7.tar", last modified: Thu Jun 22 09:35:59 2023, max compression
```

## Comparing `breeze_strategies-6.0.6.tar` & `breeze_strategies-6.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 09:13:28.834363 breeze_strategies-6.0.6/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.6/LICENSE
--rw-rw-rw-   0        0        0     1135 2023-06-22 09:13:28.830016 breeze_strategies-6.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-06-22 09:13:24.000000 breeze_strategies-6.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 09:13:28.748433 breeze_strategies-6.0.6/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.6/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    20590 2023-06-22 09:12:32.000000 breeze_strategies-6.0.6/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-22 09:13:28.818849 breeze_strategies-6.0.6/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1135 2023-06-22 09:13:28.000000 breeze_strategies-6.0.6/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-22 09:13:28.000000 breeze_strategies-6.0.6/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 09:13:28.000000 breeze_strategies-6.0.6/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-22 09:13:28.000000 breeze_strategies-6.0.6/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-22 09:13:28.000000 breeze_strategies-6.0.6/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 09:13:28.835372 breeze_strategies-6.0.6/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-22 09:13:15.000000 breeze_strategies-6.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 09:35:59.570940 breeze_strategies-6.0.7/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1135 2023-06-22 09:35:59.569941 breeze_strategies-6.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-22 09:35:52.000000 breeze_strategies-6.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 09:35:59.536572 breeze_strategies-6.0.7/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.7/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    20618 2023-06-22 09:35:37.000000 breeze_strategies-6.0.7/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-22 09:35:59.567943 breeze_strategies-6.0.7/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1135 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-22 09:35:59.000000 breeze_strategies-6.0.7/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 09:35:59.571940 breeze_strategies-6.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-22 09:35:45.000000 breeze_strategies-6.0.7/setup.py
```

### Comparing `breeze_strategies-6.0.6/LICENSE` & `breeze_strategies-6.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-6.0.6/PKG-INFO` & `breeze_strategies-6.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 6.0.6
+Version: 6.0.7
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.6
+pip install breeze_strategies==6.0.7
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.6/README.md` & `breeze_strategies-6.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.6
+pip install breeze_strategies==6.0.7
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.6/breeze_strategies/breeze_strategies.py` & `breeze_strategies-6.0.7/breeze_strategies/breeze_strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,31 +90,33 @@
         print("-------------------------------------------------------------------")
         formatted_date = self.get_date_format(expiry_date)
 
         if(net_gain_loss > 0 and net_gain_loss >= self.maxprofit):
             print("maxprofit has reached...")
             print("SquareOff operation on both contracts call and put begins....")
             
-            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Call",action = "sell", price = "")
-            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price , order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Put", action = "sell", price = "")
+            #self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Call",action = "sell", price = "")
+            #self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price , order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Put", action = "sell", price = "")
             
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
-            print("-------------END------------------")
+            self.stop()
+            #print("---------------END-----------------")
             self.flag = True
             return
         if(net_gain_loss < 0 and net_gain_loss <= self.maxloss):
             print("maxloss has reached...")
             print("SquareOff operation on both contracts call and put begins....")
-            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Call",action = "sell",price = "")
-            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Put",action = "sell",price = "")
+            #self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Call",action = "sell",price = "")
+            #self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Put",action = "sell",price = "")
 
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
-            print("---------------END-----------------")
+            self.stop()
+            #print("---------------END-----------------")
             self.flag = True
             return
 
     def calculate_current(self,product_type,stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution,flag):
         
         resultcall = []
         formatted_date = self.get_date_format(expiry_date)
@@ -315,15 +317,15 @@
 
     def create_report(self,sq_call,sq_put):
         print("Report for final P&L...")
         if(sq_call['Status'] == 200 and sq_put['Status'] == 200):
             sq_callid = sq_call["Success"]['order_id']
             sq_putid = sq_put["Success"]['order_id']
 
-            print("----lets wait for 5 seconds for getting the executed status of squareoff---")
+            print("\nGenerating Final P&L report in 5 seconds....")
             time.sleep(5)
             callrecords = self.client.get_order_detail(exchange_code=self.exchange_code,
                         order_id= sq_callid)
 
             putrecords = self.client.get_order_detail(exchange_code=self.exchange_code,
                         order_id= sq_putid)
```

### Comparing `breeze_strategies-6.0.6/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-6.0.7/breeze_strategies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 6.0.6
+Version: 6.0.7
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.6
+pip install breeze_strategies==6.0.7
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.6/setup.py` & `breeze_strategies-6.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="6.0.6",
+    version="6.0.7",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

