# Comparing `tmp/colored-1.4.3.tar.gz` & `tmp/colored-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colored-1.4.3.tar", last modified: Sat Oct 23 17:52:42 2021, max compression
+gzip compressed data, from Unix
```

## Comparing `colored-1.4.3.tar` & `colored-1.4.4.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2021-10-23 17:52:42.000000 colored-1.4.3/
--rw-r--r--   0 dslackw   (1000) users      (100)     3504 2021-10-23 17:47:20.000000 colored-1.4.3/CHANGES.md
--rw-r--r--   0 dslackw   (1000) users      (100)     1070 2021-10-23 17:47:20.000000 colored-1.4.3/LICENSE.txt
--rw-r--r--   0 dslackw   (1000) users      (100)      310 2021-10-23 17:47:20.000000 colored-1.4.3/MANIFEST.in
--rw-r--r--   0 dslackw   (1000) users      (100)    18419 2021-10-23 17:52:42.000000 colored-1.4.3/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)    13525 2021-10-23 17:47:20.000000 colored-1.4.3/README.rst
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2021-10-23 17:52:42.000000 colored-1.4.3/colored/
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2021-10-23 17:47:20.000000 colored-1.4.3/colored/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)      242 2021-10-23 17:47:20.000000 colored-1.4.3/colored/back.py
--rw-r--r--   0 dslackw   (1000) users      (100)    15842 2021-10-23 17:47:20.000000 colored-1.4.3/colored/colored.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4991 2021-10-23 17:47:20.000000 colored-1.4.3/colored/colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      242 2021-10-23 17:47:20.000000 colored-1.4.3/colored/fore.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6726 2021-10-23 17:47:20.000000 colored-1.4.3/colored/hex.py
--rw-r--r--   0 dslackw   (1000) users      (100)      515 2021-10-23 17:47:20.000000 colored-1.4.3/colored/style.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2021-10-23 17:52:42.000000 colored-1.4.3/colored.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)    18419 2021-10-23 17:52:42.000000 colored-1.4.3/colored.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)      519 2021-10-23 17:52:42.000000 colored-1.4.3/colored.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2021-10-23 17:52:42.000000 colored-1.4.3/colored.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        8 2021-10-23 17:52:42.000000 colored-1.4.3/colored.egg-info/top_level.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2021-10-23 17:52:42.000000 colored-1.4.3/docs/
--rw-r--r--   0 dslackw   (1000) users      (100)     6223 2021-10-23 17:47:20.000000 colored-1.4.3/docs/back.COLOR.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     4943 2021-10-23 17:47:20.000000 colored-1.4.3/docs/colors_list.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     6219 2021-10-23 17:47:20.000000 colored-1.4.3/docs/fore.COLOR.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     3855 2021-10-23 17:47:20.000000 colored-1.4.3/docs/hex_list.txt
--rw-r--r--   0 dslackw   (1000) users      (100)      296 2021-10-23 17:47:20.000000 colored-1.4.3/docs/style.COLOR.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       38 2021-10-23 17:52:42.000000 colored-1.4.3/setup.cfg
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1630 2021-10-23 17:47:20.000000 colored-1.4.3/setup.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2021-10-23 17:52:42.000000 colored-1.4.3/tests/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      399 2021-10-23 17:47:20.000000 colored-1.4.3/tests/test_1.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     6511 2021-10-23 17:47:20.000000 colored-1.4.3/tests/test_2.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     5424 2021-10-23 17:47:20.000000 colored-1.4.3/tests/test_3.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)    32057 2021-10-23 17:47:20.000000 colored-1.4.3/tests/test_4.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     5424 2021-10-23 17:47:20.000000 colored-1.4.3/tests/test_5.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     3111 2021-10-23 17:47:20.000000 colored-1.4.3/tests/test_hex_1.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1006 2021-10-23 17:47:20.000000 colored-1.4.3/tests/test_hex_2.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-11 16:39:51.000000 colored-1.4.4/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1070 2022-11-09 15:59:15.000000 colored-1.4.4/LICENSE.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     3665 2022-11-09 15:59:15.000000 colored-1.4.4/CHANGES.md
+-rw-r--r--   0 dslackw   (1000) users      (100)      310 2022-11-09 15:59:15.000000 colored-1.4.4/MANIFEST.in
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-09 15:59:15.000000 colored-1.4.4/docs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6223 2022-11-09 15:59:15.000000 colored-1.4.4/docs/back.COLOR.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     4943 2022-11-09 15:59:15.000000 colored-1.4.4/docs/colors_list.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     6219 2022-11-09 15:59:15.000000 colored-1.4.4/docs/fore.COLOR.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     3855 2022-11-09 15:59:15.000000 colored-1.4.4/docs/hex_list.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)      296 2022-11-09 15:59:15.000000 colored-1.4.4/docs/style.COLOR.txt
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1173 2022-11-09 15:59:15.000000 colored-1.4.4/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    13489 2022-11-09 15:59:15.000000 colored-1.4.4/README.rst
+-rw-r--r--   0 dslackw   (1000) users      (100)       32 2022-11-09 15:59:15.000000 colored-1.4.4/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-09 15:59:15.000000 colored-1.4.4/tests/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     6511 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_2.py
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      400 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_1.py
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     3111 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_hex_1.py
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1006 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_hex_2.py
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     5424 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_3.py
+-rwxr-xr-x   0 dslackw   (1000) users      (100)    32058 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_4.py
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     5424 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_5.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      153 2022-11-09 15:59:15.000000 colored-1.4.4/.travis.yml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)      519 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        8 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)    14472 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)       83 2022-11-09 15:59:15.000000 colored-1.4.4/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-11 16:39:47.000000 colored-1.4.4/colored/
+-rw-r--r--   0 dslackw   (1000) users      (100)      495 2022-11-09 15:59:15.000000 colored-1.4.4/colored/style.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4991 2022-11-09 15:59:15.000000 colored-1.4.4/colored/colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    15844 2022-11-09 15:59:15.000000 colored-1.4.4/colored/colored.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/
+-rw-r--r--   0 dslackw   (1000) users      (100)      647 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/style.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)      362 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)     3555 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/colors.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)    10798 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/colored.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)     5345 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/hex.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)      441 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/back.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)      441 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/fore.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)      255 2022-11-09 15:59:15.000000 colored-1.4.4/colored/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6742 2022-11-09 15:59:15.000000 colored-1.4.4/colored/hex.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      209 2022-11-09 15:59:15.000000 colored-1.4.4/colored/fore.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      209 2022-11-09 15:59:15.000000 colored-1.4.4/colored/back.py
```

### Comparing `colored-1.4.3/CHANGES.md` & `colored-1.4.4/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 colored
 =====
 
+Version 1.4.4 - *(09-11-2022)*
+-----
+### Updated
+- Code style
+- Switch to f string
+- Removed python2 support
+- Use windows types instead of raw ctypes. Ref #25
+
 Version 1.4.3 - *(23-10-2021)*
 -----
 ### Updated
 - Improve color enabling #18
 
 
 Version 1.4.2 - *(09-12-2019)*
```

### Comparing `colored-1.4.3/LICENSE.txt` & `colored-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colored-1.4.3/PKG-INFO` & `colored-1.4.4/colored.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,474 +1,469 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: colored
-Version: 1.4.3
+Version: 1.4.4
 Summary: Simple library for color and formatting to terminal
 Home-page: https://gitlab.com/dslackw/colored
 Author: dslackw
 Author-email: d.zlatanidis@gamil.com
 License: UNKNOWN
