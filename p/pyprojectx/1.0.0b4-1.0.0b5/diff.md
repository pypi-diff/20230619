# Comparing `tmp/pyprojectx-1.0.0b4.tar.gz` & `tmp/pyprojectx-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectx-1.0.0b4.tar", last modified: Sun May  7 12:42:55 2023, max compression
+gzip compressed data, was "pyprojectx-1.0.0b5.tar", last modified: Mon Jun 19 06:54:04 2023, max compression
```

## Comparing `pyprojectx-1.0.0b4.tar` & `pyprojectx-1.0.0b5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1071 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/LICENSE
--rw-r--r--   0        0        0     4600 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/README.md
--rw-r--r--   0        0        0     4217 2023-05-07 12:42:55.060940 pyprojectx-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/__init__.py
--rw-r--r--   0        0        0     5041 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/cli.py
--rw-r--r--   0        0        0     6377 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/config.py
--rw-r--r--   0        0        0     5471 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/env.py
--rw-r--r--   0        0        0        0 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/__init__.py
--rw-r--r--   0        0        0      348 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/global-template.toml
--rw-r--r--   0        0        0     7263 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/initializers.py
--rw-r--r--   0        0        0      839 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/pdm-template.toml
--rw-r--r--   0        0        0      858 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/poetry-template.toml
--rw-r--r--   0        0        0       32 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/poetry.toml
--rw-r--r--   0        0        0      863 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/project-template.toml
--rw-r--r--   0        0        0      303 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/log.py
--rw-r--r--   0        0        0        0 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/__init__.py
--rw-r--r--   0        0        0       30 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pw.bat
--rwxr-xr-x   0        0        0     5949 2023-05-07 12:41:03.159443 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pw.py
--rwxr-xr-x   0        0        0      253 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/px
--rw-r--r--   0        0        0      373 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/px.bat
--rwxr-xr-x   0        0        0      275 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pxg
--rw-r--r--   0        0        0      270 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pxg.bat
--rw-r--r--   0        0        0        0 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/__init__.py
--rw-r--r--   0        0        0      905 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/conftest.py
--rw-r--r--   0        0        0      188 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/alias-abbreviations.toml
--rw-r--r--   0        0        0       21 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/invalid.toml
--rw-r--r--   0        0        0      682 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/pw-test.toml
--rw-r--r--   0        0        0       19 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/test-no-config.toml
--rw-r--r--   0        0        0       94 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/test-no-tool-config.toml
--rw-r--r--   0        0        0      644 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/test.toml
--rw-r--r--   0        0        0        0 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/integration/__init__.py
--rw-r--r--   0        0        0     5341 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/integration/test_pw.py
--rw-r--r--   0        0        0     4008 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/integration/test_px.py
--rw-r--r--   0        0        0        0 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/unit/__init__.py
--rw-r--r--   0        0        0     6968 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/unit/test_cli.py
--rw-r--r--   0        0        0     4038 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/unit/test_config.py
--rw-r--r--   0        0        0     3142 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/unit/test_env.py
--rw-r--r--   0        0        0     5411 1970-01-01 00:00:00.000000 pyprojectx-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-19 06:51:31.075466 pyprojectx-1.0.0b5/LICENSE
+-rw-r--r--   0        0        0     4601 2023-06-19 06:51:31.075466 pyprojectx-1.0.0b5/README.md
+-rw-r--r--   0        0        0     4239 2023-06-19 06:54:04.772715 pyprojectx-1.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/__init__.py
+-rw-r--r--   0        0        0     5112 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/cli.py
+-rw-r--r--   0        0        0     6677 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/config.py
+-rw-r--r--   0        0        0     5471 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/env.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/global-template.toml
+-rw-r--r--   0        0        0     7263 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/initializers.py
+-rw-r--r--   0        0        0      839 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/pdm-template.toml
+-rw-r--r--   0        0        0      858 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/poetry-template.toml
+-rw-r--r--   0        0        0       32 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/poetry.toml
+-rw-r--r--   0        0        0      863 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/initializer/project-template.toml
+-rw-r--r--   0        0        0      303 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/log.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pw.bat
+-rwxr-xr-x   0        0        0     5949 2023-06-19 06:51:43.723540 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pw.py
+-rwxr-xr-x   0        0        0      253 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/px
+-rw-r--r--   0        0        0      373 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/px.bat
+-rwxr-xr-x   0        0        0      275 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pxg
+-rw-r--r--   0        0        0      270 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pxg.bat
+-rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/__init__.py
+-rw-r--r--   0        0        0      905 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/conftest.py
+-rw-r--r--   0        0        0      188 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/alias-abbreviations.toml
+-rw-r--r--   0        0        0       21 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/invalid.toml
+-rw-r--r--   0        0        0      862 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/pw-test.toml
+-rw-r--r--   0        0        0       19 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/test-no-config.toml
+-rw-r--r--   0        0        0       94 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/test-no-tool-config.toml
+-rw-r--r--   0        0        0      720 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/data/test.toml
+-rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/integration/__init__.py
+-rw-r--r--   0        0        0     5579 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/integration/test_pw.py
+-rw-r--r--   0        0        0     4008 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/integration/test_px.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/unit/__init__.py
+-rw-r--r--   0        0        0     6968 2023-06-19 06:51:31.079466 pyprojectx-1.0.0b5/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     4166 2023-06-19 06:51:31.083466 pyprojectx-1.0.0b5/tests/unit/test_config.py
+-rw-r--r--   0        0        0     3142 2023-06-19 06:51:31.083466 pyprojectx-1.0.0b5/tests/unit/test_env.py
+-rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 pyprojectx-1.0.0b5/PKG-INFO
```

### Comparing `pyprojectx-1.0.0b4/LICENSE` & `pyprojectx-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/README.md` & `pyprojectx-1.0.0b5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 **Windows**
 ```powershell
 Invoke-WebRequest https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip -OutFile wrappers.zip; Expand-Archive -Path wrappers.zip -DestinationPath .; Remove-Item -Path wrappers.zip
 ```
 
 ## Project initialization
 Initialize a new or existing project with the _--init_ option (on Windows, replace `./pw` with `pw`):
