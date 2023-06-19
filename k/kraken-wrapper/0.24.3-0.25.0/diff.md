# Comparing `tmp/kraken_wrapper-0.24.3.tar.gz` & `tmp/kraken_wrapper-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.24.3.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.25.0.tar", max compression
```

## Comparing `kraken_wrapper-0.24.3.tar` & `kraken_wrapper-0.25.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      988 2023-06-19 15:04:27.394706 kraken_wrapper-0.24.3/LICENSE
--rw-r--r--   0        0        0      433 2023-06-19 15:04:27.394804 kraken_wrapper-0.24.3/README.md
--rw-r--r--   0        0        0     1746 2023-06-19 15:05:59.420726 kraken_wrapper-0.24.3/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-19 15:05:59.420819 kraken_wrapper-0.24.3/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     3637 2023-06-19 15:04:27.395437 kraken_wrapper-0.24.3/src/kraken/wrapper/_buildend_venv.py
--rw-r--r--   0        0        0     3374 2023-06-19 15:04:27.395562 kraken_wrapper-0.24.3/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     5311 2023-06-19 15:04:27.395699 kraken_wrapper-0.24.3/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     3674 2023-06-19 15:04:27.395839 kraken_wrapper-0.24.3/src/kraken/wrapper/_buildenv_pex.py
--rw-r--r--   0        0        0     3175 2023-06-19 15:04:27.395947 kraken_wrapper-0.24.3/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4605 2023-06-19 15:04:27.396063 kraken_wrapper-0.24.3/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     3564 2023-06-19 15:04:27.396222 kraken_wrapper-0.24.3/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0     4222 2023-06-19 15:04:27.396714 kraken_wrapper-0.24.3/src/kraken/wrapper/_pex.py
--rw-r--r--   0        0        0    15754 2023-06-19 15:04:27.396949 kraken_wrapper-0.24.3/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2023-06-19 15:04:27.397039 kraken_wrapper-0.24.3/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 kraken_wrapper-0.24.3/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/LICENSE
+-rw-r--r--   0        0        0      433 2023-06-19 14:25:27.366905 kraken_wrapper-0.25.0/README.md
+-rw-r--r--   0        0        0     2174 2023-06-19 15:38:30.030178 kraken_wrapper-0.25.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-19 15:38:30.030178 kraken_wrapper-0.25.0/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     6258 2023-06-19 15:38:25.250142 kraken_wrapper-0.25.0/src/kraken/wrapper/_buildend_venv.py
+-rw-r--r--   0        0        0     3374 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     5311 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     3674 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv_pex.py
+-rw-r--r--   0        0        0     3250 2023-06-19 15:38:25.250142 kraken_wrapper-0.25.0/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4605 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     3564 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0     4222 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_pex.py
+-rw-r--r--   0        0        0    16230 2023-06-19 15:38:25.250142 kraken_wrapper-0.25.0/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 kraken_wrapper-0.25.0/PKG-INFO
```

### Comparing `kraken_wrapper-0.24.3/LICENSE` & `kraken_wrapper-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.3/pyproject.toml` & `kraken_wrapper-0.25.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.24.3"
+version = "0.25.0"
 description = ""
 authors = ["Unknown <me@unknown.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/wrapper", from = "src" }]
 classifiers = []
 keywords = []
@@ -18,18 +18,25 @@
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 keyring = "^23.8.2"
-kraken-common = "^0.24.3"
+kraken-common = "^0.25.0"
 pex = "^2.1.103"
 setuptools = ">=33.0.0"  # For pkg_resources
 termcolor = "^1.1.0"
+rich = "^13.4.2"
+
+# NOTE(@NiklasRosenstein): Need to pin transitive dependency markdown-it under 3.0 because it dropped Python 3.9
+#       support after that version. Technically this shouldn't be a big issue for runtime, but Mypy checks site
+#       packages and complains about the walrus operator used in it when it checks site-packages.
+#       See also https://github.com/python/mypy/issues/12162
+markdown-it-py = "<3.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 pytest = "*"
```

### Comparing `kraken_wrapper-0.24.3/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.3/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.3/src/kraken/wrapper/_buildenv_pex.py` & `kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.3/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.25.0/src/kraken/wrapper/_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+import os
 from pathlib import Path
 from typing import Any, MutableMapping, NamedTuple
 
 import keyring
 import keyring.backends.fail
 
 logger = logging.getLogger(__name__)
@@ -23,15 +24,17 @@
     class Credentials(NamedTuple):
         username: str
         password: str
 
     def __init__(self, config: MutableMapping[str, Any], path: Path) -> None:
         self._config = config
         self._path = path
-        self._has_keyring = not isinstance(keyring.get_keyring(), keyring.backends.fail.Keyring)
+        self._has_keyring = os.getenv("KRAKENW_NO_KEYRING") != "1" and not isinstance(
+            keyring.get_keyring(), keyring.backends.fail.Keyring
+        )
 
     def get_credentials(self, host: str) -> Credentials | None:
         auth = self._config.get("auth", {})
         if host not in auth:
             return None
         username = auth[host].get("username")
         if not username:
