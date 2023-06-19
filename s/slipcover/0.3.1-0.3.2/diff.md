# Comparing `tmp/slipcover-0.3.1.tar.gz` & `tmp/slipcover-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slipcover-0.3.1.tar", last modified: Tue Mar 21 18:04:45 2023, max compression
+gzip compressed data, was "slipcover-0.3.2.tar", last modified: Mon Jun 19 16:36:45 2023, max compression
```

## Comparing `slipcover-0.3.1.tar` & `slipcover-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-21 18:04:45.992231 slipcover-0.3.1/
--rw-r--r--   0 runner     (501) staff       (20)    11358 2023-03-21 18:04:10.000000 slipcover-0.3.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       87 2023-03-21 18:04:10.000000 slipcover-0.3.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     9697 2023-03-21 18:04:45.991740 slipcover-0.3.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     7557 2023-03-21 18:04:10.000000 slipcover-0.3.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-03-21 18:04:45.992371 slipcover-0.3.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3534 2023-03-21 18:04:10.000000 slipcover-0.3.1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-21 18:04:45.985441 slipcover-0.3.1/src/
--rw-r--r--   0 runner     (501) staff       (20)     6415 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/probe.cxx
--rw-r--r--   0 runner     (501) staff       (20)      865 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/pyptr.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-21 18:04:45.988613 slipcover-0.3.1/src/slipcover/
--rw-r--r--   0 runner     (501) staff       (20)      136 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/slipcover/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4543 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/slipcover/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     4870 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/slipcover/branch.py
--rw-r--r--   0 runner     (501) staff       (20)    25061 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/slipcover/bytecode.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/slipcover/fuzz.py
--rw-r--r--   0 runner     (501) staff       (20)     7734 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/slipcover/importer.py
--rw-r--r--   0 runner     (501) staff       (20)    20394 2023-03-21 18:04:10.000000 slipcover-0.3.1/src/slipcover/slipcover.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-21 18:04:45.991026 slipcover-0.3.1/src/slipcover.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     9697 2023-03-21 18:04:45.000000 slipcover-0.3.1/src/slipcover.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      425 2023-03-21 18:04:45.000000 slipcover-0.3.1/src/slipcover.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-03-21 18:04:45.000000 slipcover-0.3.1/src/slipcover.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-03-21 18:04:45.000000 slipcover-0.3.1/src/slipcover.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2023-03-21 18:04:45.000000 slipcover-0.3.1/src/slipcover.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-19 16:36:45.931268 slipcover-0.3.2/
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2023-06-19 16:36:21.000000 slipcover-0.3.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       87 2023-06-19 16:36:21.000000 slipcover-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    10244 2023-06-19 16:36:45.930624 slipcover-0.3.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     8040 2023-06-19 16:36:21.000000 slipcover-0.3.2/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-06-19 16:36:45.931395 slipcover-0.3.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3534 2023-06-19 16:36:21.000000 slipcover-0.3.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-19 16:36:45.923678 slipcover-0.3.2/src/
+-rw-r--r--   0 runner     (501) staff       (20)     6415 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/probe.cxx
+-rw-r--r--   0 runner     (501) staff       (20)      865 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/pyptr.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-19 16:36:45.927217 slipcover-0.3.2/src/slipcover/
+-rw-r--r--   0 runner     (501) staff       (20)      136 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/slipcover/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4786 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/slipcover/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4954 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/slipcover/branch.py
+-rw-r--r--   0 runner     (501) staff       (20)    25082 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/slipcover/bytecode.py
+-rw-r--r--   0 runner     (501) staff       (20)      437 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/slipcover/fuzz.py
+-rw-r--r--   0 runner     (501) staff       (20)     7727 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/slipcover/importer.py
+-rw-r--r--   0 runner     (501) staff       (20)    20620 2023-06-19 16:36:21.000000 slipcover-0.3.2/src/slipcover/slipcover.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-19 16:36:45.929778 slipcover-0.3.2/src/slipcover.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    10244 2023-06-19 16:36:45.000000 slipcover-0.3.2/src/slipcover.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      425 2023-06-19 16:36:45.000000 slipcover-0.3.2/src/slipcover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-19 16:36:45.000000 slipcover-0.3.2/src/slipcover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-06-19 16:36:45.000000 slipcover-0.3.2/src/slipcover.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2023-06-19 16:36:45.000000 slipcover-0.3.2/src/slipcover.egg-info/top_level.txt
```

### Comparing `slipcover-0.3.1/LICENSE` & `slipcover-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slipcover-0.3.1/PKG-INFO` & `slipcover-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,97 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 0.3.1
+Version: 0.3.2
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Description: ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
         