-Description: Very simple Python library for color and formatting in terminal.
-        Collection of color codes and names for 256 color terminal setups.
-        The following is a list of 256 colors for Xterm, containing an example
-        of the displayed color, Xterm Name, Xterm Number and HEX.
-        
-        .. image:: https://gitlab.com/dslackw/images/raw/master/colored/logo.png
-            :target: https://gitlab.com/dslackw/colored
-        
-        `[CHANGELOG] <https://gitlab.com/dslackw/colored/blob/master/CHANGELOG>`_
-        
-        Video Demo
-        ----------
-        
-        .. image:: https://gitlab.com/dslackw/images/raw/master/colored/video.png
-            :target: https://asciinema.org/a/bgxm6KisSvPkPwMsYLyBBJjth
-        
-        The following colors works with most terminals and terminals emulators.
-        ANSI/VT100 escape sequences can be used in every programming languages.
-        
-        Attributes:
-        
-        .. code-block:: bash
-        
-            +-----+------------------+
-            |Code | Description      |
-            +-----+------------------+
-            |  1  | bold             |
-            |  2  | dim              |
-            |  4  | underlined       |
-            |  5  | blink            |
-            |  7  | reverse          |
-            |  8  | hidden           |
-            |  0  | reset            |
-            |  21 | res_bold         |
-            |  22 | res_dim          |
-            |  24 | res_underlined   |
-            |  25 | res_blink        |
-            |  27 | res_reverse      |
-            |  28 | res_hidden       |
-            +------------------------+
-        
-        
-        256 Foreground and Background Colors - Full Chart:
-        
-        .. code-block:: bash
-        
-            +-----+---------------------+
-            |Code | Description         |
-            +-----+---------------------+
-            | 0   | black               |
-            | 1   | red                 |
-            | 2   | green               |
-            | 3   | yellow              |
-            | 4   | blue                |
-            | 5   | magenta             |
-            | 6   | cyan                |
-            | 7   | light_gray          |
-            | 8   | dark_gray           |
-            | 9   | light_red           |
-            | 10  | light_green         |
-            | 11  | light_yellow        |
-            | 12  | light_blue          |
-            | 13  | light_magenta       |
-            | 14  | light_cyan          |
-            | 15  | white               |
-            | 16  | grey_0              |
-            | 17  | navy_blue           |
-            | 18  | dark_blue           |
-            | 19  | blue_3a             |
-            | 20  | blue_3b             |
-            | 21  | blue_1              |
-            | 22  | dark_green          |
-            | 23  | deep_sky_blue_4a    |
-            | 24  | deep_sky_blue_4b    |
-            | 25  | deep_sky_blue_4c    |
-            | 26  | dodger_blue_3       |
-            | 27  | dodger_blue_2       |
-            | 28  | green_4             |
-            | 29  | spring_green_4      |
-            | 30  | turquoise_4         |
-            | 31  | deep_sky_blue_3a    |
-            | 32  | deep_sky_blue_3b    |
-            | 33  | dodger_blue_1       |
-            | 34  | green_3a            |
-            | 35  | spring_green_3a     |
-            | 36  | dark_cyan           |
-            | 37  | light_sea_green     |
-            | 38  | deep_sky_blue_2     |
-            | 39  | deep_sky_blue_1     |
-            | 40  | green_3b            |
-            | 41  | spring_green_3b     |
-            | 42  | spring_green_2a     |
-            | 43  | cyan_3              |
-            | 44  | dark_turquoise      |
-            | 45  | turquoise_2         |
-            | 46  | green_1             |
-            | 47  | spring_green_2b     |
-            | 48  | spring_green_1      |
-            | 49  | medium_spring_green |
-            | 50  | cyan_2              |
-            | 51  | cyan_1              |
-            | 52  | dark_red_1          |
-            | 53  | deep_pink_4a        |
-            | 54  | purple_4a           |
-            | 55  | purple_4b           |
-            | 56  | purple_3            |
-            | 57  | blue_violet         |
-            | 58  | orange_4a           |
-            | 59  | grey_37             |
-            | 60  | medium_purple_4     |
-            | 61  | slate_blue_3a       |
-            | 62  | slate_blue_3b       |
-            | 63  | royal_blue_1        |
-            | 64  | chartreuse_4        |
-            | 65  | dark_sea_green_4a   |
-            | 66  | pale_turquoise_4    |
-            | 67  | steel_blue          |
-            | 68  | steel_blue_3        |
-            | 69  | cornflower_blue     |
-            | 70  | chartreuse_3a       |
-            | 71  | dark_sea_green_4b   |
-            | 72  | cadet_blue_2        |
-            | 73  | cadet_blue_1        |
-            | 74  | sky_blue_3          |
-            | 75  | steel_blue_1a       |
-            | 76  | chartreuse_3b       |
-            | 77  | pale_green_3a       |
-            | 78  | sea_green_3         |
-            | 79  | aquamarine_3        |
-            | 80  | medium_turquoise    |
-            | 81  | steel_blue_1b       |
-            | 82  | chartreuse_2a       |
-            | 83  | sea_green_2         |
-            | 84  | sea_green_1a        |
-            | 85  | sea_green_1b        |
-            | 86  | aquamarine_1a       |
-            | 87  | dark_slate_gray_2   |
-            | 88  | dark_red_2          |
-            | 89  | deep_pink_4b        |
-            | 90  | dark_magenta_1      |
-            | 91  | dark_magenta_2      |
-            | 92  | dark_violet_1a      |
-            | 93  | purple_1a           |
-            | 94  | orange_4b           |
-            | 95  | light_pink_4        |
-            | 96  | plum_4              |
-            | 97  | medium_purple_3a    |
-            | 98  | medium_purple_3b    |
-            | 99  | slate_blue_1        |
-            | 100 | yellow_4a           |
-            | 101 | wheat_4             |
-            | 102 | grey_53             |
-            | 103 | light_slate_grey    |
-            | 104 | medium_purple       |
-            | 105 | light_slate_blue    |
-            | 106 | yellow_4b           |
-            | 107 | dark_olive_green_3a |
-            | 108 | dark_green_sea      |
-            | 109 | light_sky_blue_3a   |
-            | 110 | light_sky_blue_3b   |
-            | 111 | sky_blue_2          |
-            | 112 | chartreuse_2b       |
-            | 113 | dark_olive_green_3b |
-            | 114 | pale_green_3b       |
-            | 115 | dark_sea_green_3a   |
-            | 116 | dark_slate_gray_3   |
-            | 117 | sky_blue_1          |
-            | 118 | chartreuse_1        |
-            | 119 | light_green_2       |
-            | 120 | light_green_3       |
-            | 121 | pale_green_1a       |
-            | 122 | aquamarine_1b       |
-            | 123 | dark_slate_gray_1   |
-            | 124 | red_3a              |
-            | 125 | deep_pink_4c        |
-            | 126 | medium_violet_red   |
-            | 127 | magenta_3a          |
-            | 128 | dark_violet_1b      |
-            | 129 | purple_1b           |
-            | 130 | dark_orange_3a      |
-            | 131 | indian_red_1a       |
-            | 132 | hot_pink_3a         |
-            | 133 | medium_orchid_3     |
-            | 134 | medium_orchid       |
-            | 135 | medium_purple_2a    |
-            | 136 | dark_goldenrod      |
-            | 137 | light_salmon_3a     |
-            | 138 | rosy_brown          |
-            | 139 | grey_63             |
-            | 140 | medium_purple_2b    |
-            | 141 | medium_purple_1     |
-            | 142 | gold_3a             |
-            | 143 | dark_khaki          |
-            | 144 | navajo_white_3      |
-            | 145 | grey_69             |
-            | 146 | light_steel_blue_3  |
-            | 147 | light_steel_blue    |
-            | 148 | yellow_3a           |
-            | 149 | dark_olive_green_3  |
-            | 150 | dark_sea_green_3b   |
-            | 151 | dark_sea_green_2    |
-            | 152 | light_cyan_3        |
-            | 153 | light_sky_blue_1    |
-            | 154 | green_yellow        |
-            | 155 | dark_olive_green_2  |
-            | 156 | pale_green_1b       |
-            | 157 | dark_sea_green_5b   |
-            | 158 | dark_sea_green_5a   |
-            | 159 | pale_turquoise_1    |
-            | 160 | red_3b              |
-            | 161 | deep_pink_3a        |
-            | 162 | deep_pink_3b        |
-            | 163 | magenta_3b          |
-            | 164 | magenta_3c          |
-            | 165 | magenta_2a          |
-            | 166 | dark_orange_3b      |
-            | 167 | indian_red_1b       |
-            | 168 | hot_pink_3b         |
-            | 169 | hot_pink_2          |
-            | 170 | orchid              |
-            | 171 | medium_orchid_1a    |
-            | 172 | orange_3            |
-            | 173 | light_salmon_3b     |
-            | 174 | light_pink_3        |
-            | 175 | pink_3              |
-            | 176 | plum_3              |
-            | 177 | violet              |
-            | 178 | gold_3b             |
-            | 179 | light_goldenrod_3   |
-            | 180 | tan                 |
-            | 181 | misty_rose_3        |
-            | 182 | thistle_3           |
-            | 183 | plum_2              |
-            | 184 | yellow_3b           |
-            | 185 | khaki_3             |
-            | 186 | light_goldenrod_2a  |
-            | 187 | light_yellow_3      |
-            | 188 | grey_84             |
-            | 189 | light_steel_blue_1  |
-            | 190 | yellow_2            |
-            | 191 | dark_olive_green_1a |
-            | 192 | dark_olive_green_1b |
-            | 193 | dark_sea_green_1    |
-            | 194 | honeydew_2          |
-            | 195 | light_cyan_1        |
-            | 196 | red_1               |
-            | 197 | deep_pink_2         |
-            | 198 | deep_pink_1a        |
-            | 199 | deep_pink_1b        |
-            | 200 | magenta_2b          |
-            | 201 | magenta_1           |
-            | 202 | orange_red_1        |
-            | 203 | indian_red_1c       |
-            | 204 | indian_red_1d       |
-            | 205 | hot_pink_1a         |
-            | 206 | hot_pink_1b         |
-            | 207 | medium_orchid_1b    |
-            | 208 | dark_orange         |
-            | 209 | salmon_1            |
-            | 210 | light_coral         |
-            | 211 | pale_violet_red_1   |
-            | 212 | orchid_2            |
-            | 213 | orchid_1            |
-            | 214 | orange_1            |
-            | 215 | sandy_brown         |
-            | 216 | light_salmon_1      |
-            | 217 | light_pink_1        |
-            | 218 | pink_1              |
-            | 219 | plum_1              |
-            | 220 | gold_1              |
-            | 221 | light_goldenrod_2b  |
-            | 222 | light_goldenrod_2c  |
-            | 223 | navajo_white_1      |
-            | 224 | misty_rose1         |
-            | 225 | thistle_1           |
-            | 226 | yellow_1            |
-            | 227 | light_goldenrod_1   |
-            | 228 | khaki_1             |
-            | 229 | wheat_1             |
-            | 230 | cornsilk_1          |
-            | 231 | grey_100            |
-            | 232 | grey_3              |
-            | 233 | grey_7              |
-            | 234 | grey_11             |
-            | 235 | grey_15             |
-            | 236 | grey_19             |
-            | 237 | grey_23             |
-            | 238 | grey_27             |
-            | 239 | grey_30             |
-            | 240 | grey_35             |
-            | 241 | grey_39             |
-            | 242 | grey_42             |
-            | 243 | grey_46             |
-            | 244 | grey_50             |
-            | 245 | grey_54             |
-            | 246 | grey_58             |
-            | 247 | grey_62             |
-            | 248 | grey_66             |
-            | 249 | grey_70             |
-            | 250 | grey_74             |
-            | 251 | grey_78             |
-            | 252 | grey_82             |
-            | 253 | grey_85             |
-            | 254 | grey_89             |
-            | 255 | grey_93             |
-            | 256 | default             |
-            +-----+---------------------+
-        
-        256 Colors Foreground (text):
-        
-        .. image:: https://gitlab.com/dslackw/images/raw/master/colored/256_colors_fg.png
-            :alt: 256 fg colors
-        
-        256 Colors Background:
-        
-        .. image:: https://gitlab.com/dslackw/images/raw/master/colored/256_colors_bg.png
-            :alt: 256 bg colors
-        
-        
-        Installation
-        ------------
-        
-        .. code-block:: bash
-        
-            $ pip install colored --upgrade
-        
-            uninstall
-        
-            $ pip uninstall colored
-        
-        
-        Dependencies
-        ------------
-        
-        None, only Python programming language.
-        
-        Usage Examples
-        --------------
-        
-        How to use the module in your own python code:
-        
-        .. code-block:: bash
-        
-            >>> from colored import fg, bg, attr
-            >>>
-            >>> print ('%s Hello World !!! %s' % (fg(1), attr(0)))
-             Hello World !!!
-            >>>
-            >>> print ('%s%s Hello World !!! %s' % (fg(1), bg(15), attr(0)))
-             Hello World !!!
-        
-        Use description:
-        
-        .. code-block:: bash
-        
-            >>> print ('%s%s Hello World !!! %s' % (fg('white'), bg('yellow'), attr('reset')))
-             Hello World !!!
-            >>>
-            >>> print ('%s%s Hello World !!! %s' % (fg('orchid'), attr('bold'), attr('reset')))
-             Hello World !!!
-            >>>
-            >>> color = bg('indian_red_1a') + fg('white')
-            >>> reset = attr('reset')
-            >>> print (color + 'Hello World !!!' + reset)
-            Hello World !!!
-        
-        Or use HEX code:
-        
-        .. code-block:: bash
-        
-            >>> color = fg('#C0C0C0') + bg('#00005f')
-            >>> res = attr('reset')
-            >>> print (color + "Hello World !!!" + res)
-            Hello World !!!
-        
-        Or the convenient `stylize(text, *styles)` wrapper to save some keystrokes:
-        
-        .. code-block:: bash
-        
-            >>> import colored
-            >>> from colored import stylize
-            >>> print(stylize("This is green.", colored.fg("green")))
-            This is green.
-            >>> print("This is not.")
-            This is not.
-            >>> angry = colored.fg("red") + colored.attr("bold")
-            >>> print(stylize("This is angry text.", angry))
-            This is angry text.
-            >>> print(stylize("This is VERY angry text.", angry, colored.attr("underlined")))
-            This is VERY angry text.
-            >>> print("But this is not.")
-            But this is not.
-        
-        Or the variant `stylize_interactive(text, *styles)` for readline-friendliness:
-        
-        .. code-block:: bash
-        
-            >>> import colored, sys
-            >>> from colored import stylize_interactive, fg
-            >>> sys.ps1 = stylize_interactive("myPrompt: ", fg('red'))
-            myPrompt:
-        
-        Use directly like `colorama <https://pypi.python.org/pypi/colorama>`_ but with more colors:
-        
-        .. code-block:: bash
-        
-            >>> from colored import fore, back, style
-            >>>
-            >>> print (fore.LIGHT_BLUE + back.RED + style.BOLD + "Hello World !!!" + style.RESET)
-        
-        Import colored module:
-        
-        .. code-block:: bash
-        
-           >>> import colored
-           >>>
-           >>> colored.fg(1)
-           '\x1b[38;5;1m'
-           >>>
-           >>> colored.fg(257)
-           Traceback (most recent call last):
-             File "<input>", line 1, in <module>
-             File "/usr/lib64/python2.7/site-packages/colored/colored.py", line 381, in fg
-               return colored(color).foreground()
-             File "/usr/lib64/python2.7/site-packages/colored/colored.py", line 350, in foreground
-               color = self.reserve_paint[str(self.color)]
-           KeyError: '257'
-           >>>
-           >>> colored.bg(30)
-           '\x1b[48;5;30m'
-           >>>
-           >>> colored.fore.BLUE
-           '\x1b[38;5;4m'
-        
-            etc.
-        
-        
-        Screenshot:
-        
-        .. image:: https://gitlab.com/dslackw/images/raw/master/colored/screenshot-2.png
-            :alt: example
-        
 Keywords: color,colour,paint,ansi,terminal,linux,python
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Other
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.0
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Terminals
+License-File: LICENSE.txt
+
+Very simple Python library for color and formatting in terminal.
+Collection of color codes and names for 256 color terminal setups.
+The following is a list of 256 colors for Xterm, containing an example
+of the displayed color, Xterm Name, Xterm Number and HEX.
+
+.. image:: https://gitlab.com/dslackw/images/raw/master/colored/logo.png
+    :target: https://gitlab.com/dslackw/colored
+
+`[CHANGELOG] <https://gitlab.com/dslackw/colored/blob/master/CHANGES.md>`_
+
+Video Demo
+----------
+
+.. image:: https://gitlab.com/dslackw/images/raw/master/colored/video.png
+    :target: https://asciinema.org/a/bgxm6KisSvPkPwMsYLyBBJjth
+
+The following colors works with most terminals and terminals emulators.
+ANSI/VT100 escape sequences can be used in every programming languages.
+
+Attributes:
+
+.. code-block:: bash
+
+    +-----+------------------+
+    |Code | Description      |
+    +-----+------------------+
+    |  1  | bold             |
+    |  2  | dim              |
+    |  4  | underlined       |
+    |  5  | blink            |
+    |  7  | reverse          |
+    |  8  | hidden           |
+    |  0  | reset            |
+    |  21 | res_bold         |
+    |  22 | res_dim          |
+    |  24 | res_underlined   |
+    |  25 | res_blink        |
+    |  27 | res_reverse      |
+    |  28 | res_hidden       |
+    +------------------------+
+
+
+256 Foreground and Background Colors - Full Chart:
+
+.. code-block:: bash
+
+    +-----+---------------------+
+    |Code | Description         |
+    +-----+---------------------+
+    | 0   | black               |
+    | 1   | red                 |
+    | 2   | green               |
+    | 3   | yellow              |
+    | 4   | blue                |
+    | 5   | magenta             |
+    | 6   | cyan                |
+    | 7   | light_gray          |
+    | 8   | dark_gray           |
+    | 9   | light_red           |
+    | 10  | light_green         |
+    | 11  | light_yellow        |
+    | 12  | light_blue          |
+    | 13  | light_magenta       |
+    | 14  | light_cyan          |
+    | 15  | white               |
+    | 16  | grey_0              |
+    | 17  | navy_blue           |
+    | 18  | dark_blue           |
+    | 19  | blue_3a             |
+    | 20  | blue_3b             |
+    | 21  | blue_1              |
+    | 22  | dark_green          |
+    | 23  | deep_sky_blue_4a    |
+    | 24  | deep_sky_blue_4b    |
+    | 25  | deep_sky_blue_4c    |
+    | 26  | dodger_blue_3       |
+    | 27  | dodger_blue_2       |
+    | 28  | green_4             |
+    | 29  | spring_green_4      |
+    | 30  | turquoise_4         |
+    | 31  | deep_sky_blue_3a    |
+    | 32  | deep_sky_blue_3b    |
+    | 33  | dodger_blue_1       |
+    | 34  | green_3a            |
+    | 35  | spring_green_3a     |
+    | 36  | dark_cyan           |
+    | 37  | light_sea_green     |
+    | 38  | deep_sky_blue_2     |
+    | 39  | deep_sky_blue_1     |
+    | 40  | green_3b            |
+    | 41  | spring_green_3b     |
+    | 42  | spring_green_2a     |
+    | 43  | cyan_3              |
+    | 44  | dark_turquoise      |
+    | 45  | turquoise_2         |
+    | 46  | green_1             |
+    | 47  | spring_green_2b     |
+    | 48  | spring_green_1      |
+    | 49  | medium_spring_green |
+    | 50  | cyan_2              |
+    | 51  | cyan_1              |
+    | 52  | dark_red_1          |
+    | 53  | deep_pink_4a        |
+    | 54  | purple_4a           |
+    | 55  | purple_4b           |
+    | 56  | purple_3            |
+    | 57  | blue_violet         |
+    | 58  | orange_4a           |
+    | 59  | grey_37             |
+    | 60  | medium_purple_4     |
+    | 61  | slate_blue_3a       |
+    | 62  | slate_blue_3b       |
+    | 63  | royal_blue_1        |
+    | 64  | chartreuse_4        |
+    | 65  | dark_sea_green_4a   |
+    | 66  | pale_turquoise_4    |
+    | 67  | steel_blue          |
+    | 68  | steel_blue_3        |
+    | 69  | cornflower_blue     |
+    | 70  | chartreuse_3a       |
+    | 71  | dark_sea_green_4b   |
+    | 72  | cadet_blue_2        |
+    | 73  | cadet_blue_1        |
+    | 74  | sky_blue_3          |
+    | 75  | steel_blue_1a       |
+    | 76  | chartreuse_3b       |
+    | 77  | pale_green_3a       |
+    | 78  | sea_green_3         |
+    | 79  | aquamarine_3        |
+    | 80  | medium_turquoise    |
+    | 81  | steel_blue_1b       |
+    | 82  | chartreuse_2a       |
+    | 83  | sea_green_2         |
+    | 84  | sea_green_1a        |
+    | 85  | sea_green_1b        |
+    | 86  | aquamarine_1a       |
+    | 87  | dark_slate_gray_2   |
+    | 88  | dark_red_2          |
+    | 89  | deep_pink_4b        |
+    | 90  | dark_magenta_1      |
+    | 91  | dark_magenta_2      |
+    | 92  | dark_violet_1a      |
+    | 93  | purple_1a           |
+    | 94  | orange_4b           |
+    | 95  | light_pink_4        |
+    | 96  | plum_4              |
+    | 97  | medium_purple_3a    |
+    | 98  | medium_purple_3b    |
+    | 99  | slate_blue_1        |
+    | 100 | yellow_4a           |
+    | 101 | wheat_4             |
+    | 102 | grey_53             |
+    | 103 | light_slate_grey    |
+    | 104 | medium_purple       |
+    | 105 | light_slate_blue    |
+    | 106 | yellow_4b           |
+    | 107 | dark_olive_green_3a |
+    | 108 | dark_green_sea      |
+    | 109 | light_sky_blue_3a   |
+    | 110 | light_sky_blue_3b   |
+    | 111 | sky_blue_2          |
+    | 112 | chartreuse_2b       |
+    | 113 | dark_olive_green_3b |
+    | 114 | pale_green_3b       |
+    | 115 | dark_sea_green_3a   |
+    | 116 | dark_slate_gray_3   |
+    | 117 | sky_blue_1          |
+    | 118 | chartreuse_1        |
+    | 119 | light_green_2       |
+    | 120 | light_green_3       |
+    | 121 | pale_green_1a       |
+    | 122 | aquamarine_1b       |
+    | 123 | dark_slate_gray_1   |
+    | 124 | red_3a              |
+    | 125 | deep_pink_4c        |
+    | 126 | medium_violet_red   |
+    | 127 | magenta_3a          |
+    | 128 | dark_violet_1b      |
+    | 129 | purple_1b           |
+    | 130 | dark_orange_3a      |
+    | 131 | indian_red_1a       |
+    | 132 | hot_pink_3a         |
+    | 133 | medium_orchid_3     |
+    | 134 | medium_orchid       |
+    | 135 | medium_purple_2a    |
+    | 136 | dark_goldenrod      |
+    | 137 | light_salmon_3a     |
+    | 138 | rosy_brown          |
+    | 139 | grey_63             |
+    | 140 | medium_purple_2b    |
+    | 141 | medium_purple_1     |
+    | 142 | gold_3a             |
+    | 143 | dark_khaki          |
+    | 144 | navajo_white_3      |
+    | 145 | grey_69             |
+    | 146 | light_steel_blue_3  |
+    | 147 | light_steel_blue    |
+    | 148 | yellow_3a           |
+    | 149 | dark_olive_green_3  |
+    | 150 | dark_sea_green_3b   |
+    | 151 | dark_sea_green_2    |
+    | 152 | light_cyan_3        |
+    | 153 | light_sky_blue_1    |
+    | 154 | green_yellow        |
+    | 155 | dark_olive_green_2  |
+    | 156 | pale_green_1b       |
+    | 157 | dark_sea_green_5b   |
+    | 158 | dark_sea_green_5a   |
+    | 159 | pale_turquoise_1    |
+    | 160 | red_3b              |
+    | 161 | deep_pink_3a        |
+    | 162 | deep_pink_3b        |
+    | 163 | magenta_3b          |
+    | 164 | magenta_3c          |
+    | 165 | magenta_2a          |
+    | 166 | dark_orange_3b      |
+    | 167 | indian_red_1b       |
+    | 168 | hot_pink_3b         |
+    | 169 | hot_pink_2          |
+    | 170 | orchid              |
+    | 171 | medium_orchid_1a    |
+    | 172 | orange_3            |
+    | 173 | light_salmon_3b     |
+    | 174 | light_pink_3        |
+    | 175 | pink_3              |
+    | 176 | plum_3              |
+    | 177 | violet              |
+    | 178 | gold_3b             |
+    | 179 | light_goldenrod_3   |
+    | 180 | tan                 |
+    | 181 | misty_rose_3        |
+    | 182 | thistle_3           |
+    | 183 | plum_2              |
+    | 184 | yellow_3b           |
+    | 185 | khaki_3             |
+    | 186 | light_goldenrod_2a  |
+    | 187 | light_yellow_3      |
+    | 188 | grey_84             |
+    | 189 | light_steel_blue_1  |
+    | 190 | yellow_2            |
+    | 191 | dark_olive_green_1a |
+    | 192 | dark_olive_green_1b |
+    | 193 | dark_sea_green_1    |
+    | 194 | honeydew_2          |
+    | 195 | light_cyan_1        |
+    | 196 | red_1               |
+    | 197 | deep_pink_2         |
+    | 198 | deep_pink_1a        |
+    | 199 | deep_pink_1b        |
+    | 200 | magenta_2b          |
+    | 201 | magenta_1           |
+    | 202 | orange_red_1        |
+    | 203 | indian_red_1c       |
+    | 204 | indian_red_1d       |
+    | 205 | hot_pink_1a         |
+    | 206 | hot_pink_1b         |
+    | 207 | medium_orchid_1b    |
+    | 208 | dark_orange         |
+    | 209 | salmon_1            |
+    | 210 | light_coral         |
+    | 211 | pale_violet_red_1   |
+    | 212 | orchid_2            |
+    | 213 | orchid_1            |
+    | 214 | orange_1            |
+    | 215 | sandy_brown         |
+    | 216 | light_salmon_1      |
+    | 217 | light_pink_1        |
+    | 218 | pink_1              |
+    | 219 | plum_1              |
+    | 220 | gold_1              |
+    | 221 | light_goldenrod_2b  |
+    | 222 | light_goldenrod_2c  |
+    | 223 | navajo_white_1      |
+    | 224 | misty_rose1         |
+    | 225 | thistle_1           |
+    | 226 | yellow_1            |
+    | 227 | light_goldenrod_1   |
+    | 228 | khaki_1             |
+    | 229 | wheat_1             |
+    | 230 | cornsilk_1          |
+    | 231 | grey_100            |
+    | 232 | grey_3              |
+    | 233 | grey_7              |
+    | 234 | grey_11             |
+    | 235 | grey_15             |
+    | 236 | grey_19             |
+    | 237 | grey_23             |
+    | 238 | grey_27             |
+    | 239 | grey_30             |
+    | 240 | grey_35             |
+    | 241 | grey_39             |
+    | 242 | grey_42             |
+    | 243 | grey_46             |
+    | 244 | grey_50             |
+    | 245 | grey_54             |
+    | 246 | grey_58             |
+    | 247 | grey_62             |
+    | 248 | grey_66             |
+    | 249 | grey_70             |
+    | 250 | grey_74             |
+    | 251 | grey_78             |
+    | 252 | grey_82             |
+    | 253 | grey_85             |
+    | 254 | grey_89             |
+    | 255 | grey_93             |
+    | 256 | default             |
+    +-----+---------------------+
+
+256 Colors Foreground (text):
+
+.. image:: https://gitlab.com/dslackw/images/raw/master/colored/256_colors_fg.png
+    :alt: 256 fg colors
+
+256 Colors Background:
+
+.. image:: https://gitlab.com/dslackw/images/raw/master/colored/256_colors_bg.png
+    :alt: 256 bg colors
+
+
+Installation
+------------
+
+.. code-block:: bash
+
+    $ pip install colored --upgrade
+
+    uninstall
+
+    $ pip uninstall colored
+
+
+Dependencies
+------------
+
+None, only Python programming language.
+
+Usage Examples
+--------------
+
+How to use the module in your own python code:
+
+.. code-block:: bash
+
+    >>> from colored import fg, bg, attr
+    >>>
+    >>> print(f'{fg(1)} Hello World !!! {attr(0)}')
+     Hello World !!!
+    >>>
+    >>> print(f'{fg(1)}{bg(15)} Hello World !!! {attr(0)}')
+     Hello World !!!
+
+Use description:
+
+.. code-block:: bash
+
+    >>> print(f'{fg("white")}{bg("yellow")} Hello World !!! {attr("reset")}')
+     Hello World !!!
+    >>>
+    >>> print(f'{fg("orchid")}{attr("bold")} Hello World !!! {attr("reset")}')
+     Hello World !!!
+    >>>
+    >>> color = bg('indian_red_1a') + fg('white')
+    >>> reset = attr('reset')
+    >>> print(color + 'Hello World !!!' + reset)
+    Hello World !!!
+
+Or use HEX code:
+
+.. code-block:: bash
+
+    >>> color = fg('#C0C0C0') + bg('#00005f')
+    >>> res = attr('reset')
+    >>> print(color + "Hello World !!!" + res)
+    Hello World !!!
+
+Or the convenient `stylize(text, *styles)` wrapper to save some keystrokes:
+
+.. code-block:: bash
+
+    >>> import colored
+    >>> from colored import stylize
+    >>> print(stylize("This is green.", colored.fg("green")))
+    This is green.
+    >>> print("This is not.")
+    This is not.
+    >>> angry = colored.fg("red") + colored.attr("bold")
+    >>> print(stylize("This is angry text.", angry))
+    This is angry text.
+    >>> print(stylize("This is VERY angry text.", angry, colored.attr("underlined")))
+    This is VERY angry text.
+    >>> print("But this is not.")
+    But this is not.
+
+Or the variant `stylize_interactive(text, *styles)` for readline-friendliness:
+
+.. code-block:: bash
+
+    >>> import colored, sys
+    >>> from colored import stylize_interactive, fg
+    >>> sys.ps1 = stylize_interactive("myPrompt: ", fg('red'))
+    myPrompt:
+
+Use directly like `colorama <https://pypi.python.org/pypi/colorama>`_ but with more colors:
+
+.. code-block:: bash
+
+    >>> from colored import fore, back, style
+    >>>
+    >>> print(fore.LIGHT_BLUE + back.RED + style.BOLD + "Hello World !!!" + style.RESET)
+
+Import colored module:
+
+.. code-block:: bash
+
+   >>> import colored
+   >>>
+   >>> colored.fg(1)
+   '\x1b[38;5;1m'
+   >>>
+   >>> colored.fg(257)
+   Traceback (most recent call last):
+     File "<input>", line 1, in <module>
+     File "/usr/lib64/python2.7/site-packages/colored/colored.py", line 381, in fg
+       return colored(color).foreground()
+     File "/usr/lib64/python2.7/site-packages/colored/colored.py", line 350, in foreground
+       color = self.reserve_paint[str(self.color)]
+   KeyError: '257'
+   >>>
+   >>> colored.bg(30)
+   '\x1b[48;5;30m'
+   >>>
+   >>> colored.fore.BLUE
+   '\x1b[38;5;4m'
+
+    etc.
+
+
+Screenshot:
+
+.. image:: https://gitlab.com/dslackw/images/raw/master/colored/screenshot-2.png
+    :alt: example
+
+
```

### Comparing `colored-1.4.3/README.rst` & `colored-1.4.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Collection of color codes and names for 256 color terminal setups.
 The following is a list of 256 colors for Xterm, containing an example
 of the displayed color, Xterm Name, Xterm Number and HEX.
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/colored/logo.png
     :target: https://gitlab.com/dslackw/colored
 
