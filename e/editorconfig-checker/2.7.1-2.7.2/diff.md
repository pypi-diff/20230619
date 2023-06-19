# Comparing `tmp/editorconfig-checker-2.7.1.tar.gz` & `tmp/editorconfig-checker-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "editorconfig-checker-2.7.1.tar", last modified: Mon Jan 23 19:18:31 2023, max compression
+gzip compressed data, was "editorconfig-checker-2.7.2.tar", last modified: Mon Jun 19 06:41:38 2023, max compression
```

## Comparing `editorconfig-checker-2.7.1.tar` & `editorconfig-checker-2.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-01-23 19:18:31.643444 editorconfig-checker-2.7.1/
--rw-rw-rw-   0        0        0     1096 2023-01-22 15:35:16.000000 editorconfig-checker-2.7.1/LICENSE
--rw-rw-rw-   0        0        0     3263 2023-01-23 19:18:31.643444 editorconfig-checker-2.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     2288 2023-01-22 15:35:16.000000 editorconfig-checker-2.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-23 19:18:31.643444 editorconfig-checker-2.7.1/editorconfig_checker.egg-info/
--rw-rw-rw-   0        0        0     3263 2023-01-23 19:18:31.000000 editorconfig-checker-2.7.1/editorconfig_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-01-23 19:18:31.000000 editorconfig-checker-2.7.1/editorconfig_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-23 19:18:31.000000 editorconfig-checker-2.7.1/editorconfig_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-01-23 19:18:31.000000 editorconfig-checker-2.7.1/editorconfig_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      923 2023-01-23 19:18:31.653518 editorconfig-checker-2.7.1/setup.cfg
--rw-rw-rw-   0        0        0     6010 2023-01-23 19:17:27.000000 editorconfig-checker-2.7.1/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-19 06:41:38.331033 editorconfig-checker-2.7.2/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1075 2023-06-19 06:36:34.000000 editorconfig-checker-2.7.2/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3176 2023-06-19 06:41:38.331033 editorconfig-checker-2.7.2/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2227 2023-06-19 06:36:34.000000 editorconfig-checker-2.7.2/README.md
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-19 06:41:38.307032 editorconfig-checker-2.7.2/editorconfig_checker.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3176 2023-06-19 06:41:38.000000 editorconfig-checker-2.7.2/editorconfig_checker.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      212 2023-06-19 06:41:38.000000 editorconfig-checker-2.7.2/editorconfig_checker.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-19 06:41:38.000000 editorconfig-checker-2.7.2/editorconfig_checker.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-19 06:41:38.000000 editorconfig-checker-2.7.2/editorconfig_checker.egg-info/top_level.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      894 2023-06-19 06:41:38.339035 editorconfig-checker-2.7.2/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5822 2023-06-19 06:36:50.000000 editorconfig-checker-2.7.2/setup.py
```

### Comparing `editorconfig-checker-2.7.1/LICENSE` & `editorconfig-checker-2.7.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2019 Marco M.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2019 Marco M.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `editorconfig-checker-2.7.1/PKG-INFO` & `editorconfig-checker-2.7.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-Metadata-Version: 2.1
-Name: editorconfig-checker
-Version: 2.7.1
-Summary: Python wrapper around invoking editorconfig-checker (https://github.com/editorconfig-checker/editorconfig-checker)
-Home-page: https://github.com/editorconfig-checker/editorconfig-checker.python
-Author: Marco M.
-Author-email: mmicu.github00@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Utilities
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# editorconfig-checker.python
-
-<p align="center">
-    <a href="https://pypi.org/project/editorconfig-checker/"><img src="https://img.shields.io/pypi/v/editorconfig-checker.svg?style=flat&logo=pypi" alt="PyPI Latest Release"></a>
-    <a href="https://pepy.tech/project/editorconfig-checker"><img src="https://pepy.tech/badge/editorconfig-checker" alt="Downloads"> </a>
-    <a href="http://choosealicense.com/licenses/mit/"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="MIT License"></a>
-</p>
-
-A Python wrapper to provide a pip-installable [editorconfig-checker](https://github.com/editorconfig-checker/editorconfig-checker) binary.
-
-Internally, this package provides a convenient way to download the pre-built `editorconfig-checker` binary for your particular platform.
-
-## Installation
-
-- From source code:
-  ```
-  pip install .
-  ```
-- From `PyPI`:
-  ```
-  pip install editorconfig-checker
-  ```
-
-## Usage
-
-After installation, the `ec` binary should be available in your environment (or `ec.exe` on Windows):
-
-```
-ec -version
-```
-
-## Usage with the pre-commit git hooks framework
-
-`editorconfig-checker` can be included as a hook for [pre-commit](https://pre-commit.com/).
-The easiest way to get started is to add this configuration to your `.pre-commit-config.yaml`:
-
-```yaml
-repos:
--   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
-    rev: ''  # pick a git hash / tag to point to
-    hooks:
-    -   id: editorconfig-checker
-        alias: ec
-```
-
-The above hook is a python wrapper that automatically downloads and installs
-[editorconfig-checker](https://editorconfig-checker.github.io/) binary.
-If you manage your tools in some other way, for example, via [ASDF](https://asdf-vm.com/),
-you may want to use an alternative pre-commit hook that assumes that
-`ec` binary executable is already available on the system path:
-
-```yaml
-repos:
--   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
-    rev: ''  # pick a git hash / tag to point to
-    hooks:
-    -   id: editorconfig-checker-system
-        alias: ec
-```
-
-See the [pre-commit docs](https://pre-commit.com/#pre-commit-configyaml---hooks) to check how to customize this configuration.
-
-
+Metadata-Version: 2.1
+Name: editorconfig-checker
+Version: 2.7.2
+Summary: Python wrapper around invoking editorconfig-checker (https://github.com/editorconfig-checker/editorconfig-checker)
+Home-page: https://github.com/editorconfig-checker/editorconfig-checker.python
+Author: Marco M.
+Author-email: mmicu.github00@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Utilities
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# editorconfig-checker.python
+
+<p align="center">
+    <a href="https://pypi.org/project/editorconfig-checker/"><img src="https://img.shields.io/pypi/v/editorconfig-checker.svg?style=flat&logo=pypi" alt="PyPI Latest Release"></a>
+    <a href="https://pepy.tech/project/editorconfig-checker"><img src="https://pepy.tech/badge/editorconfig-checker" alt="Downloads"> </a>
+    <a href="http://choosealicense.com/licenses/mit/"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="MIT License"></a>
+</p>
+
+A Python wrapper to provide a pip-installable [editorconfig-checker](https://github.com/editorconfig-checker/editorconfig-checker) binary.
+
+Internally, this package provides a convenient way to download the pre-built `editorconfig-checker` binary for your particular platform.
+
+## Installation
+
+- From source code:
+  ```
+  pip install .
+  ```
+- From `PyPI`:
+  ```
+  pip install editorconfig-checker
+  ```
+
+## Usage
+
+After installation, the `ec` binary should be available in your environment (or `ec.exe` on Windows):
+
+```
+ec -version
+```
+
+## Usage with the pre-commit git hooks framework
+
+`editorconfig-checker` can be included as a hook for [pre-commit](https://pre-commit.com/).
+The easiest way to get started is to add this configuration to your `.pre-commit-config.yaml`:
+
+```yaml
+repos:
+-   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
+    rev: ''  # pick a git hash / tag to point to
+    hooks:
+    -   id: editorconfig-checker
+        alias: ec
+```
+
+The above hook is a python wrapper that automatically downloads and installs
+[editorconfig-checker](https://editorconfig-checker.github.io/) binary.
+If you manage your tools in some other way, for example, via [ASDF](https://asdf-vm.com/),
+you may want to use an alternative pre-commit hook that assumes that
+`ec` binary executable is already available on the system path:
+
+```yaml
+repos:
+-   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
+    rev: ''  # pick a git hash / tag to point to
+    hooks:
+    -   id: editorconfig-checker-system
+        alias: ec
+```
+
+See the [pre-commit docs](https://pre-commit.com/#pre-commit-configyaml---hooks) to check how to customize this configuration.
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: editorconfig-checker Version: 2.7.1 Summary: Python
+Metadata-Version: 2.1 Name: editorconfig-checker Version: 2.7.2 Summary: Python
 wrapper around invoking editorconfig-checker (https://github.com/editorconfig-
 checker/editorconfig-checker) Home-page: https://github.com/editorconfig-
 checker/editorconfig-checker.python Author: Marco M. Author-email:
 mmicu.github00@gmail.com License: MIT Platform: UNKNOWN Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 2 Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.5 Classifier:
```

