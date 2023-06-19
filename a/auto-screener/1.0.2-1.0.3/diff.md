# Comparing `tmp/auto-screener-1.0.2.tar.gz` & `tmp/auto-screener-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-1.0.2.tar", last modified: Sun Jun 18 16:06:35 2023, max compression
+gzip compressed data, was "auto-screener-1.0.3.tar", last modified: Mon Jun 19 17:20:02 2023, max compression
```

## Comparing `auto-screener-1.0.2.tar` & `auto-screener-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:06:35.272418 auto-screener-1.0.2/
--rw-rw-rw-   0        0        0       98 2023-06-18 16:06:35.000000 auto-screener-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-06-18 16:06:35.272418 auto-screener-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 16:06:35.267418 auto-screener-1.0.2/auto_screener/
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-1.0.2/auto_screener/base.py
--rw-rw-rw-   0        0        0    17321 2023-06-17 15:18:59.000000 auto-screener-1.0.2/auto_screener/collect.py
--rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-1.0.2/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-1.0.2/auto_screener/document.py
--rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-1.0.2/auto_screener/exchanges.py
--rw-rw-rw-   0        0        0    26655 2023-06-18 16:06:18.000000 auto-screener-1.0.2/auto_screener/feed.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-1.0.2/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-1.0.2/auto_screener/interval.py
--rw-rw-rw-   0        0        0    33713 2023-06-17 15:16:47.000000 auto-screener-1.0.2/auto_screener/screener.py
--rw-rw-rw-   0        0        0    32231 2023-06-17 15:14:52.000000 auto-screener-1.0.2/auto_screener/screening.py
--rw-rw-rw-   0        0        0    11992 2023-06-18 16:06:04.000000 auto-screener-1.0.2/auto_screener/symbols.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:06:35.271418 auto-screener-1.0.2/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-1.0.2/build.py
--rw-rw-rw-   0        0        0      645 2023-06-18 16:06:35.000000 auto-screener-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       79 2023-06-17 10:23:38.000000 auto-screener-1.0.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       70 2023-06-17 10:23:38.000000 auto-screener-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 16:06:35.272418 auto-screener-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1564 2023-06-18 16:06:25.000000 auto-screener-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:20:02.376059 auto-screener-1.0.3/
+-rw-rw-rw-   0        0        0       98 2023-06-19 17:20:02.000000 auto-screener-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-06-19 17:20:02.375681 auto-screener-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 17:20:02.369681 auto-screener-1.0.3/auto_screener/
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-1.0.3/auto_screener/base.py
+-rw-rw-rw-   0        0        0    17321 2023-06-17 15:18:59.000000 auto-screener-1.0.3/auto_screener/collect.py
+-rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-1.0.3/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-1.0.3/auto_screener/document.py
+-rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-1.0.3/auto_screener/exchanges.py
+-rw-rw-rw-   0        0        0    26519 2023-06-19 17:00:23.000000 auto-screener-1.0.3/auto_screener/feed.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-1.0.3/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-1.0.3/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    33904 2023-06-19 17:00:38.000000 auto-screener-1.0.3/auto_screener/screener.py
+-rw-rw-rw-   0        0        0    32231 2023-06-17 15:14:52.000000 auto-screener-1.0.3/auto_screener/screening.py
+-rw-rw-rw-   0        0        0    11992 2023-06-18 16:06:04.000000 auto-screener-1.0.3/auto_screener/symbols.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:20:02.374680 auto-screener-1.0.3/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-19 17:20:02.000000 auto-screener-1.0.3/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-06-19 17:20:02.000000 auto-screener-1.0.3/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 17:20:02.000000 auto-screener-1.0.3/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-06-19 17:20:02.000000 auto-screener-1.0.3/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 17:20:02.000000 auto-screener-1.0.3/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-1.0.3/build.py
+-rw-rw-rw-   0        0        0      645 2023-06-19 17:20:02.000000 auto-screener-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       79 2023-06-17 10:23:38.000000 auto-screener-1.0.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       70 2023-06-17 10:23:38.000000 auto-screener-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 17:20:02.376059 auto-screener-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-06-19 17:03:45.000000 auto-screener-1.0.3/setup.py
```

### Comparing `auto-screener-1.0.2/PKG-INFO` & `auto-screener-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 1.0.2
+Version: 1.0.3
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-1.0.2/README.md` & `auto-screener-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/auto_screener/base.py` & `auto-screener-1.0.3/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/auto_screener/collect.py` & `auto-screener-1.0.3/auto_screener/collect.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/auto_screener/dataset.py` & `auto-screener-1.0.3/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/auto_screener/document.py` & `auto-screener-1.0.3/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/auto_screener/feed.py` & `auto-screener-1.0.3/auto_screener/feed.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import (
     Dict, Optional, Iterable, Any,
     Union, Callable, List, Type
 )
 
 import pandas as pd
 
