# Comparing `tmp/csv-wizard-0.4.2.post1.tar.gz` & `tmp/csv-wizard-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-wizard-0.4.2.post1.tar", last modified: Thu Apr 27 20:09:19 2023, max compression
+gzip compressed data, was "csv-wizard-1.0.0.tar", last modified: Mon Jun 19 13:02:30 2023, max compression
```

## Comparing `csv-wizard-0.4.2.post1.tar` & `csv-wizard-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
--rw-r--r--   0        0        0     1099 2023-04-13 12:46:11.220776 csv-wizard-0.4.2.post1/LICENSE
--rw-r--r--   0        0        0      493 2023-04-27 20:09:07.666783 csv-wizard-0.4.2.post1/pyproject.toml
--rw-r--r--   0        0        0     9074 2023-04-26 21:18:31.649684 csv-wizard-0.4.2.post1/README.md
--rw-r--r--   0        0        0        0 2023-02-19 02:10:32.471751 csv-wizard-0.4.2.post1/src/csv_wizard/__init__.py
--rw-r--r--   0        0        0    11621 2023-04-25 12:48:02.175388 csv-wizard-0.4.2.post1/src/csv_wizard/csv_wizard.py
--rw-r--r--   0        0        0       39 2023-02-16 02:52:30.274333 csv-wizard-0.4.2.post1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-16 02:52:30.275330 csv-wizard-0.4.2.post1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-02-16 02:52:30.273335 csv-wizard-0.4.2.post1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      251 2023-02-16 02:52:30.275330 csv-wizard-0.4.2.post1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302624 csv-wizard-0.4.2.post1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302950 csv-wizard-0.4.2.post1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      689 2023-04-25 12:46:45.058770 csv-wizard-0.4.2.post1/tests/test_divide.py
--rw-r--r--   0        0        0      261 2023-04-25 12:46:45.043745 csv-wizard-0.4.2.post1/tests/test_encoding.py
--rw-r--r--   0        0        0      628 2023-04-25 12:48:02.485401 csv-wizard-0.4.2.post1/tests/test_find_common_rows.py
--rw-r--r--   0        0        0      541 2023-04-25 12:46:45.073859 csv-wizard-0.4.2.post1/tests/test_find_different_rows.py
--rw-r--r--   0        0        0      616 2023-04-25 12:48:02.522568 csv-wizard-0.4.2.post1/tests/test_get_all_rows.py
--rw-r--r--   0        0        0      979 2023-04-25 12:48:02.541536 csv-wizard-0.4.2.post1/tests/test_get_dialect.py
--rw-r--r--   0        0        0      846 2023-04-25 12:46:45.068689 csv-wizard-0.4.2.post1/tests/test_get_duplicates.py
--rw-r--r--   0        0        0      431 2023-04-25 12:48:02.573957 csv-wizard-0.4.2.post1/tests/test_get_headers.py
--rw-r--r--   0        0        0     1541 2023-04-25 12:48:02.592401 csv-wizard-0.4.2.post1/tests/test_misc.py
--rw-r--r--   0        0        0      284 2023-04-25 12:48:02.609419 csv-wizard-0.4.2.post1/tests/test_slice.py
--rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 csv-wizard-0.4.2.post1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-13 12:46:11.220776 csv-wizard-1.0.0/LICENSE
+-rw-r--r--   0        0        0      529 2023-06-19 12:54:35.526954 csv-wizard-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9516 2023-06-19 12:29:04.878243 csv-wizard-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-19 02:10:32.471751 csv-wizard-1.0.0/src/__init__.py
+-rw-r--r--   0        0        0    11690 2023-06-19 12:53:52.145338 csv-wizard-1.0.0/src/csv_wizard.py
+-rw-r--r--   0        0        0       39 2023-02-16 02:52:30.274333 csv-wizard-1.0.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-02-16 02:52:30.275330 csv-wizard-1.0.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-02-16 02:52:30.273335 csv-wizard-1.0.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      251 2023-02-16 02:52:30.275330 csv-wizard-1.0.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302624 csv-wizard-1.0.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302950 csv-wizard-1.0.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-06-15 12:57:01.556547 csv-wizard-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      852 2023-06-19 12:23:08.073079 csv-wizard-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:26:56.159429 csv-wizard-1.0.0/tests/empty.csv
+-rw-r--r--   0        0        0      698 2023-06-19 12:23:08.043157 csv-wizard-1.0.0/tests/test_divide.py
+-rw-r--r--   0        0        0      256 2023-06-19 12:23:08.026358 csv-wizard-1.0.0/tests/test_encoding.py
+-rw-r--r--   0        0        0      206 2023-06-16 16:32:30.995957 csv-wizard-1.0.0/tests/test_file_backup.csv
+-rw-r--r--   0        0        0      257 2023-06-16 15:20:44.927006 csv-wizard-1.0.0/tests/test_file_diff.csv
+-rw-r--r--   0        0        0      273 2023-06-16 15:16:32.197038 csv-wizard-1.0.0/tests/test_file_with_dups.csv
+-rw-r--r--   0        0        0      610 2023-06-19 12:23:08.060112 csv-wizard-1.0.0/tests/test_find_common_rows.py
+-rw-r--r--   0        0        0      750 2023-06-19 12:23:08.039169 csv-wizard-1.0.0/tests/test_find_different_rows.py
+-rw-r--r--   0        0        0      634 2023-06-19 12:23:08.011398 csv-wizard-1.0.0/tests/test_get_all_rows.py
+-rw-r--r--   0        0        0     1025 2023-06-19 12:23:08.022667 csv-wizard-1.0.0/tests/test_get_dialect.py
+-rw-r--r--   0        0        0      938 2023-06-19 12:23:08.080060 csv-wizard-1.0.0/tests/test_get_duplicates.py
+-rw-r--r--   0        0        0      437 2023-06-16 15:19:38.891982 csv-wizard-1.0.0/tests/test_get_headers.py
+-rw-r--r--   0        0        0     1392 2023-06-19 12:23:08.100021 csv-wizard-1.0.0/tests/test_misc.py
+-rw-r--r--   0        0        0      334 2023-06-19 12:23:08.068246 csv-wizard-1.0.0/tests/test_slice.py
+-rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 csv-wizard-1.0.0/PKG-INFO
```

### Comparing `csv-wizard-0.4.2.post1/LICENSE` & `csv-wizard-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2.post1/README.md` & `csv-wizard-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# CSV Wizard
+# csv wizard
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 ***
-## Import a CSV file by only giving the `CSVParser` class a `string` containing the full name of the file without the *.csv* extension.
-> `new_file = CSVParser("my_file")`
+## Import a CSV file by only giving the `CSVWizard` class a `string` containing the full name of the file without the *.csv* extension.
+> `new_file = CSVWizard("my_file")`
 ***
 ## Handling decoding/encoding on a file.
 All methods have an optional `encoding` argument.
 If left empty, csv_wizard will attempt to automatically figure out the encoding, however, if a `UnicodeDecodeError` or `UnicodeEncodeError` error are raised, the encoding should be specified manually. 
 The encoding parameter accepts strings.
 ```
 > file1.get_row_count(encoding='utf-8') 
 ```
 ***
 ### Getting the characters that define the CSV file's layout. The `get_dialect` method.