+
 * `./pw --init project`: add pyprojectx example sections to an existing or new _pyproject.toml_ in the current directory.
 * `./pw --init pdm`: initialize a [PDM](https://pdm.fming.dev/) project and add pyprojectx example sections to _pyproject.toml_.
 * `./pw --init poetry`: initialize a [Poetry](https://python-poetry.org/) project and add pyprojectx example sections to _pyproject.toml_.
 
 ## Configuration
 Add the _tool.pyprojectx_ section inside _pyproject.toml_ in your project's root directory.
```

### Comparing `pyprojectx-1.0.0b4/pyproject.toml` & `pyprojectx-1.0.0b5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyprojectx"
-version = "1.0.0b4"
+version = "1.0.0b5"
 description = "Execute scripts from pyproject.toml, installing tools on-the-fly"
 authors = [
     { name = "Houbie", email = "ivo@houbrechts-it.be" },
 ]
 readme = "README.md"
 keywords = [
     "build",
@@ -172,36 +172,37 @@
     "mkdocs-material ~=9.1",
     "mkdocstrings[python] ~=0.21",
     "markdown-include ~=0.8",
 ]
 
 [tool.pyprojectx.pdm]
 requirements = [
-    "pdm==2.5.5",
+    "pdm==2.7.4",
     "requests<2.30.0",
 ]
 post-install = "pw@pre-commit install"
 
 [tool.pyprojectx.aliases]
 install = "pdm install"
 run = "pdm run pyprojectx -t pyproject.toml "
+update = "pdm update"
 outdated = "pdm update --outdated"
 clean = "rm -r .venv .pytest_cache dist"
 clean-all = "pw@clean\nrm -r .pyprojectx"
 black = "black src tests"
 isort = "isort src tests"
 unit-test = "pdm run pytest tests/unit"
 integration-test = "pdm run pytest tests/integration"
 test = "pw@unit-test && pw@integration-test"
 check-ruff = "ruff check src tests"
 check-black = "black src tests --check"
 check = "pw@check-black && pw@check-ruff && pw@test"
 build = "pw@install && pw@check && pw@pdm build"
 publish = "pdm publish --username __token__"
-prep-release = "# cleanup\nrm -f wrappers.zip .changelog.md\n# extract version from tag\nRELEASE_VERSION=\"${GITHUB_REF_NAME}\"\n# replace __version__ in wrapper\nsed -i -e \"s/__version__/${RELEASE_VERSION}/g\" src/pyprojectx/wrapper/pw.py\nsed -i -e \"s/1.0.0b4/${RELEASE_VERSION}/g\" pyproject.toml\n# cleanup sed backup\nrm -r src/pyprojectx/wrapper/pw.py?*\nrm -r pyproject.toml?*\nmkdir -p dist-zip\ncp src/pyprojectx/wrapper/pw.py dist-zip/pw\ncp src/pyprojectx/wrapper/pw.bat dist-zip/pw.bat\nzip -j wrappers.zip dist-zip/pw*\nawk '/-{3,}/{flag=1;next}/Release/{if (flag==1)exit}flag' CHANGELOG.md > .changelog.md\n"
+prep-release = "# cleanup\nrm -f wrappers.zip .changelog.md\n# extract version from tag\nRELEASE_VERSION=\"${GITHUB_REF_NAME}\"\n# replace __version__ in wrapper\nsed -i -e \"s/__version__/${RELEASE_VERSION}/g\" src/pyprojectx/wrapper/pw.py\nsed -i -e \"s/1.0.0b5/${RELEASE_VERSION}/g\" pyproject.toml\n# cleanup sed backup\nrm -r src/pyprojectx/wrapper/pw.py?*\nrm -r pyproject.toml?*\nmkdir -p dist-zip\ncp src/pyprojectx/wrapper/pw.py dist-zip/pw\ncp src/pyprojectx/wrapper/pw.bat dist-zip/pw.bat\nzip -j wrappers.zip dist-zip/pw*\nawk '/-{3,}/{flag=1;next}/Release/{if (flag==1)exit}flag' CHANGELOG.md > .changelog.md\n"
 generate-usage = "pw@ --help > docs/docs/usage.txt"
 serve-docs = "@mkdocs: cd docs && mkdocs serve"
 generate-docs = "@mkdocs: pw@generate-usage && cd docs && mkdocs build"
 deploy-docs = "@mkdocs: cd docs && mkdocs gh-deploy"
 
 [tool.pyprojectx.os.win.aliases]
 clean = "rmdir /s/q .venv .pytest_cache dist"
```

### Comparing `pyprojectx-1.0.0b4/src/pyprojectx/cli.py` & `pyprojectx-1.0.0b5/src/pyprojectx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,24 @@
             )
             print(
                 f"{pw.BLUE}Candidates are:{pw.RESET}",
                 file=sys.stderr,
             )
             print(", ".join(aliases), file=sys.stderr)
             raise SystemExit(1)
-        tool, alias_cmd = config.get_alias(aliases[0])
-        if alias_cmd:
-            _run_alias(
-                tool,
-                alias_cmd,
-                pw_args,
-                requirements=config.get_tool_requirements(tool),
-                options=options,
-            )
+        alias_cmds = config.get_alias(aliases[0])
+        if alias_cmds:
+            for tool, alias_cmd in alias_cmds:
+                _run_alias(
+                    tool,
+                    alias_cmd,
+                    pw_args,
+                    requirements=config.get_tool_requirements(tool),
+                    options=options,
+                )
     elif config.is_tool(cmd):
         _run_in_tool_venv(
             cmd,
             [cmd, *options.cmd_args],
             requirements=config.get_tool_requirements(cmd),
             options=options,
             pw_args=pw_args,
```

### Comparing `pyprojectx-1.0.0b4/src/pyprojectx/config.py` & `pyprojectx-1.0.0b5/src/pyprojectx/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,23 @@
                 self._tools = toml_dict.get("tool", {}).get("pyprojectx", {})
                 self._aliases = self._tools.get("aliases", {})
                 self._os_aliases = self._merge_os_aliases()
         except Exception as e:  # noqa: BLE001
             raise Warning(f"Could not parse {toml_path}: {e}") from e
 
     def show_info(self, cmd, error=False):
-        tool, alias = self.get_alias(cmd)
+        alias_cmds = self.get_alias(cmd)
         out = sys.stderr if error else sys.stdout
-        if alias:
+        if alias_cmds:
             print(f"{cmd}{BLUE} is an alias in {CYAN}{self._toml_path.absolute()}", file=sys.stderr)
-            if tool:
-                print(f"{BLUE}and runs in the {CYAN}{tool}{BLUE} tool context", file=sys.stderr)
-            print(f"{BLUE}command:{RESET}", file=sys.stderr)
-            print(alias, file=out)
+            for tool, alias in alias_cmds:
+                if tool:
+                    print(f"{BLUE}and runs in the {CYAN}{tool}{BLUE} tool context", file=sys.stderr)
+                print(f"{BLUE}command:{RESET}", file=sys.stderr)
+                print(alias, file=out)
         elif self.is_tool(cmd):
             print(f"{cmd}{BLUE} is a tool in {CYAN}{self._toml_path.absolute()}", file=sys.stderr)
             print(f"{BLUE}requirements:{RESET}", file=sys.stderr)
             print(self.get_tool_requirements(cmd), file=out)
         else:
             if cmd:
                 print(
@@ -77,26 +78,32 @@
         """Check whether a key (tool name) exists in the [tool.pyprojectx] section.
 
         :param key: The key (tool name) to look for
         :return: True if the key exists in the [tool.pyprojectx] section.
         """
         return self._tools.get(key) is not None
 
-    def get_alias(self, key) -> Tuple[Optional[str], Optional[str]]:
+    def get_alias(self, key) -> List[Tuple[Optional[str], Optional[str]]]:
         """Get an alias command configured in the [tool.pyprojectx.alias] section.
 
         The alias is considered to be part of a tool if its command starts with the name of the tool
         or if the command starts with '@tool-name:'.
         :param key: The key (name) of the alias
-        :return: A tuple containing the corresponding tool (or None) and
+        :return: A list of tuples containing the corresponding tool (or None) and
          the alias command (without the optional @tool-name part), or None if there is no alias with the given key.
         """
-        alias_cmd = self._aliases.get(key)
-        if not alias_cmd:
-            return None, None
+        alias_cmds = self._aliases.get(key)
+        if not alias_cmds:
+            return []
+        if isinstance(alias_cmds, str):
+            alias_cmds = [alias_cmds]
+
+        return [self.parse_alias(cmd, key) for cmd in alias_cmds]
+
+    def parse_alias(self, alias_cmd, key) -> Tuple[Optional[str], Optional[str]]:
         if re.match(r"^@?[\w|-]+\s*:\s*", alias_cmd):
             tool, alias_cmd = re.split(r"\s*:\s*", alias_cmd, maxsplit=1)
             if tool.startswith("@"):
                 tool = tool[1:]
             if not self.is_tool(tool):
                 raise Warning(f"Invalid alias {key}: '{tool}' is not defined in [tool.pyprojectx]")
             return tool, alias_cmd
```

### Comparing `pyprojectx-1.0.0b4/src/pyprojectx/env.py` & `pyprojectx-1.0.0b5/src/pyprojectx/env.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/src/pyprojectx/initializer/initializers.py` & `pyprojectx-1.0.0b5/src/pyprojectx/initializer/initializers.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/src/pyprojectx/initializer/pdm-template.toml` & `pyprojectx-1.0.0b5/src/pyprojectx/initializer/pdm-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/src/pyprojectx/initializer/poetry-template.toml` & `pyprojectx-1.0.0b5/src/pyprojectx/initializer/poetry-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/src/pyprojectx/initializer/project-template.toml` & `pyprojectx-1.0.0b5/src/pyprojectx/initializer/project-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pw.py` & `pyprojectx-1.0.0b5/src/pyprojectx/wrapper/pw.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import argparse
 import os
 import subprocess
 import sys
 from pathlib import Path
 from venv import EnvBuilder
 
-VERSION = "1.0.0b4"
+VERSION = "1.0.0b5"
 
 PYPROJECTX_INSTALL_DIR_ENV_VAR = "PYPROJECTX_INSTALL_DIR"
 PYPROJECTX_PACKAGE_ENV_VAR = "PYPROJECTX_PACKAGE"
 PYPROJECT_TOML = "pyproject.toml"
 DEFAULT_INSTALL_DIR = ".pyprojectx"
 
 CYAN = "\033[96m"
```

### Comparing `pyprojectx-1.0.0b4/tests/conftest.py` & `pyprojectx-1.0.0b5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/tests/data/pw-test.toml` & `pyprojectx-1.0.0b5/tests/data/pw-test.toml`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 post-install = "pycowsay post-install-action && pw@create-file"
 
 [tool.pyprojectx.aliases]
 pycowsay = "pycowsay"
 pycowsay-hi = "pycowsay hi"
 pycowsay-hello = "@pycowsay: pycowsay hello"
 combine-pw-scripts = "pw@pycowsay-hi && pw@pycowsay-hello"
+combine-pw-scripts-list = [
+    "pw@pycowsay-hi",
+    "pw@pycowsay-hello",
+]
+failing-list = [
+    "echo first-cmd-output-ok",
+    "go-foo-bar",
+    "echo 'should not get here'",
+]
 failing-shell = "go-foo-bar"
 list-files = "ls"
 say-post-install = "@post-install-pycowsay: pycowsay after-post-install"
 create-file = "touch post-install-file.txt"
 
 [tool.pyprojectx.os.win.aliases]
 list-files = "dir /b"
```

### Comparing `pyprojectx-1.0.0b4/tests/integration/test_pw.py` & `pyprojectx-1.0.0b5/tests/integration/test_pw.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,20 @@
         assert not proc_result.stderr.decode("utf-8")
 
     cmd = f"{SCRIPT_PREFIX}pw -q list-files *.toml"
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=project_dir, env=env, check=True)
     assert proc_result.stdout.decode("utf-8").strip() == "pyproject.toml"
 
 
-def test_logs_and_stdout_when_alias_invoked_from_sub_directory_with_verbose(tmp_project):
+@pytest.mark.parametrize("alias", ["combine-pw-scripts", "combine-pw-scripts-list"])
+def test_logs_and_stdout_when_alias_invoked_from_sub_directory_with_verbose(alias, tmp_project):
     project_dir, env = tmp_project
     cwd = project_dir.joinpath("subdir")
     cwd.mkdir(parents=True, exist_ok=True)
-    cmd = f"..{os.sep}pw --verbose --verbose combine-pw-scripts"
+    cmd = f"..{os.sep}pw --verbose --verbose {alias}"
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=cwd, env=env, check=True)
 
     assert "< hi >" in proc_result.stdout.decode("utf-8")
     assert "< hello >" in proc_result.stdout.decode("utf-8")
     assert "INFO:pyprojectx.log:Running command in isolated venv pycowsay: pycowsay hi" in proc_result.stderr.decode(
         "utf-8"
     )
@@ -71,33 +72,36 @@
     assert "'pycow' is ambiguous" in proc_result.stderr.decode("utf-8")
     assert "pycowsay, pycowsay-hi, pycowsay-hello" in proc_result.stderr.decode("utf-8")
     if not sys.platform.startswith("win"):
         assert not proc_result.stdout.decode("utf-8")
 
 
 @pytest.mark.parametrize(
-    ("cmd", "stderr"),
+    ("cmd", "stdout", "stderr"),
     [
         (
             f"{SCRIPT_PREFIX}pw -q failing-install",
+            "",
             "PYPROJECTX ERROR: installation of 'failing-install' failed with exit code",
         ),
-        (f"{SCRIPT_PREFIX}pw -q failing-shell", "go-foo-bar"),
-        (f"{SCRIPT_PREFIX}pw -q foo-bar", "foo-bar.+is not configured as tool or alias in.+pyproject.toml"),
+        (f"{SCRIPT_PREFIX}pw -q failing-shell", "", "go-foo-bar"),
+        (f"{SCRIPT_PREFIX}pw -q foo-bar", "", "foo-bar.+is not configured as tool or alias in.+pyproject.toml"),
         (
             f"{SCRIPT_PREFIX}pw",
+            "",
             "usage: pyprojectx",
         ),
+        (f"{SCRIPT_PREFIX}pw -q failing-list", "first-cmd-output-ok", "go-foo-bar"),
     ],
 )
-def test_output_with_errors(cmd, stderr, tmp_project):
+def test_output_with_errors(cmd, stdout, stderr, tmp_project):
     project_dir, env = tmp_project
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=project_dir, env=env, check=False)
     assert proc_result.returncode
