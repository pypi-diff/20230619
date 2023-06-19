# Comparing `tmp/boundaryscheme-2.2.tar.gz` & `tmp/boundaryscheme-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/boundaryscheme-2.2.tar", last modified: Wed Jun 14 14:39:06 2023, max compression
+gzip compressed data, was "dist/boundaryscheme-2.3.tar", last modified: Mon Jun 19 09:01:47 2023, max compression
```

## Comparing `boundaryscheme-2.2.tar` & `boundaryscheme-2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4480 2023-06-14 14:39:06.000000 boundaryscheme-2.2/PKG-INFO
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/tests/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 07:50:58.000000 boundaryscheme-2.2/tests/__init__.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       62 2023-06-14 13:22:07.000000 boundaryscheme-2.2/tests/test_import.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4480 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/PKG-INFO
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      522 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/SOURCES.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       29 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/requires.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       30 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/top_level.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        1 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme.egg-info/dependency_links.txt
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     3380 2023-06-14 13:18:38.000000 boundaryscheme-2.2/README.md
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      940 2023-06-14 14:38:10.000000 boundaryscheme-2.2/setup.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/examples/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-05-16 09:26:00.000000 boundaryscheme-2.2/examples/__init__.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2049 2023-06-14 13:22:07.000000 boundaryscheme-2.2/examples/draw_detKLcurve.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1385 2023-06-14 13:22:07.000000 boundaryscheme-2.2/examples/draw_nbrzerosdetKL.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      909 2023-06-14 13:22:07.000000 boundaryscheme-2.2/examples/draw_symbol.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-14 14:39:06.000000 boundaryscheme-2.2/boundaryscheme/
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     6390 2023-06-04 15:21:00.000000 boundaryscheme-2.2/boundaryscheme/boundaries.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      137 2023-06-14 14:38:15.000000 boundaryscheme-2.2/boundaryscheme/__init__.py
--rwxrwxrwx   0 pierrelebarbenchon   (501) staff       (20)    10942 2023-06-05 07:45:15.000000 boundaryscheme-2.2/boundaryscheme/utils.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)    19750 2023-06-14 13:22:07.000000 boundaryscheme-2.2/boundaryscheme/schemes.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2605 2023-01-16 09:04:43.000000 boundaryscheme-2.2/boundaryscheme/complex_winding_number.py
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)    22644 2023-06-14 13:22:07.000000 boundaryscheme-2.2/boundaryscheme/pyplot.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       38 2023-06-14 14:39:06.000000 boundaryscheme-2.2/setup.cfg
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4427 2023-06-19 09:01:47.000000 boundaryscheme-2.3/PKG-INFO
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/tests/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 07:50:58.000000 boundaryscheme-2.3/tests/__init__.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       62 2023-06-14 13:22:07.000000 boundaryscheme-2.3/tests/test_import.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     4427 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/PKG-INFO
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      522 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/SOURCES.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       29 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/requires.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       30 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/top_level.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        1 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme.egg-info/dependency_links.txt
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     3327 2023-06-16 13:13:26.000000 boundaryscheme-2.3/README.md
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      940 2023-06-14 14:38:10.000000 boundaryscheme-2.3/setup.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/examples/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-05-16 09:26:00.000000 boundaryscheme-2.3/examples/__init__.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1980 2023-06-19 08:52:55.000000 boundaryscheme-2.3/examples/draw_detKLcurve.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1385 2023-06-14 13:22:07.000000 boundaryscheme-2.3/examples/draw_nbrzerosdetKL.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      909 2023-06-14 13:22:07.000000 boundaryscheme-2.3/examples/draw_symbol.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-19 09:01:47.000000 boundaryscheme-2.3/boundaryscheme/
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     6390 2023-06-04 15:21:00.000000 boundaryscheme-2.3/boundaryscheme/boundaries.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      137 2023-06-19 09:01:27.000000 boundaryscheme-2.3/boundaryscheme/__init__.py
+-rwxrwxrwx   0 pierrelebarbenchon   (501) staff       (20)    10942 2023-06-05 07:45:15.000000 boundaryscheme-2.3/boundaryscheme/utils.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)    19750 2023-06-14 13:22:07.000000 boundaryscheme-2.3/boundaryscheme/schemes.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2605 2023-01-16 09:04:43.000000 boundaryscheme-2.3/boundaryscheme/complex_winding_number.py
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)    22478 2023-06-19 08:37:41.000000 boundaryscheme-2.3/boundaryscheme/pyplot.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       38 2023-06-19 09:01:47.000000 boundaryscheme-2.3/setup.cfg
```

### Comparing `boundaryscheme-2.2/PKG-INFO` & `boundaryscheme-2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boundaryscheme
-Version: 2.2
+Version: 2.3
 Summary: This library implements Kreiss-Lopatinskii determinant for numerical scheme with boundary
 Home-page: UNKNOWN
 Author: Pierre Le Barbenchon
 License: UNKNOWN
 Description: This is the architecture for the package "boundaryscheme" : https://pypi.org/project/boundaryscheme/
         
         
