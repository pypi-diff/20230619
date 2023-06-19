# Comparing `tmp/open_webdriver-1.4.2.tar.gz` & `tmp/open_webdriver-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_webdriver-1.4.2.tar", last modified: Mon Nov 28 05:53:55 2022, max compression
+gzip compressed data, was "open_webdriver-1.4.3.tar", last modified: Mon Jun 19 03:05:16 2023, max compression
```

## Comparing `open_webdriver-1.4.2.tar` & `open_webdriver-1.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-11-28 05:53:55.219734 open_webdriver-1.4.2/
--rw-rw-rw-   0        0        0     1064 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/LICENSE
--rw-rw-rw-   0        0        0      196 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8082 2022-11-28 05:53:55.218736 open_webdriver-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     7251 2022-11-28 05:51:21.000000 open_webdriver-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 05:53:55.191735 open_webdriver-1.4.2/open_webdriver/
--rw-rw-rw-   0        0        0      400 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/open_webdriver/__init__.py
--rw-rw-rw-   0        0        0      411 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/open_webdriver/demo_app.py
--rw-rw-rw-   0        0        0     4225 2022-11-22 05:42:15.000000 open_webdriver-1.4.2/open_webdriver/download_chromium.py
--rw-rw-rw-   0        0        0     3822 2022-11-28 05:50:15.000000 open_webdriver-1.4.2/open_webdriver/open_webdriver.py
--rw-rw-rw-   0        0        0      272 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/open_webdriver/path.py
-drwxrwxrwx   0        0        0        0 2022-11-28 05:53:55.214736 open_webdriver-1.4.2/open_webdriver/tests/
--rw-rw-rw-   0        0        0        0 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/open_webdriver/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-28 05:53:55.217734 open_webdriver-1.4.2/open_webdriver/tests/unit/
--rw-rw-rw-   0        0        0        0 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/open_webdriver/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     1806 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/open_webdriver/tests/unit/test_webdriver.py
--rw-rw-rw-   0        0        0       64 2022-11-28 05:50:38.000000 open_webdriver-1.4.2/open_webdriver/version.py
-drwxrwxrwx   0        0        0        0 2022-11-28 05:53:55.213735 open_webdriver-1.4.2/open_webdriver.egg-info/
--rw-rw-rw-   0        0        0     8082 2022-11-28 05:53:54.000000 open_webdriver-1.4.2/open_webdriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2022-11-28 05:53:55.000000 open_webdriver-1.4.2/open_webdriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-28 05:53:54.000000 open_webdriver-1.4.2/open_webdriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-11-28 05:53:54.000000 open_webdriver-1.4.2/open_webdriver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       90 2022-11-28 05:53:54.000000 open_webdriver-1.4.2/open_webdriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-11-28 05:53:54.000000 open_webdriver-1.4.2/open_webdriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2022-11-28 01:34:30.000000 open_webdriver-1.4.2/requirements.testing.txt
--rw-rw-rw-   0        0        0       74 2022-11-22 04:50:01.000000 open_webdriver-1.4.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-11-28 05:53:55.220735 open_webdriver-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     3025 2022-11-17 01:18:42.000000 open_webdriver-1.4.2/setup.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-19 03:05:16.802356 open_webdriver-1.4.3/
+-rw-r--r--   0 niteris    (501) staff       (20)     1064 2022-05-25 01:01:31.000000 open_webdriver-1.4.3/LICENSE
+-rw-r--r--   0 niteris    (501) staff       (20)      196 2022-05-25 01:01:31.000000 open_webdriver-1.4.3/MANIFEST.in
+-rw-r--r--   0 niteris    (501) staff       (20)     8072 2023-06-19 03:05:16.801453 open_webdriver-1.4.3/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)     7405 2023-06-18 23:53:16.000000 open_webdriver-1.4.3/README.md
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-19 03:05:16.798253 open_webdriver-1.4.3/open_webdriver/
+-rw-r--r--   0 niteris    (501) staff       (20)      326 2023-06-18 23:37:52.000000 open_webdriver-1.4.3/open_webdriver/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)      416 2023-06-18 23:39:06.000000 open_webdriver-1.4.3/open_webdriver/demo_app.py
+-rw-r--r--   0 niteris    (501) staff       (20)     4596 2023-06-19 02:53:03.000000 open_webdriver-1.4.3/open_webdriver/download_chromium.py
+-rw-r--r--   0 niteris    (501) staff       (20)     3860 2023-06-18 23:47:57.000000 open_webdriver-1.4.3/open_webdriver/main.py
+-rw-r--r--   0 niteris    (501) staff       (20)      272 2022-05-25 01:01:32.000000 open_webdriver-1.4.3/open_webdriver/path.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-19 03:05:16.800424 open_webdriver-1.4.3/open_webdriver/tests/
+-rw-r--r--   0 niteris    (501) staff       (20)        0 2022-05-25 01:01:32.000000 open_webdriver-1.4.3/open_webdriver/tests/__init__.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-19 03:05:16.800848 open_webdriver-1.4.3/open_webdriver/tests/unit/
+-rw-r--r--   0 niteris    (501) staff       (20)        0 2022-05-25 01:01:32.000000 open_webdriver-1.4.3/open_webdriver/tests/unit/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1796 2023-06-18 23:37:52.000000 open_webdriver-1.4.3/open_webdriver/tests/unit/test_webdriver.py
+-rw-r--r--   0 niteris    (501) staff       (20)       64 2023-06-18 23:54:06.000000 open_webdriver-1.4.3/open_webdriver/version.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-19 03:05:16.800313 open_webdriver-1.4.3/open_webdriver.egg-info/
+-rw-r--r--   0 niteris    (501) staff       (20)     8072 2023-06-19 03:05:16.000000 open_webdriver-1.4.3/open_webdriver.egg-info/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      587 2023-06-19 03:05:16.000000 open_webdriver-1.4.3/open_webdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        1 2023-06-19 03:05:16.000000 open_webdriver-1.4.3/open_webdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       60 2023-06-19 03:05:16.000000 open_webdriver-1.4.3/open_webdriver.egg-info/entry_points.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      119 2023-06-19 03:05:16.000000 open_webdriver-1.4.3/open_webdriver.egg-info/requires.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       15 2023-06-19 03:05:16.000000 open_webdriver-1.4.3/open_webdriver.egg-info/top_level.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       43 2023-06-18 23:26:27.000000 open_webdriver-1.4.3/requirements.testing.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      103 2023-06-19 01:31:12.000000 open_webdriver-1.4.3/requirements.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       38 2023-06-19 03:05:16.802414 open_webdriver-1.4.3/setup.cfg
+-rw-r--r--   0 niteris    (501) staff       (20)     3025 2022-05-25 01:01:32.000000 open_webdriver-1.4.3/setup.py
```

### Comparing `open_webdriver-1.4.2/LICENSE` & `open_webdriver-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_webdriver-1.4.2/PKG-INFO` & `open_webdriver-1.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,164 +1,166 @@
-Metadata-Version: 2.1
-Name: open_webdriver
-Version: 1.4.2
-Summary: Easiest zero-config selenium webdriver for Python
-Home-page: https://github.com/zackees/open-webdriver
-Author: Zach Vorhies
-Author-email: dont@email.me
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Environment :: Console
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-# open-webdriver
-
-## The simplest and easiest way to get a selenium webdriver running
-
-# API
-
-```bash
-python -m pip install open-webdriver
-```
-
-```python
-from open_webdriver import open_webdriver
-
-def main():
-    with open_webdriver(headless=False) as driver:
-        # All Chromium / web driver dependencies are now installed.
-        driver.get("https://www.google.com")
-        assert driver.title == "Google"
-
-if __name__ == "__main__":
-    main()
-```
-
-#### Platform Unit Tests
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_macos.yml)
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Win_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_win.yml)
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu.yml)
-
-#### Platform binary nuitka build
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/MacOS_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_macos_nuitka.yml)
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Win_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_win_nuitka.yml)
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu_nuitka.yml)
-
-#### Ubuntu Install Tests
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Test_Install/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu_install.yml)
-
-
-# Versions
-
-Mac/Windows/Linux all use chromium version 101.0.4951.41
-The user agent string will always indicate a Windows client, unless overriden.
-
-# About
-
-Yet another selenium webdriver wrapper API in python, with the aims of being the easist to use with only two lines of code to get running.
-
-Unlike other selenium web driver wrappers, this one **has tests for Windows10/MacOS/Ubuntu platforms**.
-
-One function is provided, `open_webdriver(...)` which takes care of downloading, installing and then running selenium.
-
-Additionally, sane defaults are set, such as headless by default and ssl certs turned off. This code is also tested and examples are provided for use with the nuitka cross compiler, which allows you to create an binary executable. This is great for distributing a compiled binary
-for Windows/MacOS/Ubuntu of your selenium bot with all original source code removed, making it impossible to reverse engineer.
-
-
-`open-webdriver` is built on top of webdriver-manager https://pypi.org/project/webdriver-manager/ library, but with the following changes/fixes:
-```python
-os.environ['WDM_SSL_VERIFY'] = '0'
-```
-
-And other sensible platform specific fixes are applied in order for the selenium driver stack to pass the test suite.
-
-Additionally, a versioned chromium binary is downloaded for Linux & Windows, while whatever Chrome system is used for Mac, due to app signing requirements.
-
-When your app is launched, there will be a side folder name `.wdm` which contain the download of the webdriver used and brawser used. The disk cache for the driver is set for 7 day, after which it will be checked for a new version.
-
-Benefits:
-
-  * Production ready. Cross platform tests.
-  * ssl certs are turned off to reduce errors for many websites.
-  * Downloading the proper binary for your platform and stashing it next to the app.
-  * Headless by default.
-  * Intelligently forces headless in a linux environment without a display card (prevents crash).
-  * Platform tests to ensure a stable cross platform experience.
-  * Pins to a specific version of selenium driver stack to ensure reproducable behavior.
-  * Nuitka Binary Builds for all platforms are tested.
-
-Downsides:
-
-  * Only chrome is supported right now.
-
-
-# Tests
-
-#### Dev:
-
-Just simply run `tox` at the command line and everything should be tested. You may need to install `tox` with `python -m pip tox`.
-
-#### Package Test:
-
-Run `open_webdriver_test` for package tests. This is useful if you are on a server and want to figure out if open_webdriver will be able to be run in
-headless mode using the `chrome` driver.
-
-# Docker
-
-Please see `Dockerfile` for requirements for including `open_webdriver` in your Docker app.
-
-Docker is supported in this build. Please see the `Dockerfile` and `docker-compose.yml` for bringup instructions. Simply use `docker-compose up` and then ssh into the docker instance and run `open_webdriver_test` and verify that the test completes normally.
-
-# Nuitka
-
-This package supports the Nuitka cross compiler to binary app. However to make this work YOU MUST include the package data for selenium or you will get errors about missing javascript files when the program loads. To get around this you'll need to add package data:
-
-`python -m nuitka --include-package-data=selenium ...`
-
-For example see the example build file:
-[https://github.com/zackees/open-webdriver/blob/main/open_webdriver/tests/nuitka/test_binary_build.py](https://github.com/zackees/open-webdriver/blob/main/open_webdriver/tests/nuitka/test_binary_build.py)
-
-# Pull Requests
-
-
-Pull requests are welcome for this code base. When you submit your pull request you will need to have the following:
-  * New code must have a unit/test.
-  * Must pass the linting requirements. Run `tox` (also run on your pull request).
-
-# Changes
-  * 1.4.2: Prints log if chrome driver fails to launch.
-  * 1.4.1: Try and fix failed upload on last version.
-  * 1.4.0: Adds default user agent string, fixes running headless mode which uses a different user agent string.
-  * 1.3.6: Remove mac m1 runner, which doesn't exist on github
-  * 1.3.5: Fixes macOS builds, now uses versioned macOS Chromium.
-  * 1.3.4: Fixes nuitka builds that broke with panda's update. Nuitka updated from 0.7.7->1.2.2
-  * 1.3.3: Adds user_agent.
-  * 1.3.2: Adds disable_dev_shm_usage.
-  * 1.3.1: Adds disable gpu.
-  * 1.3.0: Concurrent support added for open_webdriver() using a lockfile.
-  * 1.2.9: Sets downloaded chromedriver version to 101.0.4951.41
-  * 1.2.8: Docker support has been added.
-  * 1.2.3: Fix bug in 7za unarchiver path.
-  * 1.2.2: 7za unarchiver is now included.
-  * 1.2.1: Bug fixes and other improvements that easy deployment.
-  * 1.2.0: All platforms supported now. Linux / Win32 now downloads a chromioum browser. Firefox has been removed.
-  * 1.1.14: Fixes bugs for `open_webdriver_test` cmd
-  * 1.1.10: Adds package test `open_webdriver_test` cmd
-  * 1.1.9: Moves tests into package to allow running tests from package.
-  * 1.1.8: Minor fixes
-  * 1.1.7: Nit readme.
-  * 1.1.6: Fixes failing win-tox tests due to missing "PROGRAMW6432" value in os.environ (?!). Brave browser removed as it actually didn't work.
-  * 1.1.5: Cert warnings now suppressable with non headless sessions.
-  * 1.1.3: Suppress more cert warnings.
-  * 1.1.2: Suppress certificate warnings.
-  * 1.1.1: Update readme.
-  * 1.1.0: Platform binary builds using nuitka are now tested.
-  * 1.0.4: Now pins dependencies.
-  * 1.0.0: Initial code submit.
+Metadata-Version: 2.1
+Name: open_webdriver
+Version: 1.4.3
+Summary: Easiest zero-config selenium webdriver for Python
+Home-page: https://github.com/zackees/open-webdriver
+Author: Zach Vorhies
+Author-email: dont@email.me
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Environment :: Console
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# open-webdriver
+
+## The simplest and easiest way to get a scriptable chrome browser running using selenium webdriver running.
+
+Note that this package uses a pinned dependency for urllib3 and should be installed in an isolated environment.
+
+# API
+
+```bash
+python -m pip install open-webdriver
+```
+
+```python
+from open_webdriver import open_webdriver
+
+def main():
+    with open_webdriver(headless=False) as driver:
+        # All Chromium / web driver dependencies are now installed.
+        driver.get("https://www.google.com")
+        assert driver.title == "Google"
+
+if __name__ == "__main__":
+    main()
+```
+
+#### Platform Unit Tests
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_macos.yml)
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Win_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_win.yml)
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu.yml)
+
+#### Platform binary nuitka build
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/MacOS_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_macos_nuitka.yml)
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Win_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_win_nuitka.yml)
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu_nuitka.yml)
+
+#### Ubuntu Install Tests
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Test_Install/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu_install.yml)
+
+
+# Versions
+
+Mac/Windows/Linux all use chromium version 101.0.4951.41
+The user agent string will always indicate a Windows client, unless overriden.
+
+# About
+
+Yet another selenium webdriver wrapper API in python, with the aims of being the easist to use with only two lines of code to get running.
+
+Unlike other selenium web driver wrappers, this one **has tests for Windows10/MacOS/Ubuntu platforms**.
+
+One function is provided, `open_webdriver(...)` which takes care of downloading, installing and then running selenium.
+
+Additionally, sane defaults are set, such as headless by default and ssl certs turned off. This code is also tested and examples are provided for use with the nuitka cross compiler, which allows you to create an binary executable. This is great for distributing a compiled binary
+for Windows/MacOS/Ubuntu of your selenium bot with all original source code removed, making it impossible to reverse engineer.
+
+
+`open-webdriver` is built on top of webdriver-manager https://pypi.org/project/webdriver-manager/ library, but with the following changes/fixes:
+```python
+os.environ['WDM_SSL_VERIFY'] = '0'
+```
+
+And other sensible platform specific fixes are applied in order for the selenium driver stack to pass the test suite.
+
+Additionally, a versioned chromium binary is downloaded for Linux & Windows, while whatever Chrome system is used for Mac, due to app signing requirements.
+
+When your app is launched, there will be a side folder name `.wdm` which contain the download of the webdriver used and brawser used. The disk cache for the driver is set for 7 day, after which it will be checked for a new version.
+
+Benefits:
+
+  * Production ready. Cross platform tests.
+  * ssl certs are turned off to reduce errors for many websites.
+  * Downloading the proper binary for your platform and stashing it next to the app.
+  * Headless by default.
+  * Intelligently forces headless in a linux environment without a display card (prevents crash).
+  * Platform tests to ensure a stable cross platform experience.
+  * Pins to a specific version of selenium driver stack to ensure reproducable behavior.
+  * Nuitka Binary Builds for all platforms are tested.
+
+Downsides:
+
+  * Only chrome is supported right now.
+
+
+# Tests
+
+#### Dev:
+
+Just simply run `tox` at the command line and everything should be tested. You may need to install `tox` with `python -m pip tox`.
+
+#### Package Test:
+
+Run `open_webdriver_test` for package tests. This is useful if you are on a server and want to figure out if open_webdriver will be able to be run in
+headless mode using the `chrome` driver.
+
+# Docker
+
+Please see `Dockerfile` for requirements for including `open_webdriver` in your Docker app.
+
+Docker is supported in this build. Please see the `Dockerfile` and `docker-compose.yml` for bringup instructions. Simply use `docker-compose up` and then ssh into the docker instance and run `open_webdriver_test` and verify that the test completes normally.
+
+# Nuitka
+
+This package supports the Nuitka cross compiler to binary app. However to make this work YOU MUST include the package data for selenium or you will get errors about missing javascript files when the program loads. To get around this you'll need to add package data:
+
+`python -m nuitka --include-package-data=selenium ...`
+
+For example see the example build file:
+[https://github.com/zackees/open-webdriver/blob/main/open_webdriver/tests/nuitka/test_binary_build.py](https://github.com/zackees/open-webdriver/blob/main/open_webdriver/tests/nuitka/test_binary_build.py)
+
+# Pull Requests
+
+
+Pull requests are welcome for this code base. When you submit your pull request you will need to have the following:
+  * New code must have a unit/test.
+  * Must pass the linting requirements. Run `tox` (also run on your pull request).
+
+# Changes
+  * 1.4.2: Prints log if chrome driver fails to launch.
+  * 1.4.1: Try and fix failed upload on last version.
+  * 1.4.0: Adds default user agent string, fixes running headless mode which uses a different user agent string.
+  * 1.3.6: Remove mac m1 runner, which doesn't exist on github
+  * 1.3.5: Fixes macOS builds, now uses versioned macOS Chromium.
+  * 1.3.4: Fixes nuitka builds that broke with panda's update. Nuitka updated from 0.7.7->1.2.2
+  * 1.3.3: Adds user_agent.
+  * 1.3.2: Adds disable_dev_shm_usage.
+  * 1.3.1: Adds disable gpu.
+  * 1.3.0: Concurrent support added for open_webdriver() using a lockfile.
+  * 1.2.9: Sets downloaded chromedriver version to 101.0.4951.41
+  * 1.2.8: Docker support has been added.
+  * 1.2.3: Fix bug in 7za unarchiver path.
+  * 1.2.2: 7za unarchiver is now included.
+  * 1.2.1: Bug fixes and other improvements that easy deployment.
+  * 1.2.0: All platforms supported now. Linux / Win32 now downloads a chromioum browser. Firefox has been removed.
+  * 1.1.14: Fixes bugs for `open_webdriver_test` cmd
+  * 1.1.10: Adds package test `open_webdriver_test` cmd
+  * 1.1.9: Moves tests into package to allow running tests from package.
+  * 1.1.8: Minor fixes
+  * 1.1.7: Nit readme.
+  * 1.1.6: Fixes failing win-tox tests due to missing "PROGRAMW6432" value in os.environ (?!). Brave browser removed as it actually didn't work.
+  * 1.1.5: Cert warnings now suppressable with non headless sessions.
+  * 1.1.3: Suppress more cert warnings.
+  * 1.1.2: Suppress certificate warnings.
+  * 1.1.1: Update readme.
+  * 1.1.0: Platform binary builds using nuitka are now tested.
+  * 1.0.4: Now pins dependencies.
+  * 1.0.0: Initial code submit.
```

### Comparing `open_webdriver-1.4.2/README.md` & `open_webdriver-1.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # open-webdriver
 
-## The simplest and easiest way to get a selenium webdriver running
+## The simplest and easiest way to get a scriptable chrome browser running using selenium webdriver running.
+
+Note that this package uses a pinned dependency for urllib3 and should be installed in an isolated environment.
 
 # API
 
 ```bash
 python -m pip install open-webdriver
 ```
```

### Comparing `open_webdriver-1.4.2/open_webdriver/download_chromium.py` & `open_webdriver-1.4.3/open_webdriver/download_chromium.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 """
 Module to download the Chromium browser from the repo.
 """
 
+# flake8: noqa F401
+# pylint: disable=unused-import
+
 import os
 import subprocess
 import sys
 import zipfile
+import lzma  # type: ignore # must be included for nuitka build
 
 from download import download  # type: ignore
+import six  # type: ignore # must be included for nuitka build
+import certifi  # type: ignore # must be included for nuitka build
+
 
 from open_webdriver.path import WDM_CHROMIUM_DIR
 
 
 def _set_exe_permissions(start_dir: str) -> None:
     """Sets the permissions on the chromium executable."""
     if sys.platform == "win32":
         return
     for root, _, files in os.walk(start_dir):
         for file_name in files:
             path = os.path.join(root, file_name)
             os.chmod(path, 0o755)
 
 
+def _download(url: str, path: str) -> str:
+    """Downloads a file from a url to a path."""
+
+    path = download(url=url, path=path, kind="file", progressbar=True, replace=True, timeout=5 * 60)
+    return path
+
+
 def _unzip(zip_path: str) -> None:
     """Unzips a zip file."""
 
     if sys.platform == "linux":
         print("Linux detected.")
         url = "https://github.com/zackees/open-webdriver/raw/main/chromium/7za"
         dst = os.path.join(WDM_CHROMIUM_DIR, "7za")
-        path_7za = download(url=url, path=dst, kind="file", progressbar=True, replace=True)
+        path_7za = _download(url=url, path=dst)
         path_7za = os.path.abspath(path_7za)
         assert os.path.exists(path_7za), f"{path_7za} does not exist."
         # Add executable permissions.
         os.chmod(path_7za, 0o755)
         print("Using 7za tool")
         try:
             zip_name = os.path.basename(zip_path)
@@ -70,15 +84,15 @@
     platform_dir = os.path.join(WDM_CHROMIUM_DIR, sys.platform)
     print(f"WDM_CHROMIUM_DIR: {WDM_CHROMIUM_DIR}")
     finished_stamp = os.path.join(platform_dir, "finished")
     if not os.path.exists(finished_stamp):
         ext = ".7z" if sys.platform == "darwin" else ".zip"
         archive_dst = platform_dir + ext
         print(f"Download {url_src} to {archive_dst}")
-        download(url=url_src, path=archive_dst, kind="file", progressbar=True, replace=False)
+        _download(url=url_src, path=archive_dst)
         assert os.path.exists(archive_dst), f"{archive_dst} does not exist."
         print(f"Unzipping {archive_dst}")
         _unzip(zip_path=archive_dst)
         print(f"Fixing permissions {platform_dir}")
         _set_exe_permissions(platform_dir)
         # Touch file.
         print(f"Touching file: {finished_stamp}")
```

### Comparing `open_webdriver-1.4.2/open_webdriver/open_webdriver.py` & `open_webdriver-1.4.3/open_webdriver/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,17 @@
             cache_valid_range=CACHE_TIMEOUT_DAYS, version=CHROME_VERSION, path=WDM_DIR
         ).install()
     if verbose:
         print(f"\n  Using ChromeDriver: {driver_path}")
     try:
         if os.path.exists(LOG_FILE):
             os.remove(LOG_FILE)
