# Comparing `tmp/CToolKit-1.11.tar.gz` & `tmp/CToolKit-1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CToolKit-1.11.tar", last modified: Sun Jun 18 21:36:13 2023, max compression
+gzip compressed data, was "CToolKit-1.12.tar", last modified: Mon Jun 19 15:25:02 2023, max compression
```

## Comparing `CToolKit-1.11.tar` & `CToolKit-1.12.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:36:13.485931 CToolKit-1.11/
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:36:13.457931 CToolKit-1.11/CToolKit/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      504 2023-06-18 19:59:56.000000 CToolKit-1.11/CToolKit/ComandLineExecution.py
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:36:13.485931 CToolKit-1.11/CToolKit/Errors/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      306 2023-06-17 06:47:02.000000 CToolKit-1.11/CToolKit/Errors/ComandLineError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      226 2023-06-17 06:58:51.000000 CToolKit-1.11/CToolKit/Errors/ComandLineWarning.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      110 2023-06-17 06:48:41.000000 CToolKit-1.11/CToolKit/Errors/CopilationError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      118 2023-06-17 06:49:33.000000 CToolKit-1.11/CToolKit/Errors/CopilationWarning.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      108 2023-06-17 06:47:14.000000 CToolKit-1.11/CToolKit/Errors/ExecutionError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      116 2023-06-17 06:57:42.000000 CToolKit-1.11/CToolKit/Errors/ValgrindError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      115 2023-06-17 07:04:59.000000 CToolKit-1.11/CToolKit/Errors/ValgrindLeak.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        0 2023-06-17 04:59:48.000000 CToolKit-1.11/CToolKit/Errors/__init__.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      811 2023-06-18 18:20:38.000000 CToolKit-1.11/CToolKit/__init__.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1459 2023-06-18 20:23:25.000000 CToolKit-1.11/CToolKit/amalgamation.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     4637 2023-06-18 19:58:16.000000 CToolKit-1.11/CToolKit/comand_line_functions.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2967 2023-06-18 20:01:08.000000 CToolKit-1.11/CToolKit/readme_converter.py
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:36:13.465931 CToolKit-1.11/CToolKit.egg-info/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3370 2023-06-18 21:36:13.000000 CToolKit-1.11/CToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      566 2023-06-18 21:36:13.000000 CToolKit-1.11/CToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        1 2023-06-18 21:36:13.000000 CToolKit-1.11/CToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        9 2023-06-18 21:36:13.000000 CToolKit-1.11/CToolKit.egg-info/top_level.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1060 2023-06-17 02:11:11.000000 CToolKit-1.11/LICENSE
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3370 2023-06-18 21:36:13.485931 CToolKit-1.11/PKG-INFO
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2961 2023-06-18 21:35:32.000000 CToolKit-1.11/README.md
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)       38 2023-06-18 21:36:13.485931 CToolKit-1.11/setup.cfg
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      664 2023-06-18 21:36:08.000000 CToolKit-1.11/setup.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-19 15:25:02.228693 CToolKit-1.12/
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-19 15:25:02.224693 CToolKit-1.12/CToolKit/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      504 2023-06-18 19:59:56.000000 CToolKit-1.12/CToolKit/ComandLineExecution.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-19 15:25:02.228693 CToolKit-1.12/CToolKit/Errors/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      306 2023-06-17 06:47:02.000000 CToolKit-1.12/CToolKit/Errors/ComandLineError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      226 2023-06-17 06:58:51.000000 CToolKit-1.12/CToolKit/Errors/ComandLineWarning.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      110 2023-06-17 06:48:41.000000 CToolKit-1.12/CToolKit/Errors/CopilationError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      118 2023-06-17 06:49:33.000000 CToolKit-1.12/CToolKit/Errors/CopilationWarning.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      108 2023-06-17 06:47:14.000000 CToolKit-1.12/CToolKit/Errors/ExecutionError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      116 2023-06-17 06:57:42.000000 CToolKit-1.12/CToolKit/Errors/ValgrindError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      115 2023-06-17 07:04:59.000000 CToolKit-1.12/CToolKit/Errors/ValgrindLeak.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        0 2023-06-17 04:59:48.000000 CToolKit-1.12/CToolKit/Errors/__init__.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      813 2023-06-19 15:08:57.000000 CToolKit-1.12/CToolKit/__init__.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1459 2023-06-18 20:23:25.000000 CToolKit-1.12/CToolKit/amalgamation.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     4653 2023-06-19 15:20:15.000000 CToolKit-1.12/CToolKit/comand_line_functions.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2967 2023-06-18 20:01:08.000000 CToolKit-1.12/CToolKit/readme_converter.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-19 15:25:02.224693 CToolKit-1.12/CToolKit.egg-info/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3330 2023-06-19 15:25:02.000000 CToolKit-1.12/CToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      566 2023-06-19 15:25:02.000000 CToolKit-1.12/CToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        1 2023-06-19 15:25:02.000000 CToolKit-1.12/CToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        9 2023-06-19 15:25:02.000000 CToolKit-1.12/CToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1060 2023-06-17 02:11:11.000000 CToolKit-1.12/LICENSE
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3330 2023-06-19 15:25:02.228693 CToolKit-1.12/PKG-INFO
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2921 2023-06-19 15:21:21.000000 CToolKit-1.12/README.md
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)       38 2023-06-19 15:25:02.228693 CToolKit-1.12/setup.cfg
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      664 2023-06-19 15:24:57.000000 CToolKit-1.12/setup.py
```

### Comparing `CToolKit-1.11/CToolKit/__init__.py` & `CToolKit-1.12/CToolKit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from CToolKit.amalgamation import  generate_amalgamated_code
 from CToolKit.ComandLineExecution import ComandLineExecution
