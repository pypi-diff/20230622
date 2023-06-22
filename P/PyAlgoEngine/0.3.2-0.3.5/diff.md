# Comparing `tmp/PyAlgoEngine-0.3.2.tar.gz` & `tmp/PyAlgoEngine-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAlgoEngine-0.3.2.tar", last modified: Fri Jun 16 06:22:09 2023, max compression
+gzip compressed data, was "PyAlgoEngine-0.3.5.tar", last modified: Thu Jun 22 05:29:59 2023, max compression
```

## Comparing `PyAlgoEngine-0.3.2.tar` & `PyAlgoEngine-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-16 06:22:09.049371 PyAlgoEngine-0.3.2/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-16 06:22:08.265221 PyAlgoEngine-0.3.2/AlgoEngine/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-16 06:22:08.548278 PyAlgoEngine-0.3.2/AlgoEngine/Engine/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31835 2023-06-16 06:16:26.000000 PyAlgoEngine-0.3.2/AlgoEngine/Engine/AlgoEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1517 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.2/AlgoEngine/Engine/EventEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31401 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.2/AlgoEngine/Engine/MarketEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    81182 2023-06-15 09:09:28.000000 PyAlgoEngine-0.3.2/AlgoEngine/Engine/TradeEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3584 2023-06-15 09:22:19.000000 PyAlgoEngine-0.3.2/AlgoEngine/Engine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-16 06:22:08.743163 PyAlgoEngine-0.3.2/AlgoEngine/Strategies/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1857 2023-06-15 17:00:00.000000 PyAlgoEngine-0.3.2/AlgoEngine/Strategies/BackTest.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    12578 2023-06-15 17:02:22.000000 PyAlgoEngine-0.3.2/AlgoEngine/Strategies/_StrategyEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1136 2023-06-15 09:10:19.000000 PyAlgoEngine-0.3.2/AlgoEngine/Strategies/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      444 2023-06-16 06:17:51.000000 PyAlgoEngine-0.3.2/AlgoEngine/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1087 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.2/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      515 2023-06-16 06:22:09.042211 PyAlgoEngine-0.3.2/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-16 06:22:08.986802 PyAlgoEngine-0.3.2/PyAlgoEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      515 2023-06-16 06:22:05.000000 PyAlgoEngine-0.3.2/PyAlgoEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      499 2023-06-16 06:22:06.000000 PyAlgoEngine-0.3.2/PyAlgoEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-06-16 06:22:05.000000 PyAlgoEngine-0.3.2/PyAlgoEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       56 2023-06-16 06:22:05.000000 PyAlgoEngine-0.3.2/PyAlgoEngine.egg-info/requires.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-06-16 06:22:05.000000 PyAlgoEngine-0.3.2/PyAlgoEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       44 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.2/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-06-16 06:22:09.051377 PyAlgoEngine-0.3.2/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1579 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.2/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:59.047923 PyAlgoEngine-0.3.5/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:57.915037 PyAlgoEngine-0.3.5/AlgoEngine/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:58.375515 PyAlgoEngine-0.3.5/AlgoEngine/Engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31968 2023-06-18 06:25:52.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/AlgoEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1517 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/EventEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    32583 2023-06-21 12:41:22.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/MarketEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    81457 2023-06-21 11:54:46.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/TradeEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3754 2023-06-17 05:15:57.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:58.645474 PyAlgoEngine-0.3.5/AlgoEngine/Strategies/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1866 2023-06-18 06:25:52.000000 PyAlgoEngine-0.3.5/AlgoEngine/Strategies/BackTest.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    12684 2023-06-21 11:52:19.000000 PyAlgoEngine-0.3.5/AlgoEngine/Strategies/_StrategyEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1778 2023-06-18 06:25:52.000000 PyAlgoEngine-0.3.5/AlgoEngine/Strategies/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      444 2023-06-21 12:41:36.000000 PyAlgoEngine-0.3.5/AlgoEngine/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1087 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.5/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      515 2023-06-22 05:29:59.040926 PyAlgoEngine-0.3.5/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:58.972763 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      515 2023-06-22 05:29:51.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      499 2023-06-22 05:29:53.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-06-22 05:29:51.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       56 2023-06-22 05:29:51.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/requires.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-06-22 05:29:51.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       44 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.5/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-06-22 05:29:59.051238 PyAlgoEngine-0.3.5/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1579 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.5/setup.py
```

### Comparing `PyAlgoEngine-0.3.2/AlgoEngine/Engine/AlgoEngine.py` & `PyAlgoEngine-0.3.5/AlgoEngine/Engine/AlgoEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import numpy as np
 from PyQuantKit import TransactionSide, TradeInstruction, MarketData, TradeReport, OrderState, OrderType
 
 from . import LOGGER
 from .MarketEngine import MDS
 
 LOGGER = LOGGER.getChild('AlgoEngine')
