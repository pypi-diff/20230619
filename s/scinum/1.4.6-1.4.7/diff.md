# Comparing `tmp/scinum-1.4.6.tar.gz` & `tmp/scinum-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scinum-1.4.6.tar", last modified: Thu Mar 30 18:00:04 2023, max compression
+gzip compressed data, was "scinum-1.4.7.tar", last modified: Mon Jun 19 20:34:54 2023, max compression
```

## Comparing `scinum-1.4.6.tar` & `scinum-1.4.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:00:04.306569 scinum-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-30 18:00:03.000000 scinum-1.4.6/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-30 18:00:03.000000 scinum-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-30 18:00:03.000000 scinum-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-03-30 18:00:04.306569 scinum-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-03-30 18:00:03.000000 scinum-1.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 18:00:03.000000 scinum-1.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-30 18:00:03.000000 scinum-1.4.6/requirements_docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:00:04.306569 scinum-1.4.6/scinum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-03-30 18:00:04.000000 scinum-1.4.6/scinum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-30 18:00:04.000000 scinum-1.4.6/scinum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:00:04.000000 scinum-1.4.6/scinum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:00:04.000000 scinum-1.4.6/scinum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-30 18:00:04.000000 scinum-1.4.6/scinum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 18:00:04.000000 scinum-1.4.6/scinum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    89599 2023-03-30 18:00:03.000000 scinum-1.4.6/scinum.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 18:00:04.306569 scinum-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-30 18:00:03.000000 scinum-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:34:54.101146 scinum-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-19 20:34:52.000000 scinum-1.4.7/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-19 20:34:52.000000 scinum-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 20:34:52.000000 scinum-1.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-06-19 20:34:54.101146 scinum-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-06-19 20:34:52.000000 scinum-1.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:34:53.000000 scinum-1.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-19 20:34:53.000000 scinum-1.4.7/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:34:54.101146 scinum-1.4.7/scinum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-06-19 20:34:54.000000 scinum-1.4.7/scinum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 20:34:54.000000 scinum-1.4.7/scinum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:34:54.000000 scinum-1.4.7/scinum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:34:54.000000 scinum-1.4.7/scinum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-19 20:34:54.000000 scinum-1.4.7/scinum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 20:34:54.000000 scinum-1.4.7/scinum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    90458 2023-06-19 20:34:53.000000 scinum-1.4.7/scinum.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 20:34:54.101146 scinum-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-19 20:34:53.000000 scinum-1.4.7/setup.py
```

### Comparing `scinum-1.4.6/LICENSE` & `scinum-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scinum-1.4.6/PKG-INFO` & `scinum-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinum
-Version: 1.4.6
+Version: 1.4.7
 Summary: Scientific numbers with multiple uncertainties and correlation-aware, gaussian propagation and numpy
 Home-page: https://github.com/riga/scinum
 Author: Marcel Rieger
 Author-email: python-scinum@googlegroups.com
 License: BSD-3-Clause
 Keywords: scientific,numbers,error,systematics,propagation
 Platform: UNKNOWN
```

### Comparing `scinum-1.4.6/README.md` & `scinum-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `scinum-1.4.6/scinum.egg-info/PKG-INFO` & `scinum-1.4.7/scinum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinum
-Version: 1.4.6
+Version: 1.4.7
 Summary: Scientific numbers with multiple uncertainties and correlation-aware, gaussian propagation and numpy
 Home-page: https://github.com/riga/scinum
 Author: Marcel Rieger
 Author-email: python-scinum@googlegroups.com
 License: BSD-3-Clause
 Keywords: scientific,numbers,error,systematics,propagation
 Platform: UNKNOWN
```

### Comparing `scinum-1.4.6/scinum.py` & `scinum-1.4.7/scinum.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __author__ = "Marcel Rieger"
 __email__ = "python-scinum@googlegroups.com"
 __copyright__ = "Copyright 2017-2023, Marcel Rieger"
 __credits__ = ["Marcel Rieger"]
 __contact__ = "https://github.com/riga/scinum"
 __license__ = "BSD-3-Clause"
 __status__ = "Development"