-`[CHANGELOG] <https://gitlab.com/dslackw/colored/blob/master/CHANGELOG>`_
+`[CHANGELOG] <https://gitlab.com/dslackw/colored/blob/master/CHANGES.md>`_
 
 Video Demo
 ----------
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/colored/video.png
     :target: https://asciinema.org/a/bgxm6KisSvPkPwMsYLyBBJjth
 
@@ -339,42 +339,42 @@
 
 How to use the module in your own python code:
 
 .. code-block:: bash
 
     >>> from colored import fg, bg, attr
     >>>
-    >>> print ('%s Hello World !!! %s' % (fg(1), attr(0)))
+    >>> print(f'{fg(1)} Hello World !!! {attr(0)}')
      Hello World !!!
     >>>
-    >>> print ('%s%s Hello World !!! %s' % (fg(1), bg(15), attr(0)))
+    >>> print(f'{fg(1)}{bg(15)} Hello World !!! {attr(0)}')
      Hello World !!!
 
 Use description:
 
 .. code-block:: bash
 
-    >>> print ('%s%s Hello World !!! %s' % (fg('white'), bg('yellow'), attr('reset')))
+    >>> print(f'{fg("white")}{bg("yellow")} Hello World !!! {attr("reset")}')
      Hello World !!!
     >>>
