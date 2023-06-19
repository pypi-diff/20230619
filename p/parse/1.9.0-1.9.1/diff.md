# Comparing `tmp/parse-1.9.0.tar.gz` & `tmp/parse-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parse-1.9.0.tar", last modified: Wed Oct  3 23:16:17 2018, max compression
+gzip compressed data, was "dist/parse-1.9.1.tar", last modified: Tue Jan 22 22:34:34 2019, max compression
```

## Comparing `parse-1.9.0.tar` & `parse-1.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-10-03 23:16:17.000000 parse-1.9.0/
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    19997 2018-10-03 23:16:17.000000 parse-1.9.0/PKG-INFO
--rwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)    39087 2018-10-03 23:12:29.000000 parse-1.9.0/test_parse.py
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-10-03 23:16:17.000000 parse-1.9.0/parse.egg-info/
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    19997 2018-10-03 23:16:17.000000 parse-1.9.0/parse.egg-info/PKG-INFO
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      170 2018-10-03 23:16:17.000000 parse-1.9.0/parse.egg-info/SOURCES.txt
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        6 2018-10-03 23:16:17.000000 parse-1.9.0/parse.egg-info/top_level.txt
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        1 2018-10-03 23:16:17.000000 parse-1.9.0/parse.egg-info/dependency_links.txt
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       32 2017-12-05 02:55:36.000000 parse-1.9.0/MANIFEST.in
--rwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1047 2018-10-03 22:25:29.000000 parse-1.9.0/setup.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       59 2018-10-03 23:16:17.000000 parse-1.9.0/setup.cfg
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    47551 2018-10-03 23:12:29.000000 parse-1.9.0/parse.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    16045 2018-10-03 23:16:17.000000 parse-1.9.0/README.rst
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2019-01-22 22:34:34.000000 parse-1.9.1/
+-rw-r--r--   0 richard    (501) staff       (20)    20172 2019-01-22 22:34:34.000000 parse-1.9.1/PKG-INFO
+-rwxr-xr-x   0 richard    (501) staff       (20)    39098 2019-01-22 22:29:16.000000 parse-1.9.1/test_parse.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2019-01-22 22:34:34.000000 parse-1.9.1/parse.egg-info/
+-rw-r--r--   0 richard    (501) staff       (20)    20172 2019-01-22 22:34:34.000000 parse-1.9.1/parse.egg-info/PKG-INFO
+-rw-r--r--   0 richard    (501) staff       (20)      170 2019-01-22 22:34:34.000000 parse-1.9.1/parse.egg-info/SOURCES.txt
+-rw-r--r--   0 richard    (501) staff       (20)        6 2019-01-22 22:34:34.000000 parse-1.9.1/parse.egg-info/top_level.txt
+-rw-r--r--   0 richard    (501) staff       (20)        1 2019-01-22 22:34:34.000000 parse-1.9.1/parse.egg-info/dependency_links.txt
+-rw-r--r--   0 richard    (501) staff       (20)       32 2018-05-26 23:11:29.000000 parse-1.9.1/MANIFEST.in
+-rwxr-xr-x   0 richard    (501) staff       (20)     1047 2019-01-22 22:00:23.000000 parse-1.9.1/setup.py
+-rw-r--r--   0 richard    (501) staff       (20)       38 2019-01-22 22:34:34.000000 parse-1.9.1/setup.cfg
+-rw-r--r--   0 richard    (501) staff       (20)    47751 2019-01-22 22:34:00.000000 parse-1.9.1/parse.py
+-rw-r--r--   0 richard    (501) staff       (20)    16196 2019-01-22 22:34:34.000000 parse-1.9.1/README.rst
```

### Comparing `parse-1.9.0/PKG-INFO` & `parse-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.1
 Name: parse
-Version: 1.9.0
+Version: 1.9.1
 Summary: parse() is the opposite of format()
 Home-page: https://github.com/r1chardj0n3s/parse
 Author: Richard Jones
 Author-email: rjones@ekit-inc.com
 License: UNKNOWN
 Description: Parse strings using a specification based on the Python format() syntax.
         
            ``parse()`` is the opposite of ``format()``
         
         The module is set up to only export ``parse()``, ``search()``, ``findall()``,
