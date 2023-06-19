# Comparing `tmp/american_options-0.1.4.tar.gz` & `tmp/american_options-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\american_options-0.1.4.tar", last modified: Fri Jun 16 22:26:06 2023, max compression
+gzip compressed data, was "dist\american_options-0.1.5.tar", last modified: Mon Jun 19 09:13:26 2023, max compression
```

## Comparing `american_options-0.1.4.tar` & `american_options-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 22:26:06.000000 american_options-0.1.4/
--rw-rw-rw-   0        0        0     2514 2023-06-16 22:26:06.000000 american_options-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2023-06-12 01:21:26.000000 american_options-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 22:26:06.000000 american_options-0.1.4/american_options/
--rw-rw-rw-   0        0        0    38860 2023-06-16 11:47:37.000000 american_options-0.1.4/american_options/AMoption.py
--rw-rw-rw-   0        0        0      191 2023-06-12 00:46:34.000000 american_options-0.1.4/american_options/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-06-11 22:01:15.000000 american_options-0.1.4/american_options/jump_diffusion.py
--rw-rw-rw-   0        0        0    13623 2023-06-14 22:10:53.000000 american_options-0.1.4/american_options/payoffs.py
--rw-rw-rw-   0        0        0     3844 2023-06-13 18:24:10.000000 american_options-0.1.4/american_options/próby.py
--rw-rw-rw-   0        0        0     2638 2023-06-11 17:41:22.000000 american_options-0.1.4/american_options/sobol.py
--rw-rw-rw-   0        0        0    10506 2023-06-16 18:15:53.000000 american_options-0.1.4/american_options/underlying.py
--rw-rw-rw-   0        0        0     2859 2023-06-16 10:33:51.000000 american_options-0.1.4/american_options/xd.py
-drwxrwxrwx   0        0        0        0 2023-06-16 22:26:06.000000 american_options-0.1.4/american_options.egg-info/
--rw-rw-rw-   0        0        0     2514 2023-06-16 22:26:05.000000 american_options-0.1.4/american_options.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-06-16 22:26:06.000000 american_options-0.1.4/american_options.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 22:26:05.000000 american_options-0.1.4/american_options.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-16 22:26:05.000000 american_options-0.1.4/american_options.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-16 22:26:05.000000 american_options-0.1.4/american_options.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 22:26:06.000000 american_options-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1429 2023-06-16 22:25:54.000000 american_options-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:13:26.000000 american_options-0.1.5/
+-rw-rw-rw-   0        0        0     2527 2023-06-19 09:13:26.000000 american_options-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2023-06-12 01:21:26.000000 american_options-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 09:13:26.000000 american_options-0.1.5/american_options/
+-rw-rw-rw-   0        0        0    40133 2023-06-17 17:52:46.000000 american_options-0.1.5/american_options/AMoption.py
+-rw-rw-rw-   0        0        0      191 2023-06-17 17:51:29.000000 american_options-0.1.5/american_options/__init__.py
+-rw-rw-rw-   0        0        0    13623 2023-06-14 22:10:53.000000 american_options-0.1.5/american_options/payoffs.py
+-rw-rw-rw-   0        0        0    10506 2023-06-16 18:15:53.000000 american_options-0.1.5/american_options/underlying.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:13:26.000000 american_options-0.1.5/american_options.egg-info/
+-rw-rw-rw-   0        0        0     2527 2023-06-19 09:13:26.000000 american_options-0.1.5/american_options.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-06-19 09:13:26.000000 american_options-0.1.5/american_options.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:13:26.000000 american_options-0.1.5/american_options.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-19 09:13:26.000000 american_options-0.1.5/american_options.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 09:13:26.000000 american_options-0.1.5/american_options.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:13:26.000000 american_options-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-06-19 09:11:41.000000 american_options-0.1.5/setup.py
```

### Comparing `american_options-0.1.4/PKG-INFO` & `american_options-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: american_options
-Version: 0.1.4
-Summary: Added new payoffs
+Version: 0.1.5
+Summary: Exercise time plotting updated
 Home-page: https://american_options.readthedocs.io/
 Author: Przemysław Adamski, Katarzyna Hasal, Kacper Toczek
 Author-email: kat.hasal99@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `american_options-0.1.4/README.md` & `american_options-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `american_options-0.1.4/american_options/AMoption.py` & `american_options-0.1.5/american_options/AMoption.py`

 * *Files 3% similar despite different names*

```diff
@@ -586,15 +586,15 @@
                 Ht[:, ti - i] = df['continue'] * disc
                 Vt[:, ti - i] = np.maximum(all_payoffs[:, ti - i], Ht[:, ti - i])
             Ht = np.hstack((Ht, np.zeros((n_sims, 1))))
             # print(Vt[0,:])
             # print(np.mean(Vt[:,0]))
 
             ###stopping times
