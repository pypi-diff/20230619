# Comparing `tmp/aiomql-1.tar.gz` & `tmp/aiomql-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomql-1.tar", last modified: Thu Feb 23 16:00:25 2023, max compression
+gzip compressed data, was "aiomql-2.0.tar", last modified: Mon Jun 19 00:29:56 2023, max compression
```

## Comparing `aiomql-1.tar` & `aiomql-2.0.tar`

### file list

```diff
@@ -1,54 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:25.348288 aiomql-1/
--rw-rw-rw-   0        0        0     1092 2023-02-23 15:40:36.000000 aiomql-1/LICENSE
--rw-rw-rw-   0        0        0     3261 2023-02-23 16:00:25.341291 aiomql-1/PKG-INFO
--rw-rw-rw-   0        0        0     2649 2023-02-23 15:40:36.000000 aiomql-1/README.md
--rw-rw-rw-   0        0        0      803 2023-02-23 15:59:03.000000 aiomql-1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-23 16:00:25.350291 aiomql-1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-23 15:40:36.000000 aiomql-1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:21.978362 aiomql-1/src/
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.372289 aiomql-1/src/aiomql/
--rw-rw-rw-   0        0        0      615 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/__init__.py
--rw-rw-rw-   0        0        0     1907 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/account.py
--rw-rw-rw-   0        0        0     4370 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/bot_builder.py
--rw-rw-rw-   0        0        0     3331 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/candle.py
--rw-rw-rw-   0        0        0     4106 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/config.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.704292 aiomql-1/src/aiomql/core/
--rw-rw-rw-   0        0        0     3683 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/core/__init__.py
--rw-rw-rw-   0        0        0    37666 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/core/constants.py
--rw-rw-rw-   0        0        0     6686 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/core/meta_trader.py
--rw-rw-rw-   0        0        0    15918 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/core/models.py
--rw-rw-rw-   0        0        0     2221 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/executor.py
--rw-rw-rw-   0        0        0     4542 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/history.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:23.719453 aiomql-1/src/aiomql/lib/
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.829289 aiomql-1/src/aiomql/lib/markets/
--rw-rw-rw-   0        0        0      442 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/markets/forex_market.py
--rw-rw-rw-   0        0        0      500 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/markets/synthetic_market.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.923290 aiomql-1/src/aiomql/lib/strategies/
--rw-rw-rw-   0        0        0     5433 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/strategies/finger_trap.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.946292 aiomql-1/src/aiomql/lib/symbols/
--rw-rw-rw-   0        0        0     1166 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/symbols/forex_symbol.py
--rw-rw-rw-   0        0        0      767 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/symbols/synthetic_symbol.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:25.035291 aiomql-1/src/aiomql/lib/traders/
--rw-rw-rw-   0        0        0     2715 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/traders/simple_deal_trader.py
--rw-rw-rw-   0        0        0     4261 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/market.py
--rw-rw-rw-   0        0        0     3915 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/order.py
--rw-rw-rw-   0        0        0     2885 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/positions.py
--rw-rw-rw-   0        0        0     3436 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/records.py
--rw-rw-rw-   0        0        0     3344 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/result.py
--rw-rw-rw-   0        0        0     3161 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/strategy.py
--rw-rw-rw-   0        0        0     8748 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/symbol.py
--rw-rw-rw-   0        0        0     5865 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/terminal.py
--rw-rw-rw-   0        0        0     1617 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/ticks.py
--rw-rw-rw-   0        0        0     1286 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/trader.py
--rw-rw-rw-   0        0        0      111 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.585287 aiomql-1/src/aiomql.egg-info/
--rw-rw-rw-   0        0        0     3261 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:25.288289 aiomql-1/tests/
--rw-rw-rw-   0        0        0      331 2023-02-23 15:40:36.000000 aiomql-1/tests/test_config.py
--rw-rw-rw-   0        0        0      132 2023-02-23 15:40:36.000000 aiomql-1/tests/test_constants.py
--rw-rw-rw-   0        0        0      224 2023-02-23 15:40:36.000000 aiomql-1/tests/test_symbol.py
--rw-rw-rw-   0        0        0      602 2023-02-23 15:40:36.000000 aiomql-1/tests/test_terminal.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.243166 aiomql-2.0/
+-rw-rw-rw-   0        0        0     1092 2023-04-10 06:55:09.000000 aiomql-2.0/LICENSE
+-rw-rw-rw-   0        0        0     2279 2023-06-19 00:29:56.217265 aiomql-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1665 2023-06-19 00:06:32.000000 aiomql-2.0/README.md
+-rw-rw-rw-   0        0        0      805 2023-06-19 00:12:54.000000 aiomql-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 00:29:56.244175 aiomql-2.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-10 06:55:09.000000 aiomql-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:55.972977 aiomql-2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.080952 aiomql-2.0/src/aiomql/
+-rw-rw-rw-   0        0        0      596 2023-06-18 23:07:33.000000 aiomql-2.0/src/aiomql/__init__.py
+-rw-rw-rw-   0        0        0     3453 2023-06-18 23:08:38.000000 aiomql-2.0/src/aiomql/account.py
+-rw-rw-rw-   0        0        0     3942 2023-06-18 23:07:05.000000 aiomql-2.0/src/aiomql/bot_builder.py
+-rw-rw-rw-   0        0        0     6495 2023-06-18 23:07:05.000000 aiomql-2.0/src/aiomql/candle.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.137174 aiomql-2.0/src/aiomql/core/
+-rw-rw-rw-   0        0        0       63 2023-06-13 22:43:24.000000 aiomql-2.0/src/aiomql/core/__init__.py
+-rw-rw-rw-   0        0        0     4805 2023-06-18 23:45:07.000000 aiomql-2.0/src/aiomql/core/base.py
+-rw-rw-rw-   0        0        0     4283 2023-06-18 22:58:34.000000 aiomql-2.0/src/aiomql/core/config.py
+-rw-rw-rw-   0        0        0    38105 2023-06-18 22:58:34.000000 aiomql-2.0/src/aiomql/core/constants.py
+-rw-rw-rw-   0        0        0    11636 2023-06-18 21:01:29.000000 aiomql-2.0/src/aiomql/core/meta_trader.py
+-rw-rw-rw-   0        0        0    16685 2023-06-18 23:45:07.000000 aiomql-2.0/src/aiomql/core/models.py
+-rw-rw-rw-   0        0        0     2241 2023-06-17 14:58:44.000000 aiomql-2.0/src/aiomql/executor.py
+-rw-rw-rw-   0        0        0     5069 2023-06-17 15:12:23.000000 aiomql-2.0/src/aiomql/history.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.140691 aiomql-2.0/src/aiomql/lib/
+-rw-rw-rw-   0        0        0      198 2023-06-13 22:14:26.000000 aiomql-2.0/src/aiomql/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.150924 aiomql-2.0/src/aiomql/lib/strategies/
+-rw-rw-rw-   0        0        0        0 2023-05-06 20:55:40.000000 aiomql-2.0/src/aiomql/lib/strategies/__init__.py
+-rw-rw-rw-   0        0        0     6913 2023-06-19 00:04:09.000000 aiomql-2.0/src/aiomql/lib/strategies/finger_trap.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.166616 aiomql-2.0/src/aiomql/lib/symbols/
+-rw-rw-rw-   0        0        0       86 2023-06-10 11:42:24.000000 aiomql-2.0/src/aiomql/lib/symbols/__init__.py
+-rw-rw-rw-   0        0        0     1581 2023-06-18 22:00:12.000000 aiomql-2.0/src/aiomql/lib/symbols/forex_symbol.py
+-rw-rw-rw-   0        0        0     1376 2023-06-18 23:46:29.000000 aiomql-2.0/src/aiomql/lib/symbols/synthetic_symbol.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.213254 aiomql-2.0/src/aiomql/lib/traders/
+-rw-rw-rw-   0        0        0     3079 2023-06-18 23:53:33.000000 aiomql-2.0/src/aiomql/lib/traders/simple_deal_trader.py
+-rw-rw-rw-   0        0        0      927 2023-06-18 22:11:18.000000 aiomql-2.0/src/aiomql/lib/traders/trade_result.py
+-rw-rw-rw-   0        0        0     3713 2023-06-18 23:53:33.000000 aiomql-2.0/src/aiomql/order.py
+-rw-rw-rw-   0        0        0     2537 2023-06-17 17:16:06.000000 aiomql-2.0/src/aiomql/positions.py
+-rw-rw-rw-   0        0        0     2822 2023-06-17 17:16:06.000000 aiomql-2.0/src/aiomql/records.py
+-rw-rw-rw-   0        0        0     1596 2023-06-17 17:28:36.000000 aiomql-2.0/src/aiomql/result.py
+-rw-rw-rw-   0        0        0     3284 2023-06-18 23:15:46.000000 aiomql-2.0/src/aiomql/strategy.py
+-rw-rw-rw-   0        0        0    11721 2023-06-18 21:32:40.000000 aiomql-2.0/src/aiomql/symbol.py
+-rw-rw-rw-   0        0        0     2698 2023-06-18 21:41:02.000000 aiomql-2.0/src/aiomql/terminal.py
+-rw-rw-rw-   0        0        0     3127 2023-06-18 23:07:05.000000 aiomql-2.0/src/aiomql/ticks.py
+-rw-rw-rw-   0        0        0     1160 2023-06-18 23:46:29.000000 aiomql-2.0/src/aiomql/trader.py
+-rw-rw-rw-   0        0        0      246 2023-06-18 21:41:01.000000 aiomql-2.0/src/aiomql/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:29:56.102916 aiomql-2.0/src/aiomql.egg-info/
+-rw-rw-rw-   0        0        0     2279 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1033 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 00:29:55.000000 aiomql-2.0/src/aiomql.egg-info/top_level.txt
```

### Comparing `aiomql-1/LICENSE` & `aiomql-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomql-1/PKG-INFO` & `aiomql-2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 1
+Version: 2.0
 Summary: Asynchronous MetaTrader5 library and Bot Builder
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,86 +13,65 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiomql
 ![GitHub](https://img.shields.io/github/license/ichinga-samuel/aiomql?style=plastic)
 ![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/aiomql?style=plastic)
 ![PyPI](https://img.shields.io/pypi/v/aiomql)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ichinga-samuel/aiomql/Push)
-![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/ichinga-samuel/aiomql)
+
 
 ## Installation
 ```bash
 pip install aiomql
 ```
 
 ## Key Features
 - Asynchronous Python Library For MetaTrader 5
 - Build bots for trading in different financial markets using a bot factory
-- Use threadpool or proccesspool executors to run multiple strategies on multiple instruments concurrently
+- Use threadpool executors to run multiple strategies on multiple instruments concurrently
 - Record and keep track of trades and strategies in csv files.
 - Utility classes for using the MetaTrader 5 Library
 - Sample Pre-Built strategies
 
-## Simple Usage as an Async MetaTrader5 Libray
+## Simple Usage as an asynchronous MetaTrader5 Libray
 ```python
 import asyncio
 
 # import the class
-from aiomql import MetaTrader
-from aiomql import Account, Terminal
-from aiomql import TimeFrame, OrderType
+from aiomql import MetaTrader, Account, TimeFrame, OrderType
 
 
 async def main():
-    # Initialize Terminal
-    terminal = Terminal()
-    mt5 = MetaTrader()
-    await mt5.initialize()
-
-    # create Account
-    account = Account(account_number=30371334, password="nwa0#anaEze", server="Deriv-Demo")
-
-    # login with account
-    await account.login()
-
-    # connection status with the account.connected property
-    res = "Login Successful" if account.connected else "Unable to login into account"
-    print(res)
-
-    # set account properties
-    account.risk = 0.10  # percentage of account equity to risk i.e 10%
-    account.risk_to_reward = 3
-
-    # get symbols available for the account if login was successful
-    if account.connected:
-        symbols = await mt5.symbols_get()
-        print(symbols)
-
-    # print timeframe constant for five minutes
-    print(TimeFrame.M5)
-    await terminal.shutdown()
-
+    # Assuming your login details are already defined in the aiomql.json somewhere in your project directory. 
+    acc = Account()
+    
+    # if this is unsuccessful the program exits
+    await acc.sign_in()
+    
+    # print all available symbols
+    print(acc.symbols)
 
 asyncio.run(main())
 ```
-## As a Bot Building FrameWork using a Prebuilt Strategy
+## As a Bot Building FrameWork using a Sample Strategy
 ```python
-import logging
-
 from aiomql import Bot
-from aiomql.lib import ForexMarket, FingerTrap
+from aiomql import ForexSymbol
+from aiomql.lib import FingerTrap
+
+# Create a bot instance
+bot = Bot()
 
-fmt = "%(asctime)s : %(message)s"
+# Choose a Symbol to trade
+symbol = ForexSymbol(name='EURUSD')
 
-logging.basicConfig(filename='example.log', format=fmt, level=logging.DEBUG)
+# Create a strategy
+ft_eur_usd = FingerTrap(symbol=symbol)
 
-market = ForexMarket()
-bot = Bot(market=market)
+# Add strategy to Bot
+bot.add_strategy(ft_eur_usd)
 
-# Finger strategy on all instruments in the forex markets
-bot.add_strategy_all(strategy=FingerTrap)
+# run the bot
 bot.execute()
-# This assumes that a mt5.json config file with account_number, password and server keys is available
 ```
 
 see [docs](https://github.com/Ichinga-Samuel/aiomql/tree/master/docs)
```

### Comparing `aiomql-1/pyproject.toml` & `aiomql-2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiomql"
-version = "1"
+version = "2.0"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `aiomql-1/src/aiomql/__init__.py` & `aiomql-2.0/src/aiomql/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from .account import Account, account
+from .account import Account
 from .symbol import Symbol
-from .strategy import Strategy, Entry
+from .strategy import Strategy
 from .bot_builder import Bot
-from .result import TradeResult
+from .result import Result
 from .records import Records
 from .candle import Candle, Candles
 from .positions import Positions
 from .executor import Executor
 from .order import Order
-from .ticks import Tick
+from .ticks import Tick, Ticks
 from .history import History
 from .trader import Trader
-from .market import Market
-from .terminal import Terminal, terminal
-from .config import Config
+from .terminal import Terminal
 
+from .core.config import Config
 from .core .constants import *
 from .core .meta_trader import MetaTrader
 from .core .models import *
+from .lib.symbols import *
```

### Comparing `aiomql-1/src/aiomql/account.py` & `aiomql-2.0/src/aiomql/account.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,95 @@
-from .core.meta_trader import MetaTrader
-from .core.models import AccountInfo
+from logging import getLogger
+from typing import Type
 
+from .core.models import AccountInfo, SymbolInfo
 
-class Account(AccountInfo):
-    """
-    Properties and methods of the current trading account. Subclass of AccountInfo
 
-    Args:
-        mt5 (MetaTrader): The Meta trader object for connecting to the terminal. Default Keyword Argument
-        kwargs: Arguments for AccountInfo attributes
+logger = getLogger()
+
+
+class Account(AccountInfo):
+    """A Subclass of AccountInfo and the Base class
+    Properties and methods for working with the current trading account are defined here.
+    This is a singleton class as you can only use one account at a time.
 
     Attributes:
         risk (float): Percentage of account to risk
         risk_to_reward (float): ratio of risk to reward
-        connected (float):
+        connected (bool): Status of connection to MetaTrader 5 Terminal
+        symbols (set[SymbolInfo]): A set of available symbols for the financial market.
 
     Notes:
-        Other Account properties are defined in the AccountInfo Object
-        Since bot can only use one account at a time use the account class as a module style singleton object by importing the account object declared
-        in this module instead of creating a new object.
+        Other Account properties are defined in the AccountInfo class.
     """
     risk: float = 0.05
     risk_to_reward: float = 2
     connected: bool
-
-    def __init__(self, mt5: MetaTrader = MetaTrader(), **kwargs):
-        self.mt5 = mt5
-        super().__init__(**kwargs)
+    symbols = set()
+    
+    def __new__(cls, *args, **kwargs):
+        if not hasattr(cls, '_instance'):
+            cls._instance = super().__new__(cls)
+        return cls._instance
 
     async def refresh(self):
         """
-        Update the account info object with latest values from the terminal
-        Returns:
-            Account: The Account Object with updated properties
-
+        Update the account info instance with the latest values from the terminal
         """
         account_info = await self.mt5.account_info()
         acc = account_info._asdict()
-        acc['account_number'] = acc['login']
-        del acc['login']
         self.set_attributes(**acc)
 
-    async def login(self):
+    @property
+    def account_info(self) -> dict:
+        """Creates a dictionary of login details.
+        Looks for login details in both the instance and the global config instance.
+        login details defined in the account instance takes precedence over those in the config instance
+
+        Returns (dict): A dict of login, server and password details
+
+        Note:
+            This method will only look for config details in the config instance if the login attribute of the
+            account Instance returns a falsy value
         """
-        Make sure account_number, password and server attributes have been initialized
-        Returns: True if login was successful else False
+        acc_info = self.get_dict(include={'login', 'server', 'password'})
+        return acc_info if acc_info['login'] else self.config.account_info()
+
+    async def sign_in(self) -> bool:
+        """Connect to a trading account.
 
+        Returns:
+            bool: True if login was successful else False
         """
-        self.connected = await self.mt5.login(login=self.account_number, password=self.password, server=self.server)
+        await self.mt5.initialize(**self.account_info)
+        self.connected = await self.mt5.login(**self.account_info)
         if self.connected:
             await self.refresh()
-        return self.connected
+            self.symbols = await self.symbols_get()
+            return self.connected
+        await self.mt5.shutdown()
+        return False
+
+    def has_symbol(self, symbol: str | Type[SymbolInfo]):
+        """Checks to see if a symbol is available for a trading account
+
+        Args:
+            symbol (str | SymbolInfo):
+
+        Returns:
+            bool: True if symbol is present otherwise False
+        """
+        try:
+            symbol = SymbolInfo(name=symbol) if isinstance(symbol, str) else symbol
+            return symbol in self.symbols
+        except Exception as err:
+            logger.warning(f'Error: {err}; {symbol} not available in this market')
+            return False
 
+    async def symbols_get(self) -> set[SymbolInfo]:
+        """Get all financial instruments from the MetaTrader 5 terminal available for the current account.
 
-account = Account()
+        Returns:
+            set[Symbol]: A set of available symbols.
+        """
+        syms = await self.mt5.symbols_get()
+        return {SymbolInfo(name=sym.name) for sym in syms}
```

### Comparing `aiomql-1/src/aiomql/core/constants.py` & `aiomql-2.0/src/aiomql/core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 from enum import IntEnum, IntFlag
 
 import MetaTrader5 as mt5
 
 """
 MetaTrader5 constants as IntEnum types with Python style class names and better string representation
+
 Examples:
     >>> from aiomql import OrderFilling 
     
     >>> filling = OrderFilling.FOK
     >>> print(filling)
     "ORDER_FILLING_FOK"
 """
 
 
 class Repr:
     __enum_name__ = ""
 
     def __str__(self):
-        return f"{self.__class__.__enum_name__}_{self.name}"
+        return f"{self.__enum_name__}_{self.name}"
 
 
 class TradeAction(Repr, IntEnum):
-    """
-    TRADE_REQUEST_ACTIONS
+    """TRADE_REQUEST_ACTIONS
     
     Attributes:
         DEAL (int): Delete the pending order placed previously Place a trade order for an immediate execution with the specified parameters (market order)
 
-
-        PENDING (int): Delete the pending order placed previously 
-
+        PENDING (int): Delete the pending order placed previously
 
         SLTP (int): Modify Stop Loss and Take Profit values of an opened position 
 
+        MODIFY (int): Modify the parameters of the order placed previously
 
-        MODIFY (int): Modify the parameters of the order placed previously 
-
-
-        REMOVE (int): Delete the pending order placed previously 
-
+        REMOVE (int): Delete the pending order placed previously
 
         CLOSE_BY (int): Close a position by an opposite one 
     """
     __enum_name__ = "TRADE_ACTION"
     DEAL = mt5.TRADE_ACTION_DEAL
     PENDING = mt5.TRADE_ACTION_PENDING
     SLTP = mt5.TRADE_ACTION_SLTP
@@ -222,14 +217,18 @@
 
         MN1 (int): One Month
 
     Methods:
         time: return the value of the timeframe object in seconds. Used as a property
     """
     __enum_name__ = "TIMEFRAME"
+
+    def __str__(self):
+        return self.name
+
     M1 = mt5.TIMEFRAME_M1
     M2 = mt5.TIMEFRAME_M2
     M3 = mt5.TIMEFRAME_M3
     M4 = mt5.TIMEFRAME_M4
     M5 = mt5.TIMEFRAME_M5
     M6 = mt5.TIMEFRAME_M6
     M10 = mt5.TIMEFRAME_M10
@@ -237,35 +236,43 @@
     M20 = mt5.TIMEFRAME_M20
     M30 = mt5.TIMEFRAME_M30
     H1 = mt5.TIMEFRAME_H1
     H2 = mt5.TIMEFRAME_H2
     H3 = mt5.TIMEFRAME_H3
     H4 = mt5.TIMEFRAME_H4
     H6 = mt5.TIMEFRAME_H6
-    H8 = mt5.TIMEFRAME_H1
+    H8 = mt5.TIMEFRAME_H8
+    H12 = mt5.TIMEFRAME_H12
     D1 = mt5.TIMEFRAME_D1
     W1 = mt5.TIMEFRAME_W1
     MN1 = mt5.TIMEFRAME_MN1
 
     @property
     def time(self):
         """
 
         Returns:
             int: The number of seconds in a TIMEFRAME
 
         Examples:
             >>> t = TimeFrame.H1
             >>> print(t.time)
-            3600
         """
-        times = {1: 60, 2: 120, 3: 180, 4: 240, 5: 300, 6: 360, 10: 600, 15: 900, 20: 1200, 30: 1800, 16385: 3600, 16386: 7200,
-                 16387: 10800, 16388: 14400, 16390: 21600, 16392: 21800, 16408: 86400, 32769: 604800, 49153: 2592000}
+        times = {1: 60, 2: 120, 3: 180, 4: 240, 5: 300, 6: 360, 10: 600, 15: 900, 20: 1200, 30: 1800, 16385: 3600,
+                 16386: 7200, 16387: 10800, 16388: 14400, 16390: 21600, 16392: 28800, 16396: 43200, 16408: 86400,
+                 32769: 604800, 49153: 2592000}
         return times[self]
 
+    @classmethod
+    def get(cls, time):
+        times = {60: 1, 120: 2, 180: 3, 240: 4, 300: 5, 360: 6, 600: 10, 900: 15, 1200: 20, 1800: 30, 3600: 16385,
+                 7200: 16386, 10800: 16387, 14400: 16388, 21600: 16390, 28800: 16392, 43200: 16396, 86400: 16408,
+                 604800: 32769, 2592000: 49153}
+        return TimeFrame(times[int(time)])
+
 
 class CopyTicks(Repr, IntEnum):
     """
     COPY_TICKS defines the types of ticks that can be requested using the copy_ticks_from() and copy_ticks_range() functions.
     Attributes:
         ALL (int): All ticks
```

### Comparing `aiomql-1/src/aiomql/core/models.py` & `aiomql-2.0/src/aiomql/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import MetaTrader5 as mt5
 
 from .constants import BookType, TradeAction, OrderType, OrderTime, OrderFilling, PositionType, PositionReason, DealType, DealEntry, DealReason, \
     SymbolChartMode, SymbolTradeMode, SymbolCalcMode, SymbolOptionMode, SymbolOrderGTCMode, SymbolOptionRight, SymbolTradeExecution, SymbolSwapMode, \
-    DayOfWeek, ErrorCode, AccountTradeMode, AccountStopoutMode, AccountMarginMode
+    DayOfWeek, ErrorCode, AccountTradeMode, AccountStopoutMode, AccountMarginMode, OrderReason
 
 from . import Base
 
 """
-This module hold data structures used in this library
+This module contains data models used in this library.
+They are used as base classes to other classes having the same properties but with more methods.
 """
 
 
 class AccountInfo(Base):
     """
     Information about account.
 
     Attributes:
-        account_number: int
+        login: int
         password: str
         server: str
         trade_mode: AccountTradeMode
         balance: float
         leverage: float
         profit: float
         point: float
@@ -44,17 +45,17 @@
         currency_digits: int
         assets: float
         liabilities: float
         commission_blocked: float
         name: str
         company: str
     """
-    account_number: int
-    password: str
-    server: str
+    login: int = 0
+    password: str = ''
+    server: str = ''
     trade_mode: AccountTradeMode
     balance: float
     leverage: float
     profit: float
     point: float
     amount: float = 0
     equity: float
@@ -329,84 +330,105 @@
     exchange: str
     formula: str
     isin: str
     name: str
     page: str
     path: str
 
+    def __init__(self, **kwargs):
+        if 'name' not in kwargs:
+            raise AttributeError('Symbol Object Must be initialized with a name')
+        self.name = kwargs.pop('name')
+        super().__init__(**kwargs)
+
+    def __repr__(self):
+        return self.name
+
+    def __str__(self):
+        return self.name
+
+    def __eq__(self, other: "SymbolInfo"):
+        return self.name == other.name
+
+    def __hash__(self):
+        return hash(self.name)
+
 
 class BookInfo(Base):
-    """
-    Book Info
+    """Book Info
 
     Attributes:
         type: BookType
         price: float
         volume: float
         volume_dbl: float
     """
     type: BookType
     price: float
     volume: float
     volume_dbl: float
 
 
 class TradeOrder(Base):
-    """
-    Trade Order
+    """Trade Order
 
     Attributes:
         ticket: int
         time_setup: int
         time_setup_msc: int
         time_expiration: int
-        type: int
-        type_time: int
-        type_filling: int
+        time_done: int
+        time_done_msc: int
+        type: OrderType
+        type_time: OrderTime
+        type_filling: OrderFilling
         state: int
         magic: int
+        position_id: int
+        position_by_id: int
+        reason: OrderReason
         volume_current: float
         volume_initial: float
         price_open: float
         sl: float
         tp: float
         price_current: float
-        price_open: float
-        price_stop_limit: float
-        position_id: int
-        position_by_id: int
-        reason: str
+        price_stoplimit: float
         symbol: str
+        comment: str
+        external_id: str
     """
     ticket: int
     time_setup: int
     time_setup_msc: int
     time_expiration: int
-    type: int
-    type_time: int
-    type_filling: int
+    time_done: int
+    time_done_msc: int
+    type: OrderType
+    type_time: OrderTime
+    type_filling: OrderFilling
     state: int
     magic: int
+    position_id: int
+    position_by_id: int
+    reason: OrderReason
     volume_current: float
     volume_initial: float
     price_open: float
     sl: float
     tp: float
     price_current: float
-    price_open: float
-    price_stop_limit: float
-    position_id: int
-    position_by_id: int
-    reason: str
+    price_stoplimit: float
     symbol: str
+    comment: str
+    external_id: str
 
 
 class TradeRequest(Base):
-    """
-    Trade Request
+    """Trade Request Class.
 
     Attributes:
         action: TradeAction
         type: OrderType
         order: int
         symbol: str
         volume: float
```

### Comparing `aiomql-1/src/aiomql/executor.py` & `aiomql-2.0/src/aiomql/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,67 @@
 import asyncio
-from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 from typing import Sequence
 
 from .strategy import Strategy
 from .symbol import Symbol
-from .config import Config
 
 
 class Executor:
-    """
-    Executor class for running multiple strategies and instruments concurrently.
+    """Executor class for running multiple strategies on multiple symbols concurrently.
 
     Attributes:
-        executor (ThreadPoolExecutor, ProcessPoolExecutor): Executor object.
+        executor (ThreadPoolExecutor): The executor object.
         workers (list): List of strategies.
 
     """
     def __init__(self):
-        self.config = Config()
-        self.executor = ThreadPoolExecutor if self.config.executor == 'thread' else ProcessPoolExecutor
+        self.executor = ThreadPoolExecutor
         self.workers: list[type(Strategy)] = []
 
     def add_workers(self, strategies: Sequence[type(Strategy)]):
-        """
-        Add multiple strategies at once
+        """Add multiple strategies at once
 
         Args:
             strategies (Sequence[Strategy]): A sequence of strategies.
-
-        Returns:
         """
         self.workers.extend(strategies)
 
     def remove_workers(self, *symbols: Sequence[Symbol]):
+        """Removes any worker running on a symbol not successfully initialized.
+        
+        Args:
+            *symbols: Successfully initialized symbols.
         """
-        Remove worker if the symbol of the strategy did not initialize successfully
-        Returns:
-        """
-        for strategy in self.workers:
-            if strategy.symbol not in symbols:
-                self.workers.remove(strategy)
+        self.workers = [worker for worker in self.workers if worker.symbol in symbols]
 
     def add_worker(self, strategy: type(Strategy)):
-        """
-        Add a strategy object to the list of workers
+        """Add a strategy instance to the list of workers
+
         Args:
             strategy (Strategy): A strategy object
-
-        Returns:
-
         """
         self.workers.append(strategy)
 
     @staticmethod
     def run(strategy: type(Strategy)):
-        """
-        Wrap the coroutine in asyncio.run for each thread.
+        """Wraps the coroutine trade method of each strategy with 'asyncio.run'.
+
         Args:
             strategy (Strategy): A strategy object
-
-        Returns:
-
         """
         asyncio.run(strategy.trade())
 
-    def execute(self, workers: int = 0):
-        """
-        Add workers to pool executors.
+    async def execute(self, workers: int = 0):
+        """Run the strategies with a threadpool executor.
 
         Args:
-            workers: Number of workers to use in executor pool. Defaults to zero
-
-        Returns:
+            workers: Number of workers to use in executor pool. Defaults to zero which uses all workers.
 
+        Notes:
+            No matter the number specified, the executor will always use a minimum of 5 workers.
         """
         workers = workers or len(self.workers)
+        workers = max(workers, 5)
+        loop = asyncio.get_running_loop()
         with self.executor(max_workers=workers) as executor:
-            executor.map(self.run, self.workers)
+            [loop.run_in_executor(executor, self.run, worker) for worker in self.workers]
```

### Comparing `aiomql-1/src/aiomql/history.py` & `aiomql-2.0/src/aiomql/history.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,68 @@
 import asyncio
 from datetime import datetime
+from logging import getLogger
 
-from .config import Config
+from .core.config import Config
 
 from .core.meta_trader import MetaTrader
 from .core.models import TradeDeal, TradeOrder
-from .terminal import terminal
+
+logger = getLogger()
 
 
 class History:
-    """
-    The history class handles trade deals and trade orders in the trading history.
+    """The history class handles completed trade deals and trade orders in the trading history of an account.
 
     Args:
-        mt5 (MetaTrader): The Meta trader object for connecting to the terminal. Default Keyword Argument.
-
-
-        date_from (datetime, float): Date the orders are requested from. Set by the 'datetime' object or as a number of seconds elapsed since
-            1970.01.01. Defaults to the current time in "utc"
-
-
-        date_to (datetime, float): Date, up to which the orders are requested. Set by the 'datetime' object or as a number of
-            seconds elapsed since 1970.01.01. Defaults to the current time in "utc"
+        date_from (datetime, float): Date the orders are requested from. Set by the 'datetime' object or as a
+        number of seconds elapsed since 1970.01.01. Defaults to the current time in "utc"
 
+        date_to (datetime, float): Date up to which the orders are requested. Set by the 'datetime' object or as a number of
+        seconds elapsed since 1970.01.01. Defaults to the current time in "utc"
 
         group (str): Filter for selecting history by symbols.
 
-
         ticket (int): Filter for selecting history by ticket number
 
-
         position (int): Filter for selecting history deals by position
 
     Attributes:
-        deals (Iterable[TradeDeal]): Iterable of trade deals
-        orders (Iterable[TradeOrder]): Iterable of trade orders
+        deals (list[TradeDeal]): Iterable of trade deals
+        orders (list[TradeOrder]): Iterable of trade orders
         total_deals: Total number of deals
         total_orders (int): Total number orders
         group (str): Filter for selecting history by symbols.
         ticket (int): Filter for selecting history by ticket number
         position (int): Filter for selecting history deals by position
         initialized (bool): check if initial request has been sent to the terminal to get history.
+        mt5 (MetaTrader): MetaTrader instance
+        config (Config): Config instance
     """
-    deals: list[TradeDeal] = []
-    orders: list[TradeOrder] = []
-    total_deals: int = 0
-    total_orders: int = 0
+    mt5: MetaTrader = MetaTrader()
+    config: Config = Config()
 
-    def __init__(self, *, mt5=MetaTrader(), date_from: datetime | float = datetime.utcnow(), date_to: datetime | float = datetime.utcnow(),
+    def __init__(self, *, date_from: datetime | float = 0, date_to: datetime | float = 0,
                  group: str = "", ticket: int = 0, position: int = 0):
-        self.config = Config()
-        self.mt5 = mt5
-        self.date_from = date_from
-        self.date_to = date_to
+        now = datetime.utcnow()
+        self.date_from = date_from or now
+        self.date_to = date_to or now
         self.group = group
         self.ticket = ticket
         self.position = position
+        self.deals: list[TradeDeal] = []
+        self.orders: list[TradeOrder] = []
+        self.total_deals: int = 0
+        self.total_orders: int = 0
         self.initialized = False
 
     async def init(self, deals=True, orders=True) -> bool:
         """
         Get history deals and orders
+
         Keyword Args:
             deals (bool): If true get history deals during initial request to terminal
             orders (bool): If true get history orders during initial request to terminal
 
         Returns:
             bool: True if all requests were successful else False
 
@@ -73,48 +71,58 @@
         tasks.append(self.get_deals()) if deals else ...
         tasks.append(self.get_orders()) if orders else ...
         res = await asyncio.gather(*tasks)
         self.initialized = all(res)
         return self.initialized
 
     async def get_deals(self) -> list[TradeDeal]:
-        """
-        Get trade deals
-        Returns:
-            list[TradeDeal]: Iterable of trade deals
+        """Get deals from trading history using the parameters set in the constructor.
 
+        Returns:
+            list[TradeDeal]: A list of trade deals
         """
         deals = await self.mt5.history_deals_get(date_from=self.date_from, date_to=self.date_to, group=self.group, ticket=self.ticket,
                                                  position=self.position)
+        if deals is not None:
+            self.deals = [TradeDeal(**deal._asdict()) for deal in deals] if deals else []
+            self.total_deals = len(self.deals)
+            return self.deals
 
-        self.deals = [TradeDeal(**deal._asdict()) for deal in deals] if deals else []
-        self.total_deals = len(self.deals)
+        err = await self.mt5.last_error()
+        logger.warning(err)
         return self.deals
 
     async def deals_total(self) -> int:
-        """
-        Get total number of deals
-        Returns (int): Number of Deals
+        """Get total number of deals within the specified period in the constructor.
+
+        Returns:
+            (int): Total number of Deals
         """
         self.total_deals = await self.mt5.history_deals_total(self.date_from, self.date_to)
         return self.total_deals
 
     async def get_orders(self) -> list[TradeOrder]:
-        """
-        Get trade orders
+        """Get orders from trading history using the parameters set in the constructor.
+
         Returns:
-            list[TradeOrder]): Iterable of trade orders
+            list[TradeOrder]): A list of trade orders
         """
 
-        orders = await self.mt5.history_orders_get(date_from=self.date_from, date_to=self.date_to, group=self.group, ticket=self.ticket,
-                                                   position=self.position)
-        self.orders = [TradeOrder(**order._asdict()) for order in orders] if orders else []
+        orders = await self.mt5.history_orders_get(date_from=self.date_from, date_to=self.date_to, group=self.group,
+                                                   ticket=self.ticket, position=self.position)
+        if orders is None:
+            err = await self.mt5.last_error()
+            logger.warning(err)
+            return self.orders
+
+        self.orders = [TradeOrder(**order._asdict()) for order in orders]
         self.total_orders = len(self.orders)
         return self.orders
 
     async def orders_total(self) -> int:
-        """
-        Get total number of orders
-        Returns (int): Number of orders
+        """Get total number of orders within the specified period in the constructor.
+
+        Returns:
+            (int):Total number of orders
         """
         self.total_orders = await self.mt5.history_orders_total(self.date_from, self.date_to)
         return self.total_orders
```

### Comparing `aiomql-1/src/aiomql/lib/traders/simple_deal_trader.py` & `aiomql-2.0/src/aiomql/lib/traders/simple_deal_trader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 import logging
+from datetime import datetime
 
 from ...utils import dict_to_string
-from ...result import TradeResult
-from ...symbol import Symbol
 from ...trader import Trader
 from ...core.constants import OrderType
 
-from ..symbols import ForexSymbol, SyntheticSymbol
+from .trade_result import TradeResult
 
 logger = logging.getLogger()
 
 
 class DealTrader(Trader):
-
-    def __init__(self, *, symbol: ForexSymbol | SyntheticSymbol):
-        super().__init__(symbol=symbol)
+    """A base class for placing trades based on the number of pips to target"""
 
     async def create_order(self, order: OrderType, points: float):
-        """
-        Using the amount of points i.e pips/10 determine the volume, stop_loss and take_profit.
-        Use equity and risk value on account to determine amount
+        """Using the number of target points determines the lot size, stop loss and take profit for the order,
+        and updates the order object with the values.
+
         Args:
             order (OrderType): Type of order
-            points (float): Number of points
-
-        Returns:
-
+            points (float): Number of points to target
         """
         await self.account.refresh()
-        amount = self.account.equity * self.account.risk
-        sl, tp, volume = await self.symbol.get_sl_tp_volume(amount=amount, risk_to_reward=self.account.risk_to_reward, points=points)
+        amount = self.account.margin_free * self.account.risk
+        sl, tp, volume = await self.symbol.get_sl_tp_volume(amount=amount, risk_to_reward=self.account.risk_to_reward,
+                                                            points=points)
         self.order.volume = volume
         self.order.type = order
         await self.set_order_limits(sl, tp)
 
-    async def set_order_limits(self, sl, tp):
+    async def set_order_limits(self, sl: float, tp: float):
+        """Sets the stop loss and take profit for the order.
+
+        Args:
+            sl (float): Stop loss
+            tp (float): Take profit
+        """
         tick = await self.symbol.info_tick()
         if self.order.type == OrderType.BUY:
             self.order.sl, self.order.tp = tick.ask - sl, tick.ask + tp
             self.order.price = tick.ask
         else:
             self.order.sl, self.order.tp = tick.bid + sl, tick.bid - tp
             self.order.price = tick.bid
 
-    async def place_trade(self, order: OrderType, points: float, params: dict = None):
+    async def place_trade(self, order: OrderType, points: float, params):
+        """Places a trade based on the number of points to target. The order is created, checked and sent.
+        """
         try:
-            params = params or {}
             await self.create_order(order=order, points=points)
-
             check = await self.order.check()
             if check.retcode != 0:
-                logger.warning(f"Comment: {check.comment}\tParameters: {dict_to_string(params)}\tsymbol: {self.order.symbol}")
+                logger.warning(f"Symbol: {self.order.symbol}\nResult:\n{dict_to_string(check.get_dict(include={'comment', 'retcode'}), multi=True)}")
                 return
 
             result = await self.order.send()
             if result.retcode != 10009:
-                logger.warning(f"Comment: {result.comment}\tParameters: {dict_to_string(params)}\tsymbol: {self.order.symbol}")
+                logger.warning(f"Symbol: {self.order.symbol}\nResult:\n{dict_to_string(result.get_dict(include={'comment', 'retcode'}), multi=True)}")
                 return
 
-            logger.info(f"{result.comment}\tparameters: {dict_to_string(params)}\tsymbol: {self.order.symbol}")
+            params['date'] = (date := datetime.utcnow())
+            params['time'] = date.timestamp()
+            logger.info(f"Symbol: {self.order.symbol}\nOrder: {dict_to_string(result.dict, multi=True)}\n")
             self.order.set_attributes(**result.get_dict(include={'price', 'volume'}))
             result.profit = await self.order.calc_profit()
-            TradeResult(parameters=params, request=self.order, result=result)
+            await TradeResult(result=result, parameters=params).save()
             return
+
         except Exception as err:
-            logger.error(f"{err}\tparameters: {dict_to_string(params)}\tsymbol: {self.order.symbol}")
+            logger.error(f"{err}. Symbol: {self.order.symbol}\n {self.__class__.__name__}.place_trade")
```

### Comparing `aiomql-1/src/aiomql/order.py` & `aiomql-2.0/src/aiomql/order.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,97 @@
-from .core.meta_trader import MetaTrader
+from logging import getLogger
+
 from .core.models import TradeRequest, OrderSendResult, OrderCheckResult, TradeOrder
 from .core.constants import TradeAction, OrderTime, OrderFilling
 
+logger = getLogger()
+
 
 class Order(TradeRequest):
-    """
-    Trade order related functions and properties. Subclass of TradeRequest.
+    """Trade order related functions and properties. Subclass of TradeRequest.
+    An order class must always be initialized with a symbol.
 
     Keyword Args:
-        mt5 (MetaTrader): The Meta trader object for connecting to the terminal. Default Keyword Argument
         kwargs: Arguments for initializing the order object
 
     Attributes:
         action (TradeAction): Trading operation type from TradeAction Enum
 
         type_time (OrderTime):  Order type by expiration from OrderTime
 
         type_filling (OrderFilling): Order filling type from OrderFilling Enum
-
-    Notes:
-        Other order properties are defined in the TradeRequest Object
     """
-    action: TradeAction = TradeAction.DEAL
-    type_time: OrderTime = OrderTime.SPECIFIED_DAY
-    type_filling: OrderFilling = OrderFilling.FOK
-    total: int = 0
-    orders: list[TradeOrder]
 
-    def __init__(self, mt5=MetaTrader(), **kwargs):
-        self.mt5 = mt5
+    def __init__(self, **kwargs):
+        if 'symbol' not in kwargs:
+            raise ValueError('symbol is required')
+        self.symbol = kwargs.pop('symbol')
+        self.action = kwargs.get('action', None) or TradeAction.DEAL
+        self.type_time = kwargs.get('type_time', None) or OrderTime.GTC
+        self.type_filling = kwargs.get('type_filling', None) or OrderFilling.FOK
         super().__init__(**kwargs)
 
+    @property
     async def orders_total(self):
-        """
-        Get the number of active orders. Update the total property
+        """Get the number of active orders.
 
         Returns:
-            int: Number of active orders
+            (int): total number of active orders
         """
-        self.total = await self.mt5.orders_total()
-        return self.total
-
-    async def orders_get(self, *, symbol="", group="", ticket=0):
-        """
-        Get active orders with the ability to filter by symbol or ticket. There are three call options.
-        Call without parameters. Return active orders on all symbols
+        return await self.mt5.orders_total()
 
+    @property
+    async def orders(self) -> tuple[TradeOrder]:
+        """Get active orders with the ability to filter by symbol or ticket.
         Keyword Args:
-            symbol (str): Symbol name. Optional named parameter. If a symbol is specified, the ticket parameter is ignored.
-
-            group (str): The filter for arranging a group of necessary symbols. Optional named parameter. If the group is specified, the function
-                returns only active orders meeting a specified criteria for a symbol name.
-
-            ticket (int): Order ticket (ORDER_TICKET). Optional named parameter.
+            ticket (int): Order ticket. Optional named parameter. If ticket=0, then all orders are returned using symbol as filter.
 
         Returns:
             list[TradeOrder]: A list of active trade orders as TradeOrder objects
-
         """
-        orders = await self.mt5.orders_get(group=group, ticket=ticket, symbol=symbol)
-        self.orders = [TradeOrder(**order._asdict()) for order in orders]
-        return self.orders
+        orders = await self.mt5.orders_get(symbol=self.symbol)
+        orders = (TradeOrder(**order._asdict()) for order in orders)
+        return tuple(orders)
 
     async def check(self) -> OrderCheckResult:
-        """
-        Check funds sufficiency for performing a required trading operation
+        """Check funds sufficiency for performing a required trading operation
 
         Returns:
             (OrderCheckResult): Returns OrderCheckResult object
         """
         res = await self.mt5.order_check(self.dict)
         return OrderCheckResult(**res._asdict())
 
     async def send(self) -> OrderSendResult:
-        """
-        Send a request to perform a trading operation from the terminal to the trade server.
+        """Send a request to perform a trading operation from the terminal to the trade server.
 
         Returns:
              OrderSendResult: Returns OrderSendResult object
         """
         res = await self.mt5.order_send(self.dict)
         return OrderSendResult(**res._asdict())
 
-    async def calc_margin(self) -> float | None:
-        """
-        Return margin in the account currency to perform a specified trading operation.
+    async def calc_margin(self) -> float:
+        """Return the required margin in the account currency to perform a specified trading operation.
 
         Returns:
             float: Returns float value if successful
-            None: If not successful
-        """
-        return await self.mt5.order_calc_margin(self.type, self.symbol, self.volume, self.price)
 
-    async def calc_profit(self) -> float | None:
+        Raises:
+            ValueError: If not successful
         """
-        Return profit in the account currency for a specified trading operation.
+        res = await self.mt5.order_calc_margin(self.type, self.symbol, self.volume, self.price)
+        raise ValueError(f'Failed to calculate margin for {self.symbol} {self.type} {self.volume} {self.price} {res}')
+
+    async def calc_profit(self) -> float:
+        """Return profit in the account currency for a specified trading operation.
+
         Returns:
             float: Returns float value if successful
-            None: If not successful
+
+        Raises:
+            ValueError: If not successful
         """
-        return await self.mt5.order_calc_profit(self.type, self.symbol, self.volume, self.price, self.tp)
+        res = await self.mt5.order_calc_profit(self.type, self.symbol, self.volume, self.price, self.tp)
+        if res is not None:
+            return res
+        raise ValueError(f'Failed to calculate profit for {self.symbol} {self.type} {self.volume} {self.price} {self.tp}')
```

### Comparing `aiomql-1/src/aiomql/positions.py` & `aiomql-2.0/src/aiomql/positions.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,67 +7,61 @@
 
 
 class Positions:
     """
     Hold open positions related properties and objects
 
     Keyword Args:
-        mt5 (MetaTrader): The Meta trader object for connecting to the terminal. Default Keyword Argument
         symbol (str): Financial instrument name
         group (str): The filter for arranging a group of necessary symbols. Optional named parameter. If the group is specified, the function returns
                      only positions meeting a specified criteria for a symbol name.
         ticket (int): Position ticket
 
     Attributes:
         symbol (str): Financial instrument name
 
         group (str): The filter for arranging a group of necessary symbols. Optional named parameter. If the group is specified, the function returns
                      only positions meeting a specified criteria for a symbol name.
 
         ticket (int): Position ticket
-
-        positions (list[TradePosition]): A list of trade positions
-
-        total_positions (int):
     """
-    def __init__(self, *, symbol: str = "", group: str = "", ticket: int = 0, mt5=MetaTrader()):
-        self.mt5 = mt5
+    mt5: MetaTrader = MetaTrader()
+    
+    def __init__(self, *, symbol: str = "", group: str = "", ticket: int = 0):
         self.symbol = symbol
         self.group = group
         self.ticket = ticket
-        self.total_positions: int = 0
-        self.positions: list[TradePosition] = []
 
+    @property
     async def positions_total(self) -> int:
+        """Get the number of open positions.
+        
+        Returns:
+            int: Return total number of open positions
         """
-        Get open positions with the ability to filter by symbol or ticket.
-        Returns (int): Return integer value
-
-        """
-        self.total_positions = await self.mt5.positions_total()
-        return self.total_positions
+        return await self.mt5.positions_total()
 
+    @property
     async def positions_get(self):
         """
         Get open positions with the ability to filter by symbol or ticket.
+        
         Returns:
             list[TradePosition]: A list of open trade positions
 
         """
         positions = await self.mt5.positions_get(group=self.group, symbol=self.symbol, ticket=self.ticket)
-        self.positions = [TradePosition(**pos._asdict()) for pos in positions]
-        return self.positions
+        return [TradePosition(**pos._asdict()) for pos in positions]
 
     async def close_all(self) -> int:
+        """Close all open positions for the trading account.
+        
+        Returns (int): Return number of positions closed.
         """
-        Close all open positions
-        Returns (int): Return number of open positions
-
-        """
-        orders = [Order(mt5=self.mt5, action=TradeAction.DEAL, price=pos.price_current, position=pos.ticket,
+        orders = [Order(action=TradeAction.DEAL, price=pos.price_current, position=pos.ticket,
                         type=OrderType(pos.type).opposite,
                         **pos.get_dict(include={'symbol', 'volume'})) for pos in (await self.positions_get())]
 
         results = await asyncio.gather(*[order.send() for order in orders])
         amount_closed = len([res for res in results if res.retcode == 10009])
         await self.positions_total()
         return amount_closed
```

### Comparing `aiomql-1/src/aiomql/records.py` & `aiomql-2.0/src/aiomql/records.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,81 @@
 import asyncio
 from datetime import datetime
-from typing import Iterable
 from pathlib import Path
 import csv
 
 from .history import History
-from .config import Config
+from .core.config import Config
 
 
 class Records:
-    """
-    This utility class read trade records from csv files, and update them based on their closing positions
+    """This utility class read trade records from csv files, and update them based on their closing positions
 
     Keyword Args:
         records_dir (Path): Path to directory containing record of placed trades.
 
     Attributes:
         config: Config object
-
         records_dir(Path): Path to directory containing record of placed trades, If not given takes the default from the config
     """
-
-    def __init__(self, records_dir: Path = None):
-        self.config = Config()
+    config: Config = Config()
+    
+    def __init__(self, records_dir: Path = ''):
         self.records_dir = records_dir or self.config.records_dir
 
     async def get_records(self):
-        """
-        get trade records from records_dir folder
-        Returns:
+        """Get trade records from records_dir folder
 
+        Yields:
+            files: Trade record files
         """
         for file in self.records_dir.iterdir():
             if file.is_file() and file.name.endswith('.csv'):
                 yield file
 
-    async def read_record(self, file: Path):
-        """
-        Read and update trade records
+    async def read_update(self, file: Path):
+        """Read and update trade records
 
         Args:
             file: Trade record file
-
-        Returns:
-
         """
-        with open(file, newline='') as fr:
-            reader = csv.DictReader(fr)
-            rows = (row for row in reader)
-            rows = await self.update_record(rows)
-            fr.close()
-            if not all(rows):
-                return
-            fw = open(file, newline='', mode='w')
-            writer = csv.DictWriter(fw, fieldnames=list(rows[0].keys()))
-            writer.writeheader()
-            writer.writerows(rows)
-            fw.close()
+        fr = open(file, mode='r', newline='')
+        reader = csv.DictReader(fr)
+        rows = [row for row in reader]
+        rows = await self.update_rows(rows)
+        fr.close()
+        fw = open(file, mode='w', newline='')
+        writer = csv.DictWriter(fw, fieldnames=reader.fieldnames)
+        writer.writeheader()
+        writer.writerows(rows)
+        fw.close()
 
-    async def update_record(self, rows: Iterable) -> Iterable[dict]:
-        """
-        Get update of trades in the record file.
-        Args:
-            rows: rows of recorded trade in a particular file
-
-        Returns: return rows of updated trades as an iterable of dicts
+    async def update_rows(self, rows: list[dict]) -> list[dict]:
+        """Update the rows of entered trades in the csv file with the actual profit.
 
-        """
-        rows = {row['deal']: row for row in sorted((row for row in rows), key=lambda row: float(row['time']))}
-        open_rows = [(key, value) for key, value in rows.items() if value.get('closed').title() == "False"]
-        if len(open_rows) == 0:
-            return [{}]
-
-        start, end = datetime.fromtimestamp(float(open_rows[0][1]['time'])).replace(hour=0, minute=0, second=0), datetime.now()\
-            .replace(hour=23, minute=59, second=59)
-
-        history = History(date_from=start, date_to=end)
-        await history.init(orders=False)
-        deals = {str(deal.position_id): deal.profit for deal in history.deals}
-
-        for el in open_rows:
-            row = el[1]
-            if row['order'] not in deals:
-                continue
-            profit = float(row['profit'])
-            actual_profit = deals[row['order']]
-            win = actual_profit / profit > self.config.win_percentage
-            row.update(actual_profit=actual_profit, closed=True, win=win)
-        return list(rows.values())
+        Args:
+            rows: A list of dictionaries from the dictionary writer object of the csv file.
 
-    async def update_trade_records(self):
-        """
-        Update trade records
         Returns:
+            list[dict]: A list of dictionaries with the actual profit and win status.
         """
-        records = [self.read_record(record) async for record in self.get_records()]
-        await asyncio.gather(*records)
+        start = float(min(rows, key=lambda r: r['time'])['time'])
+        end = datetime.utcnow().timestamp()
+        his = History(date_from=start, date_to=end)
+        await his.init(orders=False)
+        deals = {str(deal.position_id): deal.profit for deal in his.deals}
+        for row in rows:
+            if (deal := row['order']) in deals:
+                profit = deals[deal]
+                row.update(actual_profit=profit, win=profit > 0)
+        return rows
 
-    async def update_trade_record(self, file: Path | str):
+    async def update_records(self):
+        """Update trade records in the records_dir folder
         """
+        records = [self.read_update(record) async for record in self.get_records()]
+        await asyncio.gather(*records)
 
-        Returns:
-
+    async def update_record(self, file: Path | str):
+        """Update a single trade record file.
         """
-        await self.read_record(file)
+        await self.read_update(file)
```

### Comparing `aiomql-1/src/aiomql/strategy.py` & `aiomql-2.0/src/aiomql/strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,86 @@
 import asyncio
 import time
-from dataclasses import dataclass
-from typing import Literal, Type
+from typing import Type, TypeVar
 from abc import ABC, abstractmethod
 
 import pandas_ta as ta
-from pandas import DataFrame
 
-from .core.constants import TimeFrame, OrderType
+from .core.meta_trader import MetaTrader
+from .core.constants import TimeFrame
 from .candle import Candles, Candle
-from .symbol import Symbol
+from .symbol import Symbol as _Symbol
+from .account import Account
+from .core.config import Config
 
-
-@dataclass
-class Entry:
-    """
-    A helper class for capturing entry positions.
-
-    Attributes:
-        time (float): Time of the bar
-
-        trend (str): The trend of the chart. Can be either of "notrend", "uptrend", "downtrend".
-
-        new (bool): Shows if an entry position has been seen before.
-
-        type (OrderType): OrderType for placing trade order
-
-        points (float): points to trade.
-    """
-    time: float = 0
-    trend: Literal["notrend", "uptrend", "downtrend"] = "notrend"
-    current: float = 0
-    new: bool = True
-    type: OrderType | None = None
-    points: float = 0
+Symbol = TypeVar('Symbol', bound=_Symbol)
 
 
 class Strategy(ABC):
-    """
-    The base class for creating strategies.
+    """The base class for creating strategies.
 
     Keyword Args:
         symbol (Symbol): The Financial Instrument as a Symbol Object
-        **kwargs: Optional Keyword Arguments
+        params (dict): Configurable parameters for running the strategy
 
     Attributes:
-        Candle (Type[Candle]): Can be a subclass of the Candle class specific to the strategy and analysis carried out on it.
-
-        Candles (Type[Candles]): Candles class for the strategy can be the same or a subclass of the "candle.Candles" class.
-
-        name (str): A name for the strategy. You can initialize a new name for the strategy that will replace the one defined as class parameter
+        candle_class (Type[Candle]): Can be a subclass of the Candle class specific to the strategy and analysis carried out on it.
+        candles_class (Type[Candles]): Candles class for the strategy can be the same or a subclass of the "candle.Candles" class.
+        name (str): A name for the strategy.
+        symbol (Symbol): The Financial Instrument as a Symbol Object
+        mt5 (MetaTrader): MetaTrader instance.
+        config (Config): Config instance.
+        account (Account): Account instance.
+
+    Notes:
+        If you want to use a subclass of the Candle class, you must set the candle_class attribute to the subclass.
+        The same applies to the Candles class.
     """
-    Candle: Type[Candle] = Candle
-    Candles: Type[Candles] = Candles
+    candle_class: Type[Candle] = Candle
+    candles_class: Type[Candles] = Candles
     name:  str = ""
+    account = Account()
+    mt5: MetaTrader()
+    config = Config()
 
-    def __init__(self, *, symbol: type(Symbol), **kwargs):
+    def __init__(self, *, symbol: Symbol, params: dict = None):
         self.symbol = symbol
-        self.name = kwargs.get('name') or self.name
+        self.parameters = params or {}
+        self.parameters['symbol'] = symbol.name
 
     def __repr__(self):
         return f"{self.name}({self.symbol!r})"
 
     async def get_ema(self, *, time_frame: TimeFrame, period: int, count: int = 500) -> type(Candles):
-        """
-        Helper method that gets the ema of the bars.
+        """Helper method that gets the ema of the bars.
 
         Keyword Args:
             time_frame (TimeFrame): Timeframe of the bars returned
-
             period (int): Period of the ema
-
             count (int): Number of objects to be returned
 
-        Returns: A Candles Object
+        Returns:
+            Candles: A Candles Object
         """
-        data: DataFrame = await self.symbol.copy_rates_from_pos(timeframe=time_frame, count=count)
+        data = await self.symbol.copy_rates_from_pos(timeframe=time_frame, count=count)
         await asyncio.to_thread(data.ta.ema, length=period, append=True)
         data.rename(columns={f"EMA_{period}": 'ema'}, inplace=True)
-        return self.Candles(data=data, candle=self.Candle)
+        return self.candles_class(data=data)
 
     @staticmethod
     async def sleep(secs: float):
-        """
-        Sleep for the needed amount of seconds between requests to the terminal
-        Args:
-            secs (float): The time period of the requests, eg. when trading on the 5 minute time frame the value will be 300 secs
-
-        Returns: None.
+        """Sleep for the needed amount of seconds in between requests to the terminal.
+        computes the accurate amount of time needed to sleep ensuring that the next request is made at the start of
+        a new bar and making cooperative multitasking possible.
 
+        Args:
+            secs (float): The time in seconds. Usually the timeframe of the chart you trading with.
         """
-        await asyncio.sleep(secs - (time.time() % secs) + 1)
+        mod = time.time() % secs
+        secs = secs - mod if mod != 0 else mod
+        await asyncio.sleep(secs + 0.1)
 
     @abstractmethod
     async def trade(self):
-        """
-        Place trades using this method
-        Returns:
-
+        """Place trades using this method. This is the main method of the strategy.
+        It will be called by the strategy runner.
         """
```

### Comparing `aiomql-1/src/aiomql/symbol.py` & `aiomql-2.0/src/aiomql/symbol.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,206 +1,274 @@
 from datetime import datetime
+from logging import getLogger
 
 from pandas import DataFrame
 
-from .core.meta_trader import MetaTrader
 from .core.constants import TimeFrame, CopyTicks
-from .core.models import SymbolInfo
+from .core.models import SymbolInfo, BookInfo
 from .ticks import Tick
+from .account import Account
 
-from .terminal import terminal
+logger = getLogger()
 
 
 class Symbol(SymbolInfo):
-    """
-    Helper class with general properties and methods of a financial instrument.
-    You can inherit from this class and add your own properties and methods.
-    This class subclass of SymbolInfo which contains all symbol properties.
-    All methods of this class accept keyword only arguments.
-
-    Keyword Args:
-        mt5: Platform, defaults to the MetaTrader5 class.
+    """Main class for handling a financial instrument. A subclass of SymbolInfo and Base it have properties and methods
+    for working with a financial instrument.
 
     Attributes:
         tick (Tick): Price tick object for instrument
+        account: An instance of the current trading account
 
     Notes:
         Full properties are on the SymbolInfo Object.
         Make sure Symbol is always initialized with a name argument
     """
     tick: Tick
-
-    def __init__(self, *, mt5=MetaTrader(), **kwargs):
-        self.mt5 = mt5
-
-        if "name" not in kwargs:
-            raise TypeError("Symbol must be initialized with a name attribute")
-
-        self.name = kwargs['name']
-        del kwargs['name']
-        super().__init__(**kwargs)
-
-    def __repr__(self):
-        return f"{self.name}"
-
-    def __eq__(self, other: "Symbol"):
-        return self.name == other.name
-
-    def __lt__(self, other: "Symbol"):
-        return self.name > other.name
-
-    def __hash__(self):
-        return hash(self.name)
+    account = Account()
 
     async def info_tick(self, *, name: str = "") -> Tick:
-        """
-        Get Price Tick of the financial instrument
+        """Get the current price tick of a financial instrument.
 
         Args:
             name: if name is supplied get price tick of that financial instrument
 
         Returns:
-            Tick: Returns a Custom Tick Object
+            Tick: Return a Tick Object
+
+        Raises:
+            ValueError: If request was unsuccessful and None was returned
         """
-        _name = name if name else self.name
-        tick = await self.mt5.symbol_info_tick(_name)
+        tick = await self.mt5.symbol_info_tick(name or self.name)
+        if tick is None:
+            raise ValueError(f'Could not get tick for {name or self.name}')
         tick = Tick(**tick._asdict())
-        setattr(self, 'tick', tick) if _name == self.name else ...
+        setattr(self, 'tick', tick) if not name else ...
         return tick
 
     async def symbol_select(self, *, enable: bool = True) -> bool:
-        """
-        Select a symbol in the MarketWatch window or remove a symbol from the window.
+        """Select a symbol in the MarketWatch window or remove a symbol from the window.
         Update the select property
 
         Args:
-            enable (bool): Switch. Optional unnamed parameter. If 'false', a symbol should be removed from the MarketWatch window.
-                Otherwise, it should be selected in the MarketWatch window. A symbol cannot be removed if open charts with this symbol are currently
-                present or positions are opened on it.
+            enable (bool): Switch. Optional unnamed parameter. If 'false', a symbol should be removed from
+             the MarketWatch window.
 
         Returns:
             bool: True if successful, otherwise – False.
         """
         self.select = await self.mt5.symbol_select(self.name, enable)
         return self.select
 
-    async def info(self) -> SymbolInfo | None:
-        """
-        Get data on the specified financial instrument and update the symbol object properties
+    async def info(self) -> SymbolInfo:
+        """Get data on the specified financial instrument and update the symbol object properties
 
         Returns:
-            bool: True if successful else False
+            (SymbolInfo): SymbolInfo if successful
+
+        Raises:
+            ValueError: If request was unsuccessful and None was returned
         """
+        
         info = await self.mt5.symbol_info(self.name)
-        if not info:
-            return None
-        self.set_attributes(**info._asdict())
-        return SymbolInfo(**info._asdict())
+        if info:
+            self.set_attributes(**info._asdict())
+            return SymbolInfo(**info._asdict())
+        raise ValueError(f'Could not get info for {self.name}')
 
     async def init(self) -> bool:
-        """
-        Initialized the symbol by pulling properties from the terminal
+        """Initialized the symbol by pulling properties from the terminal
 
         Returns:
              bool: Returns True if symbol info was successful initialized
         """
-        await self.symbol_select()
-        if self.select:
-            await self.info()
-            return self.select
-        return self.select
+        try:
+            if await self.symbol_select():
+                await self.book_add()
+                await self.info()
+                return True
+            logger.warning(f'Unable to initialized symbol {self}')
+            return False
+        except Exception as err:
+            self.select = False
+            logger.warning(err)
+            return False
+
+    async def book_add(self) -> bool:
+        """Subscribes the MetaTrader 5 terminal to the Market Depth change events for a specified symbol.
+        If the symbol is not in the list of instruments for the market, This method will return False
+
+        Returns:
+             bool: True if successful, otherwise – False.
+        """
+        return await self.mt5.market_book_add(self.name)
+
+    async def book_get(self) -> tuple[BookInfo]:
+        """Returns a tuple of BookInfo featuring Market Depth entries for the specified symbol.
+
+        Returns:
+            tuple[BookInfo]: Returns the Market Depth contents as a tuples of BookInfo Objects
+
+        Raises:
+            ValueError: If request was unsuccessful and None was returned
+        """
+        infos = await self.mt5.market_book_get(self.name)
+        if infos is None:
+            raise ValueError(f'Could not get book info for {self.name}')
+        book_infos = (BookInfo(**info._asdict()) for info in infos)
+        return tuple(book_infos)
+
+    async def book_release(self) -> bool:
+        """Cancels subscription of the MetaTrader 5 terminal to the Market Depth change events for a specified symbol.
+        Args:
+            symbol: financial instrument name
+
+        Returns:
+            bool: True if successful, otherwise – False.
+        """
+        return await self.mt5.market_book_release(self.name)
+
+    async def currency_conversion(self, *, amount: float, base: str, quote: str) -> float:
+        """Convert from one currency to the other.
+
+        Args:
+            amount: amount to convert given in terms of the quote currency
+            base: The base currency of the pair
+            quote: The quote currency of the pair
+
+        Returns:
+            float: Amount in terms of the quote currency or None if it failed to convert
 
-    async def copy_rates_from(self, *, timeframe: TimeFrame, date_from: datetime | int, count: int) -> DataFrame | None:
+        Raises:
+            ValueError: If conversion is impossible
+        """
+
+        pair = f'{base}{quote}'
+        if self.account.has_symbol(pair):
+            tick = await self.info_tick(name=pair)
+            if tick is not None:
+                return amount / tick.ask
+
+        pair = f'{quote}{base}'
+        if self.account.has_symbol(pair):
+            tick = await self.info_tick(name=pair)
+            if tick is not None:
+                amount = amount * tick.bid
+                return amount
+        logger.warning(f'Currency conversion failed: Unable to convert {amount} in {quote} to {base}')
+
+        raise ValueError('Currency Conversion Failed')
+
+    async def copy_rates_from(self, *, timeframe: TimeFrame, date_from: datetime | int, count: int) -> DataFrame:
         """
         Get bars from the MetaTrader 5 terminal starting from the specified date.
 
         Args:
             timeframe (TimeFrame): Timeframe the bars are requested for. Set by a value from the TimeFrame enumeration. Required unnamed parameter.
 
             date_from (datetime | int): Date of opening of the first bar from the requested sample. Set by the 'datetime' object or as a number
                 of seconds elapsed since 1970.01.01. Required unnamed parameter.
 
             count (int): Number of bars to receive. Required unnamed parameter.
 
         Returns:
-            DateFrame: Rates as pandas DataFrame object
-            None: Return None if there is an error
+            DataFrame: Returns a Dataframe object as a collection of rates ordered chronologically
+
+        Raises:
+            ValueError: If request was unsuccessful and None was returned
         """
         rates = await self.mt5.copy_rates_from(self.name, timeframe, date_from, count)
-        return DataFrame(rates) if rates is not None else None
+        if rates is not None:
+            return DataFrame(data=rates)
+        raise ValueError(f'Could not get rates for {self.name}')
 
-    async def copy_rates_from_pos(self, *, timeframe: TimeFrame, count: int = 500, start_position: int = 0) -> DataFrame:
-        """
-        Get bars from the MetaTrader 5 terminal starting from the specified index.
+    async def copy_rates_from_pos(self, *,timeframe: TimeFrame, count: int = 500, start_position: int = 0) -> DataFrame:
+        """Get bars from the MetaTrader 5 terminal starting from the specified index.
 
         Args:
             timeframe (TimeFrame): TimeFrame value from TimeFrame Enum. Required keyword only parameter
 
             count (int): Number of bars to return. Keyword argument defaults to 500
 
-            start_position (int): Initial index of the bar the data are requested from. The numbering of bars goes from present to past.
-                Thus, the zero bar means the current one. Keyword argument defaults to 0.
+            start_position (int): Initial index of the bar the data are requested from. The numbering of bars goes from
+             present to past. Thus, the zero bar means the current one. Keyword argument defaults to 0.
 
         Returns:
-             DataFrame: Returns a Pandas DataFrame object of bars
-             None: Return None if there is an error
-        """
-        rates = await self.mt5.copy_rates_from_pos(self.name, timeframe, start_position, count)
-        return DataFrame(rates) if rates is not None else None
+             DataFrame: Returns a Dataframe object as a collection of rates ordered chronologically.
 
-    async def copy_ticks_from(self, *, date_from: datetime | int, count: int = 100, flags: CopyTicks = CopyTicks.INFO) -> DataFrame:
+        Raises:
+            ValueError: If request was unsuccessful and None was returned
         """
-        Get ticks from the MetaTrader 5 terminal starting from the specified date.
+        rates = await self.mt5.copy_rates_from_pos(self.name, timeframe, start_position, count)
+        if rates is not None:
+            return DataFrame(data=rates)
+        raise ValueError(f'Could not get rates for {self.name}')
+
+    async def copy_rates_range(self, *, timeframe: TimeFrame, date_from: datetime | int,
+                               date_to: datetime | int) -> DataFrame:
+        """Get bars in the specified date range from the MetaTrader 5 terminal.
 
         Args:
-            date_from (datetime | int): Date the ticks are requested from. Set by the 'datetime' object or as a number of seconds elapsed since 1970.01.01.
+            timeframe (TimeFrame): Timeframe for the bars using the TimeFrame enumeration. Required unnamed parameter.
 
-            count (int): Number of requested ticks. Defaults to 100
+            date_from (datetime | int): Date the bars are requested from. Set by the 'datetime' object or as a number of seconds
+                elapsed since 1970.01.01. Bars with the open time >= date_from are returned. Required unnamed parameter.
 
-            flags (CopyTicks): A flag to define the type of the requested ticks from CopyTicks enum. INFO is the default
+            date_to (datetime | int): Date, up to which the bars are requested. Set by the 'datetime' object or as a number of
+                seconds elapsed since 1970.01.01. Bars with the open time <= date_to are returned. Required unnamed parameter.
 
         Returns:
-             DataFrame: Returns a Pandas DataFrame object of ticks
-             None: Return None if there is an error
+           DataFrame: Returns a Dataframe object as a collection of rates ordered chronologically.
 
+        Raises:
+            ValueError: If request was unsuccessful and None was returned
         """
-        ticks = await self.mt5.copy_ticks_from(self.name, date_from, count, flags)
-        return DataFrame(ticks) if ticks is not None else None
+        rates = await self.mt5.copy_rates_range(symbol=self.name, timeframe=timeframe, date_from=date_from,
+                                                date_to=date_to)
+        if rates is not None:
+            return DataFrame(data=rates)
+        raise ValueError(f'Could not get rates for {self.name}')
 
-    async def copy_rates_range(self, *, timeframe: TimeFrame, date_from: datetime | int, date_to: datetime | int) -> DataFrame | None:
+    async def copy_ticks_from(self, *, date_from: datetime | int, count: int = 100, flags: CopyTicks = CopyTicks.ALL) -> DataFrame:
         """
-        Get bars in the specified date range from the MetaTrader 5 terminal.
+        Get ticks from the MetaTrader 5 terminal starting from the specified date.
 
-        Args:
-            timeframe (TimeFrame): Timeframe the bars are requested for. Set by a value from the TimeFrame enumeration. Required unnamed parameter.
+        Args: date_from (datetime | int): Date the ticks are requested from. Set by the 'datetime' object or as a
+        number of seconds elapsed since 1970.01.01.
 
-            date_from (datetime | int): Date the bars are requested from. Set by the 'datetime' object or as a number of seconds
-                elapsed since 1970.01.01. Bars with the open time >= date_from are returned. Required unnamed parameter.
+            count (int): Number of requested ticks. Defaults to 100
 
-            date_to (datetime | int): Date, up to which the bars are requested. Set by the 'datetime' object or as a number of
-                seconds elapsed since 1970.01.01. Bars with the open time <= date_to are returned. Required unnamed parameter.
+            flags (CopyTicks): A flag to define the type of the requested ticks from CopyTicks enum. INFO is the default
 
         Returns:
-            DataFrame: Rates as pandas DataFrame object
-            None: Return None if there is an error
-        """
-        rates = await self.mt5.copy_rates_range(symbol=self.name, timeframe=timeframe, date_from=date_from, date_to=date_to)
-        return DataFrame(rates) if rates is not None else None
+             DataFrame: Returns a Dataframe object as a collection of ticks ordered chronologically.
 
-    async def copy_ticks_range(self, *, date_from: datetime | int, date_to: datetime | int, flags: CopyTicks = CopyTicks.INFO):
+        Raises:
+            ValueError: If request was unsuccessful and None was returned
         """
-        Get ticks for the specified date range from the MetaTrader 5 terminal.
+        ticks = await self.mt5.copy_ticks_from(self.name, date_from, count, flags)
+        if ticks is not None:
+            return DataFrame(data=ticks)
+        raise ValueError(f'Could not get ticks for {self.name}')
+
+    async def copy_ticks_range(self, *, date_from: datetime | int, date_to: datetime | int, flags: CopyTicks = CopyTicks.ALL) -> DataFrame:
+        """Get ticks for the specified date range from the MetaTrader 5 terminal.
+
         Args:
             date_from: Date the bars are requested from. Set by the 'datetime' object or as a number of seconds elapsed since 1970.01.01. Bars with
                 the open time >= date_from are returned. Required unnamed parameter.
 
             date_to: Date, up to which the bars are requested. Set by the 'datetime' object or as a number of seconds elapsed since 1970.01.01. Bars
                 with the open time <= date_to are returned. Required unnamed parameter.
-
+                
             flags (CopyTicks):
 
         Returns:
-            DataFrame: Rates as pandas DataFrame object
-            None: Return None if there is an error
+            DataFrame: Returns a Dataframe object as a collection of ticks ordered chronologically.
+
+        Raises:
+            ValueError: If request was unsuccessful and None was returned.
         """
         ticks = await self.mt5.copy_ticks_range(self.name, date_from, date_to, flags)
-        return DataFrame(ticks) if ticks is not None else None
+        if ticks is not None:
+            return DataFrame(data=ticks)
+        raise ValueError(f'Could not get ticks for {self.name}')
```

### Comparing `aiomql-1/src/aiomql/trader.py` & `aiomql-2.0/src/aiomql/trader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 from abc import ABC, abstractmethod
+from typing import TypeVar
 
-from .account import Account, account
 from .order import Order
-from .result import TradeResult
-from .symbol import Symbol
+from .symbol import Symbol as _Symbol
+from .account import Account
+
+Symbol = TypeVar('Symbol', bound=_Symbol)
 
 
 class Trader(ABC):
-    """
-    Helper class for creating a Trader object. Handles the initializing of an order and the placing of trades
+    """ Helper class for creating a Trader object. Handles the initializing of an order and the placing of trades
+
     Args:
         symbol (Symbol): Financial instrument
 
-        account (Account): Trading account
-
     Attributes:
-
-        symbol (Symbol): Financial instrument class Symbol class or a subclass of it.
-
+        symbol (Symbol): Financial instrument class Symbol class or any subclass of it.
         account (Account): Trading account
-
         order (Order): Trade order
     """
-    def __init__(self, *, symbol: type(Symbol), account: Account = account):
-        self.account = account
+
+    def __init__(self, *, symbol: Symbol):
         self.symbol = symbol
         self.order = Order(symbol=symbol.name)
+        self.account = Account()
 
+    @abstractmethod
     async def create_order(self, *args, **kwargs):
-        """
-        Create an order, and update the order object initialized
+        """Create an order, and update the order object initialized
         Args:
             *args:
             **kwargs:
-
-        Returns:
-
         """
 
     @abstractmethod
-    async def place_trade(self, *args, **kwargs) -> TradeResult | None:
-        """
-        Send trade to server
+    async def place_trade(self, *args, **kwargs):
+        """Send trade to the broker
+
         Args:
             *args:
             **kwargs:
-
-        Returns: TradeResult if successful
-
         """
```

### Comparing `aiomql-1/src/aiomql.egg-info/PKG-INFO` & `aiomql-2.0/src/aiomql.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 1
+Version: 2.0
 Summary: Asynchronous MetaTrader5 library and Bot Builder
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,86 +13,65 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiomql
 ![GitHub](https://img.shields.io/github/license/ichinga-samuel/aiomql?style=plastic)
 ![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/aiomql?style=plastic)
 ![PyPI](https://img.shields.io/pypi/v/aiomql)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ichinga-samuel/aiomql/Push)
-![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/ichinga-samuel/aiomql)
+
 
 ## Installation
 ```bash
 pip install aiomql
 ```
 
 ## Key Features
 - Asynchronous Python Library For MetaTrader 5
 - Build bots for trading in different financial markets using a bot factory
-- Use threadpool or proccesspool executors to run multiple strategies on multiple instruments concurrently
+- Use threadpool executors to run multiple strategies on multiple instruments concurrently
 - Record and keep track of trades and strategies in csv files.
 - Utility classes for using the MetaTrader 5 Library
 - Sample Pre-Built strategies
 
-## Simple Usage as an Async MetaTrader5 Libray
+## Simple Usage as an asynchronous MetaTrader5 Libray
 ```python
 import asyncio
 
 # import the class
-from aiomql import MetaTrader
-from aiomql import Account, Terminal
-from aiomql import TimeFrame, OrderType
+from aiomql import MetaTrader, Account, TimeFrame, OrderType
 
 
 async def main():
-    # Initialize Terminal
-    terminal = Terminal()
-    mt5 = MetaTrader()
-    await mt5.initialize()
-
-    # create Account
-    account = Account(account_number=30371334, password="nwa0#anaEze", server="Deriv-Demo")
-
-    # login with account
-    await account.login()
-
-    # connection status with the account.connected property
-    res = "Login Successful" if account.connected else "Unable to login into account"
-    print(res)
-
-    # set account properties
-    account.risk = 0.10  # percentage of account equity to risk i.e 10%
-    account.risk_to_reward = 3
-
-    # get symbols available for the account if login was successful
-    if account.connected:
-        symbols = await mt5.symbols_get()
-        print(symbols)
-
-    # print timeframe constant for five minutes
-    print(TimeFrame.M5)
-    await terminal.shutdown()
-
+    # Assuming your login details are already defined in the aiomql.json somewhere in your project directory. 
+    acc = Account()
+    
+    # if this is unsuccessful the program exits
+    await acc.sign_in()
+    
+    # print all available symbols
+    print(acc.symbols)
 
 asyncio.run(main())
 ```
-## As a Bot Building FrameWork using a Prebuilt Strategy
+## As a Bot Building FrameWork using a Sample Strategy
 ```python
-import logging
-
 from aiomql import Bot
-from aiomql.lib import ForexMarket, FingerTrap
+from aiomql import ForexSymbol
+from aiomql.lib import FingerTrap
+
+# Create a bot instance
+bot = Bot()
 
-fmt = "%(asctime)s : %(message)s"
+# Choose a Symbol to trade
+symbol = ForexSymbol(name='EURUSD')
 
-logging.basicConfig(filename='example.log', format=fmt, level=logging.DEBUG)
+# Create a strategy
+ft_eur_usd = FingerTrap(symbol=symbol)
 
-market = ForexMarket()
-bot = Bot(market=market)
+# Add strategy to Bot
+bot.add_strategy(ft_eur_usd)
 
-# Finger strategy on all instruments in the forex markets
-bot.add_strategy_all(strategy=FingerTrap)
+# run the bot
 bot.execute()
-# This assumes that a mt5.json config file with account_number, password and server keys is available
 ```
 
 see [docs](https://github.com/Ichinga-Samuel/aiomql/tree/master/docs)
```

### Comparing `aiomql-1/src/aiomql.egg-info/SOURCES.txt` & `aiomql-2.0/src/aiomql.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 README.md
 pyproject.toml
 setup.py
 src/aiomql/__init__.py
 src/aiomql/account.py
 src/aiomql/bot_builder.py
 src/aiomql/candle.py
-src/aiomql/config.py
 src/aiomql/executor.py
 src/aiomql/history.py
-src/aiomql/market.py
 src/aiomql/order.py
 src/aiomql/positions.py
 src/aiomql/records.py
 src/aiomql/result.py
 src/aiomql/strategy.py
 src/aiomql/symbol.py
 src/aiomql/terminal.py
@@ -22,20 +20,20 @@
 src/aiomql/utils.py
 src/aiomql.egg-info/PKG-INFO
 src/aiomql.egg-info/SOURCES.txt
 src/aiomql.egg-info/dependency_links.txt
 src/aiomql.egg-info/requires.txt
 src/aiomql.egg-info/top_level.txt
 src/aiomql/core/__init__.py
+src/aiomql/core/base.py
+src/aiomql/core/config.py
 src/aiomql/core/constants.py
 src/aiomql/core/meta_trader.py
 src/aiomql/core/models.py
-src/aiomql/lib/markets/forex_market.py
-src/aiomql/lib/markets/synthetic_market.py
+src/aiomql/lib/__init__.py
+src/aiomql/lib/strategies/__init__.py
 src/aiomql/lib/strategies/finger_trap.py
+src/aiomql/lib/symbols/__init__.py
 src/aiomql/lib/symbols/forex_symbol.py
 src/aiomql/lib/symbols/synthetic_symbol.py
 src/aiomql/lib/traders/simple_deal_trader.py
-tests/test_config.py
-tests/test_constants.py
-tests/test_symbol.py
-tests/test_terminal.py
+src/aiomql/lib/traders/trade_result.py
```