-    >>> print ('%s%s Hello World !!! %s' % (fg('orchid'), attr('bold'), attr('reset')))
+    >>> print(f'{fg("orchid")}{attr("bold")} Hello World !!! {attr("reset")}')
      Hello World !!!
     >>>
     >>> color = bg('indian_red_1a') + fg('white')
     >>> reset = attr('reset')
-    >>> print (color + 'Hello World !!!' + reset)
+    >>> print(color + 'Hello World !!!' + reset)
     Hello World !!!
 
 Or use HEX code:
 
 .. code-block:: bash
 
     >>> color = fg('#C0C0C0') + bg('#00005f')
     >>> res = attr('reset')
-    >>> print (color + "Hello World !!!" + res)
+    >>> print(color + "Hello World !!!" + res)
     Hello World !!!
 
 Or the convenient `stylize(text, *styles)` wrapper to save some keystrokes:
 
 .. code-block:: bash
 
     >>> import colored
@@ -402,15 +402,15 @@
 
 Use directly like `colorama <https://pypi.python.org/pypi/colorama>`_ but with more colors:
 
 .. code-block:: bash
 
     >>> from colored import fore, back, style
     >>>
-    >>> print (fore.LIGHT_BLUE + back.RED + style.BOLD + "Hello World !!!" + style.RESET)
+    >>> print(fore.LIGHT_BLUE + back.RED + style.BOLD + "Hello World !!!" + style.RESET)
 
 Import colored module:
 
 .. code-block:: bash
 
    >>> import colored
    >>>