@@ -43,54 +43,54 @@
         plt.show()
         ```
         
         ![mygif](https://github.com/PLeBarbenchon/boundaryscheme/assets/92107096/2ca0d414-77a6-410e-a582-a3950699dcf0)
         
         # Creation of a scheme
         
-        Pour écrire le schéma $U_{j}^{n+1} = \dfrac{1}{3}U_{j-1}^n + U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{1}{6}U_{j+2}^n$ avec un certain bord $B$, il faut écrire 
+        To compute the scheme $U_{j}^{n+1} = \dfrac{1}{3}U_{j-1}^n + U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{1}{6}U_{j+2}^n$ with a boundary $B$, write 
         
         ```python
         S = Scheme([1/3,1,-1/6,-1/6],1, B) 
         ```
         
         
-        Pour écrire un schéma qui dépend d'un paramètre $\lambda$, on peut créer la classe du schéma de la façon suivante :
+        To compute the scheme depending on a parameter $\lambda$, create a Python class using the following formulation:
         
         ```python
         class Name(Scheme):
             """This is a class to represent ...
         
             :param lamb: The Courant number, i.e  a.dt/dx where "a" is the velocity, "dt" the time discretization and "dx" the space discretization
             :type lamb: float
             :param boundary: Boundary condition, defaults to Dirichlet()
             :type boundary: class:`Boundary`, optional
             :param sigma: Gap between the mesh and the boundary condition, defaults to 0
             :type sigma: float, optional
             """
         
-            def __init__(self, lamb, boundary=Dirichlet(), sigma=0, D=0, **kwargs):
+            def __init__(self, lamb, boundary=Dirichlet(), sigma=0, **kwargs):
                 """Constructor method"""
                 self.sigma = sigma
                 self.lamb = lamb
                 self.inter = #write the list of the coefficients of the scheme
                 self.center = #write the index of the center of the scheme
                 self.CFL = #give the CFL condition
                 super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
         
             def shortname(self):
                 """Name method"""
                 return "Name"
         ```
-        Par exemple pour écrire le schéma 
-        $U_{j}^{n+1} = \dfrac{\lambda}{3}U_{j-1}^n + \lambda^2 U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{\lambda}{6}U_{j+2}^n$ avec un certain bord $B$, il faut écrire 
+        For example, to compute the scheme 
+        $U_{j}^{n+1} = \dfrac{\lambda}{3}U_{j-1}^n + \lambda^2 U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{\lambda}{6}U_{j+2}^n$ with a boundary $B$, write 
         
         ```python
         class Name(Scheme):
