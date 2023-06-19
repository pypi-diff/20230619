# Comparing `tmp/alphaml-0.1.1.tar.gz` & `tmp/alphaml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaml-0.1.1.tar", last modified: Tue May 23 21:04:28 2023, max compression
+gzip compressed data, was "alphaml-0.1.2.tar", last modified: Mon Jun 19 20:51:40 2023, max compression
```

## Comparing `alphaml-0.1.1.tar` & `alphaml-0.1.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 21:04:28.288392 alphaml-0.1.1/
--rw-rw-rw-   0        0        0    11525 2023-05-23 18:52:45.000000 alphaml-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      252 2023-05-23 21:04:28.287382 alphaml-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-05-02 08:14:09.000000 alphaml-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 21:04:27.998311 alphaml-0.1.1/alphaml/
--rw-rw-rw-   0        0        0      333 2023-05-23 19:28:58.000000 alphaml-0.1.1/alphaml/__init__.py
--rw-rw-rw-   0        0        0     9510 2023-05-23 19:37:21.000000 alphaml-0.1.1/alphaml/guip.py
--rw-rw-rw-   0        0        0    31835 2023-05-23 19:28:58.000000 alphaml-0.1.1/alphaml/guir.py
-drwxrwxrwx   0        0        0        0 2023-05-23 21:04:28.162985 alphaml-0.1.1/alphaml/models/
--rw-rw-rw-   0        0        0      565 2023-05-04 18:19:19.000000 alphaml-0.1.1/alphaml/models/__init__.py
--rw-rw-rw-   0        0        0    25609 2023-05-14 20:45:29.000000 alphaml-0.1.1/alphaml/models/abc.py
--rw-rw-rw-   0        0        0     1593 2023-05-04 20:39:02.000000 alphaml-0.1.1/alphaml/models/all.py
--rw-rw-rw-   0        0        0    25464 2023-05-14 21:34:38.000000 alphaml-0.1.1/alphaml/models/cbc.py
--rw-rw-rw-   0        0        0    24851 2023-05-14 21:34:38.000000 alphaml-0.1.1/alphaml/models/etc.py
--rw-rw-rw-   0        0        0    25120 2023-05-14 21:34:38.000000 alphaml-0.1.1/alphaml/models/gbc.py
--rw-rw-rw-   0        0        0    25189 2023-05-14 21:34:38.000000 alphaml-0.1.1/alphaml/models/hgb.py
--rw-rw-rw-   0        0        0    25676 2023-05-14 21:34:38.000000 alphaml-0.1.1/alphaml/models/lgb.py
--rw-rw-rw-   0        0        0    24492 2023-05-21 09:54:17.000000 alphaml-0.1.1/alphaml/models/mlp.py
--rw-rw-rw-   0        0        0    24855 2023-05-14 21:34:38.000000 alphaml-0.1.1/alphaml/models/rfc.py
--rw-rw-rw-   0        0        0    25045 2023-05-14 21:34:38.000000 alphaml-0.1.1/alphaml/models/sen.py
--rw-rw-rw-   0        0        0    24722 2023-05-14 21:34:38.000000 alphaml-0.1.1/alphaml/models/sl1.py
--rw-rw-rw-   0        0        0    24723 2023-05-14 21:59:43.000000 alphaml-0.1.1/alphaml/models/sl2.py
--rw-rw-rw-   0        0        0    24591 2023-05-14 22:00:33.000000 alphaml-0.1.1/alphaml/models/svc.py
--rw-rw-rw-   0        0        0    26914 2023-05-14 22:01:54.000000 alphaml-0.1.1/alphaml/models/svn.py
--rw-rw-rw-   0        0        0    34624 2023-05-16 06:46:55.000000 alphaml-0.1.1/alphaml/models/tab.py
--rw-rw-rw-   0        0        0    26221 2023-05-14 22:02:29.000000 alphaml-0.1.1/alphaml/models/xgb.py
--rw-rw-rw-   0        0        0     3387 2023-05-23 19:30:18.000000 alphaml-0.1.1/alphaml/pred.py
--rw-rw-rw-   0        0        0     6768 2023-05-21 15:19:32.000000 alphaml-0.1.1/alphaml/run.py
-drwxrwxrwx   0        0        0        0 2023-05-23 21:04:28.213106 alphaml-0.1.1/alphaml/utils/
--rw-rw-rw-   0        0        0      141 2023-05-04 20:41:56.000000 alphaml-0.1.1/alphaml/utils/__init__.py
--rw-rw-rw-   0        0        0    10368 2023-05-14 22:05:30.000000 alphaml-0.1.1/alphaml/utils/all_ml.py
-drwxrwxrwx   0        0        0        0 2023-05-23 21:04:28.286415 alphaml-0.1.1/alphaml/utils/binary_tabnet/
--rw-rw-rw-   0        0        0      168 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/__init__.py
--rw-rw-rw-   0        0        0    24787 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/abstract_model.py
--rw-rw-rw-   0        0        0     8453 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/callbacks.py
--rw-rw-rw-   0        0        0    13838 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/metrics.py
--rw-rw-rw-   0        0        0    12673 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/multiclass_utils.py
--rw-rw-rw-   0        0        0    12873 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/pretraining.py
--rw-rw-rw-   0        0        0     3176 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/pretraining_utils.py
--rw-rw-rw-   0        0        0     8540 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/sparsemax.py
--rw-rw-rw-   0        0        0     3185 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/tab_model.py
--rw-rw-rw-   0        0        0    30084 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/tab_network.py
--rw-rw-rw-   0        0        0    10875 2023-04-23 15:35:43.000000 alphaml-0.1.1/alphaml/utils/binary_tabnet/utils.py
--rw-rw-rw-   0        0        0     8367 2023-05-12 12:07:13.000000 alphaml-0.1.1/alphaml/utils/deeplink.py
--rw-rw-rw-   0        0        0    14989 2023-05-14 22:13:10.000000 alphaml-0.1.1/alphaml/utils/metrics.py
--rw-rw-rw-   0        0        0    12988 2023-05-19 13:08:33.000000 alphaml-0.1.1/alphaml/utils/prep.py
--rw-rw-rw-   0        0        0    19536 2023-05-23 19:40:26.000000 alphaml-0.1.1/alphaml/utils/run_model.py
--rw-rw-rw-   0        0        0    32116 2023-05-23 19:39:22.000000 alphaml-0.1.1/alphaml/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 21:04:28.016510 alphaml-0.1.1/alphaml.egg-info/
--rw-rw-rw-   0        0        0      252 2023-05-23 21:04:27.000000 alphaml-0.1.1/alphaml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1283 2023-05-23 21:04:27.000000 alphaml-0.1.1/alphaml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 21:04:27.000000 alphaml-0.1.1/alphaml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2023-05-23 21:04:27.000000 alphaml-0.1.1/alphaml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 21:04:27.000000 alphaml-0.1.1/alphaml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 21:04:28.288392 alphaml-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1592 2023-05-23 20:37:04.000000 alphaml-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:51:40.161402 alphaml-0.1.2/
+-rw-rw-rw-   0        0        0    11525 2023-05-23 18:52:45.000000 alphaml-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-06-19 20:51:40.161402 alphaml-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-05-02 08:14:09.000000 alphaml-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 20:51:40.098491 alphaml-0.1.2/alphaml/
+-rw-rw-rw-   0        0        0      333 2023-06-19 20:46:00.000000 alphaml-0.1.2/alphaml/__init__.py
+-rw-rw-rw-   0        0        0     9510 2023-05-23 19:37:21.000000 alphaml-0.1.2/alphaml/guip.py
+-rw-rw-rw-   0        0        0    31867 2023-05-26 21:59:34.000000 alphaml-0.1.2/alphaml/guir.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:51:40.145767 alphaml-0.1.2/alphaml/models/
+-rw-rw-rw-   0        0        0      565 2023-05-04 18:19:19.000000 alphaml-0.1.2/alphaml/models/__init__.py
+-rw-rw-rw-   0        0        0    25609 2023-05-14 20:45:29.000000 alphaml-0.1.2/alphaml/models/abc.py
+-rw-rw-rw-   0        0        0     1593 2023-05-04 20:39:02.000000 alphaml-0.1.2/alphaml/models/all.py
+-rw-rw-rw-   0        0        0    25464 2023-05-14 21:34:38.000000 alphaml-0.1.2/alphaml/models/cbc.py
+-rw-rw-rw-   0        0        0    24851 2023-05-14 21:34:38.000000 alphaml-0.1.2/alphaml/models/etc.py
+-rw-rw-rw-   0        0        0    25120 2023-05-14 21:34:38.000000 alphaml-0.1.2/alphaml/models/gbc.py
+-rw-rw-rw-   0        0        0    25189 2023-05-14 21:34:38.000000 alphaml-0.1.2/alphaml/models/hgb.py
+-rw-rw-rw-   0        0        0    25676 2023-05-14 21:34:38.000000 alphaml-0.1.2/alphaml/models/lgb.py
+-rw-rw-rw-   0        0        0    24492 2023-05-21 09:54:17.000000 alphaml-0.1.2/alphaml/models/mlp.py
+-rw-rw-rw-   0        0        0    24855 2023-05-14 21:34:38.000000 alphaml-0.1.2/alphaml/models/rfc.py
+-rw-rw-rw-   0        0        0    25045 2023-05-14 21:34:38.000000 alphaml-0.1.2/alphaml/models/sen.py
+-rw-rw-rw-   0        0        0    24722 2023-05-14 21:34:38.000000 alphaml-0.1.2/alphaml/models/sl1.py
+-rw-rw-rw-   0        0        0    24723 2023-05-14 21:59:43.000000 alphaml-0.1.2/alphaml/models/sl2.py
+-rw-rw-rw-   0        0        0    24591 2023-05-14 22:00:33.000000 alphaml-0.1.2/alphaml/models/svc.py
+-rw-rw-rw-   0        0        0    26914 2023-05-14 22:01:54.000000 alphaml-0.1.2/alphaml/models/svn.py
+-rw-rw-rw-   0        0        0    34624 2023-05-16 06:46:55.000000 alphaml-0.1.2/alphaml/models/tab.py
+-rw-rw-rw-   0        0        0    26221 2023-05-14 22:02:29.000000 alphaml-0.1.2/alphaml/models/xgb.py
+-rw-rw-rw-   0        0        0     3517 2023-05-27 10:43:20.000000 alphaml-0.1.2/alphaml/pred.py
+-rw-rw-rw-   0        0        0     6892 2023-05-28 06:23:31.000000 alphaml-0.1.2/alphaml/run.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:51:40.145767 alphaml-0.1.2/alphaml/utils/
+-rw-rw-rw-   0        0        0      141 2023-05-04 20:41:56.000000 alphaml-0.1.2/alphaml/utils/__init__.py
+-rw-rw-rw-   0        0        0    10368 2023-05-14 22:05:30.000000 alphaml-0.1.2/alphaml/utils/all_ml.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:51:40.161402 alphaml-0.1.2/alphaml/utils/binary_tabnet/
+-rw-rw-rw-   0        0        0      168 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/__init__.py
+-rw-rw-rw-   0        0        0    24787 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/abstract_model.py
+-rw-rw-rw-   0        0        0     8453 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/callbacks.py
+-rw-rw-rw-   0        0        0    13838 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/metrics.py
+-rw-rw-rw-   0        0        0    12673 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/multiclass_utils.py
+-rw-rw-rw-   0        0        0    12873 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/pretraining.py
+-rw-rw-rw-   0        0        0     3176 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/pretraining_utils.py
+-rw-rw-rw-   0        0        0     8540 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/sparsemax.py
+-rw-rw-rw-   0        0        0     3185 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/tab_model.py
+-rw-rw-rw-   0        0        0    30084 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/tab_network.py
+-rw-rw-rw-   0        0        0    10875 2023-04-23 15:35:43.000000 alphaml-0.1.2/alphaml/utils/binary_tabnet/utils.py
+-rw-rw-rw-   0        0        0     8367 2023-05-12 12:07:13.000000 alphaml-0.1.2/alphaml/utils/deeplink.py
+-rw-rw-rw-   0        0        0    15064 2023-05-30 13:58:14.000000 alphaml-0.1.2/alphaml/utils/metrics.py
+-rw-rw-rw-   0        0        0    12641 2023-05-27 10:41:01.000000 alphaml-0.1.2/alphaml/utils/prep.py
+-rw-rw-rw-   0        0        0    19536 2023-05-23 19:40:26.000000 alphaml-0.1.2/alphaml/utils/run_model.py
+-rw-rw-rw-   0        0        0    32112 2023-05-27 11:06:20.000000 alphaml-0.1.2/alphaml/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:51:40.114117 alphaml-0.1.2/alphaml.egg-info/
+-rw-rw-rw-   0        0        0      252 2023-06-19 20:51:39.000000 alphaml-0.1.2/alphaml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1283 2023-06-19 20:51:39.000000 alphaml-0.1.2/alphaml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:51:39.000000 alphaml-0.1.2/alphaml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-06-19 20:51:39.000000 alphaml-0.1.2/alphaml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 20:51:39.000000 alphaml-0.1.2/alphaml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 20:51:40.161402 alphaml-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1592 2023-06-19 20:47:29.000000 alphaml-0.1.2/setup.py
```

### Comparing `alphaml-0.1.1/LICENSE` & `alphaml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/guip.py` & `alphaml-0.1.2/alphaml/guip.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/guir.py` & `alphaml-0.1.2/alphaml/guir.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,15 +463,15 @@
 
 # Create a frame for the dropdown/entry fields
 c03r915_frame = tk.Frame(root, borderwidth=2, relief="groove")
 # params_frame = tk.Frame(root, bd=1, relief="sunken")
 c03r915_frame.grid(row=9, column=0, columnspan=4, rowspan=10, padx=5, pady=5, sticky="w")
 
 # Add a label to the frame for the title