-        and ``with_pattern()`` when ``import *`` is used:
+        and ``with_pattern()`` when ``import \*`` is used:
         
         >>> from parse import *
         
         From there it's a simple thing to parse a string:
         
         >>> parse("It's {}, I love it!", "It's spam, I love it!")
         <Result ('spam',) {}>
@@ -136,46 +136,46 @@
           and "S" are also available.
         - The "e" and "g" types are case-insensitive so there is not need for
           the "E" or "G" types.
         
         ===== =========================================== ========
         Type  Characters Matched                          Output
         ===== =========================================== ========
-         w    Letters and underscore                      str
-         W    Non-letter and underscore                   str
-         s    Whitespace                                  str
-         S    Non-whitespace                              str
-         d    Digits (effectively integer numbers)        int
-         D    Non-digit                                   str
-         n    Numbers with thousands separators (, or .)  int
-         %    Percentage (converted to value/100.0)       float
-         f    Fixed-point numbers                         float
-         F    Decimal numbers                             Decimal
-         e    Floating-point numbers with exponent        float
+        w     Letters and underscore                      str
+        W     Non-letter and underscore                   str
+        s     Whitespace                                  str
+        S     Non-whitespace                              str
+        d     Digits (effectively integer numbers)        int
+        D     Non-digit                                   str
+        n     Numbers with thousands separators (, or .)  int
+        %     Percentage (converted to value/100.0)       float
+        f     Fixed-point numbers                         float
+        F     Decimal numbers                             Decimal
+        e     Floating-point numbers with exponent        float
               e.g. 1.1e-10, NAN (all case insensitive)
-         g    General number format (either d, f or e)    float
-         b    Binary numbers                              int
-         o    Octal numbers                               int
-         x    Hexadecimal numbers (lower and upper case)  int
-         ti   ISO 8601 format date/time                   datetime
+        g     General number format (either d, f or e)    float
+        b     Binary numbers                              int
+        o     Octal numbers                               int
+        x     Hexadecimal numbers (lower and upper case)  int
+        ti    ISO 8601 format date/time                   datetime
               e.g. 1972-01-20T10:21:36Z ("T" and "Z"
               optional)
-         te   RFC2822 e-mail format date/time             datetime
+        te    RFC2822 e-mail format date/time             datetime
               e.g. Mon, 20 Jan 1972 10:21:36 +1000
-         tg   Global (day/month) format date/time         datetime
+        tg    Global (day/month) format date/time         datetime
               e.g. 20/1/1972 10:21:36 AM +1:00
-         ta   US (month/day) format date/time             datetime
+        ta    US (month/day) format date/time             datetime
               e.g. 1/20/1972 10:21:36 PM +10:30
-         tc   ctime() format date/time                    datetime
+        tc    ctime() format date/time                    datetime
               e.g. Sun Sep 16 01:03:52 1973
-         th   HTTP log format date/time                   datetime
+        th    HTTP log format date/time                   datetime
               e.g. 21/Nov/2011:00:07:11 +0000
-         ts   Linux system log format date/time           datetime
+        ts    Linux system log format date/time           datetime
               e.g. Nov  9 03:37:44
-         tt   Time                                        time
+        tt    Time                                        time
               e.g. 10:21:36 PM -5:30
         ===== =========================================== ========
         
         Some examples of typed parsing with ``None`` returned if the typing
         does not match:
         
         >>> parse('Our {:d} {:w} are...', 'Our 3 weapons are...')
@@ -346,14 +346,17 @@
         the pattern, the actual match represents the shortest successful match for
         `dir1`.
         
         ----
         
         **Version history (in brief)**:
         
+        - 1.9.1 Fix deprecation warnings around backslashes in regex strings
+          (thanks Mickaël Schoentgen). Also fix some documentation formatting
+          issues.
         - 1.9.0 We now honor precision and width specifiers when parsing numbers
           and strings, allowing parsing of concatenated elements of fixed width
           (thanks Julia Signell)
         - 1.8.4 Add LICENSE file at request of packagers.
           Correct handling of AM/PM to follow most common interpretation.
           Correct parsing of hexadecimal that looks like a binary prefix.
           Add ability to parse case sensitively.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parse-1.9.0/test_parse.py` & `parse-1.9.1/test_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,48 +15,48 @@
 
 class TestPattern(unittest.TestCase):
     def _test_expression(self, format, expression):
         self.assertEqual(parse.Parser(format)._expression, expression)
 
     def test_braces(self):
         # pull a simple string out of another string
