# Comparing `tmp/me_setups-1.8.5.tar.gz` & `tmp/me_setups-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.8.5.tar", last modified: Thu Jun 15 09:32:27 2023, max compression
+gzip compressed data, was "me_setups-1.9.0.tar", last modified: Mon Jun 19 10:37:28 2023, max compression
```

## Comparing `me_setups-1.8.5.tar` & `me_setups-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.425586 me_setups-1.8.5/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-15 09:32:27.425643 me_setups-1.8.5/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.5/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-15 09:32:27.428591 me_setups-1.8.5/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.5/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.372950 me_setups-1.8.5/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.387617 me_setups-1.8.5/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.5/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.410119 me_setups-1.8.5/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.5/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.5/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11657 2023-06-04 13:52:01.000000 me_setups-1.8.5/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.5/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.420883 me_setups-1.8.5/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.5/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8532 2023-06-15 09:29:46.000000 me_setups-1.8.5/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    12933 2023-06-04 13:52:01.000000 me_setups-1.8.5/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.5/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.5/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.8.5/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.398644 me_setups-1.8.5/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.087595 me_setups-1.9.0/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-19 10:37:28.087611 me_setups-1.9.0/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.9.0/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-19 10:37:28.089621 me_setups-1.9.0/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.9.0/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.051569 me_setups-1.9.0/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.061603 me_setups-1.9.0/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.9.0/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.079025 me_setups-1.9.0/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.9.0/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.9.0/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11767 2023-06-15 20:19:29.000000 me_setups-1.9.0/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.9.0/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.086234 me_setups-1.9.0/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.9.0/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8703 2023-06-19 10:33:52.000000 me_setups-1.9.0/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    14193 2023-06-15 20:19:29.000000 me_setups-1.9.0/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.9.0/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.9.0/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.9.0/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.070602 me_setups-1.9.0/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.8.5/PKG-INFO` & `me_setups-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.8.5
+Version: 1.9.0
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.5/setup.cfg` & `me_setups-1.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.8.5
+version = 1.9.0
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.8.5/src/me_setups/boards/default_boards.py` & `me_setups-1.9.0/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.5/src/me_setups/boards/gas52.py` & `me_setups-1.9.0/src/me_setups/boards/gas52.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,25 +175,33 @@
                 conn.serial.open()
 
     def restart_serials(self) -> None:
         """restart all serials conns, close and open"""
         self.close_serials()
         self.open_serials()
 
-    def run_ssh_cmd_all(self, cmd: str, **kwargs: Any) -> list[CompletedProcess[str]]:
+    def run_ssh_cmd_all(
+        self,
+        cmd: str,
+        *args: Any,
+        **kwargs: Any,
+    ) -> list[CompletedProcess[str]]:
         """run ssh command on all eqs.
 
         Args:
             cmd (str): the command to run
 
         Returns:
             list[CompletedProcess[str]]: list off all commands proccesses
         """
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
-            fs = [executor.submit(eq.run_ssh_cmd, cmd, **kwargs) for eq in self.eqs]
+            fs = [
+                executor.submit(eq.run_ssh_cmd, repr(cmd), *args, **kwargs)
+                for eq in self.eqs
+            ]
         return [f.result() for f in fs]
 
     def list_cores(self) -> dict[EyeQ5, list[str]]:
         """Returns all cores found on board.
 
         Returns:
             dict[EyeQ5, list[str]]: cores for each EQ.
```

### Comparing `me_setups-1.8.5/src/me_setups/components/comp.py` & `me_setups-1.9.0/src/me_setups/components/comp.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,18 @@
             bytes: all data that been read while waiting for the msg.
         """
         self.logger.debug(f"waiting for msg {msg.decode()!r}")
 
         restart_sniffing = False
         if self.serial.sniff_thread.alive.is_set():
             restart_sniffing = True
+            assert self.serial.protocol.log_file
+            log_file = self.serial.protocol.log_file
             self.serial.stop_sniffing()
+            self.serial.protocol.log_file = open(log_file.name, "a")
 
         with self.serial.change_timeout_ctx(timeout):
             if not self.serial.is_open:  # pragma: no cover
                 self.serial.open()
             res = self.serial.read_until(msg)
 
         if restart_sniffing:
```

### Comparing `me_setups-1.8.5/src/me_setups/components/eqs.py` & `me_setups-1.9.0/src/me_setups/components/eqs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import pathlib
 import re
+import shlex
 import subprocess
 import time