-    assert not proc_result.stdout.decode("utf-8")
+    assert proc_result.stdout.decode("utf-8").strip() == stdout
     assert re.search(stderr, proc_result.stderr.decode("utf-8"))
 
 
 def test_post_install(tmp_project):
     project_dir, env = tmp_project
     cmd = f"{SCRIPT_PREFIX}pw -q say-post-install"
     assert Path(project_dir, f"{SCRIPT_PREFIX}pw").is_file()
```

### Comparing `pyprojectx-1.0.0b4/tests/integration/test_px.py` & `pyprojectx-1.0.0b5/tests/integration/test_px.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/tests/unit/test_cli.py` & `pyprojectx-1.0.0b5/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/tests/unit/test_config.py` & `pyprojectx-1.0.0b5/tests/unit/test_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from pyprojectx.config import Config
 
 
 def test_no_config():
     config = Config(Path(__file__).parent.with_name("data").joinpath("test-no-config.toml"))
     assert config.get_tool_requirements("tool") == {"requirements": [], "post-install": None}
     assert not config.is_tool("tool")
-    assert config.get_alias("alias") == (None, None)
+    assert config.get_alias("alias") == []
 
 
 def test_no_tool_config():
     config = Config(Path(__file__).parent.with_name("data").joinpath("test-no-tool-config.toml"))
