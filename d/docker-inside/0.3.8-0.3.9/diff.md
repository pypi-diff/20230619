# Comparing `tmp/docker-inside-0.3.8.tar.gz` & `tmp/docker-inside-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docker-inside-0.3.8.tar", last modified: Sun Feb 18 00:58:45 2018, max compression
+gzip compressed data, was "dist/docker-inside-0.3.9.tar", last modified: Sun May 13 09:54:08 2018, max compression
```

## Comparing `docker-inside-0.3.8.tar` & `docker-inside-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-18 00:58:45.000000 docker-inside-0.3.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3374 2018-02-18 00:57:17.000000 docker-inside-0.3.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1527 2018-02-18 00:57:17.000000 docker-inside-0.3.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-18 00:58:45.000000 docker-inside-0.3.8/docker_inside.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2018-02-18 00:58:45.000000 docker-inside-0.3.8/docker_inside.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2018-02-18 00:58:45.000000 docker-inside-0.3.8/docker_inside.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4937 2018-02-18 00:58:45.000000 docker-inside-0.3.8/docker_inside.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-02-18 00:58:45.000000 docker-inside-0.3.8/docker_inside.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2018-02-18 00:58:45.000000 docker-inside-0.3.8/docker_inside.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      394 2018-02-18 00:58:45.000000 docker-inside-0.3.8/docker_inside.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-02-18 00:58:45.000000 docker-inside-0.3.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2018-02-18 00:57:17.000000 docker-inside-0.3.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4937 2018-02-18 00:58:45.000000 docker-inside-0.3.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-18 00:58:45.000000 docker-inside-0.3.8/dockerinside/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6679 2018-02-18 00:57:17.000000 docker-inside-0.3.8/dockerinside/dockerutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2018-02-18 00:57:17.000000 docker-inside-0.3.8/dockerinside/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17024 2018-02-18 00:57:17.000000 docker-inside-0.3.8/dockerinside/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-18 00:58:45.000000 docker-inside-0.3.8/dockerinside/setup/
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2018-02-18 00:57:17.000000 docker-inside-0.3.8/dockerinside/setup/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4458 2018-02-18 00:57:17.000000 docker-inside-0.3.8/dockerinside/setup/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-13 09:54:08.000000 docker-inside-0.3.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3454 2018-05-13 09:52:46.000000 docker-inside-0.3.9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1527 2018-05-13 09:52:46.000000 docker-inside-0.3.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-13 09:54:08.000000 docker-inside-0.3.9/docker_inside.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2018-05-13 09:54:08.000000 docker-inside-0.3.9/docker_inside.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2018-05-13 09:54:08.000000 docker-inside-0.3.9/docker_inside.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5024 2018-05-13 09:54:08.000000 docker-inside-0.3.9/docker_inside.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-05-13 09:54:08.000000 docker-inside-0.3.9/docker_inside.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      353 2018-05-13 09:54:08.000000 docker-inside-0.3.9/docker_inside.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      394 2018-05-13 09:54:08.000000 docker-inside-0.3.9/docker_inside.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-05-13 09:54:08.000000 docker-inside-0.3.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2018-05-13 09:52:46.000000 docker-inside-0.3.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5024 2018-05-13 09:54:08.000000 docker-inside-0.3.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-13 09:54:08.000000 docker-inside-0.3.9/dockerinside/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6725 2018-05-13 09:52:46.000000 docker-inside-0.3.9/dockerinside/dockerutils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2018-05-13 09:52:46.000000 docker-inside-0.3.9/dockerinside/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17644 2018-05-13 09:52:46.000000 docker-inside-0.3.9/dockerinside/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-13 09:54:08.000000 docker-inside-0.3.9/dockerinside/setup/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2018-05-13 09:52:46.000000 docker-inside-0.3.9/dockerinside/setup/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4458 2018-05-13 09:52:46.000000 docker-inside-0.3.9/dockerinside/setup/__init__.py
```

### Comparing `docker-inside-0.3.8/README.md` & `docker-inside-0.3.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Docker Inside
 
