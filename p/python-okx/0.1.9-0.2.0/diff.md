# Comparing `tmp/python-okx-0.1.9.tar.gz` & `tmp/python-okx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-okx-0.1.9.tar", last modified: Wed Apr 12 06:43:15 2023, max compression
+gzip compressed data, was "python-okx-0.2.0.tar", last modified: Mon Jun 19 14:20:09 2023, max compression
```

## Comparing `python-okx-0.1.9.tar` & `python-okx-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-04-12 06:43:15.071591 python-okx-0.1.9/
--rw-r--r--   0 oker       (501) staff       (20)     2934 2023-04-12 06:43:15.071277 python-okx-0.1.9/PKG-INFO
--rw-r--r--   0 oker       (501) staff       (20)     2586 2023-02-16 06:55:25.000000 python-okx-0.1.9/README.md
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-04-12 06:43:15.061478 python-okx-0.1.9/okx/
--rw-r--r--   0 oker       (501) staff       (20)     7099 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Account.py
--rw-r--r--   0 oker       (501) staff       (20)     3699 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/BlockTrading.py
--rw-r--r--   0 oker       (501) staff       (20)     1542 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Convert.py
--rw-r--r--   0 oker       (501) staff       (20)     2139 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Earning.py
--rw-r--r--   0 oker       (501) staff       (20)      756 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/FDBroker.py
--rw-r--r--   0 oker       (501) staff       (20)     5058 2023-04-12 06:41:59.000000 python-okx-0.1.9/okx/Funding.py
--rw-r--r--   0 oker       (501) staff       (20)     4248 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Grid.py
--rw-r--r--   0 oker       (501) staff       (20)     4476 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/MarketData.py
--rw-r--r--   0 oker       (501) staff       (20)     5031 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/NDBroker.py
--rw-r--r--   0 oker       (501) staff       (20)     5056 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/PublicData.py
--rw-r--r--   0 oker       (501) staff       (20)      463 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Status.py
--rw-r--r--   0 oker       (501) staff       (20)     2660 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/SubAccount.py
--rw-r--r--   0 oker       (501) staff       (20)     8218 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/Trade.py
--rw-r--r--   0 oker       (501) staff       (20)     2299 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/TradingData.py
--rw-r--r--   0 oker       (501) staff       (20)       58 2023-04-12 06:42:27.000000 python-okx-0.1.9/okx/__init__.py
--rw-r--r--   0 oker       (501) staff       (20)     2233 2023-03-28 03:20:42.000000 python-okx-0.1.9/okx/client.py
--rw-r--r--   0 oker       (501) staff       (20)    10930 2023-03-28 03:20:01.000000 python-okx-0.1.9/okx/consts.py
--rw-r--r--   0 oker       (501) staff       (20)     1246 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/exceptions.py
--rw-r--r--   0 oker       (501) staff       (20)     1826 2022-12-12 02:06:58.000000 python-okx-0.1.9/okx/utils.py
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-04-12 06:43:15.068356 python-okx-0.1.9/okx/websocket/
--rw-r--r--   0 oker       (501) staff       (20)     2070 2022-12-16 08:49:53.000000 python-okx-0.1.9/okx/websocket/WsClientFactory.py
--rw-r--r--   0 oker       (501) staff       (20)     1712 2022-12-05 07:37:01.000000 python-okx-0.1.9/okx/websocket/WsClientProtocol.py
--rw-r--r--   0 oker       (501) staff       (20)     5393 2022-12-15 13:01:18.000000 python-okx-0.1.9/okx/websocket/WsConnectManager.py
--rw-r--r--   0 oker       (501) staff       (20)     2672 2022-12-04 06:10:10.000000 python-okx-0.1.9/okx/websocket/WsLoginFactory.py
--rw-r--r--   0 oker       (501) staff       (20)      924 2022-12-15 13:06:35.000000 python-okx-0.1.9/okx/websocket/WsPrivate.py
--rw-r--r--   0 oker       (501) staff       (20)      498 2022-12-15 12:59:40.000000 python-okx-0.1.9/okx/websocket/WsPublic.py
--rw-r--r--   0 oker       (501) staff       (20)     2234 2022-12-05 08:05:32.000000 python-okx-0.1.9/okx/websocket/WsUtils.py
--rw-r--r--   0 oker       (501) staff       (20)        0 2022-12-15 12:47:25.000000 python-okx-0.1.9/okx/websocket/__init__.py
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-04-12 06:43:15.070707 python-okx-0.1.9/python_okx.egg-info/
--rw-r--r--   0 oker       (501) staff       (20)     2934 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/PKG-INFO
--rw-r--r--   0 oker       (501) staff       (20)      723 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/SOURCES.txt
--rw-r--r--   0 oker       (501) staff       (20)        1 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/dependency_links.txt
--rw-r--r--   0 oker       (501) staff       (20)       67 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/requires.txt
--rw-r--r--   0 oker       (501) staff       (20)        4 2023-04-12 06:43:14.000000 python-okx-0.1.9/python_okx.egg-info/top_level.txt
--rw-r--r--   0 oker       (501) staff       (20)       38 2023-04-12 06:43:15.071721 python-okx-0.1.9/setup.cfg
--rw-r--r--   0 oker       (501) staff       (20)      758 2023-03-28 03:15:08.000000 python-okx-0.1.9/setup.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-06-19 14:20:09.441786 python-okx-0.2.0/
+-rw-r--r--   0 oker       (501) staff       (20)     2934 2023-06-19 14:20:09.441452 python-okx-0.2.0/PKG-INFO
+-rw-r--r--   0 oker       (501) staff       (20)     2586 2023-05-12 09:40:37.000000 python-okx-0.2.0/README.md
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-06-19 14:20:09.436357 python-okx-0.2.0/okx/
+-rw-r--r--   0 oker       (501) staff       (20)     9021 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/Account.py
+-rw-r--r--   0 oker       (501) staff       (20)     4096 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/BlockTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)     1542 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/Convert.py
+-rw-r--r--   0 oker       (501) staff       (20)     2653 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/CopyTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)     3822 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/Earning.py
+-rw-r--r--   0 oker       (501) staff       (20)      756 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/FDBroker.py
+-rw-r--r--   0 oker       (501) staff       (20)     6058 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/Funding.py
+-rw-r--r--   0 oker       (501) staff       (20)     6659 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/Grid.py
+-rw-r--r--   0 oker       (501) staff       (20)     4896 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/MarketData.py
+-rw-r--r--   0 oker       (501) staff       (20)     5031 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/NDBroker.py
+-rw-r--r--   0 oker       (501) staff       (20)     5104 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/PublicData.py
+-rw-r--r--   0 oker       (501) staff       (20)      463 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/Status.py
+-rw-r--r--   0 oker       (501) staff       (20)     3496 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/SubAccount.py
+-rw-r--r--   0 oker       (501) staff       (20)    10459 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/Trade.py
+-rw-r--r--   0 oker       (501) staff       (20)     2299 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/TradingData.py
+-rw-r--r--   0 oker       (501) staff       (20)       58 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/__init__.py
+-rw-r--r--   0 oker       (501) staff       (20)     2120 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/client.py
+-rw-r--r--   0 oker       (501) staff       (20)    13729 2023-06-19 08:56:33.000000 python-okx-0.2.0/okx/consts.py
+-rw-r--r--   0 oker       (501) staff       (20)     1182 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/exceptions.py
+-rw-r--r--   0 oker       (501) staff       (20)     1826 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/utils.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-06-19 14:20:09.439304 python-okx-0.2.0/okx/websocket/
+-rw-r--r--   0 oker       (501) staff       (20)     2070 2023-05-25 08:06:59.000000 python-okx-0.2.0/okx/websocket/WsClientFactory.py
+-rw-r--r--   0 oker       (501) staff       (20)     1712 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/websocket/WsClientProtocol.py
+-rw-r--r--   0 oker       (501) staff       (20)     5393 2023-05-29 14:26:48.000000 python-okx-0.2.0/okx/websocket/WsConnectManager.py
+-rw-r--r--   0 oker       (501) staff       (20)     2672 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/websocket/WsLoginFactory.py
+-rw-r--r--   0 oker       (501) staff       (20)      924 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/websocket/WsPrivate.py
+-rw-r--r--   0 oker       (501) staff       (20)      498 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/websocket/WsPublic.py
+-rw-r--r--   0 oker       (501) staff       (20)     2234 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/websocket/WsUtils.py
+-rw-r--r--   0 oker       (501) staff       (20)        0 2023-05-12 09:40:37.000000 python-okx-0.2.0/okx/websocket/__init__.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2023-06-19 14:20:09.441118 python-okx-0.2.0/python_okx.egg-info/
+-rw-r--r--   0 oker       (501) staff       (20)     2934 2023-06-19 14:20:09.000000 python-okx-0.2.0/python_okx.egg-info/PKG-INFO
+-rw-r--r--   0 oker       (501) staff       (20)      742 2023-06-19 14:20:09.000000 python-okx-0.2.0/python_okx.egg-info/SOURCES.txt
+-rw-r--r--   0 oker       (501) staff       (20)        1 2023-06-19 14:20:09.000000 python-okx-0.2.0/python_okx.egg-info/dependency_links.txt
+-rw-r--r--   0 oker       (501) staff       (20)       67 2023-06-19 14:20:09.000000 python-okx-0.2.0/python_okx.egg-info/requires.txt
+-rw-r--r--   0 oker       (501) staff       (20)        4 2023-06-19 14:20:09.000000 python-okx-0.2.0/python_okx.egg-info/top_level.txt
+-rw-r--r--   0 oker       (501) staff       (20)       38 2023-06-19 14:20:09.441843 python-okx-0.2.0/setup.cfg
+-rw-r--r--   0 oker       (501) staff       (20)      758 2023-05-14 08:39:08.000000 python-okx-0.2.0/setup.py
```

### Comparing `python-okx-0.1.9/PKG-INFO` & `python-okx-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python SDK for OKX
 Home-page: https://okx.com/docs-v5/
 Author: okxv5api
 Author-email: api@okg.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-okx-0.1.9/README.md` & `python-okx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/Account.py` & `python-okx-0.2.0/okx/Funding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,166 +1,142 @@
 from .client import Client
 from .consts import *
 
 
-class AccountAPI(Client):
+class FundingAPI(Client):
+
 
     def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain,debug)
 
+    # Get Deposit Address
+    def get_deposit_address(self, ccy):
+        params = {'ccy': ccy}
+        return self._request_with_params(GET, DEPOSIT_ADDRESS, params)
 
-    # Get Positions
-    def get_position_risk(self, instType=''):
-        params = {}
-        if instType:
-            params['instType'] = instType
-        return self._request_with_params(GET, POSITION_RISK, params)
+    # Get Transfer State
+    def transfer_state(self, transId,type=''):
+        params = {'transId': transId, 'type': type}
+        return self._request_with_params(GET, TRANSFER_STATE, params)
 
     # Get Balance