-Calling this method on a CSVParser object returns it's dialect property.
+Calling this method on a CSVWizard object returns it's dialect property.
 The dialect property contains:
 * lineterminator
 * quoting
 * doublequote
 * delimiter
 * quotechar
 * skipinitialspace
@@ -41,15 +41,15 @@
 **Predefined paths**
 
 There are three predefined global variables you can use: 
 * `CURRENT_DIR` to get the current directory
 * `CURRENT_PARENT_DIR` to get the parent directory of the current location
 * `ABSOLUTE_PATH` to get the current absolute path
 
-> `CSVParser.create(name="new-file", path=CURRENT_PARENT_DIR)`
+> `CSVWizard.create(name="new-file", path=CURRENT_PARENT_DIR)`
 ***
 ### Getting the headers row. The `get_headers()` method.
 Returns only the first line on the CSV file, which is presumed to be the one containing the headers.
 > ``new_file.get_headers()`` # ["Name", "Email"]
 
 ***
 ### Getting the total number of rows in the CSV file. The `get_row_count()` method.
@@ -94,52 +94,61 @@
 ### Appending the set of rows at the top of the file.
 The `append_rows()` method accepts an optional boolean argument called `append_on_top`. By default its set to `False`, which makes the method append the new rows **below** the existing rows. 
 
 If set to `True`, the `append_on_top` argument makes the method place the new rows **on top** of the file, just below the headers, moving down the existing rows.
 
 After the rows are appended, they will be seen in reverse order on the file. The last element on the `rows_object` will be on top at the file.
 ***