-        self._test_expression('{{ }}', '\{ \}')
+        self._test_expression('{{ }}', r'\{ \}')
 
     def test_fixed(self):
         # pull a simple string out of another string
-        self._test_expression('{}', '(.+?)')
-        self._test_expression('{} {}', '(.+?) (.+?)')
+        self._test_expression('{}', r'(.+?)')
+        self._test_expression('{} {}', r'(.+?) (.+?)')
 
     def test_named(self):
         # pull a named string out of another string
-        self._test_expression('{name}', '(?P<name>.+?)')
+        self._test_expression('{name}', r'(?P<name>.+?)')
         self._test_expression('{name} {other}',
-            '(?P<name>.+?) (?P<other>.+?)')
+            r'(?P<name>.+?) (?P<other>.+?)')
 
     def test_named_typed(self):
         # pull a named string out of another string
-        self._test_expression('{name:w}', '(?P<name>\w+)')
+        self._test_expression('{name:w}', r'(?P<name>\w+)')
         self._test_expression('{name:w} {other:w}',
-            '(?P<name>\w+) (?P<other>\w+)')
+            r'(?P<name>\w+) (?P<other>\w+)')
 
     def test_beaker(self):
         # skip some trailing whitespace
-        self._test_expression('{:<}', '(.+?) *')
+        self._test_expression('{:<}', r'(.+?) *')
 
     def test_left_fill(self):
         # skip some trailing periods
-        self._test_expression('{:.<}', '(.+?)\.*')
+        self._test_expression('{:.<}', r'(.+?)\.*')
 
     def test_bird(self):
         # skip some trailing whitespace
-        self._test_expression('{:>}', ' *(.+?)')
+        self._test_expression('{:>}', r' *(.+?)')
 
     def test_center(self):
         # skip some surrounding whitespace
-        self._test_expression('{:^}', ' *(.+?) *')
+        self._test_expression('{:^}', r' *(.+?) *')
 
     def test_format_variety(self):
         def _(fmt, matches):
             d = parse.extract_format(fmt, {'spam': 'spam'})
             for k in matches:
                 self.assertEqual(d.get(k), matches[k],
                     'm["%s"]=%r, expect %r' % (k, d.get(k), matches[k]))
```

### Comparing `parse-1.9.0/parse.egg-info/PKG-INFO` & `parse-1.9.1/parse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.1
 Name: parse
-Version: 1.9.0
+Version: 1.9.1
 Summary: parse() is the opposite of format()
 Home-page: https://github.com/r1chardj0n3s/parse
 Author: Richard Jones
 Author-email: rjones@ekit-inc.com
 License: UNKNOWN
 Description: Parse strings using a specification based on the Python format() syntax.
         
            ``parse()`` is the opposite of ``format()``
         
         The module is set up to only export ``parse()``, ``search()``, ``findall()``,
-        and ``with_pattern()`` when ``import *`` is used:
+        and ``with_pattern()`` when ``import \*`` is used:
         
         >>> from parse import *
         
         From there it's a simple thing to parse a string:
         
         >>> parse("It's {}, I love it!", "It's spam, I love it!")
         <Result ('spam',) {}>
@@ -136,46 +136,46 @@
           and "S" are also available.
         - The "e" and "g" types are case-insensitive so there is not need for
           the "E" or "G" types.
         
         ===== =========================================== ========
         Type  Characters Matched                          Output
         ===== =========================================== ========