-        # Slipcover: Near Zero-Overhead Python Code Coverage
-        by [Juan Altmayer Pizzorno](https://www.linkedin.com/in/juan-altmayer-pizzorno/) and [Emery Berger](https://emeryberger.com)
+        # SlipCover: Near Zero-Overhead Python Code Coverage
+        by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
         at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
         
-        [![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v0.3.1/LICENSE)
+        [![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v0.3.2/LICENSE)
         [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
         [![Downloads](https://pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
         ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
         ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
         
         ## About Slipcover
-        Slipcover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
+        SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
         It tracks a Python program as it runs and reports on the parts that executed and
         those that didn't.
         That can help guide your testing (showing code that isn't being tested), debugging,
         [fuzzing](https://en.wikipedia.org/wiki/Fuzzing) or to find "dead" code.
         
         Past code coverage tools can make programs significantly slower;
         it is not uncommon for them to take twice as long to execute.
-        Slipcover aims to provide the same information with **near-zero overhead**, often 
+        SlipCover aims to provide the same information with **near-zero overhead**, often 
         almost as fast as running the original Python program.
         
         ### How it works
         Previous coverage tools like [Coverage.py](https://github.com/nedbat/coveragepy) rely on 
         [Python's tracing facilities](https://docs.python.org/3/library/sys.html?highlight=settrace#sys.settrace),
         which add significant overhead.
-        Instead, Slipcover uses just-in-time instrumentation and de-instrumentation.
-        When Slipcover gathers coverage information, it modifies the program's Python byte codes,
+        Instead, SlipCover uses just-in-time instrumentation and de-instrumentation.
+        When SlipCover gathers coverage information, it modifies the program's Python byte codes,
         inserting instructions that let it keep track the lines executed by the program.
-        As the program executes, Slipcover gradually removes instrumentation that
+        As the program executes, SlipCover gradually removes instrumentation that
         is no longer needed, allowing those parts to run at full speed.
-        Care is taken throughout Slipcover to keep things as efficient as possible.
+        Care is taken throughout SlipCover to keep things as efficient as possible.
         
         ### Performance
-        <img src="https://github.com/plasma-umass/slipcover/blob/v0.3.1/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-        <img src="https://github.com/plasma-umass/slipcover/blob/v0.3.1/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+        <img src="https://github.com/plasma-umass/slipcover/blob/v0.3.2/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+        <img src="https://github.com/plasma-umass/slipcover/blob/v0.3.2/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
         
-        The first image on the right shows Slipcover's [speedup](https://en.wikipedia.org/wiki/Speedup)
-        in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
+        [//]: # (CPython-range)
+        The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
+        ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
         [CPython 3.10.5](https://github.com/python/cpython).
         
         The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
         and [Flask](https://flask.palletsprojects.com/);
         "sudoku" runs [Peter Norvig's Sudoku solver](http://norvig.com/sudoku.html)
         while the others were derived from the 
         [Python Benchmark Suite](https://github.com/python/pyperformance).
         
         More "Python-intensive" programs such as sudoku and those from the benchmark
         suite (with a larger proportion of execution time spent in Python, rather than in native code)
         generate more tracing events, causing more overhead in Coverage.py.
-        While each program's structure can affect Slipcover's ability to de-instrument,
+        While each program's structure can affect SlipCover's ability to de-instrument,
         its running time stays relatively close to the original.
         
-        On [PyPy 3.9](https://pypy.org), the speedup is so high for some of the benchmarks
-        that we plot it in logarithmic scale (see the second image on the right).
+        [//]: # (PyPy-range)
+        On [PyPy 3.9](https://pypy.org), the speedup ranges from 2.1x to 104.9x.
+        Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
+        
+        In a proof-of-concept integration with a property-based testing package,
+        SlipCover sped up coverage-based testing 22x.
         
         ### Accuracy
-        We verified Slipcover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-        and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v0.3.1/tools/oracle.py) of our own that collects coverage using Python tracing.
-        We found Slipcover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
+        We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
+        and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v0.3.2/tools/oracle.py) of our own that collects coverage using Python tracing.
+        We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
         
         ## Getting started
-        Slipcover is available from [PyPI](https://pypi.org/project/slipcover).
+        SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
         You can install it like any other Python module with
         ```console
         pip3 install slipcover
         ```
         
         You could then run your Python script with:
         ```console
         python3 -m slipcover myscript.py
         ```
         
         ### Using it with a test harness
-        Slipcover can also execute a Python module, as in:
+        SlipCover can also execute a Python module, as in:
         ```console
         python3 -m slipcover -m pytest -x -v
         ```
         which starts `pytest`, passing it any options (`-x -v` in this example)
         after the module name.
         No plug-in is required for pytest.
         
@@ -125,18 +130,21 @@
         its `box.py` and `image.py` components.
         
         ## Platforms
         Our GitHub workflows run the automated test suite on Linux, MacOS and Windows, but
         really it should work anywhere where CPython/PyPy does.
         
         ## Contributing
-        Slipcover is alpha software, and under active development.
+        SlipCover is alpha software, and under active development.
         Please feel free to [create a new issue](https://github.com/jaltmayerpizzorno/slipcover/issues/new)
         with any suggestions or issues you may encounter.
         
+        ## Technical Information
+        For more details about how SlipCover works please see the following paper, accepted to appear at [ISSTA'23](https://conf.researchr.org/home/issta-2023): [SlipCover: Near Zero-Overhead Code Coverage for Python](https://arxiv.org/pdf/2305.02886).
+        
         # Acknowledgements
         
         Logo design by [Sophia Berger](https://www.linkedin.com/in/sophia-berger/).
         
         This material is based upon work supported by the National Science
         Foundation under Grant No. 1955610. Any opinions, findings, and
         conclusions or recommendations expressed in this material are those of
```

### Comparing `slipcover-0.3.1/README.md` & `slipcover-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,89 @@
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
-# Slipcover: Near Zero-Overhead Python Code Coverage
-by [Juan Altmayer Pizzorno](https://www.linkedin.com/in/juan-altmayer-pizzorno/) and [Emery Berger](https://emeryberger.com)
+# SlipCover: Near Zero-Overhead Python Code Coverage
+by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
-Slipcover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
+SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
 It tracks a Python program as it runs and reports on the parts that executed and
 those that didn't.
 That can help guide your testing (showing code that isn't being tested), debugging,
 [fuzzing](https://en.wikipedia.org/wiki/Fuzzing) or to find "dead" code.
 
 Past code coverage tools can make programs significantly slower;
 it is not uncommon for them to take twice as long to execute.
-Slipcover aims to provide the same information with **near-zero overhead**, often 
+SlipCover aims to provide the same information with **near-zero overhead**, often 
 almost as fast as running the original Python program.
 
 ### How it works
 Previous coverage tools like [Coverage.py](https://github.com/nedbat/coveragepy) rely on 
 [Python's tracing facilities](https://docs.python.org/3/library/sys.html?highlight=settrace#sys.settrace),
 which add significant overhead.
-Instead, Slipcover uses just-in-time instrumentation and de-instrumentation.
-When Slipcover gathers coverage information, it modifies the program's Python byte codes,
+Instead, SlipCover uses just-in-time instrumentation and de-instrumentation.
+When SlipCover gathers coverage information, it modifies the program's Python byte codes,
 inserting instructions that let it keep track the lines executed by the program.
-As the program executes, Slipcover gradually removes instrumentation that
+As the program executes, SlipCover gradually removes instrumentation that
 is no longer needed, allowing those parts to run at full speed.
-Care is taken throughout Slipcover to keep things as efficient as possible.
+Care is taken throughout SlipCover to keep things as efficient as possible.
 
 ### Performance
 <img src="benchmarks/cpython.png?raw=True" align="right" width="65%"/>
 <img src="benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
-The first image on the right shows Slipcover's [speedup](https://en.wikipedia.org/wiki/Speedup)
-in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
+[//]: # (CPython-range)
+The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
+ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
 and [Flask](https://flask.palletsprojects.com/);
 "sudoku" runs [Peter Norvig's Sudoku solver](http://norvig.com/sudoku.html)
 while the others were derived from the 
 [Python Benchmark Suite](https://github.com/python/pyperformance).
 
 More "Python-intensive" programs such as sudoku and those from the benchmark
 suite (with a larger proportion of execution time spent in Python, rather than in native code)
 generate more tracing events, causing more overhead in Coverage.py.
-While each program's structure can affect Slipcover's ability to de-instrument,
+While each program's structure can affect SlipCover's ability to de-instrument,
 its running time stays relatively close to the original.
 
-On [PyPy 3.9](https://pypy.org), the speedup is so high for some of the benchmarks
-that we plot it in logarithmic scale (see the second image on the right).
+[//]: # (PyPy-range)
+On [PyPy 3.9](https://pypy.org), the speedup ranges from 2.1x to 104.9x.
+Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
+
+In a proof-of-concept integration with a property-based testing package,
+SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
-We verified Slipcover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
+We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
 and against a [simple script](tools/oracle.py) of our own that collects coverage using Python tracing.
-We found Slipcover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
+We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
-Slipcover is available from [PyPI](https://pypi.org/project/slipcover).
+SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
 ```
 
 You could then run your Python script with:
 ```console
 python3 -m slipcover myscript.py
 ```
 
 ### Using it with a test harness
-Slipcover can also execute a Python module, as in:
+SlipCover can also execute a Python module, as in:
 ```console
 python3 -m slipcover -m pytest -x -v
 ```
 which starts `pytest`, passing it any options (`-x -v` in this example)
 after the module name.
 No plug-in is required for pytest.
 
@@ -117,18 +122,21 @@
 its `box.py` and `image.py` components.
 
 ## Platforms
 Our GitHub workflows run the automated test suite on Linux, MacOS and Windows, but
 really it should work anywhere where CPython/PyPy does.
 
 ## Contributing
-Slipcover is alpha software, and under active development.
+SlipCover is alpha software, and under active development.
 Please feel free to [create a new issue](https://github.com/jaltmayerpizzorno/slipcover/issues/new)
 with any suggestions or issues you may encounter.
 
+## Technical Information
+For more details about how SlipCover works please see the following paper, accepted to appear at [ISSTA'23](https://conf.researchr.org/home/issta-2023): [SlipCover: Near Zero-Overhead Code Coverage for Python](https://arxiv.org/pdf/2305.02886).
+
 # Acknowledgements
 
 Logo design by [Sophia Berger](https://www.linkedin.com/in/sophia-berger/).
 
 This material is based upon work supported by the National Science
 Foundation under Grant No. 1955610. Any opinions, findings, and
 conclusions or recommendations expressed in this material are those of
```

### Comparing `slipcover-0.3.1/setup.py` & `slipcover-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `slipcover-0.3.1/src/probe.cxx` & `slipcover-0.3.2/src/probe.cxx`

 * *Files identical despite different names*

### Comparing `slipcover-0.3.1/src/pyptr.h` & `slipcover-0.3.2/src/pyptr.h`

 * *Files identical despite different names*

### Comparing `slipcover-0.3.1/src/slipcover/__main__.py` & `slipcover-0.3.2/src/slipcover/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,19 @@
 ap.add_argument('--omit', help="specify file(s) to omit")
 ap.add_argument('--immediate', action='store_true',
                 help=(argparse.SUPPRESS if platform.python_implementation() == "PyPy" else "request immediate de-instrumentation"))
 ap.add_argument('--skip-covered', action='store_true', help="omit fully covered files (from text, non-JSON output)")
 ap.add_argument('--fail-under', type=float, default=0, help="fail execution with RC 2 if the overall coverage lays lower than this")
 ap.add_argument('--threshold', type=int, default=50, metavar="T",
                 help="threshold for de-instrumentation (if not immediate)")
+ap.add_argument('--missing-width', type=int, default=80, metavar="WIDTH", help="maximum width for `missing' column")
 
 # intended for slipcover development only
 ap.add_argument('--silent', action='store_true', help=argparse.SUPPRESS)
+ap.add_argument('--dis', action='store_true', help=argparse.SUPPRESS)
 ap.add_argument('--stats', action='store_true', help=argparse.SUPPRESS)
 ap.add_argument('--debug', action='store_true', help=argparse.SUPPRESS)
 ap.add_argument('--dont-wrap-pytest', action='store_true', help=argparse.SUPPRESS)
 
 g = ap.add_mutually_exclusive_group(required=True)
 g.add_argument('-m', dest='module', nargs=1, help="run given module as __main__")
 g.add_argument('script', nargs='?', type=Path, help="the script to run")
@@ -64,29 +66,29 @@
 if args.omit:
     for o in args.omit.split(','):
         file_matcher.addOmit(o)
 
 
 sci = sc.Slipcover(collect_stats=args.stats, immediate=args.immediate,
                    d_miss_threshold=args.threshold, branch=args.branch,
-                   skip_covered=args.skip_covered)
+                   skip_covered=args.skip_covered, disassemble=args.dis)
 
 
 if not args.dont_wrap_pytest:
     sc.wrap_pytest(sci, file_matcher)
 
 
 
 def print_coverage(outfile):
     if args.json:
         import json
         print(json.dumps(sci.get_coverage(), indent=(4 if args.pretty_print else None)),
               file=outfile)
     else:
-        sci.print_coverage(outfile=outfile)
+        sci.print_coverage(missing_width=args.missing_width, outfile=outfile)
 
 
 def sci_atexit():
     if args.out:
         with open(args.out, "w") as outfile:
             print_coverage(outfile)
     else:
```

### Comparing `slipcover-0.3.1/src/slipcover/branch.py` & `slipcover-0.3.2/src/slipcover/branch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import ast
 import sys
 
 BRANCH_NAME = "_slipcover_branches"
+PYTHON_VERSION = sys.version_info[0:2]
 
 def preinstrument(tree: ast.AST) -> ast.AST:
     """Prepares an AST for Slipcover instrumentation, inserting assignments indicating where branches happen."""
 
     class SlipcoverTransformer(ast.NodeTransformer):
         def __init__(self):
             pass
 
         def _mark_branch(self, from_line: int, to_line: int) -> ast.AST:
             mark = ast.Assign([ast.Name(BRANCH_NAME, ast.Store())],
                                ast.Tuple([ast.Constant(from_line), ast.Constant(to_line)], ast.Load()))
 
             for node in ast.walk(mark):
-                node.lineno = 0 # we ignore line 0, so this avoids generating extra line probes
+                # we ignore line 0, so this avoids generating extra line probes
+                node.lineno = 0 if PYTHON_VERSION >= (3,11) else from_line
 
             return [mark]
 
         def visit_FunctionDef(self, node: ast.AST) -> ast.AST:
             # Mark BRANCH_NAME global, so that our assignment are easier to find (only STORE_NAME/STORE_GLOBAL,
             # but not STORE_FAST, etc.)
             has_docstring = ast.get_docstring(node, clean=False) is not None
@@ -50,31 +52,31 @@
 
         def visit_AsyncFor(self, node: ast.AsyncFor) -> ast.AsyncFor:
             return self._mark_branches(node)
 
         def visit_While(self, node: ast.While) -> ast.While:
             return self._mark_branches(node)
 
-        if sys.version_info[0:2] >= (3,10): # new in Python 3.10
+        if PYTHON_VERSION >= (3,10): # new in Python 3.10
             def visit_Match(self, node: ast.Match) -> ast.Match:
                 for case in node.cases:
                     case.body = self._mark_branch(node.lineno, case.body[0].lineno) + case.body
 
                 has_wildcard = isinstance(node.cases[-1].pattern, ast.MatchAs) and \
-                               node.cases[-1].pattern.pattern == None
+                               node.cases[-1].pattern.pattern is None
 
                 if not has_wildcard:
                     to_line = node.next_node.lineno if node.next_node else 0 # exit
                     node.cases.append(ast.match_case(ast.MatchAs(),
                                                      body=self._mark_branch(node.lineno, to_line)))
 
                 super().generic_visit(node)
                 return node
 
-    if sys.version_info[0:2] >= (3,10):
+    if PYTHON_VERSION >= (3,10):
         def is_Match(node: ast.AST) -> bool:
             return isinstance(node, ast.Match)
     else:
         def is_Match(node: ast.AST) -> bool:
             return False
 
     # Compute the "next" statement in case a branch flows control out of a node.
```

### Comparing `slipcover-0.3.1/src/slipcover/bytecode.py` & `slipcover-0.3.2/src/slipcover/bytecode.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,14 +572,16 @@
                 op_offset, op_len, op, op_arg = next(it)
                 while op == op_LOAD_CONST:
                     f_args.append(op_arg)
                     op_offset, op_len, op, op_arg = next(it)
 
                 return f_args
 
+        return None
+
 
     def disable_inserted_function(self, offset):
         """Disables an inserted function at a given offset."""
         assert not self.finished
 
         if self.patch is None:
             self.patch = bytearray(self.orig_code.co_code)
```

### Comparing `slipcover-0.3.1/src/slipcover/importer.py` & `slipcover-0.3.2/src/slipcover/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,24 +170,24 @@
         if 'exec' in f.__code__.co_names:
             ed = bc.Editor(f.__code__)
             wrapper_index = ed.add_const(exec_wrapper)
             ed.replace_global_with_const('exec', wrapper_index)
             f.__code__ = ed.finish()
 
     if sci.branch:
-        from inspect import signature
+        import inspect
 
         expected_sigs = {
             'rewrite_asserts': ['mod', 'source', 'module_path', 'config'],
             '_read_pyc': ['source', 'pyc', 'trace'],
             '_write_pyc': ['state', 'co', 'source_stat', 'pyc']
         }
 
         for fun, expected in expected_sigs.items():
-            sig = signature(pyrewrite.__dict__[fun])
+            sig = inspect.signature(pyrewrite.__dict__[fun])
             if list(sig.parameters) != expected:
                 import warnings
                 warnings.warn(f"Unable to activate pytest branch coverage: unexpected {fun} signature {str(sig)}"
                               +"; please open an issue at https://github.com/plasma-umass/slipcover .",
                               RuntimeWarning)
                 return
```

### Comparing `slipcover-0.3.1/src/slipcover/slipcover.py` & `slipcover-0.3.2/src/slipcover/slipcover.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from collections import defaultdict, Counter
 import threading
 from . import probe
 from . import bytecode as bc
 from . import branch as br
 from pathlib import Path
 
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 
 # FIXME provide __all__
 
 # Counter.total() is new in 3.10
 if sys.version_info[0:2] < (3,10):
     def counter_total(self: Counter) -> int:
         return sum([self[n] for n in self])
@@ -31,20 +31,22 @@
             return str(f.relative_to(self.cwd))
         except ValueError:
             return path 
 
 
 class Slipcover:
     def __init__(self, collect_stats: bool = False, immediate: bool = False,
-                 d_miss_threshold: int = 50, branch: bool = False, skip_covered: bool = False):
+                 d_miss_threshold: int = 50, branch: bool = False, skip_covered: bool = False,
+                 disassemble: bool = False):
         self.collect_stats = collect_stats
         self.immediate = immediate
         self.d_miss_threshold = d_miss_threshold
         self.branch = branch
         self.skip_covered = skip_covered
+        self.disassemble = disassemble
 
         # mutex protecting this state
         self.lock = threading.RLock()
 
         # maps to guide CodeType replacements
         self.replace_map: Dict[types.CodeType, types.CodeType] = dict()
         self.instrumented: Dict[str, set] = defaultdict(set)
@@ -147,14 +149,17 @@
 
                 delta += ed.insert_function_call(begin_off+delta, probe_signal_index, (branch_index,),
                                                  repl_length = end_off-begin_off)
 
         ed.add_const('__slipcover__')  # mark instrumented
         new_code = ed.finish()
 
+        if self.disassemble:
+            dis.dis(new_code)
+
         if self.collect_stats:
             self.all_probes.extend(probes)
 
         if self.immediate:
             for tr, off in zip(probes, ed.get_inserts()):
                 probe.set_immediate(tr, new_code.co_code, off)
         else:
@@ -368,15 +373,15 @@
 
             while missing_branches:
                 yield format_branch(missing_branches.pop(0))
 
         return ", ".join(find_ranges())
 
 
-    def print_coverage(self, outfile=sys.stdout) -> None:
+    def print_coverage(self, outfile=sys.stdout, *, missing_width=None) -> None:
         cov = self.get_coverage()
 
         from tabulate import tabulate
 
         def table(files):
             for f, f_info in sorted(files.items()):
                 exec_l = len(f_info['executed_lines'])
@@ -394,18 +399,17 @@
                 yield [f, exec_l+miss_l, miss_l,
                        *([exec_b+miss_b, miss_b] if self.branch else []),
                        round(pct),
                        Slipcover.format_missing(f_info['missing_lines'], f_info['executed_lines'],
                                                 f_info['missing_branches'] if 'missing_branches' in f_info else [])]
 
         print("", file=outfile)
-        print(tabulate(table(cov['files']),
-              headers=["File", "#lines", "#l.miss",
-                       *(["#br.", "#br.miss"] if self.branch else []),
-                       "Cover%", "Missing"]), file=outfile)
+        headers = ["File", "#lines", "#l.miss", *(["#br.", "#br.miss"] if self.branch else []), "Cover%", "Missing"]
+        maxcolwidths = [None] * (len(headers)-1) + [missing_width]
+        print(tabulate(table(cov['files']), headers=headers, maxcolwidths=maxcolwidths), file=outfile)
 
         def stats_table(files):
             for f, f_info in sorted(files.items()):
                 stats = f_info['stats']
 
                 yield (f, stats['d_misses_pct'], stats['u_misses_pct'],
                        " ".join(stats['top_d_misses'][:4]),
```

### Comparing `slipcover-0.3.1/src/slipcover.egg-info/PKG-INFO` & `slipcover-0.3.2/src/slipcover.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,97 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 0.3.1
+Version: 0.3.2
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Description: ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
         
-        # Slipcover: Near Zero-Overhead Python Code Coverage
-        by [Juan Altmayer Pizzorno](https://www.linkedin.com/in/juan-altmayer-pizzorno/) and [Emery Berger](https://emeryberger.com)
+        # SlipCover: Near Zero-Overhead Python Code Coverage
+        by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
         at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
         
-        [![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v0.3.1/LICENSE)
+        [![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v0.3.2/LICENSE)
         [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
         [![Downloads](https://pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
         ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
         ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
         
         ## About Slipcover
-        Slipcover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
+        SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
         It tracks a Python program as it runs and reports on the parts that executed and
         those that didn't.
         That can help guide your testing (showing code that isn't being tested), debugging,
         [fuzzing](https://en.wikipedia.org/wiki/Fuzzing) or to find "dead" code.
         
         Past code coverage tools can make programs significantly slower;
         it is not uncommon for them to take twice as long to execute.
-        Slipcover aims to provide the same information with **near-zero overhead**, often 
+        SlipCover aims to provide the same information with **near-zero overhead**, often 
         almost as fast as running the original Python program.
         
         ### How it works
         Previous coverage tools like [Coverage.py](https://github.com/nedbat/coveragepy) rely on 
         [Python's tracing facilities](https://docs.python.org/3/library/sys.html?highlight=settrace#sys.settrace),
         which add significant overhead.
-        Instead, Slipcover uses just-in-time instrumentation and de-instrumentation.
-        When Slipcover gathers coverage information, it modifies the program's Python byte codes,
+        Instead, SlipCover uses just-in-time instrumentation and de-instrumentation.
+        When SlipCover gathers coverage information, it modifies the program's Python byte codes,
         inserting instructions that let it keep track the lines executed by the program.
-        As the program executes, Slipcover gradually removes instrumentation that
+        As the program executes, SlipCover gradually removes instrumentation that
         is no longer needed, allowing those parts to run at full speed.
-        Care is taken throughout Slipcover to keep things as efficient as possible.
+        Care is taken throughout SlipCover to keep things as efficient as possible.
         
         ### Performance
-        <img src="https://github.com/plasma-umass/slipcover/blob/v0.3.1/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-        <img src="https://github.com/plasma-umass/slipcover/blob/v0.3.1/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+        <img src="https://github.com/plasma-umass/slipcover/blob/v0.3.2/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+        <img src="https://github.com/plasma-umass/slipcover/blob/v0.3.2/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
         
-        The first image on the right shows Slipcover's [speedup](https://en.wikipedia.org/wiki/Speedup)
-        in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
+        [//]: # (CPython-range)
+        The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
+        ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
         [CPython 3.10.5](https://github.com/python/cpython).
         
         The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
         and [Flask](https://flask.palletsprojects.com/);
         "sudoku" runs [Peter Norvig's Sudoku solver](http://norvig.com/sudoku.html)
         while the others were derived from the 
         [Python Benchmark Suite](https://github.com/python/pyperformance).
         
         More "Python-intensive" programs such as sudoku and those from the benchmark
         suite (with a larger proportion of execution time spent in Python, rather than in native code)
         generate more tracing events, causing more overhead in Coverage.py.
-        While each program's structure can affect Slipcover's ability to de-instrument,
+        While each program's structure can affect SlipCover's ability to de-instrument,
         its running time stays relatively close to the original.
         
-        On [PyPy 3.9](https://pypy.org), the speedup is so high for some of the benchmarks
-        that we plot it in logarithmic scale (see the second image on the right).
+        [//]: # (PyPy-range)
+        On [PyPy 3.9](https://pypy.org), the speedup ranges from 2.1x to 104.9x.
+        Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
+        
+        In a proof-of-concept integration with a property-based testing package,
+        SlipCover sped up coverage-based testing 22x.
         
         ### Accuracy
-        We verified Slipcover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-        and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v0.3.1/tools/oracle.py) of our own that collects coverage using Python tracing.
-        We found Slipcover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
+        We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
+        and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v0.3.2/tools/oracle.py) of our own that collects coverage using Python tracing.
+        We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
         
         ## Getting started
-        Slipcover is available from [PyPI](https://pypi.org/project/slipcover).
+        SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
         You can install it like any other Python module with
         ```console
         pip3 install slipcover
         ```
         
         You could then run your Python script with:
         ```console
         python3 -m slipcover myscript.py
         ```
         
         ### Using it with a test harness
-        Slipcover can also execute a Python module, as in:
+        SlipCover can also execute a Python module, as in:
         ```console
         python3 -m slipcover -m pytest -x -v
         ```
         which starts `pytest`, passing it any options (`-x -v` in this example)
         after the module name.
         No plug-in is required for pytest.
         
@@ -125,18 +130,21 @@
         its `box.py` and `image.py` components.
         
         ## Platforms
         Our GitHub workflows run the automated test suite on Linux, MacOS and Windows, but
         really it should work anywhere where CPython/PyPy does.
         
         ## Contributing
-        Slipcover is alpha software, and under active development.
+        SlipCover is alpha software, and under active development.
         Please feel free to [create a new issue](https://github.com/jaltmayerpizzorno/slipcover/issues/new)
         with any suggestions or issues you may encounter.
         
+        ## Technical Information
+        For more details about how SlipCover works please see the following paper, accepted to appear at [ISSTA'23](https://conf.researchr.org/home/issta-2023): [SlipCover: Near Zero-Overhead Code Coverage for Python](https://arxiv.org/pdf/2305.02886).
+        
         # Acknowledgements
         
         Logo design by [Sophia Berger](https://www.linkedin.com/in/sophia-berger/).
         
         This material is based upon work supported by the National Science
         Foundation under Grant No. 1955610. Any opinions, findings, and
         conclusions or recommendations expressed in this material are those of
```