-    def get_account_balance(self, ccy=''):
-        params = {}
-        if ccy:
-            params['ccy'] = ccy
-        return self._request_with_params(GET, ACCOUNT_INFO, params)
-
-    # Get Positions
-    def get_positions(self, instType='', instId=''):
-        params = {'instType': instType, 'instId': instId}
-        return self._request_with_params(GET, POSITION_INFO, params)
-
-    # Get Bills Details (recent 7 days)
-    def get_account_bills(self, instType='', ccy='', mgnMode='', ctType='', type='', subType='', after='', before='',
-                         limit=''):
-        params = {'instType': instType, 'ccy': ccy, 'mgnMode': mgnMode, 'ctType': ctType, 'type': type,
-                  'subType': subType, 'after': after, 'before': before, 'limit': limit}
-        return self._request_with_params(GET, BILLS_DETAIL, params)
-
-    # Get Bills Details (recent 3 months)
-    def get_account_bills_archive(self, instType='', ccy='', mgnMode='', ctType='', type='', subType='', after='', before='',
-                          limit=''):
-        params = {'instType': instType, 'ccy': ccy, 'mgnMode': mgnMode, 'ctType': ctType, 'type': type,
-                  'subType': subType, 'after': after, 'before': before, 'limit': limit}
-        return self._request_with_params(GET, BILLS_ARCHIVE, params)
-
-    # Get Account Configuration
-    def get_account_config(self):
-        return self._request_without_params(GET, ACCOUNT_CONFIG)
-
-    # Get Account Configuration
-    def set_position_mode(self, posMode):
-        params = {'posMode': posMode}
-        return self._request_with_params(POST, POSITION_MODE, params)
+    def get_balances(self, ccy=''):
+        params = {'ccy': ccy}
+        return self._request_with_params(GET, GET_BALANCES, params)
 
     # Get Account Configuration
-    def set_leverage(self, lever, mgnMode, instId='', ccy='', posSide=''):
-        params = {'lever': lever, 'mgnMode': mgnMode, 'instId': instId, 'ccy': ccy, 'posSide': posSide}
-        return self._request_with_params(POST, SET_LEVERAGE, params)
-
-    # Get Maximum Tradable Size For Instrument
-    def get_max_order_size(self, instId, tdMode, ccy='', px=''):
-        params = {'instId': instId, 'tdMode': tdMode, 'ccy': ccy, 'px': px}
-        return self._request_with_params(GET, MAX_TRADE_SIZE, params)
-
-    # Get Maximum Available Tradable Amount
-    def get_max_avail_size(self, instId, tdMode, ccy='', reduceOnly=''):
-        params = {'instId': instId, 'tdMode': tdMode, 'ccy': ccy, 'reduceOnly': reduceOnly}
-        return self._request_with_params(GET, MAX_AVAIL_SIZE, params)
-
-    # Increase / Decrease margin
-    def adjustment_margin(self, instId, posSide, type, amt,loanTrans=''):
-        params = {'instId': instId, 'posSide': posSide, 'type': type, 'amt': amt,'loanTrans':loanTrans}
-        return self._request_with_params(POST, ADJUSTMENT_MARGIN, params)
-
-    # Get Leverage
-    def get_leverage(self, instId, mgnMode):
-        params = {'instId': instId, 'mgnMode': mgnMode}
-        return self._request_with_params(GET, GET_LEVERAGE, params)
-
-    # Get the maximum loan of isolated MARGIN
-    def get_max_loan(self, instId, mgnMode, mgnCcy):
-        params = {'instId': instId, 'mgnMode': mgnMode, 'mgnCcy': mgnCcy}
-        return self._request_with_params(GET, MAX_LOAN, params)
-
-    # Get Fee Rates
-    def get_fee_rates(self, instType, instId='', uly='', category='',instFamily = ''):
-        params = {'instType': instType, 'instId': instId, 'uly': uly, 'category': category,'instFamily':instFamily}
-        return self._request_with_params(GET, FEE_RATES, params)
-
-    # Get interest-accrued
-    def get_interest_accrued(self, instId='', ccy='', mgnMode='', after='', before='', limit=''):
-        params = {'instId': instId, 'ccy': ccy, 'mgnMode': mgnMode, 'after': after, 'before': before, 'limit': limit}
-        return self._request_with_params(GET, INTEREST_ACCRUED, params)
+    def funds_transfer(self, ccy, amt, from_, to, type='0', subAcct='', instId='', toInstId='',loanTrans=''):
+        params = {'ccy': ccy, 'amt': amt, 'from': from_, 'to': to, 'type': type, 'subAcct': subAcct, 'instId': instId,
+                  'toInstId': toInstId,'loanTrans':loanTrans}
+        return self._request_with_params(POST, FUNDS_TRANSFER, params)
+
+    # Withdrawal
+    def withdrawal(self, ccy, amt, dest, toAddr, fee, chain='', areaCode='', clientId=''):
+        params = {'ccy': ccy, 'amt': amt, 'dest': dest, 'toAddr': toAddr, 'fee': fee, 'chain': chain,
+                  'areaCode': areaCode, 'clientId': clientId}
+        return self._request_with_params(POST, WITHDRAWAL_COIN, params)
+
+    # Get Deposit History
+    def get_deposit_history(self, ccy='', state='', after='', before='', limit='', txId='', depId='', fromWdId=''):
+        params = {'ccy': ccy, 'state': state, 'after': after, 'before': before, 'limit': limit, 'txId': txId,
+                  'depId': depId, 'fromWdId': fromWdId}
+        return self._request_with_params(GET, DEPOSIT_HISTORIY, params)
+
+    # Get Withdrawal History
+    def get_withdrawal_history(self, ccy='', wdId='', state='', after='', before='', limit='',txId=''):
+        params = {'ccy': ccy, 'wdId': wdId, 'state': state, 'after': after, 'before': before, 'limit': limit,'txId':txId}
+        return self._request_with_params(GET, WITHDRAWAL_HISTORIY, params)
 
-    # Get interest-accrued
-    def get_interest_rate(self, ccy=''):
+    # Get Currencies
+    def get_currencies(self, ccy=''):
         params = {'ccy': ccy}
-        return self._request_with_params(GET, INTEREST_RATE, params)
+        return self._request_with_params(GET, CURRENCY_INFO, params)
 
-    # Set Greeks (PA/BS)
-    def set_greeks(self, greeksType):
-        params = {'greeksType': greeksType}
-        return self._request_with_params(POST, SET_GREEKS, params)
-
-    # Set Isolated Mode
-    def set_isolated_mode(self, isoMode,type):
-        params = {'isoMode': isoMode, 'type':type}
-        return self._request_with_params(POST, ISOLATED_MODE, params)
+    # PiggyBank Purchase/Redemption
+    def purchase_redempt(self, ccy, amt, side, rate):
+        params = {'ccy': ccy, 'amt': amt, 'side': side,'rate':rate}
+        return self._request_with_params(POST, PURCHASE_REDEMPT, params)
+
+    # Get Withdrawal History
+    def get_bills(self, ccy='', type='', after='', before='', limit=''):
+        params = {'ccy': ccy, 'type': type, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, BILLS_INFO, params)
+
+
+    #Get Deposit Lightning
+    def get_deposit_lightning(self, ccy,amt,to=""):
+        params = {'ccy':ccy,'amt':amt}
+        if to:
+            params = {'to':to}
+        return self._request_with_params(GET, DEPOSIT_LIGHTNING, params)
+
+    # Withdrawal Lightning
+    def withdrawal_lightning(self, ccy,invoice,memo=''):
+        params = {'ccy':ccy, 'invoice':invoice, 'memo':memo}
+        return self._request_with_params(POST, WITHDRAWAL_LIGHTNING, params)
+
+    # POST SET LENDING RATE
+    def set_lending_rate(self, ccy, rate):
+        params = {'ccy': ccy, 'rate': rate}
+        return self._request_with_params(POST, SET_LENDING_RATE, params)
+
+    # GET LENDING HISTORY
+    def get_lending_history(self, ccy='', before='', after='', limit='' ):
+        params = {'ccy': ccy, 'after': after, 'before': before, 'limit': limit }
+        return self._request_with_params(GET, LENDING_HISTORY, params)
+
+    # GET LENDING RATE HISTORY
+    def get_lending_rate_history(self, ccy='',after = '',before = '',limit = '' ):
+        params = {'ccy': ccy,'after':after,'before':before,'limit':limit}
+        return self._request_with_params(GET, LENDING_RATE_HISTORY, params)
 
-    # Get Maximum Withdrawals
-    def get_max_withdrawal(self, ccy=''):
+    # GET LENDING RATE SUMMARY
+    def get_lending_rate_summary(self, ccy=''):
         params = {'ccy': ccy}
-        return self._request_with_params(GET, MAX_WITHDRAWAL, params)
+        return self._request_with_params(GET, LENDING_RATE_SUMMARY, params)
 
-    # Get borrow repay
-    def borrow_repay(self, ccy='', side='', amt=''):
-        params = {'ccy': ccy, 'side': side, 'amt': amt}
-        return self._request_with_params(POST, BORROW_REPAY, params)
-
-    # Get borrow repay history
-    def get_borrow_repay_history(self, ccy='', after='', before='', limit=''):
-        params = {'ccy': ccy, 'after': after, 'before': before, 'limit':limit}
-        return self._request_with_params(GET, BORROW_REPAY_HISTORY, params)
-
-    # Get Obtain borrowing rate and limit
-    def get_interest_limits(self, type='',ccy=''):
-        params = {'type': type, 'ccy': ccy}
-        return self._request_with_params(GET, INTEREST_LIMITS, params)
-
-    # Get Simulated Margin
-    def get_simulated_margin(self, instType	='',inclRealPos=True,instId='',pos=''):
-        params = {'instType': instType, 'inclRealPos': inclRealPos,'instId': instId,'pos': pos,}
-        return self._request_with_params(POST, SIMULATED_MARGIN, params)
 
-    # Get  Greeks
-    def get_greeks(self, ccy=''):
-        params = {'ccy': ccy}
-        return self._request_with_params(GET, GREEKS, params)
+    #POST /api/v5/asset/cancel-withdrawal
+    def cancel_withdrawal(self,wdId = ''):
+        params = {
+            'wdId':wdId
+        }
+        return self._request_with_params(POST, CANCEL_WITHDRAWAL, params)
 
-    #GET /api/v5/account/risk-state
-    def get_account_position_risk(self):
-        return self._request_without_params(GET, ACCOUNT_RISK)
+    #POST /api/v5/asset/convert-dust-assets
+    def convert_dust_assets(self,ccy = []):
+        params = {
+            'ccy':ccy
+        }
+        return self._request_with_params(POST, CONVERT_DUST_ASSETS, params)
 
-    #GET /api/v5/account/positions-history
-    def get_positions_history(self,instType = '', instId = '',mgnMode = '',type = '',posId = '',after = '',before ='',limit = ''):
+    #GET /api/v5/asset/asset-valuation
+    def get_asset_valuation(self,ccy = ''):
         params = {
-            'instType':instType,
-            'instId':instId,
-            'mgnMode':mgnMode,
-            'type':type,
-            'posId':posId,
-            'after':after,
-            'before':before,
-            'limit':limit
+            'ccy':ccy
         }
-        return self._request_with_params(GET,POSITIONS_HISTORY,params)
+        return self._request_with_params(GET, ASSET_VALUATION, params)
 