-         w    Letters and underscore                      str
-         W    Non-letter and underscore                   str
-         s    Whitespace                                  str
-         S    Non-whitespace                              str
-         d    Digits (effectively integer numbers)        int
-         D    Non-digit                                   str
-         n    Numbers with thousands separators (, or .)  int
-         %    Percentage (converted to value/100.0)       float
-         f    Fixed-point numbers                         float
-         F    Decimal numbers                             Decimal
-         e    Floating-point numbers with exponent        float
+        w     Letters and underscore                      str
+        W     Non-letter and underscore                   str
+        s     Whitespace                                  str
+        S     Non-whitespace                              str
+        d     Digits (effectively integer numbers)        int
+        D     Non-digit                                   str
+        n     Numbers with thousands separators (, or .)  int
+        %     Percentage (converted to value/100.0)       float
+        f     Fixed-point numbers                         float
+        F     Decimal numbers                             Decimal
+        e     Floating-point numbers with exponent        float
               e.g. 1.1e-10, NAN (all case insensitive)
-         g    General number format (either d, f or e)    float
-         b    Binary numbers                              int
-         o    Octal numbers                               int
-         x    Hexadecimal numbers (lower and upper case)  int
-         ti   ISO 8601 format date/time                   datetime
+        g     General number format (either d, f or e)    float
+        b     Binary numbers                              int
+        o     Octal numbers                               int
+        x     Hexadecimal numbers (lower and upper case)  int
+        ti    ISO 8601 format date/time                   datetime
               e.g. 1972-01-20T10:21:36Z ("T" and "Z"
               optional)
-         te   RFC2822 e-mail format date/time             datetime
+        te    RFC2822 e-mail format date/time             datetime
               e.g. Mon, 20 Jan 1972 10:21:36 +1000
-         tg   Global (day/month) format date/time         datetime
+        tg    Global (day/month) format date/time         datetime
               e.g. 20/1/1972 10:21:36 AM +1:00
-         ta   US (month/day) format date/time             datetime
+        ta    US (month/day) format date/time             datetime
               e.g. 1/20/1972 10:21:36 PM +10:30
-         tc   ctime() format date/time                    datetime
+        tc    ctime() format date/time                    datetime
               e.g. Sun Sep 16 01:03:52 1973
-         th   HTTP log format date/time                   datetime
+        th    HTTP log format date/time                   datetime
               e.g. 21/Nov/2011:00:07:11 +0000
-         ts   Linux system log format date/time           datetime
+        ts    Linux system log format date/time           datetime
               e.g. Nov  9 03:37:44
-         tt   Time                                        time
+        tt    Time                                        time
               e.g. 10:21:36 PM -5:30
         ===== =========================================== ========
         
         Some examples of typed parsing with ``None`` returned if the typing
         does not match:
         
         >>> parse('Our {:d} {:w} are...', 'Our 3 weapons are...')
@@ -346,14 +346,17 @@
         the pattern, the actual match represents the shortest successful match for
         `dir1`.
         
         ----
         
         **Version history (in brief)**:
         
