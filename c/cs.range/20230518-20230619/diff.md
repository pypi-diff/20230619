# Comparing `tmp/cs.range-20230518.tar.gz` & `tmp/cs.range-20230619.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.range-20230518.tar", last modified: Thu May 18 10:18:07 2023, max compression
+gzip compressed data, was "cs.range-20230619.tar", last modified: Mon Jun 19 03:48:01 2023, max compression
```

## Comparing `cs.range-20230518.tar` & `cs.range-20230619.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.383448 cs.range-20230518/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-05-18 10:17:48.000000 cs.range-20230518/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     2659 2023-05-18 10:18:07.383564 cs.range-20230518/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     6133 2023-05-18 10:17:50.000000 cs.range-20230518/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.379233 cs.range-20230518/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.379571 cs.range-20230518/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.381422 cs.range-20230518/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    16581 2023-05-18 10:17:34.000000 cs.range-20230518/lib/python/cs/range.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.383181 cs.range-20230518/lib/python/cs.range.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     2659 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       39 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     2853 2023-05-18 10:17:54.000000 cs.range-20230518/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      937 2023-05-18 10:18:07.384097 cs.range-20230518/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-05-18 10:17:50.000000 cs.range-20230518/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.028716 cs.range-20230619/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-19 03:47:45.000000 cs.range-20230619/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2875 2023-06-19 03:48:01.028853 cs.range-20230619/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6506 2023-06-19 03:47:46.000000 cs.range-20230619/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.023417 cs.range-20230619/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.023842 cs.range-20230619/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.026347 cs.range-20230619/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    18190 2023-06-19 03:46:43.000000 cs.range-20230619/lib/python/cs/range.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.028418 cs.range-20230619/lib/python/cs.range.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2875 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       39 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3069 2023-06-19 03:47:52.000000 cs.range-20230619/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)      937 2023-06-19 03:48:01.029580 cs.range-20230619/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-19 03:47:46.000000 cs.range-20230619/setup.py
```

### Comparing `cs.range-20230518/PKG-INFO` & `cs.range-20230619/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.range
-Version: 20230518
+Version: 20230619
 Summary: a Range class implementing compact integer ranges with a set-like API, and associated functions
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,16 +17,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 
-*Latest release 20230518*:
-Span,Range: new as_list() methods.
+*Latest release 20230619*:
+* Span: sanity check .start and .end.
+* Range.issubset: efficient comparison with another Range, also .issuperset.
 
 ## Function `overlap(span1, span2)`
 
 Return a list `[start,end]` denoting the overlap of two spans.
 
 Example:
 
@@ -67,14 +68,18 @@
     >>> list(spans([1,2,3,7,8,11,5]))
     [1:4, 7:9, 11:12, 5:6]
 
 # Release Log
 
 
 
+*Release 20230619*:
+* Span: sanity check .start and .end.
+* Range.issubset: efficient comparison with another Range, also .issuperset.
+
 *Release 20230518*:
 Span,Range: new as_list() methods.
 
 *Release 20190102*:
 Span: provide __len__.
 
 *Release 20171231*:
```

### Comparing `cs.range-20230518/README.md` & `cs.range-20230619/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 
-*Latest release 20230518*:
-Span,Range: new as_list() methods.
+*Latest release 20230619*:
+* Span: sanity check .start and .end.
+* Range.issubset: efficient comparison with another Range, also .issuperset.
 
 ## Function `overlap(span1, span2)`
 
 Return a list `[start,end]` denoting the overlap of two spans.
 
 Example:
 
@@ -38,22 +39,33 @@
 
 *Method `Range.__contains__(self, x)`*:
 Test `x` to see if it is wholly contained in this Range.
 
 `x` may be another `Range`, a `Span`, or a single `int` or an iterable
 yielding a pair of `int`s.
 
