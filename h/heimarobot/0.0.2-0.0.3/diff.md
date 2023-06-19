# Comparing `tmp/heimarobot-0.0.2.tar.gz` & `tmp/heimarobot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimarobot-0.0.2.tar", last modified: Mon Jun 19 10:44:48 2023, max compression
+gzip compressed data, was "heimarobot-0.0.3.tar", last modified: Mon Jun 19 11:58:23 2023, max compression
```

## Comparing `heimarobot-0.0.2.tar` & `heimarobot-0.0.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.379464 heimarobot-0.0.2/
--rw-rw-rw-   0        0        0      962 2023-06-19 10:44:48.378466 heimarobot-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      688 2023-06-19 10:31:29.000000 heimarobot-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.243466 heimarobot-0.0.2/heimarobot/
--rw-rw-rw-   0        0        0      512 2023-06-19 10:44:37.000000 heimarobot-0.0.2/heimarobot/__init__.py
--rw-rw-rw-   0        0        0      510 2023-06-19 08:11:56.000000 heimarobot-0.0.2/heimarobot/face_attribute.py
--rw-rw-rw-   0        0        0      839 2023-06-19 08:01:57.000000 heimarobot-0.0.2/heimarobot/face_detection.py
--rw-rw-rw-   0        0        0      508 2023-06-19 08:02:26.000000 heimarobot-0.0.2/heimarobot/face_landmark.py
--rw-rw-rw-   0        0        0     1088 2023-06-19 08:03:44.000000 heimarobot-0.0.2/heimarobot/face_recognition.py
--rw-rw-rw-   0        0        0     1010 2023-06-19 08:03:02.000000 heimarobot-0.0.2/heimarobot/face_swapper.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.262465 heimarobot-0.0.2/heimarobot/insightface/
--rw-rw-rw-   0        0        0      445 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.270466 heimarobot-0.0.2/heimarobot/insightface/app/
--rw-rw-rw-   0        0        0       60 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/app/__init__.py
--rw-rw-rw-   0        0        0     1516 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/app/common.py
--rw-rw-rw-   0        0        0     4331 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/app/face_analysis.py
--rw-rw-rw-   0        0        0    10078 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/app/mask_renderer.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.277467 heimarobot-0.0.2/heimarobot/insightface/commands/
--rw-rw-rw-   0        0        0      328 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/commands/__init__.py
--rw-rw-rw-   0        0        0      753 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/commands/insightface_cli.py
--rw-rw-rw-   0        0        0     1272 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/commands/model_download.py
--rw-rw-rw-   0        0        0     3358 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/commands/rec_add_mask_param.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.284465 heimarobot-0.0.2/heimarobot/insightface/data/
--rw-rw-rw-   0        0        0       69 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/__init__.py
--rw-rw-rw-   0        0        0      797 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/image.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.295464 heimarobot-0.0.2/heimarobot/insightface/data/images/
--rw-rw-rw-   0        0        0    12123 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/images/Tom_Hanks_54745.png
--rw-rw-rw-   0        0        0    21308 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/images/mask_black.jpg
--rw-rw-rw-   0        0        0    44728 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/images/mask_blue.jpg
--rw-rw-rw-   0        0        0     6116 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/images/mask_green.jpg
--rw-rw-rw-   0        0        0    78905 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/images/mask_white.jpg
--rw-rw-rw-   0        0        0   128824 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/images/t1.jpg
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.298466 heimarobot-0.0.2/heimarobot/insightface/data/objects/
--rw-rw-rw-   0        0        0      974 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/objects/meanshape_68.pkl
--rw-rw-rw-   0        0        0      432 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/pickle_object.py
--rw-rw-rw-   0        0        0     2582 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/data/rec_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.317468 heimarobot-0.0.2/heimarobot/insightface/model_zoo/
--rw-rw-rw-   0        0        0      201 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/__init__.py
--rw-rw-rw-   0        0        0     3203 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/arcface_onnx.py
--rw-rw-rw-   0        0        0     3445 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/attribute.py
--rw-rw-rw-   0        0        0     4754 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/inswapper.py
--rw-rw-rw-   0        0        0     4312 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/landmark.py
--rw-rw-rw-   0        0        0     3211 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/model_store.py
--rw-rw-rw-   0        0        0     3709 2023-06-19 10:07:39.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/model_zoo.py
--rw-rw-rw-   0        0        0    11428 2023-06-19 05:10:09.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/retinaface.py
--rw-rw-rw-   0        0        0    13200 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/model_zoo/scrfd.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.319465 heimarobot-0.0.2/heimarobot/insightface/thirdparty/
--rw-rw-rw-   0        0        0        0 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.321464 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/
--rw-rw-rw-   0        0        0       90 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.332468 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/
--rw-rw-rw-   0        0        0      301 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.343466 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/
--rw-rw-rw-   0        0        0    13718 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core.cpp
--rw-rw-rw-   0        0        0     1914 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core.h
--rw-rw-rw-   0        0        0   408856 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.c
--rw-rw-rw-   0        0        0    83456 2023-06-19 03:30:45.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0   334030 2023-06-19 07:26:28.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.cpp
--rw-rw-rw-   0        0        0     5063 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.pyx
--rw-rw-rw-   0        0        0      492 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/setup.py
--rw-rw-rw-   0        0        0     5079 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/io.py
--rw-rw-rw-   0        0        0     7705 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/light.py
--rw-rw-rw-   0        0        0     4732 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/render.py
--rw-rw-rw-   0        0        0    12589 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/transform.py
--rw-rw-rw-   0        0        0      815 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/vis.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.355467 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/
--rw-rw-rw-   0        0        0      221 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/__init__.py
--rw-rw-rw-   0        0        0     6011 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/io.py
--rw-rw-rw-   0        0        0     7717 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/light.py
--rw-rw-rw-   0        0        0    10712 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/render.py
--rw-rw-rw-   0        0        0    12703 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/transform.py
--rw-rw-rw-   0        0        0      815 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/vis.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.362465 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/morphable_model/
--rw-rw-rw-   0        0        0      198 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/morphable_model/__init__.py
--rw-rw-rw-   0        0        0     8373 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/morphable_model/fit.py
--rw-rw-rw-   0        0        0     3875 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/morphable_model/load.py
--rw-rw-rw-   0        0        0     5710 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/morphable_model/morphabel_model.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.376467 heimarobot-0.0.2/heimarobot/insightface/utils/
--rw-rw-rw-   0        0        0      627 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/utils/__init__.py
--rw-rw-rw-   0        0        0       35 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/utils/constant.py
--rw-rw-rw-   0        0        0     3455 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/utils/download.py
--rw-rw-rw-   0        0        0     3459 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/utils/face_align.py
--rw-rw-rw-   0        0        0     4407 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/utils/filesystem.py
--rw-rw-rw-   0        0        0     1943 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/utils/storage.py
--rw-rw-rw-   0        0        0     3495 2023-06-05 04:11:00.000000 heimarobot-0.0.2/heimarobot/insightface/utils/transform.py
--rw-rw-rw-   0        0        0     1302 2023-06-19 06:32:52.000000 heimarobot-0.0.2/heimarobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:44:48.256466 heimarobot-0.0.2/heimarobot.egg-info/
--rw-rw-rw-   0        0        0      962 2023-06-19 10:44:47.000000 heimarobot-0.0.2/heimarobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3791 2023-06-19 10:44:48.000000 heimarobot-0.0.2/heimarobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 10:44:47.000000 heimarobot-0.0.2/heimarobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-06-19 10:44:47.000000 heimarobot-0.0.2/heimarobot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2023-06-19 10:44:47.000000 heimarobot-0.0.2/heimarobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 10:44:47.000000 heimarobot-0.0.2/heimarobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 07:26:28.000000 heimarobot-0.0.2/heimarobot.egg-info/zip-safe
--rw-rw-rw-   0        0        0      103 2023-06-05 04:11:00.000000 heimarobot-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 10:44:48.379464 heimarobot-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3457 2023-06-19 10:34:01.000000 heimarobot-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.738239 heimarobot-0.0.3/
+-rw-rw-rw-   0        0        0     4585 2023-06-19 11:58:23.737241 heimarobot-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4311 2023-06-19 11:57:53.000000 heimarobot-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.615245 heimarobot-0.0.3/heimarobot/
+-rw-rw-rw-   0        0        0      516 2023-06-19 11:55:28.000000 heimarobot-0.0.3/heimarobot/__init__.py
+-rw-rw-rw-   0        0        0      548 2023-06-19 11:23:06.000000 heimarobot-0.0.3/heimarobot/face_attribute.py
+-rw-rw-rw-   0        0        0      876 2023-06-19 11:23:20.000000 heimarobot-0.0.3/heimarobot/face_detection.py
+-rw-rw-rw-   0        0        0      546 2023-06-19 11:23:12.000000 heimarobot-0.0.3/heimarobot/face_landmark.py
+-rw-rw-rw-   0        0        0     1126 2023-06-19 11:23:10.000000 heimarobot-0.0.3/heimarobot/face_recognition.py
+-rw-rw-rw-   0        0        0     1006 2023-06-19 11:23:09.000000 heimarobot-0.0.3/heimarobot/face_swapper.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.632238 heimarobot-0.0.3/heimarobot/insightface/
+-rw-rw-rw-   0        0        0      445 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.639240 heimarobot-0.0.3/heimarobot/insightface/app/
+-rw-rw-rw-   0        0        0       60 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/app/__init__.py
+-rw-rw-rw-   0        0        0     1516 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/app/common.py
+-rw-rw-rw-   0        0        0     4331 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/app/face_analysis.py
+-rw-rw-rw-   0        0        0    10078 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/app/mask_renderer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.646240 heimarobot-0.0.3/heimarobot/insightface/commands/
+-rw-rw-rw-   0        0        0      328 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/commands/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/commands/insightface_cli.py
+-rw-rw-rw-   0        0        0     1272 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/commands/model_download.py
+-rw-rw-rw-   0        0        0     3358 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/commands/rec_add_mask_param.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.652245 heimarobot-0.0.3/heimarobot/insightface/data/
+-rw-rw-rw-   0        0        0       69 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/__init__.py
+-rw-rw-rw-   0        0        0      797 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/image.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.662240 heimarobot-0.0.3/heimarobot/insightface/data/images/
+-rw-rw-rw-   0        0        0    12123 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/images/Tom_Hanks_54745.png
+-rw-rw-rw-   0        0        0    21308 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/images/mask_black.jpg
+-rw-rw-rw-   0        0        0    44728 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/images/mask_blue.jpg
+-rw-rw-rw-   0        0        0     6116 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/images/mask_green.jpg
+-rw-rw-rw-   0        0        0    78905 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/images/mask_white.jpg
+-rw-rw-rw-   0        0        0   128824 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/images/t1.jpg
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.664240 heimarobot-0.0.3/heimarobot/insightface/data/objects/
+-rw-rw-rw-   0        0        0      974 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/objects/meanshape_68.pkl
+-rw-rw-rw-   0        0        0      432 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/pickle_object.py
+-rw-rw-rw-   0        0        0     2582 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/data/rec_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.679240 heimarobot-0.0.3/heimarobot/insightface/model_zoo/
+-rw-rw-rw-   0        0        0      201 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/__init__.py
+-rw-rw-rw-   0        0        0     3203 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/arcface_onnx.py
+-rw-rw-rw-   0        0        0     3445 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/attribute.py
+-rw-rw-rw-   0        0        0     4754 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/inswapper.py
+-rw-rw-rw-   0        0        0     4312 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/landmark.py
+-rw-rw-rw-   0        0        0     3211 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/model_store.py
+-rw-rw-rw-   0        0        0     3709 2023-06-19 10:07:39.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/model_zoo.py
+-rw-rw-rw-   0        0        0    11428 2023-06-19 05:10:09.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/retinaface.py
+-rw-rw-rw-   0        0        0    13200 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/model_zoo/scrfd.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.681245 heimarobot-0.0.3/heimarobot/insightface/thirdparty/
+-rw-rw-rw-   0        0        0        0 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.682245 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/
+-rw-rw-rw-   0        0        0       90 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.693240 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/
+-rw-rw-rw-   0        0        0      301 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.704241 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/
+-rw-rw-rw-   0        0        0    13718 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core.cpp
+-rw-rw-rw-   0        0        0     1914 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core.h
+-rw-rw-rw-   0        0        0   408856 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.c
+-rw-rw-rw-   0        0        0    83456 2023-06-19 03:30:45.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   334030 2023-06-19 07:26:28.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.cpp
+-rw-rw-rw-   0        0        0     5063 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.pyx
+-rw-rw-rw-   0        0        0      492 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/setup.py
+-rw-rw-rw-   0        0        0     5079 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/io.py
+-rw-rw-rw-   0        0        0     7705 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/light.py
+-rw-rw-rw-   0        0        0     4732 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/render.py
+-rw-rw-rw-   0        0        0    12589 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/transform.py
+-rw-rw-rw-   0        0        0      815 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/vis.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.714245 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/
+-rw-rw-rw-   0        0        0      221 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/__init__.py
+-rw-rw-rw-   0        0        0     6011 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/io.py
+-rw-rw-rw-   0        0        0     7717 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/light.py
+-rw-rw-rw-   0        0        0    10712 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/render.py
+-rw-rw-rw-   0        0        0    12703 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/transform.py
+-rw-rw-rw-   0        0        0      815 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/vis.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.721242 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/morphable_model/
+-rw-rw-rw-   0        0        0      198 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/morphable_model/__init__.py
+-rw-rw-rw-   0        0        0     8373 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/morphable_model/fit.py
+-rw-rw-rw-   0        0        0     3875 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/morphable_model/load.py
+-rw-rw-rw-   0        0        0     5710 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/morphable_model/morphabel_model.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.734240 heimarobot-0.0.3/heimarobot/insightface/utils/
+-rw-rw-rw-   0        0        0      627 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/utils/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/utils/constant.py
+-rw-rw-rw-   0        0        0     3455 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/utils/download.py
+-rw-rw-rw-   0        0        0     3459 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/utils/face_align.py
+-rw-rw-rw-   0        0        0     4407 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/utils/filesystem.py
+-rw-rw-rw-   0        0        0     1943 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/utils/storage.py
+-rw-rw-rw-   0        0        0     3495 2023-06-05 04:11:00.000000 heimarobot-0.0.3/heimarobot/insightface/utils/transform.py
+-rw-rw-rw-   0        0        0     1302 2023-06-19 06:32:52.000000 heimarobot-0.0.3/heimarobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:58:23.627241 heimarobot-0.0.3/heimarobot.egg-info/
+-rw-rw-rw-   0        0        0     4585 2023-06-19 11:58:23.000000 heimarobot-0.0.3/heimarobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3791 2023-06-19 11:58:23.000000 heimarobot-0.0.3/heimarobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:58:23.000000 heimarobot-0.0.3/heimarobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-06-19 11:58:23.000000 heimarobot-0.0.3/heimarobot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2023-06-19 11:58:23.000000 heimarobot-0.0.3/heimarobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 11:58:23.000000 heimarobot-0.0.3/heimarobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 07:26:28.000000 heimarobot-0.0.3/heimarobot.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      103 2023-06-05 04:11:00.000000 heimarobot-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 11:58:23.738239 heimarobot-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3457 2023-06-19 10:34:01.000000 heimarobot-0.0.3/setup.py
```

### Comparing `heimarobot-0.0.2/heimarobot/__init__.py` & `heimarobot-0.0.3/heimarobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,19 @@
     #import mxnet as mx
     import onnxruntime
 except ImportError:
     raise ImportError(
         "Unable to import dependency onnxruntime. "
     )
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
+
 
 from .face_attribute import *
 from .face_detection import *
 from .face_landmark import *
 from .face_recognition import *
 from .face_swapper import *
 from .utils import *
 
 