```

### Comparing `kraken_wrapper-0.24.3/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.25.0/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.3/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.25.0/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.3/src/kraken/wrapper/_pex.py` & `kraken_wrapper-0.25.0/src/kraken/wrapper/_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.24.3/src/kraken/wrapper/main.py` & `kraken_wrapper-0.25.0/src/kraken/wrapper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from ._config import DEFAULT_CONFIG_PATH, AuthModel
 from ._lockfile import Lockfile, calculate_lockfile
 from ._option_sets import AuthOptions, EnvOptions
 
 BUILDENV_PATH = Path("build/.kraken/venv")
 BUILDSCRIPT_FILENAME = ".kraken.py"
 BUILD_SUPPORT_DIRECTORY = "build-support"
-DEFAULT_INTERPRETER_CONSTRAINT = ">=3.7"
 LOCK_FILENAME = ".kraken.lock"
 _FormatterClass = lambda prog: argparse.RawTextHelpFormatter(prog, max_help_position=60, width=120)  # noqa: 731
 logger = logging.getLogger(__name__)
 print = partial(builtins.print, "[krakenw]", flush=True)
 eprint = partial(print, file=sys.stderr)
 
 
@@ -71,15 +70,15 @@
     parser.add_argument("-V", "--version", version=__version__, action="version")
     LoggingOptions.add_to_parser(parser)
     EnvOptions.add_to_parser(parser)
 
     # NOTE (@NiklasRosenstein): If we combine "+" with remainder, we get options passed after the `cmd`
     #       passed directly into `args` without argparse treating it like an option. This is not the case
     #       when using `nargs=1` for `cmd`.
-    parser.add_argument("cmd", nargs="*", metavar="cmd", help="{a,auth,lock,l} or a kraken command")
+    parser.add_argument("cmd", nargs="*", metavar="cmd", help="{auth,list-pythons,lock} or a kraken command")
     parser.add_argument("args", nargs=argparse.REMAINDER, help="additional arguments")
     return parser
 
 
 def _get_lock_argument_parser(prog: str) -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         prog,
@@ -176,14 +175,28 @@
     else:
         parser.print_usage()
         sys.exit(1)
 
     sys.exit(0)
 
 
+def list_pythons(prog: str, argv: list[str]) -> NoReturn:
+    import rich
+    from kraken.common import findpython
+
+    if argv:
+        eprint(f"{prog}: error: unexpected arguments")
+        sys.exit(1)
+
+    interpreters = findpython.evaluate_candidates(findpython.get_candidates(), findpython.InterpreterVersionCache())
+    table = findpython.build_rich_table(interpreters)
+    rich.print(table)
+    sys.exit(0)
+
+
 def _print_env_status(manager: BuildEnvManager, project: Project) -> None:
     """Print the status of the environent as a nicely formatted table."""
 
     hash_algorithm = manager.get_hash_algorithm()
 
     table = AsciiTable()
     table.headers = ["Key", "Source", "Value"]
@@ -368,14 +381,17 @@
     cmd: str | None = args.cmd[0] if args.cmd else None
     argv: list[str] = args.cmd[1:] + args.args
 
     if cmd in ("a", "auth"):
         # The `auth` comand does not require any current project information, it can be used globally.
         auth(f"{parser.prog} auth", argv)
 
+    if cmd in ("list-pythons",):
+        list_pythons(f"{parser.prog} list-pythons", argv)
+
     # The project details and build environment manager are relevant for any command that we are delegating.
     # This includes the built-in `lock` command.
     config = TomlConfigFile(DEFAULT_CONFIG_PATH)
     project = load_project(Path.cwd(), outdated_check=not env_options.upgrade)
     manager = BuildEnvManager(project.directory / BUILDENV_PATH, AuthModel(config, DEFAULT_CONFIG_PATH))
 
     # Execute environment operations before delegating the command.
```

### Comparing `kraken_wrapper-0.24.3/PKG-INFO` & `kraken_wrapper-0.25.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.24.3
+Version: 0.25.0
 Summary: 
 License: MIT
 Author: Unknown
 Author-email: me@unknown.org
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keyring (>=23.8.2,<24.0.0)
-Requires-Dist: kraken-common (>=0.24.3,<0.25.0)
+Requires-Dist: kraken-common (>=0.25.0,<0.26.0)
+Requires-Dist: markdown-it-py (<3.0.0)
 Requires-Dist: pex (>=2.1.103,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: setuptools (>=33.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
 Project-URL: Homepage, https://kraken-build.github.io/kraken-build/
 Project-URL: Repository, https://github.com/kraken-build/kraken-build/
 Description-Content-Type: text/markdown
```