-    #GET /api/v5/account/position-tiers
-    def get_account_position_tiers(self,instType = '', uly = '',instFamily = ''):
+    #GET / api / v5 / asset / saving - balance
+    def get_saving_balance(self,ccy = ''):
         params = {
-            'instType':instType,
-            'uly':uly,
-            'instFamily':instFamily
+            'ccy':ccy
         }
-        return self._request_with_params(GET,GET_PM_LIMIT,params)
+        return self._request_with_params(GET, GET_SAVING_BALANCE, params)
 
+    #Get non-tradable assets
+    def get_non_tradable_assets(self, ccy=''):
+        params = {
+            'ccy': ccy
+        }
+        return self._request_with_params(GET, GET_NON_TRADABLE_ASSETS, params)
 
+    #Get deposit withdraw status
+    def get_deposit_withdraw_status(self, wdId='', txId='', ccy='', to='', chain=''):
+        params = {'wdId': wdId, 'txId': txId, 'ccy': ccy, 'to': to, 'chain': chain}
+        return self._request_with_params(GET, GET_DEPOSIT_WITHDrAW_STATUS, params)
+
+    #Get withdrawal history
+    def get_withdrawal_history(self, ccy='', wdId='', clientId='', txId='', type='', state='', after='', before	='', limit=''):
+        params = {'ccy': ccy, 'wdId': wdId, 'clientId': clientId, 'txId': txId, 'type': type, 'state': state, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, GET_WITHDRAWAL_HISTORY, params)
```

### Comparing `python-okx-0.1.9/okx/BlockTrading.py` & `python-okx-0.2.0/okx/BlockTrading.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,37 +6,39 @@
     def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain,debug)
 
     def counterparties(self):
         params = {}
         return self._request_with_params(GET, COUNTERPARTIES, params)
 
-    def create_rfq(self, counterparties=[], anonymous='false', clRfqId='', legs = []):
-        params = {'counterparties': counterparties, 'anonymous': anonymous, 'clRfqId': clRfqId, 'legs': legs}
+    def create_rfq(self, counterparties=[], anonymous='false', clRfqId='', tag='', allowPartialExecution='false',
+                   legs=[]):
+        params = {'counterparties': counterparties, 'anonymous': anonymous, 'clRfqId': clRfqId, 'tag': tag,
+                  'allowPartialExecution': allowPartialExecution, 'legs': legs}
         return self._request_with_params(POST, CREATE_RFQ, params)
 
     def cancel_rfq(self, rfqId = '', clRfqId = ''):
         params = {'rfqId': rfqId, 'clRfqId': clRfqId}
         return self._request_with_params(POST, CANCEL_RFQ, params)
 
     def cancel_batch_rfqs(self, rfqIds=[], clRfqIds=[]):
         params = {'rfqIds': rfqIds, 'clRfqIds': clRfqIds}
         return self._request_with_params(POST, CANCEL_BATCH_RFQS, params)
 
     def cancel_all_rfqs(self):
         params = {}
         return self._request_with_params(POST, CANCEL_ALL_RSQS, params)
 
-    def execute_quote(self, rfqId='', quoteId=''):
-        params = {'rfqId': rfqId, 'quoteId': quoteId}
+    def execute_quote(self, rfqId='', quoteId='', legs=[]):
+        params = {'rfqId': rfqId, 'quoteId': quoteId, 'legs': legs}
         return self._request_with_params(POST, EXECUTE_QUOTE, params)
 
-    def create_quote(self, rfqId='', clQuoteId='', quoteSide = '', legs = [],anonymous=False,expiresIn=''):
-        params = {'rfqId': rfqId, 'clQuoteId': clQuoteId, 'quoteSide': quoteSide, 'legs': legs,
-                  'anonymous':anonymous,'expiresIn':expiresIn}
+    def create_quote(self, rfqId='', clQuoteId='', tag='', quoteSide='', legs=[], anonymous=False, expiresIn=''):
+        params = {'rfqId': rfqId, 'clQuoteId': clQuoteId, 'tag': tag, 'quoteSide': quoteSide, 'legs': legs,
+                  'anonymous': anonymous, 'expiresIn': expiresIn}
         return self._request_with_params(POST, CREATE_QUOTE, params)
 
     def cancel_quote(self, quoteId  = '', clQuoteId = ''):
         params = {'quoteId': quoteId, 'clQuoteId': clQuoteId}
         return self._request_with_params(POST, CANCEL_QUOTE, params)
 
     def cancel_batch_quotes(self, quoteIds='', clQuoteIds=''):
@@ -51,21 +53,27 @@
         params = {'rfqId': rfqId, 'clRfqId': clRfqId, 'state': state, 'beginId': beginId, 'endId': endId, 'limit':limit}
         return self._request_with_params(GET, GET_RFQS, params)
 
     def get_quotes(self, rfqId = '', clRfqId = '', quoteId = '', clQuoteId = '', state = '', beginId = '', endId = '', limit = ''):
         params = {'rfqId': rfqId, 'clRfqId': clRfqId, 'quoteId':quoteId,'clQuoteId':clQuoteId, 'state': state, 'beginId': beginId, 'endId': endId, 'limit':limit}
         return self._request_with_params(GET, GET_QUOTES, params)
 
-    def get_trades(self, rfqId = '', clRfqId = '', quoteId = '', clQuoteId = '', state = '', beginId = '', endId = '', limit = ''):
-        params = {'rfqId': rfqId, 'clRfqId': clRfqId, 'quoteId':quoteId,'clQuoteId':clQuoteId, 'state': state, 'beginId': beginId, 'endId': endId, 'limit':limit}
+    def get_trades(self, rfqId='', clRfqId='', quoteId='', clQuoteId='', state='', beginId='', endId='', beginTs='',
+                   endTs='', limit=''):
+        params = {'rfqId': rfqId, 'clRfqId': clRfqId, 'quoteId': quoteId, 'clQuoteId': clQuoteId, 'state': state,
+                  'beginId': beginId, 'endId': endId, 'beginTs': beginTs, 'endTs': endTs, 'limit': limit}
         return self._request_with_params(GET, GET_RFQ_TRADES, params)
 
     def get_public_trades(self, beginId = '', endId = '', limit = ''):
         params = {'beginId': beginId, 'endId': endId, 'limit': limit}
         return self._request_with_params(GET, GET_PUBLIC_TRADES, params)
 
     def reset_mmp(self):
         return self._request_without_params(POST, MMP_RESET)
 
     def set_marker_instrument(self,params = []):
 
-        return self._request_with_params(POST, MARKER_INSTRUMENT_SETTING, params)
+        return self._request_with_params(POST, MARKER_INSTRUMENT_SETTING, params)
+
+    #Get Quote products
+    def get_quote_products(self):
+        return self._request_without_params(GET, MARKER_INSTRUMENT_SETTING)
```

### Comparing `python-okx-0.1.9/okx/Convert.py` & `python-okx-0.2.0/okx/Convert.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/Earning.py` & `python-okx-0.2.0/okx/TradingData.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,55 @@
 from .client import Client
 from .consts import *
 
 
-class EarningAPI(Client):
+class TradingDataAPI(Client):
+
     def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True):
-        Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug)
+        Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain,debug)
+
+
+    def get_support_coin(self):
+        return self._request_without_params(GET, SUPPORT_COIN)
+
+    def get_taker_volume(self, ccy, instType, begin='', end='', period=''):
+        params = {'ccy': ccy, 'instType': instType, 'begin': begin, 'end': end, 'period': period}
+        return self._request_with_params(GET, TAKER_VOLUME, params)
+
+    def get_margin_lending_ratio(self, ccy, begin='', end='', period=''):
+        params = {'ccy': ccy, 'begin': begin, 'end': end, 'period': period}
+        return self._request_with_params(GET, MARGIN_LENDING_RATIO, params)
+
+    def get_long_short_ratio(self, ccy, begin='', end='', period=''):
+        params = {'ccy': ccy, 'begin': begin, 'end': end, 'period': period}
+        return self._request_with_params(GET, LONG_SHORT_RATIO, params)
+
+    def get_contracts_interest_volume(self, ccy, begin='', end='', period=''):
+        params = {'ccy': ccy, 'begin': begin, 'end': end, 'period': period}
+        return self._request_with_params(GET, CONTRACTS_INTEREST_VOLUME, params)
+
+    def get_options_interest_volume(self, ccy, period=''):
+        params = {'ccy': ccy, 'period': period}
+        return self._request_with_params(GET, OPTIONS_INTEREST_VOLUME, params)
+
+    def get_put_call_ratio(self, ccy, period=''):
+        params = {'ccy': ccy, 'period': period}
+        return self._request_with_params(GET, PUT_CALL_RATIO, params)
+
+    def get_interest_volume_expiry(self, ccy, period=''):
+        params = {'ccy': ccy, 'period': period}
+        return self._request_with_params(GET, OPEN_INTEREST_VOLUME_EXPIRY, params)
+
+    def get_interest_volume_strike(self, ccy, expTime, period=''):
+        params = {'ccy': ccy, 'expTime': expTime, 'period': period}
+        return self._request_with_params(GET, INTEREST_VOLUME_STRIKE, params)
+
+    def get_taker_block_volume(self, ccy, period=''):
+        params = {'ccy': ccy, 'period': period}
+        return self._request_with_params(GET, TAKER_FLOW, params)
+
+
 
-    def get_offers(self,productId = '',protocolType = '',ccy = ''):
-        params = {
-            'productId':productId,
-            'protocolType':protocolType,
-            'ccy':ccy
-        }
-        return self._request_with_params(GET,STACK_DEFI_OFFERS,params)
-
-    def purchase(self,productId = '',investData = [],term = ''):
-
-        params = {
-            'productId':productId,
-            'investData':investData
-        }
-        if term != '':
-            params['term'] = term
-        return self._request_with_params(POST,STACK_DEFI_PURCHASE,params)
-
-    def redeem(self,ordId = '',protocolType = '',allowEarlyRedeem = ''):
-        params = {
-            'ordId':ordId,
-            'protocolType':protocolType,
-            'allowEarlyRedeem':allowEarlyRedeem
-        }
-        return self._request_with_params(POST,STACK_DEFI_REDEEM,params)
-
-    def cancel(self,ordId = '',protocolType = ''):
-        params = {
-            'ordId':ordId,
-            'protocolType':protocolType
-        }
-        return self._request_with_params(POST,STACK_DEFI_CANCEL,params)
-
-    def get_activity_orders(self,productId = '',protocolType = '',ccy = '',state = ''):
-        params = {
-            'productId':productId,
-            'protocolType':protocolType,
-            'ccy':ccy,
-            'state':state
-        }
-        return self._request_with_params(GET,STACK_DEFI_ORDERS_ACTIVITY,params)
-
-    def get_orders_history(self,productId = '',protocolType = '',ccy = '',after = '',before = '',limit = ''):
-        params = {
-            'productId':productId,
-            'protocolType':protocolType,
-            'ccy':ccy,
-            'after':after,
-            'before':before,
-            'limit':limit
-        }
-        return self._request_with_params(GET,STACK_DEFI_ORDERS_HISTORY,params)
```

### Comparing `python-okx-0.1.9/okx/FDBroker.py` & `python-okx-0.2.0/okx/FDBroker.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/Funding.py` & `python-okx-0.2.0/okx/MarketData.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,136 @@
 from .client import Client
 from .consts import *
 
 
