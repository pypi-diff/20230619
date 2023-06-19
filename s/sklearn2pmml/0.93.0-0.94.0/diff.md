# Comparing `tmp/sklearn2pmml-0.93.0.tar.gz` & `tmp/sklearn2pmml-0.94.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.93.0.tar", last modified: Tue Jun  6 07:43:51 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.94.0.tar", last modified: Mon Jun 19 19:22:25 2023, max compression
```

## Comparing `sklearn2pmml-0.93.0.tar` & `sklearn2pmml-0.94.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.93.0/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.93.0/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6244 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.29.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7312 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.29.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54279 2022-06-05 15:53:19.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pickle-1.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7978 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.29.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   432826 2023-05-01 06:26:58.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/guava-21.0.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   198275 2023-03-11 19:58:17.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-python-1.1.14.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-06-06 07:41:16.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    84309 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.29.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-05-01 06:26:58.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5704 2023-06-06 07:41:17.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    46363 2023-05-30 19:11:53.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-h2o-1.2.6.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34545 2023-05-30 08:51:06.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-statsmodels-1.0.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6333 2023-06-06 07:35:43.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.29.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   467741 2023-06-06 07:35:42.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-1.7.29.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.93.0/sklearn2pmml/resources/gson-2.10.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-06-06 07:40:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-06 07:43:51.000000 sklearn2pmml-0.93.0/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.93.0/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.0/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.0/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   202327 2023-06-11 10:10:38.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-python-1.1.15.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    33104 2023-06-11 15:37:09.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6331 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.30.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   432826 2023-05-01 06:26:58.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/guava-21.0.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7974 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.30.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    83162 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.30.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6242 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.30.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7310 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.30.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-06-19 19:18:50.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-05-01 06:26:58.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    46831 2023-06-15 18:20:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-h2o-1.2.7.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5703 2023-06-19 19:18:51.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   468727 2023-06-19 19:03:16.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-1.7.30.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pickle-1.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/gson-2.10.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-06-19 19:18:28.000000 sklearn2pmml-0.94.0/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.93.0/LICENSE.txt` & `sklearn2pmml-0.94.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/setup.py` & `sklearn2pmml-0.94.0/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/PKG-INFO` & `sklearn2pmml-0.94.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.93.0
+Version: 0.94.0
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.93.0.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.94.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/h2o.py` & `sklearn2pmml-0.94.0/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/tpot.py` & `sklearn2pmml-0.94.0/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/decoration/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.94.0/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.94.0/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.94.0/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.29.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.30.jar`

 * *Files 21% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 6244 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/statsmodels/
--rw-rw-r--  2.0 unx      152 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2083 b- defN 23-Jun-06 10:35 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Jun-06 10:35 sklearn2pmml/statsmodels/StatsModelsClassifier.class
--rw-rw-r--  2.0 unx     1920 b- defN 23-Jun-06 10:35 sklearn2pmml/statsmodels/StatsModelsUtil.class
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-06 10:35 sklearn2pmml/statsmodels/StatsModelsRegressor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
--rw-rw-r--  2.0 unx     1331 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
--rw-rw-r--  2.0 unx      120 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
-14 files, 8762 bytes uncompressed, 4122 bytes compressed:  53.0%
+Zip file size: 6242 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/statsmodels/
+-rw-rw-r--  2.0 unx      152 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Jun-19 22:03 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Jun-19 22:03 sklearn2pmml/statsmodels/StatsModelsClassifier.class
+-rw-rw-r--  2.0 unx     1920 b- defN 23-Jun-19 22:03 sklearn2pmml/statsmodels/StatsModelsUtil.class
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-19 22:03 sklearn2pmml/statsmodels/StatsModelsRegressor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
+-rw-rw-r--  2.0 unx     1331 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
+-rw-rw-r--  2.0 unx      120 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
+14 files, 8762 bytes uncompressed, 4120 bytes compressed:  53.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.29</version>
+    <version>1.7.30</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-statsmodels</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn StatsModels converter</name>
   <description>JPMML Scikit-Learn StatsModels to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Tue Jun 06 10:35:43 EEST 2023
-version=1.7.29
+#Mon Jun 19 22:03:17 EEST 2023
+version=1.7.30
 groupId=org.jpmml
 artifactId=pmml-sklearn-statsmodels
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.29.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.30.jar`

 * *Files 17% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7312 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 lightgbm/sklearn/
--rw-rw-r--  2.0 unx      177 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      170 b- defN 23-Jun-06 10:35 lightgbm/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     1953 b- defN 23-Jun-06 10:35 lightgbm/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-Jun-06 10:35 lightgbm/sklearn/LGBMRegressor.class
--rw-rw-r--  2.0 unx     2126 b- defN 23-Jun-06 10:35 lightgbm/sklearn/LGBMClassifier.class
--rw-rw-r--  2.0 unx     3298 b- defN 23-Jun-06 10:35 lightgbm/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
--rw-rw-r--  2.0 unx     1319 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
-15 files, 11392 bytes uncompressed, 5232 bytes compressed:  54.1%
+Zip file size: 7310 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 lightgbm/sklearn/
+-rw-rw-r--  2.0 unx      177 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      170 b- defN 23-Jun-19 22:03 lightgbm/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     1953 b- defN 23-Jun-19 22:03 lightgbm/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2102 b- defN 23-Jun-19 22:03 lightgbm/sklearn/LGBMRegressor.class
+-rw-rw-r--  2.0 unx     2126 b- defN 23-Jun-19 22:03 lightgbm/sklearn/LGBMClassifier.class
+-rw-rw-r--  2.0 unx     3298 b- defN 23-Jun-19 22:03 lightgbm/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
+-rw-rw-r--  2.0 unx     1319 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
+15 files, 11392 bytes uncompressed, 5230 bytes compressed:  54.1%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.29</version>
+    <version>1.7.30</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn LightGBM converter</name>
   <description>JPMML Scikit-Learn LightGBM to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Tue Jun 06 10:35:43 EEST 2023
-version=1.7.29
+#Mon Jun 19 22:03:17 EEST 2023
+version=1.7.30
 groupId=org.jpmml
 artifactId=pmml-sklearn-lightgbm
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pickle-1.3.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pickle-1.4.jar`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,41 +1,41 @@
-Zip file size: 54279 bytes, number of entries: 39
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-28 21:21 META-INF/
--rw-r--r--  2.0 unx      129 b- defN 22-Apr-28 21:21 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-28 21:21 net/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-28 21:21 net/razorvine/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-28 21:21 net/razorvine/pickle/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-28 21:21 net/razorvine/pickle/objects/
--rw-r--r--  2.0 unx      315 b- defN 22-Apr-28 21:21 net/razorvine/pickle/IObjectPickler.class
--rw-r--r--  2.0 unx      512 b- defN 22-Apr-28 21:21 net/razorvine/pickle/Pickler$Memo.class
--rw-r--r--  2.0 unx     2262 b- defN 22-Apr-28 21:21 net/razorvine/pickle/PythonException.class
--rw-r--r--  2.0 unx      655 b- defN 22-Apr-28 21:21 net/razorvine/pickle/InvalidOpcodeException.class
--rw-r--r--  2.0 unx      265 b- defN 22-Apr-28 21:21 net/razorvine/pickle/IObjectConstructor.class
--rw-r--r--  2.0 unx    21134 b- defN 22-Apr-28 21:21 net/razorvine/pickle/Unpickler.class
--rw-r--r--  2.0 unx     1980 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/AnyClassConstructor.class
--rw-r--r--  2.0 unx     1349 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$CalendarLocalizer.class
--rw-r--r--  2.0 unx     2727 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/ComplexNumber.class
--rw-r--r--  2.0 unx     2497 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/ExceptionConstructor.class
--rw-r--r--  2.0 unx     1285 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz.class
--rw-r--r--  2.0 unx     1550 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/Reconstructor.class
--rw-r--r--  2.0 unx     1327 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/ClassDictConstructor.class
--rw-r--r--  2.0 unx     8673 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/ArrayConstructor.class
--rw-r--r--  2.0 unx     1835 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/ClassDict.class
--rw-r--r--  2.0 unx     3685 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/TimeZoneConstructor.class
--rw-r--r--  2.0 unx     1966 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/TimeDelta.class
--rw-r--r--  2.0 unx     5930 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/DateTimeConstructor.class
--rw-r--r--  2.0 unx     1411 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$AttrGetterForTz.class
--rw-r--r--  2.0 unx      759 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/SetConstructor.class
--rw-r--r--  2.0 unx     1951 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/ByteArrayConstructor.class
--rw-r--r--  2.0 unx     1209 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/Tzinfo.class
--rw-r--r--  2.0 unx     1793 b- defN 22-Apr-28 21:21 net/razorvine/pickle/objects/Time.class
--rw-r--r--  2.0 unx     2339 b- defN 22-Apr-28 21:21 net/razorvine/pickle/Opcodes.class
--rw-r--r--  2.0 unx    17356 b- defN 22-Apr-28 21:21 net/razorvine/pickle/Pickler.class
--rw-r--r--  2.0 unx      624 b- defN 22-Apr-28 21:21 net/razorvine/pickle/PickleException.class
--rw-r--r--  2.0 unx     8302 b- defN 22-Apr-28 21:21 net/razorvine/pickle/PickleUtils.class
--rw-r--r--  2.0 unx     1837 b- defN 22-Apr-28 21:21 net/razorvine/pickle/UnpickleStack.class
-?rwsrwsrwt  2.0 unx        0 b- stor 22-Apr-28 21:21 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 22-Apr-28 21:21 META-INF/maven/net.razorvine/
-?rwsrwsrwt  2.0 unx        0 b- stor 22-Apr-28 21:21 META-INF/maven/net.razorvine/pickle/
--rw-r--r--  2.0 unx     2701 b- defN 22-Apr-28 21:21 META-INF/maven/net.razorvine/pickle/pom.xml
--rw-r--r--  2.0 unx      103 b- defN 22-Apr-28 21:21 META-INF/maven/net.razorvine/pickle/pom.properties
-39 files, 100461 bytes uncompressed, 48027 bytes compressed:  52.2%
+Zip file size: 54294 bytes, number of entries: 39
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 META-INF/
+-rw-r--r--  2.0 unx      129 b- defN 23-May-24 21:16 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 net/razorvine/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 net/razorvine/pickle/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-24 21:16 net/razorvine/pickle/objects/
+-rw-r--r--  2.0 unx      655 b- defN 23-May-24 21:16 net/razorvine/pickle/InvalidOpcodeException.class
+-rw-r--r--  2.0 unx     1837 b- defN 23-May-24 21:16 net/razorvine/pickle/UnpickleStack.class
+-rw-r--r--  2.0 unx      512 b- defN 23-May-24 21:16 net/razorvine/pickle/Pickler$Memo.class
+-rw-r--r--  2.0 unx    21134 b- defN 23-May-24 21:16 net/razorvine/pickle/Unpickler.class
+-rw-r--r--  2.0 unx     1209 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/Tzinfo.class
+-rw-r--r--  2.0 unx     3685 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/TimeZoneConstructor.class
+-rw-r--r--  2.0 unx     5930 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/DateTimeConstructor.class
+-rw-r--r--  2.0 unx     1411 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$AttrGetterForTz.class
+-rw-r--r--  2.0 unx     1835 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ClassDict.class
+-rw-r--r--  2.0 unx     1327 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ClassDictConstructor.class
+-rw-r--r--  2.0 unx     1550 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/Reconstructor.class
+-rw-r--r--  2.0 unx     1793 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/Time.class
+-rw-r--r--  2.0 unx      759 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/SetConstructor.class
+-rw-r--r--  2.0 unx     2497 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ExceptionConstructor.class
+-rw-r--r--  2.0 unx     1966 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ByteArrayConstructor.class
+-rw-r--r--  2.0 unx     1285 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz.class
+-rw-r--r--  2.0 unx     1349 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$CalendarLocalizer.class
+-rw-r--r--  2.0 unx     1980 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/AnyClassConstructor.class
+-rw-r--r--  2.0 unx     2727 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ComplexNumber.class
+-rw-r--r--  2.0 unx     1966 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/TimeDelta.class
+-rw-r--r--  2.0 unx     8673 b- defN 23-May-24 21:16 net/razorvine/pickle/objects/ArrayConstructor.class
+-rw-r--r--  2.0 unx      624 b- defN 23-May-24 21:16 net/razorvine/pickle/PickleException.class
+-rw-r--r--  2.0 unx     8302 b- defN 23-May-24 21:16 net/razorvine/pickle/PickleUtils.class
+-rw-r--r--  2.0 unx      265 b- defN 23-May-24 21:16 net/razorvine/pickle/IObjectConstructor.class
+-rw-r--r--  2.0 unx     2262 b- defN 23-May-24 21:16 net/razorvine/pickle/PythonException.class
+-rw-r--r--  2.0 unx     2339 b- defN 23-May-24 21:16 net/razorvine/pickle/Opcodes.class
+-rw-r--r--  2.0 unx      315 b- defN 23-May-24 21:16 net/razorvine/pickle/IObjectPickler.class
+-rw-r--r--  2.0 unx    17356 b- defN 23-May-24 21:16 net/razorvine/pickle/Pickler.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-24 21:16 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-24 21:16 META-INF/maven/net.razorvine/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-May-24 21:16 META-INF/maven/net.razorvine/pickle/
+-rw-r--r--  2.0 unx     2701 b- defN 23-May-24 21:16 META-INF/maven/net.razorvine/pickle/pom.xml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-24 21:16 META-INF/maven/net.razorvine/pickle/pom.properties
+39 files, 100476 bytes uncompressed, 48042 bytes compressed:  52.2%
```

#### zipnote «TEMP»/diffoscope_rvr563yz_/tmp1bf6yjsl_.zip

```diff
@@ -12,96 +12,96 @@
 
 Filename: net/razorvine/pickle/
 Comment: 
 
 Filename: net/razorvine/pickle/objects/
 Comment: 
 
-Filename: net/razorvine/pickle/IObjectPickler.class
+Filename: net/razorvine/pickle/InvalidOpcodeException.class
 Comment: 
 
-Filename: net/razorvine/pickle/Pickler$Memo.class
+Filename: net/razorvine/pickle/UnpickleStack.class
 Comment: 
 
-Filename: net/razorvine/pickle/PythonException.class
+Filename: net/razorvine/pickle/Pickler$Memo.class
 Comment: 
 
-Filename: net/razorvine/pickle/InvalidOpcodeException.class
+Filename: net/razorvine/pickle/Unpickler.class
 Comment: 
 
-Filename: net/razorvine/pickle/IObjectConstructor.class
+Filename: net/razorvine/pickle/objects/Tzinfo.class
 Comment: 
 
-Filename: net/razorvine/pickle/Unpickler.class
+Filename: net/razorvine/pickle/objects/TimeZoneConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/AnyClassConstructor.class
+Filename: net/razorvine/pickle/objects/DateTimeConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$CalendarLocalizer.class
+Filename: net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$AttrGetterForTz.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/ComplexNumber.class
+Filename: net/razorvine/pickle/objects/ClassDict.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/ExceptionConstructor.class
+Filename: net/razorvine/pickle/objects/ClassDictConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz.class
+Filename: net/razorvine/pickle/objects/Reconstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/Reconstructor.class
+Filename: net/razorvine/pickle/objects/Time.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/ClassDictConstructor.class
+Filename: net/razorvine/pickle/objects/SetConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/ArrayConstructor.class
+Filename: net/razorvine/pickle/objects/ExceptionConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/ClassDict.class
+Filename: net/razorvine/pickle/objects/ByteArrayConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/TimeZoneConstructor.class
+Filename: net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/TimeDelta.class
+Filename: net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$CalendarLocalizer.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/DateTimeConstructor.class
+Filename: net/razorvine/pickle/objects/AnyClassConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/OperatorAttrGetterForCalendarTz$AttrGetterForTz.class
+Filename: net/razorvine/pickle/objects/ComplexNumber.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/SetConstructor.class
+Filename: net/razorvine/pickle/objects/TimeDelta.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/ByteArrayConstructor.class
+Filename: net/razorvine/pickle/objects/ArrayConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/Tzinfo.class
+Filename: net/razorvine/pickle/PickleException.class
 Comment: 
 
-Filename: net/razorvine/pickle/objects/Time.class
+Filename: net/razorvine/pickle/PickleUtils.class
 Comment: 
 
-Filename: net/razorvine/pickle/Opcodes.class
+Filename: net/razorvine/pickle/IObjectConstructor.class
 Comment: 
 
-Filename: net/razorvine/pickle/Pickler.class
+Filename: net/razorvine/pickle/PythonException.class
 Comment: 
 
-Filename: net/razorvine/pickle/PickleException.class
+Filename: net/razorvine/pickle/Opcodes.class
 Comment: 
 
-Filename: net/razorvine/pickle/PickleUtils.class
+Filename: net/razorvine/pickle/IObjectPickler.class
 Comment: 
 
-Filename: net/razorvine/pickle/UnpickleStack.class
+Filename: net/razorvine/pickle/Pickler.class
 Comment: 
 
 Filename: META-INF/maven/
 Comment: 
 
 Filename: META-INF/maven/net.razorvine/
 Comment:
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Archiver-Version: Plexus Archiver
-Created-By: Apache Maven 3.8.4
+Created-By: Apache Maven 3.8.7
 Built-By: irmen
-Build-Jdk: 11.0.15
+Build-Jdk: 11.0.19
```

#### net/razorvine/pickle/objects/ByteArrayConstructor.class

##### procyon -ec {}

```diff
@@ -5,16 +5,19 @@
 import java.util.ArrayList;
 import net.razorvine.pickle.PickleException;
 import net.razorvine.pickle.IObjectConstructor;
 
 public class ByteArrayConstructor implements IObjectConstructor
 {
     public Object construct(final Object[] args) throws PickleException {
-        if (args.length != 1 && args.length != 2) {
-            throw new PickleException("invalid pickle data for bytearray; expected 1 or 2 args, got " + args.length);
+        if (args.length > 2) {
+            throw new PickleException("invalid pickle data for bytearray; expected 0, 1 or 2 args, got " + args.length);
+        }
+        if (args.length == 0) {
+            return new byte[0];
         }
         if (args.length == 1) {
             if (args[0] instanceof byte[]) {
                 return args[0];
             }
             final ArrayList<Number> values = (ArrayList)args[0];
             final byte[] data = new byte[values.size()];
```

#### META-INF/maven/net.razorvine/pickle/pom.xml

##### META-INF/maven/net.razorvine/pickle/pom.xml

```diff
@@ -4,15 +4,15 @@
   <parent>
     <groupId>org.sonatype.oss</groupId>
     <artifactId>oss-parent</artifactId>
     <version>9</version>
   </parent>
   <groupId>net.razorvine</groupId>
   <artifactId>pickle</artifactId>
-  <version>1.3</version>
+  <version>1.4</version>
   <packaging>jar</packaging>
   <name>pickle</name>
   <url>https://github.com/irmen/pickle</url>
   <properties>
     <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
   </properties>
   <build>
@@ -60,15 +60,15 @@
       <scope>test</scope>
     </dependency>
   </dependencies>
   <scm>
     <url>https://github.com/irmen/pickle</url>
     <connection>scm:git:ssh://git@github.com/irmen/pickle.git</connection>
     <developerConnection>scm:git:ssh://git@github.com/irmen/pickle.git</developerConnection>
-    <tag>pickle-1.3</tag>
+    <tag>pickle-1.4</tag>
   </scm>
   <issueManagement>
     <system>Github</system>
     <url>https://github.com/irmen/pickle/issues</url>
   </issueManagement>
   <developers>
     <developer>
```

#### META-INF/maven/net.razorvine/pickle/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Thu Apr 28 21:21:46 CEST 2022
+#Wed May 24 21:16:48 CEST 2023
 groupId=net.razorvine
 artifactId=pickle
-version=1.3
+version=1.4
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.29.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.30.jar`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7978 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 xgboost/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 xgboost/sklearn/
--rw-rw-r--  2.0 unx      364 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      168 b- defN 23-Jun-06 10:35 xgboost/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2270 b- defN 23-Jun-06 10:35 xgboost/sklearn/XGBClassifier.class
--rw-rw-r--  2.0 unx     2210 b- defN 23-Jun-06 10:35 xgboost/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2246 b- defN 23-Jun-06 10:35 xgboost/sklearn/XGBRegressor.class
--rw-rw-r--  2.0 unx     4204 b- defN 23-Jun-06 10:35 xgboost/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
--rw-rw-r--  2.0 unx     1453 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
--rw-rw-r--  2.0 unx      116 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
-15 files, 13161 bytes uncompressed, 5922 bytes compressed:  55.0%
+Zip file size: 7974 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 xgboost/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 xgboost/sklearn/
+-rw-rw-r--  2.0 unx      364 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      168 b- defN 23-Jun-19 22:03 xgboost/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2270 b- defN 23-Jun-19 22:03 xgboost/sklearn/XGBClassifier.class
+-rw-rw-r--  2.0 unx     2210 b- defN 23-Jun-19 22:03 xgboost/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2246 b- defN 23-Jun-19 22:03 xgboost/sklearn/XGBRegressor.class
+-rw-rw-r--  2.0 unx     4204 b- defN 23-Jun-19 22:03 xgboost/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
+15 files, 13161 bytes uncompressed, 5918 bytes compressed:  55.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.29</version>
+    <version>1.7.30</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-xgboost</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn XGBoost converter</name>
   <description>JPMML Scikit-Learn XGBoost to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Tue Jun 06 10:35:43 EEST 2023
-version=1.7.29
+#Mon Jun 19 22:03:17 EEST 2023
+version=1.7.30
 groupId=org.jpmml
 artifactId=pmml-sklearn-xgboost
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/guava-21.0.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/guava-21.0.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-python-1.1.14.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-python-1.1.15.jar`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,169 +1,174 @@
-Zip file size: 198275 bytes, number of entries: 167
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Mar-11 21:58 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 patsy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 functools/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 treelib/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 pandas/core/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 numpy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 numpy/random/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 numpy/core/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 collections/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 org/jpmml/python/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 joblib/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 scipy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 scipy/interpolate/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 scipy/sparse/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 builtins/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-11 21:58 META-INF/maven/org.jpmml/pmml-python/
--rw-rw-r--  2.0 unx     2108 b- defN 23-Mar-11 21:58 patsy/PatsyOperation.class
--rw-rw-r--  2.0 unx     2272 b- defN 23-Mar-11 21:58 patsy/PatsyOperator.class
--rw-rw-r--  2.0 unx     3106 b- defN 23-Mar-11 21:58 patsy/PatsyToken.class
--rw-rw-r--  2.0 unx      933 b- defN 23-Mar-11 21:58 patsy/PatsyFactor.class
--rw-rw-r--  2.0 unx      747 b- defN 23-Mar-11 21:58 patsy/PatsyTerm.class
--rw-rw-r--  2.0 unx     8491 b- defN 23-Mar-11 21:58 patsy/FormulaParser.class
--rw-rw-r--  2.0 unx     2807 b- defN 23-Mar-11 21:58 META-INF/python2pmml.properties
--rw-rw-r--  2.0 unx     3265 b- defN 23-Mar-11 21:58 functools/Partial.class
--rw-rw-r--  2.0 unx     2675 b- defN 23-Mar-11 21:58 treelib/Node.class
--rw-rw-r--  2.0 unx     2537 b- defN 23-Mar-11 21:58 treelib/Tree.class
--rw-rw-r--  2.0 unx     1800 b- defN 23-Mar-11 21:58 pandas/NDArrayBackedConstructor.class
--rw-rw-r--  2.0 unx     2394 b- defN 23-Mar-11 21:58 pandas/NDArrayBacked.class
--rw-rw-r--  2.0 unx     1117 b- defN 23-Mar-11 21:58 pandas/core/Index$NDArrayData.class
--rw-rw-r--  2.0 unx     3052 b- defN 23-Mar-11 21:58 pandas/core/Index.class
--rw-rw-r--  2.0 unx     3953 b- defN 23-Mar-11 21:58 pandas/core/BlockManager.class
--rw-rw-r--  2.0 unx     1602 b- defN 23-Mar-11 21:58 pandas/core/SingleBlockManager.class
--rw-rw-r--  2.0 unx      724 b- defN 23-Mar-11 21:58 pandas/core/DataFrame.class
--rw-rw-r--  2.0 unx     2419 b- defN 23-Mar-11 21:58 pandas/core/MaskedArray.class
--rw-rw-r--  2.0 unx      565 b- defN 23-Mar-11 21:58 pandas/core/StringDtype.class
--rw-rw-r--  2.0 unx     2455 b- defN 23-Mar-11 21:58 pandas/core/SeriesUtil.class
--rw-rw-r--  2.0 unx     2092 b- defN 23-Mar-11 21:58 pandas/core/Series.class
--rw-rw-r--  2.0 unx     1382 b- defN 23-Mar-11 21:58 pandas/core/Index$RangeData.class
--rw-rw-r--  2.0 unx     1397 b- defN 23-Mar-11 21:58 pandas/core/CategoricalDtype.class
--rw-rw-r--  2.0 unx      385 b- defN 23-Mar-11 21:58 pandas/core/StringArray.class
--rw-rw-r--  2.0 unx      569 b- defN 23-Mar-11 21:58 pandas/core/IntegerDtype.class
--rw-rw-r--  2.0 unx      703 b- defN 23-Mar-11 21:58 pandas/core/Index$Data.class
--rw-rw-r--  2.0 unx      569 b- defN 23-Mar-11 21:58 pandas/core/BooleanDtype.class
--rw-rw-r--  2.0 unx      713 b- defN 23-Mar-11 21:58 pandas/core/Categorical.class
--rw-rw-r--  2.0 unx     1122 b- defN 23-Mar-11 21:58 pandas/core/MaskedArray$1.class
--rw-rw-r--  2.0 unx      453 b- defN 23-Mar-11 21:58 pandas/core/ExtensionDtype.class
--rw-rw-r--  2.0 unx     1354 b- defN 23-Mar-11 21:58 pandas/core/Block.class
--rw-rw-r--  2.0 unx     1172 b- defN 23-Mar-11 21:58 numpy/DTypeUtil.class
--rw-rw-r--  2.0 unx     1392 b- defN 23-Mar-11 21:58 numpy/random/BitGeneratorUtil.class
--rw-rw-r--  2.0 unx     1052 b- defN 23-Mar-11 21:58 numpy/random/Generator.class
--rw-rw-r--  2.0 unx      853 b- defN 23-Mar-11 21:58 numpy/random/BitGenerator.class
--rw-rw-r--  2.0 unx      917 b- defN 23-Mar-11 21:58 numpy/random/RandomState.class
--rw-rw-r--  2.0 unx     1065 b- defN 23-Mar-11 21:58 numpy/random/LegacyRandomState.class
--rw-rw-r--  2.0 unx     4407 b- defN 23-Mar-11 21:58 numpy/DType.class
--rw-rw-r--  2.0 unx     2006 b- defN 23-Mar-11 21:58 numpy/core/TypeDescriptor$Kind.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-Mar-11 21:58 numpy/core/MaskedArray.class
--rw-rw-r--  2.0 unx     1100 b- defN 23-Mar-11 21:58 numpy/core/UFunc.class
--rw-rw-r--  2.0 unx    12387 b- defN 23-Mar-11 21:58 numpy/core/NDArrayUtil.class
--rw-rw-r--  2.0 unx      641 b- defN 23-Mar-11 21:58 numpy/core/Function.class
--rw-rw-r--  2.0 unx     2386 b- defN 23-Mar-11 21:58 numpy/core/FromBufferConstructor.class
--rw-rw-r--  2.0 unx     1015 b- defN 23-Mar-11 21:58 numpy/core/TypeDescriptor$1.class
--rw-rw-r--  2.0 unx     4213 b- defN 23-Mar-11 21:58 numpy/core/NDArray.class
--rw-rw-r--  2.0 unx     5185 b- defN 23-Mar-11 21:58 numpy/core/TypeDescriptor.class
--rw-rw-r--  2.0 unx     3638 b- defN 23-Mar-11 21:58 numpy/core/Scalar.class
--rw-rw-r--  2.0 unx      586 b- defN 23-Mar-11 21:58 numpy/core/ScalarUtil.class
--rw-rw-r--  2.0 unx      109 b- defN 23-Mar-11 21:58 collections/Callable.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Mar-11 21:58 collections/DefaultDict.class
--rw-rw-r--  2.0 unx     1467 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonObject$5.class
--rw-rw-r--  2.0 unx     1256 b- defN 23-Mar-11 21:58 org/jpmml/python/Token.class
--rw-rw-r--  2.0 unx     2927 b- defN 23-Mar-11 21:58 org/jpmml/python/TokenMgrException.class
--rw-rw-r--  2.0 unx     2230 b- defN 23-Mar-11 21:58 org/jpmml/python/TupleUtil.class
--rw-rw-r--  2.0 unx     2734 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonParserConstants.class
--rw-rw-r--  2.0 unx      472 b- defN 23-Mar-11 21:58 org/jpmml/python/Storage.class
--rw-rw-r--  2.0 unx     1689 b- defN 23-Mar-11 21:58 org/jpmml/python/CustomUnpickler.class
--rw-rw-r--  2.0 unx      497 b- defN 23-Mar-11 21:58 org/jpmml/python/FunctionDefParser$JJCalls.class
--rw-rw-r--  2.0 unx      914 b- defN 23-Mar-11 21:58 org/jpmml/python/CompressedInputStreamStorage$Type$2.class
--rw-rw-r--  2.0 unx     1381 b- defN 23-Mar-11 21:58 org/jpmml/python/CompressedInputStreamStorage$1.class
--rw-rw-r--  2.0 unx      242 b- defN 23-Mar-11 21:58 org/jpmml/python/ExpressionTranslator$1.class
--rw-rw-r--  2.0 unx     4157 b- defN 23-Mar-11 21:58 org/jpmml/python/ParseException.class
--rw-rw-r--  2.0 unx      282 b- defN 23-Mar-11 21:58 org/jpmml/python/HasArray.class
--rw-rw-r--  2.0 unx     3481 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonParserUtil.class
--rw-rw-r--  2.0 unx     2631 b- defN 23-Mar-11 21:58 org/jpmml/python/FunctionDefScope.class
--rw-rw-r--  2.0 unx      784 b- defN 23-Mar-11 21:58 org/jpmml/python/ExpressionTranslator$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     2861 b- defN 23-Mar-11 21:58 org/jpmml/python/CompressedInputStreamStorage.class
--rw-rw-r--  2.0 unx      777 b- defN 23-Mar-11 21:58 org/jpmml/python/PredicateTranslator$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     1016 b- defN 23-Mar-11 21:58 org/jpmml/python/CastUtil.class
--rw-rw-r--  2.0 unx      164 b- defN 23-Mar-11 21:58 org/jpmml/python/TypeInfo.class
--rw-rw-r--  2.0 unx     5550 b- defN 23-Mar-11 21:58 org/jpmml/python/ClassDictUtil.class
--rw-rw-r--  2.0 unx    39493 b- defN 23-Mar-11 21:58 org/jpmml/python/ExpressionTranslator.class
--rw-rw-r--  2.0 unx     1294 b- defN 23-Mar-11 21:58 org/jpmml/python/StreamProvider.class
--rw-rw-r--  2.0 unx     1340 b- defN 23-Mar-11 21:58 org/jpmml/python/PickleUtil$1.class
--rw-rw-r--  2.0 unx     6658 b- defN 23-Mar-11 21:58 org/jpmml/python/SimpleCharStream.class
--rw-rw-r--  2.0 unx     9499 b- defN 23-Mar-11 21:58 org/jpmml/python/FunctionDefParser.class
--rw-rw-r--  2.0 unx     1139 b- defN 23-Mar-11 21:58 org/jpmml/python/InputStreamStorage.class
--rw-rw-r--  2.0 unx      986 b- defN 23-Mar-11 21:58 org/jpmml/python/ExpressionTranslator$Block.class
--rw-rw-r--  2.0 unx      914 b- defN 23-Mar-11 21:58 org/jpmml/python/CompressedInputStreamStorage$Type$1.class
--rw-rw-r--  2.0 unx     4624 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonParser.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Mar-11 21:58 org/jpmml/python/NamedTuple.class
--rw-rw-r--  2.0 unx     1303 b- defN 23-Mar-11 21:58 org/jpmml/python/ClassDictUtil$1.class
--rw-rw-r--  2.0 unx      805 b- defN 23-Mar-11 21:58 org/jpmml/python/NullConstructor.class
--rw-rw-r--  2.0 unx     1120 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonTypeUtil.class
--rw-rw-r--  2.0 unx     1145 b- defN 23-Mar-11 21:58 org/jpmml/python/FileStorage.class
--rw-rw-r--  2.0 unx     1117 b- defN 23-Mar-11 21:58 org/jpmml/python/StringProvider.class
--rw-rw-r--  2.0 unx     1299 b- defN 23-Mar-11 21:58 org/jpmml/python/PushbackPythonParserTokenManager.class
--rw-rw-r--  2.0 unx     9731 b- defN 23-Mar-11 21:58 org/jpmml/python/AbstractTranslator.class
--rw-rw-r--  2.0 unx     8808 b- defN 23-Mar-11 21:58 org/jpmml/python/PickleUtil.class
--rw-rw-r--  2.0 unx     2017 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonEnumConstructor.class
--rw-rw-r--  2.0 unx     4475 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonObjectConstructor.class
--rw-rw-r--  2.0 unx      800 b- defN 23-Mar-11 21:58 org/jpmml/python/FunctionDef$Parameter.class
--rw-rw-r--  2.0 unx      183 b- defN 23-Mar-11 21:58 org/jpmml/python/Identifiable.class
--rw-rw-r--  2.0 unx     2647 b- defN 23-Mar-11 21:58 org/jpmml/python/ClassDictConstructorUtil.class
--rw-rw-r--  2.0 unx    10443 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonObject.class
--rw-rw-r--  2.0 unx     1442 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonObject$1.class
--rw-rw-r--  2.0 unx     8569 b- defN 23-Mar-11 21:58 org/jpmml/python/FunctionUtil.class
--rw-rw-r--  2.0 unx     1456 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonObject$3.class
--rw-rw-r--  2.0 unx      743 b- defN 23-Mar-11 21:58 org/jpmml/python/PredicateTranslator$1.class
--rw-rw-r--  2.0 unx      434 b- defN 23-Mar-11 21:58 org/jpmml/python/IConstantConstructor.class
--rw-rw-r--  2.0 unx     1338 b- defN 23-Mar-11 21:58 org/jpmml/python/FunctionDef.class
--rw-rw-r--  2.0 unx      270 b- defN 23-Mar-11 21:58 org/jpmml/python/HasContent.class
--rw-rw-r--  2.0 unx      763 b- defN 23-Mar-11 21:58 org/jpmml/python/FunctionDefParser$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     1545 b- defN 23-Mar-11 21:58 org/jpmml/python/CustomPythonObjectConstructor.class
--rw-rw-r--  2.0 unx     1784 b- defN 23-Mar-11 21:58 org/jpmml/python/CompressedInputStreamStorage$Type.class
--rw-rw-r--  2.0 unx      233 b- defN 23-Mar-11 21:58 org/jpmml/python/FunctionDefParser$1.class
--rw-rw-r--  2.0 unx      534 b- defN 23-Mar-11 21:58 org/jpmml/python/NullProvider.class
--rw-rw-r--  2.0 unx      219 b- defN 23-Mar-11 21:58 org/jpmml/python/Provider.class
--rw-rw-r--  2.0 unx      566 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonEnum.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Mar-11 21:58 org/jpmml/python/PredicateTranslator$JJCalls.class
--rw-rw-r--  2.0 unx     1201 b- defN 23-Mar-11 21:58 org/jpmml/python/CalendarUtil.class
--rw-rw-r--  2.0 unx     1793 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonObject$2.class
--rw-rw-r--  2.0 unx     2786 b- defN 23-Mar-11 21:58 org/jpmml/python/SliceUtil.class
--rw-rw-r--  2.0 unx      234 b- defN 23-Mar-11 21:58 org/jpmml/python/Castable.class
--rw-rw-r--  2.0 unx     1107 b- defN 23-Mar-11 21:58 org/jpmml/python/TupleUtil$1.class
--rw-rw-r--  2.0 unx     1512 b- defN 23-Mar-11 21:58 org/jpmml/python/AbstractTranslator$1.class
--rw-rw-r--  2.0 unx     1795 b- defN 23-Mar-11 21:58 org/jpmml/python/CastFunction.class
--rw-rw-r--  2.0 unx     1106 b- defN 23-Mar-11 21:58 org/jpmml/python/TupleUtil$3.class
--rw-rw-r--  2.0 unx     1873 b- defN 23-Mar-11 21:58 org/jpmml/python/NamedTupleConstructor.class
--rw-rw-r--  2.0 unx      509 b- defN 23-Mar-11 21:58 org/jpmml/python/ExpressionTranslator$JJCalls.class
--rw-rw-r--  2.0 unx      875 b- defN 23-Mar-11 21:58 org/jpmml/python/SliceUtil$1.class
--rw-rw-r--  2.0 unx     2975 b- defN 23-Mar-11 21:58 org/jpmml/python/BlockScope.class
--rw-rw-r--  2.0 unx     5585 b- defN 23-Mar-11 21:58 org/jpmml/python/DataFrameScope.class
--rw-rw-r--  2.0 unx      643 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonEncoder.class
--rw-rw-r--  2.0 unx     1454 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonObject$4.class
--rw-rw-r--  2.0 unx     1729 b- defN 23-Mar-11 21:58 org/jpmml/python/Scope.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Mar-11 21:58 org/jpmml/python/TupleUtil$2.class
--rw-rw-r--  2.0 unx    15414 b- defN 23-Mar-11 21:58 org/jpmml/python/PythonParserTokenManager.class
--rw-rw-r--  2.0 unx     2872 b- defN 23-Mar-11 21:58 org/jpmml/python/CustomPythonObject.class
--rw-rw-r--  2.0 unx    23578 b- defN 23-Mar-11 21:58 org/jpmml/python/PredicateTranslator.class
--rw-rw-r--  2.0 unx     1629 b- defN 23-Mar-11 21:58 org/jpmml/python/StorageUtil.class
--rw-rw-r--  2.0 unx     1128 b- defN 23-Mar-11 21:58 joblib/NDArrayWrapperConstructor$1.class
--rw-rw-r--  2.0 unx     1371 b- defN 23-Mar-11 21:58 joblib/NDArrayWrapperConstructor.class
--rw-rw-r--  2.0 unx     2667 b- defN 23-Mar-11 21:58 joblib/NumpyArrayWrapper.class
--rw-rw-r--  2.0 unx     2493 b- defN 23-Mar-11 21:58 joblib/NDArrayWrapper.class
--rw-rw-r--  2.0 unx     1056 b- defN 23-Mar-11 21:58 scipy/interpolate/BSpline.class
--rw-rw-r--  2.0 unx     1541 b- defN 23-Mar-11 21:58 scipy/sparse/CSRMatrix.class
--rw-rw-r--  2.0 unx     2618 b- defN 23-Mar-11 21:58 scipy/sparse/CSRMatrixUtil.class
--rw-rw-r--  2.0 unx     2086 b- defN 23-Mar-11 21:58 builtins/Type.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Mar-11 21:58 builtins/GetAttr.class
--rw-rw-r--  2.0 unx      536 b- defN 23-Mar-11 21:58 builtins/TypeConstructor.class
--rw-rw-r--  2.0 unx      855 b- defN 23-Mar-11 21:58 builtins/Slice.class
--rw-rw-r--  2.0 unx     5156 b- defN 23-Mar-11 21:57 META-INF/maven/org.jpmml/pmml-python/pom.xml
--rw-rw-r--  2.0 unx       56 b- defN 23-Mar-11 21:58 META-INF/maven/org.jpmml/pmml-python/pom.properties
-167 files, 371496 bytes uncompressed, 174863 bytes compressed:  52.9%
+Zip file size: 202327 bytes, number of entries: 172
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-11 13:10 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 patsy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 functools/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 treelib/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 pandas/core/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 numpy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 numpy/random/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 numpy/core/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 collections/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 org/jpmml/python/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 joblib/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 scipy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 scipy/stats/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 scipy/interpolate/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 scipy/sparse/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 builtins/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 META-INF/maven/org.jpmml/pmml-python/
+-rw-rw-r--  2.0 unx     2108 b- defN 23-Jun-11 13:10 patsy/PatsyOperation.class
+-rw-rw-r--  2.0 unx     2272 b- defN 23-Jun-11 13:10 patsy/PatsyOperator.class
+-rw-rw-r--  2.0 unx     3106 b- defN 23-Jun-11 13:10 patsy/PatsyToken.class
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-11 13:10 patsy/PatsyFactor.class
+-rw-rw-r--  2.0 unx      747 b- defN 23-Jun-11 13:10 patsy/PatsyTerm.class
+-rw-rw-r--  2.0 unx     8491 b- defN 23-Jun-11 13:10 patsy/FormulaParser.class
+-rw-rw-r--  2.0 unx     3114 b- defN 23-Jun-11 13:10 META-INF/python2pmml.properties
+-rw-rw-r--  2.0 unx     3265 b- defN 23-Jun-11 13:10 functools/Partial.class
+-rw-rw-r--  2.0 unx     2675 b- defN 23-Jun-11 13:10 treelib/Node.class
+-rw-rw-r--  2.0 unx     2537 b- defN 23-Jun-11 13:10 treelib/Tree.class
+-rw-rw-r--  2.0 unx     1800 b- defN 23-Jun-11 13:10 pandas/NDArrayBackedConstructor.class
+-rw-rw-r--  2.0 unx     2394 b- defN 23-Jun-11 13:10 pandas/NDArrayBacked.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Jun-11 13:10 pandas/core/Index$NDArrayData.class
+-rw-rw-r--  2.0 unx     3052 b- defN 23-Jun-11 13:10 pandas/core/Index.class
+-rw-rw-r--  2.0 unx     4416 b- defN 23-Jun-11 13:10 pandas/core/BlockManager.class
+-rw-rw-r--  2.0 unx     1602 b- defN 23-Jun-11 13:10 pandas/core/SingleBlockManager.class
+-rw-rw-r--  2.0 unx      724 b- defN 23-Jun-11 13:10 pandas/core/DataFrame.class
+-rw-rw-r--  2.0 unx     2419 b- defN 23-Jun-11 13:10 pandas/core/MaskedArray.class
+-rw-rw-r--  2.0 unx      565 b- defN 23-Jun-11 13:10 pandas/core/StringDtype.class
+-rw-rw-r--  2.0 unx     3212 b- defN 23-Jun-11 13:10 pandas/core/SeriesUtil.class
+-rw-rw-r--  2.0 unx     2092 b- defN 23-Jun-11 13:10 pandas/core/Series.class
+-rw-rw-r--  2.0 unx     1382 b- defN 23-Jun-11 13:10 pandas/core/Index$RangeData.class
+-rw-rw-r--  2.0 unx     1397 b- defN 23-Jun-11 13:10 pandas/core/CategoricalDtype.class
+-rw-rw-r--  2.0 unx      385 b- defN 23-Jun-11 13:10 pandas/core/StringArray.class
+-rw-rw-r--  2.0 unx      569 b- defN 23-Jun-11 13:10 pandas/core/IntegerDtype.class
+-rw-rw-r--  2.0 unx      703 b- defN 23-Jun-11 13:10 pandas/core/Index$Data.class
+-rw-rw-r--  2.0 unx      569 b- defN 23-Jun-11 13:10 pandas/core/BooleanDtype.class
+-rw-rw-r--  2.0 unx      713 b- defN 23-Jun-11 13:10 pandas/core/Categorical.class
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jun-11 13:10 pandas/core/SeriesUtil$1.class
+-rw-rw-r--  2.0 unx     1122 b- defN 23-Jun-11 13:10 pandas/core/MaskedArray$1.class
+-rw-rw-r--  2.0 unx      453 b- defN 23-Jun-11 13:10 pandas/core/ExtensionDtype.class
+-rw-rw-r--  2.0 unx     1354 b- defN 23-Jun-11 13:10 pandas/core/Block.class
+-rw-rw-r--  2.0 unx     1172 b- defN 23-Jun-11 13:10 numpy/DTypeUtil.class
+-rw-rw-r--  2.0 unx     1404 b- defN 23-Jun-11 13:10 numpy/random/BitGeneratorUtil.class
+-rw-rw-r--  2.0 unx     1064 b- defN 23-Jun-11 13:10 numpy/random/Generator.class
+-rw-rw-r--  2.0 unx      853 b- defN 23-Jun-11 13:10 numpy/random/BitGenerator.class
+-rw-rw-r--  2.0 unx      917 b- defN 23-Jun-11 13:10 numpy/random/RandomState.class
+-rw-rw-r--  2.0 unx     1077 b- defN 23-Jun-11 13:10 numpy/random/LegacyRandomState.class
+-rw-rw-r--  2.0 unx     4557 b- defN 23-Jun-11 13:10 numpy/DType.class
+-rw-rw-r--  2.0 unx     2147 b- defN 23-Jun-11 13:10 numpy/core/TypeDescriptor$Kind.class
+-rw-rw-r--  2.0 unx     2102 b- defN 23-Jun-11 13:10 numpy/core/MaskedArray.class
+-rw-rw-r--  2.0 unx     1100 b- defN 23-Jun-11 13:10 numpy/core/UFunc.class
+-rw-rw-r--  2.0 unx    12387 b- defN 23-Jun-11 13:10 numpy/core/NDArrayUtil.class
+-rw-rw-r--  2.0 unx      641 b- defN 23-Jun-11 13:10 numpy/core/Function.class
+-rw-rw-r--  2.0 unx     2386 b- defN 23-Jun-11 13:10 numpy/core/FromBufferConstructor.class
+-rw-rw-r--  2.0 unx     1065 b- defN 23-Jun-11 13:10 numpy/core/TypeDescriptor$1.class
+-rw-rw-r--  2.0 unx     4213 b- defN 23-Jun-11 13:10 numpy/core/NDArray.class
+-rw-rw-r--  2.0 unx     5262 b- defN 23-Jun-11 13:10 numpy/core/TypeDescriptor.class
+-rw-rw-r--  2.0 unx     3638 b- defN 23-Jun-11 13:10 numpy/core/Scalar.class
+-rw-rw-r--  2.0 unx      586 b- defN 23-Jun-11 13:10 numpy/core/ScalarUtil.class
+-rw-rw-r--  2.0 unx      109 b- defN 23-Jun-11 13:10 collections/Callable.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jun-11 13:10 collections/DefaultDict.class
+-rw-rw-r--  2.0 unx     1467 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$5.class
+-rw-rw-r--  2.0 unx     1256 b- defN 23-Jun-11 13:10 org/jpmml/python/Token.class
+-rw-rw-r--  2.0 unx     2927 b- defN 23-Jun-11 13:10 org/jpmml/python/TokenMgrException.class
+-rw-rw-r--  2.0 unx     2230 b- defN 23-Jun-11 13:10 org/jpmml/python/TupleUtil.class
+-rw-rw-r--  2.0 unx     2734 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonParserConstants.class
+-rw-rw-r--  2.0 unx      472 b- defN 23-Jun-11 13:10 org/jpmml/python/Storage.class
+-rw-rw-r--  2.0 unx     1689 b- defN 23-Jun-11 13:10 org/jpmml/python/CustomUnpickler.class
+-rw-rw-r--  2.0 unx      497 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefParser$JJCalls.class
+-rw-rw-r--  2.0 unx      914 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage$Type$2.class
+-rw-rw-r--  2.0 unx     1381 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage$1.class
+-rw-rw-r--  2.0 unx      242 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator$1.class
+-rw-rw-r--  2.0 unx     4157 b- defN 23-Jun-11 13:10 org/jpmml/python/ParseException.class
+-rw-rw-r--  2.0 unx      282 b- defN 23-Jun-11 13:10 org/jpmml/python/HasArray.class
+-rw-rw-r--  2.0 unx     3481 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonParserUtil.class
+-rw-rw-r--  2.0 unx     2631 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefScope.class
+-rw-rw-r--  2.0 unx      784 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     2861 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage.class
+-rw-rw-r--  2.0 unx      777 b- defN 23-Jun-11 13:10 org/jpmml/python/PredicateTranslator$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     1016 b- defN 23-Jun-11 13:10 org/jpmml/python/CastUtil.class
+-rw-rw-r--  2.0 unx      164 b- defN 23-Jun-11 13:10 org/jpmml/python/TypeInfo.class
+-rw-rw-r--  2.0 unx     5554 b- defN 23-Jun-11 13:10 org/jpmml/python/ClassDictUtil.class
+-rw-rw-r--  2.0 unx    39573 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator.class
+-rw-rw-r--  2.0 unx     1294 b- defN 23-Jun-11 13:10 org/jpmml/python/StreamProvider.class
+-rw-rw-r--  2.0 unx     1340 b- defN 23-Jun-11 13:10 org/jpmml/python/PickleUtil$1.class
+-rw-rw-r--  2.0 unx     6658 b- defN 23-Jun-11 13:10 org/jpmml/python/SimpleCharStream.class
+-rw-rw-r--  2.0 unx     9499 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefParser.class
+-rw-rw-r--  2.0 unx     1139 b- defN 23-Jun-11 13:10 org/jpmml/python/InputStreamStorage.class
+-rw-rw-r--  2.0 unx      986 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator$Block.class
+-rw-rw-r--  2.0 unx      914 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage$Type$1.class
+-rw-rw-r--  2.0 unx     4624 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonParser.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jun-11 13:10 org/jpmml/python/NamedTuple.class
+-rw-rw-r--  2.0 unx     1303 b- defN 23-Jun-11 13:10 org/jpmml/python/ClassDictUtil$1.class
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jun-11 13:10 org/jpmml/python/NullConstructor.class
+-rw-rw-r--  2.0 unx     1120 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonTypeUtil.class
+-rw-rw-r--  2.0 unx     1145 b- defN 23-Jun-11 13:10 org/jpmml/python/FileStorage.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Jun-11 13:10 org/jpmml/python/StringProvider.class
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Jun-11 13:10 org/jpmml/python/PushbackPythonParserTokenManager.class
+-rw-rw-r--  2.0 unx     9731 b- defN 23-Jun-11 13:10 org/jpmml/python/AbstractTranslator.class
+-rw-rw-r--  2.0 unx     8808 b- defN 23-Jun-11 13:10 org/jpmml/python/PickleUtil.class
+-rw-rw-r--  2.0 unx     2017 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonEnumConstructor.class
+-rw-rw-r--  2.0 unx     4475 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObjectConstructor.class
+-rw-rw-r--  2.0 unx      800 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDef$Parameter.class
+-rw-rw-r--  2.0 unx      183 b- defN 23-Jun-11 13:10 org/jpmml/python/Identifiable.class
+-rw-rw-r--  2.0 unx     2647 b- defN 23-Jun-11 13:10 org/jpmml/python/ClassDictConstructorUtil.class
+-rw-rw-r--  2.0 unx    10443 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject.class
+-rw-rw-r--  2.0 unx     1442 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$1.class
+-rw-rw-r--  2.0 unx    11022 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionUtil.class
+-rw-rw-r--  2.0 unx     1456 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$3.class
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jun-11 13:10 org/jpmml/python/PredicateTranslator$1.class
+-rw-rw-r--  2.0 unx      434 b- defN 23-Jun-11 13:10 org/jpmml/python/IConstantConstructor.class
+-rw-rw-r--  2.0 unx     1338 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDef.class
+-rw-rw-r--  2.0 unx      270 b- defN 23-Jun-11 13:10 org/jpmml/python/HasContent.class
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefParser$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     1545 b- defN 23-Jun-11 13:10 org/jpmml/python/CustomPythonObjectConstructor.class
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage$Type.class
+-rw-rw-r--  2.0 unx      233 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefParser$1.class
+-rw-rw-r--  2.0 unx      534 b- defN 23-Jun-11 13:10 org/jpmml/python/NullProvider.class
+-rw-rw-r--  2.0 unx      219 b- defN 23-Jun-11 13:10 org/jpmml/python/Provider.class
+-rw-rw-r--  2.0 unx      566 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonEnum.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jun-11 13:10 org/jpmml/python/PredicateTranslator$JJCalls.class
+-rw-rw-r--  2.0 unx     1201 b- defN 23-Jun-11 13:10 org/jpmml/python/CalendarUtil.class
+-rw-rw-r--  2.0 unx     1793 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$2.class
+-rw-rw-r--  2.0 unx     2786 b- defN 23-Jun-11 13:10 org/jpmml/python/SliceUtil.class
+-rw-rw-r--  2.0 unx      234 b- defN 23-Jun-11 13:10 org/jpmml/python/Castable.class
+-rw-rw-r--  2.0 unx     1107 b- defN 23-Jun-11 13:10 org/jpmml/python/TupleUtil$1.class
+-rw-rw-r--  2.0 unx     1512 b- defN 23-Jun-11 13:10 org/jpmml/python/AbstractTranslator$1.class
+-rw-rw-r--  2.0 unx     1795 b- defN 23-Jun-11 13:10 org/jpmml/python/CastFunction.class
+-rw-rw-r--  2.0 unx     1106 b- defN 23-Jun-11 13:10 org/jpmml/python/TupleUtil$3.class
+-rw-rw-r--  2.0 unx     1873 b- defN 23-Jun-11 13:10 org/jpmml/python/NamedTupleConstructor.class
+-rw-rw-r--  2.0 unx      509 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator$JJCalls.class
+-rw-rw-r--  2.0 unx      875 b- defN 23-Jun-11 13:10 org/jpmml/python/SliceUtil$1.class
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Jun-11 13:10 org/jpmml/python/BlockScope.class
+-rw-rw-r--  2.0 unx     5585 b- defN 23-Jun-11 13:10 org/jpmml/python/DataFrameScope.class
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonEncoder.class
+-rw-rw-r--  2.0 unx     1454 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$4.class
+-rw-rw-r--  2.0 unx     1729 b- defN 23-Jun-11 13:10 org/jpmml/python/Scope.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jun-11 13:10 org/jpmml/python/TupleUtil$2.class
+-rw-rw-r--  2.0 unx    15414 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonParserTokenManager.class
+-rw-rw-r--  2.0 unx     3168 b- defN 23-Jun-11 13:10 org/jpmml/python/CustomPythonObject.class
+-rw-rw-r--  2.0 unx    23578 b- defN 23-Jun-11 13:10 org/jpmml/python/PredicateTranslator.class
+-rw-rw-r--  2.0 unx     1629 b- defN 23-Jun-11 13:10 org/jpmml/python/StorageUtil.class
+-rw-rw-r--  2.0 unx     1128 b- defN 23-Jun-11 13:10 joblib/NDArrayWrapperConstructor$1.class
+-rw-rw-r--  2.0 unx     1371 b- defN 23-Jun-11 13:10 joblib/NDArrayWrapperConstructor.class
+-rw-rw-r--  2.0 unx     2667 b- defN 23-Jun-11 13:10 joblib/NumpyArrayWrapper.class
+-rw-rw-r--  2.0 unx     2493 b- defN 23-Jun-11 13:10 joblib/NDArrayWrapper.class
+-rw-rw-r--  2.0 unx      388 b- defN 23-Jun-11 13:10 scipy/stats/RVGeneric.class
+-rw-rw-r--  2.0 unx      559 b- defN 23-Jun-11 13:10 scipy/stats/RVContinuous.class
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Jun-11 13:10 scipy/interpolate/BSpline.class
+-rw-rw-r--  2.0 unx     1541 b- defN 23-Jun-11 13:10 scipy/sparse/CSRMatrix.class
+-rw-rw-r--  2.0 unx     2618 b- defN 23-Jun-11 13:10 scipy/sparse/CSRMatrixUtil.class
+-rw-rw-r--  2.0 unx     2086 b- defN 23-Jun-11 13:10 builtins/Type.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Jun-11 13:10 builtins/GetAttr.class
+-rw-rw-r--  2.0 unx      536 b- defN 23-Jun-11 13:10 builtins/TypeConstructor.class
+-rw-rw-r--  2.0 unx      637 b- defN 23-Jun-11 13:10 builtins/Function.class
+-rw-rw-r--  2.0 unx      855 b- defN 23-Jun-11 13:10 builtins/Slice.class
+-rw-rw-r--  2.0 unx     5158 b- defN 23-Jun-11 13:10 META-INF/maven/org.jpmml/pmml-python/pom.xml
+-rw-rw-r--  2.0 unx       56 b- defN 23-Jun-11 13:10 META-INF/maven/org.jpmml/pmml-python/pom.properties
+172 files, 378890 bytes uncompressed, 178291 bytes compressed:  52.9%
```

#### zipnote «TEMP»/diffoscope_rvr563yz_/tmpqr09iz_n_.zip

```diff
@@ -42,14 +42,17 @@
 
 Filename: joblib/
 Comment: 
 
 Filename: scipy/
 Comment: 
 
+Filename: scipy/stats/
+Comment: 
+
 Filename: scipy/interpolate/
 Comment: 
 
 Filename: scipy/sparse/
 Comment: 
 
 Filename: builtins/
@@ -144,14 +147,17 @@
 
 Filename: pandas/core/BooleanDtype.class
 Comment: 
 
 Filename: pandas/core/Categorical.class
 Comment: 
 
+Filename: pandas/core/SeriesUtil$1.class
+Comment: 
+
 Filename: pandas/core/MaskedArray$1.class
 Comment: 
 
 Filename: pandas/core/ExtensionDtype.class
 Comment: 
 
 Filename: pandas/core/Block.class
@@ -468,14 +474,20 @@
 
 Filename: joblib/NumpyArrayWrapper.class
 Comment: 
 
 Filename: joblib/NDArrayWrapper.class
 Comment: 
 
+Filename: scipy/stats/RVGeneric.class
+Comment: 
+
+Filename: scipy/stats/RVContinuous.class
+Comment: 
+
 Filename: scipy/interpolate/BSpline.class
 Comment: 
 
 Filename: scipy/sparse/CSRMatrix.class
 Comment: 
 
 Filename: scipy/sparse/CSRMatrixUtil.class
@@ -486,14 +498,17 @@
 
 Filename: builtins/GetAttr.class
 Comment: 
 
 Filename: builtins/TypeConstructor.class
 Comment: 
 
+Filename: builtins/Function.class
+Comment: 
+
 Filename: builtins/Slice.class
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-python/pom.xml
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-python/pom.properties
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-Python library
-Implementation-Version: 1.1.14
+Implementation-Version: 1.1.15
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### META-INF/python2pmml.properties

```diff
@@ -1,13 +1,14 @@
 builtins.getattr = builtins.GetAttr
 builtins.slice = builtins.Slice
 builtins.(bool|float|int|str) = builtins.TypeConstructor
 collections.defaultdict = collections.DefaultDict
 functools.partial = functools.Partial
 joblib.numpy_pickle.NumpyArrayWrapper = joblib.NumpyArrayWrapper
+math.(acos|asin|atan|atan2|ceil|copysign|cos|cosh|degrees|exp|expm1|fabs|floor|hypot|isnan|log|log1p|log10|pow|radians|sin|sinh|sqrt|tan|tanh|trunc) = builtins.Function
 numpy.(|core.fromnumeric.)clip = numpy.core.Function
 numpy.(|core._multiarray_umath.)(absolute|arccos|arcsin|arctan|arctan2|ceil|clip|cos|cosh|degrees|rad2deg|exp|expm1|floor|fmax|fmin|hypot|log|log1p|log10|negative|power|radians|deg2rad|reciprocal|rint|sign|sin|sinh|sqrt|square|tan|tanh) = numpy.core.Function
 numpy.(bool_|float_|float32|float64|int_|int8|int16|int32|int64|str_|uint8|uint16|uint32|uint64) = builtins.TypeConstructor
 numpy.core.(_multiarray_umath|multiarray)._reconstruct = numpy.core.NDArray
 numpy.core.(_multiarray_umath|multiarray).scalar = numpy.core.Scalar
 numpy.core.numeric._frombuffer = numpy.core.FromBufferConstructor
 numpy.core._ufunc_reconstruct = numpy.core.UFunc
@@ -33,10 +34,12 @@
 pandas.core.internals.managers.SingleBlockManager = pandas.core.SingleBlockManager
 pandas.core.series.Series = pandas.core.Series
 pandas._libs.arrays.__pyx_unpickle_NDArrayBacked = pandas.NDArrayBacked
 pandas._libs.internals._unpickle_block = pandas.core.Block
 pandas._libs.missing.NA = null
 scipy.interpolate._bsplines.BSpline = scipy.interpolate.BSpline
 scipy.sparse.(_csr|csr).csr_matrix = scipy.sparse.CSRMatrix
+scipy.stats._continuous_distns.logistic_gen = scipy.stats.RVContinuous
+scipy.stats._continuous_distns.norm_gen = scipy.stats.RVContinuous
 sklearn.externals.joblib.numpy_pickle.NumpyArrayWrapper = joblib.NumpyArrayWrapper
 treelib.tree.Tree = treelib.Tree
 treelib.node.Node = treelib.Node
```

#### pandas/core/BlockManager.class

##### procyon -ec {}

```diff
@@ -2,14 +2,16 @@
 package pandas.core;
 
 import java.util.stream.Collector;
 import java.util.stream.Collectors;
 import java.util.Arrays;
 import org.jpmml.python.HasArray;
 import java.util.List;
+import org.jpmml.python.ClassDictUtil;
+import java.util.Collection;
 import org.jpmml.python.CustomPythonObject;
 
 public class BlockManager extends CustomPythonObject
 {
     private static final String[] INIT_ATTRIBUTES;
     private static final String[] SETSTATE_ATTRIBUTES;
     
@@ -31,14 +33,26 @@
             final Object[] newArgs = new Object[3];
             System.arraycopy(args, 0, newArgs, 0, newArgs.length);
             args = newArgs;
         }
         super.__setstate__(createAttributeMap(BlockManager.SETSTATE_ATTRIBUTES, args));
     }
     
+    public Index getColumnAxis() {
+        final List<Index> axesArray = this.getAxesArray();
+        ClassDictUtil.checkSize(2, new Collection[] { axesArray });
+        return axesArray.get(0);
+    }
+    
+    public Index getRowAxis() {
+        final List<Index> axesArray = this.getAxesArray();
+        ClassDictUtil.checkSize(2, new Collection[] { axesArray });
+        return axesArray.get(1);
+    }
+    
     public List<Index> getAxesArray() {
         if (this.containsKey((Object)"axes_array")) {
             return this.getList("axes_array", (Class)Index.class);
         }
         return this.getList("axes", (Class)Index.class);
     }
```

#### pandas/core/SeriesUtil.class

##### procyon -ec {}

```diff
@@ -1,24 +1,32 @@
 
 package pandas.core;
 
-import org.jpmml.python.HasArray;
-import java.util.List;
 import java.util.LinkedHashMap;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import com.google.common.collect.Lists;
 import java.util.Map;
 import com.google.common.base.Function;
+import org.jpmml.python.HasArray;
+import java.util.List;
 
 public class SeriesUtil
 {
     private SeriesUtil() {
     }
     
+    public static Series createSeries(final Index index, final List<?> values) {
+        final HasArray hasArray = (HasArray)new SeriesUtil.SeriesUtil$1((List)values);
+        final SingleBlockManager singleBlockManager = new SingleBlockManager().setOnlyBlockItem(index).setOnlyBlockValue(hasArray);
+        final Series result = new Series();
+        result.setBlockManager(singleBlockManager);
+        return result;
+    }
+    
     public static <InK, OutK, InV, OutV> Map<OutK, OutV> toMap(final Series series, final Function<InK, OutK> keyFunction, final Function<InV, OutV> valueFunction) {
         final SingleBlockManager blockManager = series.getBlockManager();
         final Index blockItem = blockManager.getOnlyBlockItem();
         final List<OutK> keys = Lists.transform(blockItem.getValues(), (Function)keyFunction);
         final HasArray blockValue = blockManager.getOnlyBlockValue();
         final List<OutV> values = Lists.transform(blockValue.getArrayContent(), (Function)valueFunction);
         ClassDictUtil.checkSize(new Collection[] { keys, values });
```

#### numpy/random/BitGeneratorUtil.class

##### procyon -ec {}

```diff
@@ -6,15 +6,15 @@
 import net.razorvine.pickle.objects.ClassDictConstructor;
 
 public class BitGeneratorUtil
 {
     private BitGeneratorUtil() {
     }
     
-    public static BitGenerator create(final Object[] args) {
+    public static BitGenerator createBitGenerator(final Object[] args) {
         if (args.length == 1) {
             final String bitGeneratorName = (String)args[0];
             final BitGenerator bitGenerator = new BitGenerator("numpy.random._" + bitGeneratorName.toLowerCase(), bitGeneratorName);
             return bitGenerator;
         }
         if (args.length == 2) {
             final String bitGeneratorName = (String)args[0];
```

#### numpy/random/Generator.class

##### procyon -ec {}

```diff
@@ -7,13 +7,13 @@
 public class Generator extends CustomPythonObject
 {
     public Generator(final String module, final String name) {
         super(module, name);
     }
     
     public void __init__(final Object[] args) {
-        final Object bitGenerator = BitGeneratorUtil.create(args);
+        final Object bitGenerator = BitGeneratorUtil.createBitGenerator(args);
         final HashMap<String, Object> attributes = new HashMap<String, Object>();
         attributes.put("bit_generator", bitGenerator);
         super.__setstate__((HashMap)attributes);
     }
 }
```

#### numpy/random/LegacyRandomState.class

##### procyon -ec {}

```diff
@@ -6,13 +6,13 @@
 public class LegacyRandomState extends RandomState
 {
     public LegacyRandomState(final String module, final String name) {
         super(module, name);
     }
     
     public void __init__(final Object[] args) {
-        final Object bitGenerator = BitGeneratorUtil.create(args);
+        final Object bitGenerator = BitGeneratorUtil.createBitGenerator(args);
         final HashMap<String, Object> attributes = new HashMap<String, Object>();
         attributes.put("bit_generator", bitGenerator);
         super.__setstate__((HashMap)attributes);
     }
 }
```

#### numpy/DType.class

##### procyon -ec {}

```diff
@@ -23,15 +23,19 @@
         super(module, name);
     }
     
     public void __init__(final Object[] args) {
         super.__setstate__(createAttributeMap(DType.INIT_ATTRIBUTES, args));
     }
     
-    public void __setstate__(final Object[] args) {
+    public void __setstate__(Object[] args) {
+        if (args.length == DType.SETSTATE_ATTRIBUTES.length + 1) {
+            final Object[] datetime_data = (Object[])args[DType.SETSTATE_ATTRIBUTES.length];
+            args = extractArgs(args, 0, DType.SETSTATE_ATTRIBUTES.length);
+        }
         super.__setstate__(createAttributeMap(DType.SETSTATE_ATTRIBUTES, args));
     }
     
     public DataType getDataType() {
         final String obj = this.getObj();
         final String order = this.getOrder();
         final String descr = formatDescr(obj, order);
```

#### numpy/core/TypeDescriptor$Kind.class

##### procyon -ec {}

```diff
@@ -4,14 +4,16 @@
 public enum Kind
 {
     public static final enum Kind BOOLEAN;
     public static final enum Kind INTEGER;
     public static final enum Kind UNSIGNED_INTEGER;
     public static final enum Kind FLOAT;
     public static final enum Kind COMPLEX_FLOAT;
+    public static final enum Kind TIMEDELTA;
+    public static final enum Kind DATETIME;
     public static final enum Kind OBJECT;
     public static final enum Kind STRING;
     public static final enum Kind UNICODE;
     public static final enum Kind VOID;
     
     public static Kind valueOf(final String name) {
         return Enum.valueOf(Kind.class, name);
@@ -30,14 +32,20 @@
             }
             case 'f': {
                 return Kind.FLOAT;
             }
             case 'c': {
                 return Kind.COMPLEX_FLOAT;
             }
+            case 'm': {
+                return Kind.TIMEDELTA;
+            }
+            case 'M': {
+                return Kind.DATETIME;
+            }
             case 'O': {
                 return Kind.OBJECT;
             }
             case 'S':
             case 'a': {
                 return Kind.STRING;
             }
@@ -55,14 +63,16 @@
     
     static {
         Kind.BOOLEAN = new Kind("BOOLEAN", 0);
         Kind.INTEGER = new Kind("INTEGER", 1);
         Kind.UNSIGNED_INTEGER = new Kind("UNSIGNED_INTEGER", 2);
         Kind.FLOAT = new Kind("FLOAT", 3);
         Kind.COMPLEX_FLOAT = new Kind("COMPLEX_FLOAT", 4);
-        Kind.OBJECT = new Kind("OBJECT", 5);
-        Kind.STRING = new Kind("STRING", 6);
-        Kind.UNICODE = new Kind("UNICODE", 7);
-        Kind.VOID = new Kind("VOID", 8);
-        Kind.$VALUES = new Kind[] { Kind.BOOLEAN, Kind.INTEGER, Kind.UNSIGNED_INTEGER, Kind.FLOAT, Kind.COMPLEX_FLOAT, Kind.OBJECT, Kind.STRING, Kind.UNICODE, Kind.VOID };
+        Kind.TIMEDELTA = new Kind("TIMEDELTA", 5);
+        Kind.DATETIME = new Kind("DATETIME", 6);
+        Kind.OBJECT = new Kind("OBJECT", 7);
+        Kind.STRING = new Kind("STRING", 8);
+        Kind.UNICODE = new Kind("UNICODE", 9);
+        Kind.VOID = new Kind("VOID", 10);
+        Kind.$VALUES = new Kind[] { Kind.BOOLEAN, Kind.INTEGER, Kind.UNSIGNED_INTEGER, Kind.FLOAT, Kind.COMPLEX_FLOAT, Kind.TIMEDELTA, Kind.DATETIME, Kind.OBJECT, Kind.STRING, Kind.UNICODE, Kind.VOID };
     }
 }
```

#### numpy/core/TypeDescriptor$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,76 +1,79 @@
-  SHA-256 checksum d9d54ff44b32f08a533918d3bc86f94f5c92103ba0006e4a03bce140597cf994
+  SHA-256 checksum f2beff5967e36c92c9ae8f9161ed584ae368755bb7f53c4e32593d21b21db0f2
   Compiled from "TypeDescriptor.java"
 class numpy.core.TypeDescriptor$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
-  this_class: #13                         // numpy/core/TypeDescriptor$1
-  super_class: #14                        // java/lang/Object
+  this_class: #14                         // numpy/core/TypeDescriptor$1
+  super_class: #15                        // java/lang/Object
   interfaces: 0, fields: 1, methods: 1, attributes: 3
 Constant pool:
-   #1 = Methodref          #28.#29        // numpy/core/TypeDescriptor$Kind.values:()[Lnumpy/core/TypeDescriptor$Kind;
-   #2 = Fieldref           #13.#30        // numpy/core/TypeDescriptor$1.$SwitchMap$numpy$core$TypeDescriptor$Kind:[I
-   #3 = Fieldref           #28.#31        // numpy/core/TypeDescriptor$Kind.BOOLEAN:Lnumpy/core/TypeDescriptor$Kind;
-   #4 = Methodref          #28.#32        // numpy/core/TypeDescriptor$Kind.ordinal:()I
-   #5 = Class              #33            // java/lang/NoSuchFieldError
-   #6 = Fieldref           #28.#34        // numpy/core/TypeDescriptor$Kind.INTEGER:Lnumpy/core/TypeDescriptor$Kind;
-   #7 = Fieldref           #28.#35        // numpy/core/TypeDescriptor$Kind.UNSIGNED_INTEGER:Lnumpy/core/TypeDescriptor$Kind;
-   #8 = Fieldref           #28.#36        // numpy/core/TypeDescriptor$Kind.FLOAT:Lnumpy/core/TypeDescriptor$Kind;
-   #9 = Fieldref           #28.#37        // numpy/core/TypeDescriptor$Kind.OBJECT:Lnumpy/core/TypeDescriptor$Kind;
-  #10 = Fieldref           #28.#38        // numpy/core/TypeDescriptor$Kind.STRING:Lnumpy/core/TypeDescriptor$Kind;
-  #11 = Fieldref           #28.#39        // numpy/core/TypeDescriptor$Kind.UNICODE:Lnumpy/core/TypeDescriptor$Kind;
-  #12 = Fieldref           #28.#40        // numpy/core/TypeDescriptor$Kind.VOID:Lnumpy/core/TypeDescriptor$Kind;
-  #13 = Class              #41            // numpy/core/TypeDescriptor$1
-  #14 = Class              #43            // java/lang/Object
-  #15 = Utf8               $SwitchMap$numpy$core$TypeDescriptor$Kind
-  #16 = Utf8               [I
-  #17 = Utf8               <clinit>
-  #18 = Utf8               ()V
-  #19 = Utf8               Code
-  #20 = Utf8               LineNumberTable
-  #21 = Utf8               LocalVariableTable
-  #22 = Utf8               StackMapTable
-  #23 = Class              #33            // java/lang/NoSuchFieldError
-  #24 = Utf8               SourceFile
-  #25 = Utf8               TypeDescriptor.java
-  #26 = Utf8               EnclosingMethod
-  #27 = Class              #44            // numpy/core/TypeDescriptor
-  #28 = Class              #45            // numpy/core/TypeDescriptor$Kind
-  #29 = NameAndType        #47:#48        // values:()[Lnumpy/core/TypeDescriptor$Kind;
-  #30 = NameAndType        #15:#16        // $SwitchMap$numpy$core$TypeDescriptor$Kind:[I
-  #31 = NameAndType        #49:#50        // BOOLEAN:Lnumpy/core/TypeDescriptor$Kind;
-  #32 = NameAndType        #51:#52        // ordinal:()I
-  #33 = Utf8               java/lang/NoSuchFieldError
-  #34 = NameAndType        #53:#50        // INTEGER:Lnumpy/core/TypeDescriptor$Kind;
-  #35 = NameAndType        #54:#50        // UNSIGNED_INTEGER:Lnumpy/core/TypeDescriptor$Kind;
-  #36 = NameAndType        #55:#50        // FLOAT:Lnumpy/core/TypeDescriptor$Kind;
-  #37 = NameAndType        #56:#50        // OBJECT:Lnumpy/core/TypeDescriptor$Kind;
-  #38 = NameAndType        #57:#50        // STRING:Lnumpy/core/TypeDescriptor$Kind;
-  #39 = NameAndType        #58:#50        // UNICODE:Lnumpy/core/TypeDescriptor$Kind;
-  #40 = NameAndType        #59:#50        // VOID:Lnumpy/core/TypeDescriptor$Kind;
-  #41 = Utf8               numpy/core/TypeDescriptor$1
-  #42 = Utf8               InnerClasses
-  #43 = Utf8               java/lang/Object
-  #44 = Utf8               numpy/core/TypeDescriptor
-  #45 = Utf8               numpy/core/TypeDescriptor$Kind
-  #46 = Utf8               Kind
-  #47 = Utf8               values
-  #48 = Utf8               ()[Lnumpy/core/TypeDescriptor$Kind;
-  #49 = Utf8               BOOLEAN
-  #50 = Utf8               Lnumpy/core/TypeDescriptor$Kind;
-  #51 = Utf8               ordinal
-  #52 = Utf8               ()I
-  #53 = Utf8               INTEGER
-  #54 = Utf8               UNSIGNED_INTEGER
-  #55 = Utf8               FLOAT
-  #56 = Utf8               OBJECT
-  #57 = Utf8               STRING
-  #58 = Utf8               UNICODE
-  #59 = Utf8               VOID
+   #1 = Methodref          #29.#30        // numpy/core/TypeDescriptor$Kind.values:()[Lnumpy/core/TypeDescriptor$Kind;
+   #2 = Fieldref           #14.#31        // numpy/core/TypeDescriptor$1.$SwitchMap$numpy$core$TypeDescriptor$Kind:[I
+   #3 = Fieldref           #29.#32        // numpy/core/TypeDescriptor$Kind.BOOLEAN:Lnumpy/core/TypeDescriptor$Kind;
+   #4 = Methodref          #29.#33        // numpy/core/TypeDescriptor$Kind.ordinal:()I
+   #5 = Class              #34            // java/lang/NoSuchFieldError
+   #6 = Fieldref           #29.#35        // numpy/core/TypeDescriptor$Kind.INTEGER:Lnumpy/core/TypeDescriptor$Kind;
+   #7 = Fieldref           #29.#36        // numpy/core/TypeDescriptor$Kind.UNSIGNED_INTEGER:Lnumpy/core/TypeDescriptor$Kind;
+   #8 = Fieldref           #29.#37        // numpy/core/TypeDescriptor$Kind.FLOAT:Lnumpy/core/TypeDescriptor$Kind;
+   #9 = Fieldref           #29.#38        // numpy/core/TypeDescriptor$Kind.DATETIME:Lnumpy/core/TypeDescriptor$Kind;
+  #10 = Fieldref           #29.#39        // numpy/core/TypeDescriptor$Kind.OBJECT:Lnumpy/core/TypeDescriptor$Kind;
+  #11 = Fieldref           #29.#40        // numpy/core/TypeDescriptor$Kind.STRING:Lnumpy/core/TypeDescriptor$Kind;
+  #12 = Fieldref           #29.#41        // numpy/core/TypeDescriptor$Kind.UNICODE:Lnumpy/core/TypeDescriptor$Kind;
+  #13 = Fieldref           #29.#42        // numpy/core/TypeDescriptor$Kind.VOID:Lnumpy/core/TypeDescriptor$Kind;
+  #14 = Class              #43            // numpy/core/TypeDescriptor$1
+  #15 = Class              #45            // java/lang/Object
+  #16 = Utf8               $SwitchMap$numpy$core$TypeDescriptor$Kind
+  #17 = Utf8               [I
+  #18 = Utf8               <clinit>
+  #19 = Utf8               ()V
+  #20 = Utf8               Code
+  #21 = Utf8               LineNumberTable
+  #22 = Utf8               LocalVariableTable
+  #23 = Utf8               StackMapTable
+  #24 = Class              #34            // java/lang/NoSuchFieldError
+  #25 = Utf8               SourceFile
+  #26 = Utf8               TypeDescriptor.java
+  #27 = Utf8               EnclosingMethod
+  #28 = Class              #46            // numpy/core/TypeDescriptor
+  #29 = Class              #47            // numpy/core/TypeDescriptor$Kind
+  #30 = NameAndType        #49:#50        // values:()[Lnumpy/core/TypeDescriptor$Kind;
+  #31 = NameAndType        #16:#17        // $SwitchMap$numpy$core$TypeDescriptor$Kind:[I
+  #32 = NameAndType        #51:#52        // BOOLEAN:Lnumpy/core/TypeDescriptor$Kind;
+  #33 = NameAndType        #53:#54        // ordinal:()I
+  #34 = Utf8               java/lang/NoSuchFieldError
+  #35 = NameAndType        #55:#52        // INTEGER:Lnumpy/core/TypeDescriptor$Kind;
+  #36 = NameAndType        #56:#52        // UNSIGNED_INTEGER:Lnumpy/core/TypeDescriptor$Kind;
+  #37 = NameAndType        #57:#52        // FLOAT:Lnumpy/core/TypeDescriptor$Kind;
+  #38 = NameAndType        #58:#52        // DATETIME:Lnumpy/core/TypeDescriptor$Kind;
+  #39 = NameAndType        #59:#52        // OBJECT:Lnumpy/core/TypeDescriptor$Kind;
+  #40 = NameAndType        #60:#52        // STRING:Lnumpy/core/TypeDescriptor$Kind;
+  #41 = NameAndType        #61:#52        // UNICODE:Lnumpy/core/TypeDescriptor$Kind;
+  #42 = NameAndType        #62:#52        // VOID:Lnumpy/core/TypeDescriptor$Kind;
+  #43 = Utf8               numpy/core/TypeDescriptor$1
+  #44 = Utf8               InnerClasses
+  #45 = Utf8               java/lang/Object
+  #46 = Utf8               numpy/core/TypeDescriptor
+  #47 = Utf8               numpy/core/TypeDescriptor$Kind
+  #48 = Utf8               Kind
+  #49 = Utf8               values
+  #50 = Utf8               ()[Lnumpy/core/TypeDescriptor$Kind;
+  #51 = Utf8               BOOLEAN
+  #52 = Utf8               Lnumpy/core/TypeDescriptor$Kind;
+  #53 = Utf8               ordinal
+  #54 = Utf8               ()I
+  #55 = Utf8               INTEGER
+  #56 = Utf8               UNSIGNED_INTEGER
+  #57 = Utf8               FLOAT
+  #58 = Utf8               DATETIME
+  #59 = Utf8               OBJECT
+  #60 = Utf8               STRING
+  #61 = Utf8               UNICODE
+  #62 = Utf8               VOID
 {
   static final int[] $SwitchMap$numpy$core$TypeDescriptor$Kind;
     descriptor: [I
     flags: (0x1018) ACC_STATIC, ACC_FINAL, ACC_SYNTHETIC
 
   static {};
     descriptor: ()V
@@ -106,57 +109,65 @@
         57: getstatic     #8                  // Field numpy/core/TypeDescriptor$Kind.FLOAT:Lnumpy/core/TypeDescriptor$Kind;
         60: invokevirtual #4                  // Method numpy/core/TypeDescriptor$Kind.ordinal:()I
         63: iconst_4
         64: iastore
         65: goto          69
         68: astore_0
         69: getstatic     #2                  // Field $SwitchMap$numpy$core$TypeDescriptor$Kind:[I
-        72: getstatic     #9                  // Field numpy/core/TypeDescriptor$Kind.OBJECT:Lnumpy/core/TypeDescriptor$Kind;
+        72: getstatic     #9                  // Field numpy/core/TypeDescriptor$Kind.DATETIME:Lnumpy/core/TypeDescriptor$Kind;
         75: invokevirtual #4                  // Method numpy/core/TypeDescriptor$Kind.ordinal:()I
         78: iconst_5
         79: iastore
         80: goto          84
         83: astore_0
         84: getstatic     #2                  // Field $SwitchMap$numpy$core$TypeDescriptor$Kind:[I
-        87: getstatic     #10                 // Field numpy/core/TypeDescriptor$Kind.STRING:Lnumpy/core/TypeDescriptor$Kind;
+        87: getstatic     #10                 // Field numpy/core/TypeDescriptor$Kind.OBJECT:Lnumpy/core/TypeDescriptor$Kind;
         90: invokevirtual #4                  // Method numpy/core/TypeDescriptor$Kind.ordinal:()I
         93: bipush        6
         95: iastore
         96: goto          100
         99: astore_0
        100: getstatic     #2                  // Field $SwitchMap$numpy$core$TypeDescriptor$Kind:[I
-       103: getstatic     #11                 // Field numpy/core/TypeDescriptor$Kind.UNICODE:Lnumpy/core/TypeDescriptor$Kind;
+       103: getstatic     #11                 // Field numpy/core/TypeDescriptor$Kind.STRING:Lnumpy/core/TypeDescriptor$Kind;
        106: invokevirtual #4                  // Method numpy/core/TypeDescriptor$Kind.ordinal:()I
        109: bipush        7
        111: iastore
        112: goto          116
        115: astore_0
        116: getstatic     #2                  // Field $SwitchMap$numpy$core$TypeDescriptor$Kind:[I
-       119: getstatic     #12                 // Field numpy/core/TypeDescriptor$Kind.VOID:Lnumpy/core/TypeDescriptor$Kind;
+       119: getstatic     #12                 // Field numpy/core/TypeDescriptor$Kind.UNICODE:Lnumpy/core/TypeDescriptor$Kind;
        122: invokevirtual #4                  // Method numpy/core/TypeDescriptor$Kind.ordinal:()I
        125: bipush        8
        127: iastore
        128: goto          132
        131: astore_0
-       132: return
+       132: getstatic     #2                  // Field $SwitchMap$numpy$core$TypeDescriptor$Kind:[I
+       135: getstatic     #13                 // Field numpy/core/TypeDescriptor$Kind.VOID:Lnumpy/core/TypeDescriptor$Kind;
+       138: invokevirtual #4                  // Method numpy/core/TypeDescriptor$Kind.ordinal:()I
+       141: bipush        9
+       143: iastore
+       144: goto          148
+       147: astore_0
+       148: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             54    65    68   Class java/lang/NoSuchFieldError
             69    80    83   Class java/lang/NoSuchFieldError
             84    96    99   Class java/lang/NoSuchFieldError
            100   112   115   Class java/lang/NoSuchFieldError
            116   128   131   Class java/lang/NoSuchFieldError
+           132   144   147   Class java/lang/NoSuchFieldError
       LineNumberTable:
         line 75: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
-      StackMapTable: number_of_entries = 16
+      StackMapTable: number_of_entries = 18
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
@@ -173,13 +184,16 @@
         frame_type = 0 /* same */
         frame_type = 78 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 78 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
+        frame_type = 78 /* same_locals_1_stack_item */
+          stack = [ class java/lang/NoSuchFieldError ]
+        frame_type = 0 /* same */
 }
 SourceFile: "TypeDescriptor.java"
-EnclosingMethod: #27.#0                 // numpy.core.TypeDescriptor
+EnclosingMethod: #28.#0                 // numpy.core.TypeDescriptor
 InnerClasses:
-  static #13;                             // class numpy/core/TypeDescriptor$1
-  public static final #46= #28 of #27;    // Kind=class numpy/core/TypeDescriptor$Kind of class numpy/core/TypeDescriptor
+  static #14;                             // class numpy/core/TypeDescriptor$1
+  public static final #48= #29 of #28;    // Kind=class numpy/core/TypeDescriptor$Kind of class numpy/core/TypeDescriptor
```

#### numpy/core/TypeDescriptor.class

##### procyon -ec {}

```diff
@@ -77,40 +77,51 @@
                     default: {
                         throw new IllegalArgumentException(descr);
                     }
                 }
                 break;
             }
             case 5: {
+                switch (size) {
+                    case 8: {
+                        return DataType.DATE_TIME;
+                    }
+                    default: {
+                        throw new IllegalArgumentException(descr);
+                    }
+                }
+                break;
+            }
+            case 6: {
                 return DataType.STRING;
             }
-            case 6:
-            case 7: {
+            case 7:
+            case 8: {
                 return DataType.STRING;
             }
             default: {
                 throw new IllegalArgumentException(descr);
             }
         }
     }
     
     public Object read(final InputStream is) throws IOException {
         final String descr = this.getDescr();
         final TypeDescriptor.Kind kind = this.getKind();
         final ByteOrder byteOrder = this.getByteOrder();
         final int size = this.getSize();
-        Label_0395: {
+        Label_0399: {
             switch (TypeDescriptor.TypeDescriptor$1.$SwitchMap$numpy$core$TypeDescriptor$Kind[kind.ordinal()]) {
                 case 1: {
                     switch (size) {
                         case 1: {
                             return Boolean.valueOf(NDArrayUtil.readByte(is) == 1);
                         }
                         default: {
-                            break Label_0395;
+                            break Label_0399;
                         }
                     }
                     break;
                 }
                 case 2: {
                     switch (size) {
                         case 1: {
@@ -122,15 +133,15 @@
                         case 4: {
                             return Integer.valueOf(NDArrayUtil.readInt(is, byteOrder));
                         }
                         case 8: {
                             return Long.valueOf(NDArrayUtil.readLong(is, byteOrder));
                         }
                         default: {
-                            break Label_0395;
+                            break Label_0399;
                         }
                     }
                     break;
                 }
                 case 3: {
                     switch (size) {
                         case 1: {
@@ -143,56 +154,56 @@
                             return Long.valueOf(UnsignedInts.toLong(NDArrayUtil.readInt(is, byteOrder)));
                         }
                         case 8: {
                             final String string = Long.toUnsignedString(NDArrayUtil.readLong(is, byteOrder));
                             return Long.valueOf(Long.parseUnsignedLong(string));
                         }
                         default: {
-                            break Label_0395;
+                            break Label_0399;
                         }
                     }
                     break;
                 }
                 case 4: {
                     switch (size) {
                         case 4: {
                             return Float.valueOf(NDArrayUtil.readFloat(is, byteOrder));
                         }
                         case 8: {
                             return Double.valueOf(NDArrayUtil.readDouble(is, byteOrder));
                         }
                         default: {
-                            break Label_0395;
+                            break Label_0399;
                         }
                     }
                     break;
                 }
-                case 5: {
+                case 6: {
                     return NDArrayUtil.readObject(is);
                 }
-                case 6: {
+                case 7: {
                     return NDArrayUtil.readString(is, size);
                 }
-                case 7: {
+                case 8: {
                     return NDArrayUtil.readUnicode(is, byteOrder, size);
                 }
-                case 8: {
+                case 9: {
                     final byte[] buffer = new byte[size];
                     ByteStreams.readFully(is, buffer);
                     return buffer;
                 }
             }
         }
         throw new IllegalArgumentException(descr);
     }
     
     public boolean isObject() {
         final TypeDescriptor.Kind kind = this.getKind();
         switch (TypeDescriptor.TypeDescriptor$1.$SwitchMap$numpy$core$TypeDescriptor$Kind[kind.ordinal()]) {
-            case 5: {
+            case 6: {
                 return true;
             }
             default: {
                 return false;
             }
         }
     }
```

#### org/jpmml/python/ExpressionTranslator$LookaheadSuccess.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f4ca7ac06fc59b1d6380122a87ed56949a810ea8d03113e90a3c70d14d485dee
+  SHA-256 checksum 12d2567a42b42b73d92575a17e1742b019f86018ccb0894761baf391cdf1cd07
   Compiled from "ExpressionTranslator.java"
 final class org.jpmml.python.ExpressionTranslator$LookaheadSuccess extends java.lang.RuntimeException
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #3                          // org/jpmml/python/ExpressionTranslator$LookaheadSuccess
   super_class: #4                         // java/lang/RuntimeException
@@ -41,42 +41,42 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method java/lang/RuntimeException."<init>":()V
          4: return
       LineNumberTable:
-        line 1854: 0
+        line 1856: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/ExpressionTranslator$LookaheadSuccess;
 
   public java.lang.Throwable fillInStackTrace();
     descriptor: ()Ljava/lang/Throwable;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: areturn
       LineNumberTable:
-        line 1857: 0
+        line 1859: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lorg/jpmml/python/ExpressionTranslator$LookaheadSuccess;
 
   org.jpmml.python.ExpressionTranslator$LookaheadSuccess(org.jpmml.python.ExpressionTranslator$1);
     descriptor: (Lorg/jpmml/python/ExpressionTranslator$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokespecial #1                  // Method "<init>":()V
          4: return
       LineNumberTable:
-        line 1854: 0
+        line 1856: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/ExpressionTranslator$LookaheadSuccess;
             0       5     1    x0   Lorg/jpmml/python/ExpressionTranslator$1;
 }
 SourceFile: "ExpressionTranslator.java"
 InnerClasses:
```

#### org/jpmml/python/ClassDictUtil.class

##### procyon -ec {}

```diff
@@ -17,15 +17,15 @@
     }
     
     public static void checkSize(final Collection<?>... collections) {
         Collection<?> prevCollection = null;
         for (final Collection<?> collection : collections) {
             if (collection != null) {
                 if (prevCollection != null && collection.size() != prevCollection.size()) {
-                    throw new IllegalArgumentException("Expected the same number of elements, got different numbers of elements");
+                    throw new IllegalArgumentException("Expected the same number of elements, got a different numbers of elements");
                 }
                 prevCollection = collection;
             }
         }
     }
     
     public static void checkSize(final int size, final Collection<?>... collections) {
@@ -38,15 +38,15 @@
         }
     }
     
     public static void checkShapes(final int axis, final int[]... shapes) {
         int[] prevShape = null;
         for (final int[] shape : shapes) {
             if (prevShape != null && prevShape[axis] != shape[axis]) {
-                throw new IllegalArgumentException("Expected the same number of elements, got different number of elements");
+                throw new IllegalArgumentException("Expected the same number of elements, got a different number of elements");
             }
             prevShape = shape;
         }
     }
     
     public static void checkShapes(final int axis, final int size, final int[]... shapes) {
         for (final int[] shape : shapes) {
```

#### org/jpmml/python/ExpressionTranslator.class

##### procyon -ec {}

```diff
@@ -146,14 +146,21 @@
             case -2023840679: {
                 if (dottedName.equals("numpy.PZERO")) {
                     n = 5;
                     break;
                 }
                 break;
             }
+            case 299822018: {
+                if (dottedName.equals("math.tau")) {
+                    n = 6;
+                    break;
+                }
+                break;
+            }
         }
         switch (n) {
             case 0:
             case 1: {
                 return PMMLUtil.createConstant((Object)Double.valueOf(2.718281828459045), DataType.DOUBLE);
             }
             case 2: {
@@ -162,14 +169,17 @@
             case 3:
             case 4: {
                 return PMMLUtil.createConstant((Object)Double.valueOf(3.141592653589793), DataType.DOUBLE);
             }
             case 5: {
                 return PMMLUtil.createConstant((Object)Double.valueOf(0.0), DataType.DOUBLE);
             }
+            case 6: {
+                return PMMLUtil.createConstant((Object)Double.valueOf(6.283185307179586), DataType.DOUBLE);
+            }
             default: {
                 int n2 = -1;
                 switch (dottedName.hashCode()) {
                     case 299816245: {
                         if (dottedName.equals("math.nan")) {
                             n2 = 0;
                             break;
@@ -1728,30 +1738,30 @@
             return true;
         }
         finally {
             this.jj_save(6, xla);
         }
     }
     
-    private boolean jj_3R_ArrayIndexingExpression_1107_17_22() {
+    private boolean jj_3R_ArrayIndexingExpression_1109_17_22() {
         if (this.jj_scan_token(22)) {
             return true;
         }
         final Token xsp = this.jj_scanpos;
-        if (this.jj_3R_ArrayIndexingExpression_1108_29_25()) {
+        if (this.jj_3R_ArrayIndexingExpression_1110_29_25()) {
             this.jj_scanpos = xsp;
         }
         return this.jj_scan_token(40) || this.jj_scan_token(23);
     }
     
-    private boolean jj_3R_null_1107_39_21() {
-        return this.jj_3R_Sign_577_9_24();
+    private boolean jj_3R_null_1109_39_21() {
+        return this.jj_3R_Sign_579_9_24();
     }
     
-    private boolean jj_3R_String_561_9_26() {
+    private boolean jj_3R_String_563_9_26() {
         final Token xsp = this.jj_scanpos;
         if (this.jj_scan_token(43)) {
             this.jj_scanpos = xsp;
             if (this.jj_scan_token(50)) {
                 return true;
             }
         }
@@ -1762,15 +1772,15 @@
         return this.jj_scan_token(4) || this.jj_scan_token(5);
     }
     
     private boolean jj_3_1() {
         return this.jj_scan_token(25) || this.jj_scan_token(42);
     }
     
-    private boolean jj_3R_Sign_577_9_24() {
+    private boolean jj_3R_Sign_579_9_24() {
         final Token xsp = this.jj_scanpos;
         if (this.jj_scan_token(16)) {
             this.jj_scanpos = xsp;
             if (this.jj_scan_token(17)) {
                 return true;
             }
         }
@@ -1778,49 +1788,49 @@
     }
     
     private boolean jj_3_4() {
         return this.jj_scan_token(38) || this.jj_scan_token(29);
     }
     
     private boolean jj_3_5() {
-        return this.jj_3R_ArrayIndexingExpression_1106_9_20();
+        return this.jj_3R_ArrayIndexingExpression_1108_9_20();
     }
     
-    private boolean jj_3R_ArrayIndexingExpression_1106_9_20() {
+    private boolean jj_3R_ArrayIndexingExpression_1108_9_20() {
         final Token xsp = this.jj_scanpos;
-        if (this.jj_3R_ArrayIndexingExpression_1107_17_22()) {
+        if (this.jj_3R_ArrayIndexingExpression_1109_17_22()) {
             this.jj_scanpos = xsp;
-            if (this.jj_3R_ArrayIndexingExpression_1116_17_23()) {
+            if (this.jj_3R_ArrayIndexingExpression_1118_17_23()) {
                 return true;
             }
         }
         return false;
     }
     
-    private boolean jj_3R_ArrayIndexingExpression_1108_29_25() {
-        return this.jj_3R_Sign_577_9_24();
+    private boolean jj_3R_ArrayIndexingExpression_1110_29_25() {
+        return this.jj_3R_Sign_579_9_24();
     }
     
     private boolean jj_3_3() {
         return this.jj_scan_token(42) || this.jj_scan_token(15);
     }
     
     private boolean jj_3_6() {
         if (this.jj_scan_token(22)) {
             return true;
         }
         final Token xsp = this.jj_scanpos;
-        if (this.jj_3R_null_1107_39_21()) {
+        if (this.jj_3R_null_1109_39_21()) {
             this.jj_scanpos = xsp;
         }
         return this.jj_scan_token(40);
     }
     
-    private boolean jj_3R_ArrayIndexingExpression_1116_17_23() {
-        return this.jj_scan_token(22) || this.jj_3R_String_561_9_26() || this.jj_scan_token(23);
+    private boolean jj_3R_ArrayIndexingExpression_1118_17_23() {
+        return this.jj_scan_token(22) || this.jj_3R_String_563_9_26() || this.jj_scan_token(23);
     }
     
     private boolean jj_3_7() {
         return this.jj_scan_token(4) || this.jj_scan_token(5);
     }
     
     private static void jj_la1_init_0() {
```

#### org/jpmml/python/ExpressionTranslator$Block.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 5eef59ccd5d9985923c5d2475eac975c0e9d710b6e3b741d0ff1ece963f6eaba
+  SHA-256 checksum 3c5ee3eab72c14c8ee7c4bdd6e3fcb8fde0b9dd1b32a7828ba6c6ff09d705686
   Compiled from "ExpressionTranslator.java"
 class org.jpmml.python.ExpressionTranslator$Block extends java.util.ArrayList<org.dmg.pmml.Expression>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #3                          // org/jpmml/python/ExpressionTranslator$Block
   super_class: #4                         // java/util/ArrayList
@@ -50,16 +50,16 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokespecial #2                  // Method java/util/ArrayList."<init>":(Ljava/util/Collection;)V
          5: return
       LineNumberTable:
-        line 358: 0
-        line 359: 5
+        line 360: 0
+        line 361: 5
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lorg/jpmml/python/ExpressionTranslator$Block;
             0       6     1 statements   Ljava/util/List;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0       6     1 statements   Ljava/util/List<Lorg/dmg/pmml/Expression;>;
@@ -71,15 +71,15 @@
     Code:
       stack=2, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method "<init>":(Ljava/util/List;)V
          5: return
       LineNumberTable:
-        line 355: 0
+        line 357: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lorg/jpmml/python/ExpressionTranslator$Block;
             0       6     1    x0   Ljava/util/List;
             0       6     2    x1   Lorg/jpmml/python/ExpressionTranslator$1;
 }
 Signature: #25                          // Ljava/util/ArrayList<Lorg/dmg/pmml/Expression;>;
```

#### org/jpmml/python/FunctionUtil.class

##### procyon -ec {}

```diff
@@ -19,14 +19,17 @@
     public static Apply encodeFunction(final String module, final String name, final List<Expression> expressions) {
         if (module.equals("builtins")) {
             return encodePythonFunction(module, name, expressions);
         }
         if (module.equals("math")) {
             return encodeMathFunction(module, name, expressions);
         }
+        if (module.equals("pcre") || module.equals("re")) {
+            return encodePCREFunction(module, name, expressions);
+        }
         if (module.equals("numpy") || module.startsWith("numpy.")) {
             return encodeNumpyFunction(module, name, expressions);
         }
         if (module.equals("pandas") || module.startsWith("pandas.")) {
             return encodePandasFunction(module, name, expressions);
         }
         if (module.equals("scipy") || module.startsWith("scipy.")) {
@@ -45,146 +48,307 @@
                         break;
                     }
                     break;
                 }
             }
             switch (n) {
                 case 0: {
-                    return PMMLUtil.createApply("stringLength", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("stringLength", expressions);
                 }
             }
         }
         throw new IllegalArgumentException("Function '" + formatFunction(module, name) + "' is not supported");
     }
     
     public static Apply encodeMathFunction(final String module, final String name, final List<Expression> expressions) {
         if (module.equals("math")) {
             int n = -1;
             switch (name.hashCode()) {
+                case 2988422: {
+                    if (name.equals("acos")) {
+                        n = 0;
+                        break;
+                    }
+                    break;
+                }
+                case 3003607: {
+                    if (name.equals("asin")) {
+                        n = 1;
+                        break;
+                    }
+                    break;
+                }
+                case 3004320: {
+                    if (name.equals("atan")) {
+                        n = 2;
+                        break;
+                    }
+                    break;
+                }
+                case 93133970: {
+                    if (name.equals("atan2")) {
+                        n = 3;
+                        break;
+                    }
+                    break;
+                }
                 case 3049733: {
                     if (name.equals("ceil")) {
-                        n = 0;
+                        n = 4;
+                        break;
+                    }
+                    break;
+                }
+                case 98695: {
+                    if (name.equals("cos")) {
+                        n = 5;
+                        break;
+                    }
+                    break;
+                }
+                case 3059649: {
+                    if (name.equals("cosh")) {
+                        n = 6;
+                        break;
+                    }
+                    break;
+                }
+                case 1546218279: {
+                    if (name.equals("degrees")) {
+                        n = 7;
                         break;
                     }
                     break;
                 }
                 case 100893: {
                     if (name.equals("exp")) {
-                        n = 1;
+                        n = 8;
                         break;
                     }
                     break;
                 }
                 case 96961601: {
                     if (name.equals("expm1")) {
-                        n = 2;
+                        n = 9;
                         break;
                     }
                     break;
                 }
                 case 3135052: {
                     if (name.equals("fabs")) {
-                        n = 3;
+                        n = 10;
                         break;
                     }
                     break;
                 }
                 case 97526796: {
                     if (name.equals("floor")) {
-                        n = 4;
+                        n = 11;
+                        break;
+                    }
+                    break;
+                }
+                case 99762084: {
+                    if (name.equals("hypot")) {
+                        n = 12;
                         break;
                     }
                     break;
                 }
                 case 100504497: {
                     if (name.equals("isnan")) {
-                        n = 5;
+                        n = 13;
                         break;
                     }
                     break;
                 }
                 case 107332: {
                     if (name.equals("log")) {
-                        n = 6;
+                        n = 14;
                         break;
                     }
                     break;
                 }
                 case 103149573: {
                     if (name.equals("logp1")) {
-                        n = 7;
+                        n = 15;
                         break;
                     }
                     break;
                 }
                 case 103147619: {
                     if (name.equals("log10")) {
-                        n = 8;
+                        n = 16;
                         break;
                     }
                     break;
                 }
                 case 111192: {
                     if (name.equals("pow")) {
-                        n = 9;
+                        n = 17;
+                        break;
+                    }
+                    break;
+                }
+                case 968809074: {
+                    if (name.equals("radians")) {
+                        n = 18;
+                        break;
+                    }
+                    break;
+                }
+                case 113880: {
+                    if (name.equals("sin")) {
+                        n = 19;
+                        break;
+                    }
+                    break;
+                }
+                case 3530384: {
+                    if (name.equals("sinh")) {
+                        n = 20;
                         break;
                     }
                     break;
                 }
                 case 3538208: {
                     if (name.equals("sqrt")) {
-                        n = 10;
+                        n = 21;
+                        break;
+                    }
+                    break;
+                }
+                case 114593: {
+                    if (name.equals("tan")) {
+                        n = 22;
+                        break;
+                    }
+                    break;
+                }
+                case 3552487: {
+                    if (name.equals("tanh")) {
+                        n = 23;
                         break;
                     }
                     break;
                 }
                 case 110640556: {
                     if (name.equals("trunc")) {
-                        n = 11;
+                        n = 24;
                         break;
                     }
                     break;
                 }
             }
             switch (n) {
                 case 0: {
-                    return PMMLUtil.createApply("ceil", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("acos", expressions);
                 }
                 case 1: {
-                    return PMMLUtil.createApply("exp", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("asin", expressions);
                 }
                 case 2: {
-                    return PMMLUtil.createApply("expm1", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("atan", expressions);
                 }
                 case 3: {
-                    return PMMLUtil.createApply("abs", new Expression[] { getOnlyElement(expressions) });
+                    return encodeBinaryFunction("x-atan2", expressions);
                 }
                 case 4: {
-                    return PMMLUtil.createApply("floor", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("ceil", expressions);
                 }
                 case 5: {
-                    return PMMLUtil.createApply("isMissing", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("cos", expressions);
                 }
                 case 6: {
-                    return PMMLUtil.createApply("ln", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("cosh", expressions);
                 }
                 case 7: {
-                    return PMMLUtil.createApply("ln1p", new Expression[] { getOnlyElement(expressions) });
+                    return rad2deg(expressions);
                 }
                 case 8: {
-                    return PMMLUtil.createApply("log10", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("exp", expressions);
                 }
                 case 9: {
-                    return PMMLUtil.createApply("pow", new Expression[] { getElement(expressions, 2, 0), getElement(expressions, 2, 1) });
+                    return encodeUnaryFunction("expm1", expressions);
                 }
                 case 10: {
-                    return PMMLUtil.createApply("sqrt", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("abs", expressions);
                 }
                 case 11: {
-                    return PMMLUtil.createApply("if", new Expression[] { (Expression)PMMLUtil.createApply("lessThan", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) }), (Expression)PMMLUtil.createApply("ceil", new Expression[] { getOnlyElement(expressions) }), (Expression)PMMLUtil.createApply("floor", new Expression[] { getOnlyElement(expressions) }) });
+                    return encodeUnaryFunction("floor", expressions);
+                }
+                case 12: {
+                    return encodeUnaryFunction("hypot", expressions);
+                }
+                case 13: {
+                    return encodeUnaryFunction("isMissing", expressions);
+                }
+                case 14: {
+                    return encodeUnaryFunction("ln", expressions);
+                }
+                case 15: {
+                    return encodeUnaryFunction("ln1p", expressions);
+                }
+                case 16: {
+                    return encodeUnaryFunction("log10", expressions);
+                }
+                case 17: {
+                    return encodeBinaryFunction("pow", expressions);
+                }
+                case 18: {
+                    return deg2rad(expressions);
+                }
+                case 19: {
+                    return encodeUnaryFunction("sin", expressions);
+                }
+                case 20: {
+                    return encodeUnaryFunction("sinh", expressions);
+                }
+                case 21: {
+                    return encodeUnaryFunction("sqrt", expressions);
+                }
+                case 22: {
+                    return encodeUnaryFunction("tan", expressions);
+                }
+                case 23: {
+                    return encodeUnaryFunction("tanh", expressions);
+                }
+                case 24: {
+                    return trunc(expressions);
+                }
+            }
+        }
+        throw new IllegalArgumentException("Function '" + formatFunction(module, name) + "' is not supported");
+    }
+    
+    public static Apply encodePCREFunction(final String module, final String name, final List<Expression> expressions) {
+        if (module.equals("pcre") || module.equals("re")) {
+            int n = -1;
+            switch (name.hashCode()) {
+                case -906336856: {
+                    if (name.equals("search")) {
+                        n = 0;
+                        break;
+                    }
+                    break;
+                }
+                case 114240: {
+                    if (name.equals("sub")) {
+                        n = 1;
+                        break;
+                    }
+                    break;
+                }
+            }
+            switch (n) {
+                case 0: {
+                    return search(expressions);
+                }
+                case 1: {
+                    return sub(expressions);
                 }
             }
         }
         throw new IllegalArgumentException("Function '" + formatFunction(module, name) + "' is not supported");
     }
     
     public static Apply encodeNumpyFunction(final String module, final String name, final List<Expression> expressions) {
@@ -456,122 +620,122 @@
                         break;
                     }
                     break;
                 }
             }
             switch (n) {
                 case 0: {
-                    return PMMLUtil.createApply("abs", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("abs", expressions);
                 }
                 case 1: {
-                    return PMMLUtil.createApply("acos", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("acos", expressions);
                 }
                 case 2: {
-                    return PMMLUtil.createApply("asin", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("asin", expressions);
                 }
                 case 3: {
-                    return PMMLUtil.createApply("atan", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("atan", expressions);
                 }
                 case 4: {
-                    return PMMLUtil.createApply("x-atan2", new Expression[] { getElement(expressions, 2, 0), getElement(expressions, 2, 1) });
+                    return encodeBinaryFunction("x-atan2", expressions);
                 }
                 case 5: {
-                    return PMMLUtil.createApply("ceil", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("ceil", expressions);
                 }
                 case 6: {
-                    return PMMLUtil.createApply("min", new Expression[] { (Expression)PMMLUtil.createApply("max", new Expression[] { getElement(expressions, 3, 0), getElement(expressions, 3, 1) }), getElement(expressions, 3, 2) });
+                    return clip(expressions);
                 }
                 case 7: {
-                    return PMMLUtil.createApply("cos", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("cos", expressions);
                 }
                 case 8: {
-                    return PMMLUtil.createApply("cosh", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("cosh", expressions);
                 }
                 case 9:
                 case 10: {
-                    return PMMLUtil.createApply("*", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Double.valueOf(57.29577951308232)) });
+                    return rad2deg(expressions);
                 }
                 case 11: {
-                    return PMMLUtil.createApply("exp", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("exp", expressions);
                 }
                 case 12: {
-                    return PMMLUtil.createApply("expm1", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("expm1", expressions);
                 }
                 case 13: {
-                    return PMMLUtil.createApply("floor", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("floor", expressions);
                 }
                 case 14: {
-                    return PMMLUtil.createApply("max", new Expression[] { getElement(expressions, 2, 0), getElement(expressions, 2, 1) });
+                    return encodeBinaryFunction("max", expressions);
                 }
                 case 15: {
-                    return PMMLUtil.createApply("min", new Expression[] { getElement(expressions, 2, 0), getElement(expressions, 2, 1) });
+                    return encodeBinaryFunction("min", expressions);
                 }
                 case 16: {
-                    return PMMLUtil.createApply("hypot", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("hypot", expressions);
                 }
                 case 17: {
-                    return PMMLUtil.createApply("isMissing", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("isMissing", expressions);
                 }
                 case 18: {
-                    return PMMLUtil.createApply("ln", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("ln", expressions);
                 }
                 case 19: {
-                    return PMMLUtil.createApply("and", new Expression[] { getElement(expressions, 2, 0), getElement(expressions, 2, 1) });
+                    return encodeBinaryFunction("and", expressions);
                 }
                 case 20: {
-                    return PMMLUtil.createApply("not", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("not", expressions);
                 }
                 case 21: {
-                    return PMMLUtil.createApply("or", new Expression[] { getElement(expressions, 2, 0), getElement(expressions, 2, 1) });
+                    return encodeBinaryFunction("or", expressions);
                 }
                 case 22: {
-                    return PMMLUtil.createApply("ln1p", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("ln1p", expressions);
                 }
                 case 23: {
-                    return PMMLUtil.createApply("log10", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("log10", expressions);
                 }
                 case 24: {
-                    return PMMLUtil.createApply("*", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(-1)), getOnlyElement(expressions) });
+                    return negative(expressions);
                 }
                 case 25: {
-                    return PMMLUtil.createApply("pow", new Expression[] { getElement(expressions, 2, 0), getElement(expressions, 2, 1) });
+                    return encodeBinaryFunction("pow", expressions);
                 }
                 case 26:
                 case 27: {
-                    return PMMLUtil.createApply("*", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Double.valueOf(0.017453292519943295)) });
+                    return deg2rad(expressions);
                 }
                 case 28: {
-                    return PMMLUtil.createApply("/", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), getOnlyElement(expressions) });
+                    return reciprocal(expressions);
                 }
                 case 29: {
-                    return PMMLUtil.createApply("rint", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("rint", expressions);
                 }
                 case 30: {
-                    return PMMLUtil.createApply("if", new Expression[] { (Expression)PMMLUtil.createApply("lessThan", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) }), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(-1)), (Expression)PMMLUtil.createApply("if", new Expression[] { (Expression)PMMLUtil.createApply("greaterThan", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) }), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) }) });
+                    return sign(expressions);
                 }
                 case 31: {
-                    return PMMLUtil.createApply("sin", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("sin", expressions);
                 }
                 case 32: {
-                    return PMMLUtil.createApply("sinh", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("sinh", expressions);
                 }
                 case 33: {
-                    return PMMLUtil.createApply("sqrt", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("sqrt", expressions);
                 }
                 case 34: {
-                    return PMMLUtil.createApply("pow", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(2)) });
+                    return square(expressions);
                 }
                 case 35: {
-                    return PMMLUtil.createApply("tan", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("tan", expressions);
                 }
                 case 36: {
-                    return PMMLUtil.createApply("tanh", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("tanh", expressions);
                 }
                 case 37: {
-                    return PMMLUtil.createApply("if", new Expression[] { getElement(expressions, 3, 0), getElement(expressions, 3, 1), getElement(expressions, 3, 2) });
+                    return where(expressions);
                 }
             }
         }
         throw new IllegalArgumentException("Function '" + formatFunction(module, name) + "' is not supported");
     }
     
     public static Apply encodePandasFunction(final String module, final String name, final List<Expression> expressions) {
@@ -606,19 +770,19 @@
                     }
                     break;
                 }
             }
             switch (n) {
                 case 0:
                 case 1: {
-                    return PMMLUtil.createApply("isMissing", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("isMissing", expressions);
                 }
                 case 2:
                 case 3: {
-                    return PMMLUtil.createApply("isNotMissing", new Expression[] { getOnlyElement(expressions) });
+                    return encodeUnaryFunction("isNotMissing", expressions);
                 }
             }
         }
         throw new IllegalArgumentException("Function '" + formatFunction(module, name) + "' is not supported");
     }
     
     public static Apply encodeScipyFunction(final String module, final String name, final List<Expression> expressions) {
@@ -638,24 +802,87 @@
                         break;
                     }
                     break;
                 }
             }
             switch (n) {
                 case 0: {
-                    return PMMLUtil.createApply("/", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), (Expression)PMMLUtil.createApply("+", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), (Expression)PMMLUtil.createApply("exp", new Expression[] { (Expression)PMMLUtil.createApply("*", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(-1)), getOnlyElement(expressions) }) }) }) });
+                    return expit(expressions);
                 }
                 case 1: {
-                    return PMMLUtil.createApply("ln", new Expression[] { (Expression)PMMLUtil.createApply("/", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createApply("-", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), getOnlyElement(expressions) }) }) });
+                    return logit(expressions);
                 }
             }
         }
         throw new IllegalArgumentException("Function '" + formatFunction(module, name) + "' is not supported");
     }
     
+    public static Apply encodeUnaryFunction(final String function, final List<Expression> expressions) {
+        return PMMLUtil.createApply(function, new Expression[] { getElement(expressions, 1, 0) });
+    }
+    
+    public static Apply encodeBinaryFunction(final String function, final List<Expression> expressions) {
+        return PMMLUtil.createApply(function, new Expression[] { getElement(expressions, 2, 0), getElement(expressions, 2, 1) });
+    }
+    
+    private static Apply clip(final List<Expression> expressions) {
+        return PMMLUtil.createApply("min", new Expression[] { (Expression)PMMLUtil.createApply("max", new Expression[] { getElement(expressions, 3, 0), getElement(expressions, 3, 1) }), getElement(expressions, 3, 2) });
+    }
+    
+    private static Apply deg2rad(final List<Expression> expressions) {
+        return PMMLUtil.createApply("*", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Double.valueOf(0.017453292519943295)) });
+    }
+    
+    private static Apply expit(final List<Expression> expressions) {
+        return PMMLUtil.createApply("/", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), (Expression)PMMLUtil.createApply("+", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), (Expression)PMMLUtil.createApply("exp", new Expression[] { (Expression)PMMLUtil.createApply("*", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(-1)), getOnlyElement(expressions) }) }) }) });
+    }
+    
+    private static Apply logit(final List<Expression> expressions) {
+        final Expression expression = getOnlyElement(expressions);
+        return PMMLUtil.createApply("ln", new Expression[] { (Expression)PMMLUtil.createApply("/", new Expression[] { expression, (Expression)PMMLUtil.createApply("-", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), expression }) }) });
+    }
+    
+    private static Apply negative(final List<Expression> expressions) {
+        return PMMLUtil.createApply("*", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(-1)), getOnlyElement(expressions) });
+    }
+    
+    private static Apply rad2deg(final List<Expression> expressions) {
+        return PMMLUtil.createApply("*", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Double.valueOf(57.29577951308232)) });
+    }
+    
+    private static Apply reciprocal(final List<Expression> expressions) {
+        return PMMLUtil.createApply("/", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), getOnlyElement(expressions) });
+    }
+    
+    private static Apply search(final List<Expression> expressions) {
+        return PMMLUtil.createApply("matches", new Expression[] { getElement(expressions, 2, 1), getElement(expressions, 2, 0) });
+    }
+    
+    private static Apply sign(final List<Expression> expressions) {
+        final Expression expression = getOnlyElement(expressions);
+        return PMMLUtil.createApply("if", new Expression[] { (Expression)PMMLUtil.createApply("lessThan", new Expression[] { expression, (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) }), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(-1)), (Expression)PMMLUtil.createApply("if", new Expression[] { (Expression)PMMLUtil.createApply("greaterThan", new Expression[] { expression, (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) }), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(1)), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) }) });
+    }
+    
+    private static Apply square(final List<Expression> expressions) {
+        return PMMLUtil.createApply("pow", new Expression[] { getOnlyElement(expressions), (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(2)) });
+    }
+    
+    private static Apply sub(final List<Expression> expressions) {
+        return PMMLUtil.createApply("replace", new Expression[] { getElement(expressions, 3, 2), getElement(expressions, 3, 0), getElement(expressions, 3, 1) });
+    }
+    
+    private static Apply trunc(final List<Expression> expressions) {
+        final Expression expression = getOnlyElement(expressions);
+        return PMMLUtil.createApply("if", new Expression[] { (Expression)PMMLUtil.createApply("lessThan", new Expression[] { expression, (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(0)) }), (Expression)PMMLUtil.createApply("ceil", new Expression[] { expression }), (Expression)PMMLUtil.createApply("floor", new Expression[] { expression }) });
+    }
+    
+    private static Apply where(final List<Expression> expressions) {
+        return PMMLUtil.createApply("if", new Expression[] { getElement(expressions, 3, 0), getElement(expressions, 3, 1), getElement(expressions, 3, 2) });
+    }
+    
     private static String formatFunction(final String module, final String name) {
         return module + "." + name;
     }
     
     private static Expression getOnlyElement(final List<Expression> expressions) {
         ClassDictUtil.checkSize(1, new Collection[] { expressions });
         return expressions.get(0);
```

#### org/jpmml/python/ExpressionTranslator$JJCalls.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum adcd4c9308f279973fda6afb1ac2955a5d67346324d7a5c09944c034ccef4720
+  SHA-256 checksum 6db756745eb708eb902ba33717fa8edc5e7fdeef29aee2232845c0d49c5fc0c7
   Compiled from "ExpressionTranslator.java"
 final class org.jpmml.python.ExpressionTranslator$JJCalls
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #2                          // org/jpmml/python/ExpressionTranslator$JJCalls
   super_class: #3                         // java/lang/Object
@@ -55,15 +55,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 2044: 0
+        line 2046: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/jpmml/python/ExpressionTranslator$JJCalls;
 }
 SourceFile: "ExpressionTranslator.java"
 InnerClasses:
   static final #10= #2 of #22;            // JJCalls=class org/jpmml/python/ExpressionTranslator$JJCalls of class org/jpmml/python/ExpressionTranslator
```

#### org/jpmml/python/CustomPythonObject.class

##### procyon -ec {}

```diff
@@ -52,8 +52,14 @@
         }
         final HashMap<String, Object> result = new LinkedHashMap<String, Object>();
         for (int i = 0; i < attributes.length; ++i) {
             result.put(attributes[i], args[i]);
         }
         return result;
     }
+    
+    protected static Object[] extractArgs(final Object[] args, final int begin, final int end) {
+        final Object[] result = new Object[end - begin];
+        System.arraycopy(args, begin, result, 0, result.length);
+        return result;
+    }
 }
```

#### META-INF/maven/org.jpmml/pmml-python/pom.xml

##### META-INF/maven/org.jpmml/pmml-python/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-python</artifactId>
-    <version>1.1.14</version>
+    <version>1.1.15</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-python</artifactId>
   <packaging>jar</packaging>
   <name>JPMML Python converter</name>
   <description>JPMML Python to PMML converter</description>
   <licenses>
@@ -121,15 +121,15 @@
             </configuration>
           </execution>
         </executions>
       </plugin>
       <plugin>
         <groupId>org.codehaus.mojo</groupId>
         <artifactId>javacc-maven-plugin</artifactId>
-        <version>2.6</version>
+        <version>3.0.1</version>
         <executions>
           <execution>
             <phase>generate-sources</phase>
             <goals>
               <goal>javacc</goal>
             </goals>
             <configuration>
```

#### META-INF/maven/org.jpmml/pmml-python/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-python
 groupId=org.jpmml
-version=1.1.14
+version=1.1.15
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/classpath.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 istack-commons-runtime-4.0.1.jar
 jackson-annotations-2.13.3.jar
 jakarta.activation-2.0.1.jar
 jakarta.xml.bind-api-3.0.1.jar
 jaxb-core-3.0.2.jar
 jaxb-runtime-3.0.2.jar
 jcommander-1.72.jar
-pickle-1.3.jar
+pickle-1.4.jar
 pmml-converter-1.5.4.jar
-pmml-h2o-1.2.6.jar
+pmml-h2o-1.2.7.jar
 pmml-lightgbm-1.4.5.jar
 pmml-model-1.6.4.jar
 pmml-model-metro-1.6.4.jar
-pmml-python-1.1.14.jar
-pmml-sklearn-1.7.29.jar
-pmml-sklearn-extension-1.7.29.jar
-pmml-sklearn-h2o-1.7.29.jar
-pmml-sklearn-lightgbm-1.7.29.jar
-pmml-sklearn-statsmodels-1.7.29.jar
-pmml-sklearn-xgboost-1.7.29.jar
-pmml-statsmodels-1.0.3.jar
+pmml-python-1.1.15.jar
+pmml-sklearn-1.7.30.jar
+pmml-sklearn-extension-1.7.30.jar
+pmml-sklearn-h2o-1.7.30.jar
+pmml-sklearn-lightgbm-1.7.30.jar
+pmml-sklearn-statsmodels-1.7.30.jar
+pmml-sklearn-xgboost-1.7.30.jar
+pmml-statsmodels-1.0.4.jar
 pmml-xgboost-1.7.3.jar
 serpent-1.40.jar
 slf4j-api-1.7.36.jar
 slf4j-jdk14-1.7.36.jar
 ubjson-0.1.8.jar
 ubjson-gson-0.1.8.jar
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.29.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.30.jar`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,69 +1,68 @@
-Zip file size: 84309 bytes, number of entries: 67
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 mlxtend/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 mlxtend/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 pycaret/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 pycaret/preprocess/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 tpot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 tpot/builtins/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 optbinning/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 optbinning/scorecard/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 imblearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 category_encoders/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklego/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklego/meta/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklego/preprocessing/
--rw-rw-r--  2.0 unx      913 b- defN 23-Jun-06 10:35 mlxtend/preprocessing/DenseTransformer.class
--rw-rw-r--  2.0 unx     4244 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-06 10:35 pycaret/preprocess/FixImbalancer.class
--rw-rw-r--  2.0 unx     2818 b- defN 23-Jun-06 10:35 pycaret/preprocess/RemoveMulticollinearity.class
--rw-rw-r--  2.0 unx      907 b- defN 23-Jun-06 10:35 pycaret/preprocess/CleanColumnNames.class
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-06 10:35 pycaret/preprocess/RareCategoryGrouping.class
--rw-rw-r--  2.0 unx     7434 b- defN 23-Jun-06 10:35 pycaret/preprocess/TransformerWrapper.class
--rw-rw-r--  2.0 unx     4951 b- defN 23-Jun-06 10:35 pycaret/preprocess/TransformerWrapperWithInverse.class
--rw-rw-r--  2.0 unx      720 b- defN 23-Jun-06 10:35 tpot/builtins/StackingEstimator$1.class
--rw-rw-r--  2.0 unx     4530 b- defN 23-Jun-06 10:35 tpot/builtins/StackingEstimator.class
--rw-rw-r--  2.0 unx     2433 b- defN 23-Jun-06 10:35 optbinning/BinnedFeature.class
--rw-rw-r--  2.0 unx     8560 b- defN 23-Jun-06 10:35 optbinning/scorecard/Scorecard.class
--rw-rw-r--  2.0 unx     2133 b- defN 23-Jun-06 10:35 optbinning/OptimalBinningUtil.class
--rw-rw-r--  2.0 unx     6372 b- defN 23-Jun-06 10:35 optbinning/BinningProcess.class
--rw-rw-r--  2.0 unx     2274 b- defN 23-Jun-06 10:35 optbinning/ContinuousOptimalBinning.class
--rw-rw-r--  2.0 unx     3917 b- defN 23-Jun-06 10:35 optbinning/MulticlassOptimalBinning.class
--rw-rw-r--  2.0 unx     1242 b- defN 23-Jun-06 10:35 optbinning/BinningProcess$1.class
--rw-rw-r--  2.0 unx    14050 b- defN 23-Jun-06 10:35 optbinning/OptimalBinning.class
--rw-rw-r--  2.0 unx      860 b- defN 23-Jun-06 10:35 imblearn/Sampler.class
--rw-rw-r--  2.0 unx     1916 b- defN 23-Jun-06 10:35 category_encoders/MapEncoder.class
--rw-rw-r--  2.0 unx     8449 b- defN 23-Jun-06 10:35 category_encoders/MapFeature.class
--rw-rw-r--  2.0 unx      527 b- defN 23-Jun-06 10:35 category_encoders/TargetEncoder.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Jun-06 10:35 category_encoders/CountEncoder$1.class
--rw-rw-r--  2.0 unx      515 b- defN 23-Jun-06 10:35 category_encoders/WOEEncoder.class
--rw-rw-r--  2.0 unx     9124 b- defN 23-Jun-06 10:35 category_encoders/MeanEncoder.class
--rw-rw-r--  2.0 unx     8520 b- defN 23-Jun-06 10:35 category_encoders/CountEncoder.class
--rw-rw-r--  2.0 unx    12815 b- defN 23-Jun-06 10:35 category_encoders/BaseNFeature.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-06 10:35 category_encoders/MeanEncoder$2.class
--rw-rw-r--  2.0 unx     1481 b- defN 23-Jun-06 10:35 category_encoders/OrdinalMapEncoder$1.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-Jun-06 10:35 category_encoders/MeanEncoder$1.class
--rw-rw-r--  2.0 unx     2119 b- defN 23-Jun-06 10:35 category_encoders/OrdinalEncoder$Mapping.class
--rw-rw-r--  2.0 unx     1323 b- defN 23-Jun-06 10:35 category_encoders/LeaveOneOutEncoder$1.class
--rw-rw-r--  2.0 unx     7967 b- defN 23-Jun-06 10:35 category_encoders/OrdinalMapEncoder.class
--rw-rw-r--  2.0 unx     9241 b- defN 23-Jun-06 10:35 category_encoders/BaseNEncoder.class
--rw-rw-r--  2.0 unx     1334 b- defN 23-Jun-06 10:35 category_encoders/BinaryEncoder.class
--rw-rw-r--  2.0 unx     3547 b- defN 23-Jun-06 10:35 category_encoders/OneHotEncoder.class
--rw-rw-r--  2.0 unx     1325 b- defN 23-Jun-06 10:35 category_encoders/CatBoostEncoder.class
--rw-rw-r--  2.0 unx     2062 b- defN 23-Jun-06 10:35 category_encoders/CategoryEncoderUtil.class
--rw-rw-r--  2.0 unx     1564 b- defN 23-Jun-06 10:35 category_encoders/OrdinalEncoder$1.class
--rw-rw-r--  2.0 unx     1047 b- defN 23-Jun-06 10:35 category_encoders/LeaveOneOutEncoder.class
--rw-rw-r--  2.0 unx     4690 b- defN 23-Jun-06 10:35 category_encoders/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      742 b- defN 23-Jun-06 10:35 category_encoders/MeanEncoder$MeanFunction.class
--rw-rw-r--  2.0 unx     1378 b- defN 23-Jun-06 10:35 category_encoders/CatBoostEncoder$1.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-06 10:35 category_encoders/CategoryEncoder.class
--rw-rw-r--  2.0 unx      725 b- defN 23-Jun-06 10:35 sklego/meta/EstimatorTransformer$1.class
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-06 10:35 sklego/meta/EstimatorTransformer.class
--rw-rw-r--  2.0 unx      920 b- defN 23-Jun-06 10:35 sklego/preprocessing/IdentityTransformer.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-extension/
--rw-rw-r--  2.0 unx     1226 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
--rw-rw-r--  2.0 unx      118 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
-67 files, 171531 bytes uncompressed, 74743 bytes compressed:  56.4%
+Zip file size: 83162 bytes, number of entries: 66
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 mlxtend/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 mlxtend/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 pycaret/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 pycaret/preprocess/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 tpot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 tpot/builtins/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 optbinning/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 optbinning/scorecard/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 imblearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 category_encoders/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklego/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklego/meta/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklego/preprocessing/
+-rw-rw-r--  2.0 unx      913 b- defN 23-Jun-19 22:03 mlxtend/preprocessing/DenseTransformer.class
+-rw-rw-r--  2.0 unx     4244 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-19 22:03 pycaret/preprocess/FixImbalancer.class
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Jun-19 22:03 pycaret/preprocess/RemoveMulticollinearity.class
+-rw-rw-r--  2.0 unx      907 b- defN 23-Jun-19 22:03 pycaret/preprocess/CleanColumnNames.class
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-19 22:03 pycaret/preprocess/RareCategoryGrouping.class
+-rw-rw-r--  2.0 unx     7434 b- defN 23-Jun-19 22:03 pycaret/preprocess/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     4951 b- defN 23-Jun-19 22:03 pycaret/preprocess/TransformerWrapperWithInverse.class
+-rw-rw-r--  2.0 unx      720 b- defN 23-Jun-19 22:03 tpot/builtins/StackingEstimator$1.class
+-rw-rw-r--  2.0 unx     4530 b- defN 23-Jun-19 22:03 tpot/builtins/StackingEstimator.class
+-rw-rw-r--  2.0 unx     2433 b- defN 23-Jun-19 22:03 optbinning/BinnedFeature.class
+-rw-rw-r--  2.0 unx     8333 b- defN 23-Jun-19 22:03 optbinning/scorecard/Scorecard.class
+-rw-rw-r--  2.0 unx     2133 b- defN 23-Jun-19 22:03 optbinning/OptimalBinningUtil.class
+-rw-rw-r--  2.0 unx     6372 b- defN 23-Jun-19 22:03 optbinning/BinningProcess.class
+-rw-rw-r--  2.0 unx     2274 b- defN 23-Jun-19 22:03 optbinning/ContinuousOptimalBinning.class
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Jun-19 22:03 optbinning/MulticlassOptimalBinning.class
+-rw-rw-r--  2.0 unx     1242 b- defN 23-Jun-19 22:03 optbinning/BinningProcess$1.class
+-rw-rw-r--  2.0 unx    14050 b- defN 23-Jun-19 22:03 optbinning/OptimalBinning.class
+-rw-rw-r--  2.0 unx      860 b- defN 23-Jun-19 22:03 imblearn/Sampler.class
+-rw-rw-r--  2.0 unx     1916 b- defN 23-Jun-19 22:03 category_encoders/MapEncoder.class
+-rw-rw-r--  2.0 unx     8449 b- defN 23-Jun-19 22:03 category_encoders/MapFeature.class
+-rw-rw-r--  2.0 unx      527 b- defN 23-Jun-19 22:03 category_encoders/TargetEncoder.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Jun-19 22:03 category_encoders/CountEncoder$1.class
+-rw-rw-r--  2.0 unx      515 b- defN 23-Jun-19 22:03 category_encoders/WOEEncoder.class
+-rw-rw-r--  2.0 unx     8474 b- defN 23-Jun-19 22:03 category_encoders/MeanEncoder.class
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Jun-19 22:03 category_encoders/CountEncoder.class
+-rw-rw-r--  2.0 unx    12815 b- defN 23-Jun-19 22:03 category_encoders/BaseNFeature.class
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Jun-19 22:03 category_encoders/OrdinalMapEncoder$1.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-Jun-19 22:03 category_encoders/MeanEncoder$1.class
+-rw-rw-r--  2.0 unx     2119 b- defN 23-Jun-19 22:03 category_encoders/OrdinalEncoder$Mapping.class
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Jun-19 22:03 category_encoders/LeaveOneOutEncoder$1.class
+-rw-rw-r--  2.0 unx     7967 b- defN 23-Jun-19 22:03 category_encoders/OrdinalMapEncoder.class
+-rw-rw-r--  2.0 unx     9241 b- defN 23-Jun-19 22:03 category_encoders/BaseNEncoder.class
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Jun-19 22:03 category_encoders/BinaryEncoder.class
+-rw-rw-r--  2.0 unx     3547 b- defN 23-Jun-19 22:03 category_encoders/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     1325 b- defN 23-Jun-19 22:03 category_encoders/CatBoostEncoder.class
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Jun-19 22:03 category_encoders/CategoryEncoderUtil.class
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Jun-19 22:03 category_encoders/OrdinalEncoder$1.class
+-rw-rw-r--  2.0 unx     1047 b- defN 23-Jun-19 22:03 category_encoders/LeaveOneOutEncoder.class
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Jun-19 22:03 category_encoders/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jun-19 22:03 category_encoders/MeanEncoder$MeanFunction.class
+-rw-rw-r--  2.0 unx     1378 b- defN 23-Jun-19 22:03 category_encoders/CatBoostEncoder$1.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-19 22:03 category_encoders/CategoryEncoder.class
+-rw-rw-r--  2.0 unx      725 b- defN 23-Jun-19 22:03 sklego/meta/EstimatorTransformer$1.class
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-19 22:03 sklego/meta/EstimatorTransformer.class
+-rw-rw-r--  2.0 unx      920 b- defN 23-Jun-19 22:03 sklego/preprocessing/IdentityTransformer.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/
+-rw-rw-r--  2.0 unx     1226 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
+-rw-rw-r--  2.0 unx      118 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
+66 files, 169531 bytes uncompressed, 73746 bytes compressed:  56.5%
```

#### zipnote «TEMP»/diffoscope_rvr563yz_/tmprwa58s0g_.zip

```diff
@@ -120,17 +120,14 @@
 
 Filename: category_encoders/CountEncoder.class
 Comment: 
 
 Filename: category_encoders/BaseNFeature.class
 Comment: 
 
-Filename: category_encoders/MeanEncoder$2.class
-Comment: 
-
 Filename: category_encoders/OrdinalMapEncoder$1.class
 Comment: 
 
 Filename: category_encoders/MeanEncoder$1.class
 Comment: 
 
 Filename: category_encoders/OrdinalEncoder$Mapping.class
```

#### optbinning/scorecard/Scorecard.class

##### procyon -ec {}

```diff
@@ -3,23 +3,23 @@
 
 import java.util.stream.Collector;
 import java.util.stream.Collectors;
 import org.dmg.pmml.DataType;
 import numpy.DTypeUtil;
 import java.util.Iterator;
 import org.jpmml.python.HasArray;
+import pandas.core.Index;
 import pandas.core.BlockManager;
 import pandas.core.DataFrame;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.scorecard.Attribute;
 import org.dmg.pmml.Predicate;
 import org.dmg.pmml.scorecard.Characteristic;
 import optbinning.BinnedFeature;
 import org.dmg.pmml.scorecard.Characteristics;
-import pandas.core.Index;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.Label;
 import optbinning.BinningProcess;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
@@ -67,21 +67,15 @@
         return estimator.encode(schema);
     }
     
     private org.dmg.pmml.scorecard.Scorecard encodeScorecard(final Schema schema) {
         final DataFrame dfScorecard = this.getDFScorecard();
         final Number intercept = this.getIntercept();
         final BlockManager data = dfScorecard.getData();
-        final List<Index> axes = data.getAxesArray();
-        if (axes.size() != 2) {
-            throw new IllegalArgumentException();
-        }
-        final Index columnAxis = (Index)axes.get(0);
-        final List<?> columnValues = columnAxis.getArrayContent();
-        final Index rowAxis = (Index)axes.get(1);
+        final Index rowAxis = data.getRowAxis();
         final List<?> rowValues = rowAxis.getArrayContent();
         final List<HasArray> blockValues = data.getBlockValues();
         final Label label = schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
         final Characteristics characteristics = new Characteristics();
         final HasArray pointBlockValues = getPoints(blockValues);
         List<?> pointValues = pointBlockValues.getArrayContent();
```

#### category_encoders/MeanEncoder.class

##### procyon -ec {}

```diff
@@ -1,18 +1,17 @@
 
 package category_encoders;
 
 import numpy.core.ScalarUtil;
+import pandas.core.Index;
 import pandas.core.BlockManager;
-import pandas.core.SingleBlockManager;
 import org.jpmml.converter.CMatrixUtil;
 import com.google.common.collect.Iterables;
 import org.jpmml.python.HasArray;
 import java.util.Arrays;
-import pandas.core.Index;
 import pandas.core.DataFrame;
 import java.util.Map;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.ModelEncoder;
 import org.jpmml.converter.Decorator;
 import org.dmg.pmml.Field;
 import org.jpmml.converter.InvalidValueDecorator;
@@ -153,23 +152,17 @@
     
     public Double getMean() {
         return ValueUtil.asDouble(this.getNumber("_mean"));
     }
     
     private static Series toMeanSeries(final DataFrame dataFrame, final MeanEncoder.MeanFunction function) {
         final BlockManager data = dataFrame.getData();
-        final List<Index> axes = data.getAxesArray();
-        if (axes.size() != 2) {
-            throw new IllegalArgumentException();
-        }
-        final Index columnAxis = (Index)axes.get(0);
-        final List<?> columnValues = columnAxis.getArrayContent();
-        final Index rowAxis = (Index)axes.get(1);
-        final List<?> rowValues = rowAxis.getArrayContent();
-        if (!Arrays.asList("sum", "count").equals(columnValues)) {
+        final Index columnAxis = data.getColumnAxis();
+        final Index rowAxis = data.getRowAxis();
+        if (!Arrays.asList("sum", "count").equals(columnAxis.getValues())) {
             throw new IllegalArgumentException();
         }
         final List<HasArray> blockValues = data.getBlockValues();
         List<?> sumValues;
         List<?> countValues;
         if (blockValues.size() == 2) {
             sumValues = ((HasArray)blockValues.get(0)).getArrayContent();
@@ -185,16 +178,10 @@
         final List<Double> meanValues = new ArrayList<Double>();
         for (int i = 0; i < sumValues.size(); ++i) {
             final Double sum = ValueUtil.asDouble((Number)sumValues.get(i));
             final Integer count = ValueUtil.asInteger((Number)countValues.get(i));
             final Double mean = function.apply(sum, count);
             meanValues.add(mean);
         }
-        final HasArray hasArray = (HasArray)new MeanEncoder.MeanEncoder$2((List)meanValues);
-        final SingleBlockManager singleBlockManager = new SingleBlockManager();
-        singleBlockManager.setOnlyBlockItem((Index)axes.get(1));
-        singleBlockManager.setOnlyBlockValue(hasArray);
-        final Series result = new Series();
-        result.setBlockManager(singleBlockManager);
-        return result;
+        return SeriesUtil.createSeries(rowAxis, (List)meanValues);
     }
 }
```

#### category_encoders/MeanEncoder$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum be697dbfb71c9b6c970ea68f47af46abe6331bfa4563f3a6513e02af7a742be2
+  SHA-256 checksum 009cf6221b6faa809439ebaba2757a635ef6bfb5937118bc1866a3d425d00305
   Compiled from "MeanEncoder.java"
 class category_encoders.MeanEncoder$1 extends category_encoders.MapFeature
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #7                          // category_encoders/MeanEncoder$1
   super_class: #8                         // category_encoders/MapFeature
@@ -79,15 +79,15 @@
          7: aload_3
          8: aload         4
         10: aload         5
         12: aload         6
         14: invokespecial #2                  // Method category_encoders/MapFeature."<init>":(Lorg/jpmml/converter/PMMLEncoder;Lorg/jpmml/converter/Feature;Ljava/util/Map;Ljava/lang/Object;Ljava/lang/Number;)V
         17: return
       LineNumberTable:
-        line 117: 0
+        line 116: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      18     0  this   Lcategory_encoders/MeanEncoder$1;
             0      18     1 this$0   Lcategory_encoders/MeanEncoder;
             0      18     2 encoder   Lorg/jpmml/converter/PMMLEncoder;
             0      18     3 feature   Lorg/jpmml/converter/Feature;
             0      18     4 mapping   Ljava/util/Map;
@@ -113,15 +113,15 @@
         16: iconst_0
         17: aload_0
         18: invokevirtual #5                  // Method getName:()Ljava/lang/String;
         21: aastore
         22: invokevirtual #6                  // Method category_encoders/MeanEncoder.createFieldName:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
         25: areturn
       LineNumberTable:
-        line 121: 0
+        line 120: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      26     0  this   Lcategory_encoders/MeanEncoder$1;
 }
 SourceFile: "MeanEncoder.java"
 EnclosingMethod: #36.#37                // category_encoders.MeanEncoder.encodeFeatures
 InnerClasses:
```

#### category_encoders/MeanEncoder$MeanFunction.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 4cc85760962ec72911226e2a361869f3d73449d3e75f445e5b24307845c18d25
+  SHA-256 checksum 56f9fd4a0f084aaf725fd960eaf1a8ea62b1838a544f77679ef2dbddc7b7647c
   Compiled from "MeanEncoder.java"
 public interface category_encoders.MeanEncoder$MeanFunction extends java.util.function.BiFunction<java.lang.Double, java.lang.Integer, java.lang.Double>
   minor version: 0
   major version: 52
   flags: (0x0601) ACC_PUBLIC, ACC_INTERFACE, ACC_ABSTRACT
   this_class: #4                          // category_encoders/MeanEncoder$MeanFunction
   super_class: #5                         // java/lang/Object
@@ -50,15 +50,15 @@
          1: aload_1
          2: checkcast     #1                  // class java/lang/Double
          5: aload_2
          6: checkcast     #2                  // class java/lang/Integer
          9: invokeinterface #3,  3            // InterfaceMethod apply:(Ljava/lang/Double;Ljava/lang/Integer;)Ljava/lang/Double;
         14: areturn
       LineNumberTable:
-        line 222: 0
+        line 188: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lcategory_encoders/MeanEncoder$MeanFunction;
 }
 Signature: #18                          // Ljava/lang/Object;Ljava/util/function/BiFunction<Ljava/lang/Double;Ljava/lang/Integer;Ljava/lang/Double;>;
 SourceFile: "MeanEncoder.java"
 InnerClasses:
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.29</version>
+    <version>1.7.30</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-extension</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn extensions converter</name>
   <description>JPMML Scikit-Learn extension packages to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Tue Jun 06 10:35:43 EEST 2023
-version=1.7.29
+#Mon Jun 19 22:03:16 EEST 2023
+version=1.7.30
 groupId=org.jpmml
 artifactId=pmml-sklearn-extension
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar`

 * *Files 22% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5704 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Jun-06 10:41 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 com/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 com/sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 META-INF/maven/com.sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:41 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
--rw-rw-r--  2.0 unx     3741 b- defN 23-Jun-06 10:41 com/sklearn2pmml/Main.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-Jun-06 10:41 com/sklearn2pmml/Main$1.class
--rw-rw-r--  2.0 unx     7844 b- defN 23-Jun-06 10:40 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
--rw-rw-r--  2.0 unx       70 b- defN 23-Jun-06 10:41 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
-11 files, 13013 bytes uncompressed, 4228 bytes compressed:  67.5%
+Zip file size: 5703 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-19 22:18 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 com/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 com/sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 META-INF/maven/com.sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
+-rw-rw-r--  2.0 unx     3741 b- defN 23-Jun-19 22:18 com/sklearn2pmml/Main.class
+-rw-rw-r--  2.0 unx     1200 b- defN 23-Jun-19 22:18 com/sklearn2pmml/Main$1.class
+-rw-rw-r--  2.0 unx     7844 b- defN 23-Jun-19 22:18 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
+-rw-rw-r--  2.0 unx       70 b- defN 23-Jun-19 22:18 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
+11 files, 13013 bytes uncompressed, 4227 bytes compressed:  67.5%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: SkLearn2PMML package
-Implementation-Version: 0.93.0
+Implementation-Version: 0.94.0
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.2.2
```

#### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

##### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

```diff
@@ -24,15 +24,15 @@
     <tag>HEAD</tag>
   </scm>
   <issueManagement>
     <system>GitHub</system>
     <url>https://github.com/jpmml/sklearn2pmml/issues</url>
   </issueManagement>
   <properties>
-    <jpmml-sklearn.version>1.7.29</jpmml-sklearn.version>
+    <jpmml-sklearn.version>1.7.30</jpmml-sklearn.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>org.jpmml</groupId>
       <artifactId>pmml-sklearn</artifactId>
       <version>${jpmml-sklearn.version}</version>
       <exclusions>
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-h2o-1.2.6.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-h2o-1.2.7.jar`

 * *Files 17% similar despite different names*

#### zipinfo {}

```diff
@@ -1,39 +1,39 @@
-Zip file size: 46363 bytes, number of entries: 37
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/
--rw-r--r--  2.0 unx      154 b- defN 23-May-30 22:11 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/services/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 org/jpmml/h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 22:11 org/jpmml/h2o/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 22:11 META-INF/maven/org.jpmml/pmml-h2o/
--rw-rw-r--  2.0 unx       32 b- defN 23-May-30 22:11 META-INF/services/hex.genmodel.ModelMojoReader
--rw-rw-r--  2.0 unx     7639 b- defN 23-May-30 22:11 org/jpmml/h2o/GbmMojoModelConverter.class
--rw-rw-r--  2.0 unx     1798 b- defN 23-May-30 22:11 org/jpmml/h2o/IsolationForestMojoModelConverter$1.class
--rw-rw-r--  2.0 unx     4088 b- defN 23-May-30 22:11 org/jpmml/h2o/XGBoostMojoModelConverter.class
--rw-rw-r--  2.0 unx     2013 b- defN 23-May-30 22:11 org/jpmml/h2o/testing/H2OEncoderBatchTest.class
--rw-rw-r--  2.0 unx     2897 b- defN 23-May-30 22:11 org/jpmml/h2o/testing/H2OEncoderBatch.class
--rw-rw-r--  2.0 unx     1591 b- defN 23-May-30 22:11 org/jpmml/h2o/testing/H2OEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     8548 b- defN 23-May-30 22:11 org/jpmml/h2o/GlmMojoModelBaseConverter.class
--rw-rw-r--  2.0 unx     4387 b- defN 23-May-30 22:11 org/jpmml/h2o/IsolationForestMojoModelConverter.class
--rw-rw-r--  2.0 unx     3400 b- defN 23-May-30 22:11 org/jpmml/h2o/XGBoostMojoModelConverter$1.class
--rw-rw-r--  2.0 unx     4469 b- defN 23-May-30 22:11 org/jpmml/h2o/GlmMojoModelConverter.class
--rw-rw-r--  2.0 unx      664 b- defN 23-May-30 22:11 org/jpmml/h2o/H2OEncoder$1.class
--rw-rw-r--  2.0 unx     1344 b- defN 23-May-30 22:11 org/jpmml/h2o/MojoModelUtil$1.class
--rw-rw-r--  2.0 unx     3560 b- defN 23-May-30 22:11 org/jpmml/h2o/H2OEncoder.class
--rw-rw-r--  2.0 unx     1117 b- defN 23-May-30 22:11 org/jpmml/h2o/XGBoostMojoModel.class
--rw-rw-r--  2.0 unx    12570 b- defN 23-May-30 22:11 org/jpmml/h2o/SharedTreeMojoModelConverter.class
--rw-rw-r--  2.0 unx     4030 b- defN 23-May-30 22:11 org/jpmml/h2o/GlmMultinomialMojoModelConverter.class
--rw-rw-r--  2.0 unx     1586 b- defN 23-May-30 22:11 org/jpmml/h2o/XGBoostMojoReader.class
--rw-rw-r--  2.0 unx     1412 b- defN 23-May-30 22:11 org/jpmml/h2o/ImputerUtil.class
--rw-rw-r--  2.0 unx     7050 b- defN 23-May-30 22:11 org/jpmml/h2o/DrfMojoModelConverter.class
--rw-rw-r--  2.0 unx     5387 b- defN 23-May-30 22:11 org/jpmml/h2o/Converter.class
--rw-rw-r--  2.0 unx     1840 b- defN 23-May-30 22:11 org/jpmml/h2o/MojoModelUtil.class
--rw-rw-r--  2.0 unx     3179 b- defN 23-May-30 22:11 org/jpmml/h2o/GlmMojoModelBaseConverter$1.class
--rw-rw-r--  2.0 unx     7520 b- defN 23-May-30 22:11 org/jpmml/h2o/StackedEnsembleMojoModelConverter.class
--rw-rw-r--  2.0 unx     2304 b- defN 23-May-30 22:11 org/jpmml/h2o/ConverterFactory.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-May-30 22:11 META-INF/maven/org.jpmml/pmml-h2o/pom.xml
--rw-rw-r--  2.0 unx       52 b- defN 23-May-30 22:11 META-INF/maven/org.jpmml/pmml-h2o/pom.properties
-37 files, 96583 bytes uncompressed, 40905 bytes compressed:  57.6%
+Zip file size: 46831 bytes, number of entries: 37
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-15 21:20 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/services/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 org/jpmml/h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 org/jpmml/h2o/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/maven/org.jpmml/pmml-h2o/
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jun-15 21:20 META-INF/services/hex.genmodel.ModelMojoReader
+-rw-rw-r--  2.0 unx     7803 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GbmMojoModelConverter.class
+-rw-rw-r--  2.0 unx     1798 b- defN 23-Jun-15 21:20 org/jpmml/h2o/IsolationForestMojoModelConverter$1.class
+-rw-rw-r--  2.0 unx     4088 b- defN 23-Jun-15 21:20 org/jpmml/h2o/XGBoostMojoModelConverter.class
+-rw-rw-r--  2.0 unx     2013 b- defN 23-Jun-15 21:20 org/jpmml/h2o/testing/H2OEncoderBatchTest.class
+-rw-rw-r--  2.0 unx     2897 b- defN 23-Jun-15 21:20 org/jpmml/h2o/testing/H2OEncoderBatch.class
+-rw-rw-r--  2.0 unx     1591 b- defN 23-Jun-15 21:20 org/jpmml/h2o/testing/H2OEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     8548 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GlmMojoModelBaseConverter.class
+-rw-rw-r--  2.0 unx     4555 b- defN 23-Jun-15 21:20 org/jpmml/h2o/IsolationForestMojoModelConverter.class
+-rw-rw-r--  2.0 unx     3400 b- defN 23-Jun-15 21:20 org/jpmml/h2o/XGBoostMojoModelConverter$1.class
+-rw-rw-r--  2.0 unx     4469 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GlmMojoModelConverter.class
+-rw-rw-r--  2.0 unx      664 b- defN 23-Jun-15 21:20 org/jpmml/h2o/H2OEncoder$1.class
+-rw-rw-r--  2.0 unx     1344 b- defN 23-Jun-15 21:20 org/jpmml/h2o/MojoModelUtil$1.class
+-rw-rw-r--  2.0 unx     3560 b- defN 23-Jun-15 21:20 org/jpmml/h2o/H2OEncoder.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Jun-15 21:20 org/jpmml/h2o/XGBoostMojoModel.class
+-rw-rw-r--  2.0 unx    13590 b- defN 23-Jun-15 21:20 org/jpmml/h2o/SharedTreeMojoModelConverter.class
+-rw-rw-r--  2.0 unx     4030 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GlmMultinomialMojoModelConverter.class
+-rw-rw-r--  2.0 unx     1586 b- defN 23-Jun-15 21:20 org/jpmml/h2o/XGBoostMojoReader.class
+-rw-rw-r--  2.0 unx     1412 b- defN 23-Jun-15 21:20 org/jpmml/h2o/ImputerUtil.class
+-rw-rw-r--  2.0 unx     7050 b- defN 23-Jun-15 21:20 org/jpmml/h2o/DrfMojoModelConverter.class
+-rw-rw-r--  2.0 unx     4968 b- defN 23-Jun-15 21:20 org/jpmml/h2o/Converter.class
+-rw-rw-r--  2.0 unx     1840 b- defN 23-Jun-15 21:20 org/jpmml/h2o/MojoModelUtil.class
+-rw-rw-r--  2.0 unx     3179 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GlmMojoModelBaseConverter$1.class
+-rw-rw-r--  2.0 unx     7520 b- defN 23-Jun-15 21:20 org/jpmml/h2o/StackedEnsembleMojoModelConverter.class
+-rw-rw-r--  2.0 unx     2304 b- defN 23-Jun-15 21:20 org/jpmml/h2o/ConverterFactory.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Jun-15 21:20 META-INF/maven/org.jpmml/pmml-h2o/pom.xml
+-rw-rw-r--  2.0 unx       52 b- defN 23-Jun-15 21:20 META-INF/maven/org.jpmml/pmml-h2o/pom.properties
+37 files, 97516 bytes uncompressed, 41373 bytes compressed:  57.6%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-H2O library
-Implementation-Version: 1.2.6
+Implementation-Version: 1.2.7
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### org/jpmml/h2o/GbmMojoModelConverter.class

##### procyon -ec {}

```diff
@@ -1,10 +1,11 @@
 
 package org.jpmml.h2o;
 
+import org.dmg.pmml.tree.Node;
 import org.dmg.pmml.tree.TreeModel;
 import org.jpmml.converter.FieldNameUtil;
 import org.jpmml.converter.CMatrixUtil;
 import java.util.ArrayList;
 import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.regression.RegressionModel;
 import org.jpmml.converter.Transformation;
@@ -74,8 +75,11 @@
                 pmmlModel2.setOutput(ModelUtil.createPredictedOutput(FieldNameUtil.create("gbmValue", new Object[] { categoricalLabel.getValue(i) }), OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
                 models.add(pmmlModel2);
             }
             return (Model)MiningModelUtil.createClassification((List)models, RegressionModel.NormalizationMethod.SOFTMAX, true, schema);
         }
         throw new IllegalArgumentException("Distribution family " + model._family + " is not supported");
     }
+    
+    protected void ensureScore(final Node node, final double score) {
+    }
 }
```

#### org/jpmml/h2o/IsolationForestMojoModelConverter$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 02a2af292d60653d0ec7765a7c1f9ff278da6609181029395d8a4503af33afab
+  SHA-256 checksum 5cd63c6fbbc1541bfce92cd875a25144aceac7c2b85141e6b76fe09f7e732ff7
   Compiled from "IsolationForestMojoModelConverter.java"
 class org.jpmml.h2o.IsolationForestMojoModelConverter$1 extends org.jpmml.converter.transformations.AbstractTransformation
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // org/jpmml/h2o/IsolationForestMojoModelConverter$1
   super_class: #16                        // org/jpmml/converter/transformations/AbstractTransformation
@@ -122,43 +122,43 @@
         15: aload_0
         16: iload         4
         18: putfield      #4                  // Field val$minPathLength:I
         21: aload_0
         22: invokespecial #5                  // Method org/jpmml/converter/transformations/AbstractTransformation."<init>":()V
         25: return
       LineNumberTable:
-        line 60: 0
+        line 61: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      26     0  this   Lorg/jpmml/h2o/IsolationForestMojoModelConverter$1;
             0      26     1 this$0   Lorg/jpmml/h2o/IsolationForestMojoModelConverter;
 
   public java.lang.String getName(java.lang.String);
     descriptor: (Ljava/lang/String;)Ljava/lang/String;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=2, args_size=2
          0: ldc           #6                  // String anomalyScore
          2: areturn
       LineNumberTable:
-        line 64: 0
+        line 65: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       3     0  this   Lorg/jpmml/h2o/IsolationForestMojoModelConverter$1;
             0       3     1  name   Ljava/lang/String;
 
   public boolean isFinalResult();
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: iconst_1
          1: ireturn
       LineNumberTable:
-        line 69: 0
+        line 70: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lorg/jpmml/h2o/IsolationForestMojoModelConverter$1;
 
   public org.dmg.pmml.Expression createExpression(org.dmg.pmml.FieldRef);
     descriptor: (Lorg/dmg/pmml/FieldRef;)Lorg/dmg/pmml/Expression;
     flags: (0x0001) ACC_PUBLIC
@@ -206,15 +206,15 @@
         69: ddiv
         70: invokestatic  #12                 // Method java/lang/Double.valueOf:(D)Ljava/lang/Double;
         73: invokestatic  #13                 // Method org/jpmml/converter/PMMLUtil.createConstant:(Ljava/lang/Number;)Lorg/dmg/pmml/Constant;
         76: aastore
         77: invokestatic  #14                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         80: areturn
       LineNumberTable:
-        line 74: 0
+        line 75: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      81     0  this   Lorg/jpmml/h2o/IsolationForestMojoModelConverter$1;
             0      81     1 fieldRef   Lorg/dmg/pmml/FieldRef;
 }
 SourceFile: "IsolationForestMojoModelConverter.java"
 EnclosingMethod: #45.#46                // org.jpmml.h2o.IsolationForestMojoModelConverter.encodeModel
```

#### org/jpmml/h2o/IsolationForestMojoModelConverter.class

##### procyon -ec {}

```diff
@@ -1,12 +1,13 @@
 
 package org.jpmml.h2o;
 
 import org.dmg.pmml.Model;
 import hex.genmodel.MojoModel;
+import org.dmg.pmml.tree.Node;
 import org.dmg.pmml.tree.TreeModel;
 import org.jpmml.converter.Transformation;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
 import org.jpmml.converter.Label;
@@ -37,14 +38,17 @@
         }
         final List<TreeModel> treeModels = this.encodeTreeModels(schema);
         final Transformation anomalyScore = (Transformation)new IsolationForestMojoModelConverter.IsolationForestMojoModelConverter$1(this, maxPathLength, (List)treeModels, minPathLength);
         final MiningModel miningModel = new MiningModel(MiningFunction.REGRESSION, ModelUtil.createMiningSchema((Label)null)).setSegmentation(MiningModelUtil.createSegmentation(Segmentation.MultipleModelMethod.AVERAGE, Segmentation.MissingPredictionTreatment.RETURN_MISSING, (List)treeModels)).setOutput(ModelUtil.createPredictedOutput("meanPathLength", OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[] { anomalyScore }));
         return miningModel;
     }
     
+    protected void ensureScore(final Node node, final double score) {
+    }
+    
     public static int getMaxPathLength(final IsolationForestMojoModel model) {
         return (int)getFieldValue(IsolationForestMojoModelConverter.FIELD_MAX_PATH_LENGTH, (MojoModel)model);
     }
     
     public static int getMinPathLength(final IsolationForestMojoModel model) {
         return (int)getFieldValue(IsolationForestMojoModelConverter.FIELD_MIN_PATH_LENGTH, (MojoModel)model);
     }
```

#### org/jpmml/h2o/SharedTreeMojoModelConverter.class

##### procyon -ec {}

```diff
@@ -1,93 +1,96 @@
 
 package org.jpmml.h2o;
 
+import com.google.common.collect.Iterables;
+import org.dmg.pmml.Model;
+import org.dmg.pmml.mining.MiningModel;
+import java.util.function.Function;
+import org.jpmml.converter.ValueUtil;
+import java.util.Objects;
 import org.jpmml.converter.ContinuousFeature;
-import org.dmg.pmml.tree.BranchNode;
+import org.dmg.pmml.tree.CountingBranchNode;
 import org.jpmml.converter.Feature;
 import java.util.Collection;
-import java.util.ArrayList;
 import hex.genmodel.utils.GenmodelBitSet;
 import org.jpmml.converter.CategoricalFeature;
 import org.dmg.pmml.SimplePredicate;
 import hex.genmodel.algos.tree.NaSplitDir;
-import org.dmg.pmml.tree.LeafNode;
+import org.dmg.pmml.tree.CountingLeafNode;
 import org.dmg.pmml.tree.Node;
+import java.util.Map;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.Predicate;
 import org.jpmml.converter.CategoryManager;
 import org.dmg.pmml.True;
-import java.util.concurrent.atomic.AtomicInteger;
 import hex.genmodel.utils.ByteBufferWrapper;
 import org.jpmml.converter.ContinuousLabel;
 import org.dmg.pmml.DataType;
-import com.google.common.collect.Iterables;
-import org.dmg.pmml.Model;
-import org.dmg.pmml.mining.MiningModel;
-import java.util.function.Function;
-import java.util.stream.Collector;
-import java.util.stream.Collectors;
-import java.util.stream.Stream;
+import java.util.ArrayList;
 import org.jpmml.converter.PredicateManager;
 import org.dmg.pmml.tree.TreeModel;
 import java.util.List;
 import org.jpmml.converter.Schema;
 import hex.genmodel.MojoModel;
 import java.lang.reflect.Field;
 import hex.genmodel.algos.tree.SharedTreeMojoModel;
 
 public abstract class SharedTreeMojoModelConverter<M extends SharedTreeMojoModel> extends Converter<M>
 {
     private static final Field FIELD_COMPRESSEDTREES;
+    private static final Field FIELD_COMPRESSEDTREESAUX;
     private static final Field FIELD_NTREEGROUPS;
     private static final Field FIELD_NTREESPERGROUP;
     
     public SharedTreeMojoModelConverter(final M model) {
         super((MojoModel)model);
     }
     
     public List<TreeModel> encodeTreeModels(final Schema schema) {
         final SharedTreeMojoModel model = (SharedTreeMojoModel)this.getModel();
         if (model._mojo_version < 1.2) {
             throw new IllegalArgumentException("Version " + model._mojo_version + " is not supported");
         }
         final byte[][] compressedTrees = getCompressedTrees(model);
+        final byte[][] compressedTreesAux = getCompressedTreesAux(model);
         final PredicateManager predicateManager = new PredicateManager();
-        final List<TreeModel> result = (List<TreeModel>)Stream.of(compressedTrees).map(compressedTree -> encodeTreeModel(compressedTree, predicateManager, schema)).collect((Collector<? super Object, ?, List<TreeModel>>)Collectors.toList());
-        return result;
-    }
-    
-    public static Model encodeTreeEnsemble(final List<TreeModel> treeModels, final Function<List<TreeModel>, MiningModel> ensembleFunction) {
-        if (treeModels.size() == 1) {
-            return (Model)Iterables.getOnlyElement((Iterable)treeModels);
+        final List<TreeModel> result = new ArrayList<TreeModel>();
+        for (int i = 0, max = Math.max(compressedTrees.length, compressedTreesAux.length); i < max; ++i) {
+            final byte[] compressedTree = compressedTrees[i];
+            final byte[] compressedTreeAux = compressedTreesAux[i];
+            final TreeModel treeModel = this.encodeTreeModel(compressedTree, compressedTreeAux, predicateManager, schema);
+            result.add(treeModel);
         }
-        return (Model)ensembleFunction.apply(treeModels);
+        return result;
     }
     
-    public static TreeModel encodeTreeModel(final byte[] compressedTree, final PredicateManager predicateManager, final Schema schema) {
+    public TreeModel encodeTreeModel(final byte[] compressedTree, final byte[] compressedTreeAux, final PredicateManager predicateManager, final Schema schema) {
         final Label label = (Label)new ContinuousLabel(DataType.DOUBLE);
         final ByteBufferWrapper byteBuffer = new ByteBufferWrapper(compressedTree);
-        final AtomicInteger idSequence = new AtomicInteger(1);
-        final Node root = encodeNode(byteBuffer, (Predicate)True.INSTANCE, compressedTree, idSequence, new CategoryManager(), predicateManager, schema);
+        final Map<Integer, SharedTreeMojoModel.AuxInfo> auxInfos = SharedTreeMojoModel.readAuxInfos(compressedTreeAux);
+        final Node root = this.encodeNode(byteBuffer, Integer.valueOf(0), (Predicate)True.INSTANCE, compressedTree, auxInfos, new CategoryManager(), predicateManager, schema);
         final TreeModel treeModel = new TreeModel(MiningFunction.REGRESSION, ModelUtil.createMiningSchema(label), root).setMissingValueStrategy(TreeModel.MissingValueStrategy.DEFAULT_CHILD);
         return treeModel;
     }
     
-    public static Node encodeNode(final ByteBufferWrapper byteBuffer, final Predicate predicate, final byte[] compressedTree, final AtomicInteger idSequence, final CategoryManager categoryManager, final PredicateManager predicateManager, final Schema schema) {
-        final Integer id = nextId(idSequence);
+    public Node encodeNode(final ByteBufferWrapper byteBuffer, final Integer id, final Predicate predicate, final byte[] compressedTree, final Map<Integer, SharedTreeMojoModel.AuxInfo> auxInfos, final CategoryManager categoryManager, final PredicateManager predicateManager, final Schema schema) {
+        final SharedTreeMojoModel.AuxInfo auxInfo = (SharedTreeMojoModel.AuxInfo)auxInfos.get(id);
+        if (auxInfo == null) {
+            throw new IllegalArgumentException();
+        }
         final int nodeType = byteBuffer.get1U();
         final int lmask = nodeType & 0x33;
         final int lmask2 = (nodeType & 0xC0) >> 2;
         final int equal = nodeType & 0xC;
         final int colId = byteBuffer.get2();
         if (colId == 65535) {
             final double score = (double)byteBuffer.get4f();
-            final Node result = (Node)new LeafNode((Object)Double.valueOf(score), predicate).setId((Object)id);
+            final Node result = (Node)new CountingLeafNode((Object)Double.valueOf(score), predicate).setId((Object)id);
             return result;
         }
         final int naSplitDir = byteBuffer.get1U();
         final boolean naVsRest = naSplitDir == NaSplitDir.NAvsREST.value();
         final boolean leftward = naSplitDir == NaSplitDir.NALeft.value() || naSplitDir == NaSplitDir.Left.value();
         final Feature feature = schema.getFeature(colId);
         CategoryManager leftCategoryManager = categoryManager;
@@ -133,27 +136,29 @@
         }
         else {
             final ContinuousFeature continuousFeature = feature.toContinuousFeature();
             final Double splitVal = Double.valueOf(byteBuffer.get4f());
             leftPredicate = predicateManager.createSimplePredicate((Feature)continuousFeature, SimplePredicate.Operator.LESS_THAN, (Object)splitVal);
             rightPredicate = predicateManager.createSimplePredicate((Feature)continuousFeature, SimplePredicate.Operator.GREATER_OR_EQUAL, (Object)splitVal);
         }
+        final Integer leftId = Integer.valueOf(auxInfo.nidL);
         final ByteBufferWrapper leftByteBuffer = new ByteBufferWrapper(compressedTree);
         leftByteBuffer.skip(byteBuffer.position());
         if (lmask <= 3) {
             leftByteBuffer.skip(lmask + 1);
         }
         Node leftChild;
         if ((lmask & 0x10) != 0x0) {
             final double score2 = (double)leftByteBuffer.get4f();
-            leftChild = (Node)new LeafNode((Object)Double.valueOf(score2), leftPredicate).setId((Object)nextId(idSequence));
+            leftChild = (Node)new CountingLeafNode((Object)Double.valueOf(score2), leftPredicate).setId((Object)leftId);
         }
         else {
-            leftChild = encodeNode(leftByteBuffer, leftPredicate, compressedTree, idSequence, leftCategoryManager, predicateManager, schema);
+            leftChild = this.encodeNode(leftByteBuffer, leftId, leftPredicate, compressedTree, auxInfos, leftCategoryManager, predicateManager, schema);
         }
+        final Integer rightId = Integer.valueOf(auxInfo.nidR);
         final ByteBufferWrapper rightByteBuffer = new ByteBufferWrapper(compressedTree);
         rightByteBuffer.skip(byteBuffer.position());
         switch (lmask) {
             case 0: {
                 rightByteBuffer.skip(rightByteBuffer.get1U());
                 break;
             }
@@ -176,42 +181,77 @@
             default: {
                 throw new IllegalArgumentException("Node type " + lmask + " is not supported");
             }
         }
         Node rightChild;
         if ((lmask2 & 0x10) != 0x0) {
             final double score3 = (double)rightByteBuffer.get4f();
-            rightChild = (Node)new LeafNode((Object)Double.valueOf(score3), rightPredicate).setId((Object)nextId(idSequence));
+            rightChild = (Node)new CountingLeafNode((Object)Double.valueOf(score3), rightPredicate).setId((Object)rightId);
         }
         else {
-            rightChild = encodeNode(rightByteBuffer, rightPredicate, compressedTree, idSequence, rightCategoryManager, predicateManager, schema);
+            rightChild = this.encodeNode(rightByteBuffer, rightId, rightPredicate, compressedTree, auxInfos, rightCategoryManager, predicateManager, schema);
+        }
+        this.ensureScore(leftChild, auxInfo.predL);
+        this.ensureScore(rightChild, auxInfo.predR);
+        this.ensureRecordCount(leftChild, auxInfo.weightL);
+        this.ensureRecordCount(rightChild, auxInfo.weightR);
+        final Node result2 = new CountingBranchNode((Object)null, predicate).setId((Object)id).setDefaultChild(leftward ? leftChild.getId() : rightChild.getId()).addNodes(leftChild, rightChild);
+        if (id == 0) {
+            final float weight = auxInfo.weightL + auxInfo.weightR;
+            this.ensureScore(result2, (auxInfo.predL * auxInfo.weightL + auxInfo.predR * auxInfo.weightR) / weight);
+            this.ensureRecordCount(result2, weight);
         }
-        final Node result2 = new BranchNode((Object)null, predicate).setId((Object)id).setDefaultChild(leftward ? leftChild.getId() : rightChild.getId()).addNodes(leftChild, rightChild);
         return result2;
     }
     
+    protected void ensureScore(final Node node, final double score) {
+        if (node.hasScore()) {
+            if (!Objects.equals(node.getScore(), Double.valueOf(score))) {
+                throw new IllegalArgumentException();
+            }
+        }
+        else {
+            node.setScore((Object)Double.valueOf(score));
+        }
+    }
+    
+    protected void ensureRecordCount(final Node node, final double recordCount) {
+        if (node.getRecordCount() != null) {
+            throw new IllegalArgumentException();
+        }
+        node.setRecordCount(ValueUtil.narrow(recordCount));
+    }
+    
+    public static Model encodeTreeEnsemble(final List<TreeModel> treeModels, final Function<List<TreeModel>, MiningModel> ensembleFunction) {
+        if (treeModels.size() == 1) {
+            return (Model)Iterables.getOnlyElement((Iterable)treeModels);
+        }
+        return (Model)ensembleFunction.apply(treeModels);
+    }
+    
     public static byte[][] getCompressedTrees(final SharedTreeMojoModel model) {
         return (byte[][])getFieldValue(SharedTreeMojoModelConverter.FIELD_COMPRESSEDTREES, (MojoModel)model);
     }
     
+    public static byte[][] getCompressedTreesAux(final SharedTreeMojoModel model) {
+        return (byte[][])getFieldValue(SharedTreeMojoModelConverter.FIELD_COMPRESSEDTREESAUX, (MojoModel)model);
+    }
+    
     public static int getNTreeGroups(final SharedTreeMojoModel model) {
         return (int)getFieldValue(SharedTreeMojoModelConverter.FIELD_NTREEGROUPS, (MojoModel)model);
     }
     
     public static int getNTreesPerGroup(final SharedTreeMojoModel model) {
         return (int)getFieldValue(SharedTreeMojoModelConverter.FIELD_NTREESPERGROUP, (MojoModel)model);
     }
     
-    private static Integer nextId(final AtomicInteger id) {
-        return Integer.valueOf(id.getAndIncrement());
-    }
-    
     static {
         try {
             FIELD_COMPRESSEDTREES = SharedTreeMojoModel.class.getDeclaredField("_compressed_trees");
+            FIELD_COMPRESSEDTREESAUX = SharedTreeMojoModel.class.getDeclaredField("_compressed_trees_aux");
             FIELD_NTREEGROUPS = SharedTreeMojoModel.class.getDeclaredField("_ntree_groups");
             FIELD_NTREESPERGROUP = SharedTreeMojoModel.class.getDeclaredField("_ntrees_per_group");
         }
         catch (final ReflectiveOperationException roe) {
             throw new RuntimeException(roe);
         }
     }
```

#### org/jpmml/h2o/Converter.class

##### procyon -ec {}

```diff
@@ -1,23 +1,22 @@
 
 package org.jpmml.h2o;
 
+import java.lang.reflect.Field;
 import java.util.Objects;
 import hex.genmodel.descriptor.ModelDescriptor;
 import org.dmg.pmml.PMML;
 import org.dmg.pmml.DataField;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
-import java.lang.reflect.Field;
 import hex.genmodel.MojoModel;
 
 public abstract class Converter<M extends MojoModel>
 {
     private M model;
-    private static final Field FIELD_MODEL_DESCRIPTOR;
     
     public Converter(final M model) {
         this.model = null;
         this.setModel(model);
     }
     
     public abstract Model encodeModel(final Schema p0);
@@ -45,15 +44,15 @@
     
     public Schema toMojoModelSchema(final Schema schema) {
         return schema;
     }
     
     public PMML encodePMML() {
         final M model = this.getModel();
-        final ModelDescriptor modelDescriptor = getModelDescriptor(model);
+        final ModelDescriptor modelDescriptor = model._modelDescriptor;
         final H2OEncoder encoder = new H2OEncoder();
         Schema schema = this.encodeSchema(encoder);
         schema = this.toMojoModelSchema(schema);
         final Model pmmlModel = this.encodeModel(schema);
         if (modelDescriptor != null) {
             final String algorithmName = pmmlModel.getAlgorithmName();
             if (algorithmName == null) {
@@ -68,18 +67,14 @@
         return this.model;
     }
     
     private void setModel(final M model) {
         this.model = (M)Objects.requireNonNull(model);
     }
     
-    public static ModelDescriptor getModelDescriptor(final MojoModel model) {
-        return (ModelDescriptor)getFieldValue(Converter.FIELD_MODEL_DESCRIPTOR, model);
-    }
-    
     protected static Class<?> getDeclaredClass(final Class<?> clazz, final String name) throws ReflectiveOperationException {
         final String subclassName = clazz.getName() + "$" + name;
         final Class<?>[] declaredClasses;
         final Class<?>[] declaredClazzes = declaredClasses = clazz.getDeclaredClasses();
         for (final Class<?> declaredClazz : declaredClasses) {
             if (subclassName.equals(declaredClazz.getName())) {
                 return declaredClazz;
@@ -99,17 +94,8 @@
             }
             return field.get(object);
         }
         catch (final ReflectiveOperationException roe) {
             throw new RuntimeException(roe);
         }
     }
-    
-    static {
-        try {
-            FIELD_MODEL_DESCRIPTOR = MojoModel.class.getDeclaredField("_modelDescriptor");
-        }
-        catch (final ReflectiveOperationException roe) {
-            throw new RuntimeException(roe);
-        }
-    }
 }
```

#### META-INF/maven/org.jpmml/pmml-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-h2o</artifactId>
-    <version>1.2.6</version>
+    <version>1.2.7</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML H2O.ai converter</name>
   <description>JPMML H2O.ai to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-h2o/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-h2o
 groupId=org.jpmml
-version=1.2.6
+version=1.2.7
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-statsmodels-1.0.3.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,49 +1,44 @@
-Zip file size: 34545 bytes, number of entries: 47
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 11:51 META-INF/
--rw-r--r--  2.0 unx      162 b- defN 23-May-30 11:51 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 org/jpmml/statsmodels/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 org/jpmml/statsmodels/testing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/miscmodels/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/data/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/discrete/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/regression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 statsmodels/genmod/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 scipy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-30 11:50 scipy/stats/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 11:51 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 11:51 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-30 11:51 META-INF/maven/org.jpmml/pmml-statsmodels/
--rw-rw-r--  2.0 unx     2327 b- defN 23-May-30 11:50 META-INF/statsmodels2pmml.properties
--rw-rw-r--  2.0 unx      137 b- defN 23-May-30 11:50 META-INF/python2pmml.properties
--rw-rw-r--  2.0 unx      741 b- defN 23-May-30 11:50 org/jpmml/statsmodels/InterceptFeature.class
--rw-rw-r--  2.0 unx     1959 b- defN 23-May-30 11:50 org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest.class
--rw-rw-r--  2.0 unx     1839 b- defN 23-May-30 11:50 org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2015 b- defN 23-May-30 11:50 org/jpmml/statsmodels/testing/StatsModelsEncoderBatch.class
--rw-rw-r--  2.0 unx     3688 b- defN 23-May-30 11:50 org/jpmml/statsmodels/OrdinalLabel.class
--rw-rw-r--  2.0 unx      671 b- defN 23-May-30 11:50 org/jpmml/statsmodels/StatsModelsEncoder.class
--rw-rw-r--  2.0 unx     9305 b- defN 23-May-30 11:50 statsmodels/miscmodels/OrderedModel.class
--rw-rw-r--  2.0 unx     1425 b- defN 23-May-30 11:50 statsmodels/data/ModelData$Cache.class
--rw-rw-r--  2.0 unx     2653 b- defN 23-May-30 11:50 statsmodels/data/ModelData.class
--rw-rw-r--  2.0 unx     2299 b- defN 23-May-30 11:50 statsmodels/Results.class
--rw-rw-r--  2.0 unx     1706 b- defN 23-May-30 11:50 statsmodels/discrete/BinaryModel.class
--rw-rw-r--  2.0 unx      427 b- defN 23-May-30 11:50 statsmodels/discrete/DiscreteModel.class
--rw-rw-r--  2.0 unx     1731 b- defN 23-May-30 11:50 statsmodels/discrete/Logit.class
--rw-rw-r--  2.0 unx     4417 b- defN 23-May-30 11:50 statsmodels/discrete/MNLogit.class
--rw-rw-r--  2.0 unx     1714 b- defN 23-May-30 11:50 statsmodels/discrete/Poisson.class
--rw-rw-r--  2.0 unx     2941 b- defN 23-May-30 11:50 statsmodels/discrete/MultinomialRegressionModel.class
--rw-rw-r--  2.0 unx      414 b- defN 23-May-30 11:50 statsmodels/discrete/CountModel.class
--rw-rw-r--  2.0 unx     6687 b- defN 23-May-30 11:50 statsmodels/Model.class
--rw-rw-r--  2.0 unx     1110 b- defN 23-May-30 11:50 statsmodels/ResultsWrapper.class
--rw-rw-r--  2.0 unx     1753 b- defN 23-May-30 11:50 statsmodels/regression/LinearRegression.class
--rw-rw-r--  2.0 unx     2395 b- defN 23-May-30 11:50 statsmodels/regression/RegressionModel.class
--rw-rw-r--  2.0 unx     8223 b- defN 23-May-30 11:50 statsmodels/genmod/GLM.class
--rw-rw-r--  2.0 unx      591 b- defN 23-May-30 11:50 statsmodels/genmod/Link.class
--rw-rw-r--  2.0 unx      615 b- defN 23-May-30 11:50 statsmodels/genmod/Family.class
--rw-rw-r--  2.0 unx      388 b- defN 23-May-30 11:50 scipy/stats/RVGeneric.class
--rw-rw-r--  2.0 unx      559 b- defN 23-May-30 11:50 scipy/stats/RVContinuous.class
--rw-rw-r--  2.0 unx     1837 b- defN 23-May-30 11:50 META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml
--rw-rw-r--  2.0 unx       60 b- defN 23-May-30 11:51 META-INF/maven/org.jpmml/pmml-statsmodels/pom.properties
-47 files, 66789 bytes uncompressed, 27967 bytes compressed:  58.1%
+Zip file size: 33104 bytes, number of entries: 42
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 META-INF/
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-11 18:37 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 org/jpmml/statsmodels/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 org/jpmml/statsmodels/testing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 statsmodels/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 statsmodels/miscmodels/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 statsmodels/data/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 statsmodels/discrete/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 statsmodels/regression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 statsmodels/genmod/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 18:37 META-INF/maven/org.jpmml/pmml-statsmodels/
+-rw-rw-r--  2.0 unx     2327 b- defN 23-Jun-11 18:37 META-INF/statsmodels2pmml.properties
+-rw-rw-r--  2.0 unx      741 b- defN 23-Jun-11 18:37 org/jpmml/statsmodels/InterceptFeature.class
+-rw-rw-r--  2.0 unx     1959 b- defN 23-Jun-11 18:37 org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest.class
+-rw-rw-r--  2.0 unx     1839 b- defN 23-Jun-11 18:37 org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2015 b- defN 23-Jun-11 18:37 org/jpmml/statsmodels/testing/StatsModelsEncoderBatch.class
+-rw-rw-r--  2.0 unx     3688 b- defN 23-Jun-11 18:37 org/jpmml/statsmodels/OrdinalLabel.class
+-rw-rw-r--  2.0 unx      671 b- defN 23-Jun-11 18:37 org/jpmml/statsmodels/StatsModelsEncoder.class
+-rw-rw-r--  2.0 unx     9305 b- defN 23-Jun-11 18:37 statsmodels/miscmodels/OrderedModel.class
+-rw-rw-r--  2.0 unx     1425 b- defN 23-Jun-11 18:37 statsmodels/data/ModelData$Cache.class
+-rw-rw-r--  2.0 unx     2338 b- defN 23-Jun-11 18:37 statsmodels/data/ModelData.class
+-rw-rw-r--  2.0 unx     2299 b- defN 23-Jun-11 18:37 statsmodels/Results.class
+-rw-rw-r--  2.0 unx     1706 b- defN 23-Jun-11 18:37 statsmodels/discrete/BinaryModel.class
+-rw-rw-r--  2.0 unx      427 b- defN 23-Jun-11 18:37 statsmodels/discrete/DiscreteModel.class
+-rw-rw-r--  2.0 unx     1731 b- defN 23-Jun-11 18:37 statsmodels/discrete/Logit.class
+-rw-rw-r--  2.0 unx     4417 b- defN 23-Jun-11 18:37 statsmodels/discrete/MNLogit.class
+-rw-rw-r--  2.0 unx     1714 b- defN 23-Jun-11 18:37 statsmodels/discrete/Poisson.class
+-rw-rw-r--  2.0 unx     2941 b- defN 23-Jun-11 18:37 statsmodels/discrete/MultinomialRegressionModel.class
+-rw-rw-r--  2.0 unx      414 b- defN 23-Jun-11 18:37 statsmodels/discrete/CountModel.class
+-rw-rw-r--  2.0 unx     6687 b- defN 23-Jun-11 18:37 statsmodels/Model.class
+-rw-rw-r--  2.0 unx     1110 b- defN 23-Jun-11 18:37 statsmodels/ResultsWrapper.class
+-rw-rw-r--  2.0 unx     1753 b- defN 23-Jun-11 18:37 statsmodels/regression/LinearRegression.class
+-rw-rw-r--  2.0 unx     2395 b- defN 23-Jun-11 18:37 statsmodels/regression/RegressionModel.class
+-rw-rw-r--  2.0 unx     8223 b- defN 23-Jun-11 18:37 statsmodels/genmod/GLM.class
+-rw-rw-r--  2.0 unx      591 b- defN 23-Jun-11 18:37 statsmodels/genmod/Link.class
+-rw-rw-r--  2.0 unx      615 b- defN 23-Jun-11 18:37 statsmodels/genmod/Family.class
+-rw-rw-r--  2.0 unx     1837 b- defN 23-Jun-11 18:36 META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml
+-rw-rw-r--  2.0 unx       60 b- defN 23-Jun-11 18:37 META-INF/maven/org.jpmml/pmml-statsmodels/pom.properties
+42 files, 65390 bytes uncompressed, 27118 bytes compressed:  58.5%
```

#### zipnote «TEMP»/diffoscope_rvr563yz_/tmp7t4pc74l_.zip

```diff
@@ -30,35 +30,26 @@
 
 Filename: statsmodels/regression/
 Comment: 
 
 Filename: statsmodels/genmod/
 Comment: 
 
-Filename: scipy/
-Comment: 
-
-Filename: scipy/stats/
-Comment: 
-
 Filename: META-INF/maven/
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-statsmodels/
 Comment: 
 
 Filename: META-INF/statsmodels2pmml.properties
 Comment: 
 
-Filename: META-INF/python2pmml.properties
-Comment: 
-
 Filename: org/jpmml/statsmodels/InterceptFeature.class
 Comment: 
 
 Filename: org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest.class
 Comment: 
 
 Filename: org/jpmml/statsmodels/testing/StatsModelsEncoderBatchTest$1.class
@@ -123,20 +114,14 @@
 
 Filename: statsmodels/genmod/Link.class
 Comment: 
 
 Filename: statsmodels/genmod/Family.class
 Comment: 
 
-Filename: scipy/stats/RVGeneric.class
-Comment: 
-
-Filename: scipy/stats/RVContinuous.class
-Comment: 
-
 Filename: META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-statsmodels/pom.properties
 Comment: 
 
 Zip file comment:
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-StatsModels library
-Implementation-Version: 1.0.3
+Implementation-Version: 1.0.4
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### statsmodels/data/ModelData$Cache.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum b8bc82a1d75c14f56cdeb4ae7e743fab72f3ba6bcc86b83e23138bc461d67938
+  SHA-256 checksum 93cf2391204f41b5db5c0e90030b193608f1a8c6178cb372c2925444dd8072d1
   Compiled from "ModelData.java"
 public class statsmodels.data.ModelData$Cache extends org.jpmml.python.PythonObject
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #10                         // statsmodels/data/ModelData$Cache
   super_class: #11                        // org/jpmml/python/PythonObject
@@ -86,17 +86,17 @@
          2: putfield      #1                  // Field this$0:Lstatsmodels/data/ModelData;
          5: aload_0
          6: aload_2
          7: aload_3
          8: invokespecial #2                  // Method org/jpmml/python/PythonObject."<init>":(Ljava/lang/String;Ljava/lang/String;)V
         11: return
       LineNumberTable:
-        line 79: 0
-        line 80: 5
-        line 81: 11
+        line 73: 0
+        line 74: 5
+        line 75: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lstatsmodels/data/ModelData$Cache;
             0      12     1 this$0   Lstatsmodels/data/ModelData;
             0      12     2 module   Ljava/lang/String;
             0      12     3  name   Ljava/lang/String;
 
@@ -114,15 +114,15 @@
         12: invokevirtual #4                  // Method containsKey:(Ljava/lang/Object;)Z
         15: ifeq          22
         18: iconst_1
         19: goto          23
         22: iconst_0
         23: ireturn
       LineNumberTable:
-        line 84: 0
+        line 78: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      24     0  this   Lstatsmodels/data/ModelData$Cache;
       StackMapTable: number_of_entries = 2
         frame_type = 22 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -134,15 +134,15 @@
       stack=3, locals=1, args_size=1
          0: aload_0
          1: ldc           #3                  // String xnames
          3: ldc           #6                  // class java/lang/String
          5: invokevirtual #7                  // Method getList:(Ljava/lang/String;Ljava/lang/Class;)Ljava/util/List;
          8: areturn
       LineNumberTable:
-        line 88: 0
+        line 82: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lstatsmodels/data/ModelData$Cache;
     Signature: #32                          // ()Ljava/util/List<Ljava/lang/String;>;
 
   public java.util.List<java.lang.String> getYNames();
     descriptor: ()Ljava/util/List;
@@ -162,18 +162,18 @@
         21: areturn
         22: aload_0
         23: ldc           #5                  // String ynames
         25: ldc           #6                  // class java/lang/String
         27: invokevirtual #7                  // Method getList:(Ljava/lang/String;Ljava/lang/Class;)Ljava/util/List;
         30: areturn
       LineNumberTable:
-        line 92: 0
-        line 94: 7
-        line 95: 14
-        line 98: 22
+        line 86: 0
+        line 88: 7
+        line 89: 14
+        line 92: 22
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      31     0  this   Lstatsmodels/data/ModelData$Cache;
             7      24     1 yNames   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
           offset_delta = 22
```

#### statsmodels/data/ModelData.class

##### procyon -ec {}

```diff
@@ -1,14 +1,14 @@
 
 package statsmodels.data;
 
 import java.util.Map;
+import pandas.core.Index;
 import pandas.core.BlockManager;
 import pandas.core.DataFrame;
-import pandas.core.Index;
 import pandas.core.Series;
 import java.util.Collections;
 import java.util.List;
 import org.jpmml.python.PythonObject;
 
 public class ModelData extends PythonObject
 {
@@ -20,20 +20,15 @@
         final Series origEndog = this.getOrigEndog();
         return Collections.singletonList(origEndog.getName());
     }
     
     public List<String> getExogNames() {
         final DataFrame origExog = this.getOrigExog();
         final BlockManager data = origExog.getData();
-        final List<Index> axes = data.getAxesArray();
-        if (axes.size() != 2) {
-            throw new IllegalArgumentException();
-        }
-        final Index columnAxis = (Index)axes.get(0);
-        final Index rowAxis = (Index)axes.get(1);
+        final Index columnAxis = data.getColumnAxis();
         return columnAxis.getValues();
     }
     
     public ModelData.Cache getCache() {
         final Map<String, ?> map = (Map)this.get("_cache", (Class)Map.class);
         final ModelData.Cache cache = new ModelData.Cache(this, this.getPythonModule() + "." + this.getPythonName(), "_cache");
         cache.putAll((Map)map);
```

#### META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml

##### META-INF/maven/org.jpmml/pmml-statsmodels/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-statsmodels</artifactId>
-    <version>1.0.3</version>
+    <version>1.0.4</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-statsmodels</artifactId>
   <packaging>jar</packaging>
   <name>JPMML StatsModels converter</name>
   <description>JPMML StatsModels to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-statsmodels/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-statsmodels
 groupId=org.jpmml
-version=1.0.3
+version=1.0.4
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.29.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.30.jar`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6333 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 h2o/estimators/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/preprocessing/h2o/
--rw-rw-r--  2.0 unx      679 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     5710 b- defN 23-Jun-06 10:35 h2o/estimators/H2OEstimator.class
--rw-rw-r--  2.0 unx     1694 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
--rw-rw-r--  2.0 unx     1305 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
--rw-rw-r--  2.0 unx      112 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
-15 files, 9630 bytes uncompressed, 4317 bytes compressed:  55.2%
+Zip file size: 6331 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 h2o/estimators/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/preprocessing/h2o/
+-rw-rw-r--  2.0 unx      679 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     5710 b- defN 23-Jun-19 22:03 h2o/estimators/H2OEstimator.class
+-rw-rw-r--  2.0 unx     1694 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
+-rw-rw-r--  2.0 unx     1305 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
+-rw-rw-r--  2.0 unx      112 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
+15 files, 9630 bytes uncompressed, 4315 bytes compressed:  55.2%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.29</version>
+    <version>1.7.30</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn H2O.ai converter</name>
   <description>JPMML Scikit-Learn H2O.ai to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Tue Jun 06 10:35:43 EEST 2023
-version=1.7.29
+#Mon Jun 19 22:03:17 EEST 2023
+version=1.7.30
 groupId=org.jpmml
 artifactId=pmml-sklearn-h2o
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/pmml-sklearn-1.7.29.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-1.7.30.jar`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,405 +1,405 @@
-Zip file size: 467741 bytes, number of entries: 403
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 23-Jun-06 10:35 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn_pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 chaid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 stop_words/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/calibration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/dummy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/svm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/impute/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/naive_bayes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/logistic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/ridge/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/glm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/compose/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/model_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/decomposition/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/neighbors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/multioutput/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/isotonic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/bagging/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/stacking/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/forest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/iforest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/voting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/ensemble/weight_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/loss/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/discriminant_analysis/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/tree/visitors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/cluster/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn/multiclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/ruleset/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/decoration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/util/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/postprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 sklearn2pmml/expression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 org/jpmml/sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 org/jpmml/sklearn/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn/
--rw-rw-r--  2.0 unx    16829 b- defN 23-Jun-06 10:35 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2287 b- defN 23-Jun-06 10:35 sklearn_pandas/CategoricalImputer.class
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-06 10:35 sklearn_pandas/TransformerPipeline.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Jun-06 10:35 sklearn_pandas/DataFrameMapper$2.class
--rw-rw-r--  2.0 unx     6280 b- defN 23-Jun-06 10:35 sklearn_pandas/DataFrameMapper.class
--rw-rw-r--  2.0 unx     1126 b- defN 23-Jun-06 10:35 sklearn_pandas/DataFrameMapper$1.class
--rw-rw-r--  2.0 unx      609 b- defN 23-Jun-06 10:35 chaid/ContinuousColumn.class
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-06 10:35 chaid/Node.class
--rw-rw-r--  2.0 unx      467 b- defN 23-Jun-06 10:35 chaid/Column.class
--rw-rw-r--  2.0 unx     3283 b- defN 23-Jun-06 10:35 chaid/Split.class
--rw-rw-r--  2.0 unx      401 b- defN 23-Jun-06 10:35 chaid/InvalidSplitReason.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Jun-06 10:35 chaid/NominalColumn.class
--rw-rw-r--  2.0 unx     1912 b- defN 23-Jun-06 10:35 stop_words/english.txt
--rw-rw-r--  2.0 unx      147 b- defN 23-Jun-06 10:35 sklearn/HasHead.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Jun-06 10:35 sklearn/StepUtil.class
--rw-rw-r--  2.0 unx    11453 b- defN 23-Jun-06 10:35 sklearn/calibration/CalibratedClassifier.class
--rw-rw-r--  2.0 unx     2972 b- defN 23-Jun-06 10:35 sklearn/calibration/SigmoidCalibration.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Jun-06 10:35 sklearn/calibration/CalibratedClassifier$1.class
--rw-rw-r--  2.0 unx     1475 b- defN 23-Jun-06 10:35 sklearn/calibration/CalibratedClassifierCV.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-06 10:35 sklearn/pipeline/PipelineTransformer.class
--rw-rw-r--  2.0 unx     1671 b- defN 23-Jun-06 10:35 sklearn/pipeline/Pipeline$2.class
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-06 10:35 sklearn/pipeline/FeatureUnion.class
--rw-rw-r--  2.0 unx     5062 b- defN 23-Jun-06 10:35 sklearn/pipeline/Pipeline.class
--rw-rw-r--  2.0 unx     2003 b- defN 23-Jun-06 10:35 sklearn/pipeline/PipelineRegressor.class
--rw-rw-r--  2.0 unx     1773 b- defN 23-Jun-06 10:35 sklearn/pipeline/Pipeline$1.class
--rw-rw-r--  2.0 unx     1111 b- defN 23-Jun-06 10:35 sklearn/pipeline/PipelineUtil.class
--rw-rw-r--  2.0 unx     2298 b- defN 23-Jun-06 10:35 sklearn/pipeline/PipelineClassifier.class
--rw-rw-r--  2.0 unx     4913 b- defN 23-Jun-06 10:35 sklearn/dummy/DummyClassifier.class
--rw-rw-r--  2.0 unx     2055 b- defN 23-Jun-06 10:35 sklearn/dummy/DummyRegressor.class
--rw-rw-r--  2.0 unx      454 b- defN 23-Jun-06 10:35 sklearn/SkLearnFields.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Jun-06 10:35 sklearn/SkLearnOutlierTransformation.class
--rw-rw-r--  2.0 unx      240 b- defN 23-Jun-06 10:35 sklearn/HasEstimator.class
--rw-rw-r--  2.0 unx     3456 b- defN 23-Jun-06 10:35 sklearn/OutlierDetectorUtil.class
--rw-rw-r--  2.0 unx     1258 b- defN 23-Jun-06 10:35 sklearn/HasMultiApplyField.class
--rw-rw-r--  2.0 unx      908 b- defN 23-Jun-06 10:35 sklearn/None.class
--rw-rw-r--  2.0 unx     2393 b- defN 23-Jun-06 10:35 sklearn/svm/SupportVectorMachineUtil.class
--rw-rw-r--  2.0 unx     1109 b- defN 23-Jun-06 10:35 sklearn/svm/LinearSVC.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-Jun-06 10:35 sklearn/svm/LibSVMClassifier.class
--rw-rw-r--  2.0 unx      966 b- defN 23-Jun-06 10:35 sklearn/svm/SupportVectorMachineUtil$1.class
--rw-rw-r--  2.0 unx     1305 b- defN 23-Jun-06 10:35 sklearn/svm/OneClassSVM.class
--rw-rw-r--  2.0 unx     3594 b- defN 23-Jun-06 10:35 sklearn/svm/LibSVMRegressor.class
--rw-rw-r--  2.0 unx     4114 b- defN 23-Jun-06 10:35 sklearn/InitializerUtil$1.class
--rw-rw-r--  2.0 unx      735 b- defN 23-Jun-06 10:35 sklearn/Estimator$1.class
--rw-rw-r--  2.0 unx      214 b- defN 23-Jun-06 10:35 sklearn/HasNumberOfFeatures.class
--rw-rw-r--  2.0 unx      660 b- defN 23-Jun-06 10:35 sklearn/MultiTransformer.class
--rw-rw-r--  2.0 unx     2110 b- defN 23-Jun-06 10:35 sklearn/neural_network/MLPRegressor.class
--rw-rw-r--  2.0 unx     2555 b- defN 23-Jun-06 10:35 sklearn/neural_network/MLPClassifier.class
--rw-rw-r--  2.0 unx      759 b- defN 23-Jun-06 10:35 sklearn/neural_network/MultilayerPerceptronUtil$1.class
--rw-rw-r--  2.0 unx    11996 b- defN 23-Jun-06 10:35 sklearn/neural_network/MultilayerPerceptronUtil.class
--rw-rw-r--  2.0 unx     1880 b- defN 23-Jun-06 10:35 sklearn/Step.class
--rw-rw-r--  2.0 unx      168 b- defN 23-Jun-06 10:35 sklearn/HasDefaultValue.class
--rw-rw-r--  2.0 unx     2936 b- defN 23-Jun-06 10:35 sklearn/impute/MissingIndicator.class
--rw-rw-r--  2.0 unx     4027 b- defN 23-Jun-06 10:35 sklearn/impute/ImputerUtil.class
--rw-rw-r--  2.0 unx     5703 b- defN 23-Jun-06 10:35 sklearn/impute/SimpleImputer.class
--rw-rw-r--  2.0 unx     6948 b- defN 23-Jun-06 10:35 sklearn/naive_bayes/GaussianNB.class
--rw-rw-r--  2.0 unx     4398 b- defN 23-Jun-06 10:35 sklearn/linear_model/LinearRegressor.class
--rw-rw-r--  2.0 unx     5040 b- defN 23-Jun-06 10:35 sklearn/linear_model/LinearClassifier.class
--rw-rw-r--  2.0 unx     7648 b- defN 23-Jun-06 10:35 sklearn/linear_model/logistic/LogisticRegression.class
--rw-rw-r--  2.0 unx     1042 b- defN 23-Jun-06 10:35 sklearn/linear_model/ridge/RidgeClassifier.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Jun-06 10:35 sklearn/linear_model/glm/DistributionBoundary.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Jun-06 10:35 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/Hinge.class
--rw-rw-r--  2.0 unx     2480 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
--rw-rw-r--  2.0 unx      461 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/LossFunction.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/Log.class
--rw-rw-r--  2.0 unx     1165 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
--rw-rw-r--  2.0 unx      482 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
--rw-rw-r--  2.0 unx      932 b- defN 23-Jun-06 10:35 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
--rw-rw-r--  2.0 unx     1720 b- defN 23-Jun-06 10:35 sklearn/compose/ColumnTransformer$1.class
--rw-rw-r--  2.0 unx     3239 b- defN 23-Jun-06 10:35 sklearn/compose/TransformedTargetRegressor.class
--rw-rw-r--  2.0 unx     3649 b- defN 23-Jun-06 10:35 sklearn/compose/ColumnTransformer.class
--rw-rw-r--  2.0 unx     1534 b- defN 23-Jun-06 10:35 sklearn/compose/TransformedTargetRegressor$1.class
--rw-rw-r--  2.0 unx     4089 b- defN 23-Jun-06 10:35 sklearn/Classifier.class
--rw-rw-r--  2.0 unx     1457 b- defN 23-Jun-06 10:35 sklearn/model_selection/EstimatorSearcher.class
--rw-rw-r--  2.0 unx     1685 b- defN 23-Jun-06 10:35 sklearn/Selector.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Jun-06 10:35 sklearn/decomposition/IncrementalPCA.class
--rw-rw-r--  2.0 unx     3471 b- defN 23-Jun-06 10:35 sklearn/decomposition/TruncatedSVD.class
--rw-rw-r--  2.0 unx     4759 b- defN 23-Jun-06 10:35 sklearn/decomposition/PCA.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jun-06 10:35 sklearn/decomposition/BasePCA.class
--rw-rw-r--  2.0 unx      336 b- defN 23-Jun-06 10:35 sklearn/HasPredictField.class
--rw-rw-r--  2.0 unx     3018 b- defN 23-Jun-06 10:35 sklearn/neighbors/NearestNeighbors.class
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-06 10:35 sklearn/neighbors/KNeighborsClassifier.class
--rw-rw-r--  2.0 unx     3794 b- defN 23-Jun-06 10:35 sklearn/neighbors/NearestCentroid.class
--rw-rw-r--  2.0 unx     2025 b- defN 23-Jun-06 10:35 sklearn/neighbors/BinaryTree.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-Jun-06 10:35 sklearn/neighbors/KNeighborsUtil$1.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Jun-06 10:35 sklearn/neighbors/HasMetric.class
--rw-rw-r--  2.0 unx    10748 b- defN 23-Jun-06 10:35 sklearn/neighbors/KNeighborsUtil.class
--rw-rw-r--  2.0 unx     4387 b- defN 23-Jun-06 10:35 sklearn/neighbors/KNeighborsRegressor.class
--rw-rw-r--  2.0 unx     1032 b- defN 23-Jun-06 10:35 sklearn/neighbors/DistanceMetric.class
--rw-rw-r--  2.0 unx      351 b- defN 23-Jun-06 10:35 sklearn/neighbors/HasTrainingData.class
--rw-rw-r--  2.0 unx      176 b- defN 23-Jun-06 10:35 sklearn/neighbors/HasNumberOfNeighbors.class
--rw-rw-r--  2.0 unx     2235 b- defN 23-Jun-06 10:35 sklearn/multioutput/MultiOutputUtil.class
--rw-rw-r--  2.0 unx     3383 b- defN 23-Jun-06 10:35 sklearn/multioutput/ChainUtil.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Jun-06 10:35 sklearn/multioutput/RegressorChain.class
--rw-rw-r--  2.0 unx     1316 b- defN 23-Jun-06 10:35 sklearn/multioutput/MultiOutputClassifier.class
--rw-rw-r--  2.0 unx     1310 b- defN 23-Jun-06 10:35 sklearn/multioutput/MultiOutputRegressor.class
--rw-rw-r--  2.0 unx     1745 b- defN 23-Jun-06 10:35 sklearn/multioutput/ClassifierChain.class
--rw-rw-r--  2.0 unx     4469 b- defN 23-Jun-06 10:35 sklearn/isotonic/IsotonicRegression.class
--rw-rw-r--  2.0 unx      326 b- defN 23-Jun-06 10:35 sklearn/HasApplyField.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Jun-06 10:35 sklearn/HasEstimatorEnsemble.class
--rw-rw-r--  2.0 unx     1929 b- defN 23-Jun-06 10:35 sklearn/Transformer$1.class
--rw-rw-r--  2.0 unx      953 b- defN 23-Jun-06 10:35 sklearn/LabelEncoderClassifier.class
--rw-rw-r--  2.0 unx      937 b- defN 23-Jun-06 10:35 sklearn/PassThrough.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Jun-06 10:35 sklearn/HasPriorProbability.class
--rw-rw-r--  2.0 unx     5693 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/TfidfVectorizer.class
--rw-rw-r--  2.0 unx      809 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/TfidfVectorizer$1.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/Tokenizer.class
--rw-rw-r--  2.0 unx    13329 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/CountVectorizer.class
--rw-rw-r--  2.0 unx     2129 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/CountVectorizer$1.class
--rw-rw-r--  2.0 unx     1433 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/text/TfidfTransformer.class
--rw-rw-r--  2.0 unx     4031 b- defN 23-Jun-06 10:35 sklearn/feature_extraction/DictVectorizer.class
--rw-rw-r--  2.0 unx      762 b- defN 23-Jun-06 10:35 sklearn/Clusterer.class
--rw-rw-r--  2.0 unx     1375 b- defN 23-Jun-06 10:35 sklearn/metrics/DistanceMetric.class
--rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-06 10:35 sklearn/ensemble/EnsembleUtil.class
--rw-rw-r--  2.0 unx     2112 b- defN 23-Jun-06 10:35 sklearn/ensemble/bagging/BaggingRegressor.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-Jun-06 10:35 sklearn/ensemble/bagging/BaggingUtil.class
--rw-rw-r--  2.0 unx     3031 b- defN 23-Jun-06 10:35 sklearn/ensemble/bagging/BaggingClassifier.class
--rw-rw-r--  2.0 unx     1409 b- defN 23-Jun-06 10:35 sklearn/ensemble/EnsembleRegressor.class
--rw-rw-r--  2.0 unx     3485 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingClassifier.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
--rw-rw-r--  2.0 unx     3109 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingRegressor.class
--rw-rw-r--  2.0 unx     3960 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingUtil.class
--rw-rw-r--  2.0 unx     2524 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingClassifier$1.class
--rw-rw-r--  2.0 unx     2254 b- defN 23-Jun-06 10:35 sklearn/ensemble/stacking/StackingRegressor$1.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
--rw-rw-r--  2.0 unx     2563 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
--rw-rw-r--  2.0 unx      858 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/LossFunction.class
--rw-rw-r--  2.0 unx     1588 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
--rw-rw-r--  2.0 unx     1317 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
--rw-rw-r--  2.0 unx     7948 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
--rw-rw-r--  2.0 unx      960 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/MeanEstimator.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
--rw-rw-r--  2.0 unx     1578 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
--rw-rw-r--  2.0 unx      811 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
--rw-rw-r--  2.0 unx     3003 b- defN 23-Jun-06 10:35 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
--rw-rw-r--  2.0 unx     1148 b- defN 23-Jun-06 10:35 sklearn/ensemble/EnsembleUtil$1.class
--rw-rw-r--  2.0 unx     3059 b- defN 23-Jun-06 10:35 sklearn/ensemble/forest/ForestUtil.class
--rw-rw-r--  2.0 unx     2311 b- defN 23-Jun-06 10:35 sklearn/ensemble/forest/ForestRegressor.class
--rw-rw-r--  2.0 unx     2770 b- defN 23-Jun-06 10:35 sklearn/ensemble/forest/ForestClassifier.class
--rw-rw-r--  2.0 unx     1752 b- defN 23-Jun-06 10:35 sklearn/ensemble/iforest/IsolationForest$3.class
--rw-rw-r--  2.0 unx     2206 b- defN 23-Jun-06 10:35 sklearn/ensemble/iforest/IsolationForest$1.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Jun-06 10:35 sklearn/ensemble/iforest/IsolationForest$2.class
--rw-rw-r--  2.0 unx     8265 b- defN 23-Jun-06 10:35 sklearn/ensemble/iforest/IsolationForest.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Jun-06 10:35 sklearn/ensemble/voting/VotingClassifier.class
--rw-rw-r--  2.0 unx     3716 b- defN 23-Jun-06 10:35 sklearn/ensemble/voting/VotingRegressor.class
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
--rw-rw-r--  2.0 unx     1247 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
--rw-rw-r--  2.0 unx     3041 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
--rw-rw-r--  2.0 unx     6152 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
--rw-rw-r--  2.0 unx      490 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
--rw-rw-r--  2.0 unx     1572 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
--rw-rw-r--  2.0 unx     6377 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     8868 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Jun-06 10:35 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-06 10:35 sklearn/ensemble/EnsembleClassifier.class
--rw-rw-r--  2.0 unx     3564 b- defN 23-Jun-06 10:35 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
--rw-rw-r--  2.0 unx     5361 b- defN 23-Jun-06 10:35 sklearn/Transformer.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Jun-06 10:35 sklearn/Transformer$1$1.class
--rw-rw-r--  2.0 unx      981 b- defN 23-Jun-06 10:35 sklearn/Drop.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-06 10:35 sklearn/feature_selection/SelectKBest$Entry.class
--rw-rw-r--  2.0 unx     3486 b- defN 23-Jun-06 10:35 sklearn/feature_selection/SelectFromModel.class
--rw-rw-r--  2.0 unx     2922 b- defN 23-Jun-06 10:35 sklearn/feature_selection/SelectKBest.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Jun-06 10:35 sklearn/feature_selection/PySelector.class
--rw-rw-r--  2.0 unx      607 b- defN 23-Jun-06 10:35 sklearn/Transformer$2.class
--rw-rw-r--  2.0 unx     2216 b- defN 23-Jun-06 10:35 sklearn/SkLearnUtil.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Jun-06 10:35 sklearn/loss/HalfMultinomialLoss.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Jun-06 10:35 sklearn/loss/CyLossFunction.class
--rw-rw-r--  2.0 unx      403 b- defN 23-Jun-06 10:35 sklearn/loss/HalfBinomialLoss.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Jun-06 10:35 sklearn/loss/BaseLoss.class
--rw-rw-r--  2.0 unx      381 b- defN 23-Jun-06 10:35 sklearn/HasDecisionFunctionField.class
--rw-rw-r--  2.0 unx      338 b- defN 23-Jun-06 10:35 sklearn/SkLearnMethods.class
--rw-rw-r--  2.0 unx     3091 b- defN 23-Jun-06 10:35 sklearn/ScalarLabelUtil.class
--rw-rw-r--  2.0 unx     1582 b- defN 23-Jun-06 10:35 sklearn/OutlierDetectorUtil$1.class
--rw-rw-r--  2.0 unx      195 b- defN 23-Jun-06 10:35 sklearn/HasClasses.class
--rw-rw-r--  2.0 unx     4685 b- defN 23-Jun-06 10:35 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
--rw-rw-r--  2.0 unx      696 b- defN 23-Jun-06 10:35 sklearn/EstimatorUtil$1.class
--rw-rw-r--  2.0 unx     3311 b- defN 23-Jun-06 10:35 sklearn/Composite.class
--rw-rw-r--  2.0 unx     1194 b- defN 23-Jun-06 10:35 sklearn/preprocessing/KBinsDiscretizer$1.class
--rw-rw-r--  2.0 unx     4567 b- defN 23-Jun-06 10:35 sklearn/preprocessing/PowerTransformer.class
--rw-rw-r--  2.0 unx     2381 b- defN 23-Jun-06 10:35 sklearn/preprocessing/LabelEncoder.class
--rw-rw-r--  2.0 unx     4924 b- defN 23-Jun-06 10:35 sklearn/preprocessing/LabelBinarizer.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Jun-06 10:35 sklearn/preprocessing/EncoderUtil$3.class
--rw-rw-r--  2.0 unx      389 b- defN 23-Jun-06 10:35 sklearn/preprocessing/Scaler.class
--rw-rw-r--  2.0 unx     3242 b- defN 23-Jun-06 10:35 sklearn/preprocessing/MaxAbsScaler.class
--rw-rw-r--  2.0 unx     2948 b- defN 23-Jun-06 10:35 sklearn/preprocessing/FunctionTransformer.class
--rw-rw-r--  2.0 unx     3291 b- defN 23-Jun-06 10:35 sklearn/preprocessing/BaseEncoder.class
--rw-rw-r--  2.0 unx     1270 b- defN 23-Jun-06 10:35 sklearn/preprocessing/EncoderUtil$1.class
--rw-rw-r--  2.0 unx     4549 b- defN 23-Jun-06 10:35 sklearn/preprocessing/StandardScaler.class
--rw-rw-r--  2.0 unx     6971 b- defN 23-Jun-06 10:35 sklearn/preprocessing/EncoderUtil.class
--rw-rw-r--  2.0 unx     6343 b- defN 23-Jun-06 10:35 sklearn/preprocessing/PolynomialFeatures.class
--rw-rw-r--  2.0 unx     8486 b- defN 23-Jun-06 10:35 sklearn/preprocessing/KBinsDiscretizer.class
--rw-rw-r--  2.0 unx     4671 b- defN 23-Jun-06 10:35 sklearn/preprocessing/OneHotEncoder.class
--rw-rw-r--  2.0 unx     2553 b- defN 23-Jun-06 10:35 sklearn/preprocessing/Binarizer.class
--rw-rw-r--  2.0 unx     1054 b- defN 23-Jun-06 10:35 sklearn/preprocessing/EncoderUtil$2.class
--rw-rw-r--  2.0 unx     3595 b- defN 23-Jun-06 10:35 sklearn/preprocessing/MinMaxScaler.class
--rw-rw-r--  2.0 unx     4467 b- defN 23-Jun-06 10:35 sklearn/preprocessing/RobustScaler.class
--rw-rw-r--  2.0 unx     3740 b- defN 23-Jun-06 10:35 sklearn/preprocessing/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      957 b- defN 23-Jun-06 10:35 sklearn/preprocessing/Imputer.class
--rw-rw-r--  2.0 unx     2033 b- defN 23-Jun-06 10:35 sklearn/preprocessing/PolynomialFeatures$1.class
--rw-rw-r--  2.0 unx     7408 b- defN 23-Jun-06 10:35 sklearn/preprocessing/MultiOneHotEncoder.class
--rw-rw-r--  2.0 unx     2153 b- defN 23-Jun-06 10:35 sklearn/tree/TreeClassifier.class
--rw-rw-r--  2.0 unx     3111 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$1.class
--rw-rw-r--  2.0 unx     2664 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$4.class
--rw-rw-r--  2.0 unx     4805 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelFlattener.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelCompactor$1.class
--rw-rw-r--  2.0 unx     5431 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     2988 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelPruner.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelFlattener$1.class
--rw-rw-r--  2.0 unx      730 b- defN 23-Jun-06 10:35 sklearn/tree/visitors/TreeModelPruner$1.class
--rw-rw-r--  2.0 unx     1489 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$8.class
--rw-rw-r--  2.0 unx      879 b- defN 23-Jun-06 10:35 sklearn/tree/RegressionCriterion.class
--rw-rw-r--  2.0 unx     1151 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$5.class
--rw-rw-r--  2.0 unx      978 b- defN 23-Jun-06 10:35 sklearn/tree/PresortBestSplitter.class
--rw-rw-r--  2.0 unx      955 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$6.class
--rw-rw-r--  2.0 unx     1764 b- defN 23-Jun-06 10:35 sklearn/tree/TreeRegressor.class
--rw-rw-r--  2.0 unx     1589 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$7.class
--rw-rw-r--  2.0 unx    20072 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$3.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-06 10:35 sklearn/tree/HasTreeOptions.class
--rw-rw-r--  2.0 unx     2257 b- defN 23-Jun-06 10:35 sklearn/tree/Tree.class
--rw-rw-r--  2.0 unx      754 b- defN 23-Jun-06 10:35 sklearn/tree/TreeUtil$2.class
--rw-rw-r--  2.0 unx      150 b- defN 23-Jun-06 10:35 sklearn/tree/HasTree.class
--rw-rw-r--  2.0 unx     1967 b- defN 23-Jun-06 10:35 sklearn/InitializerUtil.class
--rw-rw-r--  2.0 unx      570 b- defN 23-Jun-06 10:35 sklearn/Regressor.class
--rw-rw-r--  2.0 unx      211 b- defN 23-Jun-06 10:35 sklearn/HasNumberOfOutputs.class
--rw-rw-r--  2.0 unx      381 b- defN 23-Jun-06 10:35 sklearn/OutlierDetector.class
--rw-rw-r--  2.0 unx     2366 b- defN 23-Jun-06 10:35 sklearn/Calibrator.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Jun-06 10:35 sklearn/HasClassifierOptions.class
--rw-rw-r--  2.0 unx     7075 b- defN 23-Jun-06 10:35 sklearn/EstimatorUtil.class
--rw-rw-r--  2.0 unx      199 b- defN 23-Jun-06 10:35 sklearn/HasType.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Jun-06 10:35 sklearn/cluster/MiniBatchKMeans.class
--rw-rw-r--  2.0 unx     5086 b- defN 23-Jun-06 10:35 sklearn/cluster/KMeans.class
--rw-rw-r--  2.0 unx    12172 b- defN 23-Jun-06 10:35 sklearn/Estimator.class
--rw-rw-r--  2.0 unx     1624 b- defN 23-Jun-06 10:35 sklearn/Initializer.class
--rw-rw-r--  2.0 unx     4598 b- defN 23-Jun-06 10:35 sklearn/multiclass/OneVsRestClassifier.class
--rw-rw-r--  2.0 unx     5157 b- defN 23-Jun-06 10:35 sklearn2pmml/ruleset/RuleSetClassifier.class
--rw-rw-r--  2.0 unx     1023 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/PMMLPipeline$3.class
--rw-rw-r--  2.0 unx    28136 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/PMMLPipeline.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/PMMLPipeline$2.class
--rw-rw-r--  2.0 unx     1421 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/PMMLPipeline$1.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-Jun-06 10:35 sklearn2pmml/pipeline/Verification.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/MultiDomain.class
--rw-rw-r--  2.0 unx     1152 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/ContinuousDomainEraser.class
--rw-rw-r--  2.0 unx     1654 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Alias.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/TemporalDomain.class
--rw-rw-r--  2.0 unx      779 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/ContinuousDomain$1.class
--rw-rw-r--  2.0 unx    11878 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain.class
--rw-rw-r--  2.0 unx     1416 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/MultiAlias.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DiscreteDomain.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/CategoricalDomain.class
--rw-rw-r--  2.0 unx     1453 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DomainEraser.class
--rw-rw-r--  2.0 unx      613 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DateTimeDomain.class
--rw-rw-r--  2.0 unx     7764 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/ContinuousDomain.class
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DiscreteDomainEraser.class
--rw-rw-r--  2.0 unx     1590 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/TransformerWrapper.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain$2.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DateDomain.class
--rw-rw-r--  2.0 unx     3544 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/DomainUtil.class
--rw-rw-r--  2.0 unx     1033 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain$1.class
--rw-rw-r--  2.0 unx     1577 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/OrdinalDomain.class
--rw-rw-r--  2.0 unx      672 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain$4.class
--rw-rw-r--  2.0 unx      799 b- defN 23-Jun-06 10:35 sklearn2pmml/decoration/Domain$3.class
--rw-rw-r--  2.0 unx     7862 b- defN 23-Jun-06 10:35 sklearn2pmml/neural_network/MLPTransformer.class
--rw-rw-r--  2.0 unx      391 b- defN 23-Jun-06 10:35 sklearn2pmml/SkLearn2PMMLFields.class
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Evaluatable.class
--rw-rw-r--  2.0 unx     1196 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Expression.class
--rw-rw-r--  2.0 unx     1189 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Predicate.class
--rw-rw-r--  2.0 unx     1434 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Reshaper.class
--rw-rw-r--  2.0 unx     3392 b- defN 23-Jun-06 10:35 sklearn2pmml/util/EvaluatableUtil.class
--rw-rw-r--  2.0 unx     1658 b- defN 23-Jun-06 10:35 sklearn2pmml/util/Slicer.class
--rw-rw-r--  2.0 unx     2418 b- defN 23-Jun-06 10:35 sklearn2pmml/feature_extraction/text/Splitter.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-Jun-06 10:35 sklearn2pmml/feature_extraction/text/Matcher.class
--rw-rw-r--  2.0 unx     1262 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/SelectFirstRegressor.class
--rw-rw-r--  2.0 unx     2083 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTUtil$2.class
--rw-rw-r--  2.0 unx     1134 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/EstimatorChain$1.class
--rw-rw-r--  2.0 unx     1934 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTLMRegressor.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTUtil$1.class
--rw-rw-r--  2.0 unx     7358 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/EstimatorChain.class
--rw-rw-r--  2.0 unx     6578 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTUtil.class
--rw-rw-r--  2.0 unx     3995 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/Link.class
--rw-rw-r--  2.0 unx     4360 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/SelectFirstUtil.class
--rw-rw-r--  2.0 unx     4252 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/GBDTLRClassifier.class
--rw-rw-r--  2.0 unx     2608 b- defN 23-Jun-06 10:35 sklearn2pmml/ensemble/SelectFirstClassifier.class
--rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-06 10:35 sklearn2pmml/EstimatorProxy$1.class
--rw-rw-r--  2.0 unx      946 b- defN 23-Jun-06 10:35 sklearn2pmml/feature_selection/SelectUnique.class
--rw-rw-r--  2.0 unx     6477 b- defN 23-Jun-06 10:35 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
--rw-rw-r--  2.0 unx      791 b- defN 23-Jun-06 10:35 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
--rw-rw-r--  2.0 unx     1197 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/PatternTransformer.class
--rw-rw-r--  2.0 unx     2908 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/ReplaceTransformer.class
--rw-rw-r--  2.0 unx     1844 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/WordCountTransformer.class
--rw-rw-r--  2.0 unx      597 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/DateTimeFormatter.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
--rw-rw-r--  2.0 unx     4621 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/DurationTransformer.class
--rw-rw-r--  2.0 unx      444 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
--rw-rw-r--  2.0 unx     2777 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/FilterLookupTransformer.class
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/Formatter.class
--rw-rw-r--  2.0 unx     3341 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/CastTransformer.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/MatchesTransformer.class
--rw-rw-r--  2.0 unx      589 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/NumberFormatter.class
--rw-rw-r--  2.0 unx     4149 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/MultiLookupTransformer.class
--rw-rw-r--  2.0 unx     3871 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/StringNormalizer.class
--rw-rw-r--  2.0 unx     7145 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/ExpressionTransformer.class
--rw-rw-r--  2.0 unx      635 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
--rw-rw-r--  2.0 unx     3604 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/DataFrameConstructor.class
--rw-rw-r--  2.0 unx     2847 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/ConcatTransformer.class
--rw-rw-r--  2.0 unx     5993 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/CutTransformer.class
--rw-rw-r--  2.0 unx     7025 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/BSplineTransformer.class
--rw-rw-r--  2.0 unx     6410 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/LookupTransformer.class
--rw-rw-r--  2.0 unx     3236 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/SubstringTransformer.class
--rw-rw-r--  2.0 unx     3181 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
--rw-rw-r--  2.0 unx     2132 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
--rw-rw-r--  2.0 unx     3328 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/Aggregator.class
--rw-rw-r--  2.0 unx      647 b- defN 23-Jun-06 10:35 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Jun-06 10:35 sklearn2pmml/tree/CHAIDRegressor.class
--rw-rw-r--  2.0 unx    10719 b- defN 23-Jun-06 10:35 sklearn2pmml/tree/CHAIDUtil.class
--rw-rw-r--  2.0 unx     2121 b- defN 23-Jun-06 10:35 sklearn2pmml/tree/CHAIDClassifier.class
--rw-rw-r--  2.0 unx     1417 b- defN 23-Jun-06 10:35 sklearn2pmml/tree/CHAIDUtil$1.class
--rw-rw-r--  2.0 unx     3864 b- defN 23-Jun-06 10:35 sklearn2pmml/EstimatorProxy.class
--rw-rw-r--  2.0 unx     1458 b- defN 23-Jun-06 10:35 sklearn2pmml/SelectorProxy.class
--rw-rw-r--  2.0 unx     2046 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionUtil.class
--rw-rw-r--  2.0 unx     3799 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionRegressor.class
--rw-rw-r--  2.0 unx      990 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionClassifier$1.class
--rw-rw-r--  2.0 unx     8687 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionClassifier.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jun-06 10:35 sklearn2pmml/expression/ExpressionUtil$1.class
--rw-rw-r--  2.0 unx     1774 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2764 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
--rw-rw-r--  2.0 unx     3549 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
--rw-rw-r--  2.0 unx    13608 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/SkLearnEncoder.class
--rw-rw-r--  2.0 unx      194 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/FieldNames.class
--rw-rw-r--  2.0 unx      171 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/HasSkLearnOptions.class
--rw-rw-r--  2.0 unx     1030 b- defN 23-Jun-06 10:35 org/jpmml/sklearn/SkLearnEncoder$1.class
--rw-rw-r--  2.0 unx     1822 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 23-Jun-06 10:35 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
-403 files, 920905 bytes uncompressed, 405921 bytes compressed:  55.9%
+Zip file size: 468727 bytes, number of entries: 403
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn_pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 chaid/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 stop_words/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/calibration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/dummy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/svm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/impute/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/naive_bayes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/logistic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/ridge/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/glm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/compose/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/model_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/decomposition/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/neighbors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/multioutput/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/isotonic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/bagging/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/stacking/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/forest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/iforest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/voting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/weight_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/loss/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/discriminant_analysis/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/tree/visitors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/cluster/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/multiclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/ruleset/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/decoration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/util/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/postprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/expression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 org/jpmml/sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 org/jpmml/sklearn/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn/
+-rw-rw-r--  2.0 unx    16829 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2287 b- defN 23-Jun-19 22:03 sklearn_pandas/CategoricalImputer.class
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-19 22:03 sklearn_pandas/TransformerPipeline.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Jun-19 22:03 sklearn_pandas/DataFrameMapper$2.class
+-rw-rw-r--  2.0 unx     6280 b- defN 23-Jun-19 22:03 sklearn_pandas/DataFrameMapper.class
+-rw-rw-r--  2.0 unx     1126 b- defN 23-Jun-19 22:03 sklearn_pandas/DataFrameMapper$1.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-Jun-19 22:03 chaid/ContinuousColumn.class
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-19 22:03 chaid/Node.class
+-rw-rw-r--  2.0 unx      467 b- defN 23-Jun-19 22:03 chaid/Column.class
+-rw-rw-r--  2.0 unx     3283 b- defN 23-Jun-19 22:03 chaid/Split.class
+-rw-rw-r--  2.0 unx      401 b- defN 23-Jun-19 22:03 chaid/InvalidSplitReason.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Jun-19 22:03 chaid/NominalColumn.class
+-rw-rw-r--  2.0 unx     1912 b- defN 23-Jun-19 22:03 stop_words/english.txt
+-rw-rw-r--  2.0 unx      147 b- defN 23-Jun-19 22:03 sklearn/HasHead.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-Jun-19 22:03 sklearn/StepUtil.class
+-rw-rw-r--  2.0 unx    12044 b- defN 23-Jun-19 22:03 sklearn/calibration/CalibratedClassifier.class
+-rw-rw-r--  2.0 unx     2953 b- defN 23-Jun-19 22:03 sklearn/calibration/SigmoidCalibration.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-Jun-19 22:03 sklearn/calibration/CalibratedClassifier$1.class
+-rw-rw-r--  2.0 unx     3672 b- defN 23-Jun-19 22:03 sklearn/calibration/CalibratedClassifierCV.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-19 22:03 sklearn/pipeline/PipelineTransformer.class
+-rw-rw-r--  2.0 unx     1671 b- defN 23-Jun-19 22:03 sklearn/pipeline/Pipeline$2.class
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-19 22:03 sklearn/pipeline/FeatureUnion.class
+-rw-rw-r--  2.0 unx     5062 b- defN 23-Jun-19 22:03 sklearn/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx     2003 b- defN 23-Jun-19 22:03 sklearn/pipeline/PipelineRegressor.class
+-rw-rw-r--  2.0 unx     1773 b- defN 23-Jun-19 22:03 sklearn/pipeline/Pipeline$1.class
+-rw-rw-r--  2.0 unx     1111 b- defN 23-Jun-19 22:03 sklearn/pipeline/PipelineUtil.class
+-rw-rw-r--  2.0 unx     2298 b- defN 23-Jun-19 22:03 sklearn/pipeline/PipelineClassifier.class
+-rw-rw-r--  2.0 unx     4913 b- defN 23-Jun-19 22:03 sklearn/dummy/DummyClassifier.class
+-rw-rw-r--  2.0 unx     2055 b- defN 23-Jun-19 22:03 sklearn/dummy/DummyRegressor.class
+-rw-rw-r--  2.0 unx      454 b- defN 23-Jun-19 22:03 sklearn/SkLearnFields.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Jun-19 22:03 sklearn/SkLearnOutlierTransformation.class
+-rw-rw-r--  2.0 unx      240 b- defN 23-Jun-19 22:03 sklearn/HasEstimator.class
+-rw-rw-r--  2.0 unx     3456 b- defN 23-Jun-19 22:03 sklearn/OutlierDetectorUtil.class
+-rw-rw-r--  2.0 unx     1258 b- defN 23-Jun-19 22:03 sklearn/HasMultiApplyField.class
+-rw-rw-r--  2.0 unx      908 b- defN 23-Jun-19 22:03 sklearn/None.class
+-rw-rw-r--  2.0 unx     2393 b- defN 23-Jun-19 22:03 sklearn/svm/SupportVectorMachineUtil.class
+-rw-rw-r--  2.0 unx     1109 b- defN 23-Jun-19 22:03 sklearn/svm/LinearSVC.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-Jun-19 22:03 sklearn/svm/LibSVMClassifier.class
+-rw-rw-r--  2.0 unx      966 b- defN 23-Jun-19 22:03 sklearn/svm/SupportVectorMachineUtil$1.class
+-rw-rw-r--  2.0 unx     1305 b- defN 23-Jun-19 22:03 sklearn/svm/OneClassSVM.class
+-rw-rw-r--  2.0 unx     3594 b- defN 23-Jun-19 22:03 sklearn/svm/LibSVMRegressor.class
+-rw-rw-r--  2.0 unx     4114 b- defN 23-Jun-19 22:03 sklearn/InitializerUtil$1.class
+-rw-rw-r--  2.0 unx      735 b- defN 23-Jun-19 22:03 sklearn/Estimator$1.class
+-rw-rw-r--  2.0 unx      342 b- defN 23-Jun-19 22:03 sklearn/HasOutlierField.class
+-rw-rw-r--  2.0 unx      214 b- defN 23-Jun-19 22:03 sklearn/HasNumberOfFeatures.class
+-rw-rw-r--  2.0 unx      660 b- defN 23-Jun-19 22:03 sklearn/MultiTransformer.class
+-rw-rw-r--  2.0 unx     2110 b- defN 23-Jun-19 22:03 sklearn/neural_network/MLPRegressor.class
+-rw-rw-r--  2.0 unx     2555 b- defN 23-Jun-19 22:03 sklearn/neural_network/MLPClassifier.class
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jun-19 22:03 sklearn/neural_network/MultilayerPerceptronUtil$1.class
+-rw-rw-r--  2.0 unx    10661 b- defN 23-Jun-19 22:03 sklearn/neural_network/MultilayerPerceptronUtil.class
+-rw-rw-r--  2.0 unx      853 b- defN 23-Jun-19 22:03 sklearn/Step.class
+-rw-rw-r--  2.0 unx      168 b- defN 23-Jun-19 22:03 sklearn/HasDefaultValue.class
+-rw-rw-r--  2.0 unx     2936 b- defN 23-Jun-19 22:03 sklearn/impute/MissingIndicator.class
+-rw-rw-r--  2.0 unx     4027 b- defN 23-Jun-19 22:03 sklearn/impute/ImputerUtil.class
+-rw-rw-r--  2.0 unx     5703 b- defN 23-Jun-19 22:03 sklearn/impute/SimpleImputer.class
+-rw-rw-r--  2.0 unx     6948 b- defN 23-Jun-19 22:03 sklearn/naive_bayes/GaussianNB.class
+-rw-rw-r--  2.0 unx     4434 b- defN 23-Jun-19 22:03 sklearn/linear_model/LinearRegressor.class
+-rw-rw-r--  2.0 unx     5040 b- defN 23-Jun-19 22:03 sklearn/linear_model/LinearClassifier.class
+-rw-rw-r--  2.0 unx     7648 b- defN 23-Jun-19 22:03 sklearn/linear_model/logistic/LogisticRegression.class
+-rw-rw-r--  2.0 unx     1042 b- defN 23-Jun-19 22:03 sklearn/linear_model/ridge/RidgeClassifier.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jun-19 22:03 sklearn/linear_model/glm/DistributionBoundary.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Jun-19 22:03 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/Hinge.class
+-rw-rw-r--  2.0 unx     2480 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
+-rw-rw-r--  2.0 unx      461 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/LossFunction.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/Log.class
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
+-rw-rw-r--  2.0 unx      482 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
+-rw-rw-r--  2.0 unx      932 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
+-rw-rw-r--  2.0 unx     1720 b- defN 23-Jun-19 22:03 sklearn/compose/ColumnTransformer$1.class
+-rw-rw-r--  2.0 unx     3239 b- defN 23-Jun-19 22:03 sklearn/compose/TransformedTargetRegressor.class
+-rw-rw-r--  2.0 unx     3649 b- defN 23-Jun-19 22:03 sklearn/compose/ColumnTransformer.class
+-rw-rw-r--  2.0 unx     1534 b- defN 23-Jun-19 22:03 sklearn/compose/TransformedTargetRegressor$1.class
+-rw-rw-r--  2.0 unx     4089 b- defN 23-Jun-19 22:03 sklearn/Classifier.class
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Jun-19 22:03 sklearn/model_selection/EstimatorSearcher.class
+-rw-rw-r--  2.0 unx     1685 b- defN 23-Jun-19 22:03 sklearn/Selector.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-Jun-19 22:03 sklearn/decomposition/IncrementalPCA.class
+-rw-rw-r--  2.0 unx     3471 b- defN 23-Jun-19 22:03 sklearn/decomposition/TruncatedSVD.class
+-rw-rw-r--  2.0 unx     4759 b- defN 23-Jun-19 22:03 sklearn/decomposition/PCA.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jun-19 22:03 sklearn/decomposition/BasePCA.class
+-rw-rw-r--  2.0 unx      336 b- defN 23-Jun-19 22:03 sklearn/HasPredictField.class
+-rw-rw-r--  2.0 unx     3018 b- defN 23-Jun-19 22:03 sklearn/neighbors/NearestNeighbors.class
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-19 22:03 sklearn/neighbors/KNeighborsClassifier.class
+-rw-rw-r--  2.0 unx     3794 b- defN 23-Jun-19 22:03 sklearn/neighbors/NearestCentroid.class
+-rw-rw-r--  2.0 unx     2025 b- defN 23-Jun-19 22:03 sklearn/neighbors/BinaryTree.class
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Jun-19 22:03 sklearn/neighbors/KNeighborsUtil$1.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jun-19 22:03 sklearn/neighbors/HasMetric.class
+-rw-rw-r--  2.0 unx    10733 b- defN 23-Jun-19 22:03 sklearn/neighbors/KNeighborsUtil.class
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Jun-19 22:03 sklearn/neighbors/KNeighborsRegressor.class
+-rw-rw-r--  2.0 unx     1032 b- defN 23-Jun-19 22:03 sklearn/neighbors/DistanceMetric.class
+-rw-rw-r--  2.0 unx      351 b- defN 23-Jun-19 22:03 sklearn/neighbors/HasTrainingData.class
+-rw-rw-r--  2.0 unx      176 b- defN 23-Jun-19 22:03 sklearn/neighbors/HasNumberOfNeighbors.class
+-rw-rw-r--  2.0 unx     2654 b- defN 23-Jun-19 22:03 sklearn/multioutput/MultiOutputUtil.class
+-rw-rw-r--  2.0 unx     3510 b- defN 23-Jun-19 22:03 sklearn/multioutput/ChainUtil.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Jun-19 22:03 sklearn/multioutput/RegressorChain.class
+-rw-rw-r--  2.0 unx     1316 b- defN 23-Jun-19 22:03 sklearn/multioutput/MultiOutputClassifier.class
+-rw-rw-r--  2.0 unx     1310 b- defN 23-Jun-19 22:03 sklearn/multioutput/MultiOutputRegressor.class
+-rw-rw-r--  2.0 unx     1745 b- defN 23-Jun-19 22:03 sklearn/multioutput/ClassifierChain.class
+-rw-rw-r--  2.0 unx     4450 b- defN 23-Jun-19 22:03 sklearn/isotonic/IsotonicRegression.class
+-rw-rw-r--  2.0 unx      326 b- defN 23-Jun-19 22:03 sklearn/HasApplyField.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jun-19 22:03 sklearn/HasEstimatorEnsemble.class
+-rw-rw-r--  2.0 unx     1929 b- defN 23-Jun-19 22:03 sklearn/Transformer$1.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-Jun-19 22:03 sklearn/LabelEncoderClassifier.class
+-rw-rw-r--  2.0 unx      937 b- defN 23-Jun-19 22:03 sklearn/PassThrough.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jun-19 22:03 sklearn/HasPriorProbability.class
+-rw-rw-r--  2.0 unx     5693 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/TfidfVectorizer.class
+-rw-rw-r--  2.0 unx      809 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/TfidfVectorizer$1.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/Tokenizer.class
+-rw-rw-r--  2.0 unx    13329 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/CountVectorizer.class
+-rw-rw-r--  2.0 unx     2129 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/CountVectorizer$1.class
+-rw-rw-r--  2.0 unx     1433 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/TfidfTransformer.class
+-rw-rw-r--  2.0 unx     4031 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/DictVectorizer.class
+-rw-rw-r--  2.0 unx      762 b- defN 23-Jun-19 22:03 sklearn/Clusterer.class
+-rw-rw-r--  2.0 unx     1375 b- defN 23-Jun-19 22:03 sklearn/metrics/DistanceMetric.class
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-19 22:03 sklearn/ensemble/EnsembleUtil.class
+-rw-rw-r--  2.0 unx     2112 b- defN 23-Jun-19 22:03 sklearn/ensemble/bagging/BaggingRegressor.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-Jun-19 22:03 sklearn/ensemble/bagging/BaggingUtil.class
+-rw-rw-r--  2.0 unx     3031 b- defN 23-Jun-19 22:03 sklearn/ensemble/bagging/BaggingClassifier.class
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Jun-19 22:03 sklearn/ensemble/EnsembleRegressor.class
+-rw-rw-r--  2.0 unx     3485 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingClassifier.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
+-rw-rw-r--  2.0 unx     3109 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingRegressor.class
+-rw-rw-r--  2.0 unx     3862 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingUtil.class
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingClassifier$1.class
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingRegressor$1.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
+-rw-rw-r--  2.0 unx     2563 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx      858 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/LossFunction.class
+-rw-rw-r--  2.0 unx     1588 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
+-rw-rw-r--  2.0 unx     1317 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
+-rw-rw-r--  2.0 unx     7948 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
+-rw-rw-r--  2.0 unx      960 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/MeanEstimator.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
+-rw-rw-r--  2.0 unx      811 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
+-rw-rw-r--  2.0 unx     3003 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
+-rw-rw-r--  2.0 unx     1148 b- defN 23-Jun-19 22:03 sklearn/ensemble/EnsembleUtil$1.class
+-rw-rw-r--  2.0 unx     3059 b- defN 23-Jun-19 22:03 sklearn/ensemble/forest/ForestUtil.class
+-rw-rw-r--  2.0 unx     2311 b- defN 23-Jun-19 22:03 sklearn/ensemble/forest/ForestRegressor.class
+-rw-rw-r--  2.0 unx     2770 b- defN 23-Jun-19 22:03 sklearn/ensemble/forest/ForestClassifier.class
+-rw-rw-r--  2.0 unx     1752 b- defN 23-Jun-19 22:03 sklearn/ensemble/iforest/IsolationForest$3.class
+-rw-rw-r--  2.0 unx     2206 b- defN 23-Jun-19 22:03 sklearn/ensemble/iforest/IsolationForest$1.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Jun-19 22:03 sklearn/ensemble/iforest/IsolationForest$2.class
+-rw-rw-r--  2.0 unx     8265 b- defN 23-Jun-19 22:03 sklearn/ensemble/iforest/IsolationForest.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Jun-19 22:03 sklearn/ensemble/voting/VotingClassifier.class
+-rw-rw-r--  2.0 unx     3716 b- defN 23-Jun-19 22:03 sklearn/ensemble/voting/VotingRegressor.class
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx     1247 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
+-rw-rw-r--  2.0 unx     6152 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
+-rw-rw-r--  2.0 unx      490 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
+-rw-rw-r--  2.0 unx     1572 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
+-rw-rw-r--  2.0 unx     6377 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     8868 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-19 22:03 sklearn/ensemble/EnsembleClassifier.class
+-rw-rw-r--  2.0 unx     3564 b- defN 23-Jun-19 22:03 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
+-rw-rw-r--  2.0 unx     6043 b- defN 23-Jun-19 22:03 sklearn/Transformer.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jun-19 22:03 sklearn/Transformer$1$1.class
+-rw-rw-r--  2.0 unx      981 b- defN 23-Jun-19 22:03 sklearn/Drop.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-19 22:03 sklearn/feature_selection/SelectKBest$Entry.class
+-rw-rw-r--  2.0 unx     3486 b- defN 23-Jun-19 22:03 sklearn/feature_selection/SelectFromModel.class
+-rw-rw-r--  2.0 unx     2922 b- defN 23-Jun-19 22:03 sklearn/feature_selection/SelectKBest.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Jun-19 22:03 sklearn/feature_selection/PySelector.class
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jun-19 22:03 sklearn/Transformer$2.class
+-rw-rw-r--  2.0 unx     2216 b- defN 23-Jun-19 22:03 sklearn/SkLearnUtil.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Jun-19 22:03 sklearn/loss/HalfMultinomialLoss.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Jun-19 22:03 sklearn/loss/CyLossFunction.class
+-rw-rw-r--  2.0 unx      403 b- defN 23-Jun-19 22:03 sklearn/loss/HalfBinomialLoss.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-Jun-19 22:03 sklearn/loss/BaseLoss.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-Jun-19 22:03 sklearn/HasDecisionFunctionField.class
+-rw-rw-r--  2.0 unx      338 b- defN 23-Jun-19 22:03 sklearn/SkLearnMethods.class
+-rw-rw-r--  2.0 unx     5114 b- defN 23-Jun-19 22:03 sklearn/ScalarLabelUtil.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Jun-19 22:03 sklearn/OutlierDetectorUtil$1.class
+-rw-rw-r--  2.0 unx      195 b- defN 23-Jun-19 22:03 sklearn/HasClasses.class
+-rw-rw-r--  2.0 unx     4685 b- defN 23-Jun-19 22:03 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
+-rw-rw-r--  2.0 unx      696 b- defN 23-Jun-19 22:03 sklearn/EstimatorUtil$1.class
+-rw-rw-r--  2.0 unx     3311 b- defN 23-Jun-19 22:03 sklearn/Composite.class
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Jun-19 22:03 sklearn/preprocessing/KBinsDiscretizer$1.class
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Jun-19 22:03 sklearn/preprocessing/PowerTransformer.class
+-rw-rw-r--  2.0 unx     2381 b- defN 23-Jun-19 22:03 sklearn/preprocessing/LabelEncoder.class
+-rw-rw-r--  2.0 unx     4924 b- defN 23-Jun-19 22:03 sklearn/preprocessing/LabelBinarizer.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Jun-19 22:03 sklearn/preprocessing/EncoderUtil$3.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-Jun-19 22:03 sklearn/preprocessing/Scaler.class
+-rw-rw-r--  2.0 unx     3242 b- defN 23-Jun-19 22:03 sklearn/preprocessing/MaxAbsScaler.class
+-rw-rw-r--  2.0 unx     2948 b- defN 23-Jun-19 22:03 sklearn/preprocessing/FunctionTransformer.class
+-rw-rw-r--  2.0 unx     3291 b- defN 23-Jun-19 22:03 sklearn/preprocessing/BaseEncoder.class
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Jun-19 22:03 sklearn/preprocessing/EncoderUtil$1.class
+-rw-rw-r--  2.0 unx     4549 b- defN 23-Jun-19 22:03 sklearn/preprocessing/StandardScaler.class
+-rw-rw-r--  2.0 unx     6971 b- defN 23-Jun-19 22:03 sklearn/preprocessing/EncoderUtil.class
+-rw-rw-r--  2.0 unx     6343 b- defN 23-Jun-19 22:03 sklearn/preprocessing/PolynomialFeatures.class
+-rw-rw-r--  2.0 unx     8486 b- defN 23-Jun-19 22:03 sklearn/preprocessing/KBinsDiscretizer.class
+-rw-rw-r--  2.0 unx     4671 b- defN 23-Jun-19 22:03 sklearn/preprocessing/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     2553 b- defN 23-Jun-19 22:03 sklearn/preprocessing/Binarizer.class
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Jun-19 22:03 sklearn/preprocessing/EncoderUtil$2.class
+-rw-rw-r--  2.0 unx     3595 b- defN 23-Jun-19 22:03 sklearn/preprocessing/MinMaxScaler.class
+-rw-rw-r--  2.0 unx     4467 b- defN 23-Jun-19 22:03 sklearn/preprocessing/RobustScaler.class
+-rw-rw-r--  2.0 unx     3740 b- defN 23-Jun-19 22:03 sklearn/preprocessing/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      957 b- defN 23-Jun-19 22:03 sklearn/preprocessing/Imputer.class
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Jun-19 22:03 sklearn/preprocessing/PolynomialFeatures$1.class
+-rw-rw-r--  2.0 unx     7408 b- defN 23-Jun-19 22:03 sklearn/preprocessing/MultiOneHotEncoder.class
+-rw-rw-r--  2.0 unx     2153 b- defN 23-Jun-19 22:03 sklearn/tree/TreeClassifier.class
+-rw-rw-r--  2.0 unx     3111 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$1.class
+-rw-rw-r--  2.0 unx     2664 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$4.class
+-rw-rw-r--  2.0 unx     4805 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelFlattener.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelCompactor$1.class
+-rw-rw-r--  2.0 unx     5431 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     2988 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelPruner.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelFlattener$1.class
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelPruner$1.class
+-rw-rw-r--  2.0 unx     1489 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$8.class
+-rw-rw-r--  2.0 unx      879 b- defN 23-Jun-19 22:03 sklearn/tree/RegressionCriterion.class
+-rw-rw-r--  2.0 unx     1151 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$5.class
+-rw-rw-r--  2.0 unx      978 b- defN 23-Jun-19 22:03 sklearn/tree/PresortBestSplitter.class
+-rw-rw-r--  2.0 unx      955 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$6.class
+-rw-rw-r--  2.0 unx     1764 b- defN 23-Jun-19 22:03 sklearn/tree/TreeRegressor.class
+-rw-rw-r--  2.0 unx     1589 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$7.class
+-rw-rw-r--  2.0 unx    20072 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$3.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-19 22:03 sklearn/tree/HasTreeOptions.class
+-rw-rw-r--  2.0 unx     2257 b- defN 23-Jun-19 22:03 sklearn/tree/Tree.class
+-rw-rw-r--  2.0 unx      754 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$2.class
+-rw-rw-r--  2.0 unx      150 b- defN 23-Jun-19 22:03 sklearn/tree/HasTree.class
+-rw-rw-r--  2.0 unx     1967 b- defN 23-Jun-19 22:03 sklearn/InitializerUtil.class
+-rw-rw-r--  2.0 unx      570 b- defN 23-Jun-19 22:03 sklearn/Regressor.class
+-rw-rw-r--  2.0 unx      211 b- defN 23-Jun-19 22:03 sklearn/HasNumberOfOutputs.class
+-rw-rw-r--  2.0 unx      494 b- defN 23-Jun-19 22:03 sklearn/OutlierDetector.class
+-rw-rw-r--  2.0 unx     2808 b- defN 23-Jun-19 22:03 sklearn/Calibrator.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jun-19 22:03 sklearn/HasClassifierOptions.class
+-rw-rw-r--  2.0 unx     7075 b- defN 23-Jun-19 22:03 sklearn/EstimatorUtil.class
+-rw-rw-r--  2.0 unx      199 b- defN 23-Jun-19 22:03 sklearn/HasType.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Jun-19 22:03 sklearn/cluster/MiniBatchKMeans.class
+-rw-rw-r--  2.0 unx     5086 b- defN 23-Jun-19 22:03 sklearn/cluster/KMeans.class
+-rw-rw-r--  2.0 unx    12903 b- defN 23-Jun-19 22:03 sklearn/Estimator.class
+-rw-rw-r--  2.0 unx     1624 b- defN 23-Jun-19 22:03 sklearn/Initializer.class
+-rw-rw-r--  2.0 unx     4598 b- defN 23-Jun-19 22:03 sklearn/multiclass/OneVsRestClassifier.class
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Jun-19 22:03 sklearn2pmml/ruleset/RuleSetClassifier.class
+-rw-rw-r--  2.0 unx     1023 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/PMMLPipeline$3.class
+-rw-rw-r--  2.0 unx    26752 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/PMMLPipeline.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/PMMLPipeline$2.class
+-rw-rw-r--  2.0 unx     1421 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/PMMLPipeline$1.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/Verification.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/MultiDomain.class
+-rw-rw-r--  2.0 unx     1152 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/ContinuousDomainEraser.class
+-rw-rw-r--  2.0 unx     1654 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Alias.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/TemporalDomain.class
+-rw-rw-r--  2.0 unx      779 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/ContinuousDomain$1.class
+-rw-rw-r--  2.0 unx    11878 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain.class
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/MultiAlias.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DiscreteDomain.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/CategoricalDomain.class
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DomainEraser.class
+-rw-rw-r--  2.0 unx      613 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DateTimeDomain.class
+-rw-rw-r--  2.0 unx     7764 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/ContinuousDomain.class
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DiscreteDomainEraser.class
+-rw-rw-r--  2.0 unx     1590 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     1045 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain$2.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DateDomain.class
+-rw-rw-r--  2.0 unx     3544 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DomainUtil.class
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain$1.class
+-rw-rw-r--  2.0 unx     1577 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/OrdinalDomain.class
+-rw-rw-r--  2.0 unx      672 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain$4.class
+-rw-rw-r--  2.0 unx      799 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain$3.class
+-rw-rw-r--  2.0 unx     7862 b- defN 23-Jun-19 22:03 sklearn2pmml/neural_network/MLPTransformer.class
+-rw-rw-r--  2.0 unx      391 b- defN 23-Jun-19 22:03 sklearn2pmml/SkLearn2PMMLFields.class
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Evaluatable.class
+-rw-rw-r--  2.0 unx     1196 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Expression.class
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Predicate.class
+-rw-rw-r--  2.0 unx     1434 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Reshaper.class
+-rw-rw-r--  2.0 unx     3392 b- defN 23-Jun-19 22:03 sklearn2pmml/util/EvaluatableUtil.class
+-rw-rw-r--  2.0 unx     1658 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Slicer.class
+-rw-rw-r--  2.0 unx     2418 b- defN 23-Jun-19 22:03 sklearn2pmml/feature_extraction/text/Splitter.class
+-rw-rw-r--  2.0 unx     3184 b- defN 23-Jun-19 22:03 sklearn2pmml/feature_extraction/text/Matcher.class
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/SelectFirstRegressor.class
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTUtil$2.class
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTLMRegressor.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTUtil$1.class
+-rw-rw-r--  2.0 unx     7398 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/EstimatorChain.class
+-rw-rw-r--  2.0 unx     6582 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTUtil.class
+-rw-rw-r--  2.0 unx     3995 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/Link.class
+-rw-rw-r--  2.0 unx     4360 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/SelectFirstUtil.class
+-rw-rw-r--  2.0 unx     4252 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTLRClassifier.class
+-rw-rw-r--  2.0 unx     2608 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/SelectFirstClassifier.class
+-rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-19 22:03 sklearn2pmml/EstimatorProxy$1.class
+-rw-rw-r--  2.0 unx      946 b- defN 23-Jun-19 22:03 sklearn2pmml/feature_selection/SelectUnique.class
+-rw-rw-r--  2.0 unx     6477 b- defN 23-Jun-19 22:03 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jun-19 22:03 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
+-rw-rw-r--  2.0 unx     1197 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/PatternTransformer.class
+-rw-rw-r--  2.0 unx     2908 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/ReplaceTransformer.class
+-rw-rw-r--  2.0 unx     1844 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/WordCountTransformer.class
+-rw-rw-r--  2.0 unx      597 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/DateTimeFormatter.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
+-rw-rw-r--  2.0 unx     4621 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/DurationTransformer.class
+-rw-rw-r--  2.0 unx      444 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/FilterLookupTransformer.class
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/Formatter.class
+-rw-rw-r--  2.0 unx     3424 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/CastTransformer.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/MatchesTransformer.class
+-rw-rw-r--  2.0 unx      589 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/NumberFormatter.class
+-rw-rw-r--  2.0 unx     4149 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/MultiLookupTransformer.class
+-rw-rw-r--  2.0 unx     3871 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/StringNormalizer.class
+-rw-rw-r--  2.0 unx     7145 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/ExpressionTransformer.class
+-rw-rw-r--  2.0 unx      635 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     3604 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/DataFrameConstructor.class
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/ConcatTransformer.class
+-rw-rw-r--  2.0 unx     5993 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/CutTransformer.class
+-rw-rw-r--  2.0 unx     7025 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/BSplineTransformer.class
+-rw-rw-r--  2.0 unx     6410 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/LookupTransformer.class
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/SubstringTransformer.class
+-rw-rw-r--  2.0 unx     3181 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
+-rw-rw-r--  2.0 unx     2132 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
+-rw-rw-r--  2.0 unx     3328 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/Aggregator.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-Jun-19 22:03 sklearn2pmml/tree/CHAIDRegressor.class
+-rw-rw-r--  2.0 unx    10719 b- defN 23-Jun-19 22:03 sklearn2pmml/tree/CHAIDUtil.class
+-rw-rw-r--  2.0 unx     2121 b- defN 23-Jun-19 22:03 sklearn2pmml/tree/CHAIDClassifier.class
+-rw-rw-r--  2.0 unx     1417 b- defN 23-Jun-19 22:03 sklearn2pmml/tree/CHAIDUtil$1.class
+-rw-rw-r--  2.0 unx     3864 b- defN 23-Jun-19 22:03 sklearn2pmml/EstimatorProxy.class
+-rw-rw-r--  2.0 unx     1458 b- defN 23-Jun-19 22:03 sklearn2pmml/SelectorProxy.class
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionUtil.class
+-rw-rw-r--  2.0 unx     3799 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionRegressor.class
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionClassifier$1.class
+-rw-rw-r--  2.0 unx     8687 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionClassifier.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionUtil$1.class
+-rw-rw-r--  2.0 unx     1774 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2764 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
+-rw-rw-r--  2.0 unx    13608 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/SkLearnEncoder.class
+-rw-rw-r--  2.0 unx      194 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/FieldNames.class
+-rw-rw-r--  2.0 unx      171 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/HasSkLearnOptions.class
+-rw-rw-r--  2.0 unx     1030 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/SkLearnEncoder$1.class
+-rw-rw-r--  2.0 unx     1822 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
+403 files, 923637 bytes uncompressed, 406937 bytes compressed:  55.9%
```

#### zipnote «TEMP»/diffoscope_rvr563yz_/tmpmsog15fp_.zip

```diff
@@ -318,14 +318,17 @@
 
 Filename: sklearn/InitializerUtil$1.class
 Comment: 
 
 Filename: sklearn/Estimator$1.class
 Comment: 
 
+Filename: sklearn/HasOutlierField.class
+Comment: 
+
 Filename: sklearn/HasNumberOfFeatures.class
 Comment: 
 
 Filename: sklearn/MultiTransformer.class
 Comment: 
 
 Filename: sklearn/neural_network/MLPRegressor.class
@@ -1026,17 +1029,14 @@
 
 Filename: sklearn2pmml/ensemble/SelectFirstRegressor.class
 Comment: 
 
 Filename: sklearn2pmml/ensemble/GBDTUtil$2.class
 Comment: 
 
-Filename: sklearn2pmml/ensemble/EstimatorChain$1.class
-Comment: 
-
 Filename: sklearn2pmml/ensemble/GBDTLMRegressor.class
 Comment: 
 
 Filename: sklearn2pmml/ensemble/GBDTUtil$1.class
 Comment: 
 
 Filename: sklearn2pmml/ensemble/EstimatorChain.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-SkLearn library
-Implementation-Version: 1.7.29
+Implementation-Version: 1.7.30
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### sklearn/calibration/CalibratedClassifier.class

##### procyon -ec {}

```diff
@@ -1,27 +1,28 @@
 
 package sklearn.calibration;
 
 import sklearn.Estimator;
 import org.dmg.pmml.DerivedField;
+import org.jpmml.converter.FieldNameUtil;
+import java.util.Arrays;
 import org.dmg.pmml.ResultFeature;
 import java.util.Iterator;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
 import org.jpmml.converter.regression.RegressionModelUtil;
 import java.util.Collections;
 import sklearn.Calibrator;
 import org.jpmml.converter.SchemaUtil;
 import java.util.List;
 import org.jpmml.converter.Label;
 import org.dmg.pmml.Output;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
-import org.jpmml.converter.FieldNameUtil;
 import org.dmg.pmml.regression.RegressionTable;
 import org.dmg.pmml.Field;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.ContinuousFeature;
 import com.google.common.collect.Iterables;
 import org.dmg.pmml.OutputField;
 import org.dmg.pmml.MiningFunction;
@@ -69,15 +70,15 @@
         }
         switch (n) {
             case 0:
             case 1: {
                 final SkLearnEncoder encoder = (SkLearnEncoder)schema.getEncoder();
                 final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
                 final List<? extends Feature> features = schema.getFeatures();
-                final Model model = estimator.encodeModel(schema);
+                final Model model = estimator.encode(schema);
                 final List<Model> models = new ArrayList<Model>();
                 List<Feature> decisionFunctionFeatures = new ArrayList<Feature>();
                 if (estimator instanceof LinearClassifier) {
                     if (model instanceof MiningModel) {
                         final MiningModel miningModel = (MiningModel)model;
                         final Segmentation segmentation = miningModel.requireSegmentation();
                         final List<Segment> segments = segmentation.requireSegments();
@@ -87,14 +88,15 @@
                                 continue;
                             }
                             final Output output = decisionFunctionModel.getOutput();
                             if (output == null) {
                                 throw new IllegalArgumentException();
                             }
                             final OutputField outputField = (OutputField)Iterables.getOnlyElement((Iterable)output.getOutputFields());
+                            outputField.setName(this.getDecisionFunctionField((Object)outputField.getName()));
                             decisionFunctionModel.setNormalizationMethod(RegressionModel.NormalizationMethod.NONE);
                             models.add((Model)decisionFunctionModel);
                             decisionFunctionFeatures.add((Feature)new ContinuousFeature((PMMLEncoder)encoder, (Field)outputField));
                         }
                     }
                     else {
                         if (!(model instanceof RegressionModel)) {
@@ -102,15 +104,15 @@
                         }
                         final RegressionModel regressionModel = (RegressionModel)model;
                         List<RegressionTable> regressionTables = regressionModel.getRegressionTables();
                         if (categoricalLabel.size() == 2) {
                             regressionTables = regressionTables.subList(0, 1);
                         }
                         for (final RegressionTable regressionTable : regressionTables) {
-                            final OutputField outputField2 = ModelUtil.createPredictedField(FieldNameUtil.create("decisionFunction", new Object[] { regressionTable.requireTargetCategory() }), OpType.CONTINUOUS, DataType.DOUBLE).setFinalResult(Boolean.valueOf(false));
+                            final OutputField outputField2 = ModelUtil.createPredictedField(this.getDecisionFunctionField(regressionTable.requireTargetCategory()), OpType.CONTINUOUS, DataType.DOUBLE).setFinalResult(Boolean.valueOf(false));
                             final Output output2 = new Output().addOutputFields(new OutputField[] { outputField2 });
                             regressionTable.setTargetCategory((Object)null);
                             final Model decisionFunctionModel2 = (Model)new RegressionModel(MiningFunction.REGRESSION, ModelUtil.createMiningSchema((Label)null), (List)null).setNormalizationMethod(RegressionModel.NormalizationMethod.NONE).addRegressionTables(new RegressionTable[] { regressionTable }).setOutput(output2);
                             models.add(decisionFunctionModel2);
                             decisionFunctionFeatures.add((Feature)new ContinuousFeature((PMMLEncoder)encoder, (Field)outputField2));
                         }
                     }
@@ -121,15 +123,15 @@
                         throw new IllegalArgumentException();
                     }
                     final List<OutputField> outputFields = output3.getOutputFields();
                     for (final OutputField outputField3 : outputFields) {
                         final ResultFeature resultFeature = outputField3.getResultFeature();
                         switch (CalibratedClassifier.CalibratedClassifier$1.$SwitchMap$org$dmg$pmml$ResultFeature[resultFeature.ordinal()]) {
                             case 1: {
-                                outputField3.setName(FieldNameUtil.create("decisionFunction", new Object[] { outputField3.getValue() }));
+                                outputField3.setName(this.getDecisionFunctionField(outputField3.getValue()));
                                 decisionFunctionFeatures.add((Feature)new ContinuousFeature((PMMLEncoder)encoder, (Field)outputField3));
                                 continue;
                             }
                         }
                     }
                     models.add(model);
                     if (categoricalLabel.size() == 2) {
@@ -185,14 +187,30 @@
         return (Classifier)this.get("estimator", (Class)Classifier.class);
     }
     
     public String getMethod() {
         return this.getString("method");
     }
     
+    private String getDecisionFunctionField(Object value) {
+        final Object segmentId = this.getPMMLSegmentId();
+        if (value instanceof String) {
+            final String name = (String)value;
+            value = extractArguments("decisionFunction", name);
+        }
+        List<?> args;
+        if (segmentId != null) {
+            args = Arrays.asList(segmentId, value);
+        }
+        else {
+            args = Arrays.asList(value);
+        }
+        return FieldNameUtil.create("decisionFunction", (List)args);
+    }
+    
     private static Feature calibrate(final Calibrator calibrator, final Model model, final Feature feature, final SkLearnEncoder encoder) {
         encoder.export(model, feature.getName());
         final Feature calibratedFeature = (Feature)Iterables.getOnlyElement((Iterable)calibrator.encodeFeatures((List)Collections.singletonList(feature), encoder));
         DerivedField derivedField = encoder.removeDerivedField(calibratedFeature.getName());
         final OutputField outputField = new OutputField(derivedField.requireName(), derivedField.requireOpType(), derivedField.requireDataType()).setResultFeature(ResultFeature.TRANSFORMED_VALUE).setExpression(derivedField.requireExpression()).setFinalResult(Boolean.valueOf(false));
         derivedField = (DerivedField)encoder.createDerivedField(model, outputField, true);
         return (Feature)new ContinuousFeature((PMMLEncoder)encoder, (Field)derivedField);
```

#### sklearn/calibration/SigmoidCalibration.class

##### procyon -ec {}

```diff
@@ -27,15 +27,15 @@
     public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
         final Number a = this.getA();
         final Number b = this.getB();
         SchemaUtil.checkSize(1, (List)features);
         final Feature feature = (Feature)features.get(0);
         Apply apply = PMMLUtil.createApply("*", new Expression[] { (Expression)PMMLUtil.createConstant((Number)Integer.valueOf(-1)), (Expression)PMMLUtil.createApply("+", new Expression[] { (Expression)PMMLUtil.createApply("*", new Expression[] { (Expression)PMMLUtil.createConstant(a), (Expression)feature.ref() }), (Expression)PMMLUtil.createConstant(b) }) });
         apply = FunctionUtil.encodeScipyFunction("scipy.special", "expit", (List)Collections.singletonList(apply));
-        final DerivedField derivedField = encoder.createDerivedField(this.createFieldName("sigmoidCalibration", new Object[] { feature }), OpType.CONTINUOUS, DataType.DOUBLE, (Expression)apply);
+        final DerivedField derivedField = encoder.createDerivedField(this.createFieldName("sigmoidCalibration", feature), OpType.CONTINUOUS, DataType.DOUBLE, (Expression)apply);
         return Collections.singletonList((Feature)new ContinuousFeature((PMMLEncoder)encoder, (Field)derivedField));
     }
     
     public Number getA() {
         return this.getNumber("a_");
     }
```

#### sklearn/calibration/CalibratedClassifier$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum b89c1a7f33429046e53ef5fa587842c1d704630d209dc6feacf6f3f6ed2b91a1
+  SHA-256 checksum 1670b626a09c373e68fe2a8b786c375e2aa8c614e27c520a609526eb68f2296a
   Compiled from "CalibratedClassifier.java"
 class sklearn.calibration.CalibratedClassifier$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #6                          // sklearn/calibration/CalibratedClassifier$1
   super_class: #7                         // java/lang/Object
@@ -67,15 +67,15 @@
         20: goto          24
         23: astore_0
         24: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 162: 0
+        line 166: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 2
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
 }
```

#### sklearn/calibration/CalibratedClassifierCV.class

##### procyon -ec {}

```diff
@@ -1,29 +1,48 @@
 
 package sklearn.calibration;
 
+import org.dmg.pmml.DataType;
 import java.util.List;
+import org.jpmml.converter.mining.MiningModelUtil;
+import org.dmg.pmml.mining.Segmentation;
+import org.dmg.pmml.mining.MiningModel;
+import org.jpmml.converter.Label;
+import org.jpmml.converter.ModelUtil;
+import org.dmg.pmml.MiningFunction;
+import java.util.ArrayList;
+import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import sklearn.Classifier;
 
 public class CalibratedClassifierCV extends Classifier
 {
     public CalibratedClassifierCV(final String module, final String name) {
         super(module, name);
     }
     
     public Model encodeModel(final Schema schema) {
         final List<CalibratedClassifier> calibratedClassifiers = this.getCalibratedClassifiers();
+        final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         if (calibratedClassifiers.size() == 1) {
             final CalibratedClassifier calibratedClassifier = (CalibratedClassifier)calibratedClassifiers.get(0);
             return calibratedClassifier.encode(schema);
         }
         if (calibratedClassifiers.size() >= 2) {
-            throw new IllegalArgumentException();
+            final Schema segmentSchema = schema.toAnonymousSchema();
+            final List<Model> models = new ArrayList<Model>();
+            for (int i = 0; i < calibratedClassifiers.size(); ++i) {
+                final CalibratedClassifier calibratedClassifier2 = (CalibratedClassifier)calibratedClassifiers.get(i);
+                final Model model = calibratedClassifier2.encode((Object)Integer.valueOf(i + 1), segmentSchema);
+                models.add(model);
+            }
+            final MiningModel miningModel = new MiningModel(MiningFunction.CLASSIFICATION, ModelUtil.createMiningSchema((Label)categoricalLabel)).setSegmentation(MiningModelUtil.createSegmentation(Segmentation.MultipleModelMethod.AVERAGE, Segmentation.MissingPredictionTreatment.RETURN_MISSING, (List)models));
+            this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
+            return (Model)miningModel;
         }
         throw new IllegalArgumentException();
     }
     
     public List<CalibratedClassifier> getCalibratedClassifiers() {
         return this.getList("calibrated_classifiers_", (Class)CalibratedClassifier.class);
     }
```

#### sklearn/neural_network/MultilayerPerceptronUtil$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 0a9efc75148e7049d0c8e0ca63d6f95541e81fc771122eea9f6d3af33b1ba65a
+  SHA-256 checksum 51075413df8f9780359ddcc50dd6872aa22432064e0d2e56be70320bd2b876a9
   Compiled from "MultilayerPerceptronUtil.java"
 class sklearn.neural_network.MultilayerPerceptronUtil$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #7                          // sklearn/neural_network/MultilayerPerceptronUtil$1
   super_class: #8                         // java/lang/Object
@@ -78,15 +78,15 @@
         38: astore_0
         39: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 140: 0
+        line 138: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 4
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### sklearn/neural_network/MultilayerPerceptronUtil.class

##### procyon -ec {}

```diff
@@ -2,19 +2,15 @@
 package sklearn.neural_network;
 
 import org.dmg.pmml.neural_network.NeuralOutput;
 import org.dmg.pmml.Expression;
 import org.dmg.pmml.DerivedField;
 import org.dmg.pmml.FieldRef;
 import org.dmg.pmml.OpType;
-import java.util.stream.Collector;
-import java.util.stream.Collectors;
-import java.util.function.Function;
-import org.jpmml.converter.MultiLabel;
-import java.util.Collections;
+import sklearn.ScalarLabelUtil;
 import org.jpmml.converter.ContinuousLabel;
 import org.jpmml.converter.CategoricalLabel;
 import com.google.common.collect.Iterables;
 import org.dmg.pmml.neural_network.NeuralEntity;
 import org.dmg.pmml.neural_network.Neuron;
 import org.jpmml.converter.CMatrixUtil;
 import java.util.ArrayList;
@@ -166,32 +162,20 @@
             default: {
                 throw new IllegalArgumentException(activation);
             }
         }
     }
     
     private static NeuralOutputs encodeRegressionNeuralOutputs(final List<? extends NeuralEntity> entities, final Label label) {
-        List<ContinuousLabel> continuousLabels;
-        if (entities.size() == 1) {
-            final ContinuousLabel continuousLabel = (ContinuousLabel)label;
-            continuousLabels = Collections.singletonList(continuousLabel);
-        }
-        else {
-            if (entities.size() < 2) {
-                throw new IllegalArgumentException();
-            }
-            final MultiLabel multiLabel = (MultiLabel)label;
-            final List<? extends Label> labels = multiLabel.getLabels();
-            continuousLabels = labels.stream().map((Function<? super Object, ?>)ContinuousLabel.class::cast).collect((Collector<? super Object, ?, List<ContinuousLabel>>)Collectors.toList());
-        }
+        final List<ContinuousLabel> continuousLabels = ScalarLabelUtil.toScalarLabels((Class)ContinuousLabel.class, label);
         ClassDictUtil.checkSize(new Collection[] { entities, continuousLabels });
         final NeuralOutputs neuralOutputs = new NeuralOutputs();
         for (int i = 0; i < entities.size(); ++i) {
             final NeuralEntity entity = (NeuralEntity)entities.get(i);
-            final ContinuousLabel continuousLabel2 = (ContinuousLabel)continuousLabels.get(i);
-            final DerivedField derivedField = new DerivedField((String)null, OpType.CONTINUOUS, continuousLabel2.getDataType(), (Expression)new FieldRef(continuousLabel2.getName()));
+            final ContinuousLabel continuousLabel = (ContinuousLabel)continuousLabels.get(i);
+            final DerivedField derivedField = new DerivedField((String)null, OpType.CONTINUOUS, continuousLabel.getDataType(), (Expression)new FieldRef(continuousLabel.getName()));
             final NeuralOutput neuralOutput = new NeuralOutput().setOutputNeuron(entity.requireId()).setDerivedField(derivedField);
             neuralOutputs.addNeuralOutputs(new NeuralOutput[] { neuralOutput });
         }
         return neuralOutputs;
     }
 }
```

#### sklearn/Step.class

##### procyon -ec {}

```diff
@@ -1,38 +1,18 @@
 
 package sklearn;
 
-import org.jpmml.converter.FieldNameUtil;
-import java.util.List;
-import java.util.Arrays;
-import org.dmg.pmml.DataType;
 import org.jpmml.python.PythonObject;
 
 public abstract class Step extends PythonObject implements HasNumberOfFeatures, HasType
 {
     public Step(final String module, final String name) {
         super(module, name);
     }
     
-    public String createFieldName(final DataType dataType, final Object... args) {
-        return this.createFieldName(dataType.name().toLowerCase(), args);
-    }
-    
-    public String createFieldName(final String function, final Object... args) {
-        return this.createFieldName(function, Arrays.asList(args));
-    }
-    
-    public String createFieldName(final String function, final List<?> args) {
-        final String pmmlName = this.getPMMLName();
-        if (pmmlName != null) {
-            return pmmlName;
-        }
-        return FieldNameUtil.create(function, (List)args);
-    }
-    
     public String getPMMLName() {
         return this.getOptionalString("pmml_name_");
     }
     
     public Step setPMMLName(final String name) {
         this.put((Object)"pmml_name_", (Object)name);
         return this;
```

#### sklearn/linear_model/LinearRegressor.class

##### procyon -ec {}

```diff
@@ -1,22 +1,23 @@
 
 package sklearn.linear_model;
 
 import org.jpmml.converter.regression.RegressionModelUtil;
 import org.dmg.pmml.regression.RegressionModel;
+import org.jpmml.converter.ScalarLabel;
 import org.jpmml.converter.Feature;
-import org.jpmml.converter.Label;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
 import java.util.List;
 import org.jpmml.converter.CMatrixUtil;
+import org.jpmml.converter.Label;
 import java.util.ArrayList;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
-import org.jpmml.converter.MultiLabel;
+import sklearn.ScalarLabelUtil;
 import com.google.common.collect.Iterables;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import sklearn.Regressor;
 
 public class LinearRegressor extends Regressor
 {
@@ -46,19 +47,19 @@
         final Label label = schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
         final int numberOfOutputs = this.getNumberOfOutputs();
         if (numberOfOutputs == 1) {
             return (Model)this.createRegression(coef, (Number)Iterables.getOnlyElement((Iterable)intercept), schema);
         }
         if (numberOfOutputs >= 2) {
-            final MultiLabel multiLabel = (MultiLabel)label;
-            ClassDictUtil.checkSize(numberOfOutputs, new Collection[] { intercept, multiLabel.getLabels() });
+            final List<ScalarLabel> scalarLabels = ScalarLabelUtil.toScalarLabels(label);
+            ClassDictUtil.checkSize(numberOfOutputs, new Collection[] { intercept, scalarLabels });
             final List<Model> models = new ArrayList<Model>();
             for (int i = 0, max = numberOfOutputs; i < max; ++i) {
-                final Schema segmentSchema = schema.toRelabeledSchema(multiLabel.getLabel(i));
+                final Schema segmentSchema = schema.toRelabeledSchema((Label)scalarLabels.get(i));
                 final Model model = (Model)this.createRegression(CMatrixUtil.getRow((List)coef, numberOfOutputs, features.size(), i), (Number)intercept.get(i), segmentSchema);
                 models.add(model);
             }
             return (Model)MiningModelUtil.createMultiModelChain((List)models, Segmentation.MissingPredictionTreatment.CONTINUE);
         }
         throw new IllegalArgumentException();
     }
```

#### sklearn/neighbors/KNeighborsUtil$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum fe599d56f633bbddd641c0a9775b51e44d28af8812e22ef1887f913cd3d7a687
+  SHA-256 checksum 4b6860fe2468f99e1d416cb880570c85ea6eac8357de083469a54eb63f8b85c8
   Compiled from "KNeighborsUtil.java"
 final class sklearn.neighbors.KNeighborsUtil$1 extends java.lang.Object implements com.google.common.base.Function<java.lang.Number, java.lang.Object>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #7                          // sklearn/neighbors/KNeighborsUtil$1
   super_class: #8                         // java/lang/Object
@@ -75,15 +75,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field val$categoricalLabel:Lorg/jpmml/converter/CategoricalLabel;
          5: aload_0
          6: invokespecial #2                  // Method java/lang/Object."<init>":()V
          9: return
       LineNumberTable:
-        line 281: 0
+        line 279: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lsklearn/neighbors/KNeighborsUtil$1;
 
   public java.lang.Object apply(java.lang.Number);
     descriptor: (Ljava/lang/Number;)Ljava/lang/Object;
     flags: (0x0001) ACC_PUBLIC
@@ -94,16 +94,16 @@
          4: istore_2
          5: aload_0
          6: getfield      #1                  // Field val$categoricalLabel:Lorg/jpmml/converter/CategoricalLabel;
          9: iload_2
         10: invokevirtual #4                  // Method org/jpmml/converter/CategoricalLabel.getValue:(I)Ljava/lang/Object;
         13: areturn
       LineNumberTable:
-        line 285: 0
-        line 287: 5
+        line 283: 0
+        line 285: 5
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      14     0  this   Lsklearn/neighbors/KNeighborsUtil$1;
             0      14     1 number   Ljava/lang/Number;
             5       9     2 index   I
 
   public java.lang.Object apply(java.lang.Object);
@@ -113,15 +113,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: checkcast     #5                  // class java/lang/Number
          5: invokevirtual #6                  // Method apply:(Ljava/lang/Number;)Ljava/lang/Object;
          8: areturn
       LineNumberTable:
-        line 281: 0
+        line 279: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/neighbors/KNeighborsUtil$1;
 }
 Signature: #28                          // Ljava/lang/Object;Lcom/google/common/base/Function<Ljava/lang/Number;Ljava/lang/Object;>;
 SourceFile: "KNeighborsUtil.java"
 EnclosingMethod: #32.#33                // sklearn.neighbors.KNeighborsUtil.translateValues
```

#### sklearn/neighbors/KNeighborsUtil.class

##### procyon -ec {}

```diff
@@ -21,16 +21,17 @@
 import org.dmg.pmml.nearest_neighbor.TrainingInstances;
 import java.util.Map;
 import org.jpmml.converter.PMMLUtil;
 import org.dmg.pmml.nearest_neighbor.KNNInput;
 import org.jpmml.converter.Feature;
 import org.dmg.pmml.nearest_neighbor.KNNInputs;
 import org.jpmml.converter.CMatrixUtil;
-import org.jpmml.converter.MultiLabel;
 import org.jpmml.converter.ScalarLabel;
+import java.util.Collections;
+import sklearn.ScalarLabelUtil;
 import org.dmg.pmml.nearest_neighbor.InstanceField;
 import org.dmg.pmml.nearest_neighbor.InstanceFields;
 import java.util.List;
 import java.util.LinkedHashMap;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import org.dmg.pmml.nearest_neighbor.NearestNeighborModel;
@@ -73,66 +74,62 @@
         final Map<String, List<?>> data = new LinkedHashMap<String, List<?>>();
         final InstanceFields instanceFields = new InstanceFields();
         if (id != null) {
             final InstanceField instanceField = new InstanceField("id").setColumn("data:id");
             instanceFields.addInstanceFields(new InstanceField[] { instanceField });
             data.put(instanceField.getColumn(), id);
         }
-        if (numberOfOutputs == 0) {
-            if (label != null) {
-                throw new IllegalArgumentException();
-            }
-        }
-        else if (numberOfOutputs == 1) {
-            final ScalarLabel scalarLabel = (ScalarLabel)label;
-            if (scalarLabel != null) {
-                final InstanceField instanceField2 = new InstanceField(scalarLabel.getName()).setColumn("data:y");
-                instanceFields.addInstanceFields(new InstanceField[] { instanceField2 });
-                data.put(instanceField2.getColumn(), translateValues(scalarLabel, y));
-            }
-        }
-        else {
-            if (numberOfOutputs < 2) {
-                throw new IllegalArgumentException();
+        final List<ScalarLabel> scalarLabels = (label != null) ? ScalarLabelUtil.toScalarLabels(label) : Collections.emptyList();
+        ClassDictUtil.checkSize(numberOfOutputs, new Collection[] { scalarLabels });
+        if (numberOfOutputs != 0) {
+            if (numberOfOutputs == 1) {
+                final ScalarLabel scalarLabel = (ScalarLabel)scalarLabels.get(0);
+                if (scalarLabel != null) {
+                    final InstanceField instanceField2 = new InstanceField(scalarLabel.getName()).setColumn("data:y");
+                    instanceFields.addInstanceFields(new InstanceField[] { instanceField2 });
+                    data.put(instanceField2.getColumn(), translateValues(scalarLabel, y));
+                }
             }
-            final MultiLabel multiLabel = (MultiLabel)label;
-            final List<? extends Label> labels = multiLabel.getLabels();
-            for (int i = 0; i < labels.size(); ++i) {
-                final ScalarLabel scalarLabel2 = (ScalarLabel)labels.get(i);
-                if (scalarLabel2 != null) {
-                    final InstanceField instanceField3 = new InstanceField(scalarLabel2.getName()).setColumn("data:y" + String.valueOf(i + 1));
-                    instanceFields.addInstanceFields(new InstanceField[] { instanceField3 });
-                    data.put(instanceField3.getColumn(), translateValues(scalarLabel2, (List<? extends Number>)CMatrixUtil.getColumn((List)y, numberOfInstances, numberOfOutputs, i)));
+            else {
+                if (numberOfOutputs < 2) {
+                    throw new IllegalArgumentException();
+                }
+                for (int i = 0; i < scalarLabels.size(); ++i) {
+                    final ScalarLabel scalarLabel2 = (ScalarLabel)scalarLabels.get(i);
+                    if (scalarLabel2 != null) {
+                        final InstanceField instanceField3 = new InstanceField(scalarLabel2.getName()).setColumn("data:y" + String.valueOf(i + 1));
+                        instanceFields.addInstanceFields(new InstanceField[] { instanceField3 });
+                        data.put(instanceField3.getColumn(), translateValues(scalarLabel2, (List<? extends Number>)CMatrixUtil.getColumn((List)y, numberOfInstances, numberOfOutputs, i)));
+                    }
                 }
             }
         }
         final DataType dataType = estimator.getDataType();
         final KNNInputs knnInputs = new KNNInputs();
-        for (int i = 0; i < features.size(); ++i) {
-            final Feature feature = (Feature)features.get(i);
+        for (int j = 0; j < features.size(); ++j) {
+            final Feature feature = (Feature)features.get(j);
             final ContinuousFeature continuousFeature = feature.toContinuousFeature(dataType);
             final String name = continuousFeature.getName();
-            final InstanceField instanceField4 = new InstanceField(name).setColumn("data:x" + String.valueOf(i + 1));
+            final InstanceField instanceField4 = new InstanceField(name).setColumn("data:x" + String.valueOf(j + 1));
             instanceFields.addInstanceFields(new InstanceField[] { instanceField4 });
             final KNNInput knnInput = new KNNInput(name);
             knnInputs.addKNNInputs(new KNNInput[] { knnInput });
-            data.put(instanceField4.getColumn(), CMatrixUtil.getColumn((List)fitX, numberOfInstances, numberOfFeatures, i));
+            data.put(instanceField4.getColumn(), CMatrixUtil.getColumn((List)fitX, numberOfInstances, numberOfFeatures, j));
         }
         final TrainingInstances trainingInstances = new TrainingInstances(instanceFields, PMMLUtil.createInlineTable((Map)data)).setTransformed(Boolean.valueOf(true));
         final ComparisonMeasure comparisonMeasure = encodeComparisonMeasure(estimator);
         Output output;
         if (numberOfOutputs == 0 || numberOfOutputs == 1) {
             output = createOutput(numberOfNeighbors, null);
         }
         else {
             if (numberOfOutputs < 2) {
                 throw new IllegalArgumentException();
             }
-            final MultiLabel multiLabel2 = (MultiLabel)label;
-            output = createOutput(numberOfNeighbors, (ScalarLabel)multiLabel2.getLabel(0));
+            output = createOutput(numberOfNeighbors, scalarLabels.get(0));
         }
         final NearestNeighborModel nearestNeighborModel = new NearestNeighborModel(miningFunction, Integer.valueOf(numberOfNeighbors), ModelUtil.createMiningSchema(schema.getLabel()), trainingInstances, comparisonMeasure, knnInputs).setOutput(output);
         if (id != null) {
             nearestNeighborModel.setInstanceIdVariable("id");
         }
         return nearestNeighborModel;
     }
```

#### sklearn/multioutput/MultiOutputUtil.class

##### procyon -ec {}

```diff
@@ -1,36 +1,42 @@
 
 package sklearn.multioutput;
 
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
+import org.jpmml.converter.Label;
+import org.jpmml.converter.ScalarLabel;
 import java.util.ArrayList;
-import org.jpmml.converter.MultiLabel;
+import org.jpmml.python.ClassDictUtil;
+import java.util.Collection;
+import sklearn.ScalarLabelUtil;
 import org.dmg.pmml.Model;
 import sklearn.Estimator;
 import org.jpmml.converter.Schema;
 import java.util.List;
 
 public class MultiOutputUtil
 {
     private MultiOutputUtil() {
     }
     
     public static <E extends Estimator> Model encodeEstimators(final List<E> estimators, final Schema schema) {
         if (estimators.size() == 1) {
             final Estimator estimator = (E)estimators.get(0);
-            return estimator.encodeModel(schema);
+            return estimator.encode(schema);
         }
         if (estimators.size() >= 2) {
-            final MultiLabel multiLabel = (MultiLabel)schema.getLabel();
+            final List<ScalarLabel> scalarLabels = ScalarLabelUtil.toScalarLabels(schema.getLabel());
+            ClassDictUtil.checkSize(new Collection[] { estimators, scalarLabels });
             final List<Model> models = new ArrayList<Model>();
             for (int i = 0; i < estimators.size(); ++i) {
                 final E estimator2 = (E)estimators.get(i);
-                final Schema segmentSchema = schema.toRelabeledSchema(multiLabel.getLabel(i));
-                final Model model = estimator2.encodeModel(segmentSchema);
+                final ScalarLabel scalarLabel = (ScalarLabel)scalarLabels.get(i);
+                final Schema segmentSchema = schema.toRelabeledSchema((Label)scalarLabel);
+                final Model model = estimator2.encode((Object)scalarLabel.getName(), segmentSchema);
                 models.add(model);
             }
             return (Model)MiningModelUtil.createMultiModelChain((List)models, Segmentation.MissingPredictionTreatment.CONTINUE);
         }
         throw new IllegalArgumentException();
     }
 }
```

#### sklearn/multioutput/ChainUtil.class

##### procyon -ec {}

```diff
@@ -3,46 +3,46 @@
 
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segmentation;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.ScalarLabel;
 import org.jpmml.converter.Feature;
-import org.jpmml.converter.MultiLabel;
 import org.dmg.pmml.Model;
 import java.util.ArrayList;
-import org.jpmml.sklearn.SkLearnEncoder;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
+import sklearn.ScalarLabelUtil;
+import org.jpmml.sklearn.SkLearnEncoder;
 import org.dmg.pmml.mining.MiningModel;
 import sklearn.Estimator;
 import org.jpmml.converter.Schema;
 import java.util.List;
 
 public class ChainUtil
 {
     private ChainUtil() {
     }
     
     public static <E extends Estimator> MiningModel encodeChain(final List<E> estimators, final List<Integer> order, final Schema schema) {
-        ClassDictUtil.checkSize(new Collection[] { estimators, order });
         final SkLearnEncoder encoder = (SkLearnEncoder)schema.getEncoder();
         final Label label = schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
+        final List<ScalarLabel> scalarLabels = ScalarLabelUtil.toScalarLabels(label);
+        ClassDictUtil.checkSize(new Collection[] { estimators, order, scalarLabels });
         final List<Model> models = new ArrayList<Model>();
-        final MultiLabel multiLabel = (MultiLabel)label;
         final List<Feature> augmentedFeatures = new ArrayList<Feature>(features);
         for (int i = 0; i < estimators.size(); ++i) {
             final E estimator = (E)estimators.get(i);
+            final ScalarLabel scalarLabel = (ScalarLabel)scalarLabels.get(i);
             if (Integer.valueOf(order.get(i)) != i) {
                 throw new IllegalArgumentException();
             }
-            final ScalarLabel scalarLabel = (ScalarLabel)multiLabel.getLabel(i);
             final Schema segmentSchema = new Schema((PMMLEncoder)encoder, (Label)scalarLabel, (List)augmentedFeatures);
-            final Model model = estimator.encodeModel(segmentSchema);
+            final Model model = estimator.encode((Object)scalarLabel.getName(), segmentSchema);
             models.add(model);
             final Feature feature = encoder.exportPrediction(model, scalarLabel);
             augmentedFeatures.add(feature);
         }
         return MiningModelUtil.createMultiModelChain((List)models, Segmentation.MissingPredictionTreatment.CONTINUE);
     }
 }
```

#### sklearn/isotonic/IsotonicRegression.class

##### procyon -ec {}

```diff
@@ -36,15 +36,15 @@
         final OutlierTreatmentMethod outlierTreatment = parseOutlierTreatment(outOfBounds);
         final NormContinuous normContinuous = new NormContinuous(feature.getName(), (List)null).setOutliers(outlierTreatment);
         for (int i = 0; i < xThresholds.size(); ++i) {
             final Number orig = (Number)xThresholds.get(i);
             final Number norm = (Number)yThresholds.get(i);
             normContinuous.addLinearNorms(new LinearNorm[] { new LinearNorm(orig, norm) });
         }
-        final DerivedField derivedField = encoder.createDerivedField(this.createFieldName("isotonicRegression", new Object[] { feature }), OpType.CONTINUOUS, DataType.DOUBLE, (Expression)normContinuous);
+        final DerivedField derivedField = encoder.createDerivedField(this.createFieldName("isotonicRegression", feature), OpType.CONTINUOUS, DataType.DOUBLE, (Expression)normContinuous);
         return Collections.singletonList((Feature)new ContinuousFeature((PMMLEncoder)encoder, (Field)derivedField));
     }
     
     public Boolean getIncreasing() {
         return this.getBoolean("increasing_");
     }
```

#### sklearn/Transformer$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 9ded74bf333381e215171090cb2e25b42bf2663c7c19961805b4b1dbafdc7c96
+  SHA-256 checksum 6f49e09d673fe56a1d332a9609c909fb75a1bc9971746efcd5cc294b8479b409
   Compiled from "Transformer.java"
 class sklearn.Transformer$1 extends org.jpmml.python.CastFunction<org.jpmml.python.TypeInfo>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #18                         // sklearn/Transformer$1
   super_class: #19                        // org/jpmml/python/CastFunction
@@ -122,15 +122,15 @@
         11: aload         4
         13: putfield      #3                  // Field val$name:Ljava/lang/String;
         16: aload_0
         17: aload_2
         18: invokespecial #4                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         21: return
       LineNumberTable:
-        line 151: 0
+        line 153: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lsklearn/Transformer$1;
             0      22     1 this$0   Lsklearn/Transformer;
             0      22     2    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -158,19 +158,19 @@
         28: areturn
         29: aload_0
         30: aload_1
         31: invokespecial #8                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
         34: checkcast     #9                  // class org/jpmml/python/TypeInfo
         37: areturn
       LineNumberTable:
-        line 156: 0
-        line 157: 7
-        line 159: 12
-        line 160: 19
-        line 170: 29
+        line 158: 0
+        line 159: 7
+        line 161: 12
+        line 162: 19
+        line 172: 29
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            12      17     2 string   Ljava/lang/String;
             0      38     0  this   Lsklearn/Transformer$1;
             0      38     1 object   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 29 /* same */
@@ -192,15 +192,15 @@
         20: invokestatic  #14                 // Method org/jpmml/python/ClassDictUtil.formatMember:(Lnet/razorvine/pickle/objects/ClassDict;Ljava/lang/String;)Ljava/lang/String;
         23: invokevirtual #13                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         26: ldc           #15                 // String ) is not a supported type info
         28: invokevirtual #13                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         31: invokevirtual #16                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         34: areturn
       LineNumberTable:
-        line 175: 0
+        line 177: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      35     0  this   Lsklearn/Transformer$1;
             0      35     1 object   Ljava/lang/Object;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
@@ -208,15 +208,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #17                 // Method apply:(Ljava/lang/Object;)Lorg/jpmml/python/TypeInfo;
          5: areturn
       LineNumberTable:
-        line 151: 0
+        line 153: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/Transformer$1;
 }
 Signature: #48                          // Lorg/jpmml/python/CastFunction<Lorg/jpmml/python/TypeInfo;>;
 SourceFile: "Transformer.java"
 EnclosingMethod: #52.#53                // sklearn.Transformer.getDType
```

#### sklearn/ensemble/stacking/StackingUtil.class

##### procyon -ec {}

```diff
@@ -27,22 +27,15 @@
         final Label label = schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
         final List<Feature> stackFeatures = new ArrayList<Feature>();
         final List<Model> models = new ArrayList<Model>();
         for (int i = 0; i < estimators.size(); ++i) {
             final E estimator = (E)estimators.get(i);
             final String stackMethod = (String)stackMethods.get(i);
-            estimator.setPMMLSegmentId((Object)Integer.valueOf(i + 1));
-            Model model;
-            try {
-                model = estimator.encode(schema);
-            }
-            finally {
-                estimator.setPMMLSegmentId((Object)null);
-            }
+            final Model model = estimator.encode((Object)Integer.valueOf(i + 1), schema);
             final List<Feature> predictFeatures = predictFunction.apply(i, model, stackMethod, encoder);
             if (predictFeatures != null && !predictFeatures.isEmpty()) {
                 stackFeatures.addAll(predictFeatures);
             }
             models.add(model);
         }
         if (passthrough) {
```

#### sklearn/Transformer.class

##### procyon -ec {}

```diff
@@ -1,10 +1,12 @@
 
 package sklearn;
 
+import org.jpmml.converter.FieldNameUtil;
+import java.util.Arrays;
 import org.jpmml.python.CastFunction;
 import org.jpmml.python.TypeInfo;
 import org.dmg.pmml.DataField;
 import java.util.Iterator;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.WildcardFeature;
 import java.util.ArrayList;
@@ -103,8 +105,20 @@
     }
     
     public TypeInfo getDType(final String name, final boolean extended) {
         final Object dtype = this.getObject(name);
         final CastFunction<TypeInfo> castFunction = (CastFunction<TypeInfo>)new Transformer.Transformer$1(this, (Class)TypeInfo.class, extended, name);
         return (TypeInfo)castFunction.apply(dtype);
     }
+    
+    public String createFieldName(final String function, final Object... args) {
+        return this.createFieldName(function, Arrays.asList(args));
+    }
+    
+    public String createFieldName(final String function, final List<?> args) {
+        final String pmmlName = this.getPMMLName();
+        if (pmmlName != null) {
+            return pmmlName;
+        }
+        return FieldNameUtil.create(function, (List)args);
+    }
 }
```

#### sklearn/Transformer$1$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 8e2823663e550891ddbae90f3cb8eac99948d6b1218607716c61add7143a8895
+  SHA-256 checksum 43c590ebf98737e2a9481b5c11b95d0ed6e2056a7301fae75c46894f0c8274cf
   Compiled from "Transformer.java"
 class sklearn.Transformer$1$1 implements org.jpmml.python.TypeInfo
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #5                          // sklearn/Transformer$1$1
   super_class: #6                         // java/lang/Object
@@ -69,15 +69,15 @@
          5: aload_0
          6: aload_2
          7: putfield      #2                  // Field val$string:Ljava/lang/String;
         10: aload_0
         11: invokespecial #3                  // Method java/lang/Object."<init>":()V
         14: return
       LineNumberTable:
-        line 160: 0
+        line 162: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lsklearn/Transformer$1$1;
             0      15     1 this$1   Lsklearn/Transformer$1;
 
   public org.dmg.pmml.DataType getDataType();
     descriptor: ()Lorg/dmg/pmml/DataType;
@@ -85,15 +85,15 @@
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #2                  // Field val$string:Ljava/lang/String;
          4: invokestatic  #4                  // Method org/jpmml/python/PythonTypeUtil.parseDataType:(Ljava/lang/String;)Lorg/dmg/pmml/DataType;
          7: areturn
       LineNumberTable:
-        line 164: 0
+        line 166: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lsklearn/Transformer$1$1;
 }
 SourceFile: "Transformer.java"
 EnclosingMethod: #11.#26                // sklearn.Transformer$1.apply
 InnerClasses:
```

#### sklearn/Transformer$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 32160f35bb9638ad4bedeab92a6ce26f2a3e29727fe1627c960a8809d4dd459d
+  SHA-256 checksum 1307c230b0c2bb35b42ec18088bb505f073e08cc990d450a488b1d971d035cf7
   Compiled from "Transformer.java"
 class sklearn.Transformer$2
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #6                          // sklearn/Transformer$2
   super_class: #7                         // java/lang/Object
@@ -67,15 +67,15 @@
         20: goto          24
         23: astore_0
         24: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 122: 0
+        line 124: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 2
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
 }
```

#### sklearn/ScalarLabelUtil.class

##### procyon -ec {}

```diff
@@ -1,18 +1,24 @@
 
 package sklearn;
 
 import java.util.Iterator;
 import java.util.Objects;
-import java.util.List;
 import org.jpmml.converter.CategoricalFeature;
 import org.jpmml.converter.ContinuousFeature;
 import org.dmg.pmml.Field;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.PMMLEncoder;
+import java.util.stream.Collector;
+import java.util.stream.Collectors;
+import java.util.function.Function;
+import org.jpmml.converter.MultiLabel;
+import java.util.Collections;
+import java.util.List;
+import org.jpmml.converter.Label;
 import org.jpmml.converter.ContinuousLabel;
 import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.OpType;
 import org.jpmml.converter.ScalarLabel;
 
 public class ScalarLabelUtil
 {
@@ -27,14 +33,31 @@
         if (scalarLabel instanceof ContinuousLabel) {
             final ContinuousLabel continuousLabel = (ContinuousLabel)scalarLabel;
             return OpType.CONTINUOUS;
         }
         throw new IllegalArgumentException();
     }
     
+    public static List<ScalarLabel> toScalarLabels(final Label label) {
+        return toScalarLabels((Class<? extends ScalarLabel>)ScalarLabel.class, label);
+    }
+    
+    public static <E extends ScalarLabel> List<E> toScalarLabels(final Class<? extends E> clazz, final Label label) {
+        if (label instanceof ScalarLabel) {
+            final ScalarLabel scalarLabel = (ScalarLabel)label;
+            return Collections.singletonList((E)clazz.cast(scalarLabel));
+        }
+        if (label instanceof MultiLabel) {
+            final MultiLabel multiLabel = (MultiLabel)label;
+            final List<? extends Label> labels = multiLabel.getLabels();
+            return labels.stream().map((Function<? super Object, ?>)clazz::cast).collect((Collector<? super Object, ?, List<E>>)Collectors.toList());
+        }
+        throw new IllegalArgumentException();
+    }
+    
     public static Feature toFeature(final ScalarLabel scalarLabel, final PMMLEncoder encoder) {
         final Field<?> field = (Field<?>)encoder.getField(scalarLabel.getName());
         return toFeature(scalarLabel, field, encoder);
     }
     
     public static Feature toFeature(final ScalarLabel scalarLabel, final Field<?> field, final PMMLEncoder encoder) {
         if (scalarLabel instanceof ContinuousLabel) {
```

#### sklearn/OutlierDetectorUtil$1.class

##### procyon -ec {}

```diff
@@ -4,15 +4,15 @@
 import org.jpmml.converter.PMMLUtil;
 import org.dmg.pmml.Expression;
 import org.dmg.pmml.FieldRef;
 import org.jpmml.converter.transformations.OutlierTransformation;
 
 static final class OutlierDetectorUtil$1 extends OutlierTransformation {
     public String getName(final String name) {
-        return this.val$estimator.createFieldName("outlier", new Object[0]);
+        return ((HasOutlierField)this.val$estimator).getOutlierField();
     }
     
     public Expression createExpression(final FieldRef fieldRef) {
         final Number threshold = ((OutlierDetector)this.val$estimator).getDecisionFunctionThreshold();
         return (Expression)PMMLUtil.createApply("lessOrEqual", new Expression[] { (Expression)fieldRef, (Expression)PMMLUtil.createConstant(threshold) });
     }
 }
```

#### sklearn/OutlierDetector.class

##### procyon -ec {}

```diff
@@ -1,9 +1,11 @@
 
 package sklearn;
 
-public interface OutlierDetector
+public interface OutlierDetector extends HasOutlierField
 {
+    public static final String FIELD_OUTLIER = "outlier";
+    
     default Number getDecisionFunctionThreshold() {
         return Double.valueOf(0.0);
     }
 }
```

#### sklearn/Calibrator.class

##### procyon -ec {}

```diff
@@ -1,11 +1,12 @@
 
 package sklearn;
 
 import org.dmg.pmml.Model;
+import org.jpmml.converter.FieldNameUtil;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.regression.RegressionModelUtil;
 import java.util.Collections;
 import com.google.common.collect.Iterables;
 import org.dmg.pmml.regression.RegressionModel;
 import org.jpmml.converter.Schema;
@@ -25,8 +26,16 @@
         final PMMLEncoder encoder = schema.getEncoder();
         final Label label = schema.getLabel();
         List<? extends Feature> features = schema.getFeatures();
         features = this.encodeFeatures((List<Feature>)features, (SkLearnEncoder)encoder);
         final Feature feature = (Feature)Iterables.getOnlyElement((Iterable)features);
         return RegressionModelUtil.createRegression((List)Collections.singletonList(feature), (List)Collections.singletonList(Double.valueOf(1.0)), (Number)Double.valueOf(0.0), RegressionModel.NormalizationMethod.NONE, schema);
     }
+    
+    public String createFieldName(final String function, final Feature feature) {
+        final String pmmlName = this.getPMMLName();
+        if (pmmlName != null) {
+            return pmmlName;
+        }
+        return FieldNameUtil.create(function, (List)Collections.singletonList(feature));
+    }
 }
```

#### sklearn/Estimator.class

##### procyon -ec {}

```diff
@@ -105,14 +105,25 @@
             final String pyClassName = this.getAlgorithmName();
             model.setAlgorithmName(pyClassName);
         }
         this.addFeatureImportances(model, schema);
         return model;
     }
     
+    public Model encode(final Object segmentId, final Schema schema) {
+        final Object prevSegmentId = this.getPMMLSegmentId();
+        try {
+            this.setPMMLSegmentId(segmentId);
+            return this.encode(schema);
+        }
+        finally {
+            this.setPMMLSegmentId(prevSegmentId);
+        }
+    }
+    
     public void checkLabel(final Label label) {
         final boolean supervised = this.isSupervised();
         if (supervised) {
             if (label == null) {
                 throw new IllegalArgumentException("Expected a label, got no label");
             }
         }
@@ -259,11 +270,18 @@
             PMMLUtil.addValues((Field)applyField, (List)values);
         }
         final Output output = ModelUtil.ensureOutput(model);
         output.getOutputFields().add(applyField);
         return applyField;
     }
     
+    protected static String extractArguments(final String function, final String name) {
+        if (name.startsWith(function + "(") && name.endsWith(")")) {
+            return name.substring((function + "(").length(), name.length() - ")".length());
+        }
+        return name;
+    }
+    
     static {
         logger = LoggerFactory.getLogger((Class)Estimator.class);
     }
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 100b5ac36b3092569b931572e64726fb0c168a5769e85768c0c3dc4ce642a52c
+  SHA-256 checksum 5b9057918c1e7db113aea39cf551eca337248ce780e430ec338cafe52ee0582f
   Compiled from "PMMLPipeline.java"
 class sklearn2pmml.pipeline.PMMLPipeline$3
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #13                         // sklearn2pmml/pipeline/PMMLPipeline$3
   super_class: #14                        // java/lang/Object
@@ -129,16 +129,16 @@
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             63    74    77   Class java/lang/NoSuchFieldError
             78    89    92   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 566: 0
-        line 332: 54
+        line 565: 0
+        line 331: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 10
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### sklearn2pmml/pipeline/PMMLPipeline.class

##### procyon -ec {}

```diff
@@ -1,13 +1,11 @@
 
 package sklearn2pmml.pipeline;
 
 import org.slf4j.LoggerFactory;
-import java.util.stream.Collector;
-import java.util.stream.Collectors;
 import com.google.common.base.Function;
 import com.google.common.collect.Lists;
 import org.jpmml.converter.ContinuousLabel;
 import org.dmg.pmml.Field;
 import org.dmg.pmml.Visitable;
 import org.dmg.pmml.Visitor;
 import org.dmg.pmml.OpType;
@@ -39,18 +37,18 @@
 import org.jpmml.converter.CMatrixUtil;
 import org.dmg.pmml.VerificationField;
 import java.util.LinkedHashMap;
 import net.razorvine.pickle.objects.ClassDict;
 import java.util.Collections;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.CategoricalLabel;
-import sklearn.ScalarLabelUtil;
 import org.jpmml.converter.FieldNameUtil;
 import org.jpmml.converter.ScalarLabel;
 import org.dmg.pmml.OutputField;
+import sklearn.ScalarLabelUtil;
 import org.jpmml.converter.ModelUtil;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.WildcardFeature;
 import java.util.Collection;
 import org.dmg.pmml.Model;
 import sklearn.Step;
@@ -153,15 +151,15 @@
         }
         if (predictTransformer != null || predictProbaTransformer != null || applyTransformer != null) {
             final Model finalModel = MiningModelUtil.getFinalModel(model);
             encoder.setModel(finalModel);
             final Label label2 = schema.getLabel();
             final Output output = ModelUtil.ensureOutput(finalModel);
             if (predictTransformer != null) {
-                final List<ScalarLabel> scalarLabels = toScalarLabels(label2);
+                final List<ScalarLabel> scalarLabels = ScalarLabelUtil.toScalarLabels(label2);
                 final List<OutputField> predictFields = new ArrayList<OutputField>();
                 for (final ScalarLabel scalarLabel : scalarLabels) {
                     final OutputField predictField = ModelUtil.createPredictedField(FieldNameUtil.create("predict", new Object[] { scalarLabel.getName() }), ScalarLabelUtil.getOpType(scalarLabel), scalarLabel.getDataType()).setFinalResult(Boolean.valueOf(false));
                     output.addOutputFields(new OutputField[] { predictField });
                     predictFields.add(predictField);
                 }
                 this.encodeOutput(output, predictFields, predictTransformer, encoder);
@@ -193,15 +191,15 @@
                         final VerificationField verificationField = ModelUtil.createVerificationField((String)activeFields.get(j));
                         final Domain domain = encoder.getDomain(verificationField.requireField());
                         data.put(verificationField, CMatrixUtil.getColumn((List)cleanValues(domain, activeValues), rows, activeFields.size(), j));
                     }
                 }
                 final Number precision = verification.getPrecision();
                 final Number zeroThreshold = verification.getZeroThreshold();
-                final List<ScalarLabel> scalarLabels2 = toScalarLabels(label3);
+                final List<ScalarLabel> scalarLabels2 = ScalarLabelUtil.toScalarLabels(label3);
                 boolean hasProbabilityValues = verification.hasProbabilityValues();
                 if (estimator instanceof Classifier) {
                     final Classifier classifier = (Classifier)estimator;
                     hasProbabilityValues &= classifier.hasProbabilityDistribution();
                 }
                 else {
                     hasProbabilityValues = false;
@@ -497,24 +495,11 @@
         final List<String> result = new ArrayList<String>(count);
         for (int i = 0; i < count; ++i) {
             result.add(name + String.valueOf(i + 1));
         }
         return result;
     }
     
-    private static List<ScalarLabel> toScalarLabels(final Label label) {
-        if (label instanceof ScalarLabel) {
-            final ScalarLabel scalarLabel = (ScalarLabel)label;
-            return Collections.singletonList(scalarLabel);
-        }
-        if (label instanceof MultiLabel) {
-            final MultiLabel multiLabel = (MultiLabel)label;
-            final List<? extends Label> labels = multiLabel.getLabels();
-            return labels.stream().map((java.util.function.Function<? super Object, ?>)ScalarLabel.class::cast).collect((Collector<? super Object, ?, List<ScalarLabel>>)Collectors.toList());
-        }
-        throw new IllegalArgumentException();
-    }
-    
     static {
         logger = LoggerFactory.getLogger((Class)PMMLPipeline.class);
     }
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 634ddfc2308d0370a574151a5617f14f9fd690611e67c2b146f4d32410146cb5
+  SHA-256 checksum b4ef8b2cb77193dfd58f7245f067ca0ddc46d32ada391595d3339de07dee10de
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$2 extends java.lang.Object implements com.google.common.base.Function<java.lang.Object, java.lang.Object>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #4                          // sklearn2pmml/pipeline/PMMLPipeline$2
   super_class: #5                         // java/lang/Object
@@ -56,15 +56,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 690: 0
+        line 689: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$2;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
     flags: (0x0001) ACC_PUBLIC
@@ -77,18 +77,18 @@
          6: invokestatic  #3                  // Method org/jpmml/converter/ValueUtil.isNaN:(Ljava/lang/Object;)Z
          9: ifeq          14
         12: aconst_null
         13: areturn
         14: aload_1
         15: areturn
       LineNumberTable:
-        line 694: 0
-        line 696: 5
-        line 697: 12
-        line 700: 14
+        line 693: 0
+        line 695: 5
+        line 696: 12
+        line 699: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$2;
             0      16     1 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 14 /* same */
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 016ba14712410a3c7ed2cba46061783aaa01b81684490ee61d584ae12fce46ee
+  SHA-256 checksum 638375fc3c828ae08ce77d45716ad720e48f816f9372542124f64ddcba4b24b4
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$1 extends org.jpmml.converter.visitors.AbstractExtender
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #9                          // sklearn2pmml/pipeline/PMMLPipeline$1
   super_class: #10                        // org/jpmml/converter/visitors/AbstractExtender
@@ -89,15 +89,15 @@
          1: aload_2
          2: putfield      #1                  // Field val$values:Ljava/util/Map;
          5: aload_0
          6: aload_1
          7: invokespecial #2                  // Method org/jpmml/converter/visitors/AbstractExtender."<init>":(Ljava/lang/String;)V
         10: return
       LineNumberTable:
-        line 641: 0
+        line 640: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$1;
             0      11     1    x0   Ljava/lang/String;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.Value);
     descriptor: (Lorg/dmg/pmml/Value;)Lorg/dmg/pmml/VisitorAction;
@@ -121,19 +121,19 @@
         26: invokestatic  #6                  // Method org/jpmml/converter/ValueUtil.asString:(Ljava/lang/Object;)Ljava/lang/String;
         29: invokevirtual #7                  // Method addExtension:(Lorg/dmg/pmml/PMMLObject;Ljava/lang/String;)V
         32: aload_0
         33: aload_1
         34: invokespecial #8                  // Method org/jpmml/converter/visitors/AbstractExtender.visit:(Lorg/dmg/pmml/Value;)Lorg/dmg/pmml/VisitorAction;
         37: areturn
       LineNumberTable:
-        line 645: 0
-        line 647: 14
-        line 648: 18
-        line 650: 23
-        line 653: 32
+        line 644: 0
+        line 646: 14
+        line 647: 18
+        line 649: 23
+        line 652: 32
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      38     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$1;
             0      38     1 pmmlValue   Lorg/dmg/pmml/Value;
            14      24     2 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
```

#### sklearn2pmml/ensemble/EstimatorChain.class

##### procyon -ec {}

```diff
@@ -1,23 +1,25 @@
 
 package sklearn2pmml.ensemble;
 
 import org.dmg.pmml.Predicate;
 import org.jpmml.python.Scope;
 import org.jpmml.converter.Feature;
-import org.jpmml.converter.Label;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.dmg.pmml.mining.Segment;
 import sklearn2pmml.util.EvaluatableUtil;
+import org.jpmml.converter.Label;
 import org.jpmml.python.TupleUtil;
+import org.jpmml.converter.ScalarLabel;
 import org.jpmml.python.DataFrameScope;
 import org.dmg.pmml.mining.Segmentation;
-import org.jpmml.converter.MultiLabel;
-import org.jpmml.converter.ScalarLabel;
+import org.jpmml.python.ClassDictUtil;
+import java.util.Collection;
+import sklearn.ScalarLabelUtil;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import java.util.Iterator;
 import java.util.stream.Collector;
 import java.util.stream.Collectors;
 import java.util.ArrayList;
 import java.util.List;
@@ -75,39 +77,38 @@
         final Boolean multioutput = this.getMultioutput();
         final List<Object[]> steps = this.getSteps();
         if (steps.isEmpty()) {
             throw new IllegalArgumentException();
         }
         final Label label = schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
-        MultiLabel multiLabel;
-        if (label instanceof ScalarLabel) {
-            final ScalarLabel scalarLabel = (ScalarLabel)label;
-            final List<Label> labels = (List<Label>)new EstimatorChain.EstimatorChain$1(this, (List)steps, scalarLabel);
-            multiLabel = new MultiLabel((List)labels);
-        }
-        else {
-            if (!(label instanceof MultiLabel)) {
-                throw new IllegalArgumentException();
-            }
-            multiLabel = (MultiLabel)label;
+        final List<ScalarLabel> scalarLabels = ScalarLabelUtil.toScalarLabels(label);
+        if ((boolean)multioutput) {
+            ClassDictUtil.checkSize(new Collection[] { steps, scalarLabels });
         }
         final List<Estimator> estimators = new ArrayList<Estimator>();
         final List<Model> models = new ArrayList<Model>();
         final Segmentation segmentation = new Segmentation(((boolean)multioutput) ? Segmentation.MultipleModelMethod.MULTI_MODEL_CHAIN : Segmentation.MultipleModelMethod.MODEL_CHAIN, (List)null);
         final Scope scope = (Scope)new DataFrameScope("X", (List)features);
         for (int i = 0; i < steps.size(); ++i) {
             final Object[] step = (Object[])steps.get(i);
+            final ScalarLabel scalarLabel = ((boolean)multioutput) ? ((ScalarLabel)scalarLabels.get(i)) : ((ScalarLabel)scalarLabels.get(0));
             final String name = (String)TupleUtil.extractElement(step, 0, (Class)String.class);
             final Estimator estimator = (Estimator)TupleUtil.extractElement(step, 1, (Class)Estimator.class);
             final Object expr = TupleUtil.extractElement(step, 2, (Class)Object.class);
             estimators.add(estimator);
-            final Schema segmentSchema = schema.toRelabeledSchema(multiLabel.getLabel(i));
+            final Schema segmentSchema = schema.toRelabeledSchema((Label)scalarLabel);
             final Predicate predicate = EvaluatableUtil.translatePredicate(expr, scope);
-            final Model model = estimator.encode(segmentSchema);
+            Model model;
+            if ((boolean)multioutput) {
+                model = estimator.encode((Object)scalarLabel.getName(), segmentSchema);
+            }
+            else {
+                model = estimator.encode(segmentSchema);
+            }
             models.add(model);
             if (estimator instanceof Link) {
                 final Link link = (Link)estimator;
                 schema = link.augmentSchema(model, segmentSchema);
             }
             final Segment segment = new Segment(predicate, model).setId(name);
             segmentation.addSegments(new Segment[] { segment });
```

#### sklearn2pmml/ensemble/GBDTUtil.class

##### procyon -ec {}

```diff
@@ -32,22 +32,22 @@
 {
     private GBDTUtil() {
     }
     
     public static MiningModel encodeModel(final Estimator gbdt, final MultiOneHotEncoder ohe, final List<? extends Number> coef, final Number intercept, final Schema schema) {
         if (gbdt instanceof HasNativeConfiguration) {
             final HasNativeConfiguration hasNativeConfiguration = (HasNativeConfiguration)gbdt;
-            final Map<String, ?> pmmlOptions = gbdt.getPMMLOptions();
+            final Map<String, ?> prevPmmlOptions = gbdt.getPMMLOptions();
             Model model;
             try {
                 gbdt.setPMMLOptions(hasNativeConfiguration.getNativeConfiguration());
                 model = gbdt.encode(schema);
             }
             finally {
-                gbdt.setPMMLOptions((Map)pmmlOptions);
+                gbdt.setPMMLOptions((Map)prevPmmlOptions);
             }
             final List<TreeModel> treeModels = new ArrayList<TreeModel>();
             final Visitor modelVisitor = (Visitor)new GBDTUtil.GBDTUtil$1((List)treeModels);
             modelVisitor.applyTo((Visitable)model);
             final List<List<?>> treeCategories = ohe.getCategories();
             ClassDictUtil.checkSize(new Collection[] { treeModels, treeCategories });
             final List<Map<Integer, Number>> treeNodeScores = new ArrayList<Map<Integer, Number>>();
```

#### sklearn2pmml/preprocessing/CastTransformer.class

##### procyon -ec {}

```diff
@@ -28,15 +28,15 @@
         final DataType dataType = dtype.getDataType();
         final OpType opType = TypeUtil.getOpType(dataType);
         final List<Feature> result = new ArrayList<Feature>();
         for (int i = 0; i < features.size(); ++i) {
             Feature feature = (Feature)features.get(i);
             if (feature.getDataType() != dataType) {
                 final FieldRef fieldRef = feature.ref();
-                final DerivedField derivedField = encoder.ensureDerivedField(this.createFieldName(dataType, new Object[] { feature }), opType, dataType, () -> fieldRef);
+                final DerivedField derivedField = encoder.ensureDerivedField(this.createFieldName(dataType.name().toLowerCase(), new Object[] { feature }), opType, dataType, () -> fieldRef);
                 feature = FeatureUtil.createFeature((Field)derivedField, (PMMLEncoder)encoder);
             }
             result.add(feature);
         }
         return result;
     }
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.29</version>
+    <version>1.7.30</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn converter</name>
   <description>JPMML Scikit-Learn to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-sklearn
 groupId=org.jpmml
-version=1.7.29
+version=1.7.30
```

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/resources/gson-2.10.jar` & `sklearn2pmml-0.94.0/sklearn2pmml/resources/gson-2.10.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.94.0/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.93.0/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.94.0/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