-__all__ = ['AlgoTemplate', 'ALGO_ENGINE', 'ALGO_REGISTRY']
+__all__ = ['AlgoTemplate', 'AlgoRegistry', 'AlgoEngine', 'ALGO_ENGINE', 'ALGO_REGISTRY']
 
 
 class AlgoStatus(enum.Enum):
     idle = 'idle'  # init state 
     preparing = 'preparing'  # preparing
     ready = 'ready'  # ready to launch order
     working = 'working'  # order launched
@@ -717,24 +717,26 @@
             raise ValueError(f'Invalid name {value}')
 
     @property
     def reversed_registry(self) -> dict[str, str]:
         reversed_registry = {algo.__name__: name for name, algo in self.registry.items()}
         return reversed_registry
 
-    def to_algo(self, name: str, **kwargs):
-        algo_engine = kwargs.get('algo_engine', ALGO_ENGINE)
+    def to_algo(self, name: str, algo_engine: AlgoEngine = None):
+        if algo_engine is None:
+            algo_engine = ALGO_ENGINE
+
         algo = self.registry.get(name.lower())
         return functools.partial(algo, algo_engine=algo_engine)
 
 
 class AlgoEngine(object):
-    def __init__(self, **kwargs):
-        self.mds = kwargs.get('mds', MDS)
-        self.registry = kwargs.get('registry', ALGO_REGISTRY)
+    def __init__(self, mds=None, registry=None):
+        self.mds = mds if mds is not None else MDS
+        self.registry = registry if registry is not None else ALGO_REGISTRY
 
     @classmethod
     def _compare_price(cls, side: TransactionSide, limit_price: float = None, original_limit: float = None, mode='strict') -> float:
         calculated_limit = original_limit
 
         if limit_price is None:
             return calculated_limit
@@ -855,8 +857,8 @@
 ALGO_REGISTRY = AlgoRegistry()
 
 ALGO_REGISTRY.add_algo('aggressive', 'aggr', handler=Aggressive)
 ALGO_REGISTRY.add_algo('passive', 'pass', handler=Passive)
 ALGO_REGISTRY.add_algo('aggressive_timeout', 'aggr_timeout', handler=AggressiveTimeout)
 ALGO_REGISTRY.add_algo('passive_timeout', 'pass_timeout', handler=PassiveTimeout)
 
-ALGO_ENGINE = AlgoEngine()
+ALGO_ENGINE = AlgoEngine(mds=MDS, registry=ALGO_REGISTRY)
```

### Comparing `PyAlgoEngine-0.3.2/AlgoEngine/Engine/EventEngine.py` & `PyAlgoEngine-0.3.5/AlgoEngine/Engine/EventEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.2/AlgoEngine/Engine/MarketEngine.py` & `PyAlgoEngine-0.3.5/AlgoEngine/Engine/MarketEngine.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,33 +7,48 @@
 import uuid
 from collections import defaultdict
 
 from PyQuantKit import TickData, TradeData, OrderBook, MarketData, Progress, TransactionSide, BarData, TransactionData
 
 from . import LOGGER
 
-__all__ = ['MDS', 'MarketDataService', 'MarketDataMonitor', 'Profile', 'ProgressiveReplay', 'SimpleReplay', 'Replay']
+__all__ = ['MDS', 'MarketDataService', 'MarketDataMonitor', 'SyntheticOrderBookMonitor', 'MinuteBarMonitor', 'Profile', 'ProgressiveReplay', 'SimpleReplay', 'Replay']
 LOGGER = LOGGER.getChild('MarketEngine')
 
 
 class MarketDataMonitor(object, metaclass=abc.ABCMeta):
+    """
+    this is a template for market data monitor
+
+    A data monitor is a module that process market data and generate custom index
+
+    When MDS receive an update of market data, the __call__ function of this monitor is triggered.
+
+    Note: all the market_data, of all subscribed ticker will be fed into monitor. It should be assumed that a storage for multiple ticker is required.
+    To access the monitor, use `monitor = MDS[monitor_id]`
+    To access the index generated by the monitor, use `monitor.value`
+    To indicate that the monitor is ready to use set `monitor.is_ready = True`
+
+    The implemented monitor should be initialized and use `MDS.add_monitor(monitor)` to attach onto the engine
+    """
+
     def __init__(self, name: str, monitor_id: str = None, mds: MarketDataService = None):
         self.name = name
         self.monitor_id = uuid.uuid4().hex if monitor_id is None else monitor_id
         self.mds = MDS if mds is None else mds
 
     @abc.abstractmethod
     def __call__(self, market_data: MarketData, **kwargs): ...
 
