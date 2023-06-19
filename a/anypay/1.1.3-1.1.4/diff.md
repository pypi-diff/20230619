# Comparing `tmp/anypay-1.1.3.tar.gz` & `tmp/anypay-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anypay-1.1.3.tar", last modified: Wed May 10 13:15:13 2023, max compression
+gzip compressed data, was "anypay-1.1.4.tar", last modified: Mon Jun 19 21:26:16 2023, max compression
```

## Comparing `anypay-1.1.3.tar` & `anypay-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-10 13:15:13.296982 anypay-1.1.3/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1210 2023-02-01 21:00:44.000000 anypay-1.1.3/LICENSE
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2817 2023-05-10 13:15:13.296982 anypay-1.1.3/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2051 2023-03-30 17:49:45.000000 anypay-1.1.3/README.md
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-10 13:15:13.296982 anypay-1.1.3/anypay/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      245 2023-02-01 20:28:21.000000 anypay-1.1.3/anypay/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)    15585 2023-05-10 13:13:50.000000 anypay-1.1.3/anypay/api.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      612 2023-03-30 10:03:25.000000 anypay-1.1.3/anypay/exceptions.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-10 13:15:13.296982 anypay-1.1.3/anypay/models/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      174 2023-02-01 20:20:14.000000 anypay-1.1.3/anypay/models/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      408 2023-03-30 10:02:29.000000 anypay-1.1.3/anypay/models/bill.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      547 2023-03-30 10:02:12.000000 anypay-1.1.3/anypay/models/payment.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      660 2023-03-30 10:02:48.000000 anypay-1.1.3/anypay/models/payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      229 2023-02-04 08:28:53.000000 anypay-1.1.3/anypay/models/rates.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-10 13:15:13.296982 anypay-1.1.3/anypay.egg-info/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2817 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      349 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/SOURCES.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/dependency_links.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       15 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/requires.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        7 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/top_level.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-05-10 13:15:13.296982 anypay-1.1.3/setup.cfg
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1242 2023-05-10 13:14:24.000000 anypay-1.1.3/setup.py
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-19 21:26:16.453138 anypay-1.1.4/
+-rw-r--r--   0 bifle     (1000) bifle     (1000)     1210 2023-06-19 21:15:54.000000 anypay-1.1.4/LICENSE
+-rw-r--r--   0 bifle     (1000) bifle     (1000)     2817 2023-06-19 21:26:16.453138 anypay-1.1.4/PKG-INFO
+-rw-r--r--   0 bifle     (1000) bifle     (1000)     2051 2023-06-19 21:15:54.000000 anypay-1.1.4/README.md
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-19 21:26:16.453138 anypay-1.1.4/anypay/
+-rw-r--r--   0 bifle     (1000) bifle     (1000)      245 2023-06-19 21:15:54.000000 anypay-1.1.4/anypay/__init__.py
+-rw-r--r--   0 bifle     (1000) bifle     (1000)    15449 2023-06-19 21:22:43.000000 anypay-1.1.4/anypay/api.py
+-rw-r--r--   0 bifle     (1000) bifle     (1000)      592 2023-06-19 21:23:31.000000 anypay-1.1.4/anypay/exceptions.py
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-19 21:26:16.453138 anypay-1.1.4/anypay/models/
+-rw-r--r--   0 bifle     (1000) bifle     (1000)      174 2023-06-19 21:15:54.000000 anypay-1.1.4/anypay/models/__init__.py
+-rw-r--r--   0 bifle     (1000) bifle     (1000)      408 2023-06-19 21:15:54.000000 anypay-1.1.4/anypay/models/bill.py
+-rw-r--r--   0 bifle     (1000) bifle     (1000)      547 2023-06-19 21:15:54.000000 anypay-1.1.4/anypay/models/payment.py
+-rw-r--r--   0 bifle     (1000) bifle     (1000)      660 2023-06-19 21:15:54.000000 anypay-1.1.4/anypay/models/payout.py
+-rw-r--r--   0 bifle     (1000) bifle     (1000)      229 2023-06-19 21:15:54.000000 anypay-1.1.4/anypay/models/rates.py
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-19 21:26:16.453138 anypay-1.1.4/anypay.egg-info/
+-rw-r--r--   0 bifle     (1000) bifle     (1000)     2817 2023-06-19 21:26:16.000000 anypay-1.1.4/anypay.egg-info/PKG-INFO
+-rw-r--r--   0 bifle     (1000) bifle     (1000)      349 2023-06-19 21:26:16.000000 anypay-1.1.4/anypay.egg-info/SOURCES.txt
+-rw-r--r--   0 bifle     (1000) bifle     (1000)        1 2023-06-19 21:26:16.000000 anypay-1.1.4/anypay.egg-info/dependency_links.txt
+-rw-r--r--   0 bifle     (1000) bifle     (1000)       15 2023-06-19 21:26:16.000000 anypay-1.1.4/anypay.egg-info/requires.txt
+-rw-r--r--   0 bifle     (1000) bifle     (1000)        7 2023-06-19 21:26:16.000000 anypay-1.1.4/anypay.egg-info/top_level.txt
+-rw-r--r--   0 bifle     (1000) bifle     (1000)       38 2023-06-19 21:26:16.456472 anypay-1.1.4/setup.cfg
+-rw-r--r--   0 bifle     (1000) bifle     (1000)     1242 2023-06-19 21:24:30.000000 anypay-1.1.4/setup.py
```

### Comparing `anypay-1.1.3/LICENSE` & `anypay-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anypay-1.1.3/PKG-INFO` & `anypay-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anypay
-Version: 1.1.3
+Version: 1.1.4
 Summary: Asynchronous AnyPay API wrapper
 Home-page: https://github.com/nikitalm8/anypay
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/anypay
 Project-URL: Bug Tracker, https://github.com/nikitalm8/anypay/issues
 Project-URL: API Docs, https://anypay.io/doc/api