```

### Comparing `colored-1.4.3/colored/colored.py` & `colored-1.4.4/colored/colored.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,458 +9,460 @@
 
 
 TTY_AWARE = True
 IS_TTY = sys.stdout.isatty() and sys.stderr.isatty()
 
 _win_vterm_mode = None
 
-class colored(object):
+
+class colored:
 
     def __init__(self, color):
 
-        self.ESC = "\x1b["
-        self.END = "m"
+        self.ESC = '\x1b['
+        self.END = 'm'
         self.color = color
         self.enable_windows_terminal_mode()
 
-        if str(color).startswith("#"):
+        if str(color).startswith('#'):
             self.HEX = HEX(color.lower())
         else:
-            self.HEX = ""
+            self.HEX = ''
 
         self.paint = {
-            "black": "0",
-            "red": "1",
-            "green": "2",
-            "yellow": "3",
-            "blue": "4",
-            "magenta": "5",
-            "cyan": "6",
-            "light_gray": "7",
-            "dark_gray": "8",
-            "light_red": "9",
-            "light_green": "10",
-            "light_yellow": "11",
-            "light_blue": "12",
-            "light_magenta": "13",
-            "light_cyan": "14",
-            "white": "15",
-            "grey_0": "16",
-            "navy_blue": "17",
-            "dark_blue": "18",
-            "blue_3a": "19",
-            "blue_3b": "20",
-            "blue_1": "21",
-            "dark_green": "22",
-            "deep_sky_blue_4a": "23",
-            "deep_sky_blue_4b": "24",
-            "deep_sky_blue_4c": "25",
-            "dodger_blue_3": "26",
-            "dodger_blue_2": "27",
-            "green_4": "28",
-            "spring_green_4": "29",
-            "turquoise_4": "30",
-            "deep_sky_blue_3a": "31",
-            "deep_sky_blue_3b": "32",
-            "dodger_blue_1": "33",
-            "green_3a": "34",
-            "spring_green_3a": "35",
-            "dark_cyan": "36",
-            "light_sea_green": "37",
-            "deep_sky_blue_2": "38",
-            "deep_sky_blue_1": "39",
-            "green_3b": "40",
-            "spring_green_3b": "41",
-            "spring_green_2a": "42",
-            "cyan_3": "43",
-            "dark_turquoise": "44",
-            "turquoise_2": "45",
-            "green_1": "46",
-            "spring_green_2b": "47",
-            "spring_green_1": "48",
-            "medium_spring_green": "49",
-            "cyan_2": "50",
-            "cyan_1": "51",
-            "dark_red_1": "52",
-            "deep_pink_4a": "53",
-            "purple_4a": "54",
-            "purple_4b": "55",
-            "purple_3": "56",
-            "blue_violet": "57",
-            "orange_4a": "58",
-            "grey_37": "59",
-            "medium_purple_4": "60",
-            "slate_blue_3a": "61",
-            "slate_blue_3b": "62",
-            "royal_blue_1": "63",
-            "chartreuse_4": "64",
-            "dark_sea_green_4a": "65",
-            "pale_turquoise_4": "66",
-            "steel_blue": "67",
-            "steel_blue_3": "68",
-            "cornflower_blue": "69",
-            "chartreuse_3a": "70",
-            "dark_sea_green_4b": "71",
-            "cadet_blue_2": "72",
-            "cadet_blue_1": "73",
-            "sky_blue_3": "74",
-            "steel_blue_1a": "75",
-            "chartreuse_3b": "76",
-            "pale_green_3a": "77",
-            "sea_green_3": "78",
-            "aquamarine_3": "79",
-            "medium_turquoise": "80",
-            "steel_blue_1b": "81",
-            "chartreuse_2a": "82",
-            "sea_green_2": "83",
-            "sea_green_1a": "84",
-            "sea_green_1b": "85",
-            "aquamarine_1a": "86",
-            "dark_slate_gray_2": "87",
-            "dark_red_2": "88",
-            "deep_pink_4b": "89",
-            "dark_magenta_1": "90",
-            "dark_magenta_2": "91",
-            "dark_violet_1a": "92",
-            "purple_1a": "93",
-            "orange_4b": "94",
-            "light_pink_4": "95",
-            "plum_4": "96",
-            "medium_purple_3a": "97",
-            "medium_purple_3b": "98",
-            "slate_blue_1": "99",
-            "yellow_4a": "100",
-            "wheat_4": "101",
-            "grey_53": "102",
-            "light_slate_grey": "103",
-            "medium_purple": "104",
-            "light_slate_blue": "105",
-            "yellow_4b": "106",
-            "dark_olive_green_3a": "107",
-            "dark_green_sea": "108",
-            "light_sky_blue_3a": "109",
-            "light_sky_blue_3b": "110",
-            "sky_blue_2": "111",
-            "chartreuse_2b": "112",
-            "dark_olive_green_3b": "113",
-            "pale_green_3b": "114",
-            "dark_sea_green_3a": "115",
-            "dark_slate_gray_3": "116",
-            "sky_blue_1": "117",
-            "chartreuse_1": "118",
-            "light_green_2": "119",
-            "light_green_3": "120",
-            "pale_green_1a": "121",
-            "aquamarine_1b": "122",
-            "dark_slate_gray_1": "123",
-            "red_3a": "124",
-            "deep_pink_4c": "125",
-            "medium_violet_red": "126",
-            "magenta_3a": "127",
-            "dark_violet_1b": "128",
-            "purple_1b": "129",
-            "dark_orange_3a": "130",
-            "indian_red_1a": "131",
-            "hot_pink_3a": "132",
-            "medium_orchid_3": "133",
-            "medium_orchid": "134",
-            "medium_purple_2a": "135",
-            "dark_goldenrod": "136",
-            "light_salmon_3a": "137",
-            "rosy_brown": "138",
-            "grey_63": "139",
-            "medium_purple_2b": "140",
-            "medium_purple_1": "141",
-            "gold_3a": "142",
-            "dark_khaki": "143",
-            "navajo_white_3": "144",
-            "grey_69": "145",
-            "light_steel_blue_3": "146",
-            "light_steel_blue": "147",
-            "yellow_3a": "148",
-            "dark_olive_green_3": "149",
-            "dark_sea_green_3b": "150",
-            "dark_sea_green_2": "151",
-            "light_cyan_3": "152",
-            "light_sky_blue_1": "153",
-            "green_yellow": "154",
-            "dark_olive_green_2": "155",
-            "pale_green_1b": "156",
-            "dark_sea_green_5b": "157",
-            "dark_sea_green_5a": "158",
-            "pale_turquoise_1": "159",
-            "red_3b": "160",
-            "deep_pink_3a": "161",
-            "deep_pink_3b": "162",
-            "magenta_3b": "163",
-            "magenta_3c": "164",
-            "magenta_2a": "165",
-            "dark_orange_3b": "166",
-            "indian_red_1b": "167",
-            "hot_pink_3b": "168",
-            "hot_pink_2": "169",
-            "orchid": "170",
-            "medium_orchid_1a": "171",
-            "orange_3": "172",
-            "light_salmon_3b": "173",
-            "light_pink_3": "174",
-            "pink_3": "175",
-            "plum_3": "176",
-            "violet": "177",
-            "gold_3b": "178",
-            "light_goldenrod_3": "179",
-            "tan": "180",
-            "misty_rose_3": "181",
-            "thistle_3": "182",
-            "plum_2": "183",
-            "yellow_3b": "184",
-            "khaki_3": "185",
-            "light_goldenrod_2a": "186",
-            "light_yellow_3": "187",
-            "grey_84": "188",
-            "light_steel_blue_1": "189",
-            "yellow_2": "190",
-            "dark_olive_green_1a": "191",
-            "dark_olive_green_1b": "192",
-            "dark_sea_green_1": "193",
-            "honeydew_2": "194",
-            "light_cyan_1": "195",
-            "red_1": "196",
-            "deep_pink_2": "197",
-            "deep_pink_1a": "198",
-            "deep_pink_1b": "199",
-            "magenta_2b": "200",
-            "magenta_1": "201",
-            "orange_red_1": "202",
-            "indian_red_1c": "203",
-            "indian_red_1d": "204",
-            "hot_pink_1a": "205",
-            "hot_pink_1b": "206",
-            "medium_orchid_1b": "207",
-            "dark_orange": "208",
-            "salmon_1": "209",
-            "light_coral": "210",
-            "pale_violet_red_1": "211",
-            "orchid_2": "212",
-            "orchid_1": "213",
-            "orange_1": "214",
-            "sandy_brown": "215",
-            "light_salmon_1": "216",
-            "light_pink_1": "217",
-            "pink_1": "218",
-            "plum_1": "219",
-            "gold_1": "220",
-            "light_goldenrod_2b": "221",
-            "light_goldenrod_2c": "222",
-            "navajo_white_1": "223",
-            "misty_rose1": "224",
-            "thistle_1": "225",
-            "yellow_1": "226",
-            "light_goldenrod_1": "227",
-            "khaki_1": "228",
-            "wheat_1": "229",
-            "cornsilk_1": "230",
-            "grey_100": "231",
-            "grey_3": "232",
-            "grey_7": "233",
-            "grey_11": "234",
-            "grey_15": "235",
-            "grey_19": "236",
-            "grey_23": "237",
-            "grey_27": "238",
-            "grey_30": "239",
-            "grey_35": "240",
-            "grey_39": "241",
-            "grey_42": "242",
-            "grey_46": "243",
-            "grey_50": "244",
-            "grey_54": "245",
-            "grey_58": "246",
-            "grey_62": "247",
-            "grey_66": "248",
-            "grey_70": "249",
-            "grey_74": "250",
-            "grey_78": "251",
-            "grey_82": "252",
-            "grey_85": "253",
-            "grey_89": "254",
-            "grey_93": "255",
+            'black': '0',
+            'red': '1',
+            'green': '2',
+            'yellow': '3',
+            'blue': '4',
+            'magenta': '5',
+            'cyan': '6',
+            'light_gray': '7',
+            'dark_gray': '8',
+            'light_red': '9',
+            'light_green': '10',
+            'light_yellow': '11',
+            'light_blue': '12',
+            'light_magenta': '13',
+            'light_cyan': '14',
+            'white': '15',
+            'grey_0': '16',
+            'navy_blue': '17',
+            'dark_blue': '18',
+            'blue_3a': '19',
+            'blue_3b': '20',
+            'blue_1': '21',
+            'dark_green': '22',
+            'deep_sky_blue_4a': '23',
+            'deep_sky_blue_4b': '24',
+            'deep_sky_blue_4c': '25',
+            'dodger_blue_3': '26',
+            'dodger_blue_2': '27',
+            'green_4': '28',
+            'spring_green_4': '29',
+            'turquoise_4': '30',
+            'deep_sky_blue_3a': '31',
+            'deep_sky_blue_3b': '32',
+            'dodger_blue_1': '33',
+            'green_3a': '34',
+            'spring_green_3a': '35',
+            'dark_cyan': '36',
+            'light_sea_green': '37',
+            'deep_sky_blue_2': '38',
+            'deep_sky_blue_1': '39',
+            'green_3b': '40',
+            'spring_green_3b': '41',
+            'spring_green_2a': '42',
+            'cyan_3': '43',
+            'dark_turquoise': '44',
+            'turquoise_2': '45',
+            'green_1': '46',
+            'spring_green_2b': '47',
+            'spring_green_1': '48',
+            'medium_spring_green': '49',
+            'cyan_2': '50',
+            'cyan_1': '51',
+            'dark_red_1': '52',
+            'deep_pink_4a': '53',
+            'purple_4a': '54',
+            'purple_4b': '55',
+            'purple_3': '56',
+            'blue_violet': '57',
+            'orange_4a': '58',
+            'grey_37': '59',
+            'medium_purple_4': '60',
+            'slate_blue_3a': '61',
+            'slate_blue_3b': '62',
+            'royal_blue_1': '63',
+            'chartreuse_4': '64',
+            'dark_sea_green_4a': '65',
+            'pale_turquoise_4': '66',
+            'steel_blue': '67',
+            'steel_blue_3': '68',
+            'cornflower_blue': '69',
+            'chartreuse_3a': '70',
+            'dark_sea_green_4b': '71',
+            'cadet_blue_2': '72',
+            'cadet_blue_1': '73',
+            'sky_blue_3': '74',
+            'steel_blue_1a': '75',
+            'chartreuse_3b': '76',
+            'pale_green_3a': '77',
+            'sea_green_3': '78',
+            'aquamarine_3': '79',
+            'medium_turquoise': '80',
+            'steel_blue_1b': '81',
+            'chartreuse_2a': '82',
+            'sea_green_2': '83',
+            'sea_green_1a': '84',
+            'sea_green_1b': '85',
+            'aquamarine_1a': '86',
+            'dark_slate_gray_2': '87',
+            'dark_red_2': '88',
+            'deep_pink_4b': '89',
+            'dark_magenta_1': '90',
+            'dark_magenta_2': '91',
+            'dark_violet_1a': '92',
+            'purple_1a': '93',
+            'orange_4b': '94',
+            'light_pink_4': '95',
+            'plum_4': '96',
+            'medium_purple_3a': '97',
+            'medium_purple_3b': '98',
+            'slate_blue_1': '99',
+            'yellow_4a': '100',
+            'wheat_4': '101',
+            'grey_53': '102',
+            'light_slate_grey': '103',
+            'medium_purple': '104',
+            'light_slate_blue': '105',
+            'yellow_4b': '106',
+            'dark_olive_green_3a': '107',
+            'dark_green_sea': '108',
+            'light_sky_blue_3a': '109',
+            'light_sky_blue_3b': '110',
+            'sky_blue_2': '111',
+            'chartreuse_2b': '112',
+            'dark_olive_green_3b': '113',
+            'pale_green_3b': '114',
+            'dark_sea_green_3a': '115',
+            'dark_slate_gray_3': '116',
+            'sky_blue_1': '117',
+            'chartreuse_1': '118',
+            'light_green_2': '119',
+            'light_green_3': '120',
+            'pale_green_1a': '121',
+            'aquamarine_1b': '122',
+            'dark_slate_gray_1': '123',
+            'red_3a': '124',
+            'deep_pink_4c': '125',
+            'medium_violet_red': '126',
+            'magenta_3a': '127',
+            'dark_violet_1b': '128',
+            'purple_1b': '129',
+            'dark_orange_3a': '130',
+            'indian_red_1a': '131',
+            'hot_pink_3a': '132',
+            'medium_orchid_3': '133',
+            'medium_orchid': '134',
+            'medium_purple_2a': '135',
+            'dark_goldenrod': '136',
+            'light_salmon_3a': '137',
+            'rosy_brown': '138',
+            'grey_63': '139',
+            'medium_purple_2b': '140',
+            'medium_purple_1': '141',
+            'gold_3a': '142',
+            'dark_khaki': '143',
+            'navajo_white_3': '144',
+            'grey_69': '145',
+            'light_steel_blue_3': '146',
+            'light_steel_blue': '147',
+            'yellow_3a': '148',
+            'dark_olive_green_3': '149',
+            'dark_sea_green_3b': '150',
+            'dark_sea_green_2': '151',
+            'light_cyan_3': '152',
+            'light_sky_blue_1': '153',
+            'green_yellow': '154',
+            'dark_olive_green_2': '155',
+            'pale_green_1b': '156',
+            'dark_sea_green_5b': '157',
+            'dark_sea_green_5a': '158',
+            'pale_turquoise_1': '159',
+            'red_3b': '160',
+            'deep_pink_3a': '161',
+            'deep_pink_3b': '162',
+            'magenta_3b': '163',
+            'magenta_3c': '164',
+            'magenta_2a': '165',
+            'dark_orange_3b': '166',
+            'indian_red_1b': '167',
+            'hot_pink_3b': '168',
+            'hot_pink_2': '169',
+            'orchid': '170',
+            'medium_orchid_1a': '171',
+            'orange_3': '172',
+            'light_salmon_3b': '173',
+            'light_pink_3': '174',
+            'pink_3': '175',
+            'plum_3': '176',
+            'violet': '177',
+            'gold_3b': '178',
+            'light_goldenrod_3': '179',
+            'tan': '180',
+            'misty_rose_3': '181',
+            'thistle_3': '182',
+            'plum_2': '183',
+            'yellow_3b': '184',
+            'khaki_3': '185',
+            'light_goldenrod_2a': '186',
+            'light_yellow_3': '187',
+            'grey_84': '188',
+            'light_steel_blue_1': '189',
+            'yellow_2': '190',
+            'dark_olive_green_1a': '191',
+            'dark_olive_green_1b': '192',
+            'dark_sea_green_1': '193',
+            'honeydew_2': '194',
+            'light_cyan_1': '195',
+            'red_1': '196',
+            'deep_pink_2': '197',
+            'deep_pink_1a': '198',
+            'deep_pink_1b': '199',
+            'magenta_2b': '200',
+            'magenta_1': '201',
+            'orange_red_1': '202',
+            'indian_red_1c': '203',
+            'indian_red_1d': '204',
+            'hot_pink_1a': '205',
+            'hot_pink_1b': '206',
+            'medium_orchid_1b': '207',
+            'dark_orange': '208',
+            'salmon_1': '209',
+            'light_coral': '210',
+            'pale_violet_red_1': '211',
+            'orchid_2': '212',
+            'orchid_1': '213',
+            'orange_1': '214',
+            'sandy_brown': '215',
+            'light_salmon_1': '216',
+            'light_pink_1': '217',
+            'pink_1': '218',
+            'plum_1': '219',
+            'gold_1': '220',
+            'light_goldenrod_2b': '221',
+            'light_goldenrod_2c': '222',
+            'navajo_white_1': '223',
+            'misty_rose1': '224',
+            'thistle_1': '225',
+            'yellow_1': '226',
+            'light_goldenrod_1': '227',
+            'khaki_1': '228',
+            'wheat_1': '229',
+            'cornsilk_1': '230',
+            'grey_100': '231',
+            'grey_3': '232',
+            'grey_7': '233',
+            'grey_11': '234',
+            'grey_15': '235',
+            'grey_19': '236',
+            'grey_23': '237',
+            'grey_27': '238',
+            'grey_30': '239',
+            'grey_35': '240',
+            'grey_39': '241',
+            'grey_42': '242',
+            'grey_46': '243',
+            'grey_50': '244',
+            'grey_54': '245',
+            'grey_58': '246',
+            'grey_62': '247',
+            'grey_66': '248',
+            'grey_70': '249',
+            'grey_74': '250',
+            'grey_78': '251',
+            'grey_82': '252',
+            'grey_85': '253',
+            'grey_89': '254',
+            'grey_93': '255',
         }
 
     def attribute(self):
