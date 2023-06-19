# Comparing `tmp/skmetpy-0.1.2.tar.gz` & `tmp/skmetpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.1.2.tar", last modified: Mon Jun 19 09:52:33 2023, max compression
+gzip compressed data, was "skmetpy-0.1.6.tar", last modified: Mon Jun 19 13:35:33 2023, max compression
```

## Comparing `skmetpy-0.1.2.tar` & `skmetpy-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:52:33.289996 skmetpy-0.1.2/
--rw-rw-rw-   0        0        0      259 2023-06-19 09:52:33.289996 skmetpy-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 09:52:33.283990 skmetpy-0.1.2/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.2/nunpy/__init__.py
--rw-rw-rw-   0        0        0    24774 2023-06-19 09:50:24.000000 skmetpy-0.1.2/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-19 09:52:33.289996 skmetpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-19 09:52:26.000000 skmetpy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:52:33.287994 skmetpy-0.1.2/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-19 09:52:33.000000 skmetpy-0.1.2/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-19 09:52:33.000000 skmetpy-0.1.2/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:52:33.000000 skmetpy-0.1.2/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 09:52:33.000000 skmetpy-0.1.2/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 13:35:33.899213 skmetpy-0.1.6/
+-rw-rw-rw-   0        0        0      259 2023-06-19 13:35:33.898211 skmetpy-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 13:35:33.893208 skmetpy-0.1.6/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.6/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    24712 2023-06-19 13:34:56.000000 skmetpy-0.1.6/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:35:33.899213 skmetpy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-19 13:35:31.000000 skmetpy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:35:33.897212 skmetpy-0.1.6/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-19 13:35:33.000000 skmetpy-0.1.6/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-19 13:35:33.000000 skmetpy-0.1.6/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:35:33.000000 skmetpy-0.1.6/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 13:35:33.000000 skmetpy-0.1.6/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.1.2/nunpy/rechape.py` & `skmetpy-0.1.6/nunpy/rechape.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,14 @@
 
             d4 = a4 - y_d
             d3 = np.multiply(np.dot(d4, initial_theta3), np.multiply(a3, 1-a3))
             d2 = np.multiply(np.dot(d3[:,1:], initial_theta2), np.multiply(a2, 1 - a2))
             d3 = d3[:,1:]
             d2 = d2[:,1:]
 
-
             delta1 = d2.T @ a1
             delta2 = d3.T @ a2
             delta3 = d4.T @ a3
 
             delta1 /= m
             delta2 /= m
             delta3 /= m
@@ -407,22 +406,20 @@
                 peliculas_recomendadas.append(np.mean(Y[i, peliculas[i]]))
         
             indices_ordenados_valoracion = np.argsort(num_valoraciones, axis=0)[::-1]
             indices_ordenados_media = np.argsort(peliculas_recomendadas, axis=0)[::-1]
         
             print(f"Primeras {num_peliculas} películas mejor valoradas (Ordenadas por valoración):")
             for i in range(num_peliculas):
-                print(f"{i} Nº {indices_ordenados_valoracion[i]} con {peliculas_recomendadas[indices_ordenados_valoracion[i]]} puntos"
-                      f", valorada {num_valoraciones[indices_ordenados_valoracion[i]]} ({movies_idx[indices_ordenados_valoracion[i]]})")
+                print(f"{i} Nº {indices_ordenados_valoracion[i]} con {peliculas_recomendadas[indices_ordenados_valoracion[i]]} puntos valorada {num_valoraciones[indices_ordenados_valoracion[i]]} ({movies_idx[indices_ordenados_valoracion[i]]})")
         
             print(f"\nPrimeras {num_peliculas} peliculas mejor valoradas (Ordenadas por media):")
             for i in range(num_peliculas):
                 print(
-                    f"{i} Nº {indices_ordenados_media[i]} con {peliculas_recomendadas[indices_ordenados_media[i]]} puntos"
-                    f", valorada {num_valoraciones[indices_ordenados_media[i]]} ({movies_idx[indices_ordenados_media[i]]})")
+                    f"{i} Nº {indices_ordenados_media[i]} con {peliculas_recomendadas[indices_ordenados_media[i]]} puntos valorada {num_valoraciones[indices_ordenados_media[i]]} ({movies_idx[indices_ordenados_media[i]]})")
       '''
     print(string)
 
 
 def cost2():
     string = '''
         # Main
@@ -489,15 +486,14 @@
 
 def fmin2():
     string = '''
         lambda_param = 1.5
         maxiter = 200
         X_rand = np.random.rand(n_movies, features) * (2 * 0.12)
         Theta_rand = np.random.rand(features, n_users) * (2 * 0.12)
-    
         params = np.hstack((np.ravel(X_rand, order='F'), np.ravel(Theta_rand, order='F')))
     
         fmin = opt.fmin_cg(maxiter=maxiter, f=cobaCostFuncReg, x0=params, fprime=cobaGradientFuncReg, args=(Y, R, features, lambda_param))
     
         X = np.reshape(fmin[:n_movies * features], (n_movies, features), 'F')
         Theta = np.reshape(fmin[n_movies * features:], (features, n_users), 'F')
       '''
```

