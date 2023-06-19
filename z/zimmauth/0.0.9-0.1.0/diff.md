# Comparing `tmp/zimmauth-0.0.9.tar.gz` & `tmp/zimmauth-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimmauth-0.0.9.tar", last modified: Sun May  7 10:30:17 2023, max compression
+gzip compressed data, was "zimmauth-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `zimmauth-0.0.9.tar` & `zimmauth-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      584 2023-05-07 10:30:11.134998 zimmauth-0.0.9/.github/workflows/test.yml
--rw-r--r--   0        0        0      566 2023-05-07 10:30:11.134998 zimmauth-0.0.9/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1770 2023-05-07 10:30:11.134998 zimmauth-0.0.9/.gitignore
--rw-r--r--   0        0        0     1056 2023-05-07 10:30:11.134998 zimmauth-0.0.9/LICENSE
--rw-r--r--   0        0        0      423 2023-05-07 10:30:11.134998 zimmauth-0.0.9/README.md
--rw-r--r--   0        0        0      711 2023-05-07 10:30:11.134998 zimmauth-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      150 2023-05-07 10:30:11.134998 zimmauth-0.0.9/zimmauth/__init__.py
--rw-r--r--   0        0        0     6437 2023-05-07 10:30:11.134998 zimmauth-0.0.9/zimmauth/core.py
--rw-r--r--   0        0        0      882 2023-05-07 10:30:11.134998 zimmauth-0.0.9/zimmauth/local_conn.py
--rw-r--r--   0        0        0     6496 2023-05-07 10:30:11.134998 zimmauth-0.0.9/zimmauth/test_core.py
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 zimmauth-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      584 2023-06-19 14:04:01.621125 zimmauth-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      566 2023-06-19 14:04:01.621125 zimmauth-0.1.0/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1770 2023-06-19 14:04:01.621125 zimmauth-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1056 2023-06-19 14:04:01.621125 zimmauth-0.1.0/LICENSE
+-rw-r--r--   0        0        0      423 2023-06-19 14:04:01.621125 zimmauth-0.1.0/README.md
+-rw-r--r--   0        0        0      718 2023-06-19 14:04:01.621125 zimmauth-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-19 14:04:01.621125 zimmauth-0.1.0/zimmauth/__init__.py
+-rw-r--r--   0        0        0     6761 2023-06-19 14:04:01.621125 zimmauth-0.1.0/zimmauth/core.py
+-rw-r--r--   0        0        0      882 2023-06-19 14:04:01.621125 zimmauth-0.1.0/zimmauth/local_conn.py
+-rw-r--r--   0        0        0     6562 2023-06-19 14:04:01.621125 zimmauth-0.1.0/zimmauth/test_core.py
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 zimmauth-0.1.0/PKG-INFO
```

### Comparing `zimmauth-0.0.9/.github/workflows/test.yml` & `zimmauth-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.9/.github/workflows/twine_release.yml` & `zimmauth-0.1.0/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.9/.gitignore` & `zimmauth-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.9/LICENSE` & `zimmauth-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.9/pyproject.toml` & `zimmauth-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [project.optional-dependencies]
 env = ["toml"]
 ssh = ["fabric", "decorator"]
 test = [
     "branthebuilder", 
     "mock-ssh-server", 
-    "dvc[s3,ssh]", 
+    "dvc[s3,ssh]>=3.1.0", 
     "moto", 
     "aiobotocore", 
     "boto3", 
     "fabric", 
     "toml", 
     "decorator"
 ]
```

### Comparing `zimmauth-0.0.9/zimmauth/core.py` & `zimmauth-0.1.0/zimmauth/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import secrets
+import sys
 from base64 import urlsafe_b64decode as b64d
 from base64 import urlsafe_b64encode as b64e
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from pathlib import Path
+from subprocess import check_call
 from tempfile import TemporaryDirectory
 from typing import Callable, Dict, Optional, Union
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.backends.openssl.backend import Backend
 from cryptography.hazmat.primitives import hashes
@@ -64,45 +66,50 @@
 
 
 @dataclass
 class S3Remote:
     bucket_name: str
     auth: S3Auth
 
-    def to_dvc_conf(self, _):
-        d = {
-            "url": f"s3://{self.bucket_name}",
-            "access_key_id": self.auth.key,
-            "secret_access_key": self.auth.secret,
-        }
-        if self.auth.endpoint:
-            d["endpointurl"] = self.auth.endpoint
-        return d
+    def get_dvc_string(self):
+        return f"s3://{self.bucket_name}"
+
+    def add_dvc_modifies(self, _):
+        for k, v in [
+            ("access_key_id", self.auth.key),
+            ("secret_access_key", self.auth.secret),
+            ("endpointurl", self.auth.endpoint),
+        ]:
+            if v:
+                yield k, v
 
 
 @dataclass
 class SSHRemote:
     host: str
     path: str = ""
     user: str = field(default_factory=os.getlogin)
