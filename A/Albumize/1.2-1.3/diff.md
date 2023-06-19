# Comparing `tmp/Albumize-1.2.tar.gz` & `tmp/Albumize-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Albumize-1.2.tar", last modified: Mon Jun 19 01:28:42 2023, max compression
+gzip compressed data, was "Albumize-1.3.tar", last modified: Mon Jun 19 01:33:27 2023, max compression
```

## Comparing `Albumize-1.2.tar` & `Albumize-1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:28:42.970774 Albumize-1.2/
-drwxrwxrwx   0        0        0        0 2023-06-19 01:28:42.969777 Albumize-1.2/Albumize.egg-info/
--rw-rw-rw-   0        0        0      107 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4693 2023-06-19 01:26:57.000000 Albumize-1.2/Albumize.py
--rw-rw-rw-   0        0        0      107 2023-06-19 01:28:42.969777 Albumize-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 01:28:42.970774 Albumize-1.2/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-06-19 01:28:30.000000 Albumize-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:33:27.702230 Albumize-1.3/
+drwxrwxrwx   0        0        0        0 2023-06-19 01:33:27.702230 Albumize-1.3/Albumize.egg-info/
+-rw-rw-rw-   0        0        0      107 2023-06-19 01:33:27.000000 Albumize-1.3/Albumize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-06-19 01:33:27.000000 Albumize-1.3/Albumize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:33:27.000000 Albumize-1.3/Albumize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:33:27.000000 Albumize-1.3/Albumize.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-19 01:33:27.000000 Albumize-1.3/Albumize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4702 2023-06-19 01:33:09.000000 Albumize-1.3/Albumize.py
+-rw-rw-rw-   0        0        0      107 2023-06-19 01:33:27.702230 Albumize-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:33:27.702230 Albumize-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-06-19 01:33:09.000000 Albumize-1.3/setup.py
```

### Comparing `Albumize-1.2/Albumize.py` & `Albumize-1.3/Albumize.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 			pass
 		pass
 	return tasks
 
 
 ################################################################
 
-def _main():
+def _main(_CONS):
 	iFiPas = [Path(_[0]) / fn for _ in os.walk(_CONS.iDiPa) for fn in _[2]]
 
 	L = len(iFiPas)
 	cons = [_CONS] * L
 	fmt = '{:0>%d}' % len(str(L - 1))
 	tDiPa = _CONS.oDiPa
 	tFiPas = [tDiPa / fmt.format(_) for _ in range(L)]
@@ -208,15 +208,14 @@
 		pass
 
 	pass
 
 
 def CLI():
 	_CONS = _Cons()
-	_main()
-
+	_main(_CONS)
 	pass
 
 
 if __name__ == '__main__':
 	CLI()
 	pass
```