-class FundingAPI(Client):
-
+class MarketAPI(Client):
 
     def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain,debug)
 
-    # Get Deposit Address
-    def get_deposit_address(self, ccy):
-        params = {'ccy': ccy}
-        return self._request_with_params(GET, DEPOSIT_ADDRESS, params)
-
-    # Get Transfer State
-    def transfer_state(self, transId,type=''):
-        params = {'transId': transId, 'type': type}
-        return self._request_with_params(GET, TRANSFER_STATE, params)
-
-    # Get Balance
-    def get_balances(self, ccy=''):
-        params = {'ccy': ccy}
-        return self._request_with_params(GET, GET_BALANCES, params)
-
-    # Get Account Configuration
-    def funds_transfer(self, ccy, amt, from_, to, type='0', subAcct='', instId='', toInstId='',loanTrans=''):
-        params = {'ccy': ccy, 'amt': amt, 'from': from_, 'to': to, 'type': type, 'subAcct': subAcct, 'instId': instId,
-                  'toInstId': toInstId,'loanTrans':loanTrans}
-        return self._request_with_params(POST, FUNDS_TRANSFER, params)
-
-    # Withdrawal
-    def withdrawal(self, ccy, amt, dest, toAddr, fee,chain = '', clientId = ''):
-        params = {'ccy': ccy, 'amt': amt, 'dest': dest, 'toAddr': toAddr, 'fee': fee,'chain':chain,'clientId':clientId}
-        return self._request_with_params(POST, WITHDRAWAL_COIN, params)
-
-    # Get Deposit History
-    def get_deposit_history(self, ccy='', state='', after='', before='', limit='',txId='',depId=''):
-        params = {'ccy': ccy, 'state': state, 'after': after, 'before': before, 'limit': limit,'txId':txId,'depId':depId}
-        return self._request_with_params(GET, DEPOSIT_HISTORIY, params)
-
-    # Get Withdrawal History
-    def get_withdrawal_history(self, ccy='', wdId='', state='', after='', before='', limit='',txId=''):
-        params = {'ccy': ccy, 'wdId': wdId, 'state': state, 'after': after, 'before': before, 'limit': limit,'txId':txId}
-        return self._request_with_params(GET, WITHDRAWAL_HISTORIY, params)
-
-    # Get Currencies
-    def get_currencies(self, ccy=''):
-        params = {'ccy': ccy}
-        return self._request_with_params(GET, CURRENCY_INFO, params)
-
-    # PiggyBank Purchase/Redemption
-    def purchase_redempt(self, ccy, amt, side, rate):
-        params = {'ccy': ccy, 'amt': amt, 'side': side,'rate':rate}
-        return self._request_with_params(POST, PURCHASE_REDEMPT, params)
-
-    # Get Withdrawal History
-    def get_bills(self, ccy='', type='', after='', before='', limit=''):
-        params = {'ccy': ccy, 'type': type, 'after': after, 'before': before, 'limit': limit}
-        return self._request_with_params(GET, BILLS_INFO, params)
-
-
-    #Get Deposit Lightning
-    def get_deposit_lightning(self, ccy,amt,to=""):
-        params = {'ccy':ccy,'amt':amt}
-        if to:
-            params = {'to':to}
-        return self._request_with_params(GET, DEPOSIT_LIGHTNING, params)
-
-    # Withdrawal Lightning
-    def withdrawal_lightning(self, ccy,invoice,memo=''):
-        params = {'ccy':ccy, 'invoice':invoice, 'memo':memo}
-        return self._request_with_params(POST, WITHDRAWAL_LIGHTNING, params)
-
-
-    # POST SET LENDING RATE
-    def set_lending_rate(self, ccy, rate):
-        params = {'ccy': ccy, 'rate': rate}
-        return self._request_with_params(POST, SET_LENDING_RATE, params)
-
-
-    # GET LENDING HISTORY
-    def get_lending_history(self, ccy='', before='', after='', limit='' ):
-        params = {'ccy': ccy, 'after': after, 'before': before, 'limit': limit }
-        return self._request_with_params(GET, LENDING_HISTORY, params)
 
+    # Get Tickers
+    def get_tickers(self, instType, uly='', instFamily =''):
+        if uly:
+            params = {'instType': instType, 'uly': uly, 'instFamily': instFamily}
+        else:
+            params = {'instType': instType, 'instFamily': instFamily}
+        return self._request_with_params(GET, TICKERS_INFO, params)
+
+    # Get Ticker
+    def get_ticker(self, instId):
+        params = {'instId': instId}
+        return self._request_with_params(GET, TICKER_INFO, params)
+
+    # Get Index Tickers
+    def get_index_tickers(self, quoteCcy='', instId=''):
+        params = {'quoteCcy': quoteCcy, 'instId': instId}
+        return self._request_with_params(GET, INDEX_TICKERS, params)
+
+    # Get Order Book
+    def get_orderbook(self, instId, sz=''):
+        params = {'instId': instId, 'sz': sz}
+        return self._request_with_params(GET, ORDER_BOOKS, params)
+
+    # Get Candlesticks
+    def get_candlesticks(self, instId, after='', before='', bar='', limit=''):
+        params = {'instId': instId, 'after': after, 'before': before, 'bar': bar, 'limit': limit}
+        return self._request_with_params(GET, MARKET_CANDLES, params)
+
+    # GGet Candlesticks History（top currencies only）
+    def get_history_candlesticks(self, instId, after='', before='', bar='', limit=''):
+        params = {'instId': instId, 'after': after, 'before': before, 'bar': bar, 'limit': limit}
+        return self._request_with_params(GET, HISTORY_CANDLES, params)
+
+    # Get Index Candlesticks
+    def get_index_candlesticks(self, instId, after='', before='', bar='', limit=''):
+        params = {'instId': instId, 'after': after, 'before': before, 'bar': bar, 'limit': limit}
+        return self._request_with_params(GET, INDEX_CANSLES, params)
+
+    # Get Mark Price Candlesticks
+    def get_mark_price_candlesticks(self, instId, after='', before='', bar='', limit=''):
+        params = {'instId': instId, 'after': after, 'before': before, 'bar': bar, 'limit': limit}
+        return self._request_with_params(GET, MARKPRICE_CANDLES, params)
+
+    # Get Index Candlesticks
+    def get_trades(self, instId, limit=''):
+        params = {'instId': instId, 'limit': limit}
+        return self._request_with_params(GET, MARKET_TRADES, params)
+
+    # Get Volume
+    def get_volume(self):
+        return self._request_without_params(GET, VOLUMNE)
+
+    # Get Oracle
+    def get_oracle(self):
+        return self._request_without_params(GET, ORACLE)
+
+    # Get Tier
+    def get_tier(self, instType='', tdMode='', uly='', instId='', ccy='', tier=''):
+        params = {'instType': instType, 'tdMode': tdMode, 'uly': uly, 'instId': instId, 'ccy': ccy, 'tier': tier}
+        return self._request_with_params(GET, TIER, params)
+
+    #GET /api/v5/market/index-components
+    def get_index_components(self,index = ''):
+        param = {
+            'index':index
+        }
+        return self._request_with_params(GET,INDEX_COMPONENTS,param)
 
-    # GET LENDING RATE HISTORY
-    def get_lending_rate_history(self, ccy='',after = '',before = '',limit = '' ):
-        params = {'ccy': ccy,'after':after,'before':before,'limit':limit}
-        return self._request_with_params(GET, LENDING_RATE_HISTORY, params)
 
+    #GET /api/v5/market/exchange-rate
+    def get_exchange_rate(self):
+        return self._request_without_params(GET, EXCHANGE_RATE)
 
-    # GET LENDING RATE SUMMARY
-    def get_lending_rate_summary(self, ccy=''):
-        params = {'ccy': ccy}
-        return self._request_with_params(GET, LENDING_RATE_SUMMARY, params)
+    #GET /api/v5/market/history-trades
+    def get_history_trades(self,instId = '',type = '',after = '',before = '',limit = ''):
+        params = {
+            'instId':instId,
+            'type':type,
+            'after':after,
+            'before':before,
+            'limit':limit
+        }
+        return self._request_with_params(GET,HISTORY_TRADES,params)
 
+    #GET /api/v5/market/block-ticker
+    def get_block_ticker(self,instId = ''):
+        params = {
+            'instId':instId
+        }
+        return self._request_with_params(GET,BLOCK_TICKER,params)
 
-    #POST /api/v5/asset/cancel-withdrawal
-    def cancel_withdrawal(self,wdId = ''):
+    #GET /api/v5/market/block-tickers
+    def get_block_tickers(self,instType = '',uly = '', instFamily = ''):
         params = {
-            'wdId':wdId
+            'instType':instType,
+            'uly':uly,
+            'instFamily':instFamily
         }
-        return self._request_with_params(POST, CANCEL_WITHDRAWAL, params)
+        return self._request_with_params(GET, BLOCK_TICKERS, params)
 
-    #POST /api/v5/asset/convert-dust-assets
-    def convert_dust_assets(self,ccy = []):
+    #GET /api/v5/market/block-trades
+    def get_block_trades(self,instId = ''):
         params = {
-            'ccy':ccy
+            'instId':instId
         }
-        return self._request_with_params(POST, CONVERT_DUST_ASSETS, params)
+        return self._request_with_params(GET, BLOCK_TRADES, params)
 
-    #GET /api/v5/asset/asset-valuation
-    def get_asset_valuation(self,ccy = ''):
+    #- Get order lite book
+    def get_order_lite_book(self,instId = ''):
         params = {
-            'ccy':ccy
+            'instId':instId
         }
-        return self._request_with_params(GET, ASSET_VALUATION, params)
+        return self._request_with_params(GET, GET_ORDER_LITE_BOOK, params)
 
-    #GET / api / v5 / asset / saving - balance
-    def get_saving_balance(self,ccy = ''):
+    #- Get option trades
+    def get_option_trades(self,instFamily = ''):
         params = {
-            'ccy':ccy
+            'instFamily':instFamily
         }
-        return self._request_with_params(GET, GET_SAVING_BALANCE, params)
+        return self._request_with_params(GET, GET_OPTION_TRADES, params)
+
+
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-okx-0.1.9/okx/Grid.py` & `python-okx-0.2.0/okx/Grid.py`

 * *Files 23% similar despite different names*

```diff
@@ -72,7 +72,61 @@
         params = {
             'algoOrdType': algoOrdType,
             'instId': instId,
             'direction': direction,
             'duration':duration
         }
         return self._request_with_params(GET, GRID_AI_PARAM, params)