-__version__ = "1.4.6"
+__version__ = "1.4.7"
 __all__ = [
     "Number", "Correlation", "DeferredResult", "Operation",
     "ops", "style_dict",
     "REL", "ABS", "NOMINAL", "UP", "DOWN", "N", "U", "D",
 ]
 
 
@@ -238,33 +238,40 @@
     When operations connect two number instances, their uncertainties are combined assuming there is
     no correlation. For correlation-aware operations, please refer to methods such as :py:meth:`add`
     or :py:meth:`mul` below. Examples:
 
     .. code-block:: python
 
         num = Number(5, 1)
-        print(num + 2)  # -> '7.0 +- 1.0'
-        print(num * 3)  # -> '15.0 +- 3.0'
+        print(num + 2)  # -> '7.0 +-1.0'
+        print(num * 3)  # -> '15.0 +-3.0'
 
         num2 = Number(2.5, 1.5)
-        print(num + num2)  # -> '7.5 +- 1.80277563773'
-        print(num * num2)  # -> '12.5 +- 7.90569415042'
+        print(num + num2)  # -> '7.5 +-1.80277563773'
+        print(num * num2)  # -> '12.5 +-7.90569415042'
 
         num.add(num2, rho=1)
-        print(num)  # -> '7.5 +- 2.5'
+        print(num)  # -> '7.5 +-2.5'
 
     See :py:meth:`str` for information on string formatting.
 
     .. py:classattribute:: default_format
 
         type: string
 
         The default format string (``"%s"``) that is used in :py:meth:`str()` when no format string
         was passed.
 
+    .. py:classattribute:: default_style
+
+        type: string
+
+        The default style name (``"plain"``) that is used in :py:meth:`str()` when no style argument
+        was passed.
+
     .. py:classattribute:: DEFAULT
 
         type: string
 
         Constant that denotes the default uncertainty (``"default"``).
 
     .. py:classattribute:: ALL
@@ -374,16 +381,17 @@
 
     # aliases
     N = NOMINAL
     U = UP
     D = DOWN
 
     default_format = "%s"
+    default_style = "plain"
 
-    def __init__(self, nominal=0.0, uncertainties=None, default_format=None):
+    def __init__(self, nominal=0.0, uncertainties=None, default_format=None, default_style=None):
         super(Number, self).__init__()
 
         # wrapped values
         self._nominal = None
         self._uncertainties = OrderedDict()
 
         # numpy settings
@@ -399,17 +407,21 @@
 
         # set initial values
         self.nominal = nominal
         if uncertainties is not None:
             self.uncertainties = uncertainties
 
         self.default_format = default_format
+        self.default_style = default_style
 
     def _init_kwargs(self):
-        return {"default_format": self.default_format}
+        return {
+            "default_format": self.default_format,
+            "default_style": self.default_style,
+        }
 
     @typed
     def nominal(self, nominal):
         # parser for the typed member holding the nominal value
         if isinstance(nominal, (int, float)):
             if self.uncertainties and is_numpy(list(self.uncertainties.values())[0][0]):
                 raise TypeError("cannot set nominal to plain value when uncertainties are arrays")
@@ -606,15 +618,15 @@
         self,
         format=None,
         combine_uncs=None,
         unit=None,
         scientific=False,
         si=False,
         labels=True,