-            stop = all_payoffs >= Ht
+            stop = all_payoffs > Ht
             exercise_time = np.argmax(stop, axis=1)
 
             res = np.mean(Yt[np.arange(len(Yt)), exercise_time])
 
             self.ET_ssp = stop.astype(int)
             self.upper_bound_price_ssp = np.mean(Vt[:,0])
 
@@ -678,15 +678,15 @@
                                     'high est': [np.mean(high_estimators)],
                                     'left high': [np.mean(high_estimators) - np.std(high_estimators) / np.sqrt(
                                         n_sims) * stats.norm.ppf(0.95)],
                                     'righ high': [np.mean(high_estimators) + np.std(high_estimators) / np.sqrt(
                                         n_sims) * stats.norm.ppf(0.95)]})
         return results
 
-    def plot_exercise_times(self, method, plot_trajectories_ratio = 0.02):
+    def plot_exercise_times(self, method, plot_trajectories_ratio = 0.02, alpha_exercise_moments=0.5, alpha_trajectories = 0.3):
         if len(self.underlyings) == 1:
             if method == 'RTM':
                 raise Exception('plot of RTM exercise times is not supported')
             elif not hasattr(self, 'ET_' + method):
                 raise Exception('''You haven't calculated price with .''' + method + ''' yet or chosen pricing method doesn't exist''')
 
             if method == 'LS':
@@ -694,21 +694,26 @@
                 asset_prices = self.LS_price_trajectories.to_numpy()[self.ET_LS.astype(bool)]
                 price_traj = self.LS_price_trajectories.to_numpy()
             elif method == 'ssp':
                 time_moments = np.argwhere(self.ET_ssp == 1)[:, 1]
                 asset_prices = self.ssp_price_trajectories[self.ET_ssp.astype(bool)]
                 price_traj = self.ssp_price_trajectories
 
-            plt.scatter(time_moments, asset_prices)
+            plt.scatter(time_moments, asset_prices, alpha = alpha_exercise_moments)
+            plt.title("Exercise moments", fontsize=40)
+            plt.xlabel("Time", fontsize=32)
+            plt.ylabel("Asset price", fontsize=32, labelpad=15)
+            plt.xticks(fontsize=30)
+            plt.yticks(fontsize=30)
 
             if plot_trajectories_ratio == 0:
                 pass
             else:
                 for k in np.arange(0, np.shape(price_traj)[0], int(plot_trajectories_ratio*np.shape(price_traj)[0])):
-                    plt.plot(np.arange(0, np.shape(price_traj)[1] , 1), price_traj[k, :], alpha=0.3)
+                    plt.plot(np.arange(0, np.shape(price_traj)[1] , 1), price_traj[k, :], alpha=alpha_trajectories)
             plt.show()
 
         elif len(self.underlyings) == 2:
             if method == 'RTM':
                 raise Exception('plot of RTM exercise times is not supported')
             elif not hasattr(self, 'ET_' + method):
                 raise Exception('''You haven't calculated price with .''' + method + ''' yet or chosen pricing method doesn't exist''')
@@ -717,42 +722,48 @@
                 rows, cols = np.shape(self.LS_price_trajectories)[1:3]
                 ET_TF = self.ET_LS.astype(bool)
                 t = np.reshape(np.tile(np.arange(0, cols), rows), (rows, cols))[ET_TF]
                 X = self.LS_price_trajectories[0].to_numpy()[ET_TF]
                 Y = self.LS_price_trajectories[1].to_numpy()[ET_TF]
                 price_traj = self.LS_price_trajectories
             elif method == 'ssp':
-                rows, cols = np.shape(self.ssp_price_trajectories)[1:3]
+
+                rows, cols = np.shape(self.ssp_price_trajectories)[0:2]
                 ET_TF = self.ET_ssp.astype(bool)
-                np.reshape(np.tile(np.arange(0, cols), rows), (rows, cols))
-                t = np.reshape(np.tile(np.arange(0, cols), rows), (rows, rows))[ET_TF]
-                X = self.LS_price_trajectories[0][ET_TF]
-                Y = self.LS_price_trajectories[1][ET_TF]
+                t = np.reshape(np.tile(np.arange(0, cols), rows), (rows, cols))[ET_TF]
+                X = self.ssp_price_trajectories[:,:,0][ET_TF]
+                Y = self.ssp_price_trajectories[:,:,1][ET_TF]
                 price_traj = self.ssp_price_trajectories
 
             fig1 = plt.figure(1)
             ax1 = fig1.add_subplot(111, projection='3d')
-            ax1.scatter(t, X, Y, color='green', alpha=0.1)
+            ax1.scatter(t, X, Y, color='green', alpha=alpha_exercise_moments)
 
