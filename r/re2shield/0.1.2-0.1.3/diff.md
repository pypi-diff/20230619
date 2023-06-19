# Comparing `tmp/re2shield-0.1.2.tar.gz` & `tmp/re2shield-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re2shield-0.1.2.tar", last modified: Wed Jun 14 04:57:45 2023, max compression
+gzip compressed data, was "re2shield-0.1.3.tar", last modified: Mon Jun 19 09:26:41 2023, max compression
```

## Comparing `re2shield-0.1.2.tar` & `re2shield-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 04:57:45.269178 re2shield-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     4559 2023-06-14 04:57:45.269178 re2shield-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-14 04:57:29.000000 re2shield-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 04:57:45.268178 re2shield-0.1.2/re2shield/
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-14 04:52:45.000000 re2shield-0.1.2/re2shield/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-06-14 04:52:45.000000 re2shield-0.1.2/re2shield/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 04:57:45.268178 re2shield-0.1.2/re2shield.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4559 2023-06-14 04:57:45.000000 re2shield-0.1.2/re2shield.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-14 04:57:45.000000 re2shield-0.1.2/re2shield.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 04:57:45.000000 re2shield-0.1.2/re2shield.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-14 04:57:45.000000 re2shield-0.1.2/re2shield.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-14 04:57:45.000000 re2shield-0.1.2/re2shield.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 04:57:45.269178 re2shield-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-14 04:52:57.000000 re2shield-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 04:57:45.269178 re2shield-0.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 04:52:45.000000 re2shield-0.1.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      815 2023-06-14 04:56:56.000000 re2shield-0.1.2/tests/test_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:26:41.776641 re2shield-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)     5510 2023-06-19 09:26:41.776641 re2shield-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4276 2023-06-19 09:23:22.000000 re2shield-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:26:41.775642 re2shield-0.1.3/re2shield/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-19 09:06:53.000000 re2shield-0.1.3/re2shield/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2023-06-19 09:12:42.000000 re2shield-0.1.3/re2shield/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:26:41.776641 re2shield-0.1.3/re2shield.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5510 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 09:26:41.776641 re2shield-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-19 09:08:11.000000 re2shield-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:26:41.776641 re2shield-0.1.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 09:06:53.000000 re2shield-0.1.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-19 09:24:22.000000 re2shield-0.1.3/tests/test_core.py
```

### Comparing `re2shield-0.1.2/PKG-INFO` & `re2shield-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,89 @@
-Metadata-Version: 2.1
-Name: re2shield
-Version: 0.1.2
-Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
-Home-page: https://github.com/Npc-coder/re2shield
-Author: mkCha
-Author-email: dxsaq0@gmail.com
-License: UNKNOWN
-Description: # re2shield
-        `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
-        
-        It allows you to compile and search for patterns in text using the powerful regular expression engine provided by `re2`.
-        
-        It allows you to hide the complexity of regular expressions and work with pattern identifiers instead.
-        
-        This project utilizes the `google/re2` library, which is licensed under the BSD 3-Clause License. Please refer to the [LICENSE](https://github.com/google/re2/blob/main/LICENSE) file of `google/re2` for more information.
-        
-        
-        
-        ## Installation
-        Before installing `re2shield`, make sure that `re2` is installed on your system. You can install `re2` by following the instructions on the [google/re2](https://github.com/google/re2.git) GitHub repository.
-        
-        Alternatively, you can use the `re2-installer.sh` script located in the `package/installed` directory. This script automates the installation process for `re2` and its dependencies. Simply run the script using the following command:
-        
-        ```shell
-        git clone https://github.com/Npc-coder/re2shield.git
-        cd re2shield
-        sh re2-installer.sh
-        ```
-        
-        You can install `re2shield` using pip:
-        ```shell
-        pip install re2shield
-        ```
-        or
-        ```shell
-        git clone https://github.com/Npc-coder/re2shield.git
-        cd re2shield
-        pip install .
-        ```
-        
-        ## Usage
-        
-        ### Importing the Library
-        Here is a simple example demonstrating how to use re2shield:
-        
-        ```python
-        import re2shield
-        
-        if __name__ == "__main__":
-            db = re2shield.Database()
-        
-            # Load patterns from file
-            try:
-                db = re2shield.load('patterns.pkl')
-            except FileNotFoundError:
-                # If pattern file doesn't exist, compile the patterns
-                patterns = [
-                    (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1, None),
-                    (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2, None),
-                    (r'\d+', 3, None)
-                ]
-        
-                expressions, ids, flags = zip(*patterns)
-                db.compile(expressions=expressions, ids=ids, flags=flags)
-                db.dump('patterns.pkl')
-        
-            # Find patterns in text
-            def match_handler(id, from_, to, flags, context):
-                print(f"Match found for pattern {id} from {from_} to {to}: {context}")
-        
-            db.scan('test@ex12ample12.com', match_handler)
-        ```
-        In this example, we create a re2shield.Database object, compile a list of patterns with their corresponding identifiers, and then search for those patterns in the provided text. 
-        
-        The match_handler function is called for each match found, allowing you to process the matches as desired.
-        
-        ## Use Case
-        One of the key advantages of re2shield is its ability to hide the actual regular expression patterns from users during distribution. By compiling the patterns with re2 and using pattern identifiers, you can distribute your code without exposing the underlying regular expression logic. This provides an additional layer of abstraction and enhances the security of your regular expression patterns.
-        
-        ## Features
-        - Hide the complexity of regular expressions
-        - Work with pattern identifiers instead of exposing the actual regular expression patterns
-        - Compile patterns for efficient matching
-        - Find all occurrences of patterns in text
-        - Customize the handling of matches using callback functions
-        
-        
-        ## License
-        This project is licensed under the BSD 3-Clause License. See the [LICENSE](https://opensource.org/license/bsd-3-clause/) file for details.
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
+# re2shield
+`re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
+
+It allows you to compile and search for patterns in text using the powerful regular expression engine provided by `re2`.
+
+It allows you to hide the complexity of regular expressions and work with pattern identifiers instead.
+
+This project utilizes the `google/re2` library, which is licensed under the BSD 3-Clause License. Please refer to the [LICENSE](https://github.com/google/re2/blob/main/LICENSE) file of `google/re2` for more information.
+
+
+
+## Installation
+Before installing `re2shield`, make sure that `re2` is installed on your system. You can install `re2` by following the instructions on the [google/re2](https://github.com/google/re2.git) GitHub repository.
+
+Alternatively, you can use the `re2-installer.sh` script located in the `package/installed` directory. This script automates the installation process for `re2` and its dependencies. Simply run the script using the following command:
+
+```shell
+git clone https://github.com/Npc-coder/re2shield.git
+cd re2shield/installed
+sh re2-installer.sh
+```
+
+You can install `re2shield` using pip:
+```shell
+pip install re2shield
+```
+or
+```shell
+git clone https://github.com/Npc-coder/re2shield.git
+cd re2shield
+pip install .
+```
+
+## Updates
+### Version 0.1.3
+- Added the ability to count the number of patterns in the Re2ShieldDatabase. You can now print the Re2Shield object to see the number of compiled patterns.
+- Added an 'overwrite' option to the compile method in Re2Shield. If 'overwrite' is False (default), new patterns are added to the existing ones. If 'overwrite' is True, new patterns replace the existing ones.
+- Enhanced ID duplication check. Now it checks for ID duplication not only among the new patterns but also between the new patterns and the existing ones in the database. If a duplicate ID is found and 'overwrite' is False, a ValueError is raised.
+Please refer to the [Usage](#usage) section for examples of how to use these new features.
+
+## Usage
+### Importing the Library
+Here is a simple example demonstrating how to use re2shield:
+
+```python
+import re2shield
+
+if __name__ == "__main__":
+    db = re2shield.Database()
+
+    # Load patterns from file
+    try:
+        db = re2shield.load('patterns.pkl')
+        print(db)  # Prints the number of patterns in the database
+    except FileNotFoundError:
+        # If pattern file doesn't exist, compile the patterns
+        patterns = [
+            (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1, None),
+            (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2, None),
+            (r'\d+', 3, None)
+        ]
+
+        expressions, ids, flags = zip(*patterns)
+        db.compile(expressions=expressions, ids=ids, flags=flags, overwrite=False)
+        print(db)  # Prints the number of patterns in the database
+        db.dump('patterns.pkl')
+
+    # Find patterns in text
+    def match_handler(id, from_, to, flags, context):
+        print(f"Match found for pattern {id} from {from_} to {to}: {context}")
+
+    db.scan('test@ex12ample12.com', match_handler)
+```
+In this example, we create a re2shield.Database object, compile a list of patterns with their corresponding identifiers, and then search for those patterns in the provided text. 
+
+The match_handler function is called for each match found, allowing you to process the matches as desired.
+
+## Use Case
+One of the key advantages of re2shield is its ability to hide the actual regular expression patterns from users during distribution. By compiling the patterns with re2 and using pattern identifiers, you can distribute your code without exposing the underlying regular expression logic. This provides an additional layer of abstraction and enhances the security of your regular expression patterns.
+
+## Features
+- Hide the complexity of regular expressions
+- Work with pattern identifiers instead of exposing the actual regular expression patterns
+- Compile patterns for efficient matching
+- Find all occurrences of patterns in text
+- Customize the handling of matches using callback functions
+
+## License
+This project is licensed under the BSD 3-Clause License. See the [LICENSE](https://opensource.org/license/bsd-3-clause/) file for details.
```

### Comparing `re2shield-0.1.2/re2shield/core.py` & `re2shield-0.1.3/re2shield/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,34 +8,46 @@
 
     def findall(self, text, callback):
         for id, pattern in self.re2_patterns.items():
             matches = pattern.finditer(text)
             for match in matches:
                 callback(id, match.start(), match.end(), None, match.group())
 
+    def count_patterns(self):
+        return len(self.re2_patterns)
+
 class Re2Shield:
     def __init__(self):
         self.db = None
 
-    def compile(self, expressions, ids, flags):
+    def __str__(self):
+        if self.db is not None:
+            return f"Re2Shield Database with {self.db.count_patterns()} patterns."
+        else:
+            return "Re2Shield Database is not compiled."
+
+    def compile(self, expressions, ids, flags, overwrite=False):
         if len(expressions) != len(ids) != len(flags):
             raise ValueError("All parameters should have the same length")
 
-        # 중복된 ID가 있는지 확인
-        if len(ids) != len(set(ids)):
-            raise ValueError("IDs should be unique")
-
         re2_patterns = {}
         raw_patterns = {}
+        if not overwrite and self.db is not None:
+            re2_patterns = self.db.re2_patterns.copy()
+            raw_patterns = self.db.raw_patterns.copy()
+
         for id, expr, flag in zip(ids, expressions, flags):
+            if id in re2_patterns:
+                raise ValueError(f"ID {id} already exists in the database. To overwrite, set overwrite=True.")
             re2_patterns[id] = re2.compile(expr, flag)
             raw_patterns[id] = (expr, flag)
 
         self.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
 
+
     def dump(self, file_path):
         if self.db is not None:
             with open(file_path, 'wb') as f:
                 pickle.dump(self.db.raw_patterns, f)
         else:
             raise ValueError("No compiled database found. Please compile patterns first.")
 
@@ -49,10 +61,8 @@
 
 def load(file_path):
     with open(file_path, 'rb') as f:
         raw_patterns = pickle.load(f)
         re2_patterns = {id: re2.compile(expr, flag) for id, (expr, flag) in raw_patterns.items()}
     re2_shield = Re2Shield()
     re2_shield.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
-    return re2_shield
-    return db
-
+    return re2_shield
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `re2shield-0.1.2/re2shield.egg-info/PKG-INFO` & `re2shield-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -20,53 +20,61 @@
         ## Installation
         Before installing `re2shield`, make sure that `re2` is installed on your system. You can install `re2` by following the instructions on the [google/re2](https://github.com/google/re2.git) GitHub repository.
         
         Alternatively, you can use the `re2-installer.sh` script located in the `package/installed` directory. This script automates the installation process for `re2` and its dependencies. Simply run the script using the following command:
         
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
-        cd re2shield
+        cd re2shield/installed
         sh re2-installer.sh
         ```
         
         You can install `re2shield` using pip:
         ```shell
         pip install re2shield
         ```
         or
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
-        ## Usage
+        ## Updates
+        ### Version 0.1.3
+        - Added the ability to count the number of patterns in the Re2ShieldDatabase. You can now print the Re2Shield object to see the number of compiled patterns.
+        - Added an 'overwrite' option to the compile method in Re2Shield. If 'overwrite' is False (default), new patterns are added to the existing ones. If 'overwrite' is True, new patterns replace the existing ones.
+        - Enhanced ID duplication check. Now it checks for ID duplication not only among the new patterns but also between the new patterns and the existing ones in the database. If a duplicate ID is found and 'overwrite' is False, a ValueError is raised.
+        Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
+        ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
         
         ```python
         import re2shield
         
         if __name__ == "__main__":
             db = re2shield.Database()
         
             # Load patterns from file
             try:
                 db = re2shield.load('patterns.pkl')
+                print(db)  # Prints the number of patterns in the database
             except FileNotFoundError:
                 # If pattern file doesn't exist, compile the patterns
                 patterns = [
                     (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1, None),
                     (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2, None),
                     (r'\d+', 3, None)
                 ]
         
                 expressions, ids, flags = zip(*patterns)
-                db.compile(expressions=expressions, ids=ids, flags=flags)
+                db.compile(expressions=expressions, ids=ids, flags=flags, overwrite=False)
+                print(db)  # Prints the number of patterns in the database
                 db.dump('patterns.pkl')
         
             # Find patterns in text
             def match_handler(id, from_, to, flags, context):
                 print(f"Match found for pattern {id} from {from_} to {to}: {context}")
         
             db.scan('test@ex12ample12.com', match_handler)
@@ -81,15 +89,14 @@
         ## Features
         - Hide the complexity of regular expressions
         - Work with pattern identifiers instead of exposing the actual regular expression patterns
         - Compile patterns for efficient matching
         - Find all occurrences of patterns in text
         - Customize the handling of matches using callback functions
         
-        
         ## License
         This project is licensed under the BSD 3-Clause License. See the [LICENSE](https://opensource.org/license/bsd-3-clause/) file for details.
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `re2shield-0.1.2/setup.py` & `re2shield-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='re2shield',
-    version='0.1.2',
+    version='0.1.3',
     url='https://github.com/Npc-coder/re2shield',  # Replace with your own GitHub project URL
     author='mkCha',
     author_email='dxsaq0@gmail.com',
     description='A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

