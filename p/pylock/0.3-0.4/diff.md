# Comparing `tmp/pylock-0.3.tar.gz` & `tmp/pylock-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylock-0.3.tar", last modified: Wed May 25 14:40:08 2016, max compression
+gzip compressed data, was "pylock-0.4.tar", last modified: Mon Jun 19 17:10:24 2023, max compression
```

## Comparing `pylock-0.3.tar` & `pylock-0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 josephkahn   (503) staff       (20)        0 2016-05-25 14:40:08.000000 pylock-0.3/
--rw-r--r--   0 josephkahn   (503) staff       (20)     1529 2016-05-20 23:52:11.000000 pylock-0.3/LICENSE
--rw-r--r--   0 josephkahn   (503) staff       (20)       27 2016-05-20 23:52:11.000000 pylock-0.3/MANIFEST.in
--rw-r--r--   0 josephkahn   (503) staff       (20)     3727 2016-05-25 14:40:08.000000 pylock-0.3/PKG-INFO
-drwxr-xr-x   0 josephkahn   (503) staff       (20)        0 2016-05-25 14:40:08.000000 pylock-0.3/pylock/
--rw-r--r--   0 josephkahn   (503) staff       (20)     3294 2016-05-25 14:35:35.000000 pylock-0.3/pylock/__init__.py
-drwxr-xr-x   0 josephkahn   (503) staff       (20)        0 2016-05-25 14:40:08.000000 pylock-0.3/pylock/backends/
--rw-r--r--   0 josephkahn   (503) staff       (20)      607 2016-05-20 23:52:11.000000 pylock-0.3/pylock/backends/__init__.py
-drwxr-xr-x   0 josephkahn   (503) staff       (20)        0 2016-05-25 14:40:08.000000 pylock-0.3/pylock/backends/open_lock/
--rw-r--r--   0 josephkahn   (503) staff       (20)      246 2016-05-20 23:52:11.000000 pylock-0.3/pylock/backends/open_lock/__init__.py
-drwxr-xr-x   0 josephkahn   (503) staff       (20)        0 2016-05-25 14:40:08.000000 pylock-0.3/pylock/backends/redis_lock/
--rw-r--r--   0 josephkahn   (503) staff       (20)     1860 2016-05-20 23:52:11.000000 pylock-0.3/pylock/backends/redis_lock/__init__.py
-drwxr-xr-x   0 josephkahn   (503) staff       (20)        0 2016-05-25 14:40:08.000000 pylock-0.3/pylock/tests/
--rw-r--r--   0 josephkahn   (503) staff       (20)        0 2016-05-20 23:52:11.000000 pylock-0.3/pylock/tests/__init__.py
--rw-r--r--   0 josephkahn   (503) staff       (20)     5746 2016-05-20 23:52:11.000000 pylock-0.3/pylock/tests/test_backends.py
--rw-r--r--   0 josephkahn   (503) staff       (20)     2802 2016-05-20 23:52:11.000000 pylock-0.3/pylock/tests/test_lock.py
-drwxr-xr-x   0 josephkahn   (503) staff       (20)        0 2016-05-25 14:40:08.000000 pylock-0.3/pylock.egg-info/
--rw-r--r--   0 josephkahn   (503) staff       (20)        1 2016-05-25 14:40:08.000000 pylock-0.3/pylock.egg-info/dependency_links.txt
--rw-r--r--   0 josephkahn   (503) staff       (20)        1 2016-05-21 00:00:58.000000 pylock-0.3/pylock.egg-info/not-zip-safe
--rw-r--r--   0 josephkahn   (503) staff       (20)     3727 2016-05-25 14:40:08.000000 pylock-0.3/pylock.egg-info/PKG-INFO
--rw-r--r--   0 josephkahn   (503) staff       (20)       13 2016-05-25 14:40:08.000000 pylock-0.3/pylock.egg-info/requires.txt
--rw-r--r--   0 josephkahn   (503) staff       (20)      422 2016-05-25 14:40:08.000000 pylock-0.3/pylock.egg-info/SOURCES.txt
--rw-r--r--   0 josephkahn   (503) staff       (20)        7 2016-05-25 14:40:08.000000 pylock-0.3/pylock.egg-info/top_level.txt
--rw-r--r--   0 josephkahn   (503) staff       (20)     2525 2016-05-20 23:52:11.000000 pylock-0.3/README.rst
--rw-r--r--   0 josephkahn   (503) staff       (20)       59 2016-05-25 14:40:08.000000 pylock-0.3/setup.cfg
--rw-r--r--   0 josephkahn   (503) staff       (20)      890 2016-05-25 14:35:35.000000 pylock-0.3/setup.py
+drwxr-xr-x   0 wnichols   (502) staff       (20)        0 2023-06-19 17:10:24.810048 pylock-0.4/
+-rw-r--r--   0 wnichols   (502) staff       (20)     1529 2023-05-31 20:20:17.000000 pylock-0.4/LICENSE
+-rw-r--r--   0 wnichols   (502) staff       (20)       27 2023-05-31 20:20:17.000000 pylock-0.4/MANIFEST.in
+-rw-r--r--   0 wnichols   (502) staff       (20)     4329 2023-06-19 17:10:24.809798 pylock-0.4/PKG-INFO
+-rw-r--r--   0 wnichols   (502) staff       (20)     3031 2023-06-01 18:58:48.000000 pylock-0.4/README.rst
+drwxr-xr-x   0 wnichols   (502) staff       (20)        0 2023-06-19 17:10:24.806115 pylock-0.4/pylock/
+-rw-r--r--   0 wnichols   (502) staff       (20)     3463 2023-06-01 18:59:16.000000 pylock-0.4/pylock/__init__.py
+drwxr-xr-x   0 wnichols   (502) staff       (20)        0 2023-06-19 17:10:24.807535 pylock-0.4/pylock/backends/
+-rw-r--r--   0 wnichols   (502) staff       (20)      607 2023-05-31 20:20:17.000000 pylock-0.4/pylock/backends/__init__.py
+drwxr-xr-x   0 wnichols   (502) staff       (20)        0 2023-06-19 17:10:24.808040 pylock-0.4/pylock/backends/open_lock/
+-rw-r--r--   0 wnichols   (502) staff       (20)      249 2023-06-01 14:46:22.000000 pylock-0.4/pylock/backends/open_lock/__init__.py
+drwxr-xr-x   0 wnichols   (502) staff       (20)        0 2023-06-19 17:10:24.808389 pylock-0.4/pylock/backends/redis_lock/
+-rw-r--r--   0 wnichols   (502) staff       (20)     1931 2023-05-31 21:00:07.000000 pylock-0.4/pylock/backends/redis_lock/__init__.py
+drwxr-xr-x   0 wnichols   (502) staff       (20)        0 2023-06-19 17:10:24.809311 pylock-0.4/pylock/tests/
+-rw-r--r--   0 wnichols   (502) staff       (20)        0 2023-05-31 20:20:17.000000 pylock-0.4/pylock/tests/__init__.py
+-rw-r--r--   0 wnichols   (502) staff       (20)     7899 2023-06-01 18:59:35.000000 pylock-0.4/pylock/tests/test_backends.py
+-rw-r--r--   0 wnichols   (502) staff       (20)     2802 2023-06-01 15:32:35.000000 pylock-0.4/pylock/tests/test_lock.py
+drwxr-xr-x   0 wnichols   (502) staff       (20)        0 2023-06-19 17:10:24.807390 pylock-0.4/pylock.egg-info/
+-rw-r--r--   0 wnichols   (502) staff       (20)     4329 2023-06-19 17:10:24.000000 pylock-0.4/pylock.egg-info/PKG-INFO
+-rw-r--r--   0 wnichols   (502) staff       (20)      437 2023-06-19 17:10:24.000000 pylock-0.4/pylock.egg-info/SOURCES.txt
+-rw-r--r--   0 wnichols   (502) staff       (20)        1 2023-06-19 17:10:24.000000 pylock-0.4/pylock.egg-info/dependency_links.txt
+-rw-r--r--   0 wnichols   (502) staff       (20)        1 2023-06-01 14:38:58.000000 pylock-0.4/pylock.egg-info/not-zip-safe
+-rw-r--r--   0 wnichols   (502) staff       (20)       12 2023-06-19 17:10:24.000000 pylock-0.4/pylock.egg-info/requires.txt
+-rw-r--r--   0 wnichols   (502) staff       (20)        7 2023-06-19 17:10:24.000000 pylock-0.4/pylock.egg-info/top_level.txt
+-rw-r--r--   0 wnichols   (502) staff       (20)      427 2023-06-01 18:58:13.000000 pylock-0.4/pyproject.toml
+-rw-r--r--   0 wnichols   (502) staff       (20)       38 2023-06-19 17:10:24.810110 pylock-0.4/setup.cfg
+-rw-r--r--   0 wnichols   (502) staff       (20)      889 2023-06-01 14:39:27.000000 pylock-0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylock-0.3/LICENSE` & `pylock-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylock-0.3/PKG-INFO` & `pylock-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pylock
-Version: 0.3
+Version: 0.4
 Summary: Python Distributed Lock
 Home-page: http://github.com/waveaccounting/pylock
 Author: Nathan Duthoit
 Author-email: nathan@waveapps.com
 License: BSD
 Description: Usage
         -----