+
+    # - Place recurring buy order
+    def place_recurring_buy_order(self, stgyName='', recurringList=[], period='', recurringDay='', recurringTime='',
+                                  timeZone='', amt='', investmentCcy='', tdMode='', algoClOrdId='', tag=''):
+        params = {'stgyName': stgyName, 'recurringList': recurringList, 'period': period, 'recurringDay': recurringDay,
+                  'recurringTime': recurringTime,
+                  'timeZone': timeZone, 'amt': amt, 'investmentCcy': investmentCcy, 'tdMode': tdMode,
+                  'algoClOrdId': algoClOrdId, 'tag': tag}
+        return self._request_with_params(POST, PLACE_RECURRING_BUY_ORDER, params)
+
+    # - Amend recurring buy order
+    def amend_recurring_buy_order(self, algoId='', stgyName=''):
+        params = {'algoId': algoId, 'stgyName': stgyName}
+        return self._request_with_params(POST, AMEND_RECURRING_BUY_ORDER, params)
+
+    # - Stop recurring buy order
+    def stop_recurring_buy_order(self, orders_data):
+        return self._request_with_params(POST, STOP_RECURRING_BUY_ORDER, orders_data)
+
+    # - Get recurring buy order list
+    def get_recurring_buy_order_list(self, algoId='', after='', before='', limit=''):
+        params = {
+            'algoId': algoId,
+            'after': after,
+            'before': before,
+            'limit': limit
+        }
+        return self._request_with_params(GET, GET_RECURRING_BUY_ORDER_LIST, params)
+
+    # - Get recurring buy order history
+    def get_recurring_buy_order_history(self, algoId='', after='', before='', limit=''):
+        params = {
+            'algoId': algoId,
+            'after': after,
+            'before': before,
+            'limit': limit
+        }
+        return self._request_with_params(GET, GET_RECURRING_BUY_ORDER_HISTORY, params)
+
+    # - Get recurring buy order details
+    def get_recurring_buy_order_details(self, algoId=''):
+        params = {'algoId': algoId}
+        return self._request_with_params(GET, GET_RECURRING_BUY_ORDER_DETAILS, params)
+
+    # - Get recurring buy sub orders
+    def get_recurring_buy_sub_orders(self, algoId='', ordId='', after='', before='', limit=''):
+        params = {
+            'algoId': algoId,
+            'ordId': ordId,
+            'after': after,
+            'before': before,
+            'limit': limit
+        }
+        return self._request_with_params(GET, GET_RECURRING_BUY_SUB_ORDERS, params)
```

### Comparing `python-okx-0.1.9/okx/MarketData.py` & `python-okx-0.2.0/okx/PublicData.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,124 @@
 from .client import Client
 from .consts import *
 
 
-class MarketAPI(Client):
+class PublicAPI(Client):
 
     def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain,debug)
 
+    # Get Instruments
+    def get_instruments(self, instType, uly='', instId='',instFamily = ''):
+        params = {'instType': instType, 'uly': uly, 'instId': instId,'instFamily':instFamily}
+        return self._request_with_params(GET, INSTRUMENT_INFO, params)
+
+    # Get Delivery/Exercise History
+    def get_delivery_exercise_history(self, instType, uly = '', after='', before='', limit='',instFamily = ''):
+        params = {'instType': instType, 'uly': uly, 'after': after, 'before': before, 'limit': limit,'instFamily':instFamily}
+        return self._request_with_params(GET, DELIVERY_EXERCISE, params)
+
+    # Get Open Interest
+    def get_open_interest(self, instType, uly='', instId='' ,instFamily =''):
+        params = {'instType': instType, 'uly': uly, 'instId': instId,'instFamily':instFamily}
+        return self._request_with_params(GET, OPEN_INTEREST, params)
 
-    # Get Tickers
-    def get_tickers(self, instType, uly='', instFamily =''):
-        if uly:
-            params = {'instType': instType, 'uly': uly, 'instFamily': instFamily}
-        else:
-            params = {'instType': instType, 'instFamily': instFamily}
-        return self._request_with_params(GET, TICKERS_INFO, params)
+    # Get Funding Rate
+    def get_funding_rate(self, instId):
+        params = {'instId': instId}
+        return self._request_with_params(GET, FUNDING_RATE, params)
+
+    # Get Funding Rate History
+    def funding_rate_history(self, instId, after='', before='', limit=''):
+        params = {'instId': instId, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, FUNDING_RATE_HISTORY, params)
 
-    # Get Ticker
-    def get_ticker(self, instId):
+    # Get Limit Price
+    def get_price_limit(self, instId):
         params = {'instId': instId}
-        return self._request_with_params(GET, TICKER_INFO, params)
+        return self._request_with_params(GET, PRICE_LIMIT, params)
 
-    # Get Index Tickers
-    def get_index_tickers(self, quoteCcy='', instId=''):
-        params = {'quoteCcy': quoteCcy, 'instId': instId}
-        return self._request_with_params(GET, INDEX_TICKERS, params)
-
-    # Get Order Book
-    def get_orderbook(self, instId, sz=''):
-        params = {'instId': instId, 'sz': sz}
-        return self._request_with_params(GET, ORDER_BOOKS, params)
-
-    # Get Candlesticks
-    def get_candlesticks(self, instId, after='', before='', bar='', limit=''):
-        params = {'instId': instId, 'after': after, 'before': before, 'bar': bar, 'limit': limit}
-        return self._request_with_params(GET, MARKET_CANDLES, params)
-
-    # GGet Candlesticks History（top currencies only）
-    def get_history_candlesticks(self, instId, after='', before='', bar='', limit=''):
-        params = {'instId': instId, 'after': after, 'before': before, 'bar': bar, 'limit': limit}
-        return self._request_with_params(GET, HISTORY_CANDLES, params)
-
-    # Get Index Candlesticks
-    def get_index_candlesticks(self, instId, after='', before='', bar='', limit=''):
-        params = {'instId': instId, 'after': after, 'before': before, 'bar': bar, 'limit': limit}
-        return self._request_with_params(GET, INDEX_CANSLES, params)
-
-    # Get Mark Price Candlesticks
-    def get_mark_price_candlesticks(self, instId, after='', before='', bar='', limit=''):
-        params = {'instId': instId, 'after': after, 'before': before, 'bar': bar, 'limit': limit}
-        return self._request_with_params(GET, MARKPRICE_CANDLES, params)
-
-    # Get Index Candlesticks
-    def get_trades(self, instId, limit=''):
-        params = {'instId': instId, 'limit': limit}
-        return self._request_with_params(GET, MARKET_TRADES, params)
-
-    # Get Volume
-    def get_volume(self):
-        return self._request_without_params(GET, VOLUMNE)
-
-    # Get Oracle
-    def get_oracle(self):
-        return self._request_without_params(GET, ORACLE)
+    # Get Option Market Data
+    def get_opt_summary(self, uly = '', expTime='',instFamily=''):
+        params = {'uly': uly, 'expTime': expTime,'instFamily':instFamily}
+        return self._request_with_params(GET, OPT_SUMMARY, params)
+
+    # Get Estimated Delivery/Excercise Price
+    def get_estimated_price(self, instId):
+        params = {'instId': instId}
+        return self._request_with_params(GET, ESTIMATED_PRICE, params)
+
+    # Get Discount Rate And Interest-Free Quota
+    def discount_interest_free_quota(self, ccy=''):
+        params = {'ccy': ccy}
+        return self._request_with_params(GET, DICCOUNT_INTETEST_INFO, params)
+
+    # Get System Time
+    def get_system_time(self):
+        return self._request_without_params(GET, SYSTEM_TIME)
+
+    # Get Mark Price
+    def get_mark_price(self, instType, uly='', instId='',instFamily = ''):
+        params = {'instType': instType, 'uly': uly, 'instId': instId,'instFamily':instFamily}
+        return self._request_with_params(GET, MARK_PRICE, params)
 
     # Get Tier
-    def get_tier(self, instType='', tdMode='', uly='', instId='', ccy='', tier=''):
-        params = {'instType': instType, 'tdMode': tdMode, 'uly': uly, 'instId': instId, 'ccy': ccy, 'tier': tier}
+    def get_position_tiers(self, instType, tdMode, uly='', instId='', ccy='', tier='',instFamily =''):
+        params = {'instType': instType, 'tdMode': tdMode, 'uly': uly, 'instId': instId, 'ccy': ccy, 'tier': tier,'instFamily':instFamily}
         return self._request_with_params(GET, TIER, params)
 
-    #GET /api/v5/market/index-components
-    def get_index_components(self,index = ''):
-        param = {
-            'index':index
-        }
-        return self._request_with_params(GET,INDEX_COMPONENTS,param)
-
+    #GET /api/v5/public/interest-rate-loan-quota
+    def get_interest_rate_loan_quota(self):
+        return self._request_without_params(GET,INTEREST_LOAN)
+
+    #GET /api/v5/public/vip-interest-rate-loan-quota
+    def get_vip_interest_rate_loan_quota(self):
+        return self._request_without_params(GET, VIP_INTEREST_RATE_LOAN_QUOTA)
 
-    #GET /api/v5/market/exchange-rate
-    def get_exchange_rate(self):
-        return self._request_without_params(GET, EXCHANGE_RATE)
+    #GET /api/v5/public/underlying
+    def get_underlying(self,instType = ''):
+        params = {
+            'instType':instType
+        }
+        return self._request_with_params(GET, UNDERLYING, params)
 
-    #GET /api/v5/market/history-trades
-    def get_history_trades(self,instId = '',type = '',after = '',before = '',limit = ''):
+    #GET /api/v5/public/insurance-fund
+    def get_insurance_fund(self,instType = '',type = '',uly = '',ccy='',before = '',after = '',limit = '',instFamily=''):
         params = {
-            'instId':instId,
+            'instType':instType,
             'type':type,
-            'after':after,
+            'uly':uly,
+            'ccy':ccy,
             'before':before,
-            'limit':limit
+            'after':after,
+            'limit':limit,
+            'instFamily':instFamily
         }
-        return self._request_with_params(GET,HISTORY_TRADES,params)
+        return self._request_with_params(GET, INSURANCE_FUND, params)
 
-    #GET /api/v5/market/block-ticker
-    def get_block_ticker(self,instId = ''):
+    #GET /api/v5/public/convert-contract-coin
+    def get_convert_contract_coin(self,type = '',instId = '',sz = '',px = '',unit = ''):
         params = {
-            'instId':instId
+            'type':type,
+            'instId':instId,
+            'sz':sz,
+            'px':px,
+            'unit':unit
         }
-        return self._request_with_params(GET,BLOCK_TICKER,params)
+        return self._request_with_params(GET, CONVERT_CONTRACT_COIN, params)
 
-    #GET /api/v5/market/block-tickers
-    def get_block_tickers(self,instType = '',uly = '', instFamily = ''):
+    # Get option tickBands
+    def get_option_tickBands(self, instType='', instFamily=''):
         params = {
-            'instType':instType,
-            'uly':uly,
-            'instFamily':instFamily
+            'instType': instType,
+            'instFamily': instFamily
         }
-        return self._request_with_params(GET, BLOCK_TICKERS, params)
+        return self._request_with_params(GET, GET_OPTION_TICKBANDS, params)
 
-    #GET /api/v5/market/block-trades
-    def get_block_trades(self,instId = ''):
+    # Get option trades
+    def get_option_trades(self, instId='', instFamily='', optType=''):
         params = {
-            'instId':instId
+            'instId': instId,
+            'instFamily': instFamily,
+            'optType': optType
         }
-        return self._request_with_params(GET, BLOCK_TRADES, params)
-
-
-
-
-
-
+        return self._request_with_params(GET, GET_OPTION_TRADES, params)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python-okx-0.1.9/okx/NDBroker.py` & `python-okx-0.2.0/okx/NDBroker.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/SubAccount.py` & `python-okx-0.2.0/okx/SubAccount.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,9 +55,29 @@
     def get_funding_balance(self,subAcct='',ccy=''):
         params = {
             'subAcct':subAcct,
             'ccy':ccy
         }
         return self._request_with_params(GET, GET_ASSET_SUBACCOUNT_BALANCE, params)
 