-        """Set or reset attributes"""
+        '''Set or reset attributes'''
         if not self.enabled():
-            return ""
+            return ''
 
         paint = {
-            "bold": self.ESC + "1" + self.END,
-            1: self.ESC + "1" + self.END,
-            "dim": self.ESC + "2" + self.END,
-            2: self.ESC + "2" + self.END,
-            "underlined": self.ESC + "4" + self.END,
-            4: self.ESC + "4" + self.END,
-            "blink": self.ESC + "5" + self.END,
-            5: self.ESC + "5" + self.END,
-            "reverse": self.ESC + "7" + self.END,
-            7: self.ESC + "7" + self.END,
-            "hidden": self.ESC + "8" + self.END,
-            8: self.ESC + "8" + self.END,
-            "reset": self.ESC + "0" + self.END,
-            0: self.ESC + "0" + self.END,
-            "res_bold": self.ESC + "21" + self.END,
-            21: self.ESC + "21" + self.END,
-            "res_dim": self.ESC + "22" + self.END,
-            22: self.ESC + "22" + self.END,
-            "res_underlined": self.ESC + "24" + self.END,
-            24: self.ESC + "24" + self.END,
-            "res_blink": self.ESC + "25" + self.END,
-            25: self.ESC + "25" + self.END,
-            "res_reverse": self.ESC + "27" + self.END,
-            27: self.ESC + "27" + self.END,
-            "res_hidden": self.ESC + "28" + self.END,
-            28: self.ESC + "28" + self.END,
+            'bold': self.ESC + '1' + self.END,
+            1: self.ESC + '1' + self.END,
+            'dim': self.ESC + '2' + self.END,
+            2: self.ESC + '2' + self.END,
+            'underlined': self.ESC + '4' + self.END,
+            4: self.ESC + '4' + self.END,
+            'blink': self.ESC + '5' + self.END,
+            5: self.ESC + '5' + self.END,
+            'reverse': self.ESC + '7' + self.END,
+            7: self.ESC + '7' + self.END,
+            'hidden': self.ESC + '8' + self.END,
+            8: self.ESC + '8' + self.END,
+            'reset': self.ESC + '0' + self.END,
+            0: self.ESC + '0' + self.END,
+            'res_bold': self.ESC + '21' + self.END,
+            21: self.ESC + '21' + self.END,
+            'res_dim': self.ESC + '22' + self.END,
+            22: self.ESC + '22' + self.END,
+            'res_underlined': self.ESC + '24' + self.END,
+            24: self.ESC + '24' + self.END,
+            'res_blink': self.ESC + '25' + self.END,
+            25: self.ESC + '25' + self.END,
+            'res_reverse': self.ESC + '27' + self.END,
+            27: self.ESC + '27' + self.END,
+            'res_hidden': self.ESC + '28' + self.END,
+            28: self.ESC + '28' + self.END,
         }
         return paint[self.color]
 
     def foreground(self):