@@ -96,15 +96,27 @@
         
         The memcache backend is inspired by the following: -
         https://github.com/snbuback/DistributedLock -
         http://jbq.caraldi.com/2010/08/simple-distributed-lock-with-memcached.html
         -
         http://www.regexprn.com/2010/05/using-memcached-as-distributed-locking.html
         
-        TODO: - better handle redis/memcache connection issues
+        
+        
+        Notes related to the 0.4 release
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Added a poetry lock file, but did not setup circleci builds
+        To build and publish a release:
+        poetry publish -r gemfury -u $GEMFURY_PUSH_TOKEN -p NOPASS --build 
+        
+        For testing I would suggest that you build and publish patch releases till it works in your app THEN publish a minor or major version
+        because if you republish multiple builds at the same version it is very difficult to get your app to install the new ones.
+        
+        Poetry builds do not include test code the way that setup.py builds did.
         
 Keywords: lock redis
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pylock-0.3/pylock/__init__.py` & `pylock-0.4/pylock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             backend_class_path = DEFAULT_BACKEND['class']
         if backend_connection is None:
             backend_connection = DEFAULT_BACKEND['connection']
         # Load backend class
         backend_class = get_backend_class(backend_class_path)
         logger.info("Using {0} lock backend".format(backend_class.__name__))
         key = "{0}{1}".format(KEY_PREFIX, key)