-            def __init__(self, lamb, boundary=Dirichlet(), sigma=0, D=0, **kwargs):
+            def __init__(self, lamb, boundary=Dirichlet(), sigma=0, **kwargs):
                 self.sigma = sigma
                 self.lamb = lamb
                 self.inter = [lamb/3, lamb**2, -1/6, -lamb/6]
                 self.center = 1
                 self.CFL = #give the CFL condition
                 super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
```

### Comparing `boundaryscheme-2.2/boundaryscheme.egg-info/PKG-INFO` & `boundaryscheme-2.3/boundaryscheme.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boundaryscheme
-Version: 2.2
+Version: 2.3
 Summary: This library implements Kreiss-Lopatinskii determinant for numerical scheme with boundary
 Home-page: UNKNOWN
 Author: Pierre Le Barbenchon
 License: UNKNOWN
 Description: This is the architecture for the package "boundaryscheme" : https://pypi.org/project/boundaryscheme/
         
         
@@ -43,54 +43,54 @@
         plt.show()
         ```
         
         ![mygif](https://github.com/PLeBarbenchon/boundaryscheme/assets/92107096/2ca0d414-77a6-410e-a582-a3950699dcf0)
         
         # Creation of a scheme
         
-        Pour écrire le schéma $U_{j}^{n+1} = \dfrac{1}{3}U_{j-1}^n + U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{1}{6}U_{j+2}^n$ avec un certain bord $B$, il faut écrire 
+        To compute the scheme $U_{j}^{n+1} = \dfrac{1}{3}U_{j-1}^n + U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{1}{6}U_{j+2}^n$ with a boundary $B$, write 
         
         ```python
         S = Scheme([1/3,1,-1/6,-1/6],1, B) 
         ```
         
         
-        Pour écrire un schéma qui dépend d'un paramètre $\lambda$, on peut créer la classe du schéma de la façon suivante :
+        To compute the scheme depending on a parameter $\lambda$, create a Python class using the following formulation:
         
         ```python
         class Name(Scheme):
             """This is a class to represent ...
         
             :param lamb: The Courant number, i.e  a.dt/dx where "a" is the velocity, "dt" the time discretization and "dx" the space discretization
             :type lamb: float
             :param boundary: Boundary condition, defaults to Dirichlet()
             :type boundary: class:`Boundary`, optional
             :param sigma: Gap between the mesh and the boundary condition, defaults to 0
             :type sigma: float, optional
             """
         
-            def __init__(self, lamb, boundary=Dirichlet(), sigma=0, D=0, **kwargs):
+            def __init__(self, lamb, boundary=Dirichlet(), sigma=0, **kwargs):
                 """Constructor method"""
                 self.sigma = sigma
                 self.lamb = lamb
                 self.inter = #write the list of the coefficients of the scheme
                 self.center = #write the index of the center of the scheme
                 self.CFL = #give the CFL condition
                 super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
         
             def shortname(self):
                 """Name method"""
                 return "Name"
         ```
-        Par exemple pour écrire le schéma 
-        $U_{j}^{n+1} = \dfrac{\lambda}{3}U_{j-1}^n + \lambda^2 U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{\lambda}{6}U_{j+2}^n$ avec un certain bord $B$, il faut écrire 
+        For example, to compute the scheme 
+        $U_{j}^{n+1} = \dfrac{\lambda}{3}U_{j-1}^n + \lambda^2 U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{\lambda}{6}U_{j+2}^n$ with a boundary $B$, write 
         
         ```python
         class Name(Scheme):
-            def __init__(self, lamb, boundary=Dirichlet(), sigma=0, D=0, **kwargs):
+            def __init__(self, lamb, boundary=Dirichlet(), sigma=0, **kwargs):
                 self.sigma = sigma
                 self.lamb = lamb
                 self.inter = [lamb/3, lamb**2, -1/6, -lamb/6]
                 self.center = 1
                 self.CFL = #give the CFL condition
                 super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