-        """Print 256 foreground colors"""
+        '''Print 256 foreground colors'''
         if not self.enabled():
-            return ""
-        code = self.ESC + "38;5;"
+            return ''
+        code = self.ESC + '38;5;'
         if str(self.color).isdigit():
             self.reverse_dict()
             color = self.reserve_paint[str(self.color)]
             return code + self.paint[color] + self.END
-        elif self.color.startswith("#"):
+        elif self.color.startswith('#'):
             return code + str(self.HEX) + self.END
         else:
             return code + self.paint[self.color] + self.END
 
     def background(self):
-        """Print 256 background colors"""
+        '''Print 256 background colors'''
         if not self.enabled():
-            return ""
-        code = self.ESC + "48;5;"
+            return ''
+        code = self.ESC + '48;5;'
         if str(self.color).isdigit():
             self.reverse_dict()
             color = self.reserve_paint[str(self.color)]
             return code + self.paint[color] + self.END
-        elif self.color.startswith("#"):
+        elif self.color.startswith('#'):
             return code + str(self.HEX) + self.END
         else:
             return code + self.paint[self.color] + self.END
 
     def reverse_dict(self):
-        """reverse dictionary"""
+        '''reverse dictionary'''
         self.reserve_paint = dict(zip(self.paint.values(), self.paint.keys()))
 
     def enable_windows_terminal_mode(self):
         '''Enable virtual terminal processing in windows terminal. Does
         nothing if not on Windows. This is based on the rejected
         enhancement <https://bugs.python.org/issue29059>.'''
         global _win_vterm_mode