-    @abc.abstractmethod
     @property
+    @abc.abstractmethod
     def value(self): ...
 
-    @abc.abstractmethod
     @property
+    @abc.abstractmethod
     def is_ready(self) -> bool: ...
 
 
 class SyntheticOrderBookMonitor(MarketDataMonitor):
     def __init__(self, keep_order_log: bool = False, **kwargs):
         self.keep_order_log = keep_order_log
 
@@ -113,15 +128,15 @@
 
 
 class MinuteBarMonitor(MarketDataMonitor):
     def __init__(self, interval: float = 60., **kwargs):
         self.interval = interval
 
         super().__init__(
-            name=kwargs.pop('name', 'Monitor.SyntheticOrderBook'),
+            name=kwargs.pop('name', 'Monitor.MinuteBarMonitor'),
             monitor_id=kwargs.pop('monitor_id', None),
             mds=kwargs.pop('mds', None),
         )
 
         self._minute_bar_data: dict[str, BarData] = {}
         self._last_bar_data: dict[str, BarData] = {}
 
@@ -461,14 +476,17 @@
             # override current orderbook
             self._order_book = _.order_book
 
     def __call__(self, **kwargs):
         if 'market_data' in kwargs:
             self.on_market_data(market_data=kwargs['market_data'])
 
+    def __getitem__(self, monitor_id: str) -> MarketDataMonitor:
+        return self._monitor[monitor_id]
+
     def add_monitor(self, monitor: MarketDataMonitor):
         self._monitor[monitor.monitor_id] = monitor
 
     def init_cn_override(self):
         self.profile = CN_Profile()
 
     def _on_trade_data(self, trade_data: TradeData):
@@ -767,14 +785,23 @@
             pass
         else:
             dtype = dtype.__name__
 
         topic = f'{ticker}.{dtype}'
         self.replay_subscription[topic] = (ticker, dtype)
 
+    def remove_subscription(self, ticker: str, dtype: type | str):
+        if isinstance(dtype, str):
+            pass
+        else:
+            dtype = dtype.__name__
+
+        topic = f'{ticker}.{dtype}'
+        self.replay_subscription.pop(topic, None)
+
     def reset(self):
         if self.calendar is None:
             md = self.start_date
             self.replay_calendar.clear()
 
             while md <= self.end_date:
                 self.replay_calendar.append(md)
@@ -813,18 +840,18 @@
 
     def next_task(self):
         if self.task_progress < len(self.replay_task):
             data = self.replay_task[self.task_progress]
             self.task_progress += 1
         else:
             if self.eod is not None and self.date_progress:
-                self.eod(market_date=self.replay_calendar[self.date_progress - 1])
+                self.eod(market_date=self.replay_calendar[self.date_progress - 1], replay=self)
 
             if self.bod is not None and self.date_progress < len(self.replay_calendar):
-                self.bod(market_date=self.replay_calendar[self.date_progress])
+                self.bod(market_date=self.replay_calendar[self.date_progress], replay=self)
 
             self.next_trade_day()
 
             data = self.next_task()
 
         if self.replay_task and self.replay_calendar:
             current_progress = (self.date_progress - 1 + (self.task_progress / len(self.replay_task))) / len(self.replay_calendar)