+from abc import ABC
 from enum import Enum
 from subprocess import CompletedProcess
 from typing import Any
 
 from me_setups.components.comp import Component
 
 
@@ -21,22 +23,70 @@
     UBOOT = "U-Boot"
     LINUX = "Linux"
 
 
 PCD_WRITE_COMPLETE = b"CAUTION P-COREDUMP TO  EMMC COMPLETE !!"
 FCD_WRITE_COMPLETE = b"OK"
 LINUX_BOOT_MSG = b"Welcome to EyeQ5"
-NO_KEY_CHECK = ["-o", "StrictHostKeyChecking=no", "-o", "LogLevel=FATAL"]
 PROMPTS = {
     OSType.LINUX: b"# ",
     OSType.VOIS: b"VOiS>>",
     OSType.UBOOT: b"EyeQ5 # ",
 }
 
 
+class Cmd(ABC):
+    NO_KEY_CHECK = "-o StrictHostKeyChecking=no -o LogLevel=FATAL"
+
+    def __init__(self, prefix: str, timeout: float) -> None:
+        self.prefix = f"{prefix} {self.NO_KEY_CHECK}"
+        self.timeout = timeout
+
+    def _run(self, cmd: str, *args: Any, **kwargs: Any) -> CompletedProcess[str]:
+        _cmd = shlex.split(f"{self.prefix} {cmd}")
+        return subprocess.run(
+            _cmd,
+            *args,
+            timeout=self.timeout,
+            capture_output=True,
+            text=True,
+            **kwargs,
+        )
+
+
+class SshCmd(Cmd):
+    def __init__(self, cmd: str, eq: str, timeout: float) -> None:
+        super().__init__("ssh", timeout)
+        self.prefix = f"{self.prefix} {eq}"
+        self.cmd = cmd
+
+    def run(self, *args: Any, **kwargs: Any) -> CompletedProcess[str]:
+        return self._run(self.cmd, *args, **kwargs)
+
+
+class ScpCmd(Cmd):
+    def __init__(
+        self,
+        src: str | pathlib.Path,
+        dst: str | pathlib.Path,
+        timeout: float,
+        recurcive: bool = False,
+    ) -> None:
+        super().__init__("scp", timeout)
+        self.src = src
+        self.dst = dst
+        self.recurcive = recurcive
+
+    def run(self, *args: Any, **kwargs: Any) -> CompletedProcess[str]:
+        cmd = f"{self.src} {self.dst}"
+        if self.recurcive:
+            cmd = f"-r {cmd}"
+        return self._run(cmd, *args, **kwargs)
+
+
 class EyeQ5(Component):
     crash_folder = pathlib.Path("/media/storage/crash")
 
     def __init__(
         self,
         pbcm: str,
         port: str,
@@ -120,14 +170,15 @@
     def copy_from(
         self,
         src: pathlib.Path | str,
         dst: pathlib.Path | str,
         timeout: float = 5,
         recurcive: bool = False,
         mkdir: bool = False,
+        *args: Any,
         **kwargs: Any,
     ) -> CompletedProcess[str]:
         """Copy files from EQ to local host
 
         Args:
             src (pathlib.Path | str): EQ path to the files
             dst (pathlib.Path | str): local path to copy to
@@ -140,24 +191,26 @@
         if mkdir:
             pathlib.Path(dst).mkdir(parents=True, exist_ok=True)
         return self._scp(
             f"{self._ssh_root}:{src}",
             str(dst),
             timeout,
             recurcive,
+            *args,
             **kwargs,
         )
 
     def copy_to(
         self,
         src: pathlib.Path | str,
         dst: pathlib.Path | str,
         timeout: float = 5,
         recurcive: bool = False,
         mkdir: bool = False,
+        *args: Any,
         **kwargs: Any,
     ) -> CompletedProcess[str]:
         """Copy files from local host to EQ
 
         Args:
             src (pathlib.Path | str): local path to the files
             dst (pathlib.Path | str): EQ path to copy to
@@ -171,14 +224,15 @@
         if mkdir:  # pragma: no cover
             self.run_ssh_cmd(f"mkdir -p {dst.parent}")
         return self._scp(
             str(src),
             f"{self._ssh_root}:{dst}",
             timeout,
             recurcive,
+            *args,
             **kwargs,
         )
 
     def copy_cores(
         self,
         dst: pathlib.Path | str,
         timeout: float = 180,
@@ -280,29 +334,49 @@
             frames=frames,
         )
 
     def run_ssh_cmd(
         self,
         cmd: str,
         timeout: float = 5,
+        skip_logging: bool = False,
+        verbose: bool = True,
+        *args: Any,
         **kwargs: Any,
     ) -> CompletedProcess[str]:
         """run ssh commad on EQ
 
         Args:
             cmd (str): the command to run
             timeout (float, optional): timeout for the command. Defaults to 5.
 
         Returns:
             CompletedProcess[str]: the command process
         """
-        assert self.os_type == OSType.LINUX
-        ssh_cmd = ["ssh"] + NO_KEY_CHECK + [self._ssh_root]
-        ssh_cmd.append(cmd)
-        return self._sp_cmd(ssh_cmd, timeout, **kwargs)
+        if self.os_type != OSType.LINUX:
+            raise RuntimeError("SSH command supported only on Linux")
+        if verbose:
+            self.logger.debug(f"[ssh] running cmd: {cmd!r}")
+        ssh_cmd = SshCmd(cmd, self._ssh_root, timeout)
+        try:
+            res = ssh_cmd.run(*args, **kwargs)
+        except subprocess.CalledProcessError as e:
+            self.logger.exception(e.stderr)
+            raise
+        if not skip_logging:
+            self.logger.debug(
+                "cmd result: ("
+                f"returncode={res.returncode}, "
+                f"stdout={res.stdout!r}, "
+                f"stderr={res.stderr!r})",
+            )
+        if verbose and res.returncode != 0:
+            self.logger.warning(f"cmd {cmd!r} return code is {res.returncode}")
+            self.logger.warning(f"cmd {cmd!r} stderr: {res.stderr!r}")
+        return res
 
     def path_exists(self, path: pathlib.Path | str) -> bool:
         """check if path exists on EQ
 
         Args:
             path (pathlib.Path | str): the path to check
 
@@ -375,62 +449,30 @@
             )
         return res
 
     def delete_crash_folder(self) -> CompletedProcess[str]:
         """Delete PCD and FCD crash folder"""
         return self.run_ssh_cmd(f"rm -rf {self.crash_folder}", timeout=20)
 
-    def _sp_cmd(
+    def _scp(
         self,
-        cmd: list[str],
-        timeout: float,
-        skip_logging: bool = False,
-        verbose: bool = True,
+        src: str | pathlib.Path,
+        dst: str | pathlib.Path,
+        timeout: float = 5,
+        recurcive: bool = False,
+        *args: Any,
         **kwargs: Any,
     ) -> CompletedProcess[str]:
-        str_cmd = " ".join(cmd)
-        if verbose:
-            self.logger.debug(f"[ssh] running cmd: {str_cmd!r}")
+        cmd = ScpCmd(src, dst, timeout, recurcive)
+        self.logger.debug(f"copy from: {src} to: {dst}")
         try:
-            res = subprocess.run(
-                cmd,
-                capture_output=True,
-                timeout=timeout,
-                text=True,
-                **kwargs,
-            )
+            return cmd.run(*args, **kwargs)
         except subprocess.CalledProcessError as e:
             self.logger.exception(e.stderr)
             raise
-        if not skip_logging:
-            self.logger.debug(
-                "cmd result: ("
-                f"returncode={res.returncode}, "
-                f"stdout={res.stdout!r}, "
-                f"stderr={res.stderr!r})",
-            )
-        if verbose and res.returncode != 0:
-            self.logger.warning(f"cmd {str_cmd!r} return code is {res.returncode}")
-            self.logger.warning(f"cmd {str_cmd!r} stderr: {res.stderr!r}")
-        return res
-
-    def _scp(
-        self,
-        _from: str,
-        _to: str,
-        timeout: float = 5,
-        recurcive: bool = False,
-        **kwargs: Any,
-    ) -> CompletedProcess[str]:
-        cmd = ["scp"] + NO_KEY_CHECK
-        if recurcive:
-            cmd += ["-r"]
-        cmd += [_from]
-        cmd += [_to]
-        return self._sp_cmd(cmd, timeout, **kwargs)
 
     def __str__(self) -> str:
         """name of the EQ in this format - 'EQ5_PBCM_<pbcm>'
 
         Returns:
             str: the name of the EQ
         """
```

### Comparing `me_setups-1.8.5/src/me_setups/components/mcu.py` & `me_setups-1.9.0/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.5/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.9.0/src/me_setups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.8.5
+Version: 1.9.0
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.5/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.9.0/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