```

### Comparing `boundaryscheme-2.2/boundaryscheme.egg-info/SOURCES.txt` & `boundaryscheme-2.3/boundaryscheme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.2/README.md` & `boundaryscheme-2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -36,54 +36,54 @@
 plt.show()
 ```
 
 ![mygif](https://github.com/PLeBarbenchon/boundaryscheme/assets/92107096/2ca0d414-77a6-410e-a582-a3950699dcf0)
 
 # Creation of a scheme
 
-Pour écrire le schéma $U_{j}^{n+1} = \dfrac{1}{3}U_{j-1}^n + U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{1}{6}U_{j+2}^n$ avec un certain bord $B$, il faut écrire 
+To compute the scheme $U_{j}^{n+1} = \dfrac{1}{3}U_{j-1}^n + U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{1}{6}U_{j+2}^n$ with a boundary $B$, write 
 
 ```python
 S = Scheme([1/3,1,-1/6,-1/6],1, B) 
 ```
 
 
-Pour écrire un schéma qui dépend d'un paramètre $\lambda$, on peut créer la classe du schéma de la façon suivante :
+To compute the scheme depending on a parameter $\lambda$, create a Python class using the following formulation:
 
 ```python
 class Name(Scheme):
     """This is a class to represent ...
 
     :param lamb: The Courant number, i.e  a.dt/dx where "a" is the velocity, "dt" the time discretization and "dx" the space discretization
     :type lamb: float
     :param boundary: Boundary condition, defaults to Dirichlet()
     :type boundary: class:`Boundary`, optional
     :param sigma: Gap between the mesh and the boundary condition, defaults to 0
     :type sigma: float, optional
     """
 
-    def __init__(self, lamb, boundary=Dirichlet(), sigma=0, D=0, **kwargs):
+    def __init__(self, lamb, boundary=Dirichlet(), sigma=0, **kwargs):
         """Constructor method"""
         self.sigma = sigma
         self.lamb = lamb
         self.inter = #write the list of the coefficients of the scheme
         self.center = #write the index of the center of the scheme
         self.CFL = #give the CFL condition
         super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
 
     def shortname(self):
         """Name method"""
         return "Name"
 ```
-Par exemple pour écrire le schéma 
-$U_{j}^{n+1} = \dfrac{\lambda}{3}U_{j-1}^n + \lambda^2 U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{\lambda}{6}U_{j+2}^n$ avec un certain bord $B$, il faut écrire 
+For example, to compute the scheme 
+$U_{j}^{n+1} = \dfrac{\lambda}{3}U_{j-1}^n + \lambda^2 U_j^n -\dfrac{1}{6} U_{j+1}^n - \dfrac{\lambda}{6}U_{j+2}^n$ with a boundary $B$, write 
 
 ```python
 class Name(Scheme):
-    def __init__(self, lamb, boundary=Dirichlet(), sigma=0, D=0, **kwargs):
+    def __init__(self, lamb, boundary=Dirichlet(), sigma=0, **kwargs):
         self.sigma = sigma
         self.lamb = lamb
         self.inter = [lamb/3, lamb**2, -1/6, -lamb/6]
         self.center = 1
         self.CFL = #give the CFL condition
         super().__init__(inter=self.inter, center=self.center, boundary=boundary, sigma=sigma, **kwargs)