```

### Comparing `anypay-1.1.3/README.md` & `anypay-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `anypay-1.1.3/anypay/api.py` & `anypay-1.1.4/anypay/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-import httpx
 import hashlib
+import httpx
 
-from .models import (
-    Bill, 
-    Payment, 
-    Payout, 
-    Rates,
-)
-from .exceptions import AnyPayAPIError
+from typing import List, Optional, Union
 
-from typing import Union, Optional, List
+from .exceptions import AnyPayAPIError
+from .models import Bill, Payment, Payout, Rates
 
 
 class AnyPayAPI(object):
     """
     AnyPay API wrapper.
     Docs: https://anypay.io/doc/api
     """
@@ -22,33 +17,33 @@
     HEADERS = {
         'Accept': 'application/json',
         'Content-Type': 'multipart/form-data',
     }
 
 
     def __init__(
-        self, 
-        api_id: str, 
-        api_key: str, 
-        project_id: Optional[int]=None, 
+        self,
+        api_id: str,
+        api_key: str,
+        project_id: Optional[int]=None,
         project_secret: Optional[str]=None,
         use_md5: bool=False,
         check: bool=True,
     ):
         """
         Initialize AnyPay API wrapper.
 
         :param api_id: API ID, can be found in your profile settings.
         :param api_key: API Key, can be found in your profile settings.
         :param project_id: Project ID, can be found in your project settings.
         :param project_secret: Project Secret, can be found in your project settings. Add it if you need to use SCI.
         :param use_md5: Use MD5 signature instead of SHA256 (change to MD5 in settings).
         :param check: Disable API ID and API Key check.
 
-        :raises: AnyPayAPIError if API ID or API Key is invalid. 
+        :raises: AnyPayAPIError if API ID or API Key is invalid.
         """
 
         self.api_id = api_id
         self.api_key = api_key
 
         self.project_id = project_id
         self.project_secret = project_secret
@@ -73,17 +68,17 @@
 
         :return: Encoded signature string.
         """
 
         encryption_method = hashlib.sha256 if not use_md5 else hashlib.md5
         signature = encryption_method(
             (
-                method 
-                + self.api_id 
-                + template % params 
+                method
+                + self.api_id
+                + template % params
                 + self.api_key
             ).encode('utf-8'),
         )
 
         return signature.hexdigest()
 
 
@@ -183,63 +178,63 @@
         :return: Balance.
         :raises: AnyPayAPIError
         """
 
         result = await self._make_request_async('balance')
         return result['balance']
 
-    
+
     @property
     def balance(self) -> Union[float, int]:
         """
         Get balance.
         Docs: https://anypay.io/doc/api/balance
-        
+
         :return: Balance.
         :raises: AnyPayAPIError
         """
 
         result = self._make_request('balance')
         return result['balance']
 
 
     async def get_convertion_rates(self) -> Rates:
         """
         Get convertion rates.
         Docs: https://anypay.io/doc/api/rates
-        
+
         :return: Rates object.
         :raises: AnyPayAPIError
         """
 
         result = await self._make_request_async('rates')
         return Rates(**result)
 
 
     @property
     def convertion_rates(self) -> Rates:
         """
         Get convertion rates from property. Synchronous.
         Docs: https://anypay.io/doc/api/rates
-        
+
         :return: Rates object.
         :raises: AnyPayAPIError
         """
 
 
         result = self._make_request('rates')
         return Rates(**result)
 
 
     async def get_commissions(self, project_id: Optional[int]=None) -> dict:
         """
         Get commissions.
         Docs: https://anypay.io/doc/api/commissions
-         
-        :param project_id: Project ID, can be found in your project settings.  
+
+        :param project_id: Project ID, can be found in your project settings.
 
         :return: Commissions object.
         :raises: AnyPayAPIError
         """
 
         result = await self._make_request_async(
             'commissions',
@@ -250,29 +245,29 @@
 
 
     @property
     def commissions(self) -> dict:
         """
         Get commissions from property. Synchronous.
         Docs: https://anypay.io/doc/api/commissions
-        
+
         :return: Commissions object.
         :raises: AnyPayAPIError
         """
 
         result = self._make_request(
             'commissions',
             '%(project_id)s',
             project_id=self.project_id,
         )
         return result
 
 
     async def create_payment(
-        self, 
+        self,
         pay_id: int,
         amount: float,
         email: str,
         method: str,
         project_id: Optional[int] = None,
         currency: str='RUB',
         desc: str='',
@@ -280,38 +275,38 @@
         phone: Optional[str]=None,
         tail: Optional[str]=None,
         success_url: Optional[str]=None,
         fail_url: Optional[str]=None,
         lang: Optional[str]=None,
     ) -> Bill:
         """
-        Create a payout.
+        Create a bill.
         Docs: https://anypay.io/doc/api/create-payment
-        
+
         :param pay_id: Payment ID.
         :param amount: Payment amount.
         :param email: User email.
         :param method: Payment method.
         :param project_id: Project ID.
         :param currency: Payment currency.
         :param desc: Payment description.
         :param method_currency: Payment method currency.
         :param phone: User phone.
         :param tail: Payment tail (for `card` payment method).
         :param success_url: Success URL.
         :param fail_url: Fail URL.
         :param lang: Bill page language.
-        
-        :return: Payout object.
+
+        :return: Bill object.
         :raises: AnyPayAPIError
         """
 
         result = await self._make_request_async(
             'create-payment',
-            '%(project_id)s%(amount)s%(currency)s%(desc)s%(method)s',
+            '%(project_id)s%(pay_id)s%(amount)s%(currency)s%(desc)s%(method)s',
             project_id=project_id or self.project_id,
             pay_id=pay_id,
             amount=amount,
             currency=currency,
             desc=desc,
             method=method,
             method_currency=method_currency,
@@ -331,15 +326,15 @@
         transaction_id: Optional[int]=None,
         pay_id: Optional[int]=None,
         offset: int=0,
     ) -> List[Payment]:
         """
         Get payments.
         Docs: https://anypay.io/doc/api/payments
-        
+
         :param project_id: Project ID, can be found in your project settings.
         :param transaction_id: Transaction ID.
         :param pay_id: Payment ID.
         :param offset: Offset (defaults to 0).
 
         :return: List of Payment objects.
         :raises: AnyPayAPIError
@@ -370,23 +365,23 @@
         wallet_currency: Optional[str]=None,
         commission_type: Optional[str]=None,
         status_url: Optional[str]=None,
     ) -> Payout:
         """
         Create a payout.
         Docs: https://anypay.io/doc/api/create-payout
-        
+
         :param payout_id: Payout ID.
         :param payout_type: Payout type (qiwi, ym, ...).
         :param amount: Amount.
         :param wallet: Wallet number.
         :param wallet_currency: Wallet currency (defaults to RUB).
         :param commission_type: From where to deduct the commission (payment or balance).
         :param status_url: Status URL (Optional).
-        
+
         :return: Payout object.
         :raises: AnyPayAPIError
         """
 
         result = await self._make_request_async(
             'create-payout',
             '%(payout_id)s%(payout_type)s%(amount)s%(wallet)s',
@@ -407,15 +402,15 @@
         transaction_id: Optional[int]=None,
         payout_id: Optional[int]=None,
         offset: int=0,
     ) -> List[Payout]:
         """
         Get payouts.
         Docs: https://anypay.io/doc/api/payouts
-        
+
         :param transaction_id: Transaction ID.
         :param payout_id: Payout ID.
         :param offset: Offset (defaults to 0).
 
         :return: List of Payout objects.
         :raises: AnyPayAPIError
         """
@@ -425,15 +420,15 @@
             transaction_id=transaction_id,
             payout_id=payout_id,
             offset=offset,
         )
 
         return [
             Payout(**payout)
-            for payout 
+            for payout
             in result['payouts'].values()
         ] if result['payouts'] else []
 
 
     async def get_service_ip(self) -> List[str]:
         """
         Get service IPs.
@@ -456,15 +451,15 @@
         :raises: AnyPayAPIError
         """
 
         return self._make_request('ip-notification')
 
 
     async def create_bill(
-        self, 
+        self,
         pay_id: int,
         amount: Union[int, float],
         project_id: Optional[int]=None,
         project_secret: Optional[str]=None,
         currency: str='RUB',
         description: str='Payment',
         method: Optional[str]=None,
@@ -475,15 +470,15 @@
         lang: Optional[str]=None,
         use_md5: bool=True,
         **kwargs,
     ) -> Bill:
         """
         Create a bill via eased up SCI methods (only pay_id, amount, project_id and project_secret are required).
         Note that this method does not raise an exception if the credentials are incorrect, the exception is show to user on the bill's page.
-        
+
         Docs: https://anypay.io/doc/sci/
 
         :param pay_id: Payment ID.
         :param amount: Payment amount.
         :param project_id: Project ID, can be added in __init__.
         :param project_secret: Project secret key, can be added in __init__.
         :param currency: Payment currency.
@@ -494,15 +489,15 @@
         :param success_url: Success URL.
         :param fail_url: Fail URL.
         :param lang: Bill page language.
         :param use_md5: Use MD5 (defaults to True).
 
         :return: Bill object.
         """
-    
+
         if use_md5:
 
             singature_string = '%s:%s:%s:%s:%s' % (
                 currency,
                 amount,
                 project_secret or self.project_secret,
                 project_id or self.project_id,
```