+Example:
+
+    >>> R = Range(4,7)
+    >>> R.add(11,15)
+    >>> (3,7) in R
+    False
+    >>> (4,7) in R
+    True
+    >>> (4,8) in R
+    False
+
 *Method `Range.__ge__(self, other)`*:
-Test that self is a superset of other.
+Test that `self` is a superset of `other`.
 
 *Method `Range.__iter__(self)`*:
 Yield all the elements.
 
 *Method `Range.__le__(self, other)`*:
-Test that self is a subset of other.
+Test that `self` is a subset of `other`.
 
 *Method `Range.__or__(self, other)`*:
 Return a new `Range` containing the elements of `self` and `other`.
 
 *Method `Range.__sub__(self, start, end=None)`*:
 Subtract `start`, or `start:end`, from the `Range`.
 
@@ -114,18 +126,18 @@
 Update the `Range`, keeping only elements
 found in both `self` and `other`.
 
 *Method `Range.isempty(self)`*:
 Test if the Range is empty.
 
 *Method `Range.issubset(self, other)`*:
-Test that self is a subset of other.
+Test that `self` is a subset of `other`.
 
 *Method `Range.issuperset(self, other)`*:
-Test that self is a superset of other.
+Test that `self` is a superset of `other`.
 
 *Method `Range.pop(self)`*:
 Remove and return an arbitrary element.
 Raise `KeyError` if the `Range` is empty.
 
 *Method `Range.remove(self, start, end=None)`*:
 Like `set.remove` but with an extended signature.
@@ -187,14 +199,18 @@
     >>> list(spans([1,2,3,7,8,11,5]))
     [1:4, 7:9, 11:12, 5:6]
 
 # Release Log
 
 
 
+*Release 20230619*:
+* Span: sanity check .start and .end.
+* Range.issubset: efficient comparison with another Range, also .issuperset.
+
 *Release 20230518*:
 Span,Range: new as_list() methods.
 
 *Release 20190102*:
 Span: provide __len__.
 
 *Release 20171231*:
```

### Comparing `cs.range-20230518/lib/python/cs/range.py` & `cs.range-20230619/lib/python/cs/range.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 
 '''
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 '''
 
 from __future__ import print_function
-import sys
+
 from bisect import bisect_left
 from collections import namedtuple
+import sys
+
 from cs.logutils import ifdebug
 from cs.seq import first
 