-        style="plain",
+        style=None,
         styles=None,
         force_asymmetric=False,
         **kwargs  # noqa
     ):
         r"""
         Returns a readable string representiation of the number. *format* is used to format
         non-NumPy nominal and uncertainty values. It can be a string such as ``"%d"``, a function
@@ -627,46 +639,51 @@
         When *combine_uncs* is set, uncertainties are reduced via :py:meth:`combine_uncertaintes`.
         When *unit* is set, it is appended to the end of the string. When *scientific* is *True*,
         all values are represented by their scientific notation. When *scientific* is *False* and
         *si* is *True*, the appropriate SI prefix is used.
 
         *labels* controls whether uncertainty labels are shown in the string. When *True*,
         uncertainty names are used, but it can also be a list of labels whose order should match the
-        uncertainty dict traversal order. *style* can be ``"plain"``, ``"latex"``, or ``"root"``.
+        uncertainty dict traversal order. *style* can be ``"plain"``, ``"fancy"``, ``"latex"``, or
+        ``"root"``. When *None* (the default), :py:attr:`default_style` is used.
 
         *styles* can be a dict with fields ``"space"``, ``"label"``, ``"unit"``, ``"sym"``,
         ``"asym"``, ``"sci"`` to customize every aspect of the format style on top of
         :py:attr:`style_dict`. Unless *force_asymmetric* is *True*, an uncertainty is quoted
         symmetric if it yields identical values in both directions.
 
         Examples:
 
         .. code-block:: python
 
             n = Number(17.321, {"a": 1.158, "b": 0.453})
-            n.str()                    # -> '17.321 +- 1.158 (a) +- 0.453 (b)'
-            n.str("%.1f")              # -> '17.3 +- 1.2 (a) +- 0.5 (b)'
-            n.str("publication")       # -> '17.32 +- 1.16 (a) +- 0.45 (b)'
-            n.str("pdg")               # -> '17.3 +- 1.2 (a) +- 0.5 (b)'
+            n.str()                    # -> '17.321 +-1.158 (a) +-0.453 (b)'
+            n.str("%.1f")              # -> '17.3 +-1.2 (a) +-0.5 (b)'
+            n.str("publication")       # -> '17.32 +-1.16 (a) +-0.45 (b)'
+            n.str("pdg")               # -> '17.3 +-1.2 (a) +-0.5 (b)'
             n.str(combine_uncs="all")  # -> 'TODO'
 
             n = Number(8848, 10)
-            n.str(unit="m")                           # -> "8848.0 +- 10.0 m"
+            n.str(unit="m")                           # -> "8848.0 +-10.0 m"
             n.str(unit="m", force_asymmetric=True)    # -> "8848.0 +10.0-10.0 m"
-            n.str(unit="m", scientific=True)          # -> "8.848 +- 0.01 x 1E3 m"
-            n.str("%.2f", unit="m", scientific=True)  # -> "8.85 +- 0.01 x 1E3 m"
-            n.str(unit="m", si=True)                  # -> "8.848 +- 0.01 km"
-            n.str("%.2f", unit="m", si=True)          # -> "8.85 +- 0.01 km"
-            n.str(unit="m", style="latex")            # -> "8848.0 \pm 10.0\,m"
-            n.str(unit="m", style="latex", si=True)   # -> "8.848 \pm 0.01\,km"
-            n.str(unit="m", style="root")             # -> "8848.0 #pm 10.0 m"
-            n.str(unit="m", style="root", si=True)    # -> "8.848 #pm 0.01 km"
+            n.str(unit="m", scientific=True)          # -> "8.848 +-0.01 x 1E3 m"
+            n.str("%.2f", unit="m", scientific=True)  # -> "8.85 +-0.01 x 1E3 m"
+            n.str(unit="m", si=True)                  # -> "8.848 +-0.01 km"
+            n.str("%.2f", unit="m", si=True)          # -> "8.85 +-0.01 km"
+            n.str(style="fancy")                      # -> "8848.0 ±10.0"
+            n.str(unit="m", style="fancy")            # -> "8848.0 ±10.0 m"
+            n.str(unit="m", style="latex")            # -> "8848.0 \pm10.0\,m"
+            n.str(unit="m", style="latex", si=True)   # -> "8.848 \pm0.01\,km"
+            n.str(unit="m", style="root")             # -> "8848.0 #pm10.0 m"
+            n.str(unit="m", style="root", si=True)    # -> "8.848 #pm0.01 km"
         """
         if format is None:
             format = self.default_format or self.__class__.default_format