-[![Build Status](https://travis-ci.org/boon-code/docker-inside.svg?branch=release%2F0.3.0)](https://travis-ci.org/boon-code/docker-inside)
+[![Build Status](https://travis-ci.org/boon-code/docker-inside.svg)](https://travis-ci.org/boon-code/docker-inside)
+[![PyPI](https://img.shields.io/pypi/v/docker-inside.svg)](https://pypi.python.org/pypi/docker-inside)
 
 `dockerinside` is a python package that shall simplify running docker images as the current user
 similar to the way *Jenkins* awesome ``docker.inside()`` works.
 There are two main use-cases:
 
 - You want to easily share access between a container and your environment without having to
   manually modify the user id and group id of the files created by the running container.
```

### Comparing `docker-inside-0.3.8/setup.py` & `docker-inside-0.3.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import datetime
 
 YEAR = datetime.date.today().year
 
 __author__ = "Manuel Huber"
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 __license__ = "MIT"
 __copyright__ = u'%s, Manuel Huber' % YEAR
 
 
 setup(
     name='docker-inside',
     version=__version__,
```

### Comparing `docker-inside-0.3.8/docker_inside.egg-info/PKG-INFO` & `docker-inside-0.3.9/docker_inside.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 1.1
 Name: docker-inside
-Version: 0.3.8
+Version: 0.3.9
 Summary: Run a docker container with you workspace and user
 Home-page: https://github.com/boon-code/docker-inside
 Author: Manuel Huber
 Author-email: Manuel.h87@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: Docker Inside
         =============
         
-        |Build Status|
+        |Build Status| |PyPI|
         
         ``dockerinside`` is a python package that shall simplify running docker
         images as the current user similar to the way *Jenkins* awesome
         ``docker.inside()`` works. There are two main use-cases:
         
         -  You want to easily share access between a container and your
            environment without having to manually modify the user id and group
@@ -112,15 +111,17 @@
         
         Please let me know I you need support for more options from original
         ``docker run`` command or have any other suggestions how to improve this
         package. Please also let me know if your Docker image is failing using
         this package and I will see if I can fix the issue. Adding users and
         groups is unfortunately quite different among distributions.
         
-        .. |Build Status| image:: https://travis-ci.org/boon-code/docker-inside.svg?branch=release%2F0.3.0
+        .. |Build Status| image:: https://travis-ci.org/boon-code/docker-inside.svg
            :target: https://travis-ci.org/boon-code/docker-inside
+        .. |PyPI| image:: https://img.shields.io/pypi/v/docker-inside.svg
+           :target: https://pypi.python.org/pypi/docker-inside
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Systems Administration
```

### Comparing `docker-inside-0.3.8/PKG-INFO` & `docker-inside-0.3.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 1.1
 Name: docker-inside
-Version: 0.3.8
+Version: 0.3.9
 Summary: Run a docker container with you workspace and user
 Home-page: https://github.com/boon-code/docker-inside
 Author: Manuel Huber
 Author-email: Manuel.h87@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: Docker Inside
         =============
         
-        |Build Status|
+        |Build Status| |PyPI|
         
         ``dockerinside`` is a python package that shall simplify running docker
         images as the current user similar to the way *Jenkins* awesome
         ``docker.inside()`` works. There are two main use-cases:
         
         -  You want to easily share access between a container and your
            environment without having to manually modify the user id and group
@@ -112,15 +111,17 @@
         
         Please let me know I you need support for more options from original
         ``docker run`` command or have any other suggestions how to improve this
         package. Please also let me know if your Docker image is failing using
         this package and I will see if I can fix the issue. Adding users and
         groups is unfortunately quite different among distributions.
         
-        .. |Build Status| image:: https://travis-ci.org/boon-code/docker-inside.svg?branch=release%2F0.3.0
+        .. |Build Status| image:: https://travis-ci.org/boon-code/docker-inside.svg
            :target: https://travis-ci.org/boon-code/docker-inside
+        .. |PyPI| image:: https://img.shields.io/pypi/v/docker-inside.svg
+           :target: https://pypi.python.org/pypi/docker-inside
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Systems Administration
```

### Comparing `docker-inside-0.3.8/dockerinside/dockerutils.py` & `docker-inside-0.3.9/dockerinside/dockerutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,29 @@
         return int(v[0]), default_protocol
 
 
 def normalize_port(port_spec, **kwargs):
     return "{0}/{1}".format(*split_port_normalized(port_spec, **kwargs))
 
 
+def normalize_volume_spec(spec):
+    mode = 'rw'
+    tmp = spec.split(":", 2)
+    if len(tmp) == 3:
+        pass
+    elif len(tmp) == 2:
+        tmp.append(mode)
+    elif len(tmp) == 1:
+        tmp.append(tmp[0])
+        tmp.append(mode)
+    else:
+        raise ValueError("Wrong volume spec: '{0}".format(i))
+    return tmp
+
+
 def port_list_to_dict(port_list):
     if port_list is None:
         port_list = []
     for i in port_list:
         tmp = i.split(":", 2)
         if len(tmp) == 3:
             host_map = (tmp[0], split_port_normalized(tmp[1])[0])
@@ -190,25 +205,16 @@
         if status not in allowed_states:
             raise InvalidContainerState(cname, status)
 
     @staticmethod
     def volume_args_to_dict(args):
         d = dict()
         for i in args:
-            mode = 'rw'
-            tmp = i.split(":", 2)
-            if len(tmp) == 3:
-                mode = tmp[2]
-            elif len(tmp) == 2:
-                pass
-            elif len(tmp) == 1:
-                tmp.append(tmp[0])
-            else:
-                raise ValueError("Wrong volume spec: '{0}".format(i))
-            d[tmp[0]] = dict(bind=tmp[1], mode=mode)
+            tmp = normalize_volume_spec(i)
+            d[tmp[0]] = dict(bind=tmp[1], mode=tmp[2])
         return d
 
     def __init__(self, log, env=None):
         self._log = log
         self._env = env
         self._dc = docker.from_env(environment=env)
```

### Comparing `docker-inside-0.3.8/dockerinside/__init__.py` & `docker-inside-0.3.9/dockerinside/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,16 +236,19 @@
                             help="Set environment variables (default [])")
         parser.add_argument('-p', '--publish',
                             dest='ports',
                             action='append',
                             help="Publish a container's port(s) to the host ([ip:]hostp:contp)")
         parser.add_argument('--shm-size',
                             help="Size of /dev/shm, default value is 64MB")
-        parser.add_argument('-w', '--workdir',
-                            help="Working directory inside the container")
+        group = parser.add_mutually_exclusive_group(required=False)
+        group.add_argument('-w', '--workdir',
+                           help="Working directory inside the container")
+        group.add_argument('-W', '--mount-workdir',
+                           help="Mount and set working directory inside the container (volume spec)")
 
     @classmethod
     def _parse_args(cls, argv):
         parser = argparse.ArgumentParser()
         loglevel_group = parser.add_mutually_exclusive_group()
         loglevel_group.add_argument('--verbose',
                                     dest='loglevel',
@@ -391,14 +394,23 @@
                 }
             })
         script_pack = dockerutils.tar_pack(pack_conf)
         ports = dict(dockerutils.port_list_to_dict(self._args.ports))
         env = self._prepare_environment(image_info)
         cmd = self._prepare_command(image_info)
         volumes = dict(self.volume_args_to_dict(self._args.volumes))
+        workdir = self._args.workdir
+        if self._args.mount_workdir:
+            wd_spec = dockerutils.normalize_volume_spec(self._args.mount_workdir)
+            self._log.debug("Mount and set workdir {1} (volume spec: {0}:{1}:{2})".format(*wd_spec))
+            volumes[wd_spec[0]] = {
+                "bind": wd_spec[1],
+                "mode": wd_spec[2]
+            }
+            workdir = wd_spec[1]
         if self._args.gui:
             if os.path.exists(self.X11_SOCKET):
                 self._log.debug("Mount X11 unix socket")
                 volumes[self.X11_SOCKET] = {
                     "bind": self.X11_SOCKET,
                     "mode": 'rw'
                 }
@@ -424,15 +436,15 @@
             environment=env,
             entrypoint=entrypoint,
             name=self._args.name,
             cap_add=self._args.cap_add,
             cap_drop=self._args.cap_drop,
             devices=self._args.devices,
             ports=ports,
-            working_dir=self._args.workdir,
+            working_dir=workdir,
             shm_size=self._args.shm_size,
             tty=True,
             stdin_open=True,
             init=self._args.init,
         )
         if self._args.switch_root:
             creation_kwargs['user'] = "0"
```

### Comparing `docker-inside-0.3.8/dockerinside/setup/__init__.py` & `docker-inside-0.3.9/dockerinside/setup/__init__.py`

 * *Files identical despite different names*