-c03r915_label = tk.Label(c03r915_frame, text="Data preprocessing", font=("Helvetica", 12, "bold"), fg="blue")
+c03r915_label = tk.Label(c03r915_frame, text="Feature selection", font=("Helvetica", 12, "bold"), fg="blue")
 c03r915_label.grid(row=0, column=0, columnspan=4, pady=5)
 # feature_label.config(width=50)
 
 
 # Add a dropdown list for the Feature selection method
 features_label = tk.Label(c03r915_frame, text="Feature selection method 1:", font=("Helvetica", 10, "bold"), anchor="e")
 features_label.grid(row=1, column=0, padx=5, pady=3)
@@ -480,37 +480,37 @@
                      'RecursiveFeatElim', 'SeqFeatSel', 'ModelX', 'Suggested']
 features_var = tk.StringVar(root)
 features_var.set(features_methods[0])
 features_dropdown = tk.OptionMenu(c03r915_frame, features_var, *features_methods)
 features_dropdown.grid(row=1, column=1, padx=5, pady=5)
 features_dropdown.config(width=18)  # Set the width of the widget
 
-features2_label = tk.Label(c03r915_frame, text="Method 2:", font=("Helvetica", 10, "bold"), anchor="e")
+features2_label = tk.Label(c03r915_frame, text="Method 2 (optional):", font=("Helvetica", 10, "bold"), anchor="e")
 features2_label.grid(row=2, column=0, padx=5, pady=5)
 features2_label.config(width=22)
 features2_methods = ['HVF', 'MedianMAD', 'SelByPCA', 'RandomProjection', 'SelByClustering', 'SelByNMF', 'SelectByRF',
                      'RecursiveFeatElim', 'SeqFeatSel', 'ModelX', 'None']
 features2_var = tk.StringVar(root)
 features2_var.set(features2_methods[10])
 features2_dropdown = tk.OptionMenu(c03r915_frame, features2_var, *features2_methods)
 features2_dropdown.grid(row=2, column=1, padx=5, pady=5)
 features2_dropdown.config(width=18)  # Set the width of the widget
 