### Comparing `editorconfig-checker-2.7.1/README.md` & `editorconfig-checker-2.7.2/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-# editorconfig-checker.python
-
-<p align="center">
-    <a href="https://pypi.org/project/editorconfig-checker/"><img src="https://img.shields.io/pypi/v/editorconfig-checker.svg?style=flat&logo=pypi" alt="PyPI Latest Release"></a>
-    <a href="https://pepy.tech/project/editorconfig-checker"><img src="https://pepy.tech/badge/editorconfig-checker" alt="Downloads"> </a>
-    <a href="http://choosealicense.com/licenses/mit/"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="MIT License"></a>
-</p>
-
-A Python wrapper to provide a pip-installable [editorconfig-checker](https://github.com/editorconfig-checker/editorconfig-checker) binary.
-
-Internally, this package provides a convenient way to download the pre-built `editorconfig-checker` binary for your particular platform.
-
-## Installation
-
-- From source code:
-  ```
-  pip install .
-  ```
-- From `PyPI`:
-  ```
-  pip install editorconfig-checker
-  ```
-
-## Usage
-
-After installation, the `ec` binary should be available in your environment (or `ec.exe` on Windows):
-
-```
-ec -version
-```
-
-## Usage with the pre-commit git hooks framework
-
-`editorconfig-checker` can be included as a hook for [pre-commit](https://pre-commit.com/).
-The easiest way to get started is to add this configuration to your `.pre-commit-config.yaml`:
-
-```yaml
-repos:
--   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
-    rev: ''  # pick a git hash / tag to point to
-    hooks:
-    -   id: editorconfig-checker
-        alias: ec
-```
-
-The above hook is a python wrapper that automatically downloads and installs
-[editorconfig-checker](https://editorconfig-checker.github.io/) binary.
-If you manage your tools in some other way, for example, via [ASDF](https://asdf-vm.com/),
-you may want to use an alternative pre-commit hook that assumes that
-`ec` binary executable is already available on the system path:
-
-```yaml
-repos:
--   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
-    rev: ''  # pick a git hash / tag to point to
-    hooks:
-    -   id: editorconfig-checker-system
-        alias: ec
-```
-
-See the [pre-commit docs](https://pre-commit.com/#pre-commit-configyaml---hooks) to check how to customize this configuration.
+# editorconfig-checker.python
+
+<p align="center">
+    <a href="https://pypi.org/project/editorconfig-checker/"><img src="https://img.shields.io/pypi/v/editorconfig-checker.svg?style=flat&logo=pypi" alt="PyPI Latest Release"></a>
+    <a href="https://pepy.tech/project/editorconfig-checker"><img src="https://pepy.tech/badge/editorconfig-checker" alt="Downloads"> </a>
+    <a href="http://choosealicense.com/licenses/mit/"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="MIT License"></a>
+</p>
+
+A Python wrapper to provide a pip-installable [editorconfig-checker](https://github.com/editorconfig-checker/editorconfig-checker) binary.
+
+Internally, this package provides a convenient way to download the pre-built `editorconfig-checker` binary for your particular platform.
+
+## Installation
+
+- From source code:
+  ```
+  pip install .
+  ```
+- From `PyPI`:
+  ```
+  pip install editorconfig-checker
+  ```
+
+## Usage
+
+After installation, the `ec` binary should be available in your environment (or `ec.exe` on Windows):
+
+```
+ec -version
+```
+
+## Usage with the pre-commit git hooks framework
+
+`editorconfig-checker` can be included as a hook for [pre-commit](https://pre-commit.com/).
+The easiest way to get started is to add this configuration to your `.pre-commit-config.yaml`:
+
+```yaml
+repos:
+-   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
+    rev: ''  # pick a git hash / tag to point to
+    hooks:
+    -   id: editorconfig-checker
+        alias: ec
+```
+
+The above hook is a python wrapper that automatically downloads and installs
+[editorconfig-checker](https://editorconfig-checker.github.io/) binary.
+If you manage your tools in some other way, for example, via [ASDF](https://asdf-vm.com/),
+you may want to use an alternative pre-commit hook that assumes that
+`ec` binary executable is already available on the system path:
+
+```yaml
+repos:
+-   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
+    rev: ''  # pick a git hash / tag to point to
+    hooks:
+    -   id: editorconfig-checker-system
+        alias: ec
+```
+
+See the [pre-commit docs](https://pre-commit.com/#pre-commit-configyaml---hooks) to check how to customize this configuration.
```

### Comparing `editorconfig-checker-2.7.1/editorconfig_checker.egg-info/PKG-INFO` & `editorconfig-checker-2.7.2/editorconfig_checker.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-Metadata-Version: 2.1
-Name: editorconfig-checker
-Version: 2.7.1
-Summary: Python wrapper around invoking editorconfig-checker (https://github.com/editorconfig-checker/editorconfig-checker)
-Home-page: https://github.com/editorconfig-checker/editorconfig-checker.python
-Author: Marco M.
-Author-email: mmicu.github00@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Utilities
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# editorconfig-checker.python
-
-<p align="center">
-    <a href="https://pypi.org/project/editorconfig-checker/"><img src="https://img.shields.io/pypi/v/editorconfig-checker.svg?style=flat&logo=pypi" alt="PyPI Latest Release"></a>
-    <a href="https://pepy.tech/project/editorconfig-checker"><img src="https://pepy.tech/badge/editorconfig-checker" alt="Downloads"> </a>
-    <a href="http://choosealicense.com/licenses/mit/"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="MIT License"></a>
-</p>
-
-A Python wrapper to provide a pip-installable [editorconfig-checker](https://github.com/editorconfig-checker/editorconfig-checker) binary.
-
-Internally, this package provides a convenient way to download the pre-built `editorconfig-checker` binary for your particular platform.
-
-## Installation
-
-- From source code:
-  ```
-  pip install .
-  ```
-- From `PyPI`:
-  ```
-  pip install editorconfig-checker
-  ```
-
-## Usage
-
-After installation, the `ec` binary should be available in your environment (or `ec.exe` on Windows):
-
-```
-ec -version
-```
-
-## Usage with the pre-commit git hooks framework
-
-`editorconfig-checker` can be included as a hook for [pre-commit](https://pre-commit.com/).
-The easiest way to get started is to add this configuration to your `.pre-commit-config.yaml`:
-
-```yaml
-repos:
--   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
-    rev: ''  # pick a git hash / tag to point to
-    hooks:
-    -   id: editorconfig-checker
-        alias: ec
-```
-
-The above hook is a python wrapper that automatically downloads and installs
-[editorconfig-checker](https://editorconfig-checker.github.io/) binary.
-If you manage your tools in some other way, for example, via [ASDF](https://asdf-vm.com/),
-you may want to use an alternative pre-commit hook that assumes that
-`ec` binary executable is already available on the system path:
-
-```yaml
-repos:
--   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
-    rev: ''  # pick a git hash / tag to point to
-    hooks:
-    -   id: editorconfig-checker-system
-        alias: ec
-```
-
-See the [pre-commit docs](https://pre-commit.com/#pre-commit-configyaml---hooks) to check how to customize this configuration.
-
-
+Metadata-Version: 2.1
+Name: editorconfig-checker
+Version: 2.7.2
+Summary: Python wrapper around invoking editorconfig-checker (https://github.com/editorconfig-checker/editorconfig-checker)
+Home-page: https://github.com/editorconfig-checker/editorconfig-checker.python
+Author: Marco M.
+Author-email: mmicu.github00@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Utilities
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# editorconfig-checker.python
+
+<p align="center">
+    <a href="https://pypi.org/project/editorconfig-checker/"><img src="https://img.shields.io/pypi/v/editorconfig-checker.svg?style=flat&logo=pypi" alt="PyPI Latest Release"></a>
+    <a href="https://pepy.tech/project/editorconfig-checker"><img src="https://pepy.tech/badge/editorconfig-checker" alt="Downloads"> </a>
+    <a href="http://choosealicense.com/licenses/mit/"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="MIT License"></a>
+</p>
+
+A Python wrapper to provide a pip-installable [editorconfig-checker](https://github.com/editorconfig-checker/editorconfig-checker) binary.
+
+Internally, this package provides a convenient way to download the pre-built `editorconfig-checker` binary for your particular platform.
+
+## Installation
+
+- From source code:
+  ```
+  pip install .
+  ```
+- From `PyPI`:
+  ```
+  pip install editorconfig-checker
+  ```
+
+## Usage
+
+After installation, the `ec` binary should be available in your environment (or `ec.exe` on Windows):
+
+```
+ec -version
+```
+
+## Usage with the pre-commit git hooks framework
+
+`editorconfig-checker` can be included as a hook for [pre-commit](https://pre-commit.com/).
+The easiest way to get started is to add this configuration to your `.pre-commit-config.yaml`:
+
+```yaml
+repos:
+-   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
+    rev: ''  # pick a git hash / tag to point to
+    hooks:
+    -   id: editorconfig-checker
+        alias: ec
+```
+
+The above hook is a python wrapper that automatically downloads and installs
+[editorconfig-checker](https://editorconfig-checker.github.io/) binary.
+If you manage your tools in some other way, for example, via [ASDF](https://asdf-vm.com/),
+you may want to use an alternative pre-commit hook that assumes that
+`ec` binary executable is already available on the system path:
+
+```yaml
+repos:
+-   repo: https://github.com/editorconfig-checker/editorconfig-checker.python
+    rev: ''  # pick a git hash / tag to point to
+    hooks:
+    -   id: editorconfig-checker-system
+        alias: ec
+```
+
+See the [pre-commit docs](https://pre-commit.com/#pre-commit-configyaml---hooks) to check how to customize this configuration.
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: editorconfig-checker Version: 2.7.1 Summary: Python
+Metadata-Version: 2.1 Name: editorconfig-checker Version: 2.7.2 Summary: Python
 wrapper around invoking editorconfig-checker (https://github.com/editorconfig-
 checker/editorconfig-checker) Home-page: https://github.com/editorconfig-
 checker/editorconfig-checker.python Author: Marco M. Author-email:
 mmicu.github00@gmail.com License: MIT Platform: UNKNOWN Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 2 Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.5 Classifier:
```

### Comparing `editorconfig-checker-2.7.1/setup.cfg` & `editorconfig-checker-2.7.2/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2065 6469 746f 7263 6f6e 6669 672d   = editorconfig-
-00000020: 6368 6563 6b65 720d 0a64 6573 6372 6970  checker..descrip
-00000030: 7469 6f6e 203d 2050 7974 686f 6e20 7772  tion = Python wr
-00000040: 6170 7065 7220 6172 6f75 6e64 2069 6e76  apper around inv
-00000050: 6f6b 696e 6720 6564 6974 6f72 636f 6e66  oking editorconf
-00000060: 6967 2d63 6865 636b 6572 2028 6874 7470  ig-checker (http
-00000070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00000080: 6469 746f 7263 6f6e 6669 672d 6368 6563  ditorconfig-chec
-00000090: 6b65 722f 6564 6974 6f72 636f 6e66 6967  ker/editorconfig
-000000a0: 2d63 6865 636b 6572 290d 0a6c 6f6e 675f  -checker)..long_
-000000b0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-000000c0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-000000d0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-000000e0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-000000f0: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
-00000100: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
-00000110: 7562 2e63 6f6d 2f65 6469 746f 7263 6f6e  ub.com/editorcon
-00000120: 6669 672d 6368 6563 6b65 722f 6564 6974  fig-checker/edit
-00000130: 6f72 636f 6e66 6967 2d63 6865 636b 6572  orconfig-checker
-00000140: 2e70 7974 686f 6e0d 0a61 7574 686f 7220  .python..author 
-00000150: 3d20 4d61 7263 6f20 4d2e 0d0a 6175 7468  = Marco M...auth
-00000160: 6f72 5f65 6d61 696c 203d 206d 6d69 6375  or_email = mmicu
-00000170: 2e67 6974 6875 6230 3040 676d 6169 6c2e  .github00@gmail.
-00000180: 636f 6d0d 0a6c 6963 656e 7365 203d 204d  com..license = M
-00000190: 4954 0d0a 6c69 6365 6e73 655f 6669 6c65  IT..license_file
-000001a0: 203d 204c 4943 454e 5345 0d0a 636c 6173   = LICENSE..clas
-000001b0: 7369 6669 6572 7320 3d20 0d0a 0950 726f  sifiers = ...Pro
-000001c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000001d0: 6520 3a3a 2050 7974 686f 6e0d 0a09 5072  e :: Python...Pr
-000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000200: 320d 0a09 5072 6f67 7261 6d6d 696e 6720  2...Programming 
-00000210: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000220: 6f6e 203a 3a20 322e 370d 0a09 5072 6f67  on :: 2.7...Prog
-00000230: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000240: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-00000250: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000260: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000270: 203a 3a20 332e 350d 0a09 5072 6f67 7261   :: 3.5...Progra
-00000280: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000290: 3a20 5079 7468 6f6e 203a 3a20 332e 360d  : Python :: 3.6.
-000002a0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002c0: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
-000002d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002e0: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-000002f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000300: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000310: 203a 3a20 332e 390d 0a09 546f 7069 6320   :: 3.9...Topic 
-00000320: 3a3a 2054 6578 7420 5072 6f63 6573 7369  :: Text Processi
-00000330: 6e67 0d0a 0954 6f70 6963 203a 3a20 5574  ng...Topic :: Ut
-00000340: 696c 6974 6965 730d 0a0d 0a5b 6f70 7469  ilities....[opti
-00000350: 6f6e 735d 0d0a 7079 7468 6f6e 5f72 6571  ons]..python_req
-00000360: 7569 7265 7320 3d20 3e3d 322e 370d 0a0d  uires = >=2.7...
-00000370: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000380: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000390: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6564 6974 6f72 636f 6e66 6967 2d63  = editorconfig-c
+00000020: 6865 636b 6572 0a64 6573 6372 6970 7469  hecker.descripti
+00000030: 6f6e 203d 2050 7974 686f 6e20 7772 6170  on = Python wrap
+00000040: 7065 7220 6172 6f75 6e64 2069 6e76 6f6b  per around invok
+00000050: 696e 6720 6564 6974 6f72 636f 6e66 6967  ing editorconfig
+00000060: 2d63 6865 636b 6572 2028 6874 7470 733a  -checker (https:
+00000070: 2f2f 6769 7468 7562 2e63 6f6d 2f65 6469  //github.com/edi
+00000080: 746f 7263 6f6e 6669 672d 6368 6563 6b65  torconfig-checke
+00000090: 722f 6564 6974 6f72 636f 6e66 6967 2d63  r/editorconfig-c
+000000a0: 6865 636b 6572 290a 6c6f 6e67 5f64 6573  hecker).long_des
+000000b0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000c0: 2052 4541 444d 452e 6d64 0a6c 6f6e 675f   README.md.long_
+000000d0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+000000e0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+000000f0: 6d61 726b 646f 776e 0a75 726c 203d 2068  markdown.url = h
+00000100: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000110: 6d2f 6564 6974 6f72 636f 6e66 6967 2d63  m/editorconfig-c
+00000120: 6865 636b 6572 2f65 6469 746f 7263 6f6e  hecker/editorcon
+00000130: 6669 672d 6368 6563 6b65 722e 7079 7468  fig-checker.pyth
+00000140: 6f6e 0a61 7574 686f 7220 3d20 4d61 7263  on.author = Marc
+00000150: 6f20 4d2e 0a61 7574 686f 725f 656d 6169  o M..author_emai
+00000160: 6c20 3d20 6d6d 6963 752e 6769 7468 7562  l = mmicu.github
+00000170: 3030 4067 6d61 696c 2e63 6f6d 0a6c 6963  00@gmail.com.lic
+00000180: 656e 7365 203d 204d 4954 0a6c 6963 656e  ense = MIT.licen
+00000190: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
+000001a0: 5345 0a63 6c61 7373 6966 6965 7273 203d  SE.classifiers =
+000001b0: 200a 0950 726f 6772 616d 6d69 6e67 204c   ..Programming L
+000001c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001d0: 6e0a 0950 726f 6772 616d 6d69 6e67 204c  n..Programming L
+000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001f0: 6e20 3a3a 2032 0a09 5072 6f67 7261 6d6d  n :: 2..Programm
+00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000210: 5079 7468 6f6e 203a 3a20 322e 370a 0950  Python :: 2.7..P
+00000220: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000230: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000240: 2033 0a09 5072 6f67 7261 6d6d 696e 6720   3..Programming 
+00000250: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000260: 6f6e 203a 3a20 332e 350a 0950 726f 6772  on :: 3.5..Progr
+00000270: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000280: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e36  :: Python :: 3.6
+00000290: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000002a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002b0: 203a 3a20 332e 370a 0950 726f 6772 616d   :: 3.7..Program
+000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002d0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a09   Python :: 3.8..
+000002e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000300: 3a20 332e 390a 0954 6f70 6963 203a 3a20  : 3.9..Topic :: 
+00000310: 5465 7874 2050 726f 6365 7373 696e 670a  Text Processing.
+00000320: 0954 6f70 6963 203a 3a20 5574 696c 6974  .Topic :: Utilit
+00000330: 6965 730a 0a5b 6f70 7469 6f6e 735d 0a70  ies..[options].p
+00000340: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000350: 203e 3d32 2e37 0a0a 5b65 6767 5f69 6e66   >=2.7..[egg_inf
+00000360: 6f5d 0a74 6167 5f62 7569 6c64 203d 200a  o].tag_build = .
+00000370: 7461 675f 6461 7465 203d 2030 0a0a       tag_date = 0..
```

### Comparing `editorconfig-checker-2.7.1/setup.py` & `editorconfig-checker-2.7.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-
-"""
-This setup logic is highly ispired to the one used in `https://github.com/shellcheck-py/shellcheck-py`.
-
-After `https://github.com/editorconfig-checker/editorconfig-checker.python/issues/15` was opened,
-we decided to move the wrapper logic directly in the setup phase.
-
-During setup, the tarball that contains the executable will be downloaded based on
-the target machine and its content extracted in the proper output directory.
-
-Once the setup is complete, the `ec` executable should be available on your machine.
-"""
-
-from io import BytesIO
-from distutils.command.build import build as orig_build
-from distutils.core import Command
-from os import chmod, makedirs, path, stat
-from platform import architecture, machine, system
-from setuptools import setup
-from setuptools.command.install import install as orig_install
-from stat import S_IXUSR, S_IXGRP, S_IXOTH
-from tarfile import open as tarfile_open
-
-try:
-    # Python 3
-    from urllib.request import urlopen
-except ImportError:
-    # Python 2.7
-    from urllib2 import urlopen
-
-
-WRAPPER_VERSION = '2.7.1'
-EDITORCONFIG_CHECKER_CORE_VERSION = '2.7.0'
-EDITORCONFIG_CHECKER_EXE_NAME = 'ec'
-
-
-def get_tarball_url():
-    def get_ec_name_by_system():
-        # Platform              architecture()      system()    machine()
-        # ---------------------------------------------------------------
-        # Linux x86 64bit       ('64bit', 'ELF')    'Linux'     'x86_64'
-        # Linux AWS Graviton2   ('64bit', 'ELF')    'Linux'     'aarch64'
-        # Mac x86 64bit         ('64bit', '')       'Darwin'    'x86_64'
-        # Mac M1 64bit          ('64bit', '')       'Darwin'    'arm64'
-        _system = system()
-        _machine = machine()
-        if _machine == 'x86_64':
-            _architecture = 'amd64'
-        elif _machine == 'aarch64' or _machine == 'arm64':
-            _architecture = 'arm64'
-        elif isinstance(architecture(), tuple) and len(architecture()) > 0:
-            _architecture = 'amd64' if architecture()[0] == '64bit' else '386'
-        else:
-            raise ValueError('Cannot determine architecture')
-
-        # The core, from `2.7.0`, introduces the extension in the tarball name
-        # (e.g. `ec-windows-386.exe.tar.gz`, `ec-windows-arm.exe.tar.gz`)
-        _ext = '.exe' if _system == 'Windows' else ''
-
-        return 'ec-{}-{}{}'.format(
-            _system.lower(),
-            _architecture,
-            _ext,
-        )
-
-    return 'https://github.com/editorconfig-checker/editorconfig-checker/releases/download/{}/{}.tar.gz'.format(
-        EDITORCONFIG_CHECKER_CORE_VERSION,
-        get_ec_name_by_system(),
-    )
-
-
-def download_tarball(url):
-    sock = urlopen(url)
-    code = sock.getcode()
-
-    if code != 200:
-        sock.close()
-        raise ValueError('HTTP failure. Code: {}'.format(code))
-
-    data = sock.read()
-    sock.close()
-
-    return data
-
-
-def extract_tarball(url, data):
-    with BytesIO(data) as bio:
-        if '.tar.' in url:
-            with tarfile_open(fileobj=bio) as tarf:
-                for info in tarf.getmembers():
-                    if info.isfile() and info.name.startswith('bin/ec-'):
-                        return tarf.extractfile(info).read()
-
-    raise AssertionError('unreachable `extract` function')
-
-
-def save_executables(data, base_dir):
-    exe = EDITORCONFIG_CHECKER_EXE_NAME
-    if system() == 'Windows':
-        exe += '.exe'
-
-    output_path = path.join(base_dir, exe)
-    makedirs(base_dir)
-
-    with open(output_path, 'wb') as fp:
-        fp.write(data)
-
-    # Mark as executable ~ https://stackoverflow.com/a/14105527
-    mode = stat(output_path).st_mode
-    mode |= S_IXUSR | S_IXGRP | S_IXOTH
-    chmod(output_path, mode)
-
-
-class build(orig_build):
-    sub_commands = orig_build.sub_commands + [('fetch_binaries', None)]
-
-
-class install(orig_install):
-    sub_commands = orig_install.sub_commands + [('install_editorconfig_checker', None)]
-
-
-class fetch_binaries(Command):
-    build_temp = None
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        self.set_undefined_options('build', ('build_temp', 'build_temp'))
-
-    def run(self):
-        # save binary to self.build_temp
-        url = get_tarball_url()
-        archive = download_tarball(url)
-        data = extract_tarball(url, archive)
-        save_executables(data, self.build_temp)
-
-
-class install_editorconfig_checker(Command):
-    description = 'install the editorconfig-checker executable'
-    outfiles = ()
-    build_dir = install_dir = None
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        # this initializes attributes based on other commands' attributes
-        self.set_undefined_options('build', ('build_temp', 'build_dir'))
-        self.set_undefined_options('install', ('install_scripts', 'install_dir'))
-
-    def run(self):
-        self.outfiles = self.copy_tree(self.build_dir, self.install_dir)
-
-    def get_outputs(self):
-        return self.outfiles
-
-
-command_overrides = {
-    'install': install,
-    'install_editorconfig_checker': install_editorconfig_checker,
-    'build': build,
-    'fetch_binaries': fetch_binaries,
-}
-
-
-try:
-    from wheel.bdist_wheel import bdist_wheel as orig_bdist_wheel
-except ImportError:
-    pass
-else:
-    class bdist_wheel(orig_bdist_wheel):
-        def finalize_options(self):
-            orig_bdist_wheel.finalize_options(self)
-            # Mark us as not a pure python package
-            self.root_is_pure = False
-
-        def get_tag(self):
-            _, _, plat = orig_bdist_wheel.get_tag(self)
-            # We don't contain any python source, nor any python extensions
-            return 'py2.py3', 'none', plat
-
-    command_overrides['bdist_wheel'] = bdist_wheel
-
-
-setup(version=WRAPPER_VERSION, cmdclass=command_overrides)
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+
+"""
+This setup logic is highly ispired to the one used in `https://github.com/shellcheck-py/shellcheck-py`.
+
+After `https://github.com/editorconfig-checker/editorconfig-checker.python/issues/15` was opened,
+we decided to move the wrapper logic directly in the setup phase.
+
+During setup, the tarball that contains the executable will be downloaded based on
+the target machine and its content extracted in the proper output directory.
+
+Once the setup is complete, the `ec` executable should be available on your machine.
+"""
+
+from io import BytesIO
+from distutils.command.build import build as orig_build
+from distutils.core import Command
+from os import chmod, makedirs, path, stat
+from platform import architecture, machine, system
+from setuptools import setup
+from setuptools.command.install import install as orig_install
+from stat import S_IXUSR, S_IXGRP, S_IXOTH
+from tarfile import open as tarfile_open
+
+try:
+    # Python 3
+    from urllib.request import urlopen
+except ImportError:
+    # Python 2.7
+    from urllib2 import urlopen
+
+
+WRAPPER_VERSION = '2.7.2'
+EDITORCONFIG_CHECKER_CORE_VERSION = '2.7.0'
+EDITORCONFIG_CHECKER_EXE_NAME = 'ec'
+
+
+def get_tarball_url():
+    def get_ec_name_by_system():
+        # Platform              architecture()      system()    machine()
+        # ---------------------------------------------------------------
+        # Linux x86 64bit       ('64bit', 'ELF')    'Linux'     'x86_64'
+        # Linux AWS Graviton2   ('64bit', 'ELF')    'Linux'     'aarch64'
+        # Mac x86 64bit         ('64bit', '')       'Darwin'    'x86_64'
+        # Mac M1 64bit          ('64bit', '')       'Darwin'    'arm64'
+        _system = system()
+        _machine = machine()
+        if _machine == 'x86_64':
+            _architecture = 'amd64'
+        elif _machine == 'aarch64' or _machine == 'arm64':
+            _architecture = 'arm64'
+        elif isinstance(architecture(), tuple) and len(architecture()) > 0:
+            _architecture = 'amd64' if architecture()[0] == '64bit' else '386'
+        else:
+            raise ValueError('Cannot determine architecture')
+
+        # The core, from `2.7.0`, introduces the extension in the tarball name
+        # (e.g. `ec-windows-386.exe.tar.gz`, `ec-windows-arm.exe.tar.gz`)
+        _ext = '.exe' if _system == 'Windows' else ''
+
+        return 'ec-{}-{}{}'.format(
+            _system.lower(),
+            _architecture,
+            _ext,
+        )
+
+    return 'https://github.com/editorconfig-checker/editorconfig-checker/releases/download/{}/{}.tar.gz'.format(
+        EDITORCONFIG_CHECKER_CORE_VERSION,
+        get_ec_name_by_system(),
+    )
+
+
+def download_tarball(url):
+    sock = urlopen(url)
+    code = sock.getcode()
+
+    if code != 200:
+        sock.close()
+        raise ValueError('HTTP failure. Code: {}'.format(code))
+
+    data = sock.read()
+    sock.close()
+
+    return data
+
+
+def extract_tarball(url, data):
+    with BytesIO(data) as bio:
+        if '.tar.' in url:
+            with tarfile_open(fileobj=bio) as tarf:
+                for info in tarf.getmembers():
+                    if info.isfile() and info.name.startswith('bin/ec-'):
+                        return tarf.extractfile(info).read()
+
+    raise AssertionError('unreachable `extract` function')
+
+
+def save_executables(data, base_dir):
+    exe = EDITORCONFIG_CHECKER_EXE_NAME
+    if system() == 'Windows':
+        exe += '.exe'
+
+    output_path = path.join(base_dir, exe)
+    makedirs(base_dir)
+
+    with open(output_path, 'wb') as fp:
+        fp.write(data)
+
+    # Mark as executable ~ https://stackoverflow.com/a/14105527
+    mode = stat(output_path).st_mode
+    mode |= S_IXUSR | S_IXGRP | S_IXOTH
+    chmod(output_path, mode)
+
+
+class build(orig_build):
+    sub_commands = orig_build.sub_commands + [('fetch_binaries', None)]
+
+
+class install(orig_install):
+    sub_commands = orig_install.sub_commands + [('install_editorconfig_checker', None)]
+
+
+class fetch_binaries(Command):
+    build_temp = None
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        self.set_undefined_options('build', ('build_temp', 'build_temp'))
+
+    def run(self):
+        # save binary to self.build_temp
+        url = get_tarball_url()
+        archive = download_tarball(url)
+        data = extract_tarball(url, archive)
+        save_executables(data, self.build_temp)
+
+
+class install_editorconfig_checker(Command):
+    description = 'install the editorconfig-checker executable'
+    outfiles = ()
+    build_dir = install_dir = None
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        # this initializes attributes based on other commands' attributes
+        self.set_undefined_options('build', ('build_temp', 'build_dir'))
+        self.set_undefined_options('install', ('install_scripts', 'install_dir'))
+
+    def run(self):
+        self.outfiles = self.copy_tree(self.build_dir, self.install_dir)
+
+    def get_outputs(self):
+        return self.outfiles
+
+
+command_overrides = {
+    'install': install,
+    'install_editorconfig_checker': install_editorconfig_checker,
+    'build': build,
+    'fetch_binaries': fetch_binaries,
+}
+
+
+try:
+    from wheel.bdist_wheel import bdist_wheel as orig_bdist_wheel
+except ImportError:
+    pass
+else:
+    class bdist_wheel(orig_bdist_wheel):
+        def finalize_options(self):
+            orig_bdist_wheel.finalize_options(self)
+            # Mark us as not a pure python package
+            self.root_is_pure = False
+
+        def get_tag(self):
+            _, _, plat = orig_bdist_wheel.get_tag(self)
+            # We don't contain any python source, nor any python extensions
+            return 'py2.py3', 'none', plat
+
+    command_overrides['bdist_wheel'] = bdist_wheel
+
+
+setup(version=WRAPPER_VERSION, cmdclass=command_overrides)
```