```

### Comparing `boundaryscheme-2.2/setup.py` & `boundaryscheme-2.3/setup.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.2/examples/draw_detKLcurve.py` & `boundaryscheme-2.3/examples/draw_detKLcurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 
 
 if __name__ == "__main__":
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda = 1.4"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = 1.4)
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda in [1.4, 0.7, 1] with sigma = 0.4"""
-    # bsplt.detKLplot(BeamWarming, SILW(2, 3), lamb=np.array([1.4, 0.7, 1]), sigma=0)
+    bsplt.detKLplot(BeamWarming, SILW(2, 3), lamb=np.array([1.4, 0.7, 1]), sigma=0)
 
-    bsplt.detKLplot(LaxWendroff(5), SILW(2, 3), lambdacursor=True)
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda = 1 with sigma in [-0.2, 0, 0.1,0.4]"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = 1, sigma = np.array([-0.2, 0, 0.1,0.4]))
 
     """plot the Kreiss-Lopatinskii determinant curve for BeamWarming and for lambda in [1.4, 0.7] with sigma in [-0.2, 0, 0.4]"""
     # bsplt.detKLplot(BeamWarming, SILW(2,3), lamb = [1.4, 0.7], sigma = np.array([-0.2, 0, 0.4]))
```

### Comparing `boundaryscheme-2.2/examples/draw_nbrzerosdetKL.py` & `boundaryscheme-2.3/examples/draw_nbrzerosdetKL.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.2/examples/draw_symbol.py` & `boundaryscheme-2.3/examples/draw_symbol.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.2/boundaryscheme/boundaries.py` & `boundaryscheme-2.3/boundaryscheme/boundaries.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.2/boundaryscheme/utils.py` & `boundaryscheme-2.3/boundaryscheme/utils.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.2/boundaryscheme/schemes.py` & `boundaryscheme-2.3/boundaryscheme/schemes.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.2/boundaryscheme/complex_winding_number.py` & `boundaryscheme-2.3/boundaryscheme/complex_winding_number.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-2.2/boundaryscheme/pyplot.py` & `boundaryscheme-2.3/boundaryscheme/pyplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2)
     ax.axvline(x=0, color="0.5")
     ax.axhline(y=0, color="0.5")
     ax.axis("equal")
     plt.show()
 
 
-def detKLplot(schem, left_bound=Dirichlet(), lamb=None, sigma=0, lambdacursor=False, sigmacursor=False, nparam=300, parametrization_bool=True, fig_size=(6, 4)):
+def detKLplot(schem, left_bound=Dirichlet(), lamb=None, sigma=0, lambdacursor=False, sigmacursor=False, nparam=300, parametrization_bool=True, fig_size=(10, 8)):
     """Computes the Kreiss-Lopatinskii determinant curve for different lambdas and different sigmas or with cursor(s)
 
     :param schem: Scheme depending on a parameter lambda
     :type schem: class:`Scheme`
     :param left_bound: Left boundary of the class Boundary, defaults to Dirichlet()
     :type left_bound: class:`Boundary`, optional
     :param lamb: A value lambda or a numpy.ndarray of several values of lambda (lambda is the Courant number a.dt/dx), defaults to None
@@ -75,15 +75,15 @@
                 for l in lamb:
                     S = schem(l, left_bound, sigma=sigma[0])
                     Param, Det = S.detKL(nparam, parametrization_bool)
                     ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, label=f"$\lambda$ = " + str(l))
                 ax.axvline(x=0, color="0.5")
                 ax.axhline(y=0, color="0.5")
                 ax.legend(loc="best")
-                plt.title("Symbol of " + S.name(boundary_bool=True, sigma_bool=True, lambda_bool=False))
+                plt.title("Kreiss-Lopatinskii determinant curve of " + S.name(boundary_bool=True, sigma_bool=True, lambda_bool=False))
             elif len(lamb) == 1:
                 sigma = np.sort(sigma)
                 fig, ax = plt.subplots(figsize=fig_size)
                 for sig in sigma:
                     S = schem(lamb[0], left_bound, sigma=sig)
                     Param, Det = S.detKL(nparam, parametrization_bool)
                     ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, label=f"$\sigma$ = " + str(sig))
@@ -109,20 +109,19 @@
             lambmax = np.max(lamb)
             if len(lamb) == 1 or np.min(lamb) < 0.001:
                 lambmin = 0.001
             else:
                 lambmin = np.min(lamb)
 
             lamb0 = (lambmax + lambmin) / 2
-            fig = plt.figure(1, figsize=(10, 8))
+            fig, ax = plt.subplots(figsize=fig_size)
             plt.title("DKL curve of " + schem(1, left_bound, sigma=sigma[0]).name(boundary_bool=True, sigma_bool=True))