-features3_label = tk.Label(c03r915_frame, text="Method 3:", font=("Helvetica", 10, "bold"), anchor="e")
+features3_label = tk.Label(c03r915_frame, text="Method 3 (optional):", font=("Helvetica", 10, "bold"), anchor="e")
 features3_label.grid(row=3, column=0, padx=5, pady=5)
 features3_label.config(width=22)
 features3_methods = ['HVF', 'MedianMAD', 'SelByPCA', 'RandomProjection', 'SelByClustering', 'SelByNMF', 'SelectByRF',
                      'RecursiveFeatElim', 'SeqFeatSel', 'ModelX', 'RemoveHighCorrFeat', 'IterativeFeatSel', 'None']
 features3_var = tk.StringVar(root)
 features3_var.set(features3_methods[12])
 features3_dropdown = tk.OptionMenu(c03r915_frame, features3_var, *features3_methods)
 features3_dropdown.grid(row=3, column=1, padx=5, pady=5)
 features3_dropdown.config(width=18)  # Set the width of the widget
 
-features4_label = tk.Label(c03r915_frame, text="Method 4:", font=("Helvetica", 10, "bold"), anchor="e")
+features4_label = tk.Label(c03r915_frame, text="Method 4 (optional):", font=("Helvetica", 10, "bold"), anchor="e")
 features4_label.grid(row=4, column=0, padx=5, pady=5)
 features4_label.config(width=22)
 features4_methods = ['HVF', 'MedianMAD', 'SelByPCA', 'RandomProjection', 'SelByClustering', 'SelByNMF', 'SelectByRF',
                      'RecursiveFeatElim', 'SeqFeatSel', 'ModelX', 'RemoveHighCorrFeat', 'IterativeFeatSel', 'None']
 features4_var = tk.StringVar(root)
 features4_var.set(features3_methods[12])
 features4_dropdown = tk.OptionMenu(c03r915_frame, features4_var, *features4_methods)
