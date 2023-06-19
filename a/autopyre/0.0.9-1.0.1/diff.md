# Comparing `tmp/autopyre-0.0.9.tar.gz` & `tmp/autopyre-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-0.0.9.tar", last modified: Sun Jun 18 15:01:02 2023, max compression
+gzip compressed data, was "autopyre-1.0.1.tar", last modified: Mon Jun 19 11:48:05 2023, max compression
```

## Comparing `autopyre-0.0.9.tar` & `autopyre-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 15:01:02.722979 autopyre-0.0.9/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.9/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 15:01:02.720747 autopyre-0.0.9/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.9/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 15:01:02.718770 autopyre-0.0.9/autopyre.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/requires.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   191861 2023-06-18 15:00:44.000000 autopyre-0.0.9/autopyre.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 15:01:02.728448 autopyre-0.0.9/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-18 14:00:07.000000 autopyre-0.0.9/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 11:48:05.334239 autopyre-1.0.1/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-1.0.1/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-19 11:48:05.333580 autopyre-1.0.1/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-1.0.1/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-19 11:48:05.332241 autopyre-1.0.1/autopyre.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-19 11:48:05.000000 autopyre-1.0.1/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-19 11:48:05.000000 autopyre-1.0.1/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 11:48:05.000000 autopyre-1.0.1/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-19 11:48:05.000000 autopyre-1.0.1/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-19 11:48:05.000000 autopyre-1.0.1/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-19 11:48:05.000000 autopyre-1.0.1/autopyre.egg-info/requires.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-19 11:48:05.000000 autopyre-1.0.1/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   192441 2023-06-19 11:47:46.000000 autopyre-1.0.1/autopyre.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-19 11:48:05.337063 autopyre-1.0.1/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-19 11:47:50.000000 autopyre-1.0.1/setup.py
```

### Comparing `autopyre-0.0.9/LICENSE` & `autopyre-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.9/PKG-INFO` & `autopyre-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.9
+Version: 1.0.1
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.9/autopyre.egg-info/PKG-INFO` & `autopyre-1.0.1/autopyre.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.9
+Version: 1.0.1
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.9/autopyre.py` & `autopyre-1.0.1/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '0.0.9'
+__version__ = '1.0.1'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
 
 
@@ -1889,16 +1889,19 @@
     match = re.search(pattern, code)
     if match:
         return match.group(1)
     return None
 
 
 # 추가한 부분 - 김위성 - 프로젝트의 경로
-def get_project_path():
-    return os.path.dirname(os.path.abspath(__file__))
+def get_project_path(filename):
+    
+    absolute_path = os.path.abspath(filename)
+    project_path = os.path.dirname(absolute_path)
+    return project_path
 
 
 
 # 추가한 부분 - 김위성 - import 하고 있는 파일과 해당 파일의 모든 식별자와 참조되는 식별자
 def find_all_identifiers(project_path, target_file):
     identifiers = set()
     referenced = set()
@@ -1926,28 +1929,28 @@
     for root, dirs, files in os.walk(project_path):
         for file_name in files:
             
             file_path = os.path.join(root, file_name)
             if file_name.endswith('.py') and file_path != target_file_path:
                 
                 # iuput 파일이 import되고 있는 경우
-                if is_file_imported(file_path, target_file_name): 
+                if is_file_imported(file_path, target_file_name, project_path): 
                     importing_files.add(file_path)
     
     # iuput 파일이 import하는 파일(라이브러리)의 경우
     import_path = get_import_paths(project_path, target_file)
     importing_files.update(import_path)
     return importing_files
 
 
 # 추가한 부분 - 김위성 - 프로젝트내의 어떤 파일이 input파일을 import하는지 여부
 # 보안 적용 - 
 # 적절한 자원 반환 - with문 내의 코드에 예외가 발생하더라도 항상 파일 닫기가 보장 
 # 예외 처리 - try-except : 사용자가 syntax 에러가 있는 소스 코드에 대해 작명 컨벤션을 적용할 경우
-def is_file_imported(file_path, target_file):
+def is_file_imported(file_path, target_file, project_path):
     with open(file_path, 'r', errors='ignore') as file:
         source_code = file.read()
     tree = None
     
     try:
         tree = ast.parse(source_code)
     except SyntaxError:
@@ -1957,19 +1960,41 @@
         if isinstance(node, ast.Import):
             
             for alias in node.names:
                 imported_module = alias.name
                 if target_file == imported_module or '.' + target_file in imported_module:
                     return True
         elif isinstance(node, ast.ImportFrom):
-            try:
-                if node.module == target_file or '.' + target_file in node.module:
-                    return True
-            except TypeError:
-                pass
+            if node.module == target_file or '.' + target_file in node.module:
+                return True
+
+    
+    
+    
+    # import_paths = []
+    # library_paths = []
+    
+    # try:
+    #     tree = ast.parse(source_code)
+    # except SyntaxError:
+    #     return False
+    
+    # for node in ast.walk(tree):
+    #     if isinstance(node, ast.Import):
+    #         for alias in node.names:
+    #             import_paths.append(alias.name)
+
+    #     elif isinstance(node, ast.ImportFrom):
+    #         module_name = node.module if node.module else ''
+    #         import_paths.append(module_name)
+    
+    
+            
+    # if target_file in import_paths: 
+    #     return True
     
     return False
 
 
 # 추가한 부분 - 김위성 - 식별자, 참조되는 식별자를 모두 저장
 def analyze_file(file_path):
     with open(file_path, 'r', errors='ignore') as file:
@@ -2041,27 +2066,26 @@
         if isinstance(node, ast.Import):
             for alias in node.names:
                 import_paths.append(alias.name)
 
         elif isinstance(node, ast.ImportFrom):
             module_name = node.module if node.module else ''
             import_paths.append(module_name)
-
                 
     for import_path in import_paths:
         if "." in import_path:
             import_path = import_path.split('.')[-1]
 
         library_path = get_library_path(project_path, import_path)
         
         if library_path is None: continue
         if library_path.startswith(project_path):
 
             library_paths.append(library_path)
-    # print("library_paths", library_paths)
+
     return library_paths
 
 
 # 추가한 부분 - 김위성 - input 파일의 경로를 가져온다.
 def get_file_path(project_path, file_name):
     for root, _, files in os.walk(project_path):
         for file in files:
@@ -4422,15 +4446,15 @@
             sys.exit()
         elif command.upper() != 'Y':
             print('잘못 입력하였습니다.')
             sys.exit()
             
         global all_origin_identifiers 
         global all_origin_referenced
-        project_path = get_project_path()
+        project_path = get_project_path(filename)
         all_origin_identifiers, all_origin_referenced = find_all_identifiers(project_path, filename)
         
         
     original_source = readlines_from_file(filename)
 
     fixed_source = original_source
```

### Comparing `autopyre-0.0.9/setup.py` & `autopyre-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import io
 
 from setuptools import setup
 
 # read the contents of your README file
 
 INSTALL_REQUIRES = (
-    ['pyrestyle >= 0.0.4', 'tomli; python_version < "3.11"']
+    ['pyrestyle >= 0.0.7', 'tomli; python_version < "3.11"']
 )
 
 
 def version():
     """Return version string."""
     with io.open('autopyre.py') as input_file:
         for line in input_file:
```