-            ax = fig.add_subplot(111, label="cursor1")
             fig.subplots_adjust(left=0.25, bottom=0.25)
             ax.set_xlim(-3, 3)
-            ax.axis("equal")
+            
 
             def calc_det(l):
                 S = schem(l, left_bound, sigma=sigma[0])
                 return S.detKL(nparam, parametrization_bool)[1]
 
             Det = calc_det(lamb0)
             [line] = ax.plot([z.real for z in Det], [z.imag for z in Det], linewidth=2, color="red")
@@ -137,15 +136,15 @@
                 Det = calc_det(lambda_slider.val)
                 line.set_xdata([z.real for z in Det])
                 line.set_ydata([z.imag for z in Det])
                 xmin = min([z.real for z in Det])
                 xmax = max([z.real for z in Det])
                 ymin = min([z.imag for z in Det])
                 ymax = max([z.imag for z in Det])
-                ax.set_xlim(xmin, xmax)
+                ax.set_xlim(min(xmin,-0.5), max(xmax,0.5))
                 ax.set_ylim(ymin, ymax)
                 fig.canvas.draw_idle()
 
             # register the update function with each slider
             lambda_slider.on_changed(update)
 
             # Create a `matplotlib.widgets.Button` to reset the sliders to initial values.
@@ -164,17 +163,16 @@
         else:
             sigmax = np.max(sigma)
             sigmin = np.min(sigma)
         if lambdacursor == False:
             if len(lamb) > 1:
                 raise TypeError("With a sigma cursor, lambda has to be a single value")
             sigma0 = (sigmax + sigmin) / 2
-            fig = plt.figure(1, figsize=(10, 8))
+            fig, ax = plt.subplots(figsize=fig_size)
             plt.title("DKL curve of " + schem(lamb[0], left_bound).name(boundary_bool=True, lambda_bool=True))
-            ax = fig.add_subplot(111, label="cursor2")
             fig.subplots_adjust(left=0.25, bottom=0.25)
             ax.set_xlim(-3, 3)
             ax.axis("equal")
 
             def calc_det(sig):
                 S = schem(lamb[0], left_bound, sigma=sig)
                 return S.detKL(nparam, parametrization_bool)[1]
@@ -218,17 +216,16 @@
                 lambmin = 0.001
             else:
                 lambmin = np.min(lamb)
 
             sigma0 = (sigmax + sigmin) / 2
             lamb0 = (lambmin + lambmax) / 2
 
-            fig = plt.figure(1, figsize=(10, 8))
+            fig, ax = plt.subplots(figsize=fig_size)
             plt.title("DKL curve of " + schem(1, left_bound).name(boundary_bool=True))
-            ax = fig.add_subplot(111, label="cursor3")
             fig.subplots_adjust(left=0.25, bottom=0.25)
             ax.set_xlim(-3, 3)
             ax.axis("equal")
 
             def calc_det(l, sigm):
                 S = schem(l, left_bound, sigma=sigm)
                 return S.detKL(nparam, parametrization_bool)[1]
@@ -322,17 +319,16 @@
             plt.title("Symbol of " + S.name(lambda_bool=False))
 
     else:
         if lamb == None:
             lamb = schem(1).CFL
         if isinstance(lamb, (int, float)):
             lamb = np.array([lamb], dtype=float)
-        fig = plt.figure(1, figsize=(10, 8))
+        fig, ax = plt.subplots(figsize=fig_size)
         plt.title("Symbol of " + schem(1).name(lambda_bool=False))
-        ax = fig.add_subplot(111, label="cursor4")
         fig.subplots_adjust(left=0.25, bottom=0.25)
         ax.set_xlim(-3, 3)
         ax.axis("equal")
 
         if len(lamb) == 1:
             lamb0 = lamb[0] / 2
         else:
```