-        if _win_vterm_mode != None:
+        if _win_vterm_mode is not None:
             return _win_vterm_mode
 
-        # Note: Cygwin should return something like "CYGWIN_NT..."
+        # Note: Cygwin should return something like 'CYGWIN_NT...'
         _win_vterm_mode = platform.system().lower() == 'windows'
-        if _win_vterm_mode == False:
+        if _win_vterm_mode is False:
             return
 
-        from ctypes import windll, c_int, byref, c_void_p
+        from ctypes import windll, wintypes, byref, c_void_p
         ENABLE_VIRTUAL_TERMINAL_PROCESSING = 0x0004
         INVALID_HANDLE_VALUE = c_void_p(-1).value
-        STD_OUTPUT_HANDLE = c_int(-11)
+        STD_OUTPUT_HANDLE = wintypes.DWORD(-11)
 
         hStdout = windll.kernel32.GetStdHandle(STD_OUTPUT_HANDLE)
         if hStdout == INVALID_HANDLE_VALUE:
             _win_vterm_mode = False
             return
 
-        mode = c_int(0)
-        ok = windll.kernel32.GetConsoleMode(c_int(hStdout), byref(mode))
+        mode = wintypes.DWORD(0)
+        ok = windll.kernel32.GetConsoleMode(wintypes.HANDLE(hStdout), byref(mode))
         if not ok:
             _win_vterm_mode = False
             return
 
-        mode = c_int(mode.value | ENABLE_VIRTUAL_TERMINAL_PROCESSING)
-        ok = windll.kernel32.SetConsoleMode(c_int(hStdout), mode)
+        mode = wintypes.DWORD(mode.value | ENABLE_VIRTUAL_TERMINAL_PROCESSING)
+        ok = windll.kernel32.SetConsoleMode(wintypes.HANDLE(hStdout), mode)
         if not ok:
-            # Something went wrong, proably an too old version
-            # that doesn't support the VT100 mode.
+            # Something went wrong, probably a version too old
+            # to support the VT100 mode.
             # To be more certain we could check kernel32.GetLastError
             # for STATUS_INVALID_PARAMETER, but since we only enable
             # one flag we can be certain enough.
             _win_vterm_mode = False
             return
 
     def enabled(self):
 
         # https://github.com/chalk/supports-color#info
         # Use the environment variable FORCE_COLOR=1 (level 1), FORCE_COLOR=2
         # (level 2), or FORCE_COLOR=3 (level 3) to forcefully enable color, or
         # FORCE_COLOR=0 to forcefully disable. The use of FORCE_COLOR overrides
         # all other color support checks.
-        if "FORCE_COLOR" in os.environ:
-            if int(os.environ["FORCE_COLOR"]) == 0:
+        if 'FORCE_COLOR' in os.environ:
+            if int(os.environ['FORCE_COLOR']) == 0:
                 return False
             else:
                 return True
 
         # https://no-color.org/
         # Check for the presence of a NO_COLOR environment variable that, when
         # present (regardless of its value), prevents the addition of ANSI
         # color.
-        if "NO_COLOR" in os.environ:
+        if 'NO_COLOR' in os.environ:
             return False
 
         # Also disable coloring when not printing to a TTY.
         if TTY_AWARE and not IS_TTY:
             return False
 
         # In all other cases, enable coloring.
         return True
 
 
 def attr(color):
-    """alias for colored().attribute()"""
+    '''alias for colored().attribute()'''
     return colored(color).attribute()
 
 
 def fg(color):
-    """alias for colored().foreground()"""
+    '''alias for colored().foreground()'''
     return colored(color).foreground()
 
 
 def bg(color):
-    """alias for colored().background()"""
+    '''alias for colored().background()'''
     return colored(color).background()
 
 
 def stylize(text, styles, reset=True):
-    """conveniently styles your text as and resets ANSI codes at its end."""
-    terminator = attr("reset") if reset else ""
-    return "{}{}{}".format("".join(styles), text, terminator)
+    '''conveniently styles your text as and resets ANSI codes at its end.'''
+    terminator = attr('reset') if reset else ''
+    return f'{"".join(styles)}{text}{terminator}'
 
 
 def _c0wrap(styles):
-    """wrap a set of ANSI styles in C0 control codes for readline safety."""
+    '''wrap a set of ANSI styles in C0 control codes for readline safety.'''
     C0_SOH = '\x01'   # mark the beginning of nonprinting characters
     C0_STX = '\x02'   # mark the end of nonprinting characters
-    return "{}{}{}".format(C0_SOH, "".join(styles), C0_STX)
+    return f'{C0_SOH}{"".join(styles)}{C0_STX}'
 
 
 def stylize_interactive(text, styles, reset=True):
-    """stylize() variant that adds C0 control codes (SOH/STX) for readline
-    safety."""
+    '''stylize() variant that adds C0 control codes (SOH/STX) for readline
+    safety.'''
     # problem: readline includes bare ANSI codes in width calculations.
     # solution: wrap nonprinting codes in SOH/STX when necessary.
     # see: https://gitlab.com/dslackw/colored/issues/5
-    terminator = _c0wrap(attr("reset")) if reset else ""
-    return "{}{}{}".format(_c0wrap(styles), text, terminator)
+    terminator = _c0wrap(attr('reset')) if reset else ''
+    return f'{_c0wrap(styles)}{text}{terminator}'
+
 
 def set_tty_aware(awareness=True):
-    """Makes all interactions here tty aware.  This means that if either
+    '''Makes all interactions here tty aware.  This means that if either
     stdout or stderr are directed to something other than a tty,
-    colorization will not be added."""
+    colorization will not be added.'''
     global TTY_AWARE
     TTY_AWARE = awareness
```

### Comparing `colored-1.4.3/colored/colors.py` & `colored-1.4.4/colored/colors.py`

 * *Files identical despite different names*

### Comparing `colored-1.4.3/colored.egg-info/SOURCES.txt` & `colored-1.4.4/colored.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colored-1.4.3/docs/back.COLOR.txt` & `colored-1.4.4/docs/back.COLOR.txt`

 * *Files identical despite different names*

### Comparing `colored-1.4.3/docs/colors_list.txt` & `colored-1.4.4/docs/colors_list.txt`

 * *Files identical despite different names*

### Comparing `colored-1.4.3/docs/fore.COLOR.txt` & `colored-1.4.4/docs/fore.COLOR.txt`

 * *Files identical despite different names*

### Comparing `colored-1.4.3/docs/hex_list.txt` & `colored-1.4.4/docs/hex_list.txt`

 * *Files identical despite different names*

### Comparing `colored-1.4.3/tests/test_hex_1.py` & `colored-1.4.4/tests/test_hex_1.py`

 * *Files identical despite different names*

### Comparing `colored-1.4.3/tests/test_hex_2.py` & `colored-1.4.4/tests/test_hex_2.py`

 * *Files identical despite different names*