-    port: Optional[int] = None
+    port: int | None = None
     rsa_key: Optional[str] = None
 
     def __repr__(self) -> str:
         return f"SSH: {self.host}:/{self.path}"
 
-    def to_dvc_conf(self, key_store: Path):
+    def get_dvc_string(self):
         if self.host in _get_local_names():
-            return {"url": self.path}
-        d = {"url": f"ssh://{self.host}{self.path}", "user": self.user}
-        if self.port:
-            d["port"] = self.port
+            return self.path
+        return f"ssh://{self.user}@{self.host}{self.path}"
+
+    def add_dvc_modifies(self, key_store: Path):
+        if self.host in _get_local_names():
+            return []
         if self.rsa_key:
-            d["keyfile"] = (key_store / self.rsa_key).as_posix()
-        return d
+            yield ("keyfile", (key_store / self.rsa_key).as_posix())
+        if self.port:
+            yield ("port", str(self.port))
 
 
 class ZimmAuth:
     def __init__(self, dic: dict) -> None:
         def _pop(key):
             return dic.pop(key, {})
 
@@ -149,22 +156,23 @@
                 port=ssh_rem.port,
                 connect_kwargs=c_kwargs,
             )
         with ctx.cd(ssh_rem.path):
             yield ctx
         tmp_dir.cleanup()
 
-    def dump_dvc(self, local=True, key_store=CONF_PATH):
-        from dvc.config import Config
+    def dump_dvc(self, local=True, key_store=CONF_PATH, executable=sys.executable):
+        for k, v in self._remotes.items():
+            runbase = [executable, "-m", "dvc", "remote"]
+            lflag = "--local" if local else "--global"
+            remstr = v.get_dvc_string()
+            check_call([*runbase, "add", lflag, "-f", k, remstr])
+            for mod_k, mod_v in v.add_dvc_modifies(key_store):
+                check_call([*runbase, "modify", lflag, k, mod_k, mod_v])
 
-        conf = Config(Path(".dvc"))
-        with conf.edit("local" if local else "global") as ced:
-            ced["remote"] = {
-                k: v.to_dvc_conf(key_store) for k, v in self._remotes.items()
-            }
         self._dump_keys(key_store)
 
     def get_boto_bucket(self, remote_name):
         import boto3
 
         s3_rem = self._s3_remotes[remote_name]
         auth = s3_rem.auth
```

### Comparing `zimmauth-0.0.9/zimmauth/local_conn.py` & `zimmauth-0.1.0/zimmauth/local_conn.py`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.9/zimmauth/test_core.py` & `zimmauth-0.1.0/zimmauth/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,19 @@
         repo = Repo()
         kp = Path("sg")
         kp.write_text("ABC")
         repo.add(kp.as_posix())
         repo.push([kp.as_posix()], remote="ssh-conn-1")
         # repo.push([kp.as_posix()], remote="bucket-1") TODO maybe this will work again
         repo.push([kp.as_posix()], remote="ssh-conn-3")
-        assert ["90"] == [f.name for f in far_file.parent.iterdir() if f != far_file]
+        assert ["90"] == [
+            f.name
+            for f in (far_file.parent / "files" / "md5").iterdir()
+            if f != far_file
+        ]
 
     finally:
         os.chdir(cwd)
 
 
 def test_boto(zauth: ZimmAuth, zauth_bucket: boto3, tmp_path: Path):
     bucket = zauth.get_boto_bucket("bucket-1")
```

### Comparing `zimmauth-0.0.9/PKG-INFO` & `zimmauth-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: zimmauth
-Version: 0.0.9
+Version: 0.1.0
 Summary: Authentication encryption and storage
 Author-email: Endre Márk Borza <endremborza@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
 Requires-Dist: branthebuilder[doc] ; extra == "doc"
 Requires-Dist: toml ; extra == "env"
 Requires-Dist: fabric ; extra == "ssh"
 Requires-Dist: decorator ; extra == "ssh"
 Requires-Dist: branthebuilder ; extra == "test"
 Requires-Dist: mock-ssh-server ; extra == "test"
-Requires-Dist: dvc[s3,ssh] ; extra == "test"
+Requires-Dist: dvc[s3,ssh]>=3.1.0 ; extra == "test"
 Requires-Dist: moto ; extra == "test"
 Requires-Dist: aiobotocore ; extra == "test"
 Requires-Dist: boto3 ; extra == "test"
 Requires-Dist: fabric ; extra == "test"
 Requires-Dist: toml ; extra == "test"
 Requires-Dist: decorator ; extra == "test"
 Project-URL: Homepage, https://github.com/endremborza/zimmauth
```