@@ -549,15 +549,15 @@
 n_components_label.grid(row=8, column=0, padx=5, pady=5)
 n_components_var = tk.IntVar(root)
 n_components_var.set(500)
 n_components_entry = tk.Entry(c03r915_frame, textvariable=n_components_var)
 n_components_entry.config(width=22)  # Set the width of the widget
 n_components_entry.grid(row=8, column=1, padx=5, pady=5)
 
-min_sel_features_rfe_label = tk.Label(c03r915_frame, text="RFE Min features:", font=("Helvetica", 10, "bold"), anchor="e")
+min_sel_features_rfe_label = tk.Label(c03r915_frame, text="RFE min features:", font=("Helvetica", 10, "bold"), anchor="e")
 min_sel_features_rfe_label.config(width=22)
 min_sel_features_rfe_label.grid(row=9, column=0, padx=5, pady=5)
 min_sel_features_rfe_var = tk.IntVar(root)
 min_sel_features_rfe_var.set(10)
 min_sel_features_rfe_entry = tk.Entry(c03r915_frame, textvariable=min_sel_features_rfe_var)
 min_sel_features_rfe_entry.config(width=22)  # Set the width of the widget
 min_sel_features_rfe_entry.grid(row=9, column=1, padx=9, pady=5)
@@ -570,63 +570,63 @@
 flavor_methods = ['log2', 'log10', 'ln', 'None']
 flavor_var = tk.StringVar(root)
 flavor_var.set(flavor_methods[0])
 flavor_dropdown = tk.OptionMenu(c03r915_frame, flavor_var, *flavor_methods)
 flavor_dropdown.config(width=18)
 flavor_dropdown.grid(row=1, column=3, padx=5, pady=5)
 
-topgenes_label = tk.Label(c03r915_frame, text="HVF Top features:", font=("Helvetica", 10, "bold"), anchor="e")
+topgenes_label = tk.Label(c03r915_frame, text="HVF top features:", font=("Helvetica", 10, "bold"), anchor="e")
 topgenes_label.config(width=22)
 topgenes_label.grid(row=2, column=2, padx=5, pady=5)
 topgenes_var = tk.IntVar(root)
 topgenes_var.set(0)
 topgenes_entry = tk.Entry(c03r915_frame, textvariable=topgenes_var)
 topgenes_entry.config(width=22)  # Set the width of the widget
 topgenes_entry.grid(row=2, column=3, padx=5, pady=5)
 
-disp_label = tk.Label(c03r915_frame, text="HVG Min dispersion:", font=("Helvetica", 10, "bold"), anchor="e")
+disp_label = tk.Label(c03r915_frame, text="HVG min dispersion:", font=("Helvetica", 10, "bold"), anchor="e")
 disp_label.config(width=22)
 disp_label.grid(row=3, column=2, padx=5, pady=5)
 disp_var = tk.DoubleVar(root)
 disp_var.set(1.5)
 disp_entry = tk.Entry(c03r915_frame, textvariable=disp_var)
 disp_entry.config(width=22)  # Set the width of the widget
 disp_entry.grid(row=3, column=3, padx=5, pady=5)
 
 
-max_features_label = tk.Label(c03r915_frame, text="RF Maximum features:", font=("Helvetica", 10, "bold"), anchor="e")
+max_features_label = tk.Label(c03r915_frame, text="RF maximum features:", font=("Helvetica", 10, "bold"), anchor="e")
 max_features_label.config(width=22)
 max_features_label.grid(row=4, column=2, padx=5, pady=5)
 max_features_var = tk.IntVar(root)
 max_features_var.set(0)
 max_features_entry = tk.Entry(c03r915_frame, textvariable=max_features_var)
 max_features_entry.config(width=22)  # Set the width of the widget
 max_features_entry.grid(row=4, column=3, padx=9, pady=5)
 
-threshold_label = tk.Label(c03r915_frame, text="RF Threshold(mean/median):", font=("Helvetica", 9, "bold"), anchor="e")
+threshold_label = tk.Label(c03r915_frame, text="RF threshold(mean/median):", font=("Helvetica", 9, "bold"), anchor="e")
 threshold_label.config(width=25)
 threshold_label.grid(row=5, column=2, padx=5, pady=5)
 threshold_var = tk.StringVar(root)
 threshold_var.set("1.5*mean")
 threshold_entry = tk.Entry(c03r915_frame, textvariable=threshold_var)
 threshold_entry.config(width=22)  # Set the width of the widget
 threshold_entry.grid(row=5, column=3, padx=9, pady=5)
 
 # params_label.config(width=50)
