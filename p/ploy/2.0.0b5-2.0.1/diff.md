# Comparing `tmp/ploy-2.0.0b5.tar.gz` & `tmp/ploy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ploy-2.0.0b5.tar", last modified: Sat Jul 17 08:45:38 2021, max compression
+gzip compressed data, was "dist/ploy-2.0.1.tar", last modified: Mon Jun 19 08:42:19 2023, max compression
```

## Comparing `ploy-2.0.0b5.tar` & `ploy-2.0.1.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-07-17 08:45:38.000000 ploy-2.0.0b5/
--rw-r--r--   0 fschulze   (501) staff       (20)    28681 2021-07-17 08:45:38.000000 ploy-2.0.0b5/PKG-INFO
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy_pytest_plugin/
--rw-r--r--   0 fschulze   (501) staff       (20)     4997 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy_pytest_plugin/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       72 2021-07-17 08:45:37.000000 ploy-2.0.0b5/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     1657 2021-07-17 08:45:37.000000 ploy-2.0.0b5/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy/
--rw-r--r--   0 fschulze   (501) staff       (20)    31997 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/config.py
--rw-r--r--   0 fschulze   (501) staff       (20)      193 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/hookspecs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2016 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/proxy.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy/tests/
--rw-r--r--   0 fschulze   (501) staff       (20)    15561 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/test_common.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3183 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/dummy_plugin.py
--rw-r--r--   0 fschulze   (501) staff       (20)    18996 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/test_plain.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1010 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/dummy_proxy_plugin.py
--rw-r--r--   0 fschulze   (501) staff       (20)        2 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)    26882 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/test_ploy.py
--rw-r--r--   0 fschulze   (501) staff       (20)    23478 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/test_config.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3495 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/test_proxy.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3126 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/tests/test_template.py
--rw-r--r--   0 fschulze   (501) staff       (20)    25205 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)    21029 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/common.py
--rw-r--r--   0 fschulze   (501) staff       (20)    12092 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/plain.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2146 2021-07-17 08:45:37.000000 ploy-2.0.0b5/ploy/template.py
--rw-r--r--   0 fschulze   (501) staff       (20)    13569 2021-07-17 08:45:37.000000 ploy-2.0.0b5/HISTORY.rst
--rw-r--r--   0 fschulze   (501) staff       (20)      372 2021-07-17 08:45:37.000000 ploy-2.0.0b5/tox.ini
--rw-r--r--   0 fschulze   (501) staff       (20)      115 2021-07-17 08:45:38.000000 ploy-2.0.0b5/setup.cfg
--rw-r--r--   0 fschulze   (501) staff       (20)     7489 2021-07-17 08:45:37.000000 ploy-2.0.0b5/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)    28681 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy.egg-info/not-zip-safe
--rw-r--r--   0 fschulze   (501) staff       (20)      636 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      213 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       50 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       24 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2021-07-17 08:45:38.000000 ploy-2.0.0b5/ploy.egg-info/dependency_links.txt
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-06-19 08:42:19.639633 ploy-2.0.1/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-06-19 08:42:19.620690 ploy-2.0.1/.github/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-06-19 08:42:19.624733 ploy-2.0.1/.github/workflows/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1155 2022-08-17 11:12:42.000000 ploy-2.0.1/.github/workflows/main.yml
+-rw-r--r--   0 fschulze   (501) staff       (20)      218 2022-08-17 11:12:39.000000 ploy-2.0.1/.travis.yml
+-rw-r--r--   0 fschulze   (501) staff       (20)    14010 2023-06-19 08:41:52.000000 ploy-2.0.1/HISTORY.rst
+-rw-r--r--   0 fschulze   (501) staff       (20)     1486 2014-07-02 12:36:21.000000 ploy-2.0.1/LICENSE.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       72 2014-06-20 13:22:40.000000 ploy-2.0.1/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)    22401 2023-06-19 08:42:19.639847 ploy-2.0.1/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     7489 2018-02-03 12:57:42.000000 ploy-2.0.1/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-06-19 08:42:19.630556 ploy-2.0.1/ploy/
+-rw-r--r--   0 fschulze   (501) staff       (20)    25622 2023-06-14 11:16:28.000000 ploy-2.0.1/ploy/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    22049 2023-06-19 08:34:49.000000 ploy-2.0.1/ploy/common.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    32171 2023-06-14 10:45:18.000000 ploy-2.0.1/ploy/config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      193 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/hookspecs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    12092 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/plain.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2016 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/proxy.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2146 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/template.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-06-19 08:42:19.638853 ploy-2.0.1/ploy/tests/
+-rw-r--r--   0 fschulze   (501) staff       (20)        2 2014-06-20 13:22:40.000000 ploy-2.0.1/ploy/tests/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3183 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/tests/dummy_plugin.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1010 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/tests/dummy_proxy_plugin.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    15555 2023-06-14 10:47:03.000000 ploy-2.0.1/ploy/tests/test_common.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    23478 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/tests/test_config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    18990 2023-06-14 10:47:08.000000 ploy-2.0.1/ploy/tests/test_plain.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    26882 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/tests/test_ploy.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3495 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/tests/test_proxy.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3126 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy/tests/test_template.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-06-19 08:42:19.633590 ploy-2.0.1/ploy.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)    22401 2023-06-19 08:42:19.000000 ploy-2.0.1/ploy.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      710 2023-06-19 08:42:19.000000 ploy-2.0.1/ploy.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-06-19 08:42:19.000000 ploy-2.0.1/ploy.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      154 2023-06-19 08:42:19.000000 ploy-2.0.1/ploy.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2014-06-20 13:53:03.000000 ploy-2.0.1/ploy.egg-info/not-zip-safe
+-rw-r--r--   0 fschulze   (501) staff       (20)       47 2015-04-28 09:51:26.000000 ploy-2.0.1/ploy.egg-info/pbr.json
+-rw-r--r--   0 fschulze   (501) staff       (20)       85 2023-06-19 08:42:19.000000 ploy-2.0.1/ploy.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       24 2023-06-19 08:42:19.000000 ploy-2.0.1/ploy.egg-info/top_level.txt
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-06-19 08:42:19.639230 ploy-2.0.1/ploy_pytest_plugin/
+-rw-r--r--   0 fschulze   (501) staff       (20)     4997 2022-08-17 11:12:42.000000 ploy-2.0.1/ploy_pytest_plugin/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      115 2023-06-19 08:42:19.640593 ploy-2.0.1/setup.cfg
+-rw-r--r--   0 fschulze   (501) staff       (20)     1694 2023-06-19 08:41:58.000000 ploy-2.0.1/setup.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      456 2022-08-17 11:15:02.000000 ploy-2.0.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ploy-2.0.0b5/ploy_pytest_plugin/__init__.py` & `ploy-2.0.1/ploy_pytest_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/setup.py` & `ploy-2.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from setuptools import setup
 import os
 