-### Getting the common rows between two instances of the CSVParser class. The `find_common_rows()` method.
-The `find_common_rows()` method compares the complete set of rows of two instances of the CSVParser class and returns a list containing the rows that are present on both instances. One CSVParser instance is the one the method is called on, the other one is passed as an argument.
+### Getting the common rows between two instances of the CSVWizard class. The `find_common_rows()` method.
+The `find_common_rows()` method compares the complete set of rows of two instances of the CSVWizard class and returns a list containing the rows that are present on both instances. One CSVWizard instance is the one the method is called on, the other one is passed as an argument.
 
 This method internally calls the `get_all_rows()` method, and it specifically asks fora `row_structure` of tuples. This is done for performance reasons. So the rows will be returned in the format `[('col1', 'col2')]`.
 ```
-file1 = CSVParser('fileNo1')
-file2 = CSVParser('fileNo2')
+file1 = CSVWizard('fileNo1')
+file2 = CSVWizard('fileNo2')
 file1.find_common_rows(file2)
 > [(row1"), ("row2), ("row3)] 
 ``` 
 
 ***
-### Finding the different rows between two instances of the CSVParser class. The `find_different_rows()` method.
-The `find_different_rows()` method compares the complete set of rows of two instances of the CSVParser class and returns a list containing only the rows that are present on the firts file but not on the second. One CSVParser instance is the one the method is called on, the other one is passed as an argument.
+### Finding the different rows between two instances of the CSVWizard class. The `find_different_rows()` method.
+The `find_different_rows()` method compares the complete set of rows of two instances of the CSVWizard class and returns a list containing only the rows that are present on the firts file but not on the second. One CSVWizard instance is the one the method is called on, the other one is passed as an argument.
 
-This method internally calls the `get_all_rows()` method, and it specifically asks fora `row_structure` of tuples. This is done for performance reasons. So the rows will be returned in the format `[('col1', 'col2')]`.
+This method internally calls the `get_all_rows()` method, and it specifically asks for a `row_structure` of tuples. This is done for performance reasons. So the rows will be returned in the format `[('col1', 'col2')]`.
 ```
-file1 = CSVParser('fileNo1')
-file2 = CSVParser('fileNo2')
+file1 = CSVWizard('fileNo1')
+file2 = CSVWizard('fileNo2')
 file1.find_different_rows(file2)
 > [(row5"), ("row8), (row14)] 
 ```
 ```
-file1 = CSVParser('fileNo1')
-file2 = CSVParser('fileNo2')
+file1 = CSVWizard('fileNo1')
+file2 = CSVWizard('fileNo2')
 file2.find_different_rows(file1)
 > [(row1"), ("row4), (row34)] 
 ``` 
 
 ***
 ### Finding duplicate rows in a file. The `get_duplicates()` method.
-When called on an instance of the CSVParser class, this method will return a dictionary with the following format: `{'row_name': number_of occurrences}`
+When called on an instance of the CSVWizard class, this method will return a dictionary with the following format: `{'row_name': number_of occurrences}`
 ```
-file1 = CSVParser('fileNo1')
+file1 = CSVWizard('fileNo1')
 file1.get_duplicates()
 > {"[' Alex ', 'alex@mail.com']": 2, "[' Adriana ', 'adriana@mail.com']": 5}
 ```
 ***
 ### In case there's empty rows in the file. The `delete_blanks()` method.
-Executing this method on a `CSVParser` instance will delete all blank rows from the CSV file. If there are many empty rows, the method may fail to delete them all in one run. If this happens, running it again should eventually delete them all.
+Executing this method on a `CSVWizard` instance will delete all blank rows from the CSV file. If there are many empty rows, the method may fail to delete them all in one run. If this happens, running it again should eventually delete them all.
 ***
 # Usage warnings
 1. When finding common rows or different rows between very large CSV files, keep in mind that execution time can be slower. To provide a frame of reference, while testing, comparing two files of a bit over 91000 rows, took between 1.7 and 2.1 seconds.
 2. When comparing files, if they contain special characters like spanish *tildes* (eg. á, í), if the files' encoding differs, and on of them recognizes this characters but the other one doesn't, they will be read as different characters, thus being recognized as different rows.
