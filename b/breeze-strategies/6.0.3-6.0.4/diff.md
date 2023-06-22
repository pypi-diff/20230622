# Comparing `tmp/breeze_strategies-6.0.3.tar.gz` & `tmp/breeze_strategies-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-6.0.3.tar", last modified: Wed Jun 21 06:02:16 2023, max compression
+gzip compressed data, was "breeze_strategies-6.0.4.tar", last modified: Thu Jun 22 07:36:04 2023, max compression
```

## Comparing `breeze_strategies-6.0.3.tar` & `breeze_strategies-6.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 06:02:16.142026 breeze_strategies-6.0.3/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.3/LICENSE
--rw-rw-rw-   0        0        0     1135 2023-06-21 06:02:16.140004 breeze_strategies-6.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-06-19 10:01:44.000000 breeze_strategies-6.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 06:02:16.051430 breeze_strategies-6.0.3/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.3/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    18286 2023-06-21 05:54:42.000000 breeze_strategies-6.0.3/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-21 06:02:16.136210 breeze_strategies-6.0.3/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1135 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 06:02:16.142026 breeze_strategies-6.0.3/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-19 10:01:32.000000 breeze_strategies-6.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:36:04.987253 breeze_strategies-6.0.4/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1135 2023-06-22 07:36:04.984253 breeze_strategies-6.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-22 07:28:15.000000 breeze_strategies-6.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 07:36:04.831358 breeze_strategies-6.0.4/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.4/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    20409 2023-06-22 07:33:12.000000 breeze_strategies-6.0.4/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:36:04.979261 breeze_strategies-6.0.4/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1135 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-22 07:36:04.000000 breeze_strategies-6.0.4/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:36:04.987253 breeze_strategies-6.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-22 07:28:24.000000 breeze_strategies-6.0.4/setup.py
```

### Comparing `breeze_strategies-6.0.3/LICENSE` & `breeze_strategies-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-6.0.3/PKG-INFO` & `breeze_strategies-6.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 6.0.3
+Version: 6.0.4
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
 
-pip install breeze_strategies==6.0.3
+pip install breeze_strategies==6.0.4
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.3/README.md` & `breeze_strategies-6.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.3
+pip install breeze_strategies==6.0.4
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.3/breeze_strategies/breeze_strategies.py` & `breeze_strategies-6.0.4/breeze_strategies/breeze_strategies.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         self.product_type = ""
         self.expiry_date = ""
         self.strike_price = ""
         self.order_type = ""
         self.validity = ""
         self.stoploss = ""
         self.validity_date = ""
+        self.callexecution = ""
+        self.putexecution = ""
     
     def squareoff(self,exchange_code, stock_code, product_type, expiry_date, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity,right):
         data = self.client.square_off(exchange_code=exchange_code,
                             product="options",
                             stock_code=stock_code,
                             expiry_date=expiry_date,
                             right=right,
@@ -46,21 +48,24 @@
                             validity=validity,
                             stoploss="0",
                             quantity=quantity,
                             price=price,
                             validity_date=validity_date,
                             trade_password="",
                             disclosed_quantity="0")
+
+        print(f"Squaring off {right} ..")
         response = None
         if(data['Status'] == 200):
             response = data['Success']['message']
+            print(f"Success : {response}")
         else:
             response = data['Error']
-        
-        print(f"square off status of {right} is",response)
+            print(f"Error : {response}")
+        return(data)
         
     def get_date_format(self,expiry_date):
         month_names = {
                             '01': 'Jan',
                             '02': 'Feb',
                             '03': 'Mar',
                             '04': 'Apr',
@@ -77,15 +82,15 @@
         month = expiry_date[5:7]
         day = expiry_date[8:10]
         formatted_date = f"{day}-{month_names[month]}-{year}"
         return(formatted_date)
         
     def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution,put_execution):
         net_gain_loss = (self.currentcall + self.currentput)*int(quantity)
-        print(f"P&L (NET): {round(net_gain_loss,2)}/- Rs")
+        print(f"P&L (NET) : {round(net_gain_loss,2)}/- Rs")
         print("-------------------------------------------------------------------")
         formatted_date = self.get_date_format(expiry_date)
 
         if(net_gain_loss > 0 and net_gain_loss >= self.maxprofit):
             print("maxprofit has reached...")
             print("SquareOff operation on both contracts call and put begins....")
             
@@ -116,22 +121,22 @@
         
         def on_ticks(data):
             
             value = data
             
             if(value['right'] == "Call"):
                 self.currentcall = round(float(value['last']) - float(call_execution), 2)