-version = "2.0.0b5"
+version = "2.0.1"
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.rst')).read()
 HISTORY = open(os.path.join(here, 'HISTORY.rst')).read()
 
 install_requires = [
     'attrs',
+    'importlib.metadata;python_version<"3.8"',
     'lazy',
     'paramiko',
     'pluggy',
-    'ruamel.yaml',
-    'setuptools']
+    'ruamel.yaml']
 
 setup(
     version=version,
     description="A tool to manage servers through a central configuration. Plugins allow provisioning, configuration and other management tasks.",
     long_description=README + "\n\n" + HISTORY,
     name="ploy",
     author='Florian Schulze',
     author_email='florian.schulze@gmx.net',
     license="BSD 3-Clause License",
     url='http://github.com/ployground/ploy',
     classifiers=[
         'Environment :: Console',
         'Intended Audience :: System Administrators',
         'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: System :: Installation/Setup',
         'Topic :: System :: Systems Administration'],
     include_package_data=True,
     zip_safe=False,
     packages=['ploy', 'ploy.tests', 'ploy_pytest_plugin'],
     install_requires=install_requires,
-    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
+    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*',
     entry_points="""
         [console_scripts]
         ploy = ploy:ploy
         ploy-ssh = ploy:ploy_ssh
         [ploy.plugins]
         plain = ploy.plain:plugin
         [pytest11]
```

### Comparing `ploy-2.0.0b5/ploy/config.py` & `ploy-2.0.1/ploy/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from __future__ import unicode_literals
 from ploy.common import Hooks
 try:
     import configparser
 except ImportError:  # pragma: nocover
     import ConfigParser as configparser  # for Python 2.7
-from collections import MutableMapping
+try:
+    from collections.abc import MutableMapping
+except ImportError:
+    from collections import MutableMapping
+try:
+    from inspect import getfullargspec
+except ImportError:
+    from inspect import getargspec as getfullargspec
 from io import BytesIO
 from ploy.common import split_option
 from pluggy import HookimplMarker
 from weakref import proxy
 import attr
-import inspect
 import logging
 import os
 import sys
 import warnings
 
 
 log = logging.getLogger('ploy')
@@ -210,15 +216,15 @@
     def _get_massager(self, key):
         if key in self._dict:
             if self._config is not None:
                 massage = self._config.massagers.get((self.sectiongroupname, key))
                 if not callable(massage):
                     massage = self._config.massagers.get((None, key))
                     if callable(massage):
-                        if len(inspect.getargspec(massage.__call__).args) == 3:
+                        if len(getfullargspec(massage.__call__).args) == 3:
                             return (massage, (self.sectionname,))
                         else:
                             return (massage, (self.sectiongroupname, self.sectionname))
                 else:
                     return (massage, (self.sectionname,))
             massage = self.massagers.get((self.sectiongroupname, key))
             if callable(massage):
```

### Comparing `ploy-2.0.0b5/ploy/proxy.py` & `ploy-2.0.1/ploy/proxy.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy/tests/test_common.py` & `ploy-2.0.1/ploy/tests/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         instance.max_startup_script_size = 10
         with mock.patch('ploy.common.log') as LogMock:
             instance.startup_script(debug=True)
             LogMock.error.assert_called_with('Startup script too big (%s > %s).', 15, 10)
 
 
 class TestBaseMaster:
-    @pytest.yield_fixture
+    @pytest.fixture
     def ctrl(self, ployconf):
         from ploy import Controller
         import ploy.tests.dummy_plugin
         ployconf.fill([
             '[dummy-master:warden]',
             '[dummy-master:master]',
             '[dummy-master:another]',
```

### Comparing `ploy-2.0.0b5/ploy/tests/dummy_plugin.py` & `ploy-2.0.1/ploy/tests/dummy_plugin.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy/tests/test_plain.py` & `ploy-2.0.1/ploy/tests/test_plain.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         ctrl(['./bin/ploy', 'ssh', 'foo'])
         known_hosts = os.path.join(ployconf.directory, 'known_hosts')
         os_execvp_mock.assert_called_with(
             'ssh',
             ['ssh', '-o', 'Forwardagent=yes', '-o', 'StrictHostKeyChecking=yes', '-o', 'UserKnownHostsFile=%s' % known_hosts, '-l', 'root', '-p', '22', 'localhost'])
 
 
-@pytest.yield_fixture
+@pytest.fixture
 def sshclient(mock):
     with mock.patch("ploy.plain.wait_for_ssh"):
         with mock.patch("ploy.plain.wait_for_ssh_on_sock"):
             with mock.patch("paramiko.SSHClient") as ssh_client_mock:
                 yield ssh_client_mock
```

### Comparing `ploy-2.0.0b5/ploy/tests/dummy_proxy_plugin.py` & `ploy-2.0.1/ploy/tests/dummy_proxy_plugin.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy/tests/test_ploy.py` & `ploy-2.0.1/ploy/tests/test_ploy.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy/tests/test_config.py` & `ploy-2.0.1/ploy/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy/tests/test_proxy.py` & `ploy-2.0.1/ploy/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy/tests/test_template.py` & `ploy-2.0.1/ploy/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy/__init__.py` & `ploy-2.0.1/ploy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from __future__ import print_function, unicode_literals
-import pkg_resources
-from collections import MutableMapping
+try:
+    from collections.abc import MutableMapping
+except ImportError:
+    from collections import MutableMapping
+try:
+    from importlib.metadata import PackageNotFoundError
+    from importlib.metadata import distribution
+    from importlib.metadata import entry_points
+except ImportError:
+    from importlib_metadata import PackageNotFoundError
+    from importlib_metadata import distribution
+    from importlib_metadata import entry_points
 from lazy import lazy
 from ploy import hookspecs, template
 from ploy.common import sorted_choices
 from pluggy import PluginManager
 from traceback import format_exc
 import logging
 import argparse
@@ -18,31 +28,37 @@
 # shutup pyflakes
 __all__ = [template.__name__]
 
 
 log = logging.getLogger('ploy')
 
 
+def package_version_info(name):
+    dist = distribution(name)
+    return " ".join((
+        name, dist.version,
+        "(%s)" % dist.locate_file('.').as_posix()))
+
+
 def versionaction_factory(ctrl):
     class VersionAction(argparse.Action):
         def __init__(self, *args, **kw):
             kw['nargs'] = 0
             argparse.Action.__init__(self, *args, **kw)
 
         def __call__(self, parser, namespace, values, option_string=None):
             import inspect
-            versions = [repr(pkg_resources.get_distribution("ploy"))]
+            versions = [package_version_info("ploy")]
             for plugin in ctrl.plugins.values():
                 for item in plugin.values():
                     module = inspect.getmodule(item)
                     try:
-                        pkg = pkg_resources.get_distribution(module.__name__)
-                    except pkg_resources.DistributionNotFound:
+                        versions.append(package_version_info(module.__name__))
+                    except PackageNotFoundError:
                         continue
-                    versions.append(repr(pkg))
                     break
             print('\n'.join(sorted(versions)))
             sys.exit(0)
     return VersionAction
 
 
 class LazyInstanceDict(MutableMapping):
@@ -124,20 +140,20 @@
         self.pm.check_pending()
         return self.pm.hook
 
     @lazy
     def plugins(self):
         plugins = {}
         group = 'ploy.plugins'
-        for entrypoint in pkg_resources.iter_entry_points(group=group):
+        for entrypoint in entry_points()[group]:
             try:
                 plugin = entrypoint.load()
-            except pkg_resources.DistributionNotFound:
+            except PackageNotFoundError:
                 continue
-            except pkg_resources.VersionConflict as e:
+            except Exception as e:
                 log.error(
                     "Plugin %r could not be loaded: %s" % (entrypoint.name, e))
                 continue
             plugins[entrypoint.name] = plugin
         return plugins
 
     @lazy
```

### Comparing `ploy-2.0.0b5/ploy/common.py` & `ploy-2.0.1/ploy/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import binascii
 import gzip
 import hashlib
 import logging
 import os
 import paramiko
 import re
+import select
 import socket
 import subprocess
 import sys
-import time
 
 
 log = logging.getLogger('ploy')
 
 
 try:
     get_input = raw_input
@@ -293,56 +293,30 @@
         instance_ssh_args = instance.ssh_args_from_info(instance_ssh_info)
         ssh_args = ['nohup', 'ssh']
         ssh_args.extend(instance_ssh_args)
         ssh_args.extend(['-W', '%s:%s' % (self.get_host(), self.get_port())])
         return shjoin(ssh_args)
 
 
-class Executor:
+class BaseExecutor:
     def __init__(self, instance=None, prefix_args=(), splitlines=False):
         self.instance = instance
         self.prefix_args = tuple(prefix_args)
         self.splitlines = splitlines
 
+    def _run(self):
+        raise NotImplementedError
+
     def __call__(self, *cmd_args, **kw):
         args = self.prefix_args + cmd_args
         rc = kw.pop('rc', None)
         out = kw.pop('out', None)
         err = kw.pop('err', None)
         stdin = kw.pop('stdin', None)
-        if self.instance is None:
-            log.debug('Executing locally:\n%s', args)
-            popen_kw = dict(stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-            if stdin is not None:
-                popen_kw['stdin'] = subprocess.PIPE
-            proc = subprocess.Popen(args, **popen_kw)
-            _out, _err = proc.communicate(input=stdin)
-            _rc = proc.returncode
-        else:
-            cmd = shjoin(args)
-            log.debug('Executing on instance %s:\n%s', self.instance.uid, cmd)
-            chan = self.instance.conn.get_transport().open_session()
-            if stdin is not None:
-                rin = chan.makefile('wb', -1)
-            rout = chan.makefile('rb', -1)
-            rerr = chan.makefile_stderr('rb', -1)
-            forward = None
-            if self.instance.conn._ploy_forward_agent:
-                forward = paramiko.agent.AgentRequestHandler(chan)
-            chan.exec_command(cmd)
-            if stdin is not None:
-                rin.write(stdin)
-                rin.flush()
-                chan.shutdown_write()
-            _out = rout.read()
-            _err = rerr.read()
-            _rc = chan.recv_exit_status()
-            chan.close()
-            if forward is not None:
-                forward.close()
+        (_rc, _out, _err) = self._run(args, stdin)
         result = []
         if rc is None:
             result.append(_rc)
         else:
             try:
                 if not any(x == _rc for x in rc):
                     raise subprocess.CalledProcessError(_rc, ' '.join(args), _err)
@@ -375,14 +349,91 @@
         if len(result) == 0:
             return
         elif len(result) == 1:
             return result[0]
         return tuple(result)
 
 
+class LocalExecutor(BaseExecutor):
+    def __init__(self, **kw):
+        BaseExecutor.__init__(self, **kw)
+
+    def _run(self, args, stdin):
+        log.debug('Executing locally:\n%s', args)
+        popen_kw = dict(stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        if stdin is not None:
+            popen_kw['stdin'] = subprocess.PIPE
+        proc = subprocess.Popen(args, **popen_kw)
+        (out, err) = proc.communicate(input=stdin)
+        rc = proc.returncode
+        return (rc, out, err)
+
+
+class InstanceExecutor(BaseExecutor):
+    def __init__(self, instance, **kw):
+        BaseExecutor.__init__(self, **kw)
+        self.instance = instance
+
+    def _run(self, args, stdin):
+        cmd = shjoin(args)
+        log.debug('Executing on instance %s:\n%s', self.instance.uid, cmd)
+        chan = self.instance.conn.get_transport().open_session()
+        if stdin is not None:
+            rin = chan.makefile('wb', -1)
+        rout = chan.makefile('rb', -1)
+        rerr = chan.makefile_stderr('rb', -1)
+        forward = None
+        if self.instance.conn._ploy_forward_agent:
+            forward = paramiko.agent.AgentRequestHandler(chan)
+        chan.exec_command(cmd)
+        if stdin is not None:
+            rin.write(stdin)
+            rin.flush()
+            rin.close()
+            del rin
+            chan.shutdown_write()
+        out_chunks = []
+        err_chunks = []
+        assert chan == rout.channel
+        assert chan == rerr.channel
+        while 1:
+            # stop if channel was closed prematurely,
+            # and there is no data in the buffers
+            should_break = True
+            (readq, _, _) = select.select([chan], [], [])
+            assert len(readq) == 1 and readq[0] == chan
+            if chan.recv_ready():
+                out_chunks.append(chan.recv(len(chan.in_buffer)))
+                should_break = False
+            if chan.recv_stderr_ready():
+                err_chunks.append(chan.recv_stderr(len(chan.in_stderr_buffer)))
+                should_break = False
+            should_break = (
+                should_break
+                and chan.exit_status_ready()
+                and not chan.recv_ready()
+                and not chan.recv_stderr_ready())
+            if should_break:
+                break
+        rc = chan.recv_exit_status()
+        chan.shutdown_read()
+        chan.close()
+        rout.close()
+        rerr.close()
+        if forward is not None:
+            forward.close()
+        return (rc, b''.join(out_chunks), b''.join(err_chunks))
+
+
+def Executor(instance=None, **kw):
+    if instance is None:
+        return LocalExecutor(**kw)
+    return InstanceExecutor(**kw)
+
+
 class Hooks(object):
     def __init__(self):
         self.hooks = []
 
     def add(self, hook):
         self.hooks.append(hook)
 
@@ -590,38 +641,22 @@
             if match:
                 info['keytype'] = match.group(1)
         fingerprints.append(SSHKeyFingerprint(**info))
     return fingerprints
 
 
 def wait_for_ssh(host, port, timeout=5):
-    while timeout > 0:
-        with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
-            try:
-                s.settimeout(1)
-                if s.connect_ex((host, port)) == 0:
-                    if s.recv(128).startswith(b'SSH-2'):
-                        return
-            except socket.timeout:
-                timeout -= 1
-                if timeout <= 0:
-                    raise
-        time.sleep(1)
-        timeout -= 1
+    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
+        s.settimeout(timeout)
+        if s.connect_ex((host, port)) == 0:
+            if s.recv(128).startswith(b'SSH-2'):
+                return
 
 
 def wait_for_ssh_on_sock(socket_factory, timeout=5):
-    while timeout > 0:
-        sock = socket_factory()
-        if sock is None:
+    sock = socket_factory()
+    if sock is None:
+        return
+    with closing(sock) as s:
+        s.settimeout(timeout)
+        if s.recv(128).startswith(b'SSH-2'):
             return
-        with closing(sock) as s:
-            try:
-                s.settimeout(1)
-                if s.recv(128).startswith(b'SSH-2'):
-                    return
-            except socket.timeout:
-                timeout -= 1
-                if timeout <= 0:
-                    raise
-        time.sleep(1)
-        timeout -= 1
```

### Comparing `ploy-2.0.0b5/ploy/plain.py` & `ploy-2.0.1/ploy/plain.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy/template.py` & `ploy-2.0.1/ploy/template.py`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/HISTORY.rst` & `ploy-2.0.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 Changelog
 =========
 
+2.0.1 - 2023-06-19
+------------------
+
+* Fix ssh timeout handling.
+  [witsch, fschulze]
+
+* Fix getargspec deprecation warning with Python 3.x.
+  [kappeck, fschulze]
+
+
+2.0.0 - 2022-08-17
+------------------
+
+* Dropped support for Python 3.6.
+  [fschulze]
+
+* Added support for Python 3.10.
+  [fschulze]
+
+
 2.0.0b5 - 2021-07-17
 --------------------
 
 * Make a proper copy of the configuration for instances with multiple masters.
   [fschulze]
 
 * Use ``format_exc`` for error reporting in ``ssh`` command for more details.
@@ -44,14 +64,24 @@
 * Dropped support ``ssh`` lib, only ``paramiko`` is supported.
   [fschulze]
 
 * Dropped support for Python 2.6 and 3.3.
   [fschulze]
 
 
+1.5.2 - 2018-08-20
+------------------
+
+* Stop testing on Python 3.3.
+  [fschulze]
+
+* Fix multiple masters for ``instance``.
+  [fschulze]
+
+
 1.5.1 - 2017-12-17
 ------------------
 
 * Fix getting fingerprints automatically when ``ssh-host-keys`` is used.
   [fschulze]
```

### Comparing `ploy-2.0.0b5/README.rst` & `ploy-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ploy-2.0.0b5/ploy.egg-info/SOURCES.txt` & `ploy-2.0.1/ploy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+.travis.yml
 HISTORY.rst
+LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/main.yml
 ploy/__init__.py
 ploy/common.py
 ploy/config.py
 ploy/hookspecs.py
 ploy/plain.py
 ploy/proxy.py
 ploy/template.py
 ploy.egg-info/PKG-INFO
 ploy.egg-info/SOURCES.txt
 ploy.egg-info/dependency_links.txt
 ploy.egg-info/entry_points.txt
 ploy.egg-info/not-zip-safe
+ploy.egg-info/pbr.json
 ploy.egg-info/requires.txt
 ploy.egg-info/top_level.txt
 ploy/tests/__init__.py
 ploy/tests/dummy_plugin.py
 ploy/tests/dummy_proxy_plugin.py
 ploy/tests/test_common.py
 ploy/tests/test_config.py
```