-3. When writing to an empty file (created manually or with the `create` method), an encoding must be specified.
+3. When writing to an empty file (created manually or with the `create` method), an encoding must be specified.
+
+***
+
+# Testing instructions
+The unit tests for this library is made with pytest. 
+
+Every time the tests run, a CSV file is created from the test_file_backup.csv. The tests will run on that copy file. Once they are finished, the copy file will stay there, until you review it and manually delete it.
+
+This is because some of the methods tested here make modifications on the test file that make it unusable for running tests again.
```

### Comparing `csv-wizard-0.4.2.post1/src/csv_wizard/csv_wizard.py` & `csv-wizard-1.0.0/src/csv_wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 
 CURRENT_DIR = os.path.realpath(".")
 CURRENT_PARENT_DIR = os.path.realpath("..")
 ABSOLUTE_PATH = os.path.abspath(".")
 
 
 @dataclass
-class CSVParser:
+class CSVWizard:
+    __slots__ = (
+        "source", 
+        "path"
+    )
+
     source: str
-    path: str = None
+    path: str
 
     def __post_init__(self) -> None:
         # concat the .csv extension so it is not necessary when instatiating
         if self.path:
             self.source = f"{os.path.join(self.path, self.source)}.csv"
         else:
             self.source = f"{self.source}.csv"
@@ -231,15 +236,15 @@
                 rows.insert(1, i)
             else:
                 rows.append(i)
         # overwrite the resulting list into the file
         self.overwrite(rows, encoding=encoding)
 
     def find_common_rows(
-        self, second_file: "CSVParser", encoding: str = ""
+        self, second_file: "CSVWizard", encoding: str = ""
     ) -> list[list[str]]:
         """
         Find the rows that are on both files
         """
         if not encoding:
             encoding = self.get_encoding()
         all_rows_1 = set(self.get_all_rows(encoding=encoding, row_structure="tuple"))
@@ -247,15 +252,15 @@
             second_file.get_all_rows(encoding=encoding, row_structure="tuple")
         )
         common_rows = list(all_rows_1.intersection(all_rows_2))
 
         return common_rows
 
     def find_different_rows(
-        self, second_file: "CSVParser", encoding: str = ""
+        self, second_file: "CSVWizard", encoding: str = ""
     ) -> list[list[str]]:
         """
         Returns the rows that are on the first file
         but not on the second one
         """
         if not encoding:
             encoding = self.get_encoding()
@@ -275,15 +280,15 @@
             encoding = self.get_encoding()
         rows = self.get_all_rows(encoding=encoding)
 
         dups_dict = {}
 
         for i in rows:
             # iterate over the file's rows
-            if rows.count(i) > 1:
+            if rows.count(i) > 1 and i != []:
                 # if the count for this element is > 1 is duplicated
                 # add that element and it's count to the dict
                 dups_dict.update({str(i): rows.count(i)})
 
         if len(dups_dict) > 0:
             return dups_dict
         else:
```

### Comparing `csv-wizard-0.4.2.post1/tests/test_divide.py` & `csv-wizard-1.0.0/tests/test_divide.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from pytest import raises
-
-from .test_misc import test_file
+import pytest
 
 # test divide()
 
 
-def test_divide_raises_error_for_float_argument():
-    with raises(TypeError):
+def test_divide_raises_error_for_float_argument(test_file):
+    with pytest.raises(TypeError):
         test_file.divide(4.5)
 
 
-def test_divide_raises_error_for_number_of_parts_greater_than_row_count():
-    with raises(IndexError):
+def test_divide_raises_error_for_number_of_parts_greater_than_row_count(test_file):
+    with pytest.raises(IndexError):
         test_file.divide(300)
 
 
-def test_divide_type_is_list():
+def test_divide_type_is_list(test_file):
     parts = test_file.divide(4)
     assert type(parts) == list
 
 
-def test_divide_elem_type_is_list():
+def test_divide_elem_type_is_list(test_file):
     parts = test_file.divide(4)
     for elem in parts:
         assert type(elem) == list
 
 
-def test_divide():
+def test_divide(test_file):
     parts = test_file.divide(3)
     for elem in parts:
-        assert len(elem) <= 124
+        assert len(elem) <= 4
```

### Comparing `csv-wizard-0.4.2.post1/tests/test_find_common_rows.py` & `csv-wizard-1.0.0/tests/test_find_common_rows.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from pytest import raises
-
-from .test_misc import test_file, test_file2
+import pytest
 
 # test find_common_rows()
 
 
