# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.6.1.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.1.tar", last modified: Fri Jun 16 04:54:57 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.2.tar", last modified: Mon Jun 19 04:39:45 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1.tar` & `hyutils-hyutil-hoyun-lab-0.0.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 04:54:57.087312 hyutils-hyutil-hoyun-lab-0.0.6.1/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/LICENSE.txt
--rw-rw-rw-   0        0        0      600 2023-06-16 04:54:57.086813 hyutils-hyutil-hoyun-lab-0.0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 04:54:57.087312 hyutils-hyutil-hoyun-lab-0.0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-06-16 04:54:15.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 04:54:57.068184 hyutils-hyutil-hoyun-lab-0.0.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 04:54:57.081185 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      347 2023-06-16 04:54:05.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1144 2023-06-15 02:19:32.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/filejob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    13711 2023-06-09 05:56:06.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0     4046 2023-06-16 04:49:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 04:54:57.085184 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      600 2023-06-16 04:54:57.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-06-16 04:54:57.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 04:54:57.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-16 04:54:57.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 04:39:45.134768 hyutils-hyutil-hoyun-lab-0.0.6.2/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-06-19 04:39:45.134296 hyutils-hyutil-hoyun-lab-0.0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 04:39:45.135100 hyutils-hyutil-hoyun-lab-0.0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-06-19 04:39:18.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 04:39:45.111597 hyutils-hyutil-hoyun-lab-0.0.6.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 04:39:45.127597 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      347 2023-06-19 04:39:23.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1144 2023-06-15 02:19:32.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    14695 2023-06-19 04:38:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0     4046 2023-06-16 04:49:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-06-19 04:39:45.132598 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-06-19 04:39:45.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-06-19 04:39:45.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 04:39:45.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 04:39:45.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.6.1",
+    version="0.0.6.2",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,34 +42,45 @@
             xml_list.append(value)
     column_name = ['filename', 'width', 'height', 'class', 'xmin', 'ymin', 'xmax', 'ymax']
     xml_df = pd.DataFrame(xml_list, columns=column_name)
     classes_names = list(set(classes_names))
     classes_names.sort()
     return xml_df, classes_names
 
-
-def convert_to_csv(xml_path, include_string, output_file, labelmap_name):
+"""
+설명: 특정 경로와 확장자 정보(*.xml 등)를 입력받아서 입력된 경로의 모든 파일을 대상으로
+     coco xml 파일 형식을 가정하고 읽어서 특정 경로 위 폴더에 csv 파일을 생성하고, 
+     입력된 label map 파일명으로 입력되었던 특정 경로 바로 위 폴더에 라벨맵을 생성한다.
+     
+사용예:
+  python 5_xml_to_csv_in_divided_data.py 
+    --xml_path=D:\python_work\tf-train-data\faces\new_face_train_label 
+    --include_string=01*.xml 
+    --output_file=D:\python_work\tf-train-data\faces\new_face_train_label01.csv 
+    --labelmap_name=new_face_labelmap_01.pbtxt 
+"""
+def convert_to_csv(xml_path, include_string, output_file, labelmap_path):
 
     xml_df, classes_names = xml_to_dataframe(xml_path, include_string)
 
     # label map 생성
-    labelmap_dir = os.path.dirname(output_file)
-    label_map_path = os.path.join(labelmap_dir, labelmap_name)
-    print(f'label_map_path > {label_map_path}')
+    # labelmap_dir = os.path.dirname(output_file)
+    # label_map_path = os.path.join(labelmap_dir, labelmap_name)
+    print(f'label_map_path > {labelmap_path}')
     pbtxt_content = ""
 
     for i, class_name in enumerate(classes_names):
         pbtxt_content = (
                 pbtxt_content
                 + "item {{\n    id: {0}\n    name: '{1}'\n}}\n\n".format(i + 1, class_name)
         )
     pbtxt_content = pbtxt_content.strip()
-    with open(label_map_path, "w") as f:
+    with open(labelmap_path, "w") as f:
         f.write(pbtxt_content)
-        print(f'Successfully created {labelmap_name}')
+        print(f'Successfully created {labelmap_path}')
 
     # csv 파일 생성.
     output_path = os.path.dirname(output_file)
     if not os.path.exists(output_path):
         os.makedirs(output_path, exist_ok=True)
 
     xml_df.to_csv(output_file, index=None)
@@ -199,29 +210,35 @@
     image_path = os.path.join(image_path)
 
     class_dict = class_dict_from_pbtxt(pbtxt_path)
     writer = tf.compat.v1.python_io.TFRecordWriter(output_path)
 
     csv_list = csv_list.split(',')
     for csv_input in csv_list:
-        csv_target = os.path.join(csv_path, csv_path.strip())
+        csv_target = os.path.join(csv_path, csv_input.strip())
 
         examples = pd.read_csv(csv_target)
         grouped = __split(examples, 'filename')
 
         for group in tqdm(grouped, desc='groups'):
             tf_example = create_one_tf_example(group, image_path, class_dict)
             writer.write(tf_example.SerializeToString())
 
         print(f'{csv_input} was processed')
         writer.flush()
 
     writer.close()
     print('Successfully created the TFRecords: {}'.format(output_path))
 
+"""
+주석이 들어있는 폴더를 입력받아서 xml 파일들을 랜덤으로 섞어서, 훈련 주석 0.8, 테스트 주석 0.2 비율로 나눈후,
+test용 폴더에 test용 xml을, train 폴더에 train용 xml을 복사해준다.
+
+python divide_annotation.py -a .\ANNOTATION_PATH -t1 .\train -t2 .\test
+"""
 def divide_annotation(annotation_path, train_label, test_label):
     if not os.path.exists(annotation_path):
         print('Not Found: {}'.format(annotation_path))
         return
 
     if not os.path.exists(train_label):
         os.makedirs(train_label, exist_ok=True)
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt` & `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