+
```

### Comparing `heimarobot-0.0.2/heimarobot/face_detection.py` & `heimarobot-0.0.3/heimarobot/face_detection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import insightface
-from insightface.app.common import Face
+import heimarobot.insightface as insightface
+from heimarobot.insightface.app.common import Face
 
 class FaceDetection:
     def __init__(self):
         self.model = insightface.model_zoo.get_model('best-detect.onnx', download=False, download_zip=False)
         self.model.prepare(0, input_size=(640, 640), det_thresh=0.5)
 
     def predict(self,src,max_num=0):
```

### Comparing `heimarobot-0.0.2/heimarobot/face_recognition.py` & `heimarobot-0.0.3/heimarobot/face_recognition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import insightface
-from face_detection import FaceDetection
-from insightface.app.common import Face
+import heimarobot.insightface as insightface
+from .face_detection import FaceDetection
+from heimarobot.insightface.app.common import Face
 
 class FaceRecognition:
 
     def __init__(self):
         self.detector = FaceDetection()
 
         self.model = insightface.model_zoo.get_model('best-recognition.onnx', download=False, download_zip=False)
```

### Comparing `heimarobot-0.0.2/heimarobot/face_swapper.py` & `heimarobot-0.0.3/heimarobot/face_swapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import insightface
-from face_detection import FaceDetection
-from insightface.app.common import Face
-from face_recognition import FaceRecognition
+import heimarobot.insightface as insightface
+from heimarobot.insightface.app.common import Face
+from .face_recognition import FaceRecognition
 
 class FaceSwapper:
 
     def __init__(self):
         self.recognition = FaceRecognition()
         self.model = insightface.model_zoo.get_model('best-swapper.onnx', download=False, download_zip=False)