-def test_find_common_rows_returns_list():
-    common = test_file.find_common_rows(test_file2, "utf-8")
+def test_find_common_rows_returns_list(test_file, test_file_diff):
+    common = test_file.find_common_rows(test_file_diff)
     assert type(common) == list
 
 
-def test_find_common_rows_is_same_when_files_reversed():
-    common0 = test_file.find_common_rows(test_file2, "utf-8")
-    common1 = test_file2.find_common_rows(test_file, "utf-8")
+def test_find_common_rows_is_same_when_files_reversed(test_file, test_file_diff):
+    common0 = test_file.find_common_rows(test_file_diff)
+    common1 = test_file_diff.find_common_rows(test_file)
     assert len(common0) == len(common1)
 
 
-def test_find_common_rows_incorrect_argument_type():
-    with raises(AttributeError):
-        test_file.find_common_rows(["dummy list"], "utf-8")
+def test_find_common_rows_incorrect_argument_type(test_file):
+    with pytest.raises(AttributeError):
+        test_file.find_common_rows(["dummy list"])
```

### Comparing `csv-wizard-0.4.2.post1/tests/test_get_all_rows.py` & `csv-wizard-1.0.0/tests/test_get_all_rows.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from .test_misc import test_file
-
+import pytest
 
 # test get_all_rows()
-def test_get_all_rows_type_is_list():
+
+
+def test_get_all_rows_type_is_list(test_file):
     result = test_file.get_all_rows()
     assert type(result) == list
 
 
-def test_get_all_rows_element_type_is_list():
+def test_get_all_rows_element_type_is_list(test_file):
     result = test_file.get_all_rows()
     for elem in result:
         assert type(elem) == list
 
 
-def test_get_all_rows_element_type_child_is_string():
+def test_get_all_rows_element_type_child_is_string(test_file):
     result = test_file.get_all_rows()
     for elem in result:
         for child in elem:
             assert type(child) == str
 
 
-def test_get_all_rows():
+def test_get_all_rows(test_file):
     all_rows = test_file.get_all_rows()
-    assert len(all_rows) == 248
+    assert len(all_rows) == 12
```

### Comparing `csv-wizard-0.4.2.post1/tests/test_get_dialect.py` & `csv-wizard-1.0.0/tests/test_get_dialect.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-from .test_misc import test_file
-
+import pytest
 
 # dialect tests
-def test_get_dialect_type_is_object():
+
+
+def test_get_dialect_type_is_object(test_file):
     dialect = test_file.get_dialect()
     assert type(dialect) == type
 
 
-def test_delimiter_type_is_string():
+def test_delimiter_type_is_string(test_file):
     delimiter = test_file.get_dialect().delimiter
     assert type(delimiter) == str
 
 
-def test_quoting_type_is_int():
+def test_quoting_type_is_int(test_file):
     quoting = test_file.get_dialect().quoting
     assert type(quoting) == int
 
 
-def test_doublequote_type_is_bool():
+def test_doublequote_type_is_bool(test_file):
     doublequote = test_file.get_dialect().doublequote
     assert type(doublequote) == bool
 
 
-def test_lineterminator_type_is_string():
+def test_lineterminator_type_is_string(test_file):
     lineterminator = test_file.get_dialect().lineterminator
     assert type(lineterminator) == str
 
 
-def test_quotechar_type_is_string():
+def test_quotechar_type_is_string(test_file):
     quotechar = test_file.get_dialect().quotechar
     assert type(quotechar) == str
 
 
-def test_skipinitialspace_type_is_bool():
+def test_skipinitialspace_type_is_bool(test_file):
     skipinitialspace = test_file.get_dialect().skipinitialspace
     assert type(skipinitialspace) == bool
```

### Comparing `csv-wizard-0.4.2.post1/tests/test_get_duplicates.py` & `csv-wizard-1.0.0/tests/test_get_duplicates.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from ..csv_parser import CSVParser
-
-test_file = CSVParser("everyone 248")
-test_file_no_dups = CSVParser("everyone 246")
+import pytest
 
 # test get_duplicates
 
 
-def test_get_duplicates_returns_dict():
-    dups = test_file.get_duplicates()
+def test_get_duplicates_returns_dict(test_file_with_dups):
+    dups = test_file_with_dups.get_duplicates()
     assert type(dups) == dict
 
 