+        - 1.9.1 Fix deprecation warnings around backslashes in regex strings
+          (thanks Mickaël Schoentgen). Also fix some documentation formatting
+          issues.
         - 1.9.0 We now honor precision and width specifiers when parsing numbers
           and strings, allowing parsing of concatenated elements of fixed width
           (thanks Julia Signell)
         - 1.8.4 Add LICENSE file at request of packagers.
           Correct handling of AM/PM to follow most common interpretation.
           Correct parsing of hexadecimal that looks like a binary prefix.
           Add ability to parse case sensitively.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parse-1.9.0/setup.py` & `parse-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `parse-1.9.0/parse.py` & `parse-1.9.1/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# -*- encoding: utf-8 -*-
 r'''Parse strings using a specification based on the Python format() syntax.
 
    ``parse()`` is the opposite of ``format()``
 
 The module is set up to only export ``parse()``, ``search()``, ``findall()``,
-and ``with_pattern()`` when ``import *`` is used:
+and ``with_pattern()`` when ``import \*`` is used:
 
 >>> from parse import *
 
 From there it's a simple thing to parse a string:
 
 >>> parse("It's {}, I love it!", "It's spam, I love it!")
 <Result ('spam',) {}>
@@ -128,46 +129,46 @@
   and "S" are also available.
 - The "e" and "g" types are case-insensitive so there is not need for
   the "E" or "G" types.
 
 ===== =========================================== ========
 Type  Characters Matched                          Output
 ===== =========================================== ========
- w    Letters and underscore                      str
- W    Non-letter and underscore                   str
- s    Whitespace                                  str
- S    Non-whitespace                              str
- d    Digits (effectively integer numbers)        int
- D    Non-digit                                   str
- n    Numbers with thousands separators (, or .)  int
- %    Percentage (converted to value/100.0)       float
- f    Fixed-point numbers                         float
- F    Decimal numbers                             Decimal
- e    Floating-point numbers with exponent        float
+w     Letters and underscore                      str
+W     Non-letter and underscore                   str
+s     Whitespace                                  str
+S     Non-whitespace                              str
+d     Digits (effectively integer numbers)        int
+D     Non-digit                                   str
+n     Numbers with thousands separators (, or .)  int
+%     Percentage (converted to value/100.0)       float
+f     Fixed-point numbers                         float
+F     Decimal numbers                             Decimal
+e     Floating-point numbers with exponent        float
       e.g. 1.1e-10, NAN (all case insensitive)
- g    General number format (either d, f or e)    float
- b    Binary numbers                              int
- o    Octal numbers                               int
- x    Hexadecimal numbers (lower and upper case)  int
- ti   ISO 8601 format date/time                   datetime
+g     General number format (either d, f or e)    float
+b     Binary numbers                              int
+o     Octal numbers                               int
+x     Hexadecimal numbers (lower and upper case)  int
+ti    ISO 8601 format date/time                   datetime
       e.g. 1972-01-20T10:21:36Z ("T" and "Z"
       optional)
- te   RFC2822 e-mail format date/time             datetime
+te    RFC2822 e-mail format date/time             datetime
       e.g. Mon, 20 Jan 1972 10:21:36 +1000
- tg   Global (day/month) format date/time         datetime
+tg    Global (day/month) format date/time         datetime
       e.g. 20/1/1972 10:21:36 AM +1:00
- ta   US (month/day) format date/time             datetime
+ta    US (month/day) format date/time             datetime
       e.g. 1/20/1972 10:21:36 PM +10:30
- tc   ctime() format date/time                    datetime
+tc    ctime() format date/time                    datetime
       e.g. Sun Sep 16 01:03:52 1973
- th   HTTP log format date/time                   datetime
+th    HTTP log format date/time                   datetime
       e.g. 21/Nov/2011:00:07:11 +0000
- ts   Linux system log format date/time           datetime
+ts    Linux system log format date/time           datetime
       e.g. Nov  9 03:37:44
- tt   Time                                        time
+tt    Time                                        time
       e.g. 10:21:36 PM -5:30
 ===== =========================================== ========
 
 Some examples of typed parsing with ``None`` returned if the typing
 does not match:
 
 >>> parse('Our {:d} {:w} are...', 'Our 3 weapons are...')
@@ -338,14 +339,17 @@
 the pattern, the actual match represents the shortest successful match for
 `dir1`.
 
 ----
 
 **Version history (in brief)**:
 
+- 1.9.1 Fix deprecation warnings around backslashes in regex strings
+  (thanks Mickaël Schoentgen). Also fix some documentation formatting
+  issues.
 - 1.9.0 We now honor precision and width specifiers when parsing numbers
   and strings, allowing parsing of concatenated elements of fixed width
   (thanks Julia Signell)
 - 1.8.4 Add LICENSE file at request of packagers.
   Correct handling of AM/PM to follow most common interpretation.
   Correct parsing of hexadecimal that looks like a binary prefix.
   Add ability to parse case sensitively.
@@ -401,15 +405,15 @@
 - 1.0.0 initial release
 
 This code is copyright 2012-2017 Richard Jones <richard@python.org>
 See the end of the source file for the license of use.
 '''
 
 from __future__ import absolute_import
-__version__ = '1.9.0'
+__version__ = '1.9.1'
 
 # yes, I now have two problems
 import re
 import sys
 from datetime import datetime, time, tzinfo, timedelta
 from decimal import Decimal
 from functools import partial
@@ -526,17 +530,17 @@
     Jul=7, July=7,
     Aug=8, August=8,
     Sep=9, September=9,
     Oct=10, October=10,
     Nov=11, November=11,
     Dec=12, December=12
 )
-DAYS_PAT = '(Mon|Tue|Wed|Thu|Fri|Sat|Sun)'
-MONTHS_PAT = '(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)'
-ALL_MONTHS_PAT = '(%s)' % '|'.join(MONTHS_MAP)
+DAYS_PAT = r'(Mon|Tue|Wed|Thu|Fri|Sat|Sun)'
+MONTHS_PAT = r'(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)'
+ALL_MONTHS_PAT = r'(%s)' % '|'.join(MONTHS_MAP)
 TIME_PAT = r'(\d{1,2}:\d{1,2}(:\d{1,2}(\.\d+)?)?)'
 AM_PAT = r'(\s+[AP]M)'
 TZ_PAT = r'(\s+[-+]\d\d?:?\d\d)'
 
 
 def date_convert(string, match, ymd=None, mdy=None, dmy=None,
         d_m_y=None, hms=None, am=None, tz=None, mm=None, dd=None):
@@ -546,19 +550,19 @@
     groups = match.groups()
     time_only = False
     if mm and dd:
         y=datetime.today().year
         m=groups[mm]
         d=groups[dd]
     elif ymd is not None:
-        y, m, d = re.split('[-/\s]', groups[ymd])
+        y, m, d = re.split(r'[-/\s]', groups[ymd])
     elif mdy is not None:
-        m, d, y = re.split('[-/\s]', groups[mdy])
+        m, d, y = re.split(r'[-/\s]', groups[mdy])
     elif dmy is not None:
-        d, m, y = re.split('[-/\s]', groups[dmy])
+        d, m, y = re.split(r'[-/\s]', groups[dmy])
     elif d_m_y is not None:
         d, m, y = d_m_y
         d = groups[d]
         m = groups[m]
         y = groups[y]
     else:
         time_only = True
@@ -632,15 +636,15 @@
 
 class RepeatedNameError(ValueError):
     pass
 
 
 # note: {} are handled separately
 # note: I don't use r'' here because Sublime Text 2 syntax highlight has a fit
-REGEX_SAFETY = re.compile('([?\\\\.[\]()*+\^$!\|])')
+REGEX_SAFETY = re.compile(r'([?\\\\.[\]()*+\^$!\|])')
 
 # allowed field types
 ALLOWED_TYPES = set(list('nbox%fFegwWdDsS') +
     ['t' + c for c in 'ieahgcts'])
 
 
 def extract_format(format, extra_types):
@@ -741,15 +745,15 @@
                     raise TooManyFields('sorry, you are attempting to parse '
                         'too many complex fields')
         return self.__search_re
 
     @property
     def _match_re(self):
         if self.__match_re is None:
-            expression = '^%s$' % self._expression
+            expression = r'^%s$' % self._expression
             try:
                 self.__match_re = re.compile(expression, self._re_flags)
             except AssertionError:
                 # access error through sys to keep py3k and backward compat
                 e = str(sys.exc_info()[1])
                 if e.endswith('this version only supports 100 named groups'):
                     raise TooManyFields('sorry, you are attempting to parse '
@@ -919,32 +923,32 @@
             if name in self._name_to_group_map:
                 if self._name_types[name] != format:
                     raise RepeatedNameError('field type %r for field "%s" '
                         'does not match previous seen type %r' % (format,
                         name, self._name_types[name]))
                 group = self._name_to_group_map[name]
                 # match previously-seen value
-                return '(?P=%s)' % group
+                return r'(?P=%s)' % group
             else:
                 group = self._to_group_name(name)
                 self._name_types[name] = format
             self._named_fields.append(group)
             # this will become a group, which must not contain dots
-            wrap = '(?P<%s>%%s)' % group
+            wrap = r'(?P<%s>%%s)' % group
         else:
             self._fixed_fields.append(self._group_index)
-            wrap = '(%s)'
+            wrap = r'(%s)'
             if ':' in field:
                 format = field[1:]
             group = self._group_index
 
         # simplest case: no type specifier ({} or {name})
         if not format:
             self._group_index += 1
-            return wrap % '.+?'
+            return wrap % r'.+?'
 
         # decode the format specification
         format = extract_format(format, self._extra_types)
 
         # figure type conversions, if any
         type = format['type']
         is_numeric = type and type in 'n%fegdobh'
@@ -956,27 +960,27 @@
                 regex_group_count = 0
             self._group_index += regex_group_count
 
             def f(string, m):
                 return type_converter(string)
             self._type_conversions[group] = f
         elif type == 'n':
-            s = '\d{1,3}([,.]\d{3})*'
+            s = r'\d{1,3}([,.]\d{3})*'
             self._group_index += 1
             self._type_conversions[group] = int_convert(10)
         elif type == 'b':
-            s = '(0[bB])?[01]+'
+            s = r'(0[bB])?[01]+'
             self._type_conversions[group] = int_convert(2)
             self._group_index += 1
         elif type == 'o':
-            s = '(0[oO])?[0-7]+'
+            s = r'(0[oO])?[0-7]+'
             self._type_conversions[group] = int_convert(8)
             self._group_index += 1
         elif type == 'x':
-            s = '(0[xX])?[0-9a-fA-F]+'
+            s = r'(0[xX])?[0-9a-fA-F]+'
             self._type_conversions[group] = int_convert(16)
             self._group_index += 1
         elif type == '%':
             s = r'\d+(\.\d+)?%'
             self._group_index += 1
             self._type_conversions[group] = percentage
         elif type == 'f':
@@ -990,18 +994,18 @@
             self._type_conversions[group] = lambda s, m: float(s)
         elif type == 'g':
             s = r'\d+(\.\d+)?([eE][-+]?\d+)?|nan|NAN|[-+]?inf|[-+]?INF'
             self._group_index += 2
             self._type_conversions[group] = lambda s, m: float(s)
         elif type == 'd':
             if format.get('width'):
-                width = '{1,%s}' % int(format['width'])
+                width = r'{1,%s}' % int(format['width'])
             else:
                 width = '+'
-            s = '\\d{w}|0[xX][0-9a-fA-F]{w}|0[bB][01]{w}|0[oO][0-7]{w}'.format(w=width)
+            s = r'\d{w}|0[xX][0-9a-fA-F]{w}|0[bB][01]{w}|0[oO][0-7]{w}'.format(w=width)
             self._type_conversions[group] = int_convert(10)
         elif type == 'ti':
             s = r'(\d{4}-\d\d-\d\d)((\s+|T)%s)?(Z|\s*[-+]\d\d:?\d\d)?' % \
                 TIME_PAT
             n = self._group_index
             self._type_conversions[group] = partial(date_convert, ymd=n + 1,
                 hms=n + 4, tz=n + 7)
@@ -1056,34 +1060,34 @@
                 hms=n + 5)
             self._group_index += 5
 
         elif type:
             s = r'\%s+' % type
         elif format.get('precision'):
             if format.get('width'):
-                s = '.{%s,%s}?' % (format['width'], format['precision'])
+                s = r'.{%s,%s}?' % (format['width'], format['precision'])
             else:
-                s = '.{1,%s}?' % format['precision']
+                s = r'.{1,%s}?' % format['precision']
         elif format.get('width'):
-            s = '.{%s,}?' % format['width']
+            s = r'.{%s,}?' % format['width']
         else:
-            s = '.+?'
+            s = r'.+?'
 
         align = format['align']
         fill = format['fill']
 
         # handle some numeric-specific things like fill and sign
         if is_numeric:
             # prefix with something (align "=" trumps zero)
             if align == '=':
                 # special case - align "=" acts like the zero above but with
                 # configurable fill defaulting to "0"
                 if not fill:
                     fill = '0'
-                s = '%s*' % fill + s
+                s = r'%s*' % fill + s
 
             # allow numbers to be prefixed with a sign
             s = r'[-+ ]?' + s
 
         if not fill:
             fill = ' '
 
@@ -1097,15 +1101,15 @@
             # all we really care about is that if the format originally
             # specified a width then there will probably be padding - without
             # an explicit alignment that'll mean right alignment with spaces
             # padding
             if not align:
                 align = '>'
 
-        if fill in '.\+?*[](){}^$':
+        if fill in r'.\+?*[](){}^$':
             fill = '\\' + fill
 
         # align "=" has been handled
         if align == '<':
             s = '%s%s*' % (s, fill)
         elif align == '>':
             s = '%s*%s' % (fill, s)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parse-1.9.0/README.rst` & `parse-1.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Parse strings using a specification based on the Python format() syntax.
 
    ``parse()`` is the opposite of ``format()``
 
 The module is set up to only export ``parse()``, ``search()``, ``findall()``,
-and ``with_pattern()`` when ``import *`` is used:
+and ``with_pattern()`` when ``import \*`` is used:
 
 >>> from parse import *
 
 From there it's a simple thing to parse a string:
 
 >>> parse("It's {}, I love it!", "It's spam, I love it!")
 <Result ('spam',) {}>
@@ -128,46 +128,46 @@
   and "S" are also available.
 - The "e" and "g" types are case-insensitive so there is not need for
   the "E" or "G" types.
 
 ===== =========================================== ========
 Type  Characters Matched                          Output
 ===== =========================================== ========
- w    Letters and underscore                      str
- W    Non-letter and underscore                   str
- s    Whitespace                                  str
- S    Non-whitespace                              str
- d    Digits (effectively integer numbers)        int
- D    Non-digit                                   str
- n    Numbers with thousands separators (, or .)  int
- %    Percentage (converted to value/100.0)       float
- f    Fixed-point numbers                         float
- F    Decimal numbers                             Decimal
- e    Floating-point numbers with exponent        float
+w     Letters and underscore                      str
+W     Non-letter and underscore                   str
+s     Whitespace                                  str
+S     Non-whitespace                              str
+d     Digits (effectively integer numbers)        int
+D     Non-digit                                   str
+n     Numbers with thousands separators (, or .)  int
+%     Percentage (converted to value/100.0)       float
+f     Fixed-point numbers                         float
+F     Decimal numbers                             Decimal
+e     Floating-point numbers with exponent        float
       e.g. 1.1e-10, NAN (all case insensitive)
- g    General number format (either d, f or e)    float
- b    Binary numbers                              int
- o    Octal numbers                               int
- x    Hexadecimal numbers (lower and upper case)  int
- ti   ISO 8601 format date/time                   datetime
+g     General number format (either d, f or e)    float
+b     Binary numbers                              int
+o     Octal numbers                               int
+x     Hexadecimal numbers (lower and upper case)  int
+ti    ISO 8601 format date/time                   datetime
       e.g. 1972-01-20T10:21:36Z ("T" and "Z"
       optional)
- te   RFC2822 e-mail format date/time             datetime
+te    RFC2822 e-mail format date/time             datetime
       e.g. Mon, 20 Jan 1972 10:21:36 +1000
- tg   Global (day/month) format date/time         datetime
+tg    Global (day/month) format date/time         datetime
       e.g. 20/1/1972 10:21:36 AM +1:00
- ta   US (month/day) format date/time             datetime
+ta    US (month/day) format date/time             datetime
       e.g. 1/20/1972 10:21:36 PM +10:30
- tc   ctime() format date/time                    datetime
+tc    ctime() format date/time                    datetime
       e.g. Sun Sep 16 01:03:52 1973
- th   HTTP log format date/time                   datetime
+th    HTTP log format date/time                   datetime
       e.g. 21/Nov/2011:00:07:11 +0000
- ts   Linux system log format date/time           datetime
+ts    Linux system log format date/time           datetime
       e.g. Nov  9 03:37:44
- tt   Time                                        time
+tt    Time                                        time
       e.g. 10:21:36 PM -5:30
 ===== =========================================== ========
 
 Some examples of typed parsing with ``None`` returned if the typing
 does not match:
 
 >>> parse('Our {:d} {:w} are...', 'Our 3 weapons are...')
@@ -338,14 +338,17 @@
 the pattern, the actual match represents the shortest successful match for
 `dir1`.
 
 ----
 
 **Version history (in brief)**:
 
+- 1.9.1 Fix deprecation warnings around backslashes in regex strings
+  (thanks Mickaël Schoentgen). Also fix some documentation formatting
+  issues.
 - 1.9.0 We now honor precision and width specifiers when parsing numbers
   and strings, allowing parsing of concatenated elements of fixed width
   (thanks Julia Signell)
 - 1.8.4 Add LICENSE file at request of packagers.
   Correct handling of AM/PM to follow most common interpretation.
   Correct parsing of hexadecimal that looks like a binary prefix.
   Add ability to parse case sensitively.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