-        connection_info = parse_url(backend_connection, url_scheme=backend_class.url_scheme)
+        connection_info = parse_url(backend_connection, url_schemes=backend_class.url_schemes)
         client = backend_class.get_client(**connection_info)
         self._lock = backend_class(key, expires, timeout, client)
 
     def __enter__(self):
         self._lock.acquire()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -77,28 +77,33 @@
         raise ImproperlyConfigured('Error importing pylock backend module %s: "%s"' % (module, e))
     try:
         return getattr(mod, classname)
     except AttributeError:
         raise ImproperlyConfigured('Pylock backend module "%s" does not define a "%s" class.' % (module, classname))
 
 
-def parse_url(url, url_scheme):
+def parse_url(url, url_schemes):
     """Parses a distributed lock backend URL."""
     # Register extra schemes in URLs.
-    parse.uses_netloc.append(url_scheme)
+    for scheme in url_schemes:
+        parse.uses_netloc.append(scheme)
 
     url = parse.urlparse(url)
 
     # Remove query strings.
     path = url.path[1:]
     path = path.split('?', 2)[0]
+    path = path.split('/', 2)[0]
+    ssl = True if url.scheme == "rediss" else False
 
     # Update with environment configuration.
     connection_info = {
         'db': path,
         'user': url.username,
         'password': url.password,
         'host': url.hostname,
-        'port': url.port
+        'port': url.port,
+        'scheme': url.scheme,
+        'ssl': ssl
     }
 
     return connection_info
