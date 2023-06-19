# Comparing `tmp/requests-futures-1.0.0.tar.gz` & `tmp/requests-futures-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/requests-futures-1.0.0.tar", last modified: Tue Jun 11 03:22:21 2019, max compression
+gzip compressed data, was "requests-futures-1.0.1.tar", last modified: Mon Jun 19 19:59:04 2023, max compression
```

## Comparing `requests-futures-1.0.0.tar` & `requests-futures-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-06-11 03:22:21.000000 requests-futures-1.0.0/
--rw-r--r--   0 ross       (501) staff       (20)    12134 2019-06-11 03:22:21.000000 requests-futures-1.0.0/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      582 2017-11-03 13:09:48.000000 requests-futures-1.0.0/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)      106 2017-11-03 13:09:48.000000 requests-futures-1.0.0/MANIFEST.in
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-06-11 03:22:21.000000 requests-futures-1.0.0/requests_futures/
--rw-r--r--   0 ross       (501) staff       (20)     7016 2019-06-11 03:17:00.000000 requests-futures-1.0.0/requests_futures/sessions.py
--rw-r--r--   0 ross       (501) staff       (20)      590 2019-06-11 03:18:01.000000 requests-futures-1.0.0/requests_futures/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    10604 2019-06-11 03:17:00.000000 requests-futures-1.0.0/test_requests_futures.py
--rw-r--r--   0 ross       (501) staff       (20)     1448 2019-06-11 03:17:01.000000 requests-futures-1.0.0/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-06-11 03:22:21.000000 requests-futures-1.0.0/requests_futures.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)    12134 2019-06-11 03:22:21.000000 requests-futures-1.0.0/requests_futures.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)        1 2017-11-06 14:54:45.000000 requests-futures-1.0.0/requests_futures.egg-info/not-zip-safe
--rw-r--r--   0 ross       (501) staff       (20)      414 2019-06-11 03:22:21.000000 requests-futures-1.0.0/requests_futures.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)       58 2019-06-11 03:22:21.000000 requests-futures-1.0.0/requests_futures.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       17 2019-06-11 03:22:21.000000 requests-futures-1.0.0/requests_futures.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2019-06-11 03:22:21.000000 requests-futures-1.0.0/requests_futures.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       16 2017-11-03 13:09:48.000000 requests-futures-1.0.0/requirements-python-3.txt
--rw-r--r--   0 ross       (501) staff       (20)       38 2019-06-11 03:22:21.000000 requests-futures-1.0.0/setup.cfg
--rw-r--r--   0 ross       (501) staff       (20)     9362 2019-06-11 03:22:02.000000 requests-futures-1.0.0/README.rst
--rw-r--r--   0 ross       (501) staff       (20)       24 2017-11-03 13:09:48.000000 requests-futures-1.0.0/requirements-python-2.7.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-06-19 19:59:04.770749 requests-futures-1.0.1/
+-rw-r--r--   0 ross       (501) staff       (20)      582 2021-05-27 19:20:50.000000 requests-futures-1.0.1/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)       69 2022-08-31 12:14:51.000000 requests-futures-1.0.1/MANIFEST.in
+-rw-r--r--   0 ross       (501) staff       (20)    12181 2023-06-19 19:59:04.770016 requests-futures-1.0.1/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)    11365 2022-08-31 12:14:51.000000 requests-futures-1.0.1/README.rst
+-rw-r--r--   0 ross       (501) staff       (20)      295 2023-06-19 19:51:23.000000 requests-futures-1.0.1/pyproject.toml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-06-19 19:59:04.764241 requests-futures-1.0.1/requests_futures/
+-rw-r--r--   0 ross       (501) staff       (20)      592 2023-06-19 19:57:28.000000 requests-futures-1.0.1/requests_futures/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     7165 2023-06-19 19:51:23.000000 requests-futures-1.0.1/requests_futures/sessions.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-06-19 19:59:04.768211 requests-futures-1.0.1/requests_futures.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)    12181 2023-06-19 19:59:04.000000 requests-futures-1.0.1/requests_futures.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      398 2023-06-19 19:59:04.000000 requests-futures-1.0.1/requests_futures.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-06-19 19:59:04.000000 requests-futures-1.0.1/requests_futures.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2021-09-29 00:14:51.000000 requests-futures-1.0.1/requests_futures.egg-info/not-zip-safe
+-rw-r--r--   0 ross       (501) staff       (20)      174 2023-06-19 19:59:04.000000 requests-futures-1.0.1/requests_futures.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       17 2023-06-19 19:59:04.000000 requests-futures-1.0.1/requests_futures.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)       86 2023-06-19 19:51:23.000000 requests-futures-1.0.1/requirements.txt
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-06-19 19:59:04.770871 requests-futures-1.0.1/setup.cfg
+-rw-r--r--   0 ross       (501) staff       (20)     1920 2023-06-19 19:51:23.000000 requests-futures-1.0.1/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-06-19 19:59:04.769232 requests-futures-1.0.1/tests/
+-rw-r--r--   0 ross       (501) staff       (20)    10769 2023-06-19 19:51:23.000000 requests-futures-1.0.1/tests/test_requests_futures.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `requests-futures-1.0.0/PKG-INFO` & `requests-futures-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,276 +1,346 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: requests-futures
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous Python HTTP for Humans.
 Home-page: https://github.com/ross/requests-futures
 Author: Ross McFarland
-Author-email: rwmcfa1@neces.com
+Author-email: rwmcfa1@rwmcfa1.com
 License: Apache License v2
-Description: Asynchronous Python HTTP Requests for Humans
-        ============================================
-        
-        .. image:: https://travis-ci.org/ross/requests-futures.png?branch=master
-                :target: https://travis-ci.org/ross/requests-futures
-        
-        Small add-on for the python requests_ http library. Makes use of python 3.2's
-        `concurrent.futures`_ or the backport_ for prior versions of python.
-        
-        The additional API and changes are minimal and strives to avoid surprises.
-        
-        The following synchronous code:
-        
-        .. code-block:: python
-        
-            from requests import Session
-        
-            session = Session()
-            # first requests starts and blocks until finished
-            response_one = session.get('http://httpbin.org/get')
-            # second request starts once first is finished
-            response_two = session.get('http://httpbin.org/get?foo=bar')
-            # both requests are complete
-            print('response one status: {0}'.format(response_one.status_code))
-            print(response_one.content)
-            print('response two status: {0}'.format(response_two.status_code))
-            print(response_two.content)
-        
-        Can be translated to make use of futures, and thus be asynchronous by creating
-        a FuturesSession and catching the returned Future in place of Response. The
-        Response can be retrieved by calling the result method on the Future:
-        
-        .. code-block:: python
-        
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession()
-            # first request is started in background
-            future_one = session.get('http://httpbin.org/get')
-            # second requests is started immediately
-            future_two = session.get('http://httpbin.org/get?foo=bar')
-            # wait for the first request to complete, if it hasn't already
-            response_one = future_one.result()
-            print('response one status: {0}'.format(response_one.status_code))
-            print(response_one.content)
-            # wait for the second request to complete, if it hasn't already
-            response_two = future_two.result()
-            print('response two status: {0}'.format(response_two.status_code))
-            print(response_two.content)
-        
-        By default a ThreadPoolExecutor is created with 8 workers. If you would like to
-        adjust that value or share a executor across multiple sessions you can provide
-        one to the FuturesSession constructor.
-        
-        .. code-block:: python
-        
-            from concurrent.futures import ThreadPoolExecutor
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession(executor=ThreadPoolExecutor(max_workers=10))
-            # ...
-        
-        As a shortcut in case of just increasing workers number you can pass
-        `max_workers` straight to the `FuturesSession` constructor:
-        
-        .. code-block:: python
-        
-            from requests_futures.sessions import FuturesSession
-            session = FuturesSession(max_workers=10)
-        
-        FutureSession will use an existing session object if supplied:
-        
-        .. code-block:: python
-        
-            from requests import session
-            from requests_futures.sessions import FuturesSession
-            my_session = session()
-            future_session = FuturesSession(session=my_session)
-        
-        That's it. The api of requests.Session is preserved without any modifications
-        beyond returning a Future rather than Response. As with all futures exceptions
-        are shifted (thrown) to the future.result() call so try/except blocks should be
-        moved there.
-        
-        Canceling queued requests (a.k.a cleaning up after yourself)
-        ============================================================
-        
-        If you know that you won't be needing any additional responses from futures that
-        haven't yet resolved, it's a good idea to cancel those requests. You can do this
-        by using the session as a context manager:
-        
-        .. code-block:: python
-        
-            from requests_futures.sessions import FuturesSession
-            with FuturesSession(max_workers=1) as session:
-                future = session.get('https://httpbin.org/get')
-                future2 = session.get('https://httpbin.org/delay/10')
-                future3 = session.get('https://httpbin.org/delay/10')
-                response = future.result()
-        
-        In this example, the second or third request will be skipped, saving time and
-        resources that would otherwise be wasted.
-        
-        Working in the Background
-        =========================
-        
-        Additional processing can be done in the background using requests's hooks_
-        functionality. This can be useful for shifting work out of the foreground, for
-        a simple example take json parsing.
-        
-        .. code-block:: python
-        
-            from pprint import pprint
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession()
-        
-            def response_hook(resp, *args, **kwargs):
-                # parse the json storing the result on the response object
-                resp.data = resp.json()
-        
-            future = session.get('http://httpbin.org/get', hooks={
-                'response': response_hook,
-            })
-            # do some other stuff, send some more requests while this one works
-            response = future.result()
-            print('response status {0}'.format(response.status_code))
-            # data will have been attached to the response object in the background
-            pprint(response.data)
-        
-        Hooks can also be applied to the session.
-        
-        .. code-block:: python
-        
-            from pprint import pprint
-            from requests_futures.sessions import FuturesSession
-        
-            def response_hook(resp, *args, **kwargs):
-                # parse the json storing the result on the response object
-                resp.data = resp.json()
-        
-            session = FuturesSession()
-            session.hooks['response'] = response_hook
-        
-            future = session.get('http://httpbin.org/get')
-            # do some other stuff, send some more requests while this one works
-            response = future.result()
-            print('response status {0}'.format(response.status_code))
-            # data will have been attached to the response object in the background
-            pprint(response.data)   pprint(response.data)
-        
-        A more advanced example that adds an `elapsed` property to all requests.
-        
-        .. code-block:: python
-        
-            from pprint import pprint
-            from requests_futures.sessions import FuturesSession
-            from time import time
-        
-        
-            class ElapsedFuturesSession(FuturesSession):
-        
-                def request(self, method, url, hooks={}, *args, **kwargs):
-                    start = time()
-        
-                    def timing(r, *args, **kwargs):
-                        r.elapsed = time() - start
-        
-                    try:
-                        if isinstance(hooks['response'], (list, tuple)):
-                            # needs to be first so we don't time other hooks execution
-                            hooks['response'].insert(0, timing)
-                        else:
-                            hooks['response'] = [timing, hooks['response']]
-                    except KeyError:
-                        hooks['response'] = timing
-        
-                    return super(ElapsedFuturesSession, self) \
-                        .request(method, url, hooks=hooks, *args, **kwargs)
-        
-        
-        
-            session = ElapsedFuturesSession()
-            future = session.get('http://httpbin.org/get')
-            # do some other stuff, send some more requests while this one works
-            response = future.result()
-            print('response status {0}'.format(response.status_code))
-            print('response elapsed {0}'.format(response.elapsed))
-        
-        Using ProcessPoolExecutor
-        =========================
-        
-        Similarly to `ThreadPoolExecutor`, it is possible to use an instance of
-        `ProcessPoolExecutor`. As the name suggest, the requests will be executed
-        concurrently in separate processes rather than threads.
-        
-        .. code-block:: python
-        
-            from concurrent.futures import ProcessPoolExecutor
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10))
-            # ... use as before
-        
-        .. HINT::
-            Using the `ProcessPoolExecutor` is useful, in cases where memory
-            usage per request is very high (large response) and cycling the interpretor
-            is required to release memory back to OS.
-        
-        A base requirement of using `ProcessPoolExecutor` is that the `Session.request`,
-        `FutureSession` all be pickle-able.
-        
-        This means that only Python 3.5 is fully supported, while Python versions
-        3.4 and above REQUIRE an existing `requests.Session` instance to be passed
-        when initializing `FutureSession`. Python 2.X and < 3.4 are currently not
-        supported.
-        
-        .. code-block:: python
-        
-            # Using python 3.4
-            from concurrent.futures import ProcessPoolExecutor
-            from requests import Session
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10),
-                                     session=Session())
-            # ... use as before
-        
-        In case pickling fails, an exception is raised pointing to this documentation.
-        
-        .. code-block:: python
-        
-            # Using python 2.7
-            from concurrent.futures import ProcessPoolExecutor
-            from requests import Session
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10),
-                                     session=Session())
-            Traceback (most recent call last):
-            ...
-            RuntimeError: Cannot pickle function. Refer to documentation: https://github.com/ross/requests-futures/#using-processpoolexecutor
-        
-        .. IMPORTANT::
-          * Python >= 3.4 required
-          * A session instance is required when using Python < 3.5
-          * If sub-classing `FuturesSession` it must be importable (module global)
-        
-        Installation
-        ============
-        
-            pip install requests-futures
-        
-        .. _`requests`: https://github.com/kennethreitz/requests
-        .. _`concurrent.futures`: http://docs.python.org/dev/library/concurrent.futures.html
-        .. _backport: https://pypi.python.org/pypi/futures
-        .. _hooks: http://docs.python-requests.org/en/master/user/advanced/#event-hooks
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
+Asynchronous Python HTTP Requests for Humans
+============================================
+
+.. image:: https://travis-ci.org/ross/requests-futures.svg?branch=master
+        :target: https://travis-ci.org/ross/requests-futures
+
+Small add-on for the python requests_ http library. Makes use of python 3.2's
+`concurrent.futures`_ or the backport_ for prior versions of python.
+
+The additional API and changes are minimal and strives to avoid surprises.
+
+The following synchronous code:
+
+.. code-block:: python
+
+    from requests import Session
+
+    session = Session()
+    # first requests starts and blocks until finished
+    response_one = session.get('http://httpbin.org/get')
+    # second request starts once first is finished
+    response_two = session.get('http://httpbin.org/get?foo=bar')
+    # both requests are complete
+    print('response one status: {0}'.format(response_one.status_code))
+    print(response_one.content)
+    print('response two status: {0}'.format(response_two.status_code))
+    print(response_two.content)
+
+Can be translated to make use of futures, and thus be asynchronous by creating
+a FuturesSession and catching the returned Future in place of Response. The
+Response can be retrieved by calling the result method on the Future:
+
+.. code-block:: python
+
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+    # first request is started in background
+    future_one = session.get('http://httpbin.org/get')
+    # second requests is started immediately
+    future_two = session.get('http://httpbin.org/get?foo=bar')
+    # wait for the first request to complete, if it hasn't already
+    response_one = future_one.result()
+    print('response one status: {0}'.format(response_one.status_code))
+    print(response_one.content)
+    # wait for the second request to complete, if it hasn't already
+    response_two = future_two.result()
+    print('response two status: {0}'.format(response_two.status_code))
+    print(response_two.content)
+
+By default a ThreadPoolExecutor is created with 8 workers. If you would like to
+adjust that value or share a executor across multiple sessions you can provide
+one to the FuturesSession constructor.
+
+.. code-block:: python
+
+    from concurrent.futures import ThreadPoolExecutor
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession(executor=ThreadPoolExecutor(max_workers=10))
+    # ...
+
+As a shortcut in case of just increasing workers number you can pass
+`max_workers` straight to the `FuturesSession` constructor:
+
+.. code-block:: python
+
+    from requests_futures.sessions import FuturesSession
+    session = FuturesSession(max_workers=10)
+
+FutureSession will use an existing session object if supplied:
+
+.. code-block:: python
+
+    from requests import session
+    from requests_futures.sessions import FuturesSession
+    my_session = session()
+    future_session = FuturesSession(session=my_session)
+
+That's it. The api of requests.Session is preserved without any modifications
+beyond returning a Future rather than Response. As with all futures exceptions
+are shifted (thrown) to the future.result() call so try/except blocks should be
+moved there.
+
+
+Tying extra information to the request/response
+===============================================
+
+The most common piece of information needed is the URL of the request. This can
+be accessed without any extra steps using the `request` property of the
+response object.
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+
+    futures=[session.get(f'http://httpbin.org/get?{i}') for i in range(3)]
+
+    for future in as_completed(futures):
+        resp = future.result()
+        pprint({
+            'url': resp.request.url,
+            'content': resp.json(),
+        })
+
+There are situations in which you may want to tie additional information to a
+request/response. There are a number of ways to go about this, the simplest is
+to attach additional information to the future object itself.
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+
+    futures=[]
+    for i in range(3):
+        future = session.get('http://httpbin.org/get')
+        future.i = i
+        futures.append(future)
+
+    for future in as_completed(futures):
+        resp = future.result()
+        pprint({
+            'i': future.i,
+            'content': resp.json(),
+        })
+
+Canceling queued requests (a.k.a cleaning up after yourself)
+============================================================
+
+If you know that you won't be needing any additional responses from futures that
+haven't yet resolved, it's a good idea to cancel those requests. You can do this
+by using the session as a context manager:
+
+.. code-block:: python
+
+    from requests_futures.sessions import FuturesSession
+    with FuturesSession(max_workers=1) as session:
+        future = session.get('https://httpbin.org/get')
+        future2 = session.get('https://httpbin.org/delay/10')
+        future3 = session.get('https://httpbin.org/delay/10')
+        response = future.result()
+
+In this example, the second or third request will be skipped, saving time and
+resources that would otherwise be wasted.
+
+Iterating over a list of requests responses
+===========================================
+
+Without preserving the requests order:
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from requests_futures.sessions import FuturesSession
+    with FuturesSession() as session:
+        futures = [session.get('https://httpbin.org/delay/{}'.format(i % 3)) for i in range(10)]
+        for future in as_completed(futures):
+            resp = future.result()
+            print(resp.json()['url'])
+
+Working in the Background
+=========================
+
+Additional processing can be done in the background using requests's hooks_
+functionality. This can be useful for shifting work out of the foreground, for
+a simple example take json parsing.
+
+.. code-block:: python
+
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+
+    def response_hook(resp, *args, **kwargs):
+        # parse the json storing the result on the response object
+        resp.data = resp.json()
+
+    future = session.get('http://httpbin.org/get', hooks={
+        'response': response_hook,
+    })
+    # do some other stuff, send some more requests while this one works
+    response = future.result()
+    print('response status {0}'.format(response.status_code))
+    # data will have been attached to the response object in the background
+    pprint(response.data)
+
+Hooks can also be applied to the session.
+
+.. code-block:: python
+
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    def response_hook(resp, *args, **kwargs):
+        # parse the json storing the result on the response object
+        resp.data = resp.json()
+
+    session = FuturesSession()
+    session.hooks['response'] = response_hook
+
+    future = session.get('http://httpbin.org/get')
+    # do some other stuff, send some more requests while this one works
+    response = future.result()
+    print('response status {0}'.format(response.status_code))
+    # data will have been attached to the response object in the background
+    pprint(response.data)   pprint(response.data)
+
+A more advanced example that adds an `elapsed` property to all requests.
+
+.. code-block:: python
+
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+    from time import time
+
+
+    class ElapsedFuturesSession(FuturesSession):
+
+        def request(self, method, url, hooks=None, *args, **kwargs):
+            start = time()
+            if hooks is None:
+                hooks = {}
+
+            def timing(r, *args, **kwargs):
+                r.elapsed = time() - start
+
+            try:
+                if isinstance(hooks['response'], (list, tuple)):
+                    # needs to be first so we don't time other hooks execution
+                    hooks['response'].insert(0, timing)
+                else:
+                    hooks['response'] = [timing, hooks['response']]
+            except KeyError:
+                hooks['response'] = timing
+
+            return super(ElapsedFuturesSession, self) \
+                .request(method, url, hooks=hooks, *args, **kwargs)
+
+
+
+    session = ElapsedFuturesSession()
+    future = session.get('http://httpbin.org/get')
+    # do some other stuff, send some more requests while this one works
+    response = future.result()
+    print('response status {0}'.format(response.status_code))
+    print('response elapsed {0}'.format(response.elapsed))
+
+Using ProcessPoolExecutor
+=========================
+
+Similarly to `ThreadPoolExecutor`, it is possible to use an instance of
+`ProcessPoolExecutor`. As the name suggest, the requests will be executed
+concurrently in separate processes rather than threads.
+
+.. code-block:: python
+
+    from concurrent.futures import ProcessPoolExecutor
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10))
+    # ... use as before
+
+.. HINT::
+    Using the `ProcessPoolExecutor` is useful, in cases where memory
+    usage per request is very high (large response) and cycling the interpreter
+    is required to release memory back to OS.
+
+A base requirement of using `ProcessPoolExecutor` is that the `Session.request`,
+`FutureSession` all be pickle-able.
+
+This means that only Python 3.5 is fully supported, while Python versions
+3.4 and above REQUIRE an existing `requests.Session` instance to be passed
+when initializing `FutureSession`. Python 2.X and < 3.4 are currently not
+supported.
+
+.. code-block:: python
+
+    # Using python 3.4
+    from concurrent.futures import ProcessPoolExecutor
+    from requests import Session
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10),
+                             session=Session())
+    # ... use as before
+
+In case pickling fails, an exception is raised pointing to this documentation.
+
+.. code-block:: python
+
+    # Using python 2.7
+    from concurrent.futures import ProcessPoolExecutor
+    from requests import Session
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10),
+                             session=Session())
+    Traceback (most recent call last):
+    ...
+    RuntimeError: Cannot pickle function. Refer to documentation: https://github.com/ross/requests-futures/#using-processpoolexecutor
+
+.. IMPORTANT::
+  * Python >= 3.4 required
+  * A session instance is required when using Python < 3.5
+  * If sub-classing `FuturesSession` it must be importable (module global)
+
+Installation
+============
+
+    pip install requests-futures
+
+.. _`requests`: https://github.com/kennethreitz/requests
+.. _`concurrent.futures`: http://docs.python.org/dev/library/concurrent.futures.html
+.. _backport: https://pypi.python.org/pypi/futures
+.. _hooks: http://docs.python-requests.org/en/master/user/advanced/#event-hooks
```