-from CToolKit.comand_line_functions import copile_project_by_command
-from CToolKit.comand_line_functions import copile_project
+from CToolKit.comand_line_functions import compile_project_by_command
+from CToolKit.comand_line_functions import compile_project
 from CToolKit.comand_line_functions import test_binary_with_valgrind
 from CToolKit.comand_line_functions import execute_test_for_file
 from CToolKit.comand_line_functions import execute_test_for_folder
 
 
 from CToolKit.Errors.CopilationError import CopilationError
 from CToolKit.Errors.CopilationWarning import CopilationWarning
```

### Comparing `CToolKit-1.11/CToolKit/amalgamation.py` & `CToolKit-1.12/CToolKit/amalgamation.py`

 * *Files identical despite different names*

### Comparing `CToolKit-1.11/CToolKit/comand_line_functions.py` & `CToolKit-1.12/CToolKit/comand_line_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from CToolKit.Errors.ValgrindLeak import  ValgrindLeak
 from CToolKit.ComandLineExecution import ComandLineExecution
 
 from platform import system as current_os
 
 from os import listdir,remove
 
-def copile_project_by_command(command: str, raise_errors: bool = True, raise_warnings: bool = True):
+
+def compile_project_by_command(command: str, raise_errors: bool = True, raise_warnings: bool = True):
     """execute an copilation with the given comand
     Args:
         command (str): the comand copilation ,ex: 'gcc test.c'
         raise_errors (bool, optional): if its to raise An copilation Error
         raise_warnings (bool, optional): if is to raise an warning Error
 
     Raises:
@@ -29,20 +30,20 @@
         raise CopilationError(result.output, result.status_code)
 
 
     if raise_warnings and 'warning:' in result.output:
         raise CopilationWarning(result.output)
 
 
-def copile_project(compiler: str, file: str, output: str = None, flags: List[str] = None, raise_errors: bool = True,
+def compile_project(compiler: str, file: str, output: str = None, flags: List[str] = None, raise_errors: bool = True,
                     raise_warnings: bool = True)->str:
     """Copiles an project file
 
     Args:
-        compiler (str): the current copiler , ex: gcc,clang
+        compiler (str): the current compiler , ex: gcc,clang
         file (str): the file to copile, ex: test.c
         output (str, optional): the file output, ex: test.out ,if were None , it will be
         the file replaced with .out or .exe
         flags (List[str], optional): the optional flags copilatin
         raise_errors (bool, optional): if its to raise An copilation Error
         raise_warnings (bool, optional): if is to raise an warning Error
 
@@ -56,15 +57,15 @@
     if output is None:
         if current_os() == 'Windows':
             output = file.replace('.c', 'exe').replace('.cpp', '.exe')
         else:
             output = file.replace('.c', '.out').replace('.cpp', '.out')
 
     command = f'{compiler} {file} -o {output} ' + ' '.join(flags)
-    copile_project_by_command(command, raise_errors, raise_warnings)
+    compile_project_by_command(command, raise_errors, raise_warnings)
     return output
 
 
 
 
 
 def test_binary_with_valgrind(binary_file:str,flags: List[str]= None):
@@ -86,53 +87,53 @@
     if 'ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 0 from 0)' not in result.output:
         raise ValgrindError(result.output)
 
     if 'All heap blocks were freed -- no leaks are possible' not in result.output:
         raise ValgrindLeak(result.output)
 
 
-def execute_test_for_file(copiler:str, file: str):
+def execute_test_for_file(compiler:str, file: str):
     """Execute an presset test for the current file
     Args:
-        copiler (str): the copiler to use, ex: gcc or clang
+        compiler (str): the compiler to use, ex: gcc or clang
         file (str): the file to copile , ex: test.c
 
     Raises:
         e: all possible errors
     """