-                print(f"P&L (CALL)  : {round(self.currentcall * int(self.quantity),2)}/- Rs")
+                #print(f"P&L (CALL)  : {round(self.currentcall * int(self.quantity),2)}/- Rs")
                 #print("-------------------------------------------------------------------")
                 if(self.flag == False):
                     self.trigger(product_type, "Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
             
             if(value['right'] == "Put"):
                 self.currentput = round(float(value['last']) - float(put_execution), 2)
-                print(f"P&L (PUT) :  {round(self.currentput * int(self.quantity),2)}/- Rs")
+                #print(f"P&L (PUT) :  {round(self.currentput * int(self.quantity),2)}/- Rs")
                 #print("-------------------------------------------------------------------")
                 if(self.flag == False):
                     self.trigger(product_type, "Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
             
         self.client.on_ticks = on_ticks
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Call", get_exchange_quotes=True, get_market_depth=False)
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Put", get_exchange_quotes=True, get_market_depth=False) 
@@ -241,23 +246,25 @@
             put_execution = -1
             
             print(f"order ids are : {orderids}")
             for entry in details['Success']:
                 if(entry['status'] == "Executed"):
                     call_execution = entry['average_price']
                     call_status = "Executed"
+                    self.callexecution = call_execution
                     break
                     
             details = self.client.get_order_detail(exchange_code=exchange_code,
                         order_id= orderids[1])
             #print(details)
             for entry in details['Success']:
                 if(entry['status'] == "Executed"):
                     put_execution = entry['average_price']
                     put_status = "Executed"
+                    self.putexecution = put_execution
                     break
                     
             if(call_execution == -1 or put_execution == -1):
                 print("Dear User order could not execute within time limit ..cancelling it")
                 if(call_execution == -1 and put_execution == -1):
                     print("Both Order Call and Put could not execute to so cancelling it ..... ")
                     self.client.cancel_order(exchange_code=exchange_code,
@@ -285,22 +292,64 @@
                     
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
                 self.profit_and_loss(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
             
     def stop(self):
 
-        print("squaring off the contract and exiting strategy...")
+        print("squaring off the both contracts and exiting strategy...")
+        square_call = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call", action = "sell")
+        square_put = self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put", action = "sell")
         self.client.ws_disconnect()
-        self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call", action = "sell")
-        self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put", action = "sell")
-
+        self.create_report(square_call,square_put)
         
 
     def get_pnl(self):
-        print("- Negative indicates loss")
-        print(f"P&L (CALL):  {round(self.currentcall*int(self.quantity),2)}/- Rs")
-        print(f"P&L (PUT):  {round(self.currentput*int(self.quantity),2)}/- Rs")
+        #print("- Negative indicates loss")
+        #print(f"P&L (CALL):  {round(self.currentcall*int(self.quantity),2)}/- Rs")
+        #print(f"P&L (PUT):  {round(self.currentput*int(self.quantity),2)}/- Rs")
         outcome = (self.currentcall + self.currentput)*int(self.quantity)
-        print(f"P&L (NET) for QUANTITY = {self.quantity} is {outcome}/- Rs")
+        print(f"P&L (NET) : {round(outcome,2)}/- Rs")
 
         print("------------------------------------------------------------------------------")
+
+
+    def create_report(self,sq_call,sq_put):
+        print("Report for final P&L...")
+        if(sq_call['Status'] == 200 and sq_put['Status'] == 200):
+            sq_callid = sq_call["Success"]['order_id']
+            sq_putid = sq_put["Success"]['order_id']
+
+            callrecords = self.client.get_order_detail(exchange_code=self.exchange_code,
+                        order_id= sq_callid)
+
+            putrecords = self.client.get_order_detail(exchange_code=self.exchange_code,
+                        order_id= sq_putid)
+
+            sqcall_price = -1
+            sqput_price = -1
+            for record in callrecords['Success']:
+                if(record['status'] == "Executed"):
+                    sqcall_price = record["average_price"]
+                    break
+            for record in putrecords["Success"]:
+                if(record['status'] == "Executed"):
+                    sqput_price = record["average_price"]
+                    break
+            
+            plcall = round((float(sqcall_price) - int(self.callexecution))*int(self.quantity),2)
+            plput = round((float(sqput_price) - int(self.putexecution))*int(self.quantity),2)
+
+            self.currentcall = (float(sqcall_price) - int(self.callexecution))
+            self.currentput = (float(sqput_price) - int(self.putexecution))
+
+            print("-------------------------------------------------------")
+            print("Profit and Loss Report........")
+            print(f"P&L (CALL) : {plcall}/- Rs")
+            print(f"P&L (PUT) : {plput}/- Rs")
+            print(f"P&L (NET) : {plput + plcall}/- Rs")
+            print("-------------------------------------------------------")
+        else:
+            print("One of Square off operation failed..")
+
+
+
```

### Comparing `breeze_strategies-6.0.3/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-6.0.4/breeze_strategies.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 6.0.3
+Version: 6.0.4
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
 
-pip install breeze_strategies==6.0.3
+pip install breeze_strategies==6.0.4
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.3/setup.py` & `breeze_strategies-6.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="6.0.3",
+    version="6.0.4",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