### Comparing `requests-futures-1.0.0/LICENSE` & `requests-futures-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-futures-1.0.0/requests_futures/sessions.py` & `requests-futures-1.0.1/requests_futures/sessions.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,37 +15,45 @@
     # ... do other stuff ...
     # wait for the request to complete, if it hasn't already
     response = future.result()
     print('response status: {0}'.format(response.status_code))
     print(response.content)
 
 """
-from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from functools import partial
 from logging import getLogger
-from pickle import dumps, PickleError
+from pickle import PickleError, dumps
 
 from requests import Session
 from requests.adapters import DEFAULT_POOLSIZE, HTTPAdapter
 
 
 def wrap(self, sup, background_callback, *args_, **kwargs_):
-    """ A global top-level is required for ProcessPoolExecutor """
+    """A global top-level is required for ProcessPoolExecutor"""
     resp = sup(*args_, **kwargs_)
     return background_callback(self, resp) or resp
 
 
-PICKLE_ERROR = ('Cannot pickle function. Refer to documentation: https://'
-                'github.com/ross/requests-futures/#using-processpoolexecutor')
+PICKLE_ERROR = (
+    'Cannot pickle function. Refer to documentation: https://'
+    'github.com/ross/requests-futures/#using-processpoolexecutor'
+)
 
 
 class FuturesSession(Session):
-
-    def __init__(self, executor=None, max_workers=8, session=None,
-                 adapter_kwargs=None, *args, **kwargs):
+    def __init__(
+        self,
+        executor=None,
+        max_workers=8,
+        session=None,
+        adapter_kwargs=None,
+        *args,
+        **kwargs
+    ):
         """Creates a FuturesSession
 
         Notes
         ~~~~~
         * `ProcessPoolExecutor` may be used with Python > 3.4;
           see README for more information.
 
