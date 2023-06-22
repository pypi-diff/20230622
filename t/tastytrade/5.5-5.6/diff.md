# Comparing `tmp/tastytrade-5.5.tar.gz` & `tmp/tastytrade-5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-5.5.tar", last modified: Wed Jun 21 15:20:51 2023, max compression
+gzip compressed data, was "tastytrade-5.6.tar", last modified: Thu Jun 22 14:59:41 2023, max compression
```

## Comparing `tastytrade-5.5.tar` & `tastytrade-5.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:20:51.173865 tastytrade-5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-21 15:20:41.000000 tastytrade-5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-21 15:20:51.173865 tastytrade-5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-06-21 15:20:41.000000 tastytrade-5.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:20:51.173865 tastytrade-5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-21 15:20:41.000000 tastytrade-5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:20:51.165865 tastytrade-5.5/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:20:51.169865 tastytrade-5.5/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    22045 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-21 15:20:41.000000 tastytrade-5.5/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:20:51.169865 tastytrade-5.5/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 15:20:51.000000 tastytrade-5.5/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:59:41.991850 tastytrade-5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 14:59:29.000000 tastytrade-5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-22 14:59:41.991850 tastytrade-5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-06-22 14:59:29.000000 tastytrade-5.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:59:41.991850 tastytrade-5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-22 14:59:29.000000 tastytrade-5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:59:41.987849 tastytrade-5.6/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:59:41.991850 tastytrade-5.6/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:59:41.987849 tastytrade-5.6/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-5.5/LICENSE` & `tastytrade-5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/PKG-INFO` & `tastytrade-5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.5
+Version: 5.6
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -55,15 +55,20 @@
 
    from tastytrade.streamer import DataStreamer, EventType
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
    # this function fetches quotes once, then closes the subscription
-   quotes = await streamer.oneshot(EventType.QUOTE, subs_list)
+   await streamer.subscribe(EventType.QUOTE, subs_list)
+   quotes = []
+   async for quote in streamer.listen():
+      quotes.append(quote)
+      if len(quotes) >= len(subs_list):
+         break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Getting current positions
 -------------------------
 
@@ -122,15 +127,20 @@
 
    from tastytrade.instruments import get_option_chain
    from datetime import date
 
    chain = get_option_chain(session, 'SPLG')
    subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
 
-   greeks = await streamer.oneshot(EventType.GREEKS, subs_list)
+   await streamer.subscribe(EventType.GREEKS, subs_list)
+   greeks = []
+   async for greek in streamer.listen():
+      greeks.append(greek)
+      if len(greeks) >= len(subs_list):
+         break
    print(greeks)
 
 >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
 
 For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
 
 Disclaimer
```

### Comparing `tastytrade-5.5/README.rst` & `tastytrade-5.6/tastytrade.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: tastytrade
+Version: 5.6
+Summary: An unofficial SDK for Tastytrade!
+Home-page: https://github.com/tastyware/tastytrade
+Author: Graeme Holliday
+Author-email: graeme.holliday@pm.me
+License: MIT
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
    :target: https://pypi.org/project/tastytrade
    :alt: PyPI Package
@@ -44,15 +55,20 @@
 
    from tastytrade.streamer import DataStreamer, EventType
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
    # this function fetches quotes once, then closes the subscription
-   quotes = await streamer.oneshot(EventType.QUOTE, subs_list)
+   await streamer.subscribe(EventType.QUOTE, subs_list)
+   quotes = []
+   async for quote in streamer.listen():
+      quotes.append(quote)
+      if len(quotes) >= len(subs_list):
+         break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Getting current positions
 -------------------------
 
@@ -111,15 +127,20 @@
 
    from tastytrade.instruments import get_option_chain
    from datetime import date
 
    chain = get_option_chain(session, 'SPLG')
    subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
 
-   greeks = await streamer.oneshot(EventType.GREEKS, subs_list)
+   await streamer.subscribe(EventType.GREEKS, subs_list)
+   greeks = []
+   async for greek in streamer.listen():
+      greeks.append(greek)
+      if len(greeks) >= len(subs_list):
+         break
    print(greeks)
 
 >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
 
 For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
 
 Disclaimer
