# Comparing `tmp/bindlab-0.0.2.tar.gz` & `tmp/bindlab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bindlab-0.0.2.tar", last modified: Mon Jun 19 15:02:15 2023, max compression
+gzip compressed data, was "bindlab-0.0.3.tar", last modified: Mon Jun 19 15:33:54 2023, max compression
```

## Comparing `bindlab-0.0.2.tar` & `bindlab-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-19 15:02:15.632000 bindlab-0.0.2/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      255 2023-06-19 15:02:15.631758 bindlab-0.0.2/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      103 2023-04-22 17:21:31.000000 bindlab-0.0.2/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-19 15:02:15.631389 bindlab-0.0.2/bindlab.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      255 2023-06-19 15:02:15.000000 bindlab-0.0.2/bindlab.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      202 2023-06-19 15:02:15.000000 bindlab-0.0.2/bindlab.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-19 15:02:15.000000 bindlab-0.0.2/bindlab.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-19 15:02:15.000000 bindlab-0.0.2/bindlab.egg-info/not-zip-safe
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       20 2023-06-19 15:02:15.000000 bindlab-0.0.2/bindlab.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        4 2023-06-19 15:02:15.000000 bindlab-0.0.2/bindlab.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-19 15:02:15.632084 bindlab-0.0.2/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5738 2023-06-19 15:01:32.000000 bindlab-0.0.2/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-19 15:33:54.468256 bindlab-0.0.3/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      391 2023-06-19 15:33:54.467984 bindlab-0.0.3/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      103 2023-04-22 17:21:31.000000 bindlab-0.0.3/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-19 15:33:54.467094 bindlab-0.0.3/bindlab.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      391 2023-06-19 15:33:53.000000 bindlab-0.0.3/bindlab.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      218 2023-06-19 15:33:54.000000 bindlab-0.0.3/bindlab.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-19 15:33:53.000000 bindlab-0.0.3/bindlab.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-19 15:33:53.000000 bindlab-0.0.3/bindlab.egg-info/not-zip-safe
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       20 2023-06-19 15:33:54.000000 bindlab-0.0.3/bindlab.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        4 2023-06-19 15:33:54.000000 bindlab-0.0.3/bindlab.egg-info/top_level.txt
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-19 15:33:54.467408 bindlab-0.0.3/lab/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-06-19 15:30:31.000000 bindlab-0.0.3/lab/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-19 15:33:54.468367 bindlab-0.0.3/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5987 2023-06-19 15:31:05.000000 bindlab-0.0.3/setup.py
```

### Comparing `bindlab-0.0.2/setup.py` & `bindlab-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,22 +119,28 @@
             ["cmake", ext.sourcedir, *cmake_args], cwd=build_temp, check=True
         )
         subprocess.run(
             ["cmake", "--build", ".", *build_args], cwd=build_temp, check=True
         )
 
 
+directory = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="bindlab",
-    version="0.0.2",
+    version="0.0.3",
     author="Marco Salvalaggio",
     author_email="mar.salvalaggio@gmail.com",
     description="A test project using pybind11 and CMake",
-    long_description="",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    packages = ['lab'],
     ext_modules=[CMakeExtension("lab")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     extras_require={"test": ["pytest>=6.0"]},
     python_requires=">=3.7",
 )
```