-def test_get_duplicates_dict_values_are_int():
-    dups = test_file.get_duplicates()
+def test_get_duplicates_dict_values_are_int(test_file_with_dups):
+    dups = test_file_with_dups.get_duplicates()
     for k, v in dups.items():
         assert type(v) == int
 
 
-def test_get_duplicates_dict_keys_are_strings():
-    dups = test_file.get_duplicates()
+def test_get_duplicates_dict_keys_are_strings(test_file_with_dups):
+    dups = test_file_with_dups.get_duplicates()
     for k, v in dups.items():
         assert type(k) == str
 
 
-def test_get_duplicates_on_file_without_duplicates():
-    dups = test_file_no_dups.get_duplicates()
+def test_get_duplicates_on_file_without_duplicates(test_file):
+    dups = test_file.get_duplicates()
     assert dups == {"Result": "No duplicate rows in the file"}
 
 
-def test_get_duplicates():
-    dups = test_file.get_duplicates()
-    assert dups == {"[' ']": 3}
+def test_get_duplicates(test_file_with_dups):
+    dups = test_file_with_dups.get_duplicates()
+    assert dups == {
+        "['Bastian', 'bastian@yahoo.com']": 3,
+        "['Eva', 'eva@gmail.com']": 2,
+    }
```

### Comparing `csv-wizard-0.4.2.post1/PKG-INFO` & `csv-wizard-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: csv_wizard
-Version: 0.4.2.post1
+Version: 1.0.0
 Summary: Handy extension to Python csv standard library package
 License: MIT
 Author-email: liquidsnake <bentsoft365@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-# CSV Wizard
+# csv wizard
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 ***
-## Import a CSV file by only giving the `CSVParser` class a `string` containing the full name of the file without the *.csv* extension.
-> `new_file = CSVParser("my_file")`
+## Import a CSV file by only giving the `CSVWizard` class a `string` containing the full name of the file without the *.csv* extension.
+> `new_file = CSVWizard("my_file")`
 ***
 ## Handling decoding/encoding on a file.
 All methods have an optional `encoding` argument.
 If left empty, csv_wizard will attempt to automatically figure out the encoding, however, if a `UnicodeDecodeError` or `UnicodeEncodeError` error are raised, the encoding should be specified manually. 
 The encoding parameter accepts strings.
 ```
 > file1.get_row_count(encoding='utf-8') 
 ```
 ***
 ### Getting the characters that define the CSV file's layout. The `get_dialect` method.
-Calling this method on a CSVParser object returns it's dialect property.
+Calling this method on a CSVWizard object returns it's dialect property.
 The dialect property contains:
 * lineterminator
 * quoting
 * doublequote
 * delimiter
 * quotechar
 * skipinitialspace
@@ -50,15 +50,15 @@
 **Predefined paths**
 
 There are three predefined global variables you can use: 
 * `CURRENT_DIR` to get the current directory
 * `CURRENT_PARENT_DIR` to get the parent directory of the current location
 * `ABSOLUTE_PATH` to get the current absolute path
 
-> `CSVParser.create(name="new-file", path=CURRENT_PARENT_DIR)`
+> `CSVWizard.create(name="new-file", path=CURRENT_PARENT_DIR)`
 ***
 ### Getting the headers row. The `get_headers()` method.
 Returns only the first line on the CSV file, which is presumed to be the one containing the headers.
 > ``new_file.get_headers()`` # ["Name", "Email"]
 
 ***
 ### Getting the total number of rows in the CSV file. The `get_row_count()` method.
@@ -103,52 +103,61 @@
 ### Appending the set of rows at the top of the file.
 The `append_rows()` method accepts an optional boolean argument called `append_on_top`. By default its set to `False`, which makes the method append the new rows **below** the existing rows. 
 
 If set to `True`, the `append_on_top` argument makes the method place the new rows **on top** of the file, just below the headers, moving down the existing rows.
 
 After the rows are appended, they will be seen in reverse order on the file. The last element on the `rows_object` will be on top at the file.
 ***