```

### Comparing `PyAlgoEngine-0.3.2/AlgoEngine/Engine/TradeEngine.py` & `PyAlgoEngine-0.3.5/AlgoEngine/Engine/TradeEngine.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,19 +180,21 @@
 
     a range of easy method is provided to facilitate development
     """
 
     def __init__(
             self,
             dma: DirectMarketAccess,
+            algo_engine=None,
             default_algo: str = None,
             **kwargs
     ):
         self.dma = dma
-        self.algo_registry = ALGO_ENGINE.registry
+        self.algo_engine = algo_engine if algo_engine is not None else ALGO_ENGINE
+        self.algo_registry = self.algo_engine.registry
         self.default_algo = self.algo_registry.passive if default_algo is None else default_algo
         self.position_id = kwargs.pop('position_id', uuid.uuid4().hex)
         self.logger = kwargs.pop('logger', LOGGER)
 
         self.algos: dict[str, AlgoTemplate] = {}
         self.working_algos: dict[str, AlgoTemplate] = {}
 
@@ -357,14 +359,18 @@
     def algo_done(self, algo: AlgoTemplate):
         self.working_algos.pop(algo.algo_id, None)
 
     def algo_error(self, algo: AlgoTemplate):
         self.working_algos.pop(algo.algo_id, None)
         self.logger.warning(f'{algo} encounter error, manual intervention')
 
+    def clear(self):
+        self.algos.clear()
+        self.working_algos.clear()
+
     def pnl(self) -> dict[str, float]:
         pnl = {}
         for algo_id in list(self.algos):
             algo = self.algos.get(algo_id)
 
             if algo is None:
                 continue
@@ -545,16 +551,16 @@
 
 
 class Balance(object):
     """
     Balance handles mapping of PositionTracker <-> Strategy
     """
 
-    def __init__(self, **kwargs):
-        self.inventory: Inventory = kwargs.pop('inventory', None)
+    def __init__(self, inventory: Inventory = None):
+        self.inventory = inventory if inventory is not None else Inventory()
 
         self.strategy = {}
         self.trade_logs: list[TradeReport] = []
         self.position_tracker: dict[str, PositionManagementService] = {}
 
         self.last_update_timestamp = None
 
@@ -1953,18 +1959,18 @@
             if rules[key] is not None:
                 info_dict['global'][key] = rules[key]
 
         return pd.DataFrame(info_dict).T
 
 
 class SimMatch(object):
-    def __init__(self, ticker, **kwargs):
+    def __init__(self, ticker, event_engine=None, **kwargs):
         self.ticker = ticker
+        self.event_engine = event_engine if event_engine is not None else EVENT_ENGINE
         self.topic_set = kwargs.pop('topic_set', TOPIC)
-        self.event_engine = kwargs.pop('event_engine', EVENT_ENGINE)
 
         self.fee = kwargs.pop('fee', 0.)
         self.working: dict[str, TradeInstruction] = {}
         self.history: dict[str, TradeInstruction] = {}
 
         self.market_time = datetime.datetime.min
```

### Comparing `PyAlgoEngine-0.3.2/AlgoEngine/Engine/__init__.py` & `PyAlgoEngine-0.3.5/AlgoEngine/Engine/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,11 +88,14 @@
     LOGGER = logger
 
 
 _ = get_logger()
 
 from .EventEngine import EVENT_ENGINE, TOPIC
 from .AlgoEngine import AlgoTemplate, ALGO_ENGINE, ALGO_REGISTRY
-from .MarketEngine import MDS, MarketDataService, ProgressiveReplay, SimpleReplay, Replay
+from .MarketEngine import MDS, MarketDataService, MarketDataMonitor, SyntheticOrderBookMonitor, MinuteBarMonitor, ProgressiveReplay, SimpleReplay, Replay
 from .TradeEngine import DirectMarketAccess, Balance, PositionManagementService, Inventory, RiskProfile, SimMatch
 
-__all__ = ['set_logger', 'LOGGER', 'EVENT_ENGINE', 'TOPIC', 'AlgoTemplate', 'ALGO_ENGINE', 'ALGO_REGISTRY', 'MDS', 'MarketDataService', 'ProgressiveReplay', 'SimpleReplay', 'Replay', 'DirectMarketAccess', 'Balance', 'PositionManagementService', 'Inventory', 'RiskProfile', 'SimMatch']
+__all__ = ['set_logger', 'LOGGER', 'EVENT_ENGINE', 'TOPIC',
+           'AlgoTemplate', 'ALGO_ENGINE', 'ALGO_REGISTRY',
+           'MDS', 'MarketDataService', 'MarketDataMonitor', 'SyntheticOrderBookMonitor', 'MinuteBarMonitor', 'ProgressiveReplay', 'SimpleReplay', 'Replay',
+           'DirectMarketAccess', 'Balance', 'PositionManagementService', 'Inventory', 'RiskProfile', 'SimMatch']
```

### Comparing `PyAlgoEngine-0.3.2/AlgoEngine/Strategies/_StrategyEngine.py` & `PyAlgoEngine-0.3.5/AlgoEngine/Strategies/_StrategyEngine.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 
 
 class StrategyEngine(StrategyEngineTemplate):
     def __init__(self, position_tracker: PositionManagementService, **kwargs):
         super().__init__(position_tracker=position_tracker)
 
         self.mds = kwargs.pop('mds', MDS)
+        self.event_engine = kwargs.pop('event_engine', EVENT_ENGINE)
         self.multi_threading = kwargs.pop('multi_threading', False)
         self.lock = threading.Lock()
-        self.event_engine = kwargs.pop('event_engine', EVENT_ENGINE)
         self.topic_set = kwargs.pop('topic_set', TOPIC)
 
         self._on_market_data = []
         self._on_report = []
         self._on_order = []
         self._on_eod = []
         self._on_bod = []
@@ -256,23 +256,23 @@
             algo=algo,
             limit_price=limit_price,
             **kwargs
         )
 
         return algo
 
-    def eod(self, **kwargs):
+    def eod(self, market_date: datetime.date, **kwargs):
 
         for handler in self._on_eod:
-            handler(**kwargs)
+            handler(market_date=market_date, **kwargs)
 
-    def bod(self, **kwargs):
+    def bod(self, market_date: datetime.date, **kwargs):
 
         for handler in self._on_bod:
-            handler(**kwargs)
+            handler(market_date=market_date, **kwargs)
 
     def back_test(self, start_date: datetime.date, end_date: datetime.date, data_loader: callable, **kwargs):
         from ..Engine import ProgressiveReplay
 
         replay = ProgressiveReplay(
             loader=data_loader,
             tickers=list(self.subscription),
```

### Comparing `PyAlgoEngine-0.3.2/AlgoEngine/Strategies/__init__.py` & `PyAlgoEngine-0.3.5/AlgoEngine/Strategies/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 from __future__ import annotations
 
 import threading
 
 from PyQuantKit import TradeInstruction
 
+from ._StrategyEngine import StrategyEngine
 from ..Engine import LOGGER
 from ..Engine.EventEngine import EVENT_ENGINE, TOPIC
-from ..Engine.MarketEngine import MDS
-from ..Engine.TradeEngine import Balance, DirectMarketAccess, RiskProfile, PositionManagementService
+from ..Engine.MarketEngine import MDS, MarketDataService
+from ..Engine.TradeEngine import Balance, Inventory, DirectMarketAccess, RiskProfile, PositionManagementService
 
 LOGGER = LOGGER.getChild('Strategies')
 
 
-class SimDMA(DirectMarketAccess):
+class EventDMA(DirectMarketAccess):
+    def __init__(self, mds: MarketDataService, risk_profile: RiskProfile, event_engine=None, cool_down: float = None):
+        self.event_engine = EVENT_ENGINE if event_engine is None else event_engine
+        super().__init__(mds=mds, risk_profile=risk_profile, cool_down=cool_down)
 
     def _launch_order_handler(self, order: TradeInstruction, **kwargs):
-        EVENT_ENGINE.put(topic=TOPIC.launch_order(ticker=order.ticker), order=order, **kwargs)
+        self.event_engine.put(topic=TOPIC.launch_order(ticker=order.ticker), order=order, **kwargs)
 
     def _cancel_order_handler(self, order: TradeInstruction, **kwargs):
-        EVENT_ENGINE.put(topic=TOPIC.cancel_order(ticker=order.ticker), order_id=order.order_id, **kwargs)
+        self.event_engine.put(topic=TOPIC.cancel_order(ticker=order.ticker), order_id=order.order_id, **kwargs)
 
     def _reject_order_handler(self, order: TradeInstruction, **kwargs):
         raise NotImplementedError()
 
 
 REPLAY_LOCK = threading.Lock()
-BALANCE = Balance()
+INVENTORY = Inventory()
+BALANCE = Balance(inventory=INVENTORY)
 RISK_PROFILE = RiskProfile(mds=MDS, balance=BALANCE)
-DMA = SimDMA(mds=MDS, risk_profile=RISK_PROFILE)
+DMA = EventDMA(mds=MDS, risk_profile=RISK_PROFILE)
 POSITION_TRACKER = PositionManagementService(dma=DMA)
-BALANCE.add(position_tracker=POSITION_TRACKER)
+STRATEGY_ENGINE = StrategyEngine(event_engine=EVENT_ENGINE, position_tracker=POSITION_TRACKER)
+BALANCE.add(strategy=STRATEGY_ENGINE, position_tracker=POSITION_TRACKER)
+
+__all__ = ['INVENTORY', 'BALANCE', 'RISK_PROFILE', 'DMA', 'POSITION_TRACKER', 'STRATEGY_ENGINE']
```

### Comparing `PyAlgoEngine-0.3.2/LICENSE` & `PyAlgoEngine-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.2/PKG-INFO` & `PyAlgoEngine-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.2
+Version: 0.3.5
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `PyAlgoEngine-0.3.2/PyAlgoEngine.egg-info/PKG-INFO` & `PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.2
+Version: 0.3.5
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `PyAlgoEngine-0.3.2/setup.py` & `PyAlgoEngine-0.3.5/setup.py`

 * *Files identical despite different names*