+    # - Get the user's affiliate rebate information
+    def get_the_user_affiliate_rebate_information(self, apiKey=''):
+        params = {
+            'apiKey': apiKey
+        }
+        return self._request_with_params(GET, GET_THE_USER_AFFILIATE_REBATE, params)
 
+    # - Set sub_accounts VIP loan%
+    def set_sub_accounts_VIP_loan(self, enable='', alloc=[]):
+        params = {
+            'enable': enable,
+            'alloc': alloc
+        }
+        return self._request_with_params(POST, SET_SUB_ACCOUNTS_VIP_LOAN, params)
 
+    # - Get sub_account borrow interest and limit
+    def get_sub_account_borrow_interest_and_limit(self, subAcct='', ccy=''):
+        params = {
+            'subAcct': subAcct,
+            'ccy': ccy
+        }
+        return self._request_with_params(GET, GET_SUB_ACCOUNT_BORROW_INTEREST_AND_LIMIT, params)
```

### Comparing `python-okx-0.1.9/okx/Trade.py` & `python-okx-0.2.0/okx/Account.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,199 @@
 from .client import Client
 from .consts import *
 
 
-class TradeAPI(Client):
+class AccountAPI(Client):
 
     def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain,debug)
 
-    # Place Order
-    def place_order(self, instId, tdMode, side, ordType, sz, ccy='', clOrdId='', tag='', posSide='', px='',
-                    reduceOnly='', tgtCcy=''):
-        params = {'instId': instId, 'tdMode': tdMode, 'side': side, 'ordType': ordType, 'sz': sz, 'ccy': ccy,
-                  'clOrdId': clOrdId, 'tag': tag, 'posSide': posSide, 'px': px, 'reduceOnly': reduceOnly,
-                  'tgtCcy': tgtCcy}
-        return self._request_with_params(POST, PLACR_ORDER, params)
-
-    # Place Multiple Orders
-    def place_multiple_orders(self, orders_data):
-        return self._request_with_params(POST, BATCH_ORDERS, orders_data)
-
-    # Cancel Order
-    def cancel_order(self, instId, ordId='', clOrdId=''):
-        params = {'instId': instId, 'ordId': ordId, 'clOrdId': clOrdId}
-        return self._request_with_params(POST, CANAEL_ORDER, params)
-
-    # Cancel Multiple Orders
-    def cancel_multiple_orders(self, orders_data):
-        return self._request_with_params(POST, CANAEL_BATCH_ORDERS, orders_data)
-
-    # Amend Order
-    def amend_order(self, instId, cxlOnFail='', ordId='', clOrdId='', reqId='', newSz='', newPx=''):
-        params = {'instId': instId, 'cxlOnFailc': cxlOnFail, 'ordId': ordId, 'clOrdId': clOrdId, 'reqId': reqId,
-                  'newSz': newSz,
-                  'newPx': newPx}
-        return self._request_with_params(POST, AMEND_ORDER, params)
-
-    # Amend Multiple Orders
-    def amend_multiple_orders(self, orders_data):
-        return self._request_with_params(POST, AMEND_BATCH_ORDER, orders_data)
-
-    # Close Positions
-    def close_positions(self, instId, mgnMode, posSide='', ccy='',autoCxl=''):
-        params = {'instId': instId, 'mgnMode': mgnMode, 'posSide': posSide, 'ccy': ccy,'autoCxl':autoCxl}
-        return self._request_with_params(POST, CLOSE_POSITION, params)
-
-    # Get Order Details
-    def get_order(self, instId, ordId='', clOrdId=''):
-        params = {'instId': instId, 'ordId': ordId, 'clOrdId': clOrdId}
-        return self._request_with_params(GET, ORDER_INFO, params)
-
-    # Get Order List
-    def get_order_list(self, instType='', uly='', instId='', ordType='', state='', after='', before='', limit='',instFamily = ''):
-        params = {'instType': instType, 'uly': uly, 'instId': instId, 'ordType': ordType, 'state': state,
-                  'after': after, 'before': before, 'limit': limit,'instFamily':instFamily}
-        return self._request_with_params(GET, ORDERS_PENDING, params)
-
-    # Get Order History (last 7 days）
-    def get_orders_history(self, instType, uly='', instId='', ordType='', state='', after='', before='', limit='',instFamily = ''):
-        params = {'instType': instType, 'uly': uly, 'instId': instId, 'ordType': ordType, 'state': state,
-                  'after': after, 'before': before, 'limit': limit,'instFamily':instFamily}
-        return self._request_with_params(GET, ORDERS_HISTORY, params)
-
-    # Get Order History (last 3 months)
-    def get_orders_history_archive(self, instType, uly='', instId='', ordType='', state='', after='', before='', limit='',instFamily = ''):
-        params = {'instType': instType, 'uly': uly, 'instId': instId, 'ordType': ordType, 'state': state,
-                  'after': after, 'before': before, 'limit': limit,'instFamily':instFamily}
-        return self._request_with_params(GET, ORDERS_HISTORY_ARCHIVE, params)
-
-    # Get Transaction Details
-    def get_fills(self, instType='', uly='', instId='', ordId='', after='', before='', limit='',instFamily = ''):
-        params = {'instType': instType, 'uly': uly, 'instId': instId, 'ordId': ordId, 'after': after, 'before': before,
-                  'limit': limit,'instFamily':instFamily}
-        return self._request_with_params(GET, ORDER_FILLS, params)
-
-    # Place Algo Order
-    def place_algo_order(self, instId='', tdMode='', side='', ordType='', sz='', ccy='',
-                         posSide='', reduceOnly='', tpTriggerPx='',
-                         tpOrdPx='', slTriggerPx='', slOrdPx='',
-                         triggerPx='', orderPx='', tgtCcy='', pxVar='',
-                         pxSpread='',
-                         szLimit='', pxLimit='', timeInterval='', tpTriggerPxType='', slTriggerPxType='',
-                         callbackRatio='',callbackSpread='',activePx='',tag='',triggerPxType=''):
-        params = {'instId': instId, 'tdMode': tdMode, 'side': side, 'ordType': ordType, 'sz': sz, 'ccy': ccy,
-                  'posSide': posSide, 'reduceOnly': reduceOnly, 'tpTriggerPx': tpTriggerPx, 'tpOrdPx': tpOrdPx,
-                  'slTriggerPx': slTriggerPx, 'slOrdPx': slOrdPx, 'triggerPx': triggerPx, 'orderPx': orderPx,
-                  'tgtCcy': tgtCcy, 'pxVar': pxVar, 'szLimit': szLimit, 'pxLimit': pxLimit,
-                  'timeInterval': timeInterval,
-                  'pxSpread': pxSpread, 'tpTriggerPxType': tpTriggerPxType, 'slTriggerPxType': slTriggerPxType,
-                  'callbackRatio' : callbackRatio, 'callbackSpread':callbackSpread,'activePx':activePx,
-                  'tag':tag,'triggerPxType':triggerPxType,}
-        return self._request_with_params(POST, PLACE_ALGO_ORDER, params)
-
-
-
-    # Cancel Algo Order
-    def cancel_algo_order(self, params):
-        return self._request_with_params(POST, CANCEL_ALGOS, params)
-
-    # Cancel Advance Algos
-    def cancel_advance_algos(self,params):
-        return self._request_with_params(POST, Cancel_Advance_Algos, params)
-
-    # Get Algo Order List
-    def order_algos_list(self, ordType ='', algoId='', instType='', instId='', after='', before='', limit=''):
-        params = {'ordType': ordType, 'algoId': algoId, 'instType': instType, 'instId': instId, 'after': after,
-                  'before': before, 'limit': limit}
-        return self._request_with_params(GET, ORDERS_ALGO_OENDING, params)
-
-    # Get Algo Order History
-    def order_algos_history(self, ordType, state='', algoId='', instType='', instId='', after='', before='', limit=''):
-        params = {'ordType': ordType, 'state': state, 'algoId': algoId, 'instType': instType, 'instId': instId,
-                  'after': after, 'before': before, 'limit': limit}
-        return self._request_with_params(GET, ORDERS_ALGO_HISTORY, params)
-
-    # Get Transaction Details History
-    def get_fills_history(self, instType, uly='', instId='', ordId='', after='', before='', limit='',instFamily=''):
-        params = {'instType': instType, 'uly': uly, 'instId': instId, 'ordId': ordId, 'after': after, 'before': before,
-                  'limit': limit,'instFamily':instFamily}
-        return self._request_with_params(GET, ORDERS_FILLS_HISTORY, params)
+    # Get Positions
+    def get_position_risk(self, instType=''):
+        params = {}
+        if instType:
+            params['instType'] = instType
+        return self._request_with_params(GET, POSITION_RISK, params)
+
+    # Get Balance
+    def get_account_balance(self, ccy=''):
+        params = {}
+        if ccy:
+            params['ccy'] = ccy
+        return self._request_with_params(GET, ACCOUNT_INFO, params)
+
+    # Get Positions
+    def get_positions(self, instType='', instId=''):
+        params = {'instType': instType, 'instId': instId}
+        return self._request_with_params(GET, POSITION_INFO, params)
+
+    # Get Bills Details (recent 7 days)
+    def get_account_bills(self, instType='', ccy='', mgnMode='', ctType='', type='', subType='', after='', before='',
+                         limit=''):
+        params = {'instType': instType, 'ccy': ccy, 'mgnMode': mgnMode, 'ctType': ctType, 'type': type,
+                  'subType': subType, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, BILLS_DETAIL, params)
+
+    # Get Bills Details (recent 3 months)
+    def get_account_bills_archive(self, instType='', ccy='', mgnMode='', ctType='', type='', subType='', after='', before='',
+                          limit=''):
+        params = {'instType': instType, 'ccy': ccy, 'mgnMode': mgnMode, 'ctType': ctType, 'type': type,
+                  'subType': subType, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, BILLS_ARCHIVE, params)
+
+    # Get Account Configuration
+    def get_account_config(self):
+        return self._request_without_params(GET, ACCOUNT_CONFIG)
+
+    # Get Account Configuration
+    def set_position_mode(self, posMode):
+        params = {'posMode': posMode}
+        return self._request_with_params(POST, POSITION_MODE, params)
+
+    # Get Account Configuration
+    def set_leverage(self, lever, mgnMode, instId='', ccy='', posSide=''):
+        params = {'lever': lever, 'mgnMode': mgnMode, 'instId': instId, 'ccy': ccy, 'posSide': posSide}
+        return self._request_with_params(POST, SET_LEVERAGE, params)
+
+    # Get Maximum Tradable Size For Instrument
+    def get_max_order_size(self, instId, tdMode, ccy='', px=''):
+        params = {'instId': instId, 'tdMode': tdMode, 'ccy': ccy, 'px': px}
+        return self._request_with_params(GET, MAX_TRADE_SIZE, params)
+
+    # Get Maximum Available Tradable Amount
+    def get_max_avail_size(self, instId, tdMode, ccy='', reduceOnly='', unSpotOffset='', quickMgnType=''):
+        params = {'instId': instId, 'tdMode': tdMode, 'ccy': ccy, 'reduceOnly': reduceOnly,
+                  'unSpotOffset': unSpotOffset, 'quickMgnType': quickMgnType}
+        return self._request_with_params(GET, MAX_AVAIL_SIZE, params)
+
+    # Increase / Decrease margin
+    def adjustment_margin(self, instId, posSide, type, amt,loanTrans=''):
+        params = {'instId': instId, 'posSide': posSide, 'type': type, 'amt': amt,'loanTrans':loanTrans}
+        return self._request_with_params(POST, ADJUSTMENT_MARGIN, params)
+
+    # Get Leverage
+    def get_leverage(self, instId, mgnMode):
+        params = {'instId': instId, 'mgnMode': mgnMode}
+        return self._request_with_params(GET, GET_LEVERAGE, params)
+
+    # Get the maximum loan of isolated MARGIN
+    def get_max_loan(self, instId, mgnMode, mgnCcy):
+        params = {'instId': instId, 'mgnMode': mgnMode, 'mgnCcy': mgnCcy}
+        return self._request_with_params(GET, MAX_LOAN, params)
+
+    # Get Fee Rates
+    def get_fee_rates(self, instType, instId='', uly='', category='',instFamily = ''):
+        params = {'instType': instType, 'instId': instId, 'uly': uly, 'category': category,'instFamily':instFamily}
+        return self._request_with_params(GET, FEE_RATES, params)
+
+    # Get interest-accrued
+    def get_interest_accrued(self, instId='', ccy='', mgnMode='', after='', before='', limit=''):
+        params = {'instId': instId, 'ccy': ccy, 'mgnMode': mgnMode, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, INTEREST_ACCRUED, params)
+
+    # Get interest-accrued
+    def get_interest_rate(self, ccy=''):
+        params = {'ccy': ccy}
+        return self._request_with_params(GET, INTEREST_RATE, params)
+
+    # Set Greeks (PA/BS)
+    def set_greeks(self, greeksType):
+        params = {'greeksType': greeksType}
+        return self._request_with_params(POST, SET_GREEKS, params)
+
+    # Set Isolated Mode
+    def set_isolated_mode(self, isoMode,type):
+        params = {'isoMode': isoMode, 'type':type}
+        return self._request_with_params(POST, ISOLATED_MODE, params)
+
+    # Get Maximum Withdrawals
+    def get_max_withdrawal(self, ccy=''):
+        params = {'ccy': ccy}
+        return self._request_with_params(GET, MAX_WITHDRAWAL, params)
+
+    # Get borrow repay
+    def borrow_repay(self, ccy='', side='', amt='', ordId=''):
+        params = {'ccy': ccy, 'side': side, 'amt': amt, 'ordId': ordId}
+        return self._request_with_params(POST, BORROW_REPAY, params)
+
+    # Get borrow repay history
+    def get_borrow_repay_history(self, ccy='', after='', before='', limit=''):
+        params = {'ccy': ccy, 'after': after, 'before': before, 'limit':limit}
+        return self._request_with_params(GET, BORROW_REPAY_HISTORY, params)
+
+    # Get Obtain borrowing rate and limit
+    def get_interest_limits(self, type='',ccy=''):
+        params = {'type': type, 'ccy': ccy}
+        return self._request_with_params(GET, INTEREST_LIMITS, params)
+
+    # Get Simulated Margin
+    def get_simulated_margin(self, instType='', inclRealPos=True, spotOffsetType='', simPos=[]):
+        params = {'instType': instType, 'inclRealPos': inclRealPos, 'spotOffsetType': spotOffsetType, 'simPos': simPos}
+        return self._request_with_params(POST, SIMULATED_MARGIN, params)
+
+    # Get  Greeks
+    def get_greeks(self, ccy=''):
+        params = {'ccy': ccy}
+        return self._request_with_params(GET, GREEKS, params)
+
+    #GET /api/v5/account/risk-state
+    def get_account_position_risk(self):
+        return self._request_without_params(GET, ACCOUNT_RISK)
 