```

### Comparing `pylock-0.3/pylock/backends/__init__.py` & `pylock-0.4/pylock/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pylock-0.3/pylock/backends/redis_lock/__init__.py` & `pylock-0.4/pylock/backends/redis_lock/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 from redis import StrictRedis
 
 from .. import BaseLock, LockTimeout
 
 
 class RedisLock(BaseLock):
-    url_scheme = 'redis'
+    url_schemes = ['redis','rediss']
 
     @classmethod
     def get_client(cls, **connection_args):
         host = connection_args.get('host') or 'localhost'
         port = connection_args.get('port') or 6379
         password = connection_args.get('password')
         db = connection_args.get('db') or 0
-        return StrictRedis(host, port, db, password)
+        ssl = connection_args.get('ssl') or False
+        return StrictRedis(host, port, db, password, ssl=ssl)
 
     def __init__(self, key, expires, timeout, client):
         super(RedisLock, self).__init__(key, expires, timeout, client)
         self.start_time = time.time()
 
     def acquire(self):
         redis = self.client
```

### Comparing `pylock-0.3/pylock/tests/test_lock.py` & `pylock-0.4/pylock/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `pylock-0.3/pylock.egg-info/PKG-INFO` & `pylock-0.4/pylock.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pylock
-Version: 0.3
+Version: 0.4
 Summary: Python Distributed Lock
 Home-page: http://github.com/waveaccounting/pylock
 Author: Nathan Duthoit
 Author-email: nathan@waveapps.com
 License: BSD
 Description: Usage
         -----
@@ -96,15 +96,27 @@
         
         The memcache backend is inspired by the following: -
         https://github.com/snbuback/DistributedLock -
         http://jbq.caraldi.com/2010/08/simple-distributed-lock-with-memcached.html
         -
         http://www.regexprn.com/2010/05/using-memcached-as-distributed-locking.html
         
-        TODO: - better handle redis/memcache connection issues
+        
+        
+        Notes related to the 0.4 release
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Added a poetry lock file, but did not setup circleci builds
+        To build and publish a release:
+        poetry publish -r gemfury -u $GEMFURY_PUSH_TOKEN -p NOPASS --build 
+        
+        For testing I would suggest that you build and publish patch releases till it works in your app THEN publish a minor or major version
+        because if you republish multiple builds at the same version it is very difficult to get your app to install the new ones.
+        
+        Poetry builds do not include test code the way that setup.py builds did.
         
 Keywords: lock redis
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pylock-0.3/setup.py` & `pylock-0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import os
 
 from setuptools import setup, find_packages
 
-__version__ = '0.3'
+__version__ = '0.4'
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.rst')).read()
 
 setup(
     name='pylock',
     version=__version__,
     description='Python Distributed Lock',
     long_description=README,
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.7",
     ],
     keywords='lock redis',
     author="Nathan Duthoit",
     author_email="nathan@waveapps.com",
     url="http://github.com/waveaccounting/pylock",
     license="BSD",
     packages=find_packages(),
     test_suite="pylock.tests",
     include_package_data=True,
     zip_safe=False,
     tests_require=['Mock>=2.0.0', 'nose'],
     install_requires=[
-        "redis>=2.6.1",
+        "redis>4.0.0",
     ]
 )
```