```

### Comparing `tastytrade-5.5/setup.py` & `tastytrade-5.6/setup.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/account.py` & `tastytrade-5.6/tastytrade/account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/candle.py` & `tastytrade-5.6/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/event.py` & `tastytrade-5.6/tastytrade/dxfeed/event.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/greeks.py` & `tastytrade-5.6/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/profile.py` & `tastytrade-5.6/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/quote.py` & `tastytrade-5.6/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/summary.py` & `tastytrade-5.6/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/theoprice.py` & `tastytrade-5.6/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/timeandsale.py` & `tastytrade-5.6/tastytrade/dxfeed/timeandsale.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/dxfeed/trade.py` & `tastytrade-5.6/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/instruments.py` & `tastytrade-5.6/tastytrade/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/metrics.py` & `tastytrade-5.6/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/order.py` & `tastytrade-5.6/tastytrade/order.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/search.py` & `tastytrade-5.6/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/session.py` & `tastytrade-5.6/tastytrade/session.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/streamer.py` & `tastytrade-5.6/tastytrade/streamer.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,15 +244,20 @@
 
     Example usage::
 
         session = Session('user', 'pass')
         streamer = await DataStreamer.create(session)
 
         subs = ['SPY', 'GLD']  # list of quotes to fetch
-        quote = await streamer.oneshot(EventType.QUOTE, subs)
+        await streamer.subscribe(EventType.QUOTE, subs)
+        quotes = []
+        async for quote in streamer.listen():
+            quotes.append(quote)
+            if len(quotes) >= len(subs):
+                break
 
     """
     def __init__(self, session: Session):
         #: The active session used to initiate the streamer or make requests
         self.session: Session = session
 
         self._counter = 0
@@ -282,25 +287,14 @@
 
         :param session: active user session to use
         """
         self = cls(session)
         while not self.client_id:
             await asyncio.sleep(0.1)
 
-        # see Github issue #45:
-        # once the handshake completes, although setup is completed locally, remotely there
-        # is still some kind of setup process that hasn't happened that takes about 8-9
-        # seconds, and afterwards you're good to go. Unfortunately, there's no way to know
-        # when that process concludes remotely, as there's no kind of confirmation message
-        # sent. This is a hacky solution to ensure streamer setup completes.
-        await self.oneshot(EventType.QUOTE, ['SPY'])
-        # clear queue if there's any lingering data
-        while not self._queue.empty():
-            self._queue.get_nowait()
-
         return self
 
     async def _next_id(self):
         async with self._lock:
             self._counter += 1
         return self._counter
 
@@ -406,16 +400,15 @@
             logger.debug('sending heartbeat: %s', message)
             await self._websocket.send(json.dumps([message]))
             # send the heartbeat every 10 seconds
             await asyncio.sleep(10)
 
     async def subscribe(self, event_type: EventType, symbols: list[str], reset: bool = False) -> None:
         """
-        Subscribes to quotes for given list of symbols. Used for recurring data feeds;
-        if you just want to get a one-time quote, use :meth:`oneshot`.
+        Subscribes to quotes for given list of symbols. Used for recurring data feeds.
 
         :param event_type: type of subscription to add
         :param symbols: list of symbols to subscribe for
         :param reset:
             whether to reset the subscription list (remove all other subscriptions of all types)
         """
         id = await self._next_id()