+        if style is None:
+            style = self.default_style or self.__class__.default_style
 
         # when uncertainties should be combined, create a new instance and forward to its formatting
         if combine_uncs:
             return self.combine_uncertaintes(combine=combine_uncs).str(
                 format=format,
                 unit=unit,
                 scientific=scientific,
@@ -730,15 +747,15 @@
 
             # start building the text
             text = fmt(nominal, **kwargs)
 
             # no uncertainties
             if len(names) == 0:
                 text += ending()
-                if style == "plain" and labels:
+                if style in ("plain", "fancy") and labels:
                     text += d["space"] + d["label"].format(label="no uncertainties")
 
             # one ore more uncertainties
             else:
                 # special case: only the default uncertainty
                 if len(names) == 1 and names[0] == self.DEFAULT:
                     labels = False
@@ -1236,22 +1253,22 @@
     uncertainty correlations when combined with an other :py:class:`Number`. Example:
 
     .. code-block:: python
 
         n = Number(2, 5)
 
         n * Correlation(1) * n
-        # -> '25.0 +- 20.0' (the default)
+        # -> '25.0 +-20.0' (the default)
 
         n * Correlation(0) * n
-        # -> '25.00 +- 14.14'
+        # -> '25.00 +-14.14'
 
         # note the multiplication n * c, which creates the DeferredResult
         n**(n * c)
-        # -> '3125.00 +- 11842.54'
+        # -> '3125.00 +-11842.54'
 
     .. py:attribute:: number
        type: Number
 
        The wrapped number object.
 
     .. py:attribute:: correlation
@@ -2606,48 +2623,56 @@
         value_node = y_map(value_node_items)
 
         return value_node
 
     return representer
 
 
-#: Dictionaly containing formatting styles for ``"plain"``, ``"latex"`` and ``"root"`` styles which
-#: are used in :py:meth:`Number.str`. Each style dictionary contains 6 fields: ``"space"``,
-#: ``"label"``, ``"unit"``, ``"sym"``, ``"asym"``, and ``"sci"``. As an example, the plain style is
-#: configured as
+#: Dictionaly containing formatting styles for ``"plain"``, ``"fancy"``, ``"latex"`` and ``"root"``
+#: styles which are used in :py:meth:`Number.str`. Each style dictionary contains 6 fields:
+#: ``"space"``, ``"label"``, ``"unit"``, ``"sym"``, ``"asym"``, and ``"sci"``. As an example, the
+#: plain style is configured as
 #:
 #: .. code-block:: python
 #:
 #:     {
 #:         "space": " ",
 #:         "label": "({label})",
 #:         "unit": " {unit}",
-#:         "sym": "+- {unc}",
+#:         "sym": "+-{unc}",
 #:         "asym": "+{up}-{down}",
 #:         "sci": "x 1E{mag}",
 #:     }
 style_dict = {
     "plain": {
         "space": " ",
         "label": "({label})",
         "unit": " {unit}",
-        "sym": "+- {unc}",
+        "sym": "+-{unc}",
+        "asym": "+{up}-{down}",
+        "sci": "x 1E{mag}",
+    },
+    "fancy": {
+        "space": " ",
+        "label": "({label})",
+        "unit": " {unit}",
+        "sym": "±{unc}",
         "asym": "+{up}-{down}",
         "sci": "x 1E{mag}",
     },
     "latex": {
         "space": r" ",
         "label": r"\left(\text{{{label}}}\right)",
         "unit": r"\,{unit}",
-        "sym": r"\pm {unc}",
+        "sym": r"\pm{unc}",
         "asym": r"\,^{{+{up}}}_{{-{down}}}",
         "sci": r"\times 10^{{{mag}}}",
     },
     "root": {
         "space": " ",
         "label": "#left({label}#right)",
         "unit": " {unit}",
-        "sym": "#pm {unc}",
+        "sym": "#pm{unc}",
         "asym": "^{{+{up}}}_{{-{down}}}",
         "sci": "#times 10^{{{mag}}}",
     },
 }
```

### Comparing `scinum-1.4.6/setup.py` & `scinum-1.4.7/setup.py`

 * *Files identical despite different names*