-            # Increase the size of the axes
-            ax1.xaxis._axinfo['juggled'] = (0, 0, 2)
-            ax1.yaxis._axinfo['juggled'] = (1, 1, 2)
-            ax1.zaxis._axinfo['juggled'] = (2, 2, 2)
-
-            # Add labels to the axes
-            ax1.set_xlabel('t')
-            ax1.set_ylabel('S2')
-            ax1.set_zlabel('S1')
+            ax1.set_title("Exercise moments", fontsize=40)
+
+            # Set x, y, and z labels with adjusted size
+            ax1.set_xlabel("Time", fontsize=30, labelpad= 20)
+            ax1.set_ylabel("1st asset price", fontsize=30, labelpad= 20)
+            ax1.set_zlabel("2nd asset price", fontsize=30, labelpad= 20)
+
+            # Increase the size of tick labels on all axes
+            ax1.tick_params(axis='x', labelsize=25)
+            ax1.tick_params(axis='y', labelsize=25)
+            ax1.tick_params(axis='z', labelsize=25)
 
             #Plot trajectories
             if plot_trajectories_ratio == 0:
                 pass
             else:
-                for k in np.arange(0, np.shape(price_traj)[1], int(plot_trajectories_ratio*np.shape(price_traj)[1])):
-                    plt.plot(np.arange(0, cols, 1), price_traj[0].to_numpy()[k, :],price_traj[1].to_numpy()[k, :], alpha=0.5)
+                if method == 'LS':
+                    for k in np.arange(0, np.shape(price_traj)[1], int(plot_trajectories_ratio*np.shape(price_traj)[1])):
+                        plt.plot(np.arange(0, cols, 1), price_traj[0].to_numpy()[k, :],price_traj[1].to_numpy()[k, :], alpha=alpha_trajectories)
+                elif method == 'ssp':
+                    for k in np.arange(0, np.shape(price_traj)[0], int(plot_trajectories_ratio*np.shape(price_traj)[1])):
+                        plt.plot(np.arange(0, cols, 1), price_traj[k,:,0],price_traj[k,:,1], alpha=alpha_trajectories)
             plt.show()
         else:
             raise Exception('Exercise times for options based on 3 or more assets cannot be visualized')
 
     def hist_optimal_exercise(self, method):
         if method == 'RTM':
             raise Exception('plot of RTM exercise times is not supported')
@@ -768,17 +779,24 @@
         else:
             if method == 'LS':
                 price_traj = self.LS_price_trajectories[0]
             elif method == 'ssp':
                 price_traj = self.ssp_price_trajectories[0]
 
         if method == 'LS':
-            density, bins = np.histogram(np.argmax(self.ET_LS, axis=1), bins=np.shape(price_traj)[1])
+            v = np.argmax(self.ET_LS, axis=1)
+            pe = str(100 * np.round(np.mean(v != 0), 3))
+            v = v[v != 0]
         elif method == 'ssp':
-            density, bins = np.histogram(np.argmax(self.ET_ssp, axis=1), bins=np.shape(price_traj)[1])
-
-        plt.hist(density, bins)
+            v = np.argmax(self.ET_ssp, axis=1)
+            pe = str(100 * np.round(np.mean(v != 0), 3))
+            v = v[v != 0]
+
+        plt.hist(v, bins=np.arange(0, np.shape(price_traj)[1]))
+        plt.title(pe + "% of options have been exercised", fontsize=35)
+        plt.text(0.5, 1.05, "Optimal exercise moments", fontsize=40, ha='center', transform=plt.gca().transAxes)
+        plt.xlabel("Time", fontsize=32)
+        plt.ylabel("Density", fontsize=32, labelpad=15)
+        plt.xticks(fontsize=30)
+        plt.yticks(fontsize=30)
         plt.show()
 
-
-
-
```

### Comparing `american_options-0.1.4/american_options/payoffs.py` & `american_options-0.1.5/american_options/payoffs.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.4/american_options/underlying.py` & `american_options-0.1.5/american_options/underlying.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.4/american_options.egg-info/PKG-INFO` & `american_options-0.1.5/american_options.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: american-options
-Version: 0.1.4
-Summary: Added new payoffs
+Version: 0.1.5
+Summary: Exercise time plotting updated
 Home-page: https://american_options.readthedocs.io/
 Author: Przemysław Adamski, Katarzyna Hasal, Kacper Toczek
 Author-email: kat.hasal99@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `american_options-0.1.4/setup.py` & `american_options-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Get the long description on pypi from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="american_options",
-    version="0.1.4",
-    description="Added new payoffs",
+    version="0.1.5",
+    description="Exercise time plotting updated",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://american_options.readthedocs.io/",
     author="Przemysław Adamski, Katarzyna Hasal, Kacper Toczek",
     author_email="kat.hasal99@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
```