-from represent import Modifiers, BaseModel
+from represent import Modifiers
 
 from cryptofeed import FeedHandler
 from cryptofeed.feed import Feed
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from auto_screener.dataset import (
@@ -121,17 +121,14 @@
     >>> from auto_screener.feed import market_order_book_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = market_order_book_recorder(data=market)
     """
 
-    modifiers = Modifiers(**BaseModel.modifiers)
-    modifiers.excluded.append("market")
-
     __slots__ = "market"
 
     COLUMNS = (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME)
 
     def parameters(self) -> RecorderParameters:
         """
         Returns the order book parameters.
@@ -401,20 +398,22 @@
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> screener = market_order_book_screener(data=structure)
     >>> screener.run()
     """
 
     modifiers = Modifiers(**BaseMultiScreener.modifiers)
-    modifiers.excluded.extend(['update_process'])
+    modifiers.excluded.extend(
+        ['screening_parameters', 'feeds_parameters', 'handler']
+    )
 
     __slots__ = (
-        "handler", "recorder", "updating",
-        "update_process", "loop", "limited",
-        "feeds_parameters", "screening_parameters"
+        "handler", 'amount',
+        "loop", "limited", "feeds_parameters",
+        "screening_parameters", 'refresh'
     )
 
     DELAY = 10
     AMOUNT = 50
 
     REFRESH = dt.timedelta(minutes=5)
 
@@ -462,15 +461,14 @@
         self.handler = handler or MarketHandler()
         self.limited = limited or False
         self.amount = amount or self.AMOUNT
         self.refresh = refresh
 
         self.screeners[:] = list(screeners or []) or self.create_screeners()
 
-        self.update_process: Optional[threading.Thread] = None
         self.loop: Optional[asyncio.AbstractEventLoop] = None
 
         self.feeds_parameters: Optional[Dict[str, Any]] = None
         self.screening_parameters: Optional[Dict[str, Any]] = None
     # end __init__
 
     def create_screener(
```

### Comparing `auto-screener-1.0.2/auto_screener/interval.py` & `auto-screener-1.0.3/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/auto_screener/screener.py` & `auto-screener-1.0.3/auto_screener/screener.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "structure_screener_datasets",
     "validate_market"
 ]
 
 class WaitingState(BaseModel):
     """A class to represent the waiting state of screener objects."""
 
-    modifiers = Modifiers(excluded=["create_screeners"])
+    modifiers = Modifiers(hidden=["screeners"], properties=["time"])
 
     __slots__ = "screeners", "delay", "count", "canceled", "cancel"
 
     def __init__(
             self,
             screeners: Iterable,
             delay: Number,
@@ -92,18 +92,24 @@
 class DataCollector(BaseModel, metaclass=ABCMeta):
     """A class to represent an abstract parent class of data collectors."""
 
     modifiers = Modifiers(**BaseModel.modifiers)
     modifiers.excluded.extend(
         [
             'screening_process', 'timeout_process',
-            'saving_process'
+            'saving_process', 'update_process'
         ]
     )
 
+    __slots__ = (
+        'screening_process', 'timeout_process',
+        'saving_process', 'update_process',
+        "location", "cancel", "delay", "market"
+    )
+
     LOCATION = "datasets"
 
     DELAY = 0.0
     CANCEL = 0
 
     def __init__(
             self,
@@ -422,17 +428,17 @@
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
     """
 
     modifiers = Modifiers(**DataCollector.modifiers)
-    modifiers.excluded.append("market")
+    modifiers.hidden.append("market")
 
-    __slots__ = "symbol", "exchange", "location", "cancel", "delay", "market"
+    __slots__ = "symbol", "exchange", "market"
 
     def __init__(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
             cancel: Optional[Union[Number, dt.timedelta]] = None,
@@ -610,15 +616,15 @@
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = market_order_book_recorder(data=market)
 
     """
 
     modifiers = Modifiers(**BaseModel.modifiers)
-    modifiers.excluded.append("market")
+    modifiers.hidden.append("market")
 
     __slots__ = "market"
 
     def __init__(self, market: Optional[Market] = None) -> None:
         """
         Defines the class attributes.
 
@@ -714,19 +720,19 @@
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
     """
 
     modifiers = Modifiers(**DataCollector.modifiers)
-    modifiers.excluded.append("market")
+    modifiers.hidden.extend(["screeners", 'market'])
 
     screeners: List[BaseScreener]
 
-    __slots__ = "screeners", "location", "cancel", "delay"
+    __slots__ = "screeners", "location", "cancel", "delay", 'recorder'
 
     def __init__(
             self,
             screeners: Optional[Iterable[BaseScreener]] = None,
             recorder: Optional[MarketRecorder] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[Number, dt.timedelta]] = None,
```

### Comparing `auto-screener-1.0.2/auto_screener/screening.py` & `auto-screener-1.0.3/auto_screener/screening.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/auto_screener/symbols.py` & `auto-screener-1.0.3/auto_screener/symbols.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/auto_screener.egg-info/PKG-INFO` & `auto-screener-1.0.3/auto_screener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 1.0.2
+Version: 1.0.3
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-1.0.2/auto_screener.egg-info/SOURCES.txt` & `auto-screener-1.0.3/auto_screener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/build.py` & `auto-screener-1.0.3/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.2/pyproject.toml` & `auto-screener-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '1.0.2'
+version = '1.0.3'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-1.0.2/setup.py` & `auto-screener-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='1.0.2',
+        version='1.0.3',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