-__version__ = '20230518'
+__version__ = '20230619'
 
 DISTINFO = {
     'description':
     "a Range class implementing compact integer ranges with a set-like API,"
     " and associated functions",
     'keywords': ["python2", "python3"],
     'classifiers': [
@@ -77,38 +79,49 @@
   if prev is not None:
     yield Span(*prev)
 
 class Span(namedtuple('Span', 'start end')):
   ''' A namedtuple with `.start` and `.end` attributes.
   '''
 
+  def __new__(cls, start, end):
+    if not isinstance(start, int):
+      raise TypeError("start:%r must be an int" % (start,))
+    if not isinstance(end, int):
+      raise TypeError("end:%r must be an int" % (end,))
+    if start > end:
+      raise ValueError("start:%d > end:%d" % (start, end))
+    return super().__new__(cls, start, end)
+
   def __str__(self):
     return "%d:%d" % (self.start, self.end)
 
   __repr__ = __str__
 
   def __eq__(self, other):
+    # equal spans
     return self[0] == other[0] and self[1] == other[1]
 
   def __lt__(self, other):
-    return self[0] < other[0] or (self[0] == other[0] and self[1] < other[1])
+    return self[0] < other[0]
 
   def __len__(self):
     return self.end - self.start
 
   @property
   def size(self):
     ''' The `.size` of a `Span` is its length: `end - start`.
     '''
     return len(self)
 
   def as_list(self):
     ''' This `Span` as a 2 element `list`. '''
     return [self.start, self.end]
 
+# pylint: disable=too-many-public-methods,protected-access
 class Range(object):
   ''' A collection of `int`s that collates adjacent ints.
 
       The interface is as for a `set` with additional methods:
       * `spans()`: return an iterable of `Span`s, with `.start`
         included in each `Span` and `.end` just beyond
 
@@ -193,15 +206,15 @@
     self._check_spans()
 
   def _check_spans(self):
     ''' Sanity check the ._spans attribute.
         Raises TypeError or ValueError on failure.
     '''
     _spans = self._spans
-    if type(_spans) is not list:
+    if type(_spans) is not list:  # pylint: disable=unidiomatic-typecheck
       raise TypeError("._spans should be a list")
     ospan = None
     for span in _spans:
       if not isinstance(span, Span):
         raise TypeError(
             "._spans elements should be lists, found " + repr(span)
         )
@@ -241,61 +254,71 @@
   def start(self):
     ''' Return the start offset of the `Range`,
         the minimum `Span` .start or `0` if the `Range` is empty.
     '''
     spans = self._spans
     if len(spans) > 0:
       return spans[0].start
-    else:
-      return 0
+    return 0
 
   @property
   def end(self):
     ''' Return the end offset of the `Range`,
         the maximum `Span` .end or `0` if the `Range` is empty.
     '''
     spans = self._spans
     if len(spans) > 0:
       return spans[-1].end
-    else:
-      return 0
+    return 0
 
   def isempty(self):
     ''' Test if the Range is empty.
     '''
     return not self
 
   def __contains__(self, x):
     ''' Test `x` to see if it is wholly contained in this Range.
 
         `x` may be another `Range`, a `Span`, or a single `int` or an iterable
         yielding a pair of `int`s.
+
+        Example:
+
+            >>> R = Range(4,7)
+            >>> R.add(11,15)
+            >>> (3,7) in R
+            False
+            >>> (4,7) in R
+            True
+            >>> (4,8) in R
+            False
     '''
     if isinstance(x, Range):
       return self.issuperset(x)
     if isinstance(x, Span):
       start = x.start
       end = x.end
     elif isinstance(x, int):
       start, end = x, x + 1
     else:
-      start, end = list(x)
+      start, end = x
     _spans = self._spans
     ndx = bisect_left(_spans, Span(start, start))
     if ndx > 0 and _spans[ndx - 1].end > start:
       ndx -= 1
     elif ndx >= len(_spans):
       return False
     span = _spans[ndx]
     if start < span.start:
       return False
     if end > span.end:
       return False
     return True
 
+  # pylint: disable=unused-argument
   def span_position(self, start, end):
     ''' Somewhat like `bisect_left`, return indices `(i,j)`
         such that all spans with indices < `i`
         strictly preceed `start` amd all spans with indices > `j`
         strictly follow `end`.
     '''
     _spans = self._spans
@@ -343,28 +366,58 @@
         If `end` is omitted, use the maximum span in the Range.
     '''
     for inside, span in self.slices(start=start, end=end):
       if not inside:
         yield span
 
   def issubset(self, other):
-    ''' Test that self is a subset of other.
+    ''' Test that `self` is a subset of `other`.
     '''
-    # TODO: handle other Ranges specially
+    if isinstance(other, Range):
+      # ordered comparison of spans
+      ospans = iter(other._spans)
+      try:
+        ospan = next(ospans)
+      except StopIteration:
+        ospan = None
+      for span in self._spans:
+        assert span.start < span.end
+        # skip early other spans
+        while ospan is not None and span.start >= ospan.end:
+          try:
+            ospan = next(ospans)
+          except StopIteration:
+            ospan = None
+        if ospan is None:
+          # no other span we can be in
+          return False
+        assert span.start < ospan.end
+        if span.start < ospan.start:
+          # we have elements before the other span
+          return False
+        if span.end > ospan.end:
+          # we have elements beyond the other span
+          return False
+        # we are completely contained in the other span
+        # proceed to the next span
+      return True
+    # expensive iteration based comparison
     for x in self:
       if x not in other:
         return False
     return True
 
   __le__ = issubset
 
   def issuperset(self, other):
-    ''' Test that self is a superset of other.
+    ''' Test that `self` is a superset of `other`.
     '''
-    # TODO: handle ranges specially
+    if isinstance(other, Range):
+      return other.issubset(self)
+    # expensive iteration based comparison
     for x in other:
       if x not in self:
         return False
     return True
 
   __ge__ = issuperset
 
@@ -426,26 +479,22 @@
       if remove_mode and start < span.start:
         raise KeyError("span %s not entirely in Range" % (ospan,))
       if span.end > start:
         # this span should be considered
         if drop_from is None:
           drop_from = i
         # split span on cropping range
-        low_span = Span(span.start, start)
-        high_span = Span(end, span.end)
+        low_span = Span(span.start, start) if span.start < start else None
+        high_span = Span(end, span.end) if end < span.end else None
         start = max(start, span.end)
         # keep non-empty subspans
-        if low_span.start < low_span.end:
+        if low_span is not None:
           insert_spans.append(low_span)
-        else:
-          pass
-        if high_span.start < high_span.end:
+        if high_span is not None:
           insert_spans.append(high_span)
-        else:
-          pass
       i += 1
 
     if remove_mode and start < end:
       raise KeyError("span %s not entirely in Range" % (ospan,))
 
     drop_to = i
     if (drop_from is not None
```

### Comparing `cs.range-20230518/lib/python/cs.range.egg-info/PKG-INFO` & `cs.range-20230619/lib/python/cs.range.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.range
-Version: 20230518
+Version: 20230619
 Summary: a Range class implementing compact integer ranges with a set-like API, and associated functions
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,16 +17,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 
-*Latest release 20230518*:
-Span,Range: new as_list() methods.
+*Latest release 20230619*:
+* Span: sanity check .start and .end.
+* Range.issubset: efficient comparison with another Range, also .issuperset.
 
 ## Function `overlap(span1, span2)`
 
 Return a list `[start,end]` denoting the overlap of two spans.
 
 Example:
 
@@ -67,14 +68,18 @@
     >>> list(spans([1,2,3,7,8,11,5]))
     [1:4, 7:9, 11:12, 5:6]
 
 # Release Log
 
 
 
+*Release 20230619*:
+* Span: sanity check .start and .end.
+* Range.issubset: efficient comparison with another Range, also .issuperset.
+
 *Release 20230518*:
 Span,Range: new as_list() methods.
 
 *Release 20190102*:
 Span: provide __len__.
 
 *Release 20171231*:
```

### Comparing `cs.range-20230518/pyproject.toml` & `cs.range-20230619/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -18,29 +18,30 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230518"
+version = "20230619"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 
-*Latest release 20230518*:
-Span,Range: new as_list() methods.
+*Latest release 20230619*:
+* Span: sanity check .start and .end.
+* Range.issubset: efficient comparison with another Range, also .issuperset.
 
 ## Function `overlap(span1, span2)`
 
 Return a list `[start,end]` denoting the overlap of two spans.
 
 Example:
 
@@ -81,14 +82,18 @@
     >>> list(spans([1,2,3,7,8,11,5]))
     [1:4, 7:9, 11:12, 5:6]
 
 # Release Log
 
 
 
+*Release 20230619*:
+* Span: sanity check .start and .end.
+* Range.issubset: efficient comparison with another Range, also .issuperset.
+
 *Release 20230518*:
 Span,Range: new as_list() methods.
 
 *Release 20190102*:
 Span: provide __len__.
 
 *Release 20171231*:
```

### Comparing `cs.range-20230518/setup.cfg` & `cs.range-20230619/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.range
-version = 20230518
+version = 20230619
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = a Range class implementing compact integer ranges with a set-like API, and associated functions
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```