-min_sel_features_label = tk.Label(c03r915_frame, text="ModelX Min feature:", font=("Helvetica", 10, "bold"),
+min_sel_features_label = tk.Label(c03r915_frame, text="ModelX min feature:", font=("Helvetica", 10, "bold"),
                                   anchor="e")
 min_sel_features_label.config(width=22)
 min_sel_features_label.grid(row=6, column=2, padx=12, pady=5)
 min_sel_features_var = tk.IntVar(root)
 min_sel_features_var.set(10)
 min_sel_features_entry = tk.Entry(c03r915_frame, textvariable=min_sel_features_var)
 min_sel_features_entry.config(width=22)  # Set the width of the widget
 min_sel_features_entry.grid(row=6, column=3, padx=9, pady=5)
 
-latent_dim_label = tk.Label(c03r915_frame, text="ModelX Latent dimensions:", font=("Helvetica", 10, "bold"), anchor="e")
+latent_dim_label = tk.Label(c03r915_frame, text="ModelX latent dimensions:", font=("Helvetica", 10, "bold"), anchor="e")
 latent_dim_label.config(width=22)
 latent_dim_label.grid(row=7, column=2, padx=5, pady=5)
 latent_dim_var = tk.IntVar(root)
 latent_dim_var.set(32)
 latent_dim_entry = tk.Entry(c03r915_frame, textvariable=latent_dim_var)
 latent_dim_entry.config(width=22)  # Set the width of the widget
 latent_dim_entry.grid(row=7, column=3, padx=9, pady=5)
@@ -636,15 +636,15 @@
 fdr_label.grid(row=8, column=2, padx=5, pady=5)
 fdr_var = tk.DoubleVar(root)
 fdr_var.set(0.25)
 fdr_entry = tk.Entry(c03r915_frame, textvariable=fdr_var)
 fdr_entry.config(width=22)  # Set the width of the widget
 fdr_entry.grid(row=8, column=3, padx=9, pady=5)
 
-min_sel_features_sfs_label = tk.Label(c03r915_frame, text="SFS Min features:", font=("Helvetica", 10, "bold"), anchor="e")
+min_sel_features_sfs_label = tk.Label(c03r915_frame, text="SFS min features:", font=("Helvetica", 10, "bold"), anchor="e")
 min_sel_features_sfs_label.config(width=22)
 min_sel_features_sfs_label.grid(row=9, column=2, padx=5, pady=3)
 min_sel_features_sfs_var = tk.IntVar(root)
 min_sel_features_sfs_var.set(10)
 min_sel_features_sfs_entry = tk.Entry(c03r915_frame, textvariable=min_sel_features_sfs_var)
 min_sel_features_sfs_entry.config(width=22)  # Set the width of the widget
 min_sel_features_sfs_entry.grid(row=9, column=3, padx=9, pady=5)
```

### Comparing `alphaml-0.1.1/alphaml/models/__init__.py` & `alphaml-0.1.2/alphaml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/abc.py` & `alphaml-0.1.2/alphaml/models/abc.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/all.py` & `alphaml-0.1.2/alphaml/models/all.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/cbc.py` & `alphaml-0.1.2/alphaml/models/cbc.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/etc.py` & `alphaml-0.1.2/alphaml/models/etc.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/gbc.py` & `alphaml-0.1.2/alphaml/models/gbc.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/hgb.py` & `alphaml-0.1.2/alphaml/models/hgb.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/lgb.py` & `alphaml-0.1.2/alphaml/models/lgb.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/mlp.py` & `alphaml-0.1.2/alphaml/models/mlp.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/rfc.py` & `alphaml-0.1.2/alphaml/models/rfc.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/sen.py` & `alphaml-0.1.2/alphaml/models/sen.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/sl1.py` & `alphaml-0.1.2/alphaml/models/sl1.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/sl2.py` & `alphaml-0.1.2/alphaml/models/sl2.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/svc.py` & `alphaml-0.1.2/alphaml/models/svc.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/svn.py` & `alphaml-0.1.2/alphaml/models/svn.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/tab.py` & `alphaml-0.1.2/alphaml/models/tab.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/models/xgb.py` & `alphaml-0.1.2/alphaml/models/xgb.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/pred.py` & `alphaml-0.1.2/alphaml/pred.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,24 @@
     log_level = logging.INFO
     log_file_path = os.path.abspath(result_path + "alphaPred_run.log")
     # Configure logging settings
     logging.basicConfig(filename=log_file_path,
                         level=log_level,
                         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
-    model, test_data = test_data_preprocessing(data_path=data_path, normalization=normalization)
+    model, test_data = test_data_preprocessing(data_path=data_path,
+                                               normalization=normalization)
     test_data.index.name = 'IndexName'
     algorithm = model.__class__.__name__
     path = result_path
     sampling_method = ''
     param_search = ''
     control_fitting = ''
     p_name = path + col_label + '_' + sampling_method + '_' + param_search + '_' + algorithm + '_fit_' + control_fitting
+    test_data.to_csv(p_name + 'normalized_test_data.csv')
     test_data_pred = model.predict(test_data.to_numpy())
     test_data_proba = model.predict_proba(test_data.to_numpy())[:, 1] if hasattr(model, "predict_proba") else None
     test_data_pred_df = pd.DataFrame(test_data_pred, columns=['predictions'])
     if test_data_proba is not None:
         test_data_proba_df = pd.DataFrame(test_data_proba, columns=['pred_proba'])
         combined_df = pd.concat([test_data_pred_df, test_data_proba_df], axis=1)
     else:
@@ -61,15 +63,17 @@
               path=result_path,
               sampling_method=sampling_method,
               param_search=param_search,
               algorithm=algorithm,
               col_label=col_label,
               control_fitting=control_fitting
               )
-    elif run_lime == 'Yes':
+    else:
+        pass
+    if run_lime == 'Yes':
         lime_(model=model,
               x_test=test_data,
               path=result_path,
               sampling_method=sampling_method,
               param_search=param_search,
               algorithm=algorithm,
               col_label=col_label,
```

### Comparing `alphaml-0.1.1/alphaml/run.py` & `alphaml-0.1.2/alphaml/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 
     # Check the availability of result and log folder otherwise create
     user_documents = os.path.expanduser("~/Documents")
     data_path = os.path.join(user_documents, "alphaML_data/")
     result_path = os.path.join(user_documents, "alphaML_results/")
     if not os.path.exists(result_path):
         os.makedirs(result_path)
-
+    f_name = col_label + '_' + sampling_method + '_' + param_search + '_' + model_name + '_fit_' + control_fitting
     # Set the log level (DEBUG, INFO, WARNING, ERROR, or CRITICAL)
     log_level = logging.INFO
-    log_file_path = os.path.abspath(result_path + "alphaML_run.log")
+    log_file_path = os.path.abspath(result_path + f"{f_name}_alphaML_run.log")
     # Configure logging settings
     logging.basicConfig(filename=log_file_path,
                         level=log_level,
                         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
     start = time.strftime("%Y-%m-%d %H:%M:%S")
     warnings.filterwarnings("ignore")
```

### Comparing `alphaml-0.1.1/alphaml/utils/all_ml.py` & `alphaml-0.1.2/alphaml/utils/all_ml.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/abstract_model.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/abstract_model.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/callbacks.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/metrics.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/metrics.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/multiclass_utils.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/multiclass_utils.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/pretraining.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/pretraining.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/pretraining_utils.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/pretraining_utils.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/sparsemax.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/sparsemax.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/tab_model.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/tab_model.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/tab_network.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/tab_network.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/binary_tabnet/utils.py` & `alphaml-0.1.2/alphaml/utils/binary_tabnet/utils.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/deeplink.py` & `alphaml-0.1.2/alphaml/utils/deeplink.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/metrics.py` & `alphaml-0.1.2/alphaml/utils/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,30 +214,33 @@
 
         return metrics
 
 # Combined Cohen's kappa and MCC scorer
 
 
 def kappa_mcc_error(y_true, y_pred):
-    kappa = cohen_kappa_score(y_true, y_pred)
-    mcc = matthews_corrcoef(y_true, y_pred)
-    return 1-(kappa*mcc)**0.5
+    k = cohen_kappa_score(y_true, y_pred)
+    m = matthews_corrcoef(y_true, y_pred)
+    return 1 - (k*m)**0.5
 
 # Make a custom scorer to use for optimization considering test and train scores
 
 
 def custom_score(model, x_train, y_train, x_test, y_test):
     train_pred = model.predict(x_train)
     test_pred = model.predict(x_test)
 
-    train_score = kappa_mcc_error(y_train, train_pred)
-    test_score = kappa_mcc_error(y_test, test_pred)
-    diff = (train_score - test_score)**2
-    ts = test_score**2
-    return (diff*ts)**0.25
+    train_error = kappa_mcc_error(y_train, train_pred)
+    test_error = kappa_mcc_error(y_test, test_pred)
+    diff = ((train_error - test_error)**2)**0.5
+    if train_error == test_error:
+        cs = test_error
+    else:
+        cs = (diff*test_error)**0.5
+    return cs
 
 # ***************** Confusion Matrix by SKLEARN **********************************
 
 
 def confusion_matrix_(model, x_test, y_true, path, col_label, sampling_method,
                       param_search, axis_labels, algorithm, control_fitting):
 
@@ -311,15 +314,15 @@
     # Calculate RMS of differences between train and test scores
     renamed_test_df = test_df.rename(columns=lambda col: col.replace("Test", "Diff")).drop(drop_metrics)
     renamed_train_df = train_df.rename(columns=lambda col: col.replace("Train", "Diff")).drop(drop_metrics)
     diff = np.mean(np.mean(np.square(renamed_train_df - renamed_test_df), axis=1)) ** 0.5
     # Calculate RMS of test scores losses
     loss_ = np.mean(np.mean(np.square(losses_df.drop(drop_metrics)), axis=1)) ** 0.5
     # Calculate final scores by taking geometric mean, and then making negative log2
-    factor = -1 * np.log2((diff * loss_) ** 0.5)
+    factor = -1 * np.log2(((diff+0.05) * loss_) ** 0.5)
     all_score_df = pd.concat([train_df, test_df, losses_df], axis=1).round(decimals=3)
     all_score_df.loc['NegLog2-RMSL'] = factor  # Negative log2 Root Mean Squared Loss
     return all_score_df, factor
 
 # Export test result with probabilities
```

### Comparing `alphaml-0.1.1/alphaml/utils/prep.py` & `alphaml-0.1.2/alphaml/utils/prep.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,37 +95,39 @@
                                  )
     data_for_feature_selection = pd.read_csv(data_path+'data_for_feature_selection.csv',
                                              index_col=0,
                                              header=0,
                                              sep=',',
                                              low_memory=False
                                              )
-    # Encode labels "Change here drug name if you have a table with multiple drugs
+    # Encode labels
+    pos_class = pos_class.strip().lower()
+    neg_class = neg_class.strip().lower()
     data_labels[column_name] = data_labels[column_name].apply(
         lambda x: int(1) if x.strip().lower() == pos_class else int(0) if x.strip().lower() == neg_class else None)
     labels = data_labels[column_name]
 
-    def apply_fs(feature, df1, df2, labels_, result_path_, fs_name):
+    def apply_(feature, df1, df2, fs_name):
 
         def execute_feature_selection_method(method, kwargs):
             return method(**kwargs)
 
-        def save_and_log_selected_features(feature_, path_, fs_name_):
-            if not feature_:
+        def save_and_log_selected_features(selected_features_):
+            if not selected_features_:
                 raise ValueError(
                     'Method returned empty feature. Please consider an alternative method.')
-            elif isinstance(feature_, Exception):
+            elif isinstance(selected_features_, Exception):
                 raise ValueError(
                     f'Method raised an error. Please consider an alternative method.')
 
-            df = pd.DataFrame(feature_, columns=['Selected features'])
-            df.to_csv(f"{path_}{fs_name_}.csv", index=False)
-            logging.info(f"select by {fs_name_}, and saved as features_{fs_name_}.csv in alphaML_results folder")
+            df = pd.DataFrame(selected_features_, columns=['Selected features'])
+            df.to_csv(f"{result_path}{fs_name}.csv", index=False)
+            logging.info(f"select by {fs_name}, and saved as features_{fs_name}.csv in alphaML_results folder")
 
-        FEATURE_SELECTION_METHODS = {
+        feature_selection_methods = {
             'HVF': {
                 'function': hvf,
                 'kwargs': {'data': df1, 'log_type': log_type, 'n_top_features': n_top_features, 'min_disp': min_disp}
             },
             'MedianMAD': {
                 'function': select_by_mad,
                 'kwargs': {'df': df1}
@@ -148,90 +150,82 @@
             },
             'RemoveHighCorrFeat': {
                 'function': remove_highly_correlated_feat,
                 'kwargs': {'df': df1},
             },
             'SelectByRF': {
                 'function': select_from_rf,
-                'kwargs': {'x_train': df2, 'y_train': labels_, 'threshold': threshold, 'max_features': max_features},
+                'kwargs': {'x_train': df2, 'y_train': labels, 'threshold': threshold, 'max_features': max_features},
             },
             'RecursiveFeatElim': {
                 'function': recursive_feature_elimination,
-                'kwargs': {'x_train': df2, 'y_train': labels_, 'min_sel_features_rfe': min_sel_features_rfe},
+                'kwargs': {'x_train': df2, 'y_train': labels, 'min_sel_features_rfe': min_sel_features_rfe},
             },
             'SeqFeatSel': {
                 'function': seq_feat_sel,
-                'kwargs': {'x_train': df2, 'y_train': labels_, 'min_sel_features_sfs': min_sel_features_sfs},
+                'kwargs': {'x_train': df2, 'y_train': labels, 'min_sel_features_sfs': min_sel_features_sfs},
             },
             'ModelX': {
                 'function': modelx,
-                'kwargs': {'data': df2, 'dataY': labels_, 'latent_dim': latent_dim,
+                'kwargs': {'data': df2, 'dataY': labels, 'latent_dim': latent_dim,
                            'min_sel_features': min_sel_features,
                            'fdr': fdr, 'result_path': result_path},
             },
             'IterativeFeatSel': {
                 'function': iterative_feature_selector,
-                'kwargs': {'x_train': df2, 'y_train': labels_},
+                'kwargs': {'x_train': df2, 'y_train': labels},
             }
         }
         if feature == 'Suggested':
-            selected_features = pd.read_csv(result_path_+'suggested_features.csv',
+            selected_features = pd.read_csv(data_path+'suggested_features.csv',
                                             index_col=None,
                                             header=0,
                                             sep=',',
                                             low_memory=False
                                             ).values.ravel().tolist()
             logging.info("Suggested features is being used")
         elif feature == 'None':
             selected_features = df2.columns.tolist()
-        elif feature in FEATURE_SELECTION_METHODS:
+        elif feature in feature_selection_methods:
             print(f'Selecting features by {feature}')
-            selected_features = execute_feature_selection_method(FEATURE_SELECTION_METHODS[feature]['function'],
-                                                                 FEATURE_SELECTION_METHODS[feature]['kwargs'])
+            selected_features = execute_feature_selection_method(feature_selection_methods[feature]['function'],
+                                                                 feature_selection_methods[feature]['kwargs'])
             if not selected_features:
                 selected_features = df2.columns.tolist()
                 error_txt = f'{feature} failed to generate a feature list, '
                 logging.info(error_txt+f'we reverted the list to the current dataframe index')
                 print(error_txt+f'we reverted the list to the current dataframe index')
             else:
                 selected_features = selected_features
-            save_and_log_selected_features(selected_features, result_path, fs_name)
+            save_and_log_selected_features(selected_features)
         else:
             raise ValueError('Please provide a valid feature selection method!')
 
         return df1[selected_features], df2[selected_features]
 
-    df11, df21 = apply_fs(features,
-                          data_for_feature_selection,
-                          labeled_data,
-                          labels,
-                          result_path,
-                          column_name + '_' + features + '_' + 'None' + '_' + 'None' + '_' + 'None' + '_Feat_M1'
-                          )
-    df12, df22 = apply_fs(features2,
-                          df11,
-                          df21,
-                          labels,
-                          result_path,
-                          column_name + '_' + features + '_' + features2 + '_' + 'None' + '_' + 'None' + '_Feat_M2'
-                          )
-    df13, df23 = apply_fs(features3,
-                          df12,
-                          df22,
-                          labels,
-                          result_path,
-                          column_name + '_' + features + '_' + features2 + '_' + features3 + '_' + 'None' + '_Feat_M3'
-                          )
-    df14, df24 = apply_fs(features4,
-                          df13,
-                          df23,
-                          labels,
-                          result_path,
-                          column_name + '_' + features + '_' + features2 + '_' + features3 + '_' + features4 + '_Feat_M4'
-                          )
+    df11, df21 = apply_(features,
+                        data_for_feature_selection,
+                        labeled_data,
+                        column_name + '_' + features + '_' + 'None' + '_' + 'None' + '_' + 'None' + '_Feat_M1'
+                        )
+    df12, df22 = apply_(features2,
+                        df11,
+                        df21,
+                        column_name + '_' + features + '_' + features2 + '_' + 'None' + '_' + 'None' + '_Feat_M2'
+                        )
+    df13, df23 = apply_(features3,
+                        df12,
+                        df22,
+                        column_name + '_' + features + '_' + features2 + '_' + features3 + '_' + 'None' + '_Feat_M3'
+                        )
+    df14, df24 = apply_(features4,
+                        df13,
+                        df23,
+                        column_name + '_' + features + '_' + features2 + '_' + features3 + '_' + features4 + '_Feat_M4'
+                        )
 
     features_ = df14.columns
     df_labeled = labeled_data[features_]
     df_unlabeled = unlabeled_data[features_]
 
     if normalization == 'min_max':
         # Normalize data using min-max normalization between 0 and 1.
@@ -243,16 +237,16 @@
         sel_unlabeled_data4 = standardize_dataframe(df_unlabeled.T).T
     elif normalization == 'None':
         sel_labeled_data4 = df_labeled
         sel_unlabeled_data4 = df_unlabeled
     else:
         raise ValueError('Please provide a valid normalization method!')
 
-    sel_labeled_data4.to_csv(data_path + 'normalized_labeled_data.csv')
-    sel_unlabeled_data4.to_csv(data_path + 'normalized_unlabeled_data.csv')
+    sel_labeled_data4.to_csv(result_path + column_name + '_' + features + '_normalized_labeled_data.csv')
+    sel_unlabeled_data4.to_csv(result_path + column_name + '_' + features + '_normalized_unlabeled_data.csv')
     return labels, sel_labeled_data4, sel_unlabeled_data4
 
 
 def test_data_preprocessing(data_path,
                             normalization='min_max'):
 
     """
@@ -286,9 +280,9 @@
     elif normalization == 'standardization':
         # Normalize data using min-max normalization between 0 and 1.
         normalized_test_data = standardize_dataframe(selected_test_data.T).T
     elif normalization == 'None':
         normalized_test_data = selected_test_data
     else:
         raise ValueError('Please provide a valid normalization method!')
-    normalized_test_data.to_csv(data_path+'normalized_test_data.csv')
+
     return model, normalized_test_data
```

### Comparing `alphaml-0.1.1/alphaml/utils/run_model.py` & `alphaml-0.1.2/alphaml/utils/run_model.py`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/alphaml/utils/utils.py` & `alphaml-0.1.2/alphaml/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,15 @@
                             TabNetClassifier)
                     ):
         explainer = shap.Explainer(model.predict, x_test.to_numpy())
         shap_values = explainer(x_test, max_evals=round(2*x_test.shape[1]+1))
     else:
         raise ValueError("Unsupported model type")
 
-    with PdfPages(f"{p_name}_X_TEST_SHAP.pdf") as pdf:
+    with PdfPages(f"{p_name}_test_SHAP.pdf") as pdf:
         shap.summary_plot(shap_values, x_test, plot_type='layered_violin', color='#cccccc', show=False)
         plt.title('SHAP layered violin plot gray scale')
         plt.grid(None)
         pdf.savefig(transparent=False, facecolor='auto', edgecolor='auto')
         plt.close()
         shap.summary_plot(shap_values, x_test, plot_type='layered_violin', show=False)
         plt.title('SHAP layered violin plot')
@@ -294,15 +294,15 @@
                                          feature_names=x_test.columns,
                                          class_names=['0', '1'],
                                          mode='classification' if hasattr(model, 'predict_proba') else 'regression',
                                          verbose=False)
     else:
         raise ValueError("Unsupported model type")
 
-    with PdfPages(f"{p_name}_X_TEST_LIME.pdf") as pdf:
+    with PdfPages(f"{p_name}_test_LIME.pdf") as pdf:
         for i in range(len(x_test)):
             if hasattr(model, 'predict_proba'):
                 prob_func = model.predict_proba
             else:
                 prob_func = model.predict
 
             exp = explainer.explain_instance(x_test.iloc[i].values,
@@ -474,15 +474,15 @@
     missing_files = [file for file in csv_files if not os.path.isfile(os.path.join(data_path, file))]
 
     # 2. Check if CSV files are available, else download data.zip
     if missing_files:
         if not is_connected():
             raise ValueError("No internet connection. Please connect to the internet and try again.")
 
-        url_ = "https://drive.google.com/uc?id=1RR26k1gcckinoqwxAPimPJRElpB3P84G&export=download&confirm=no_antivirus"
+        url_ = "https://drive.google.com/uc?id=1v9Bwe4TdXd-20SGKDBqUxwJp0Gzzdetl&export=download&confirm=no_antivirus"
         response = requests.get(url_)
 
         zip_filename = os.path.join(data_path, "data.zip")
         with open(zip_filename, "wb") as zip_file:
             zip_file.write(response.content)
 
         # 3. Unzip and delete the zip file
@@ -490,15 +490,15 @@
             zip_ref.extractall(data_path)
         os.remove(zip_filename)
 
     # 4. Confirm that all files are available, else raise ValueError
     for file in csv_files:
         if not os.path.isfile(os.path.join(data_path, file)):
             raise ValueError(f"{file} is missing. Please download the zip file manually from "
-                             f"'https://drive.google.com/drive/folders/1RR26k1gcckinoqwxAPimPJRElpB3P84G?usp=sharing',"
+                             f"'https://drive.google.com/drive/folders/1v9Bwe4TdXd-20SGKDBqUxwJp0Gzzdetl?usp=sharing',"
                              f"unzip, and put the files in the alphaML_data folder.")
     logging.info("All files are available in the alphaML_data folder.")
     print("All files are available in the alphaML_data folder.")
 
 # Data preprocessing
 # 1. Select from model using Random Forest
 
@@ -791,15 +791,15 @@
     missing_files = [file for file in csv_files if not os.path.isfile(os.path.join(data_path, file))]
 
     # 2. Check if CSV files are available, else download data.zip
     if missing_files:
         if not is_connected():
             raise ValueError("No internet connection. Please connect to the internet and try again.")
 
-        url_ = "https://drive.google.com/uc?id=1oIwrDJCOdVLq650O_bV2RrvnEHb50Uzm&export=download&confirm=no_antivirus"
+        url_ = "https://drive.google.com/uc?id=1Ng5GeY_eLEILgojtnsLoaDCvs7cdApR5&export=download&confirm=no_antivirus"
         response = requests.get(url_)
 
         zip_filename = os.path.join(data_path, "predict.zip")
         with open(zip_filename, "wb") as zip_file:
             zip_file.write(response.content)
 
         # 3. Unzip and delete the zip file
@@ -807,11 +807,11 @@
             zip_ref.extractall(data_path)
         os.remove(zip_filename)
 
     # 4. Confirm that all files are available, else raise ValueError
     for file in csv_files:
         if not os.path.isfile(os.path.join(data_path, file)):
             raise ValueError(f"{file} is missing. Please download the zip file manually from "
-                             f"'https://drive.google.com/drive/folders/1oIwrDJCOdVLq650O_bV2RrvnEHb50Uzm?usp=sharing',"
+                             f"'https://drive.google.com/drive/folders/1Ng5GeY_eLEILgojtnsLoaDCvs7cdApR5?usp=sharing',"
                              f"unzip, and put the files in the alphaPred_data folder.")
     logging.info("All files are available in the alphaML_data folder.")
     print("All files are available in the alphaML_data folder.")
```

### Comparing `alphaml-0.1.1/alphaml.egg-info/SOURCES.txt` & `alphaml-0.1.2/alphaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaml-0.1.1/setup.py` & `alphaml-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                 'You are using Python {0}.{1}'.format(
                     sys.version_info[0], sys.version_info[1])
                 )
 
 # main setup command
 setup(
       name='alphaml',
-      version='0.1.1', # Major.Minor.Patch
+      version='0.1.2', # Major.Minor.Patch
       author='Julhash Kazi',
       author_email='aml@kazilab.se',
       url='https://www.kazilab.se',
       description='Build a CLETE Binary Classification Model',
       license='Apache-2.0',
       install_requires=[
                         'catboost',
```