@@ -55,16 +63,20 @@
         _adapter_kwargs = {}
         super(FuturesSession, self).__init__(*args, **kwargs)
         self._owned_executor = executor is None
         if executor is None:
             executor = ThreadPoolExecutor(max_workers=max_workers)
             # set connection pool size equal to max_workers if needed
             if max_workers > DEFAULT_POOLSIZE:
-                _adapter_kwargs.update({'pool_connections': max_workers,
-                                        'pool_maxsize': max_workers})
+                _adapter_kwargs.update(
+                    {
+                        'pool_connections': max_workers,
+                        'pool_maxsize': max_workers,
+                    }
+                )
 
         _adapter_kwargs.update(adapter_kwargs or {})
 
         if _adapter_kwargs:
             self.mount('https://', HTTPAdapter(**_adapter_kwargs))
             self.mount('http://', HTTPAdapter(**_adapter_kwargs))
 
@@ -87,16 +99,18 @@
         else:
             # avoid calling super to not break pickled method
             func = partial(Session.request, self)
 
         background_callback = kwargs.pop('background_callback', None)
         if background_callback:
             logger = getLogger(self.__class__.__name__)
-            logger.warning('`background_callback` is deprecated and will be '
-                        'removed in 1.0, use `hooks` instead')
+            logger.warning(
+                '`background_callback` is deprecated and will be '
+                'removed in 1.0, use `hooks` instead'
+            )
             func = partial(wrap, self, func, background_callback)
 
         if isinstance(self.executor, ProcessPoolExecutor):
             # verify function can be pickled
             try:
                 dumps(func)
             except (TypeError, PickleError):