```

### Comparing `heimarobot-0.0.2/heimarobot/insightface/app/common.py` & `heimarobot-0.0.3/heimarobot/insightface/app/common.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/app/face_analysis.py` & `heimarobot-0.0.3/heimarobot/insightface/app/face_analysis.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/app/mask_renderer.py` & `heimarobot-0.0.3/heimarobot/insightface/app/mask_renderer.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/commands/insightface_cli.py` & `heimarobot-0.0.3/heimarobot/insightface/commands/insightface_cli.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/commands/model_download.py` & `heimarobot-0.0.3/heimarobot/insightface/commands/model_download.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/commands/rec_add_mask_param.py` & `heimarobot-0.0.3/heimarobot/insightface/commands/rec_add_mask_param.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/image.py` & `heimarobot-0.0.3/heimarobot/insightface/data/image.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/images/Tom_Hanks_54745.png` & `heimarobot-0.0.3/heimarobot/insightface/data/images/Tom_Hanks_54745.png`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/images/mask_black.jpg` & `heimarobot-0.0.3/heimarobot/insightface/data/images/mask_black.jpg`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/images/mask_blue.jpg` & `heimarobot-0.0.3/heimarobot/insightface/data/images/mask_blue.jpg`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/images/mask_green.jpg` & `heimarobot-0.0.3/heimarobot/insightface/data/images/mask_green.jpg`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/images/mask_white.jpg` & `heimarobot-0.0.3/heimarobot/insightface/data/images/mask_white.jpg`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/images/t1.jpg` & `heimarobot-0.0.3/heimarobot/insightface/data/images/t1.jpg`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/objects/meanshape_68.pkl` & `heimarobot-0.0.3/heimarobot/insightface/data/objects/meanshape_68.pkl`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/data/rec_builder.py` & `heimarobot-0.0.3/heimarobot/insightface/data/rec_builder.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/model_zoo/arcface_onnx.py` & `heimarobot-0.0.3/heimarobot/insightface/model_zoo/arcface_onnx.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/model_zoo/attribute.py` & `heimarobot-0.0.3/heimarobot/insightface/model_zoo/attribute.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/model_zoo/inswapper.py` & `heimarobot-0.0.3/heimarobot/insightface/model_zoo/inswapper.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/model_zoo/landmark.py` & `heimarobot-0.0.3/heimarobot/insightface/model_zoo/landmark.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/model_zoo/model_store.py` & `heimarobot-0.0.3/heimarobot/insightface/model_zoo/model_store.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/model_zoo/model_zoo.py` & `heimarobot-0.0.3/heimarobot/insightface/model_zoo/model_zoo.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/model_zoo/retinaface.py` & `heimarobot-0.0.3/heimarobot/insightface/model_zoo/retinaface.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/model_zoo/scrfd.py` & `heimarobot-0.0.3/heimarobot/insightface/model_zoo/scrfd.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core.cpp` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core.cpp`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core.h` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core.h`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.c` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.c`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.cpp` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.cpp`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.pyx` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/cython/mesh_core_cython.pyx`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/io.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/io.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/light.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/light.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/render.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/render.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/transform.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/transform.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh/vis.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh/vis.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/io.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/io.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/light.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/light.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/render.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/render.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/transform.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/transform.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/mesh_numpy/vis.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/mesh_numpy/vis.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/morphable_model/fit.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/morphable_model/fit.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/morphable_model/load.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/morphable_model/load.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/thirdparty/face3d/morphable_model/morphabel_model.py` & `heimarobot-0.0.3/heimarobot/insightface/thirdparty/face3d/morphable_model/morphabel_model.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/utils/__init__.py` & `heimarobot-0.0.3/heimarobot/insightface/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/utils/download.py` & `heimarobot-0.0.3/heimarobot/insightface/utils/download.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/utils/face_align.py` & `heimarobot-0.0.3/heimarobot/insightface/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/utils/filesystem.py` & `heimarobot-0.0.3/heimarobot/insightface/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/utils/storage.py` & `heimarobot-0.0.3/heimarobot/insightface/utils/storage.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/insightface/utils/transform.py` & `heimarobot-0.0.3/heimarobot/insightface/utils/transform.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot/utils.py` & `heimarobot-0.0.3/heimarobot/utils.py`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/heimarobot.egg-info/SOURCES.txt` & `heimarobot-0.0.3/heimarobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heimarobot-0.0.2/setup.py` & `heimarobot-0.0.3/setup.py`

 * *Files identical despite different names*

