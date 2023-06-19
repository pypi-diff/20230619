# Comparing `tmp/bring-order-0.1.3.tar.gz` & `tmp/bring-order-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring-order-0.1.3.tar", last modified: Sat Jun 17 17:36:05 2023, max compression
+gzip compressed data, was "bring-order-0.2.0.tar", last modified: Mon Jun 19 15:41:20 2023, max compression
```

## Comparing `bring-order-0.1.3.tar` & `bring-order-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-17 17:36:05.288634 bring-order-0.1.3/
--rw-r--r--   0 evgeniia  (1000) users      (100)     1067 2023-06-06 06:49:56.000000 bring-order-0.1.3/LICENSE
--rw-r--r--   0 evgeniia  (1000) users      (100)     3503 2023-06-17 17:36:05.288634 bring-order-0.1.3/PKG-INFO
--rw-r--r--   0 evgeniia  (1000) users      (100)     2888 2023-06-14 17:19:21.000000 bring-order-0.1.3/README.md
-drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-17 17:36:05.288634 bring-order-0.1.3/bring_order/
--rw-r--r--   0 evgeniia  (1000) users      (100)       46 2023-06-04 16:23:23.000000 bring-order-0.1.3/bring_order/__init__.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     5304 2023-06-17 06:20:51.000000 bring-order-0.1.3/bring_order/bodi.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     3399 2023-06-16 17:57:11.000000 bring-order-0.1.3/bring_order/bogui.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     9124 2023-06-17 06:21:30.000000 bring-order-0.1.3/bring_order/boutils.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     2580 2023-06-17 12:53:35.000000 bring-order-0.1.3/bring_order/bringorder.py
--rw-r--r--   0 evgeniia  (1000) users      (100)    10770 2023-06-17 06:25:41.000000 bring-order-0.1.3/bring_order/deductive.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     5316 2023-06-17 16:18:17.000000 bring-order-0.1.3/bring_order/inductive.py
--rw-r--r--   0 evgeniia  (1000) users      (100)      280 2023-06-14 17:19:21.000000 bring-order-0.1.3/bring_order/inductive_summary_storage.py
-drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-17 17:36:05.288634 bring-order-0.1.3/bring_order.egg-info/
--rw-r--r--   0 evgeniia  (1000) users      (100)     3503 2023-06-17 17:36:05.000000 bring-order-0.1.3/bring_order.egg-info/PKG-INFO
--rw-r--r--   0 evgeniia  (1000) users      (100)      420 2023-06-17 17:36:05.000000 bring-order-0.1.3/bring_order.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniia  (1000) users      (100)        1 2023-06-17 17:36:05.000000 bring-order-0.1.3/bring_order.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniia  (1000) users      (100)       11 2023-06-17 17:36:05.000000 bring-order-0.1.3/bring_order.egg-info/requires.txt
--rw-r--r--   0 evgeniia  (1000) users      (100)       12 2023-06-17 17:36:05.000000 bring-order-0.1.3/bring_order.egg-info/top_level.txt
--rw-r--r--   0 evgeniia  (1000) users      (100)      529 2023-06-17 17:35:55.000000 bring-order-0.1.3/pyproject.toml
--rw-r--r--   0 evgeniia  (1000) users      (100)       38 2023-06-17 17:36:05.288634 bring-order-0.1.3/setup.cfg
--rw-r--r--   0 evgeniia  (1000) users      (100)     1093 2023-06-17 17:35:36.000000 bring-order-0.1.3/setup.py
+drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-19 15:41:20.461287 bring-order-0.2.0/
+-rw-r--r--   0 evgeniia  (1000) users      (100)     1067 2023-06-06 06:49:56.000000 bring-order-0.2.0/LICENSE
+-rw-r--r--   0 evgeniia  (1000) users      (100)     4407 2023-06-19 15:41:20.461287 bring-order-0.2.0/PKG-INFO
+-rw-r--r--   0 evgeniia  (1000) users      (100)     3792 2023-06-19 15:15:00.000000 bring-order-0.2.0/README.md
+drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-19 15:41:20.457287 bring-order-0.2.0/bring_order/
+-rw-r--r--   0 evgeniia  (1000) users      (100)       46 2023-06-04 16:23:23.000000 bring-order-0.2.0/bring_order/__init__.py
+-rw-r--r--   0 evgeniia  (1000) users      (100)     6798 2023-06-19 14:35:03.000000 bring-order-0.2.0/bring_order/bodi.py
+-rw-r--r--   0 evgeniia  (1000) users      (100)     3262 2023-06-19 14:35:03.000000 bring-order-0.2.0/bring_order/bogui.py
+-rw-r--r--   0 evgeniia  (1000) users      (100)     9124 2023-06-17 06:21:30.000000 bring-order-0.2.0/bring_order/boutils.py
+-rw-r--r--   0 evgeniia  (1000) users      (100)     2542 2023-06-18 16:42:54.000000 bring-order-0.2.0/bring_order/bringorder.py
+-rw-r--r--   0 evgeniia  (1000) users      (100)     9019 2023-06-19 14:35:03.000000 bring-order-0.2.0/bring_order/deductive.py
+-rw-r--r--   0 evgeniia  (1000) users      (100)     7349 2023-06-19 14:35:03.000000 bring-order-0.2.0/bring_order/inductive.py
+drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-19 15:41:20.457287 bring-order-0.2.0/bring_order.egg-info/
+-rw-r--r--   0 evgeniia  (1000) users      (100)     4407 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniia  (1000) users      (100)      379 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniia  (1000) users      (100)        1 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniia  (1000) users      (100)       11 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/requires.txt
+-rw-r--r--   0 evgeniia  (1000) users      (100)       12 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/top_level.txt
+-rw-r--r--   0 evgeniia  (1000) users      (100)      529 2023-06-19 15:22:50.000000 bring-order-0.2.0/pyproject.toml
+-rw-r--r--   0 evgeniia  (1000) users      (100)       38 2023-06-19 15:41:20.461287 bring-order-0.2.0/setup.cfg
+-rw-r--r--   0 evgeniia  (1000) users      (100)     1093 2023-06-19 15:22:17.000000 bring-order-0.2.0/setup.py
```

### Comparing `bring-order-0.1.3/LICENSE` & `bring-order-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bring-order-0.1.3/PKG-INFO` & `bring-order-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,30 @@
-Metadata-Version: 2.1
-Name: bring-order
-Version: 0.1.3
-Summary: The tool library is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.
-Home-page: https://github.com/Order-Team/bring-order/tree/main
-Author: Bring-Order team
-Author-email: example@email.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bring-order
 ![GitHub Actions](https://github.com/Order-Team/bring-order/workflows/CI/badge.svg)
 [![codecov](https://codecov.io/gh/Order-team/bring-order/branch/main/graph/badge.svg?token=e8bdd46f-46b0-410c-820b-84ffca9ca53c)](https://codecov.io/gh/Order-team/bring-order)
 [![GitHub](https://img.shields.io/github/license/Order-Team/bring-order)](LICENSE.md)
 
 The tool is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.
-User can choose deductive or inductive analysis.
+User can import and prepare data for analysis, add limitations and perform deductive or inductive analysis.
 Deductive analysis asks the user to set the hypothesis and null hypothesis, run their analysis, and confirm one of the hypotheses.
 Inductive analysis is an option to perform explorative analysis and write notes about it.
 
 
 ## Documentation
 * [Product backlog](https://docs.google.com/spreadsheets/d/1xqybqVAUIn4vhW-fBfhInQun7nY-uYH79M6l8oCiAzg/edit#gid=0)
 
 * [Definition of Done](https://github.com/Order-Team/bring-order/blob/main/documentation/DoD.md)
 
 * [Minutes of meetings](https://drive.google.com/drive/folders/1kwXCKbx7egHf8qYDIb4fRffNnad6Qd1t)
 
 ## Installation
+### Installation from PyPi
+
+### Linux
 
-### Installation from TestPypi
 - If you don't have Jupyter Notebook installed, install it with
 ```bash
     pip install notebook
 ```
 
 - If you don't have ipywidgets installed, install it with
 
@@ -48,29 +34,65 @@
 
 - If you have an old version of ipywidgets installed, upgrade it with
 
 ```bash
     pip install --upgrade ipywidgets
 ```
 
-- Install testbringorder extention:
+- Install bring-order extention:
+```bash
+    pip install bring-order
+```
+
+### Windows
+
+- If you don't have Jupyter Notebook installed, install Anaconda with [Anaconda download](https://www.anaconda.com/download)
+
+- Use Anaconda Powershell Prompt 
+
+- If you don't have ipywidgets installed, install it with
 ```bash
-    pip install -i https://test.pypi.org/simple/ testbringorder
+    pip install ipywidgets
+```
+- If you have an old version of ipywidgets installed, upgrade it with
+```bash
+    pip install --upgrade ipywidgets
 ```
 
+- Install bring-order extention:
+```bash
+    pip install bring-order
+```
+
+### MacOS
+- If you don't have ipywidgets installed, install it with
+```bash
+    python3 -m pip install "ipywidgets"
+```
+- If you have an old version of ipywidgets installed, upgrade it with
+```bash
+    python3 -m pip install --upgrade ipywidgets
+```
+- Install bring-order extention:
+```bash
+    python3 -m pip install "bring-order"
+```
 ### Usage
 - Open Jupyter Notebook with
 ```bash
     jupyter notebook
 ```
 
 - In Jupyter Notebook execute
 
 ``` 
-    from bringorder import BringOrder
+    from bring_order import BringOrder  or  from bring_order import *
+```
+- Start using package by executing
+``` 
     BringOrder()
 ```
 
 - Make sure that your notebook is in Trusted state. Otherwise the widgets might not work correctly.
 
 ## Development
```

### Comparing `bring-order-0.1.3/README.md` & `bring-order-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,46 @@
+Metadata-Version: 2.1
+Name: bring-order
+Version: 0.2.0
+Summary: The tool library is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.
+Home-page: https://github.com/Order-Team/bring-order/tree/main
+Author: Bring-Order team
+Author-email: example@email.com
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bring-order
 ![GitHub Actions](https://github.com/Order-Team/bring-order/workflows/CI/badge.svg)
 [![codecov](https://codecov.io/gh/Order-team/bring-order/branch/main/graph/badge.svg?token=e8bdd46f-46b0-410c-820b-84ffca9ca53c)](https://codecov.io/gh/Order-team/bring-order)
 [![GitHub](https://img.shields.io/github/license/Order-Team/bring-order)](LICENSE.md)
 
 The tool is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.
-User can choose deductive or inductive analysis.
+User can import and prepare data for analysis, add limitations and perform deductive or inductive analysis.
 Deductive analysis asks the user to set the hypothesis and null hypothesis, run their analysis, and confirm one of the hypotheses.
 Inductive analysis is an option to perform explorative analysis and write notes about it.
 
 
 ## Documentation
 * [Product backlog](https://docs.google.com/spreadsheets/d/1xqybqVAUIn4vhW-fBfhInQun7nY-uYH79M6l8oCiAzg/edit#gid=0)
 
 * [Definition of Done](https://github.com/Order-Team/bring-order/blob/main/documentation/DoD.md)
 
 * [Minutes of meetings](https://drive.google.com/drive/folders/1kwXCKbx7egHf8qYDIb4fRffNnad6Qd1t)
 
 ## Installation
+### Installation from PyPi
+
+### Linux
 
-### Installation from TestPypi
 - If you don't have Jupyter Notebook installed, install it with
 ```bash
     pip install notebook
 ```
 
 - If you don't have ipywidgets installed, install it with
 
@@ -32,29 +50,65 @@
 
 - If you have an old version of ipywidgets installed, upgrade it with
 
 ```bash
     pip install --upgrade ipywidgets
 ```
 
-- Install testbringorder extention:
+- Install bring-order extention:
+```bash
+    pip install bring-order
+```
+
+### Windows
+
+- If you don't have Jupyter Notebook installed, install Anaconda with [Anaconda download](https://www.anaconda.com/download)
+
+- Use Anaconda Powershell Prompt 
+
+- If you don't have ipywidgets installed, install it with
 ```bash
-    pip install -i https://test.pypi.org/simple/ testbringorder
+    pip install ipywidgets
+```
+- If you have an old version of ipywidgets installed, upgrade it with
+```bash
+    pip install --upgrade ipywidgets
 ```
 
+- Install bring-order extention:
+```bash
+    pip install bring-order
+```
+
+### MacOS
+- If you don't have ipywidgets installed, install it with
+```bash
+    python3 -m pip install "ipywidgets"
+```
+- If you have an old version of ipywidgets installed, upgrade it with
+```bash
+    python3 -m pip install --upgrade ipywidgets
+```
+- Install bring-order extention:
+```bash
+    python3 -m pip install "bring-order"
+```
 ### Usage
 - Open Jupyter Notebook with
 ```bash
     jupyter notebook
 ```
 
 - In Jupyter Notebook execute
 
 ``` 
-    from bringorder import BringOrder
+    from bring_order import BringOrder  or  from bring_order import *
+```
+- Start using package by executing
+``` 
     BringOrder()
 ```
 
 - Make sure that your notebook is in Trusted state. Otherwise the widgets might not work correctly.
 
 ## Development
```

### Comparing `bring-order-0.1.3/bring_order/bogui.py` & `bring-order-0.2.0/bring_order/bogui.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,36 +28,34 @@
         for button in buttons:
             new_button = self.create_button(desc=button[0],
                                                   command=button[1],
                                                   style=button[2])
             button_list[button[0]] = new_button
         return button_list
 
-    def create_message(self, value, style={'font-family': 'Arial, Helvetica, sans-serif',
-                                           'font_size': '15px'}):
+    def create_message(self, value, style={'font_size': '15px'}):
         """Creates HTML"""
         message = widgets.HTML(value=value, style=style)
         return message
 
     def create_error_message(self, value=''):
         """Creates HTML, color: red"""
         error = self.create_message(value=value,
-                                    style={'font-family': 'Arial, Helvetica, sans-serif',
-                                           'font_size': '12px',
+                                    style={'font_size': '12px',
                                            'text_color': 'red'})
         return error
 
     def create_input_field(self, default_value=''):
         """Creates input field"""
         input_field = widgets.Text(value=default_value)
         return input_field
 
-    def create_text_area(self, default_value=''):
+    def create_text_area(self, default_value='', place_holder=''):
         """Creates text box"""
-        text_area = widgets.Textarea(value=default_value,layout={'width': '80%'})
+        text_area = widgets.Textarea(value=default_value,layout={'width': '70%'}, placeholder=place_holder)
         return text_area
 
     def create_label(self, value):
         """Creates label"""
         label = widgets.Label(value=value,
                               layout=widgets.Layout(justify_content='flex-end'))
         return label
```

### Comparing `bring-order-0.1.3/bring_order/boutils.py` & `bring-order-0.2.0/bring_order/boutils.py`

 * *Files identical despite different names*

### Comparing `bring-order-0.1.3/bring_order/bringorder.py` & `bring-order-0.2.0/bring_order/bringorder.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,27 @@
 from boutils import BOUtils
 from deductive import Deductive
 from inductive import Inductive
 
 
 class BringOrder:
     """Main class"""
-    def __init__(self, data_import=True):
+    def __init__(self):
         """Class constructor"""
         self.boutils = BOUtils()
         self.bogui = BOGui()
         self.deductive = None
         self.inductive = None
         self.deductive_button = None
         self.inductive_button = None
         self.bodi = Bodi(
             self.boutils,
             self.bogui,
             self.start_analysis)
-        if data_import:
-            self.bring_order()
-        else:
-            self.start_analysis()
+        self.bring_order()
 
     def create_deductive_button(self):
         """Creates deductive button"""
         button = self.bogui.create_button(
             desc='Deductive',
             command=self.start_deductive_analysis)
 
@@ -55,36 +52,38 @@
         self.inductive_button.close()
 
     def start_deductive_analysis(self, _=None):
         """Starts deductive analysis"""
 
         self.close_buttons()
         if not hasattr(self, 'data_limitations'):
-            self.data_limitations = self.bodi.data_limitations.value
-        self.deductive.data_limitations = self.bodi.data_limitations.value
+            self.data_limitations = self.bodi.data_limitations
+        self.deductive.data_limitations = self.bodi.data_limitations
         self.deductive.start_deductive_analysis()
 
     def start_inductive_analysis(self, _=None):
         """Starts inductive analysis"""
         self.close_buttons()
         self.inductive.start_inductive_analysis()
 
     def bring_order(self):
         """Starts data import phase"""
         self.bodi.bodi()
 
     def start_analysis(self):
+        """Starts analysis phase"""
         self.deductive = Deductive(
             self.bogui,
             self.boutils,
             self.start_analysis
         )
         self.inductive = Inductive(
             self.bogui,
-            self.boutils
+            self.boutils,
+            self.start_analysis
         )
         self.deductive_button = self.create_deductive_button()
         self.inductive_button = self.create_inductive_button()
         display(widgets.HBox([self.deductive_button, self.inductive_button]))
 
     def __repr__(self):
-        return ''
+        return ''
```

### Comparing `bring-order-0.1.3/bring_order/deductive.py` & `bring-order-0.2.0/bring_order/deductive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,98 +1,90 @@
 """Deductive class"""
 from ipywidgets import widgets
 from IPython.display import display
 
-
 class Deductive:
     """Class that guides deductive analysis"""
     def __init__(self, bogui, boutils, start_new):
         """Class constructor
         
         Args:
             bogui (BOGui)
             boutils (BOUtils)
             start_new (function): Function to start new analysis with same data
         """
         self.cell_count = 0
         self.start_new = start_new
         self.bogui = bogui
         self.boutils = boutils
-        self.hypothesis_input = self.bogui.create_input_field()
+        self.buttons = self.bogui.init_buttons(self.button_list)
+        #List of hypotheses: 0 = hypothesis, 1 = null hypothesis
+        self.hypotheses = [self.bogui.create_input_field(), self.bogui.create_input_field()]
         self.empty_hypo_error = self.bogui.create_error_message()
-        self.null_input = self.bogui.create_input_field()
         self.empty_null_error = self.bogui.create_error_message()
         self.hypotheses_grid = self.create_hypotheses_grid()
         self.add_cells_int = self.bogui.create_int_text()
         self.confirmed_grid = None
         self.conclusion = None
-        self.data_limitations = 'Data limitations missing'
+        self.data_limitations = ['Data limitations missing']
         self.limitation_prompt = None
 
+    @property
+    def button_list(self):
+        """Buttons for deductive class.
+
+        Returns:
+            list of tuples in format (description: str, command: func, style: str)"""
+        button_list = [('Open cells', self.open_cells, 'warning'),
+                       ('Delete last cell', self.delete_last_cell, 'danger'),
+                       ('Save', self.check_data_limitations, 'success'),
+                       ('Clear', self.clear_hypotheses, 'primary'),
+                       ('Yes', self.valid_hypotheses, 'success'),
+                       ('No', self.bad_hypotheses, 'warning'),
+                       ('Run cells', self.run_cells, 'primary'),
+                       ('Clear cells', self.clear_cells, 'danger'),
+                       ('New analysis', self.start_new_analysis, 'success'),
+                       ('Prepare new data', self.start_analysis_with_new_data, 'success'),
+                       ('All done', self.all_done, 'success')]
+        return button_list
+
     def create_hypotheses_grid(self):
         """Creates widgets"""
         hypothesis_label = self.bogui.create_label('Hypothesis:')
         null_label = self.bogui.create_label('Null hypothesis:')
-        save_button = self.bogui.create_button(
-            desc='Save',
-            command=self.check_data_limitations)
-        clear_button = self.bogui.create_button(
-            desc='Clear',
-            command=self.clear_hypotheses,
-            style='primary')
         empty = self.bogui.create_placeholder()
 
-        grid = self.bogui.create_grid(
-            5,
-            2,
-            [empty,
-             self.empty_hypo_error,
-             hypothesis_label,
-             self.hypothesis_input,
-             null_label,
-             self.null_input,
-             empty,
-             self.empty_null_error,
-             empty,
-             widgets.HBox(
-                [save_button, clear_button])
+        grid = self.bogui.create_grid(5, 2,
+            [empty, self.empty_hypo_error,
+             hypothesis_label, self.hypotheses[0],
+             null_label, self.hypotheses[1],
+             empty, self.empty_null_error,
+             empty, widgets.HBox([self.buttons['Save'], self.buttons['Clear']])
             ])
-
         return grid
 
     def start_deductive_analysis(self, _=None):
         """Button function for deductive analysis"""
         display(self.hypotheses_grid)
-        self.hypothesis_input.focus()
+        self.hypotheses[0].focus()
 
     def check_data_limitations(self, _=None):
         """Displays the prompt for the check against data limitations"""
         #print('checking limits: ' + self.data_limitations) #This is for debugging
-        self.limitation_prompt_text = widgets.HTML(
-            'Do the hypotheses fit within the limitations of the data set?' 
-            + '<br>'
-            + self.data_limitations)
-        valid_hypotheses_button = self.bogui.create_button(
-            desc='Yes',
-            command=self.valid_hypotheses
-        )
-        bad_hypotheses_button = self.bogui.create_button(
-            desc='No',
-            command=self.bad_hypotheses,
-            style='warning'
-        )
-        self.limitation_prompt = widgets.VBox(
-            [
-            self.limitation_prompt_text,
-            widgets.HBox([
-                valid_hypotheses_button, bad_hypotheses_button
+        if self.check_hypotheses():
+            limitations = ''.join(f"Limitation {count}: {item.value} <br>" for count, item in enumerate(self.data_limitations, start=1))
+
+            limitation_prompt_text = widgets.HTML(
+                'Do the hypotheses fit within the limitations of the data set?' 
+                + '<br>' + limitations)
+
+            self.limitation_prompt = widgets.VBox([limitation_prompt_text,
+                widgets.HBox([self.buttons['Yes'], self.buttons['No']])
                 ])
-            ]
-        )
-        display(self.limitation_prompt)
+            display(self.limitation_prompt)
 
     def valid_hypotheses(self, _=None):
         """Closes the data limitation check prompt and calls save_hypotheses()"""
         self.limitation_prompt.close()
         self.save_hypotheses()
 
     def bad_hypotheses(self, _=None):
@@ -104,218 +96,128 @@
 
     def check_hypotheses(self):
         """Checks that hypothesis and null hypothesis are not empty.
 
         Returns:
             True/False
         """
-        if len(self.hypothesis_input.value) > 0 and len(self.null_input.value) > 0:
+        if len(self.hypotheses[0].value) > 0 and len(self.hypotheses[1].value) > 0:
             return True
 
-        if self.hypothesis_input.value == '':
+        if self.hypotheses[0].value == '':
             self.empty_hypo_error.value = 'Hypothesis missing'
         else:
             self.empty_hypo_error.value = ''
 
-        if self.null_input.value == '':
+        if self.hypotheses[1].value == '':
             self.empty_null_error.value = 'Null hypothesis missing'
         else:
             self.empty_null_error.value = ''
 
         return False
 
     def save_hypotheses(self, _=None):
         """Saves hypotheses and displays buttons for running code"""
-        hypotheses = f'- Hypothesis: {self.hypothesis_input.value}\\n- Null hypothesis: {self.null_input.value}'
+        hypotheses = f'- Hypothesis: {self.hypotheses[0].value}\
+        \\n- Null hypothesis: {self.hypotheses[1].value}'
         text = f'# Deductive analysis\\n## Hypotheses\\n{hypotheses}\\n## Data analysis'
         if self.check_hypotheses():
             self.boutils.create_markdown_cells_above(1, text=text)
-            confirmed_hypothesis = self.bogui.create_message(
-                value=f'Hypothesis: {self.hypothesis_input.value}')
-            confirmed_null = self.bogui.create_message(
-                value=f'Null hypothesis: {self.null_input.value}')
-            self.confirmed_grid = self.create_confirmed_grid(
-                confirmed_hypothesis,
-                confirmed_null)
+            self.confirmed_grid = self.create_confirmed_grid()
             self.hypotheses_grid.close()
             display(self.confirmed_grid)
 
     def clear_hypotheses(self, _=None):
         """Button function for resetting hypothesis and null hypothesis inputs"""
-        self.hypothesis_input.value = ''
-        self.null_input.value = ''
+        self.hypotheses[0].value = ''
+        self.hypotheses[1].value = ''
         self.empty_hypo_error.value = ''
         self.empty_null_error.value = ''
-        self.hypothesis_input.focus()
-
-    def create_open_cells_button(self):
-        """Creates button for opening new code cells for analysis.
+        self.hypotheses[0].focus()
 
-        Returns:
-            button
-        """
-        def open_cells(_=None):
-            """Button function"""
+    def open_cells(self, _=None):
+        """Button function for opening new code cells"""
+        if self.add_cells_int.value > 0:
             self.cell_count += self.add_cells_int.value
             self.boutils.create_code_cells_above(self.add_cells_int.value)
 
-        button = self.bogui.create_button(
-            desc='Open cells',
-            command=open_cells,
-            style='warning')
-
-        return button
+    def delete_last_cell(self, _=None):
+        """Button function for deleting the last code cell"""
+        if self.cell_count > 0:
+            self.boutils.delete_cell_above()
+            self.cell_count -= 1
+
+    def deactivate_cell_operations(self):
+        """Deactivates buttons after runnig code block"""
+        self.buttons['Open cells'].disabled = True
+        self.buttons['Clear cells'].disabled = True
+        self.buttons['Delete last cell'].disabled = True
+
+    def run_cells(self, _=None):
+        """Button function"""
+        self.boutils.run_cells_above(
+            self.cell_count)
+        self.deactivate_cell_operations()
+
+        if self.conclusion:
+            self.conclusion.close()
+
+        question = self.bogui.create_message(value='What happened?')
+        conclusion_label = self.bogui.create_message(value='Accepted hypothesis:')
+        conclusion = self.bogui.create_radiobuttons(
+            options=[f'Hypothesis: {self.hypotheses[0].value}',
+                     f'Null hypothesis: {self.hypotheses[1].value}'])
+
+        self.conclusion = widgets.AppLayout(
+            header=question,
+            left_sidebar=conclusion_label,
+            center=conclusion,
+            footer=widgets.HBox([
+                self.buttons['New analysis'],
+                self.buttons['Prepare new data'],
+                self.buttons['All done']])
+        )
+        display(self.conclusion)
 
-    def create_delete_button(self):
-        """Creates button for deleting the last code cell
+    def clear_cells(self, _=None):
+        """Clear button function to clear cells above"""
+        self.boutils.clear_code_cells_above(self.cell_count)
 
-        Returns:
-            button
-        """
-        def delete_last_cell(_=None):
-            """Button function"""
-            if self.cell_count > 0:
-                self.boutils.delete_cell_above()
-                self.cell_count -= 1
-
-        button = self.bogui.create_button(
-            desc='Delete last cell',
-            command=delete_last_cell,
-            style='danger')
-
-        return button
-
-    def create_run_button(self, hypothesis, null_hypothesis):
-        """Creates button"""
-        def run_cells(_=None):
-            """Button function"""
-            self.boutils.run_cells_above(
-                self.cell_count)
-
-            if self.conclusion:
-                self.conclusion.close()
-
-            conclusion_label = self.bogui.create_message(
-                value='Accepted hypothesis:')
-            conclusion = self.bogui.create_radiobuttons(
-                options=[hypothesis.value, null_hypothesis.value])
-            new_analysis_button = self.create_new_analysis_button(
-                conclusion)
-            new_data_button = self.create_new_data_button(conclusion)
-            all_done_button = self.create_all_done_button(conclusion)
-            self.conclusion = widgets.AppLayout(
-                left_sidebar=conclusion_label,
-                center=conclusion,
-                footer=widgets.HBox([new_analysis_button, new_data_button, all_done_button])
-            )
-
-            display(self.conclusion)
-
-        button = self.bogui.create_button(
-            desc='Run cells',
-            command=run_cells,
-            style='primary')
-
-        return button
-
-    def create_clear_button(self):
-        """Creates button"""
-        def clear_cells(_=None):
-            """Button function"""
-            self.boutils.clear_code_cells_above(
-                self.cell_count)
-
-        button = self.bogui.create_button(
-            desc='Clear cells',
-            command=clear_cells,
-            style='danger')
-        return button
-
-    def create_confirmed_grid(self, hypothesis, null_hypothesis):
+    def create_confirmed_grid(self):
         """Creates widget grid"""
-        cell_number_label = self.bogui.create_label(
-            'Add code cells for your analysis:')
+        cell_number_label = self.bogui.create_label('Add code cells for your analysis:')
 
-        open_cells_button = self.create_open_cells_button()
-        delete_cell_button = self.create_delete_button()
-        run_cells_button = self.create_run_button(hypothesis, null_hypothesis)
-        clear_cells_button = self.create_clear_button()
-
-        grid = widgets.GridspecLayout(
-            2,
-            2,
-            justify_items='center',
-            width='70%',
-            align_items='top')
-        grid[1, 0] = widgets.HBox(
-            [cell_number_label, self.add_cells_int])
+        grid = widgets.GridspecLayout(2, 2, justify_items='center', width='70%', align_items='top')
+        grid[1, 0] = widgets.HBox([cell_number_label, self.add_cells_int])
         grid[1, 1] = widgets.TwoByTwoLayout(
-            top_left=open_cells_button,
-            bottom_left=run_cells_button,
-            top_right=delete_cell_button,
-            bottom_right=clear_cells_button)
+            top_left=self.buttons['Open cells'],
+            bottom_left=self.buttons['Run cells'],
+            top_right=self.buttons['Delete last cell'],
+            bottom_right=self.buttons['Clear cells'])
 
         return grid
 
-    def save_results(self, confirmed):
+    def save_results(self):
         """Prints results and hides widgets"""
-        text = f'## Conclusion\\nAccepted: {confirmed.value}'
+        text = f'## Accepted hypothesis\\n{self.conclusion.center.value}'
         self.boutils.create_markdown_cells_above(1, text=text)
         self.confirmed_grid.close()
         self.conclusion.close()
 
-    def create_new_analysis_button(self, radio):
-        """Creates button
-        
-        Args:
-            radio (radiobutton): the hypothesis radiobutton widget
-        """
-        def start_new_analysis(_=None):
-            """Button function"""
-            self.save_results(radio)
-            self.start_new()
-
-        button = self.bogui.create_button(
-            desc='New analysis',
-            command=start_new_analysis)
-
-        return button
-
-    def create_new_data_button(self, radio):
-        """Creates button
-        
-        Args:
-            radio (radiobutton): the hypothesis radiobutton widget
-        """
+    def start_new_analysis(self, _=None):
+        """Button function to save results and star new analysis"""
+        self.save_results()
+        self.start_new()
+
+    def start_analysis_with_new_data(self, _=None):
+        """Button function to start over with new data"""
+        self.save_results()
+        self.boutils.execute_cell_from_current(1, 'BringOrder()')
 
-        def start_analysis_with_new_data(_=None):
-            """Button function"""
-            self.save_results(radio)
-            self.boutils.execute_cell_from_current(1, 'BringOrder()')
-
-        button = self.bogui.create_button(
-            desc='Prepare new data',
-            command=start_analysis_with_new_data
-        )
-
-        return button
-
-    def create_all_done_button(self, radio):
-        """Creates button
-        
-        Args:
-            radio (radiobutton): the hypothesis radiobutton widget
-        """
-
-        def all_done(_=None):
-            self.save_results(radio)
-            self.boutils.delete_cell_from_current(1)
-
-        button = self.bogui.create_button(
-            desc='All done',
-            command=all_done
-        )
 
-        return button
+    def all_done(self, _=None):
+        """Button function to save results when ready."""
+        self.save_results()
+        self.boutils.delete_cell_from_current(1)
 
     def __repr__(self):
         return ''
```

### Comparing `bring-order-0.1.3/bring_order.egg-info/PKG-INFO` & `bring-order-0.2.0/bring_order.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-order
-Version: 0.1.3
+Version: 0.2.0
 Summary: The tool library is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.
 Home-page: https://github.com/Order-Team/bring-order/tree/main
 Author: Bring-Order team
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,29 +16,31 @@
 
 # bring-order
 ![GitHub Actions](https://github.com/Order-Team/bring-order/workflows/CI/badge.svg)
 [![codecov](https://codecov.io/gh/Order-team/bring-order/branch/main/graph/badge.svg?token=e8bdd46f-46b0-410c-820b-84ffca9ca53c)](https://codecov.io/gh/Order-team/bring-order)
 [![GitHub](https://img.shields.io/github/license/Order-Team/bring-order)](LICENSE.md)
 
 The tool is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.
-User can choose deductive or inductive analysis.
+User can import and prepare data for analysis, add limitations and perform deductive or inductive analysis.
 Deductive analysis asks the user to set the hypothesis and null hypothesis, run their analysis, and confirm one of the hypotheses.
 Inductive analysis is an option to perform explorative analysis and write notes about it.
 
 
 ## Documentation
 * [Product backlog](https://docs.google.com/spreadsheets/d/1xqybqVAUIn4vhW-fBfhInQun7nY-uYH79M6l8oCiAzg/edit#gid=0)
 
 * [Definition of Done](https://github.com/Order-Team/bring-order/blob/main/documentation/DoD.md)
 
 * [Minutes of meetings](https://drive.google.com/drive/folders/1kwXCKbx7egHf8qYDIb4fRffNnad6Qd1t)
 
 ## Installation
+### Installation from PyPi
+
+### Linux
 
-### Installation from TestPypi
 - If you don't have Jupyter Notebook installed, install it with
 ```bash
     pip install notebook
 ```
 
 - If you don't have ipywidgets installed, install it with
 
@@ -48,29 +50,65 @@
 
 - If you have an old version of ipywidgets installed, upgrade it with
 
 ```bash
     pip install --upgrade ipywidgets
 ```
 
-- Install testbringorder extention:
+- Install bring-order extention:
+```bash
+    pip install bring-order
+```
+
+### Windows
+
+- If you don't have Jupyter Notebook installed, install Anaconda with [Anaconda download](https://www.anaconda.com/download)
+
+- Use Anaconda Powershell Prompt 
+
+- If you don't have ipywidgets installed, install it with
+```bash
+    pip install ipywidgets
+```
+- If you have an old version of ipywidgets installed, upgrade it with
+```bash
+    pip install --upgrade ipywidgets
+```
+
+- Install bring-order extention:
 ```bash
-    pip install -i https://test.pypi.org/simple/ testbringorder
+    pip install bring-order
 ```
 
+### MacOS
+- If you don't have ipywidgets installed, install it with
+```bash
+    python3 -m pip install "ipywidgets"
+```
+- If you have an old version of ipywidgets installed, upgrade it with
+```bash
+    python3 -m pip install --upgrade ipywidgets
+```
+- Install bring-order extention:
+```bash
+    python3 -m pip install "bring-order"
+```
 ### Usage
 - Open Jupyter Notebook with
 ```bash
     jupyter notebook
 ```
 
 - In Jupyter Notebook execute
 
 ``` 
-    from bringorder import BringOrder
+    from bring_order import BringOrder  or  from bring_order import *
+```
+- Start using package by executing
+``` 
     BringOrder()
 ```
 
 - Make sure that your notebook is in Trusted state. Otherwise the widgets might not work correctly.
 
 ## Development
```

### Comparing `bring-order-0.1.3/pyproject.toml` & `bring-order-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bring-order"
-version = "0.1.3"
+version = "0.2.0"
 description = ""
 authors = ["BringOrder team"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bring-order-0.1.3/setup.py` & `bring-order-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="bring-order",
-    version="0.1.3",
+    version="0.2.0",
     description="The tool library is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Order-Team/bring-order/tree/main",
     author="Bring-Order team",
     author_email="example@email.com",
     license="MIT",
```