-    result = copile_project(
-        copiler,
+    result = compile_project(
+        compiler,
         file,
         raise_errors=True,
         raise_warnings=False
     )
     try:
         test_binary_with_valgrind(result)
         remove(result)
     except Exception as e:
         remove(result)
         raise e
 
 
-def execute_test_for_folder(copiler:str, folder: str,print_values:bool = True):
+def execute_test_for_folder(compiler:str, folder: str, print_values:bool = True):
     """execute tests for all .c or cpp files in the given folder
     Args:
-        copiler (str): the copiler, ex: gcc , or clang
+        compiler (str): the compiler, ex: gcc , or clang
         folder (str): the folder to copile
         print_values (bool, optional): if is to print errors and sucess
     Raises:
         e: if happen some error
     """
     files = listdir(folder)
     for file in files:
         if not file.endswith('.c') or file.endswith('.cpp'):
             continue
 
         try:
-            execute_test_for_file(copiler,f'{folder}/{file}')
+            execute_test_for_file(compiler, f'{folder}/{file}')
             if print_values:
                 print('\033[92m'+f'passed: {file}' + '\33[37m')
 
         except Exception as e:
             if print_values:
                 print('\033[91m' + f'fail with file: {file}' + '\33[37m')
                 print('\033[0m')
```

### Comparing `CToolKit-1.11/CToolKit/readme_converter.py` & `CToolKit-1.12/CToolKit/readme_converter.py`

 * *Files identical despite different names*

### Comparing `CToolKit-1.11/CToolKit.egg-info/PKG-INFO` & `CToolKit-1.12/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: CToolKit
-Version: 1.11
-Summary: CToolKit to manipulate CPipeLines and Repos
-Home-page: https://oui.tec.br/
-Author: Mateus Moutinho
-Author-email: mateusmoutinho01@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CToolkit
  is An Python Package to manipulate C/C++ buildings and  PipeLines
  providing easy automation tools to increase your code pipelines 
  with amalgamations, black box testing, and readme replacment
 
 ### Instalation from Pip
 for install the lib from pip call 
@@ -62,100 +49,101 @@
 OUTPUT = 'amalgamated.h'
 amalgamated_code = ct.generate_amalgamated_code(STARTER,OUTPUT)
 
 ~~~
 
 ### Comand Line Operations
 
-#### Copile an Project 
-it wil copile the given file 
+#### Compile an Project 
+it wil copile the given file
 
 ~~~python
 
 
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 ~~~
 
 #### Testing copilation with valgrind 
 
 Execute an valgrind testing of the given binary ( you need to have valgrind installed in your os)
 
 ~~~python
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
-
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 
 FLAGS = ['-libcur']
-ct.test_binary_with_valgrind(OUTPUT,FLAGS)
+ct.test_binary_with_valgrind(OUTPUT, FLAGS)
 ~~~
 Executing copilation and test with file with a single comand 
 ~~~python
 import CToolKit as ct
 
-COPILER = 'gcc'
+COMPILER = 'gcc'
 FILE = 'test.c'
 
-ct.execute_test_for_file(COPILER,FILE)
+ct.execute_test_for_file(COMPILER,FILE)
 
 ~~~
 
 Executing Test with all .c or .cpp files in the given folder 
 
 ~~~python 
 
 import CToolKit as ct
 
-COPILER = 'gcc'
+COMPILER = 'gcc'
 FOLDER ='test'
-ct.execute_test_for_folder(COPILER,FOLDER,print_values=True)
+ct.execute_test_for_folder(COMPILER,FOLDER,print_values=True)
 
 ~~~
 
 #### Execution 
 you can execute an binary with the ComandLine Execution class
 
 ~~~python
 
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
-
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 
 execution = ct.ComandLineExecution(f'./{OUTPUT}')
 
-print('output:',execution.output)
-print('statuscode:',execution.status_code)
+print('output:', execution.output)
+print('statuscode:', execution.status_code)
 ~~~
 #### Readme Replacement 
 you can replace readme content with code system 
 for these just tipe: < + !--codeof:test.c-->, you can see 
 these example in the following lib:
 https://github.com/OUIsolutions/CTextEngine
```

### Comparing `CToolKit-1.11/CToolKit.egg-info/SOURCES.txt` & `CToolKit-1.12/CToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CToolKit-1.11/LICENSE` & `CToolKit-1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `CToolKit-1.11/PKG-INFO` & `CToolKit-1.12/CToolKit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CToolKit
-Version: 1.11
+Version: 1.12
 Summary: CToolKit to manipulate CPipeLines and Repos
 Home-page: https://oui.tec.br/
 Author: Mateus Moutinho
 Author-email: mateusmoutinho01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,100 +62,101 @@
 OUTPUT = 'amalgamated.h'
 amalgamated_code = ct.generate_amalgamated_code(STARTER,OUTPUT)
 
 ~~~
 
 ### Comand Line Operations
 
-#### Copile an Project 
-it wil copile the given file 
+#### Compile an Project 
+it wil copile the given file
 
 ~~~python
 
 
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 ~~~
 
 #### Testing copilation with valgrind 
 
 Execute an valgrind testing of the given binary ( you need to have valgrind installed in your os)
 
 ~~~python
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
-
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 
 FLAGS = ['-libcur']
-ct.test_binary_with_valgrind(OUTPUT,FLAGS)
+ct.test_binary_with_valgrind(OUTPUT, FLAGS)
 ~~~
 Executing copilation and test with file with a single comand 
 ~~~python
 import CToolKit as ct
 
-COPILER = 'gcc'
+COMPILER = 'gcc'
 FILE = 'test.c'
 
-ct.execute_test_for_file(COPILER,FILE)
+ct.execute_test_for_file(COMPILER,FILE)
 
 ~~~
 
 Executing Test with all .c or .cpp files in the given folder 
 
 ~~~python 
 
 import CToolKit as ct
 
-COPILER = 'gcc'
+COMPILER = 'gcc'
 FOLDER ='test'
-ct.execute_test_for_folder(COPILER,FOLDER,print_values=True)
+ct.execute_test_for_folder(COMPILER,FOLDER,print_values=True)
 
 ~~~
 
 #### Execution 
 you can execute an binary with the ComandLine Execution class
 
 ~~~python
 
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
-
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 
 execution = ct.ComandLineExecution(f'./{OUTPUT}')
 
-print('output:',execution.output)
-print('statuscode:',execution.status_code)
+print('output:', execution.output)
+print('statuscode:', execution.status_code)
 ~~~
 #### Readme Replacement 
 you can replace readme content with code system 
 for these just tipe: < + !--codeof:test.c-->, you can see 
 these example in the following lib:
 https://github.com/OUIsolutions/CTextEngine
```

### Comparing `CToolKit-1.11/README.md` & `CToolKit-1.12/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: CToolKit
+Version: 1.12
+Summary: CToolKit to manipulate CPipeLines and Repos
+Home-page: https://oui.tec.br/
+Author: Mateus Moutinho
+Author-email: mateusmoutinho01@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CToolkit
  is An Python Package to manipulate C/C++ buildings and  PipeLines
  providing easy automation tools to increase your code pipelines 
  with amalgamations, black box testing, and readme replacment
 
 ### Instalation from Pip
 for install the lib from pip call 
@@ -49,100 +62,101 @@
 OUTPUT = 'amalgamated.h'
 amalgamated_code = ct.generate_amalgamated_code(STARTER,OUTPUT)
 
 ~~~
 
 ### Comand Line Operations
 
-#### Copile an Project 
-it wil copile the given file 
+#### Compile an Project 
+it wil copile the given file
 
 ~~~python
 
 
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 ~~~
 
 #### Testing copilation with valgrind 
 
 Execute an valgrind testing of the given binary ( you need to have valgrind installed in your os)
 
 ~~~python
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
-
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 
 FLAGS = ['-libcur']
-ct.test_binary_with_valgrind(OUTPUT,FLAGS)
+ct.test_binary_with_valgrind(OUTPUT, FLAGS)
 ~~~
 Executing copilation and test with file with a single comand 
 ~~~python
 import CToolKit as ct
 
-COPILER = 'gcc'
+COMPILER = 'gcc'
 FILE = 'test.c'
 
-ct.execute_test_for_file(COPILER,FILE)
+ct.execute_test_for_file(COMPILER,FILE)
 
 ~~~
 
 Executing Test with all .c or .cpp files in the given folder 
 
 ~~~python 
 
 import CToolKit as ct
 
-COPILER = 'gcc'
+COMPILER = 'gcc'
 FOLDER ='test'
-ct.execute_test_for_folder(COPILER,FOLDER,print_values=True)
+ct.execute_test_for_folder(COMPILER,FOLDER,print_values=True)
 
 ~~~
 
 #### Execution 
 you can execute an binary with the ComandLine Execution class
 
 ~~~python
 
 import CToolKit as ct
-COPILER = 'gcc'
+
+COMPILER = 'gcc'
 
 FILE = 'test.c'
 OUTPUT = 'test.out'
-ct.copile_project(
-    COPILER,
-    FILE,
-    OUTPUT,
-    raise_errors=True,
-    raise_warnings=True
-    )
-
+ct.compile_project(
+ COMPILER,
+ FILE,
+ OUTPUT,
+ raise_errors=True,
+ raise_warnings=True
+)
 
 execution = ct.ComandLineExecution(f'./{OUTPUT}')
 
-print('output:',execution.output)
-print('statuscode:',execution.status_code)
+print('output:', execution.output)
+print('statuscode:', execution.status_code)
 ~~~
 #### Readme Replacement 
 you can replace readme content with code system 
 for these just tipe: < + !--codeof:test.c-->, you can see 
 these example in the following lib:
 https://github.com/OUIsolutions/CTextEngine
```

### Comparing `CToolKit-1.11/setup.py` & `CToolKit-1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='CToolKit',
-    version='1.11',
+    version='1.12',
     description='CToolKit to manipulate CPipeLines and Repos',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mateus Moutinho',
     author_email='mateusmoutinho01@gmail.com',
     url='https://oui.tec.br/',
     packages=find_packages(),
```

