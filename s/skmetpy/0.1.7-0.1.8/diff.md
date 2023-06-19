# Comparing `tmp/skmetpy-0.1.7.tar.gz` & `tmp/skmetpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.1.7.tar", last modified: Mon Jun 19 13:43:23 2023, max compression
+gzip compressed data, was "skmetpy-0.1.8.tar", last modified: Mon Jun 19 13:48:18 2023, max compression
```

## Comparing `skmetpy-0.1.7.tar` & `skmetpy-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:43:23.725192 skmetpy-0.1.7/
--rw-rw-rw-   0        0        0      259 2023-06-19 13:43:23.724190 skmetpy-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 13:43:23.718113 skmetpy-0.1.7/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.7/nunpy/__init__.py
--rw-rw-rw-   0        0        0    24712 2023-06-19 13:34:56.000000 skmetpy-0.1.7/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-19 13:43:23.725192 skmetpy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-19 13:43:21.000000 skmetpy-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:43:23.723188 skmetpy-0.1.7/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-19 13:43:23.000000 skmetpy-0.1.7/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-19 13:43:23.000000 skmetpy-0.1.7/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:43:23.000000 skmetpy-0.1.7/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 13:43:23.000000 skmetpy-0.1.7/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 13:48:18.256930 skmetpy-0.1.8/
+-rw-rw-rw-   0        0        0      259 2023-06-19 13:48:18.255415 skmetpy-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 13:48:18.248408 skmetpy-0.1.8/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.8/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    24710 2023-06-19 13:47:49.000000 skmetpy-0.1.8/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:48:18.256930 skmetpy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-19 13:48:10.000000 skmetpy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:48:18.254413 skmetpy-0.1.8/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-19 13:48:18.000000 skmetpy-0.1.8/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-19 13:48:18.000000 skmetpy-0.1.8/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:48:18.000000 skmetpy-0.1.8/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 13:48:18.000000 skmetpy-0.1.8/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.1.7/nunpy/rechape.py` & `skmetpy-0.1.8/nunpy/rechape.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
             indices_ordenados_valoracion = np.argsort(num_valoraciones, axis=0)[::-1]
             indices_ordenados_media = np.argsort(peliculas_recomendadas, axis=0)[::-1]
         
             print(f"Primeras {num_peliculas} películas mejor valoradas (Ordenadas por valoración):")
             for i in range(num_peliculas):
                 print(f"{i} Nº {indices_ordenados_valoracion[i]} con {peliculas_recomendadas[indices_ordenados_valoracion[i]]} puntos valorada {num_valoraciones[indices_ordenados_valoracion[i]]} ({movies_idx[indices_ordenados_valoracion[i]]})")
         
-            print(f"\nPrimeras {num_peliculas} peliculas mejor valoradas (Ordenadas por media):")
+            print(f"Primeras {num_peliculas} peliculas mejor valoradas (Ordenadas por media):")
             for i in range(num_peliculas):
                 print(
                     f"{i} Nº {indices_ordenados_media[i]} con {peliculas_recomendadas[indices_ordenados_media[i]]} puntos valorada {num_valoraciones[indices_ordenados_media[i]]} ({movies_idx[indices_ordenados_media[i]]})")
       '''
     print(string)
```

