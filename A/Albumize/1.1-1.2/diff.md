# Comparing `tmp/Albumize-1.1.tar.gz` & `tmp/Albumize-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Albumize-1.1.tar", last modified: Mon Jun 19 01:23:40 2023, max compression
+gzip compressed data, was "Albumize-1.2.tar", last modified: Mon Jun 19 01:28:42 2023, max compression
```

## Comparing `Albumize-1.1.tar` & `Albumize-1.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:23:40.594967 Albumize-1.1/
-drwxrwxrwx   0        0        0        0 2023-06-19 01:23:40.593971 Albumize-1.1/Albumize.egg-info/
--rw-rw-rw-   0        0        0      107 2023-06-19 01:23:40.000000 Albumize-1.1/Albumize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-06-19 01:23:40.000000 Albumize-1.1/Albumize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:23:40.000000 Albumize-1.1/Albumize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 01:23:40.000000 Albumize-1.1/Albumize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4608 2023-06-19 01:10:49.000000 Albumize-1.1/Albumize.py
--rw-rw-rw-   0        0        0      107 2023-06-19 01:23:40.593971 Albumize-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 01:23:40.594967 Albumize-1.1/setup.cfg
--rw-rw-rw-   0        0        0      139 2023-06-19 01:10:49.000000 Albumize-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:28:42.970774 Albumize-1.2/
+drwxrwxrwx   0        0        0        0 2023-06-19 01:28:42.969777 Albumize-1.2/Albumize.egg-info/
+-rw-rw-rw-   0        0        0      107 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-19 01:28:42.000000 Albumize-1.2/Albumize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4693 2023-06-19 01:26:57.000000 Albumize-1.2/Albumize.py
+-rw-rw-rw-   0        0        0      107 2023-06-19 01:28:42.969777 Albumize-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:28:42.970774 Albumize-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-06-19 01:28:30.000000 Albumize-1.2/setup.py
```

### Comparing `Albumize-1.1/Albumize.py` & `Albumize-1.2/Albumize.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,8 +206,17 @@
 		oFiPa.parent.mkdir(parents=True, exist_ok=True)
 		iFiPa.rename(oFiPa)
 		pass
 
 	pass
 
 
+def CLI():
+	_CONS = _Cons()
+	_main()
 
+	pass
+
+
+if __name__ == '__main__':
+	CLI()
+	pass
```