-        driver = webdriver.Chrome(driver_path, options=opts, service_log_path=LOG_FILE)
+        driver = webdriver.Chrome(
+            executable_path=driver_path, options=opts, service_log_path=LOG_FILE
+        )
         return driver
     except Exception as err:  # pylint: disable=broad-except
         traceback.print_exc()
         log_file_text = ""
         if os.path.exists(LOG_FILE):
             with open(LOG_FILE, encoding="utf-8", mode="r") as filed:
                 log_file_text = filed.read()
```

### Comparing `open_webdriver-1.4.2/open_webdriver/tests/unit/test_webdriver.py` & `open_webdriver-1.4.3/open_webdriver/tests/unit/test_webdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     Tests the open_webdriver package.
 """
 
 import argparse
 import unittest
 
-from open_webdriver.open_webdriver import open_webdriver
+from open_webdriver.main import open_webdriver
 
 
 def do_google_test(headless: bool) -> bool:
     """Runs the tests for a given driver."""
     with open_webdriver(headless=headless, verbose=True) as driver:
         driver.get("https://www.google.com")
         return driver.title == "Google"
```

### Comparing `open_webdriver-1.4.2/open_webdriver.egg-info/PKG-INFO` & `open_webdriver-1.4.3/open_webdriver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,164 +1,166 @@
-Metadata-Version: 2.1
-Name: open-webdriver
-Version: 1.4.2
-Summary: Easiest zero-config selenium webdriver for Python
-Home-page: https://github.com/zackees/open-webdriver
-Author: Zach Vorhies
-Author-email: dont@email.me
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Environment :: Console
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-# open-webdriver
-
-## The simplest and easiest way to get a selenium webdriver running
-
-# API
-
-```bash
-python -m pip install open-webdriver
-```
-
-```python
-from open_webdriver import open_webdriver
-
-def main():
-    with open_webdriver(headless=False) as driver:
-        # All Chromium / web driver dependencies are now installed.
-        driver.get("https://www.google.com")
-        assert driver.title == "Google"
-
-if __name__ == "__main__":
-    main()
-```
-
-#### Platform Unit Tests
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_macos.yml)
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Win_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_win.yml)
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu.yml)
-
-#### Platform binary nuitka build
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/MacOS_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_macos_nuitka.yml)
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Win_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_win_nuitka.yml)
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu_nuitka.yml)
-
-#### Ubuntu Install Tests
-[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Test_Install/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu_install.yml)
-
-
-# Versions
-
-Mac/Windows/Linux all use chromium version 101.0.4951.41
-The user agent string will always indicate a Windows client, unless overriden.
-
-# About
-
-Yet another selenium webdriver wrapper API in python, with the aims of being the easist to use with only two lines of code to get running.
-
-Unlike other selenium web driver wrappers, this one **has tests for Windows10/MacOS/Ubuntu platforms**.
-
-One function is provided, `open_webdriver(...)` which takes care of downloading, installing and then running selenium.
-
-Additionally, sane defaults are set, such as headless by default and ssl certs turned off. This code is also tested and examples are provided for use with the nuitka cross compiler, which allows you to create an binary executable. This is great for distributing a compiled binary
-for Windows/MacOS/Ubuntu of your selenium bot with all original source code removed, making it impossible to reverse engineer.
-
-
-`open-webdriver` is built on top of webdriver-manager https://pypi.org/project/webdriver-manager/ library, but with the following changes/fixes:
-```python
-os.environ['WDM_SSL_VERIFY'] = '0'
-```
-
-And other sensible platform specific fixes are applied in order for the selenium driver stack to pass the test suite.
-
-Additionally, a versioned chromium binary is downloaded for Linux & Windows, while whatever Chrome system is used for Mac, due to app signing requirements.
-
-When your app is launched, there will be a side folder name `.wdm` which contain the download of the webdriver used and brawser used. The disk cache for the driver is set for 7 day, after which it will be checked for a new version.
-
-Benefits:
-
-  * Production ready. Cross platform tests.
-  * ssl certs are turned off to reduce errors for many websites.
-  * Downloading the proper binary for your platform and stashing it next to the app.
-  * Headless by default.
-  * Intelligently forces headless in a linux environment without a display card (prevents crash).
-  * Platform tests to ensure a stable cross platform experience.
-  * Pins to a specific version of selenium driver stack to ensure reproducable behavior.
-  * Nuitka Binary Builds for all platforms are tested.
-
-Downsides:
-
-  * Only chrome is supported right now.
-
-
-# Tests
-
-#### Dev:
-
-Just simply run `tox` at the command line and everything should be tested. You may need to install `tox` with `python -m pip tox`.
-
-#### Package Test:
-
-Run `open_webdriver_test` for package tests. This is useful if you are on a server and want to figure out if open_webdriver will be able to be run in
-headless mode using the `chrome` driver.
-
-# Docker
-
-Please see `Dockerfile` for requirements for including `open_webdriver` in your Docker app.
-
-Docker is supported in this build. Please see the `Dockerfile` and `docker-compose.yml` for bringup instructions. Simply use `docker-compose up` and then ssh into the docker instance and run `open_webdriver_test` and verify that the test completes normally.
-
-# Nuitka
-
-This package supports the Nuitka cross compiler to binary app. However to make this work YOU MUST include the package data for selenium or you will get errors about missing javascript files when the program loads. To get around this you'll need to add package data:
-
-`python -m nuitka --include-package-data=selenium ...`
-
-For example see the example build file:
-[https://github.com/zackees/open-webdriver/blob/main/open_webdriver/tests/nuitka/test_binary_build.py](https://github.com/zackees/open-webdriver/blob/main/open_webdriver/tests/nuitka/test_binary_build.py)
-
-# Pull Requests
-
-
-Pull requests are welcome for this code base. When you submit your pull request you will need to have the following:
-  * New code must have a unit/test.
-  * Must pass the linting requirements. Run `tox` (also run on your pull request).
-
-# Changes
-  * 1.4.2: Prints log if chrome driver fails to launch.
-  * 1.4.1: Try and fix failed upload on last version.
-  * 1.4.0: Adds default user agent string, fixes running headless mode which uses a different user agent string.
-  * 1.3.6: Remove mac m1 runner, which doesn't exist on github
-  * 1.3.5: Fixes macOS builds, now uses versioned macOS Chromium.
-  * 1.3.4: Fixes nuitka builds that broke with panda's update. Nuitka updated from 0.7.7->1.2.2
-  * 1.3.3: Adds user_agent.
-  * 1.3.2: Adds disable_dev_shm_usage.
-  * 1.3.1: Adds disable gpu.
-  * 1.3.0: Concurrent support added for open_webdriver() using a lockfile.
-  * 1.2.9: Sets downloaded chromedriver version to 101.0.4951.41
-  * 1.2.8: Docker support has been added.
-  * 1.2.3: Fix bug in 7za unarchiver path.
-  * 1.2.2: 7za unarchiver is now included.
-  * 1.2.1: Bug fixes and other improvements that easy deployment.
-  * 1.2.0: All platforms supported now. Linux / Win32 now downloads a chromioum browser. Firefox has been removed.
-  * 1.1.14: Fixes bugs for `open_webdriver_test` cmd
-  * 1.1.10: Adds package test `open_webdriver_test` cmd
-  * 1.1.9: Moves tests into package to allow running tests from package.
-  * 1.1.8: Minor fixes
-  * 1.1.7: Nit readme.
-  * 1.1.6: Fixes failing win-tox tests due to missing "PROGRAMW6432" value in os.environ (?!). Brave browser removed as it actually didn't work.
-  * 1.1.5: Cert warnings now suppressable with non headless sessions.
-  * 1.1.3: Suppress more cert warnings.
-  * 1.1.2: Suppress certificate warnings.
-  * 1.1.1: Update readme.
-  * 1.1.0: Platform binary builds using nuitka are now tested.
-  * 1.0.4: Now pins dependencies.
-  * 1.0.0: Initial code submit.
+Metadata-Version: 2.1
+Name: open-webdriver
+Version: 1.4.3
+Summary: Easiest zero-config selenium webdriver for Python
+Home-page: https://github.com/zackees/open-webdriver
+Author: Zach Vorhies
+Author-email: dont@email.me
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Environment :: Console
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# open-webdriver
+
+## The simplest and easiest way to get a scriptable chrome browser running using selenium webdriver running.
+
+Note that this package uses a pinned dependency for urllib3 and should be installed in an isolated environment.
+
+# API
+
+```bash
+python -m pip install open-webdriver
+```
+
+```python
+from open_webdriver import open_webdriver
+
+def main():
+    with open_webdriver(headless=False) as driver:
+        # All Chromium / web driver dependencies are now installed.
+        driver.get("https://www.google.com")
+        assert driver.title == "Google"
+
+if __name__ == "__main__":
+    main()
+```
+
+#### Platform Unit Tests
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_macos.yml)
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Win_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_win.yml)
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu.yml)
+
+#### Platform binary nuitka build
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/MacOS_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_macos_nuitka.yml)
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Win_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_win_nuitka.yml)
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Nuitka/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu_nuitka.yml)
+
+#### Ubuntu Install Tests
+[![Actions Status](https://github.com/zackees/open-webdriver/workflows/Ubuntu_Test_Install/badge.svg)](https://github.com/zackees/open-webdriver/actions/workflows/test_ubuntu_install.yml)
+
+
+# Versions
+
+Mac/Windows/Linux all use chromium version 101.0.4951.41
+The user agent string will always indicate a Windows client, unless overriden.
+
+# About
+
+Yet another selenium webdriver wrapper API in python, with the aims of being the easist to use with only two lines of code to get running.
+
+Unlike other selenium web driver wrappers, this one **has tests for Windows10/MacOS/Ubuntu platforms**.
+
+One function is provided, `open_webdriver(...)` which takes care of downloading, installing and then running selenium.
+
+Additionally, sane defaults are set, such as headless by default and ssl certs turned off. This code is also tested and examples are provided for use with the nuitka cross compiler, which allows you to create an binary executable. This is great for distributing a compiled binary
+for Windows/MacOS/Ubuntu of your selenium bot with all original source code removed, making it impossible to reverse engineer.
+
+
+`open-webdriver` is built on top of webdriver-manager https://pypi.org/project/webdriver-manager/ library, but with the following changes/fixes:
+```python
+os.environ['WDM_SSL_VERIFY'] = '0'
+```
+
+And other sensible platform specific fixes are applied in order for the selenium driver stack to pass the test suite.
+
+Additionally, a versioned chromium binary is downloaded for Linux & Windows, while whatever Chrome system is used for Mac, due to app signing requirements.
+
+When your app is launched, there will be a side folder name `.wdm` which contain the download of the webdriver used and brawser used. The disk cache for the driver is set for 7 day, after which it will be checked for a new version.
+
+Benefits:
+
+  * Production ready. Cross platform tests.
+  * ssl certs are turned off to reduce errors for many websites.
+  * Downloading the proper binary for your platform and stashing it next to the app.
+  * Headless by default.
+  * Intelligently forces headless in a linux environment without a display card (prevents crash).
+  * Platform tests to ensure a stable cross platform experience.
+  * Pins to a specific version of selenium driver stack to ensure reproducable behavior.
+  * Nuitka Binary Builds for all platforms are tested.
+
+Downsides:
+
+  * Only chrome is supported right now.
+
+
+# Tests
+
+#### Dev:
+
+Just simply run `tox` at the command line and everything should be tested. You may need to install `tox` with `python -m pip tox`.
+
+#### Package Test:
+
+Run `open_webdriver_test` for package tests. This is useful if you are on a server and want to figure out if open_webdriver will be able to be run in
+headless mode using the `chrome` driver.
+
+# Docker
+
+Please see `Dockerfile` for requirements for including `open_webdriver` in your Docker app.
+
+Docker is supported in this build. Please see the `Dockerfile` and `docker-compose.yml` for bringup instructions. Simply use `docker-compose up` and then ssh into the docker instance and run `open_webdriver_test` and verify that the test completes normally.
+
+# Nuitka
+
+This package supports the Nuitka cross compiler to binary app. However to make this work YOU MUST include the package data for selenium or you will get errors about missing javascript files when the program loads. To get around this you'll need to add package data:
+
+`python -m nuitka --include-package-data=selenium ...`
+
+For example see the example build file:
+[https://github.com/zackees/open-webdriver/blob/main/open_webdriver/tests/nuitka/test_binary_build.py](https://github.com/zackees/open-webdriver/blob/main/open_webdriver/tests/nuitka/test_binary_build.py)
+
+# Pull Requests
+
+
+Pull requests are welcome for this code base. When you submit your pull request you will need to have the following:
+  * New code must have a unit/test.
+  * Must pass the linting requirements. Run `tox` (also run on your pull request).
+
+# Changes
+  * 1.4.2: Prints log if chrome driver fails to launch.
+  * 1.4.1: Try and fix failed upload on last version.
+  * 1.4.0: Adds default user agent string, fixes running headless mode which uses a different user agent string.
+  * 1.3.6: Remove mac m1 runner, which doesn't exist on github
+  * 1.3.5: Fixes macOS builds, now uses versioned macOS Chromium.
+  * 1.3.4: Fixes nuitka builds that broke with panda's update. Nuitka updated from 0.7.7->1.2.2
+  * 1.3.3: Adds user_agent.
+  * 1.3.2: Adds disable_dev_shm_usage.
+  * 1.3.1: Adds disable gpu.
+  * 1.3.0: Concurrent support added for open_webdriver() using a lockfile.
+  * 1.2.9: Sets downloaded chromedriver version to 101.0.4951.41
+  * 1.2.8: Docker support has been added.
+  * 1.2.3: Fix bug in 7za unarchiver path.
+  * 1.2.2: 7za unarchiver is now included.
+  * 1.2.1: Bug fixes and other improvements that easy deployment.
+  * 1.2.0: All platforms supported now. Linux / Win32 now downloads a chromioum browser. Firefox has been removed.
+  * 1.1.14: Fixes bugs for `open_webdriver_test` cmd
+  * 1.1.10: Adds package test `open_webdriver_test` cmd
+  * 1.1.9: Moves tests into package to allow running tests from package.
+  * 1.1.8: Minor fixes
+  * 1.1.7: Nit readme.
+  * 1.1.6: Fixes failing win-tox tests due to missing "PROGRAMW6432" value in os.environ (?!). Brave browser removed as it actually didn't work.
+  * 1.1.5: Cert warnings now suppressable with non headless sessions.
+  * 1.1.3: Suppress more cert warnings.
+  * 1.1.2: Suppress certificate warnings.
+  * 1.1.1: Update readme.
+  * 1.1.0: Platform binary builds using nuitka are now tested.
+  * 1.0.4: Now pins dependencies.
+  * 1.0.0: Initial code submit.
```

### Comparing `open_webdriver-1.4.2/open_webdriver.egg-info/SOURCES.txt` & `open_webdriver-1.4.3/open_webdriver.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 README.md
 requirements.testing.txt
 requirements.txt
 setup.py
 open_webdriver/__init__.py
 open_webdriver/demo_app.py
 open_webdriver/download_chromium.py
-open_webdriver/open_webdriver.py
+open_webdriver/main.py
 open_webdriver/path.py
 open_webdriver/version.py
 open_webdriver.egg-info/PKG-INFO
 open_webdriver.egg-info/SOURCES.txt
 open_webdriver.egg-info/dependency_links.txt
 open_webdriver.egg-info/entry_points.txt
 open_webdriver.egg-info/requires.txt
```

### Comparing `open_webdriver-1.4.2/setup.py` & `open_webdriver-1.4.3/setup.py`

 * *Files identical despite different names*