-### Getting the common rows between two instances of the CSVParser class. The `find_common_rows()` method.
-The `find_common_rows()` method compares the complete set of rows of two instances of the CSVParser class and returns a list containing the rows that are present on both instances. One CSVParser instance is the one the method is called on, the other one is passed as an argument.
+### Getting the common rows between two instances of the CSVWizard class. The `find_common_rows()` method.
+The `find_common_rows()` method compares the complete set of rows of two instances of the CSVWizard class and returns a list containing the rows that are present on both instances. One CSVWizard instance is the one the method is called on, the other one is passed as an argument.
 
 This method internally calls the `get_all_rows()` method, and it specifically asks fora `row_structure` of tuples. This is done for performance reasons. So the rows will be returned in the format `[('col1', 'col2')]`.
 ```
-file1 = CSVParser('fileNo1')
-file2 = CSVParser('fileNo2')
+file1 = CSVWizard('fileNo1')
+file2 = CSVWizard('fileNo2')
 file1.find_common_rows(file2)
 > [(row1"), ("row2), ("row3)] 
 ``` 
 
 ***
-### Finding the different rows between two instances of the CSVParser class. The `find_different_rows()` method.
-The `find_different_rows()` method compares the complete set of rows of two instances of the CSVParser class and returns a list containing only the rows that are present on the firts file but not on the second. One CSVParser instance is the one the method is called on, the other one is passed as an argument.
+### Finding the different rows between two instances of the CSVWizard class. The `find_different_rows()` method.
+The `find_different_rows()` method compares the complete set of rows of two instances of the CSVWizard class and returns a list containing only the rows that are present on the firts file but not on the second. One CSVWizard instance is the one the method is called on, the other one is passed as an argument.
 
-This method internally calls the `get_all_rows()` method, and it specifically asks fora `row_structure` of tuples. This is done for performance reasons. So the rows will be returned in the format `[('col1', 'col2')]`.
+This method internally calls the `get_all_rows()` method, and it specifically asks for a `row_structure` of tuples. This is done for performance reasons. So the rows will be returned in the format `[('col1', 'col2')]`.
 ```
-file1 = CSVParser('fileNo1')
-file2 = CSVParser('fileNo2')
+file1 = CSVWizard('fileNo1')
+file2 = CSVWizard('fileNo2')
 file1.find_different_rows(file2)
 > [(row5"), ("row8), (row14)] 
 ```
 ```
-file1 = CSVParser('fileNo1')
-file2 = CSVParser('fileNo2')
+file1 = CSVWizard('fileNo1')
+file2 = CSVWizard('fileNo2')
 file2.find_different_rows(file1)
 > [(row1"), ("row4), (row34)] 
 ``` 
 
 ***
 ### Finding duplicate rows in a file. The `get_duplicates()` method.
-When called on an instance of the CSVParser class, this method will return a dictionary with the following format: `{'row_name': number_of occurrences}`
+When called on an instance of the CSVWizard class, this method will return a dictionary with the following format: `{'row_name': number_of occurrences}`
 ```
-file1 = CSVParser('fileNo1')
+file1 = CSVWizard('fileNo1')
 file1.get_duplicates()
 > {"[' Alex ', 'alex@mail.com']": 2, "[' Adriana ', 'adriana@mail.com']": 5}
 ```
 ***
 ### In case there's empty rows in the file. The `delete_blanks()` method.
-Executing this method on a `CSVParser` instance will delete all blank rows from the CSV file. If there are many empty rows, the method may fail to delete them all in one run. If this happens, running it again should eventually delete them all.
+Executing this method on a `CSVWizard` instance will delete all blank rows from the CSV file. If there are many empty rows, the method may fail to delete them all in one run. If this happens, running it again should eventually delete them all.
 ***
 # Usage warnings
 1. When finding common rows or different rows between very large CSV files, keep in mind that execution time can be slower. To provide a frame of reference, while testing, comparing two files of a bit over 91000 rows, took between 1.7 and 2.1 seconds.
 2. When comparing files, if they contain special characters like spanish *tildes* (eg. á, í), if the files' encoding differs, and on of them recognizes this characters but the other one doesn't, they will be read as different characters, thus being recognized as different rows.
 3. When writing to an empty file (created manually or with the `create` method), an encoding must be specified.
+
+***
+
+# Testing instructions
+The unit tests for this library is made with pytest. 
+
+Every time the tests run, a CSV file is created from the test_file_backup.csv. The tests will run on that copy file. Once they are finished, the copy file will stay there, until you review it and manually delete it.
+
+This is because some of the methods tested here make modifications on the test file that make it unusable for running tests again.
```

