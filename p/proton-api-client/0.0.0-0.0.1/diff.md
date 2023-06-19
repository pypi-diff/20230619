# Comparing `tmp/proton-api-client-0.0.0.tar.gz` & `tmp/proton-api-client-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-api-client-0.0.0.tar", last modified: Mon Jun 19 18:16:43 2023, max compression
+gzip compressed data, was "proton-api-client-0.0.1.tar", last modified: Mon Jun 19 18:24:01 2023, max compression
```

## Comparing `proton-api-client-0.0.0.tar` & `proton-api-client-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:16:43.726896 proton-api-client-0.0.0/
--rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.0/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)      408 2023-06-19 18:16:43.726896 proton-api-client-0.0.0/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      758 2023-06-19 18:12:16.000000 proton-api-client-0.0.0/README.md
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:16:43.726896 proton-api-client-0.0.0/proton/
--rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.0/proton/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9188 2023-06-19 17:57:18.000000 proton-api-client-0.0.0/proton/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4131 2023-06-17 23:49:57.000000 proton-api-client-0.0.0/proton/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4711 2023-06-19 17:57:55.000000 proton-api-client-0.0.0/proton/client.py
--rw-r--r--   0 x         (1000) x         (1000)     2134 2023-06-19 18:15:31.000000 proton-api-client-0.0.0/proton/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     2174 2023-06-19 17:57:18.000000 proton-api-client-0.0.0/proton/helpers.py
--rw-r--r--   0 x         (1000) x         (1000)     1537 2023-06-19 18:15:31.000000 proton-api-client-0.0.0/proton/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:16:43.726896 proton-api-client-0.0.0/proton_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)      408 2023-06-19 18:16:43.000000 proton-api-client-0.0.0/proton_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-19 18:16:43.000000 proton-api-client-0.0.0/proton_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-19 18:16:43.000000 proton-api-client-0.0.0/proton_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       59 2023-06-19 18:16:43.000000 proton-api-client-0.0.0/proton_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-19 18:16:43.000000 proton-api-client-0.0.0/proton_api_client.egg-info/top_level.txt
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-19 18:16:43.726896 proton-api-client-0.0.0/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)      788 2023-06-19 18:03:13.000000 proton-api-client-0.0.0/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:24:01.267434 proton-api-client-0.0.1/
+-rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.1/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)      408 2023-06-19 18:24:01.267434 proton-api-client-0.0.1/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      758 2023-06-19 18:12:16.000000 proton-api-client-0.0.1/README.md
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:24:01.267434 proton-api-client-0.0.1/proton/
+-rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.1/proton/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.1/proton/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     4077 2023-06-19 18:23:32.000000 proton-api-client-0.0.1/proton/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     4711 2023-06-19 17:57:55.000000 proton-api-client-0.0.1/proton/client.py
+-rw-r--r--   0 x         (1000) x         (1000)     2134 2023-06-19 18:15:31.000000 proton-api-client-0.0.1/proton/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     2174 2023-06-19 17:57:18.000000 proton-api-client-0.0.1/proton/helpers.py
+-rw-r--r--   0 x         (1000) x         (1000)     1537 2023-06-19 18:15:31.000000 proton-api-client-0.0.1/proton/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:24:01.267434 proton-api-client-0.0.1/proton_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)      408 2023-06-19 18:24:01.000000 proton-api-client-0.0.1/proton_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-19 18:24:01.000000 proton-api-client-0.0.1/proton_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-19 18:24:01.000000 proton-api-client-0.0.1/proton_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       59 2023-06-19 18:24:01.000000 proton-api-client-0.0.1/proton_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-19 18:24:01.000000 proton-api-client-0.0.1/proton_api_client.egg-info/top_level.txt
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-19 18:24:01.267434 proton-api-client-0.0.1/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)      788 2023-06-19 18:23:32.000000 proton-api-client-0.0.1/setup.py
```

### Comparing `proton-api-client-0.0.0/LICENSE` & `proton-api-client-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.0/README.md` & `proton-api-client-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.0/proton/_ctsrp.py` & `proton-api-client-0.0.1/proton/_ctsrp.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 x    Private key (derived from p and s)
 v    Password verifier
 """
 
 import ctypes
 import sys, os
 
-from .constants import  SRP_LEN_BYTES, SALT_LEN_BYTES
+from .constants import SRP_LEN_BYTES, SALT_LEN_BYTES
 from .helpers import pm_hash, hash_password
 
 dlls = []
-
 platform = sys.platform
 if platform == 'darwin':
     dlls.append(ctypes.cdll.LoadLibrary('libssl.dylib'))
 elif 'win' in platform:
     for d in ('libeay32.dll', 'libssl32.dll', 'ssleay32.dll'):
         try:
             dlls.append(ctypes.cdll.LoadLibrary(d))
@@ -149,17 +148,15 @@
     BN_bn2bin(N, bin2)  # noqa
     h.update(bin1)
     h.update(bin2[::-1])
     bytes_to_bn(dest, h.digest())
 
 
 def calculate_x(hash_class, dest, salt, password, modulus):
-    exp = hash_password(
-        hash_class, password, salt, bn_to_bytes(modulus, SRP_LEN_BYTES)
-    )
+    exp = hash_password(hash_class, password, salt, bn_to_bytes(modulus, SRP_LEN_BYTES))
     bytes_to_bn(dest, exp)
 
 
 def update_hash(h, n):
     h.update(bn_to_bytes(n, SRP_LEN_BYTES))
 
 
@@ -179,19 +176,17 @@
     return h.digest()
 
 
 def get_ngk(hash_class, n_bin, g_hex, ctx):
     N = new_bn()  # noqa
     g = new_bn()  # noqa
     k = new_bn()  # noqa
-
     bytes_to_bn(N, n_bin)
     BN_hex2bn(g, g_hex)  # noqa
     bn_hash_k(hash_class, k, g, N, SRP_LEN_BYTES)
-
     return N, g, k
 
 
 class User(object):
     def __init__(self, password, n_bin, g_hex=b"2", bytes_a=None, bytes_A=None):  # noqa
         if bytes_a and len(bytes_a) != 32:
             raise ValueError("32 bytes required for bytes_a")
@@ -256,64 +251,49 @@
 
     def get_session_key(self):
         return self.K if self._authenticated else None
 
     def get_challenge(self):
         return bn_to_bytes(self.A, SRP_LEN_BYTES)
 
-    # Returns M or None if SRP-6a safety check is violated
     def process_challenge(self, bytes_s, bytes_server_challenge):
+        """ Returns M or None if SRP-6a safety check is violated """
         self.bytes_s = bytes_s
         bytes_to_bn(self.B, bytes_server_challenge)
-
         # SRP-6a safety check
         if bn_is_zero(self.B):
             return None
-
         bn_hash(self.hash_class, self.u, self.A, self.B)
-
         # SRP-6a safety check
         if bn_is_zero(self.u):
             return None
-
         calculate_x(self.hash_class, self.x, self.bytes_s, self.password, self.N)
         BN_mod_exp(self.v, self.g, self.x, self.N, self.ctx)  # noqa
-
         # S = (B - k*(g^x)) ^ (a + ux)
         BN_mul(self.tmp1, self.u, self.x, self.ctx)  # noqa
         BN_add(self.tmp2, self.a, self.tmp1)  # noqa tmp2 = (a + ux)
         BN_mod_exp(self.tmp1, self.g, self.x, self.N, self.ctx)  # noqa
         BN_mul(self.tmp3, self.k, self.tmp1, self.ctx)  # noqa tmp3 = k*(g^x)
         BN_sub(self.tmp1, self.B, self.tmp3)  # noqa tmp1 = (B - K*(g^x))
         BN_mod_exp(self.S, self.tmp1, self.tmp2, self.N, self.ctx)  # noqa
-
         self.K = bn_to_bytes(self.S, SRP_LEN_BYTES)
-        self.M = calculate_client_challenge(
-            self.hash_class, self.A, self.B, self.K
-        )
-        self.expected_server_proof = calculate_server_challenge(
-            self.hash_class, self.A, self.M, self.K
-        )
-
+        self.M = calculate_client_challenge(self.hash_class, self.A, self.B, self.K)
+        self.expected_server_proof = calculate_server_challenge(self.hash_class, self.A, self.M, self.K)
         return self.M
 
     def verify_session(self, server_proof):
         if self.expected_server_proof == server_proof:
             self._authenticated = True
 
     def compute_v(self, bytes_s=None):
         if bytes_s is None:
             salt = new_bn()
             BN_rand(salt, 10 * 8, 0, 0)  # noqa
             self.bytes_s = bn_to_bytes(salt, SALT_LEN_BYTES)
         else:
             self.bytes_s = bytes_s
-
         calculate_x(self.hash_class, self.x, self.bytes_s, self.password, self.N)
         BN_mod_exp(self.v, self.g, self.x, self.N, self.ctx)  # noqa
         return self.bytes_s, bn_to_bytes(self.v, SRP_LEN_BYTES)
 
 
-# ---------------------------------------------------------
-# Init
-#
 RAND_seed(os.urandom(32), 32)  # noqa
```

### Comparing `proton-api-client-0.0.0/proton/_pysrp.py` & `proton-api-client-0.0.1/proton/_pysrp.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,48 +79,37 @@
 
     def get_session_key(self) -> bytes | None:
         return self.K if self._authenticated else None
 
     def get_challenge(self) -> bytes:
         return long_to_bytes(self.A, SRP_LEN_BYTES)
 
-    # Returns M or None if SRP-6a safety check is violated
+
     def process_challenge(self, bytes_s: bytes, bytes_server_challenge: bytes) -> bytes | None:
+        """ Returns M or None if SRP-6a safety check is violated """
         self.bytes_s = bytes_s
         self.B = bytes_to_long(bytes_server_challenge)
-
         # SRP-6a safety check
         if (self.B % self.N) == 0:
             return None
-
         self.u = custom_hash(self.hash_class, self.A, self.B)
-
         # SRP-6a safety check
         if self.u == 0:
             return None
-
         self.x = calc_x(self.hash_class, self.bytes_s, self.p, self.N)
-
         self.v = pow(self.g, self.x, self.N)
-
-        self.S = pow(
-            (self.B - self.k * self.v), (self.a + self.u * self.x), self.N
-        )
-
+        self.S = pow((self.B - self.k * self.v), (self.a + self.u * self.x), self.N)
         self.K = long_to_bytes(self.S, SRP_LEN_BYTES)
         self.M = calc_client_proof(self.hash_class, self.A, self.B, self.K)  # noqa
-        self.expected_server_proof = calc_server_proof(
-            self.hash_class, self.A, self.M, self.K
-        )
-
+        self.expected_server_proof = calc_server_proof(self.hash_class, self.A, self.M, self.K)
         return self.M
 
     def verify_session(self, server_proof: bytes) -> None:
         if self.expected_server_proof == server_proof:
             self._authenticated = True
 
     def compute_v(self, bytes_s: bytes = None) -> tuple[bytes, bytes]:
-        self.bytes_s = long_to_bytes(get_random_of_length(SALT_LEN_BYTES),
-                                     SALT_LEN_BYTES) if bytes_s is None else bytes_s
+        self.bytes_s = long_to_bytes(
+            get_random_of_length(SALT_LEN_BYTES),
+            SALT_LEN_BYTES) if bytes_s is None else bytes_s
         self.x = calc_x(self.hash_class, self.bytes_s, self.p, self.N)
-
         return self.bytes_s, long_to_bytes(pow(self.g, self.x, self.N), SRP_LEN_BYTES)
```

### Comparing `proton-api-client-0.0.0/proton/client.py` & `proton-api-client-0.0.1/proton/client.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.0/proton/constants.py` & `proton-api-client-0.0.1/proton/constants.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.0/proton/helpers.py` & `proton-api-client-0.0.1/proton/helpers.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.0/proton/login.py` & `proton-api-client-0.0.1/proton/login.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.0/setup.py` & `proton-api-client-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'orjson',
     'httpx',
     'tqdm',
 ]
 
 setup(
     name='proton-api-client',
-    version='0.0.0',
+    version='0.0.1',
     python_requires='>=3.10.10',
     description='Proton Mail API',
     long_description=dedent('''
     
     ### Proton Mail API
     
     '''),
```