@@ -143,15 +157,17 @@
         :param url: URL for the new :class:`Request` object.
         :param data: (optional) Dictionary, list of tuples, bytes, or file-like
             object to send in the body of the :class:`Request`.
         :param json: (optional) json to send in the body of the :class:`Request`.
         :param \*\*kwargs: Optional arguments that ``request`` takes.
         :rtype : concurrent.futures.Future
         """
-        return super(FuturesSession, self).post(url, data=data, json=json, **kwargs)
+        return super(FuturesSession, self).post(
+            url, data=data, json=json, **kwargs
+        )
 
     def put(self, url, data=None, **kwargs):
         r"""Sends a PUT request. Returns :class:`Future` object.
 
         :param url: URL for the new :class:`Request` object.
         :param data: (optional) Dictionary, list of tuples, bytes, or file-like
             object to send in the body of the :class:`Request`.
```

### Comparing `requests-futures-1.0.0/requests_futures/__init__.py` & `requests-futures-1.0.1/requests_futures/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 
 
 """
 
 import logging
 
 __title__ = 'requests-futures'
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __build__ = 0x000000
 __author__ = 'Ross McFarland'
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2013 Ross McFarland'
 
 # Set default logging handler to avoid "No handler found" warnings.
 try:  # Python 2.7+
     from logging import NullHandler
 except ImportError:
+
     class NullHandler(logging.Handler):
         def emit(self, record):
             pass
 
+
 logging.getLogger(__name__).addHandler(NullHandler())
```

### Comparing `requests-futures-1.0.0/test_requests_futures.py` & `requests-futures-1.0.1/tests/test_requests_futures.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 # -*- coding: utf-8 -*-
 
 """Tests for Requests."""
 
 from concurrent.futures import Future, ProcessPoolExecutor
 from os import environ
 from sys import version_info
+
 try:
     from sys import pypy_version_info
 except ImportError:
     pypy_version_info = None
-from unittest import TestCase, main, skipIf
 import logging
+from unittest import TestCase, main, skipIf
 
+import pytest
 from requests import Response, session
 from requests.adapters import DEFAULT_POOLSIZE
+
 from requests_futures.sessions import FuturesSession
 
-HTTPBIN = environ.get('HTTPBIN_URL', 'http://httpbin.org/')
+HTTPBIN = environ.get('HTTPBIN_URL', 'https://nghttp2.org/httpbin/')
 logging.basicConfig(level=logging.DEBUG)
 logging.getLogger('urllib3.connectionpool').level = logging.WARNING
 logging.getLogger('FuturesSession').level = logging.ERROR
 
 
 def httpbin(*suffix):
     """Returns url for HTTPBIN resource."""
     return HTTPBIN + '/'.join(suffix)
 
 
 class RequestsTestCase(TestCase):
-
+    @pytest.mark.network
     def test_futures_session(self):
         # basic futures get
         sess = FuturesSession()
         future = sess.get(httpbin('get'))
         self.assertIsInstance(future, Future)
         resp = future.result()
         self.assertIsInstance(resp, Response)
@@ -61,79 +64,88 @@
             raise Exception('boom')
 
         future = sess.get(httpbin('get'), background_callback=rasing_cb)
         with self.assertRaises(Exception) as cm:
             resp = future.result()
         self.assertEqual('boom', cm.exception.args[0])
 
+    @pytest.mark.network
     def test_supplied_session(self):
-        """ Tests the `session` keyword argument. """
+        """Tests the `session` keyword argument."""
         requests_session = session()
         requests_session.headers['Foo'] = 'bar'
         sess = FuturesSession(session=requests_session)
         future = sess.get(httpbin('headers'))
         self.assertIsInstance(future, Future)
         resp = future.result()
         self.assertIsInstance(resp, Response)
         self.assertEqual(200, resp.status_code)
         self.assertEqual(resp.json()['headers']['Foo'], 'bar')
 
     def test_max_workers(self):
-        """ Tests the `max_workers` shortcut. """
+        """Tests the `max_workers` shortcut."""
         from concurrent.futures import ThreadPoolExecutor
+
         session = FuturesSession()
         self.assertEqual(session.executor._max_workers, 8)
         session = FuturesSession(max_workers=5)
         self.assertEqual(session.executor._max_workers, 5)
         session = FuturesSession(executor=ThreadPoolExecutor(max_workers=10))
         self.assertEqual(session.executor._max_workers, 10)
-        session = FuturesSession(executor=ThreadPoolExecutor(max_workers=10),
-                                 max_workers=5)
+        session = FuturesSession(
+            executor=ThreadPoolExecutor(max_workers=10), max_workers=5
+        )
         self.assertEqual(session.executor._max_workers, 10)
 
     def test_adapter_kwargs(self):
-        """ Tests the `adapter_kwargs` shortcut. """
+        """Tests the `adapter_kwargs` shortcut."""
         from concurrent.futures import ThreadPoolExecutor
+
         session = FuturesSession()
         self.assertFalse(session.get_adapter('http://')._pool_block)
-        session = FuturesSession(max_workers=DEFAULT_POOLSIZE + 1,
-                                 adapter_kwargs={'pool_block': True})
+        session = FuturesSession(
+            max_workers=DEFAULT_POOLSIZE + 1,
+            adapter_kwargs={'pool_block': True},
+        )
         adapter = session.get_adapter('http://')
         self.assertTrue(adapter._pool_block)
         self.assertEqual(adapter._pool_connections, DEFAULT_POOLSIZE + 1)
         self.assertEqual(adapter._pool_maxsize, DEFAULT_POOLSIZE + 1)
-        session = FuturesSession(executor=ThreadPoolExecutor(max_workers=10),
-                                 adapter_kwargs={'pool_connections': 20})
+        session = FuturesSession(
+            executor=ThreadPoolExecutor(max_workers=10),
+            adapter_kwargs={'pool_connections': 20},
+        )
         self.assertEqual(session.get_adapter('http://')._pool_connections, 20)
 
+    @pytest.mark.network
     def test_redirect(self):
-        """ Tests for the ability to cleanly handle redirects. """
+        """Tests for the ability to cleanly handle redirects."""
         sess = FuturesSession()
         future = sess.get(httpbin('redirect-to?url=get'))
         self.assertIsInstance(future, Future)
         resp = future.result()
         self.assertIsInstance(resp, Response)
         self.assertEqual(200, resp.status_code)
 
         future = sess.get(httpbin('redirect-to?url=status/404'))
         resp = future.result()
         self.assertEqual(404, resp.status_code)
 
+    @pytest.mark.network
     def test_context(self):
-
         class FuturesSessionTestHelper(FuturesSession):
-
             def __init__(self, *args, **kwargs):
                 super(FuturesSessionTestHelper, self).__init__(*args, **kwargs)
                 self._exit_called = False
 
             def __exit__(self, *args, **kwargs):
                 self._exit_called = True
-                return super(FuturesSessionTestHelper, self).__exit__(*args,
-                                                                      **kwargs)
+                return super(FuturesSessionTestHelper, self).__exit__(
+                    *args, **kwargs
+                )
 
         passout = None
         with FuturesSessionTestHelper() as sess:
             passout = sess
             future = sess.get(httpbin('get'))
             self.assertIsInstance(future, Future)
             resp = future.result()
@@ -142,53 +154,55 @@
 
         self.assertTrue(passout._exit_called)
 
 
 # << test process pool executor >>
 # see discussion https://github.com/ross/requests-futures/issues/11
 def global_cb_modify_response(s, r):
-    """ add the parsed json data to the response """
+    """add the parsed json data to the response"""
     assert s, FuturesSession
     assert r, Response
     r.data = r.json()
     r.__attrs__.append('data')  # required for pickling new attribute
 
 
 def global_cb_return_result(s, r):
-    """ simply return parsed json data """
+    """simply return parsed json data"""
     assert s, FuturesSession
     assert r, Response
     return r.json()
 
 
 def global_rasing_cb(s, r):
     raise Exception('boom')
 
 
 # pickling instance method supported only from here
 unsupported_platform = version_info < (3, 4) and not pypy_version_info
-session_required = version_info < (3, 5,) and not pypy_version_info
+session_required = version_info < (3, 5) and not pypy_version_info
 
 
 @skipIf(unsupported_platform, 'not supported in python < 3.4')
 class RequestsProcessPoolTestCase(TestCase):
-
     def setUp(self):
         self.proc_executor = ProcessPoolExecutor(max_workers=2)
         self.session = session()
 
+    @pytest.mark.network
     @skipIf(session_required, 'not supported in python < 3.5')
     def test_futures_session(self):
         self._assert_futures_session()
 
+    @pytest.mark.network
     @skipIf(not session_required, 'fully supported on python >= 3.5')
     def test_exception_raised(self):
         with self.assertRaises(RuntimeError):
             self._assert_futures_session()
 
+    @pytest.mark.network
     def test_futures_existing_session(self):
         self.session.headers['Foo'] = 'bar'
         self._assert_futures_session(session=self.session)
 
     def _assert_futures_session(self, session=None):
         # basic futures get
         if session:
@@ -203,26 +217,28 @@
         self.assertEqual(200, resp.status_code)
 
         # non-200, 404
         future = sess.get(httpbin('status/404'))
         resp = future.result()
         self.assertEqual(404, resp.status_code)
 
-        future = sess.get(httpbin('get'),
-                          background_callback=global_cb_modify_response)
+        future = sess.get(
+            httpbin('get'), background_callback=global_cb_modify_response
+        )
         # this should block until complete
         resp = future.result()
         if session:
             self.assertEqual(resp.json()['headers']['Foo'], 'bar')
         self.assertEqual(200, resp.status_code)
         # make sure the callback was invoked
         self.assertTrue(hasattr(resp, 'data'))
 
-        future = sess.get(httpbin('get'),
-                          background_callback=global_cb_return_result)
+        future = sess.get(
+            httpbin('get'), background_callback=global_cb_return_result
+        )
         # this should block until complete
         resp = future.result()
         # make sure the callback was invoked
         self.assertIsInstance(resp, dict)
 
         future = sess.get(httpbin('get'), background_callback=global_rasing_cb)
         with self.assertRaises(Exception) as cm:
@@ -236,25 +252,28 @@
         self.assertIsInstance(resp, Response)
         self.assertEqual(200, resp.status_code)
 
         future = sess.get(httpbin('redirect-to?url=status/404'))
         resp = future.result()
         self.assertEqual(404, resp.status_code)
 
+    @pytest.mark.network
     @skipIf(session_required, 'not supported in python < 3.5')
     def test_context(self):
         self._assert_context()
 
+    @pytest.mark.network
     def test_context_with_session(self):
         self._assert_context(session=self.session)
 
     def _assert_context(self, session=None):
         if session:
-            helper_instance = TopLevelContextHelper(executor=self.proc_executor,
-                                                    session=self.session)
+            helper_instance = TopLevelContextHelper(
+                executor=self.proc_executor, session=self.session
+            )
         else:
             helper_instance = TopLevelContextHelper(executor=self.proc_executor)
         passout = None
         with helper_instance as sess:
             passout = sess
             future = sess.get(httpbin('get'))
             self.assertIsInstance(future, Future)
@@ -263,26 +282,25 @@
             self.assertEqual(200, resp.status_code)
 
         self.assertTrue(passout._exit_called)
 
 
 class TopLevelContextHelper(FuturesSession):
     def __init__(self, *args, **kwargs):
-        super(TopLevelContextHelper, self).__init__(
-            *args, **kwargs)
+        super(TopLevelContextHelper, self).__init__(*args, **kwargs)
         self._exit_called = False
 
     def __exit__(self, *args, **kwargs):
         self._exit_called = True
-        return super(TopLevelContextHelper, self).__exit__(
-            *args, **kwargs)
+        return super(TopLevelContextHelper, self).__exit__(*args, **kwargs)
 
 
 @skipIf(not unsupported_platform, 'Exception raised when unsupported')
 class ProcessPoolExceptionRaisedTestCase(TestCase):
+    @pytest.mark.network
     def test_exception_raised(self):
         executor = ProcessPoolExecutor(max_workers=2)
         sess = FuturesSession(executor=executor, session=session())
         with self.assertRaises(RuntimeError):
             sess.get(httpbin('get'))
```

### Comparing `requests-futures-1.0.0/requests_futures.egg-info/PKG-INFO` & `requests-futures-1.0.1/requests_futures.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,276 +1,346 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: requests-futures
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous Python HTTP for Humans.
 Home-page: https://github.com/ross/requests-futures
 Author: Ross McFarland
-Author-email: rwmcfa1@neces.com
+Author-email: rwmcfa1@rwmcfa1.com
 License: Apache License v2
-Description: Asynchronous Python HTTP Requests for Humans
-        ============================================
-        
-        .. image:: https://travis-ci.org/ross/requests-futures.png?branch=master
-                :target: https://travis-ci.org/ross/requests-futures
-        
-        Small add-on for the python requests_ http library. Makes use of python 3.2's
-        `concurrent.futures`_ or the backport_ for prior versions of python.
-        
-        The additional API and changes are minimal and strives to avoid surprises.
-        
-        The following synchronous code:
-        
-        .. code-block:: python
-        
-            from requests import Session
-        
-            session = Session()
-            # first requests starts and blocks until finished
-            response_one = session.get('http://httpbin.org/get')
-            # second request starts once first is finished
-            response_two = session.get('http://httpbin.org/get?foo=bar')
-            # both requests are complete
-            print('response one status: {0}'.format(response_one.status_code))
-            print(response_one.content)
-            print('response two status: {0}'.format(response_two.status_code))
-            print(response_two.content)
-        
-        Can be translated to make use of futures, and thus be asynchronous by creating
-        a FuturesSession and catching the returned Future in place of Response. The
-        Response can be retrieved by calling the result method on the Future:
-        
-        .. code-block:: python
-        
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession()
-            # first request is started in background
-            future_one = session.get('http://httpbin.org/get')
-            # second requests is started immediately
-            future_two = session.get('http://httpbin.org/get?foo=bar')
-            # wait for the first request to complete, if it hasn't already
-            response_one = future_one.result()
-            print('response one status: {0}'.format(response_one.status_code))
-            print(response_one.content)
-            # wait for the second request to complete, if it hasn't already
-            response_two = future_two.result()
-            print('response two status: {0}'.format(response_two.status_code))
-            print(response_two.content)
-        
-        By default a ThreadPoolExecutor is created with 8 workers. If you would like to
-        adjust that value or share a executor across multiple sessions you can provide
-        one to the FuturesSession constructor.
-        
-        .. code-block:: python
-        
-            from concurrent.futures import ThreadPoolExecutor
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession(executor=ThreadPoolExecutor(max_workers=10))
-            # ...
-        
-        As a shortcut in case of just increasing workers number you can pass
-        `max_workers` straight to the `FuturesSession` constructor:
-        
-        .. code-block:: python
-        
-            from requests_futures.sessions import FuturesSession
-            session = FuturesSession(max_workers=10)
-        
-        FutureSession will use an existing session object if supplied:
-        
-        .. code-block:: python
-        
-            from requests import session
-            from requests_futures.sessions import FuturesSession
-            my_session = session()
-            future_session = FuturesSession(session=my_session)
-        
-        That's it. The api of requests.Session is preserved without any modifications
-        beyond returning a Future rather than Response. As with all futures exceptions
-        are shifted (thrown) to the future.result() call so try/except blocks should be
-        moved there.
-        
-        Canceling queued requests (a.k.a cleaning up after yourself)
-        ============================================================
-        
-        If you know that you won't be needing any additional responses from futures that
-        haven't yet resolved, it's a good idea to cancel those requests. You can do this
-        by using the session as a context manager:
-        
-        .. code-block:: python
-        
-            from requests_futures.sessions import FuturesSession
-            with FuturesSession(max_workers=1) as session:
-                future = session.get('https://httpbin.org/get')
-                future2 = session.get('https://httpbin.org/delay/10')
-                future3 = session.get('https://httpbin.org/delay/10')
-                response = future.result()
-        
-        In this example, the second or third request will be skipped, saving time and
-        resources that would otherwise be wasted.
-        
-        Working in the Background
-        =========================
-        
-        Additional processing can be done in the background using requests's hooks_
-        functionality. This can be useful for shifting work out of the foreground, for
-        a simple example take json parsing.
-        
-        .. code-block:: python
-        
-            from pprint import pprint
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession()
-        
-            def response_hook(resp, *args, **kwargs):
-                # parse the json storing the result on the response object
-                resp.data = resp.json()
-        
-            future = session.get('http://httpbin.org/get', hooks={
-                'response': response_hook,
-            })
-            # do some other stuff, send some more requests while this one works
-            response = future.result()
-            print('response status {0}'.format(response.status_code))
-            # data will have been attached to the response object in the background
-            pprint(response.data)
-        
-        Hooks can also be applied to the session.
-        
-        .. code-block:: python
-        
-            from pprint import pprint
-            from requests_futures.sessions import FuturesSession
-        
-            def response_hook(resp, *args, **kwargs):
-                # parse the json storing the result on the response object
-                resp.data = resp.json()
-        
-            session = FuturesSession()
-            session.hooks['response'] = response_hook
-        
-            future = session.get('http://httpbin.org/get')
-            # do some other stuff, send some more requests while this one works
-            response = future.result()
-            print('response status {0}'.format(response.status_code))
-            # data will have been attached to the response object in the background
-            pprint(response.data)   pprint(response.data)
-        
-        A more advanced example that adds an `elapsed` property to all requests.
-        
-        .. code-block:: python
-        
-            from pprint import pprint
-            from requests_futures.sessions import FuturesSession
-            from time import time
-        
-        
-            class ElapsedFuturesSession(FuturesSession):
-        
-                def request(self, method, url, hooks={}, *args, **kwargs):
-                    start = time()
-        
-                    def timing(r, *args, **kwargs):
-                        r.elapsed = time() - start
-        
-                    try:
-                        if isinstance(hooks['response'], (list, tuple)):
-                            # needs to be first so we don't time other hooks execution
-                            hooks['response'].insert(0, timing)
-                        else:
-                            hooks['response'] = [timing, hooks['response']]
-                    except KeyError:
-                        hooks['response'] = timing
-        
-                    return super(ElapsedFuturesSession, self) \
-                        .request(method, url, hooks=hooks, *args, **kwargs)
-        
-        
-        
-            session = ElapsedFuturesSession()
-            future = session.get('http://httpbin.org/get')
-            # do some other stuff, send some more requests while this one works
-            response = future.result()
-            print('response status {0}'.format(response.status_code))
-            print('response elapsed {0}'.format(response.elapsed))
-        
-        Using ProcessPoolExecutor
-        =========================
-        
-        Similarly to `ThreadPoolExecutor`, it is possible to use an instance of
-        `ProcessPoolExecutor`. As the name suggest, the requests will be executed
-        concurrently in separate processes rather than threads.
-        
-        .. code-block:: python
-        
-            from concurrent.futures import ProcessPoolExecutor
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10))
-            # ... use as before
-        
-        .. HINT::
-            Using the `ProcessPoolExecutor` is useful, in cases where memory
-            usage per request is very high (large response) and cycling the interpretor
-            is required to release memory back to OS.
-        
-        A base requirement of using `ProcessPoolExecutor` is that the `Session.request`,
-        `FutureSession` all be pickle-able.
-        
-        This means that only Python 3.5 is fully supported, while Python versions
-        3.4 and above REQUIRE an existing `requests.Session` instance to be passed
-        when initializing `FutureSession`. Python 2.X and < 3.4 are currently not
-        supported.
-        
-        .. code-block:: python
-        
-            # Using python 3.4
-            from concurrent.futures import ProcessPoolExecutor
-            from requests import Session
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10),
-                                     session=Session())
-            # ... use as before
-        
-        In case pickling fails, an exception is raised pointing to this documentation.
-        
-        .. code-block:: python
-        
-            # Using python 2.7
-            from concurrent.futures import ProcessPoolExecutor
-            from requests import Session
-            from requests_futures.sessions import FuturesSession
-        
-            session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10),
-                                     session=Session())
-            Traceback (most recent call last):
-            ...
-            RuntimeError: Cannot pickle function. Refer to documentation: https://github.com/ross/requests-futures/#using-processpoolexecutor
-        
-        .. IMPORTANT::
-          * Python >= 3.4 required
-          * A session instance is required when using Python < 3.5
-          * If sub-classing `FuturesSession` it must be importable (module global)
-        
-        Installation
-        ============
-        
-            pip install requests-futures
-        
-        .. _`requests`: https://github.com/kennethreitz/requests
-        .. _`concurrent.futures`: http://docs.python.org/dev/library/concurrent.futures.html
-        .. _backport: https://pypi.python.org/pypi/futures
-        .. _hooks: http://docs.python-requests.org/en/master/user/advanced/#event-hooks
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
+Asynchronous Python HTTP Requests for Humans
+============================================
+
+.. image:: https://travis-ci.org/ross/requests-futures.svg?branch=master
+        :target: https://travis-ci.org/ross/requests-futures
+
+Small add-on for the python requests_ http library. Makes use of python 3.2's
+`concurrent.futures`_ or the backport_ for prior versions of python.
+
+The additional API and changes are minimal and strives to avoid surprises.
+
+The following synchronous code:
+
+.. code-block:: python
+
+    from requests import Session
+
+    session = Session()
+    # first requests starts and blocks until finished
+    response_one = session.get('http://httpbin.org/get')
+    # second request starts once first is finished
+    response_two = session.get('http://httpbin.org/get?foo=bar')
+    # both requests are complete
+    print('response one status: {0}'.format(response_one.status_code))
+    print(response_one.content)
+    print('response two status: {0}'.format(response_two.status_code))
+    print(response_two.content)
+
+Can be translated to make use of futures, and thus be asynchronous by creating
+a FuturesSession and catching the returned Future in place of Response. The
+Response can be retrieved by calling the result method on the Future:
+
+.. code-block:: python
+
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+    # first request is started in background
+    future_one = session.get('http://httpbin.org/get')
+    # second requests is started immediately
+    future_two = session.get('http://httpbin.org/get?foo=bar')
+    # wait for the first request to complete, if it hasn't already
+    response_one = future_one.result()
+    print('response one status: {0}'.format(response_one.status_code))
+    print(response_one.content)
+    # wait for the second request to complete, if it hasn't already
+    response_two = future_two.result()
+    print('response two status: {0}'.format(response_two.status_code))
+    print(response_two.content)
+
+By default a ThreadPoolExecutor is created with 8 workers. If you would like to
+adjust that value or share a executor across multiple sessions you can provide
+one to the FuturesSession constructor.
+
+.. code-block:: python
+
+    from concurrent.futures import ThreadPoolExecutor
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession(executor=ThreadPoolExecutor(max_workers=10))
+    # ...
+
+As a shortcut in case of just increasing workers number you can pass
+`max_workers` straight to the `FuturesSession` constructor:
+
+.. code-block:: python
+
+    from requests_futures.sessions import FuturesSession
+    session = FuturesSession(max_workers=10)
+
+FutureSession will use an existing session object if supplied:
+
+.. code-block:: python
+
+    from requests import session
+    from requests_futures.sessions import FuturesSession
+    my_session = session()
+    future_session = FuturesSession(session=my_session)
+
+That's it. The api of requests.Session is preserved without any modifications
+beyond returning a Future rather than Response. As with all futures exceptions
+are shifted (thrown) to the future.result() call so try/except blocks should be
+moved there.
+
+
+Tying extra information to the request/response
+===============================================
+
+The most common piece of information needed is the URL of the request. This can
+be accessed without any extra steps using the `request` property of the
+response object.
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+
+    futures=[session.get(f'http://httpbin.org/get?{i}') for i in range(3)]
+
+    for future in as_completed(futures):
+        resp = future.result()
+        pprint({
+            'url': resp.request.url,
+            'content': resp.json(),
+        })
+
+There are situations in which you may want to tie additional information to a
+request/response. There are a number of ways to go about this, the simplest is
+to attach additional information to the future object itself.
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+
+    futures=[]
+    for i in range(3):
+        future = session.get('http://httpbin.org/get')
+        future.i = i
+        futures.append(future)
+
+    for future in as_completed(futures):
+        resp = future.result()
+        pprint({
+            'i': future.i,
+            'content': resp.json(),
+        })
+
+Canceling queued requests (a.k.a cleaning up after yourself)
+============================================================
+
+If you know that you won't be needing any additional responses from futures that
+haven't yet resolved, it's a good idea to cancel those requests. You can do this
+by using the session as a context manager:
+
+.. code-block:: python
+
+    from requests_futures.sessions import FuturesSession
+    with FuturesSession(max_workers=1) as session:
+        future = session.get('https://httpbin.org/get')
+        future2 = session.get('https://httpbin.org/delay/10')
+        future3 = session.get('https://httpbin.org/delay/10')
+        response = future.result()
+
+In this example, the second or third request will be skipped, saving time and
+resources that would otherwise be wasted.
+
+Iterating over a list of requests responses
+===========================================
+
+Without preserving the requests order:
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from requests_futures.sessions import FuturesSession
+    with FuturesSession() as session:
+        futures = [session.get('https://httpbin.org/delay/{}'.format(i % 3)) for i in range(10)]
+        for future in as_completed(futures):
+            resp = future.result()
+            print(resp.json()['url'])
+
+Working in the Background
+=========================
+
+Additional processing can be done in the background using requests's hooks_
+functionality. This can be useful for shifting work out of the foreground, for
+a simple example take json parsing.
+
+.. code-block:: python
+
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+
+    def response_hook(resp, *args, **kwargs):
+        # parse the json storing the result on the response object
+        resp.data = resp.json()
+
+    future = session.get('http://httpbin.org/get', hooks={
+        'response': response_hook,
+    })
+    # do some other stuff, send some more requests while this one works
+    response = future.result()
+    print('response status {0}'.format(response.status_code))
+    # data will have been attached to the response object in the background
+    pprint(response.data)
+
+Hooks can also be applied to the session.
+
+.. code-block:: python
+
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    def response_hook(resp, *args, **kwargs):
+        # parse the json storing the result on the response object
+        resp.data = resp.json()
+
+    session = FuturesSession()
+    session.hooks['response'] = response_hook
+
+    future = session.get('http://httpbin.org/get')
+    # do some other stuff, send some more requests while this one works
+    response = future.result()
+    print('response status {0}'.format(response.status_code))
+    # data will have been attached to the response object in the background
+    pprint(response.data)   pprint(response.data)
+
+A more advanced example that adds an `elapsed` property to all requests.
+
+.. code-block:: python
+
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+    from time import time
+
+
+    class ElapsedFuturesSession(FuturesSession):
+
+        def request(self, method, url, hooks=None, *args, **kwargs):
+            start = time()
+            if hooks is None:
+                hooks = {}
+
+            def timing(r, *args, **kwargs):
+                r.elapsed = time() - start
+
+            try:
+                if isinstance(hooks['response'], (list, tuple)):
+                    # needs to be first so we don't time other hooks execution
+                    hooks['response'].insert(0, timing)
+                else:
+                    hooks['response'] = [timing, hooks['response']]
+            except KeyError:
+                hooks['response'] = timing
+
+            return super(ElapsedFuturesSession, self) \
+                .request(method, url, hooks=hooks, *args, **kwargs)
+
+
+
+    session = ElapsedFuturesSession()
+    future = session.get('http://httpbin.org/get')
+    # do some other stuff, send some more requests while this one works
+    response = future.result()
+    print('response status {0}'.format(response.status_code))
+    print('response elapsed {0}'.format(response.elapsed))
+
+Using ProcessPoolExecutor
+=========================
+
+Similarly to `ThreadPoolExecutor`, it is possible to use an instance of
+`ProcessPoolExecutor`. As the name suggest, the requests will be executed
+concurrently in separate processes rather than threads.
+
+.. code-block:: python
+
+    from concurrent.futures import ProcessPoolExecutor
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10))
+    # ... use as before
+
+.. HINT::
+    Using the `ProcessPoolExecutor` is useful, in cases where memory
+    usage per request is very high (large response) and cycling the interpreter
+    is required to release memory back to OS.
+
+A base requirement of using `ProcessPoolExecutor` is that the `Session.request`,
+`FutureSession` all be pickle-able.
+
+This means that only Python 3.5 is fully supported, while Python versions
+3.4 and above REQUIRE an existing `requests.Session` instance to be passed
+when initializing `FutureSession`. Python 2.X and < 3.4 are currently not
+supported.
+
+.. code-block:: python
+
+    # Using python 3.4
+    from concurrent.futures import ProcessPoolExecutor
+    from requests import Session
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10),
+                             session=Session())
+    # ... use as before
+
+In case pickling fails, an exception is raised pointing to this documentation.
+
+.. code-block:: python
+
+    # Using python 2.7
+    from concurrent.futures import ProcessPoolExecutor
+    from requests import Session
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10),
+                             session=Session())
+    Traceback (most recent call last):
+    ...
+    RuntimeError: Cannot pickle function. Refer to documentation: https://github.com/ross/requests-futures/#using-processpoolexecutor
+
+.. IMPORTANT::
+  * Python >= 3.4 required
+  * A session instance is required when using Python < 3.5
+  * If sub-classing `FuturesSession` it must be importable (module global)
+
+Installation
+============
+
+    pip install requests-futures
+
+.. _`requests`: https://github.com/kennethreitz/requests
+.. _`concurrent.futures`: http://docs.python.org/dev/library/concurrent.futures.html
+.. _backport: https://pypi.python.org/pypi/futures
+.. _hooks: http://docs.python-requests.org/en/master/user/advanced/#event-hooks
```

### Comparing `requests-futures-1.0.0/README.rst` & `requests-futures-1.0.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Asynchronous Python HTTP Requests for Humans
 ============================================
 
-.. image:: https://travis-ci.org/ross/requests-futures.png?branch=master
+.. image:: https://travis-ci.org/ross/requests-futures.svg?branch=master
         :target: https://travis-ci.org/ross/requests-futures
 
 Small add-on for the python requests_ http library. Makes use of python 3.2's
 `concurrent.futures`_ or the backport_ for prior versions of python.
 
 The additional API and changes are minimal and strives to avoid surprises.
 
@@ -78,14 +78,64 @@
     future_session = FuturesSession(session=my_session)
 
 That's it. The api of requests.Session is preserved without any modifications
 beyond returning a Future rather than Response. As with all futures exceptions
 are shifted (thrown) to the future.result() call so try/except blocks should be
 moved there.
 
+
+Tying extra information to the request/response
+===============================================
+
+The most common piece of information needed is the URL of the request. This can
+be accessed without any extra steps using the `request` property of the
+response object.
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+
+    futures=[session.get(f'http://httpbin.org/get?{i}') for i in range(3)]
+
+    for future in as_completed(futures):
+        resp = future.result()
+        pprint({
+            'url': resp.request.url,
+            'content': resp.json(),
+        })
+
+There are situations in which you may want to tie additional information to a
+request/response. There are a number of ways to go about this, the simplest is
+to attach additional information to the future object itself.
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from pprint import pprint
+    from requests_futures.sessions import FuturesSession
+
+    session = FuturesSession()
+
+    futures=[]
+    for i in range(3):
+        future = session.get('http://httpbin.org/get')
+        future.i = i
+        futures.append(future)
+
+    for future in as_completed(futures):
+        resp = future.result()
+        pprint({
+            'i': future.i,
+            'content': resp.json(),
+        })
+
 Canceling queued requests (a.k.a cleaning up after yourself)
 ============================================================
 
 If you know that you won't be needing any additional responses from futures that
 haven't yet resolved, it's a good idea to cancel those requests. You can do this
 by using the session as a context manager:
 
@@ -97,14 +147,29 @@
         future2 = session.get('https://httpbin.org/delay/10')
         future3 = session.get('https://httpbin.org/delay/10')
         response = future.result()
 
 In this example, the second or third request will be skipped, saving time and
 resources that would otherwise be wasted.
 
+Iterating over a list of requests responses
+===========================================
+
+Without preserving the requests order:
+
+.. code-block:: python
+
+    from concurrent.futures import as_completed
+    from requests_futures.sessions import FuturesSession
+    with FuturesSession() as session:
+        futures = [session.get('https://httpbin.org/delay/{}'.format(i % 3)) for i in range(10)]
+        for future in as_completed(futures):
+            resp = future.result()
+            print(resp.json()['url'])
+
 Working in the Background
 =========================
 
 Additional processing can be done in the background using requests's hooks_
 functionality. This can be useful for shifting work out of the foreground, for
 a simple example take json parsing.
 
@@ -156,16 +221,18 @@
     from pprint import pprint
     from requests_futures.sessions import FuturesSession
     from time import time
 
 
     class ElapsedFuturesSession(FuturesSession):
 
-        def request(self, method, url, hooks={}, *args, **kwargs):
+        def request(self, method, url, hooks=None, *args, **kwargs):
             start = time()
+            if hooks is None:
+                hooks = {}
 
             def timing(r, *args, **kwargs):
                 r.elapsed = time() - start
 
             try:
                 if isinstance(hooks['response'], (list, tuple)):
                     # needs to be first so we don't time other hooks execution
@@ -200,15 +267,15 @@
     from requests_futures.sessions import FuturesSession
 
     session = FuturesSession(executor=ProcessPoolExecutor(max_workers=10))
     # ... use as before
 
 .. HINT::
     Using the `ProcessPoolExecutor` is useful, in cases where memory
-    usage per request is very high (large response) and cycling the interpretor
+    usage per request is very high (large response) and cycling the interpreter
     is required to release memory back to OS.
 
 A base requirement of using `ProcessPoolExecutor` is that the `Session.request`,
 `FutureSession` all be pickle-able.
 
 This means that only Python 3.5 is fully supported, while Python versions
 3.4 and above REQUIRE an existing `requests.Session` instance to be passed
```

