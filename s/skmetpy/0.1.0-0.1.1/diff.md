# Comparing `tmp/skmetpy-0.1.0.tar.gz` & `tmp/skmetpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.1.0.tar", last modified: Sun Jun 18 21:26:26 2023, max compression
+gzip compressed data, was "skmetpy-0.1.1.tar", last modified: Sun Jun 18 22:49:46 2023, max compression
```

## Comparing `skmetpy-0.1.0.tar` & `skmetpy-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 21:26:26.694148 skmetpy-0.1.0/
--rw-rw-rw-   0        0        0      259 2023-06-18 21:26:26.693147 skmetpy-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 21:26:26.685140 skmetpy-0.1.0/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.0/nunpy/__init__.py
--rw-rw-rw-   0        0        0    25182 2023-06-18 21:25:23.000000 skmetpy-0.1.0/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-18 21:26:26.695149 skmetpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-18 21:26:17.000000 skmetpy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 21:26:26.691144 skmetpy-0.1.0/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-18 21:26:26.000000 skmetpy-0.1.0/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-18 21:26:26.000000 skmetpy-0.1.0/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 21:26:26.000000 skmetpy-0.1.0/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-18 21:26:26.000000 skmetpy-0.1.0/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 22:49:46.502636 skmetpy-0.1.1/
+-rw-rw-rw-   0        0        0      259 2023-06-18 22:49:46.501979 skmetpy-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 22:49:46.384545 skmetpy-0.1.1/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.1/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    24662 2023-06-18 22:49:36.000000 skmetpy-0.1.1/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-18 22:49:46.502636 skmetpy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-18 22:49:43.000000 skmetpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:49:46.499977 skmetpy-0.1.1/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-18 22:49:46.000000 skmetpy-0.1.1/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-18 22:49:46.000000 skmetpy-0.1.1/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 22:49:46.000000 skmetpy-0.1.1/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-18 22:49:46.000000 skmetpy-0.1.1/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.1.0/nunpy/rechape.py` & `skmetpy-0.1.1/nunpy/rechape.py`

 * *Files 5% similar despite different names*

```diff
@@ -396,17 +396,17 @@
             # Funcion
             def ranking_peliculas(Y, R, movie_idx):
                 n_movies = Y.shape[0]
                 Yval = np.zeros((n_movies, 1))
                 Ymean = np.zeros((n_movies, 1))
 
                 for i in range(n_movies):
-                    idx = np.where(R[i, :] == 1)[0] # Esta linea devuelve los indices de las columnas donde la fila i de R tiene el valor 1
-                    Yval[i] = len(idx)              # R[i, :] lo que hace es recorrer las filas de la matriz con i, mientras que los dos puntos (:) devuelve las columnas
-                    Ymean[i] = Y[i, idx].mean()     # osea devuelve el vector que contiene las columnas
+                    idx = np.where(R[i, :] == 1)[0] 
+                    Yval[i] = len(idx)             
+                    Ymean[i] = Y[i, idx].mean()
 
                 idxYval = np.argsort(Yval, axis=0)[::-1]
                 idxYmean = np.argsort(Ymean, axis=0)[::-1]
 
                 print(f"Primeras {n} peliculas mejor valoradas (con nº de vistas)")
                 for i in range(n):
                     print(f"{i} Nº {idxYmean[i]} con {Ymean[int(idxYmean[i])]} puntos, valorada {int(Yval[int(idxYmean[i])])} veces "
@@ -563,15 +563,15 @@
     print(string)
 
 def fcc3():
     string = '''
         # Main
         print("Finding closest centroids\n")
         idx = findClosestCentroids(X, initial_centroids)
-        print("Closest centroids for the first 3 examples: ", idx[0:3], " (the closest centroids should be 0, 2, 1 respectively)\n")
+        print("Closest centroids for the first 3 examples: ", idx[0:3])
         
         # Funcion
         def findClosestCentroids(x, initial_centroids):
             closest_centroids = list()
         
             for i in range(len(x)):
                 distancia_minima = float('inf')
@@ -615,15 +615,15 @@
             max_iters = 10
             centroids, idx = runKmeans(X, initial_centroids, max_iters, plot=True)
             
             # Funcion
             def runKmeans(X, initial_centroids, max_iters, plot=True):
                 centroids_finales = initial_centroids
                 indices_centroides_finales = list()
-                K = len(initial_centroids) # Como hay solo 3, po el numero de centroides es la longitud
+                K = len(initial_centroids)
             
                 for i in range(max_iters):
                     indices_centroides_finales = findClosestCentroids(X, centroids_finales)
                     centroids_finales = computeCentroids(X, indices_centroides_finales, K)
             
                 if plot:
                     plotClusters(X, indices_centroides_finales, centroids_finales, initial_centroids)
@@ -663,15 +663,14 @@
                 for K in range(1,11):
                     coste = 0
                     initial_centroids = kMeansInitCentroids(X, K)
                     centroids, indice_centroid = runKmeans(X, initial_centroids, max_iters=10, plot=False)
             
                     # h es cada elemento de X
                     for j in range(len(X)):
-                        # si coincide el numero de cluster que se esta viendo y el elemento de x tiene ese indice, calcula la distancia
                         coste += np.sum(np.power((X[j] - centroids[indice_centroid[j]]), 2))
                     costes.append(coste)
             
                 num_clusters = [i for i in range(1,11)]
                 plt.plot(num_clusters, costes)
                 plt.show()
     '''
```