-    def get_easy_convert_currency_list(self):
-        return self._request_without_params(GET, EASY_CONVERT_CURRENCY_LIST)
-
-    def easy_convert(self,fromCcy = [],toCcy = ''):
-        params = {
-            'fromCcy':fromCcy,
-            'toCcy':toCcy
-        }
-        return self._request_with_params(POST, EASY_CONVERT, params)
-
-    def get_easy_convert_history(self,before = '',after = '',limit = ''):
+    #GET /api/v5/account/positions-history
+    def get_positions_history(self,instType = '', instId = '',mgnMode = '',type = '',posId = '',after = '',before ='',limit = ''):
         params = {
-            'before':before,
+            'instType':instType,
+            'instId':instId,
+            'mgnMode':mgnMode,
+            'type':type,
+            'posId':posId,
             'after':after,
+            'before':before,
             'limit':limit
         }
-        return self._request_with_params(GET,CONVERT_EASY_HISTORY,params)
+        return self._request_with_params(GET,POSITIONS_HISTORY,params)
 
-    def get_oneclick_repay_list(self,debtType = ''):
+    #GET /api/v5/account/position-tiers
+    def get_account_position_tiers(self,instType = '', uly = '',instFamily = ''):
         params = {
-            'debtType':debtType
+            'instType':instType,
+            'uly':uly,
+            'instFamily':instFamily
         }
-        return self._request_with_params(GET,ONE_CLICK_REPAY_SUPPORT,params)
+        return self._request_with_params(GET,GET_PM_LIMIT,params)
 