-    assert config.get_alias("run") == (None, "run command")
+    assert config.get_alias("run") == [(None, "run command")]
     with pytest.raises(
         Warning, match=r"Invalid alias wrong-tool-alias: 'wrong-tool' is not defined in \[tool.pyprojectx\]"
     ):
         config.get_alias("wrong-tool-alias")
 
 
 def test_tool_config():
@@ -44,30 +44,31 @@
 
     assert not config.is_tool("nope")
     assert config.get_tool_requirements("nope") == {"requirements": [], "post-install": None}
 
 
 def test_alias_config():
     config = Config(Path(__file__).parent.with_name("data").joinpath("test.toml"))
-    assert config.get_alias("alias-1") == ("tool-1", "tool-1 arg")
-    assert config.get_alias("alias-2") == ("tool-2", "tool-2 arg1 arg2")
-    assert config.get_alias("alias-3") == ("tool-1", "command arg")
-    assert config.get_alias("alias-4") == ("tool-2", "command --default @arg:x")
-    assert config.get_alias("combined-alias") == (None, "pw@alias-1 && pw@alias-2 pw@shell-command")
-    assert config.get_alias("shell-command") == (None, "ls -al")
-    assert config.get_alias("backward-compatible-tool-ref") == ("tool-1", "command arg")
+    assert config.get_alias("alias-1") == [("tool-1", "tool-1 arg")]
+    assert config.get_alias("alias-2") == [("tool-2", "tool-2 arg1 arg2")]
+    assert config.get_alias("alias-3") == [("tool-1", "command arg")]
+    assert config.get_alias("alias-4") == [("tool-2", "command --default @arg:x")]
+    assert config.get_alias("combined-alias") == [(None, "pw@alias-1 && pw@alias-2 pw@shell-command")]
+    assert config.get_alias("alias-list") == [(None, "pw@alias-1"), (None, "pw@alias-2"), (None, "pw@shell-command")]
+    assert config.get_alias("shell-command") == [(None, "ls -al")]
+    assert config.get_alias("backward-compatible-tool-ref") == [("tool-1", "command arg")]
 
 
 def test_os_specific_alias_config(mocker):
     config = Config(Path(__file__).parent.with_name("data").joinpath("test.toml"))