### Comparing `anypay-1.1.3/anypay/exceptions.py` & `anypay-1.1.4/anypay/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 class AnyPayAPIError(Exception):
     """
     Base AnyPay Exception.
     Exception codes and their meanings can be found here: https://anypay.io/doc/api/errors
     """
-    
+
     def __init__(self, exception: dict):
         """
         AnyPay API Exception.
         Docs: https://anypay.io/doc/api/errors
-        
+
         :param exception: Exception data (code and message).
-        
+
         :raises: AnyPayAPIError
         """
 
         self.message = exception['message']
         self.code = exception['code']
 
         super().__init__(
```

### Comparing `anypay-1.1.3/anypay/models/payment.py` & `anypay-1.1.4/anypay/models/payment.py`

 * *Files identical despite different names*

### Comparing `anypay-1.1.3/anypay/models/payout.py` & `anypay-1.1.4/anypay/models/payout.py`

 * *Files identical despite different names*

### Comparing `anypay-1.1.3/anypay.egg-info/PKG-INFO` & `anypay-1.1.4/anypay.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anypay
-Version: 1.1.3
+Version: 1.1.4
 Summary: Asynchronous AnyPay API wrapper
 Home-page: https://github.com/nikitalm8/anypay
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/anypay
 Project-URL: Bug Tracker, https://github.com/nikitalm8/anypay/issues
 Project-URL: API Docs, https://anypay.io/doc/api
```

### Comparing `anypay-1.1.3/setup.py` & `anypay-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as file:
 
     long_description = "\n" + file.read()
 
-VERSION = '1.1.3'
+VERSION = '1.1.4'
 DESCRIPTION = 'Asynchronous AnyPay API wrapper'
 
 setup(
     name="anypay",
     version=VERSION,
     author="Nikita Minaev",
     author_email="<nikita@minaev.su>",
```