-    def oneclick_repay(self,debtCcy = [] , repayCcy=''):
-        params = {
-            'debtCcy':debtCcy,
-            'repayCcy':repayCcy
-        }
-        return self._request_with_params(POST,ONE_CLICK_REPAY,params)
+    #- Get VIP interest accrued data
+    def get_VIP_interest_accrued_data(self, ccy='', ordId='', after='', before='', limit=''):
+        params = {'ccy': ccy, 'ordId': ordId, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, GET_VIP_INTEREST_ACCRUED_DATA, params)
+
+    #- Get VIP interest deducted data
+    def get_VIP_interest_deducted_data(self, ccy='', ordId='', after='', before='', limit=''):
+        params = {'ccy': ccy, 'ordId': ordId, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, GET_VIP_INTEREST_DEDUCTED_DATA, params)
+
+    # - Get VIP loan order list
+    def get_VIP_loan_order_list(self, ordId='',state='', ccy='', after='', before='', limit=''):
+        params = {'ordId': ordId, 'state': state, 'ccy': ccy,'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, GET_VIP_LOAN_ORDER_LIST, params)
+
+    #- Get VIP loan order detail
+    def get_VIP_loan_order_detail(self, ccy='', ordId='', after='', before='', limit=''):
+        params = {'ccy': ccy, 'ordId': ordId, 'after': after, 'before': before, 'limit': limit}
+        return self._request_with_params(GET, GET_VIP_LOAN_ORDER_DETAIL, params)
+
+    #- Set risk offset type
+    def set_risk_offset_typel(self, type=''):
+        params = {'type': type}
+        return self._request_with_params(POST, SET_RISK_OFFSET_TYPE,params)
 
-    def oneclick_repay_history(self,after = '',before = '',limit = ''):
+    # - Set auto loan
+    def set_auto_loan(self, autoLoan=''):
         params = {
-            'after':after,
-            'before':before,
-            'limit':limit
+            'autoLoan': autoLoan
         }
-        return self._request_with_params(GET,ONE_CLICK_REPAY_HISTORY,params)
+        return self._request_with_params(POST, SET_AUTO_LOAN, params)
+
+    #- Activate option
+    def activate_option(self):
+        return self._request_without_params(POST, ACTIVSTE_OPTION)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python-okx-0.1.9/okx/client.py` & `python-okx-0.2.0/okx/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,16 +33,14 @@
         if self.debug == True:
             print('domain:',self.domain)
             print('url:',request_path)
         if method == c.GET:
             response = self.client.get(request_path, headers=header)
         elif method == c.POST:
             response = self.client.post(request_path, data=body, headers=header)
-        if not str(response.status_code).startswith('2'):
-            raise exceptions.OkxAPIException(response)
         return response.json()
 
     def _request_without_params(self, method, request_path):
         return self._request(method, request_path, {})
 
     def _request_with_params(self, method, request_path, params):
         return self._request(method, request_path, params)
```

### Comparing `python-okx-0.1.9/okx/consts.py` & `python-okx-0.2.0/okx/consts.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,21 @@
 BORROW_REPAY = '/api/v5/account/borrow-repay'
 BORROW_REPAY_HISTORY = '/api/v5/account/borrow-repay-history'
 INTEREST_LIMITS = '/api/v5/account/interest-limits'
 SIMULATED_MARGIN = '/api/v5/account/simulated_margin'
 GREEKS = '/api/v5/account/greeks'
 POSITIONS_HISTORY = '/api/v5/account/positions-history' #need add
 GET_PM_LIMIT = '/api/v5/account/position-tiers' #need add
+GET_VIP_INTEREST_ACCRUED_DATA = '/api/v5/account/vip-interest-accrued'
+GET_VIP_INTEREST_DEDUCTED_DATA = '/api/v5/account/vip-interest-deducted'
+GET_VIP_LOAN_ORDER_LIST= '/api/v5/account/vip-loan-order-list'
+GET_VIP_LOAN_ORDER_DETAIL= '/api/v5/account/vip-loan-order-detail'
+SET_RISK_OFFSET_TYPE = '/api/v5/account/set-riskOffset-type'
+SET_AUTO_LOAN = '/api/v5/account/set-auto-loan'
+ACTIVSTE_OPTION = '/api/v5/account/activate-option'
 
 # funding-complete-testcomplete
 DEPOSIT_ADDRESS = '/api/v5/asset/deposit-address'
 GET_BALANCES = '/api/v5/asset/balances'
 FUNDS_TRANSFER = '/api/v5/asset/transfer'
 TRANSFER_STATE = '/api/v5/asset/transfer-state'
 WITHDRAWAL_COIN = '/api/v5/asset/withdrawal'
@@ -64,14 +71,17 @@
 CONVERT_DUST_ASSETS = '/api/v5/asset/convert-dust-assets' #need add
 ASSET_VALUATION = '/api/v5/asset/asset-valuation' #need add
 SET_LENDING_RATE = '/api/v5/asset/set-lending-rate'
 LENDING_HISTORY = '/api/v5/asset/lending-history'
 LENDING_RATE_HISTORY = '/api/v5/asset/lending-rate-history'
 LENDING_RATE_SUMMARY = '/api/v5/asset/lending-rate-summary'
 GET_SAVING_BALANCE = '/api/v5/asset/saving-balance' #need to add
+GET_WITHDRAWAL_HISTORY = '/api/v5/asset/withdrawal-history'
+GET_NON_TRADABLE_ASSETS = '/api/v5/asset/non-tradable-assets'
+GET_DEPOSIT_WITHDrAW_STATUS = '/api/v5/asset/deposit-withdraw-status'
 
 
 # Market Data-Complete-testComplete
 TICKERS_INFO = '/api/v5/market/tickers'
 TICKER_INFO = '/api/v5/market/ticker'
 INDEX_TICKERS = '/api/v5/market/index-tickers'
 ORDER_BOOKS = '/api/v5/market/books'
@@ -84,14 +94,16 @@
 ORACLE = '/api/v5/market/open-oracle' #need to update? if it is open oracle
 INDEX_COMPONENTS = '/api/v5/market/index-components' #need to add
 EXCHANGE_RATE = '/api/v5/market/exchange-rate' #need to add
 HISTORY_TRADES = '/api/v5/market/history-trades' #need to add
 BLOCK_TICKERS = '/api/v5/market/block-tickers' #need to add
 BLOCK_TICKER = '/api/v5/market/block-ticker'#need to add
 BLOCK_TRADES = '/api/v5/market/block-trades'#need to add
+GET_ORDER_LITE_BOOK = '/api/v5/market/books-lite'
+GET_OPTION_TRADES = '/api/v5/market/option/instrument-family-trades'
 
 # Public Data-Complete-testComplete
 INSTRUMENT_INFO = '/api/v5/public/instruments'
 DELIVERY_EXERCISE = '/api/v5/public/delivery-exercise-history'
 OPEN_INTEREST = '/api/v5/public/open-interest'
 FUNDING_RATE = '/api/v5/public/funding-rate'
 FUNDING_RATE_HISTORY = '/api/v5/public/funding-rate-history'
@@ -104,14 +116,16 @@
 MARK_PRICE = '/api/v5/public/mark-price'
 TIER = '/api/v5/public/position-tiers'
 INTEREST_LOAN = '/api/v5/public/interest-rate-loan-quota' #need to add
 UNDERLYING = '/api/v5/public/underlying' #need to add
 VIP_INTEREST_RATE_LOAN_QUOTA = '/api/v5/public/vip-interest-rate-loan-quota' #need to add
 INSURANCE_FUND = '/api/v5/public/insurance-fund'#need to add
 CONVERT_CONTRACT_COIN = '/api/v5/public/convert-contract-coin' #need to add
+GET_OPTION_TICKBANDS = '/api/v5/public/instrument-tick-bands'
+GET_OPTION_TRADES = '/api/v5/public/option-trades'
 
 # TRADING DATA-COMPLETE
 SUPPORT_COIN = '/api/v5/rubik/stat/trading-data/support-coin'
 TAKER_VOLUME = '/api/v5/rubik/stat/taker-volume'
 MARGIN_LENDING_RATIO = '/api/v5/rubik/stat/margin/loan-ratio'
 LONG_SHORT_RATIO = '/api/v5/rubik/stat/contracts/long-short-account-ratio'
 CONTRACTS_INTEREST_VOLUME = '/api/v5/rubik/stat/contracts/open-interest-volume'
@@ -136,14 +150,16 @@
 ORDER_FILLS = '/api/v5/trade/fills'
 ORDERS_FILLS_HISTORY = '/api/v5/trade/fills-history'
 PLACE_ALGO_ORDER = '/api/v5/trade/order-algo'
 CANCEL_ALGOS = '/api/v5/trade/cancel-algos'
 Cancel_Advance_Algos = '/api/v5/trade/cancel-advance-algos'
 ORDERS_ALGO_OENDING = '/api/v5/trade/orders-algo-pending'
 ORDERS_ALGO_HISTORY = '/api/v5/trade/orders-algo-history'
+GET_ALGO_ORDER_DETAILS = '/api/v5/trade/order-algo'
+AMEND_ALGO_ORDER = '/api/v5/trade/amend-algos'
 
 EASY_CONVERT_CURRENCY_LIST = '/api/v5/trade/easy-convert-currency-list'
 EASY_CONVERT = '/api/v5/trade/easy-convert'
 CONVERT_EASY_HISTORY = '/api/v5/trade/easy-convert-history'
 ONE_CLICK_REPAY_SUPPORT = '/api/v5/trade/one-click-repay-currency-list'
 ONE_CLICK_REPAY = '/api/v5/trade/one-click-repay'
 ONE_CLICK_REPAY_HISTORY = '/api/v5/trade/one-click-repay-history'
@@ -154,14 +170,17 @@
 BILLs = '/api/v5/asset/subaccount/bills'
 RESET = '/api/v5/users/subaccount/modify-apikey'
 VIEW_LIST = '/api/v5/users/subaccount/list'
 SUBACCOUNT_TRANSFER = '/api/v5/asset/subaccount/transfer'
 ENTRUST_SUBACCOUNT_LIST = '/api/v5/users/entrust-subaccount-list' #need to add
 SET_TRSNSFER_OUT = '/api/v5/users/subaccount/set-transfer-out' #need to add
 GET_ASSET_SUBACCOUNT_BALANCE = '/api/v5/asset/subaccount/balances' #need to add
+GET_THE_USER_AFFILIATE_REBATE = '/api/v5/users/partner/if-rebate'
+SET_SUB_ACCOUNTS_VIP_LOAN = '/api/v5/account/subaccount/set-loan-allocation'
+GET_SUB_ACCOUNT_BORROW_INTEREST_AND_LIMIT = '/api/v5/account/subaccount/interest-limits'
 
 # Broker-all need to implmented-completed
 BROKER_INFO = '/api/v5/broker/nd/info'
 CREATE_SUBACCOUNT = '/api/v5/broker/nd/create-subaccount'
 DELETE_SUBACCOUNT = '/api/v5/broker/nd/delete-subaccount'
 SUBACCOUNT_INFO = '/api/v5/broker/nd/subaccount-info'
 SET_SUBACCOUNT_LEVEL = '/api/v5/broker/nd/set-subaccount-level'
@@ -218,18 +237,43 @@
 GRID_SUB_ORDERS = '/api/v5/tradingBot/grid/sub-orders'
 GRID_POSITIONS = '/api/v5/tradingBot/grid/positions'
 GRID_WITHDRAW_INCOME = '/api/v5/tradingBot/grid/withdraw-income'
 #--------need to add:
 GRID_COMPUTE_MARIGIN_BALANCE = '/api/v5/tradingBot/grid/compute-margin-balance'
 GRID_MARGIN_BALANCE = '/api/v5/tradingBot/grid/margin-balance'
 GRID_AI_PARAM = '/api/v5/tradingBot/grid/ai-param'
+PLACE_RECURRING_BUY_ORDER = '/api/v5/tradingBot/recurring/order-algo'
+AMEND_RECURRING_BUY_ORDER = '/api/v5/tradingBot/recurring/amend-order-algo'
+STOP_RECURRING_BUY_ORDER = '/api/v5/tradingBot/recurring/stop-order-algo'
+GET_RECURRING_BUY_ORDER_LIST = '/api/v5/tradingBot/recurring/orders-algo-pending'
+GET_RECURRING_BUY_ORDER_HISTORY = '/api/v5/tradingBot/recurring/orders-algo-history'
+GET_RECURRING_BUY_ORDER_DETAILS = '/api/v5/tradingBot/recurring/orders-algo-details'
+GET_RECURRING_BUY_SUB_ORDERS = '/api/v5/tradingBot/recurring/sub-orders'
 
 #stacking - all need to implement-testcomplete
 STACK_DEFI_OFFERS = '/api/v5/finance/staking-defi/offers'
 STACK_DEFI_PURCHASE = '/api/v5/finance/staking-defi/purchase'
 STACK_DEFI_REDEEM = '/api/v5/finance/staking-defi/redeem'
 STACK_DEFI_CANCEL = '/api/v5/finance/staking-defi/cancel'
 STACK_DEFI_ORDERS_ACTIVITY = '/api/v5/finance/staking-defi/orders-active'
 STACK_DEFI_ORDERS_HISTORY = '/api/v5/finance/staking-defi/orders-history'
+GET_SAVING_BALANCE = '/api/v5/finance/savings/balance'
+SAVING_PURCHASE_REDEMPTION = '/api/v5/finance/savings/purchase-redempt'
+SET_LENDING_RATE = '/api/v5/finance/savings/set-lending-rate'
+GET_LENDING_HISTORY = '/api/v5/finance/savings/lending-history'
+GET_PUBLIC_BORROW_INFO = '/api/v5/finance/savings/lending-rate-summary'
+GET_PUBLIC_BORROW_HISTORY = '/api/v5/finance/savings/lending-rate-history'
 
 # status-complete
 STATUS = '/api/v5/system/status'
+
+#Copy Trading
+GET_EXISTING_LEADING_POSITIONS = '/api/v5/copytrading/current-subpositions'
+GET_LEADING_POSITIONS_HISTORY = '/api/v5/copytrading/subpositions-history'
+PLACE_LEADING_STOP_ORDER = '/api/v5/copytrading/algo-order'
+CLOSE_LEADING_POSITIONS = '/api/v5/copytrading/close-subposition'
+GET_LEADING_POSITIONS = '/api/v5/copytrading/instruments'
+AMEND_EXISTING_LEADING_POSITIONS = '/api/v5/copytrading/set-instruments'
+GET_PROFIT_SHARING_DETAILS = '/api/v5/copytrading/profit-sharing-details'
+GET_TOTAL_PROFIT_SHARING = '/api/v5/copytrading/total-profit-sharing'
+GET_UNREALIZED_PROFIT_SHARING_DETAILS = '/api/v5/copytrading/unrealized-profit-sharing-details'
+
```

### Comparing `python-okx-0.1.9/okx/exceptions.py` & `python-okx-0.2.0/okx/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # coding=utf-8
 
 
 class OkxAPIException(Exception):
 
     def __init__(self, response):
-        print(response.text + ', ' + str(response.status_code))
         self.code = 0
         try:
             json_res = response.json()
         except ValueError:
             self.message = 'Invalid JSON error message from Okx: {}'.format(response.text)
         else:
             if "code" in json_res.keys() and "msg" in json_res.keys():
```

### Comparing `python-okx-0.1.9/okx/utils.py` & `python-okx-0.2.0/okx/utils.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/websocket/WsClientFactory.py` & `python-okx-0.2.0/okx/websocket/WsClientFactory.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/websocket/WsClientProtocol.py` & `python-okx-0.2.0/okx/websocket/WsClientProtocol.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/websocket/WsConnectManager.py` & `python-okx-0.2.0/okx/websocket/WsConnectManager.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/websocket/WsLoginFactory.py` & `python-okx-0.2.0/okx/websocket/WsLoginFactory.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/websocket/WsPrivate.py` & `python-okx-0.2.0/okx/websocket/WsPrivate.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/okx/websocket/WsUtils.py` & `python-okx-0.2.0/okx/websocket/WsUtils.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.1.9/python_okx.egg-info/PKG-INFO` & `python-okx-0.2.0/python_okx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python SDK for OKX
 Home-page: https://okx.com/docs-v5/
 Author: okxv5api
 Author-email: api@okg.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-okx-0.1.9/python_okx.egg-info/SOURCES.txt` & `python-okx-0.2.0/python_okx.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 okx/Account.py
 okx/BlockTrading.py
 okx/Convert.py
+okx/CopyTrading.py
 okx/Earning.py
 okx/FDBroker.py
 okx/Funding.py
 okx/Grid.py
 okx/MarketData.py
 okx/NDBroker.py
 okx/PublicData.py
```

### Comparing `python-okx-0.1.9/setup.py` & `python-okx-0.2.0/setup.py`

 * *Files identical despite different names*