-    assert config.get_alias("os-specific") == (None, "cmd")
+    assert config.get_alias("os-specific") == [(None, "cmd")]
 
     mocker.patch("sys.platform", "my-os")
     config = Config(Path(__file__).parent.with_name("data").joinpath("test.toml"))
-    assert config.get_alias("os-specific") == (None, "my-os-cmd")
+    assert config.get_alias("os-specific") == [(None, "my-os-cmd")]
 
 
 def test_invalid_toml():
     with pytest.raises(Warning, match=r".+invalid.toml: Illegal character"):
         Config(Path(__file__).parent.with_name("data").joinpath("invalid.toml"))
```

### Comparing `pyprojectx-1.0.0b4/tests/unit/test_env.py` & `pyprojectx-1.0.0b5/tests/unit/test_env.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b4/PKG-INFO` & `pyprojectx-1.0.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprojectx
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: Execute scripts from pyproject.toml, installing tools on-the-fly
 Keywords: build dependency pyprojectx
 Home-page: https://github.com/pyprojectx/pyprojectx
 Author-Email: Houbie <ivo@houbrechts-it.be>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -61,14 +61,15 @@
 **Windows**
 ```powershell
 Invoke-WebRequest https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip -OutFile wrappers.zip; Expand-Archive -Path wrappers.zip -DestinationPath .; Remove-Item -Path wrappers.zip
 ```
 
 ## Project initialization
 Initialize a new or existing project with the _--init_ option (on Windows, replace `./pw` with `pw`):
+
 * `./pw --init project`: add pyprojectx example sections to an existing or new _pyproject.toml_ in the current directory.
 * `./pw --init pdm`: initialize a [PDM](https://pdm.fming.dev/) project and add pyprojectx example sections to _pyproject.toml_.
 * `./pw --init poetry`: initialize a [Poetry](https://python-poetry.org/) project and add pyprojectx example sections to _pyproject.toml_.
 
 ## Configuration
 Add the _tool.pyprojectx_ section inside _pyproject.toml_ in your project's root directory.
```