@@ -447,39 +440,14 @@
                 'remove': {event_type: symbols}
             },
             'clientId': self.client_id
         }
         logger.debug('sending unsubscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
-    async def oneshot(self, event_type: EventType, symbols: list[str]) -> list[Event]:
-        """
-        Using the given information, subscribes to the list of symbols passed, streams
-        the requested information once, then unsubscribes. If you want to maintain the
-        subscription open, add a subscription with :meth:`subscribe` and listen with
-        :meth:`listen`.
-
-        If you use this alongside :meth:`subscribe` and :meth:`listen`, you will get
-        some unexpected behavior. Most apps should use either this or :meth:`listen`
-        but not both.
-
-        :param event_type: the type of subscription to stream, either greeks or quotes
-        :param symbols: list of symbols to subscribe to
-
-        :return: list of :class:`~tastytrade.dxfeed.event.Event`s pulled.
-        """
-        await self.subscribe(event_type, symbols)
-        data = []
-        async for item in self.listen():
-            data.append(item)
-            if len(data) >= len(symbols):
-                break
-        await self.unsubscribe(event_type, symbols)
-        return data
-
     async def subscribe_candle(self, ticker: str, start_time: datetime, interval: str) -> None:
         """
         Subscribes to candle-style 'OHLC' data for the given symbol.
 
         :param ticker: symbol to get date for
         :param start_time: starting time for the data range
         :param interval: the width of each candle in time, e.g. '5m', '1h', '3d', '1w', '1mo'
@@ -516,36 +484,14 @@
                 'removeTimeSeries': {'Candle': [f'{ticker}{{={interval}}}']}
             },
             'clientId': self.client_id
         }
         logger.debug('sending unsubscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
-    async def oneshot_candle(self, ticker: str, start_time: datetime, interval: str) -> list[Candle]:
-        """
-        Subscribes to candle-style 'OHLC' data for the given symbol, waits for
-        the complete range to be received, then unsubscribes.
-
-        :param ticker: symbol to get date for
-        :param start_time: starting time for the data range
-        :param interval: the width of each candle in time, e.g. '5m', '1h', '3d', '1w', '1mo'
-        """
-        await self.subscribe_candle(ticker, start_time, interval)
-        candles = []
-        async for candle in self.listen_candle():
-            candles.append(candle)
-            # until we hit the start date, keep going
-            # use timestamp to support timezone in start_time
-            if candle.time <= start_time.timestamp() * 1000:
-                break
-        await self.unsubscribe_candle(ticker, interval)
-
-        candles.reverse()
-        return candles
-
     def _map_message(self, message) -> list[Event]:
         """
         Takes the raw JSON data and returns a list of parsed :class:`~tastytrade.dxfeed.event.Event` objects.
         """
         # the first time around, types are shown
         if isinstance(message[0], str):
             msg_type = message[0]
```

### Comparing `tastytrade-5.5/tastytrade/utils.py` & `tastytrade-5.6/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade/watchlists.py` & `tastytrade-5.6/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.5/tastytrade.egg-info/PKG-INFO` & `tastytrade-5.6/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: tastytrade
-Version: 5.5
-Summary: An unofficial SDK for Tastytrade!
-Home-page: https://github.com/tastyware/tastytrade
-Author: Graeme Holliday
-Author-email: graeme.holliday@pm.me
-License: MIT
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
    :target: https://pypi.org/project/tastytrade
    :alt: PyPI Package
@@ -55,15 +44,20 @@
 
    from tastytrade.streamer import DataStreamer, EventType
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
    # this function fetches quotes once, then closes the subscription
-   quotes = await streamer.oneshot(EventType.QUOTE, subs_list)
+   await streamer.subscribe(EventType.QUOTE, subs_list)
+   quotes = []
+   async for quote in streamer.listen():
+      quotes.append(quote)
+      if len(quotes) >= len(subs_list):
+         break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Getting current positions
 -------------------------
 
@@ -122,15 +116,20 @@
 
    from tastytrade.instruments import get_option_chain
    from datetime import date
 
    chain = get_option_chain(session, 'SPLG')
    subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
 
-   greeks = await streamer.oneshot(EventType.GREEKS, subs_list)
+   await streamer.subscribe(EventType.GREEKS, subs_list)
+   greeks = []
+   async for greek in streamer.listen():
+      greeks.append(greek)
+      if len(greeks) >= len(subs_list):
+         break
    print(greeks)
 
 >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
 
 For more examples, check out the `documentation <https://tastyworks-api.readthedocs.io/en/latest/>`_.
 
 Disclaimer
```

### Comparing `tastytrade-5.5/tastytrade.egg-info/SOURCES.txt` & `tastytrade-5.6/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

