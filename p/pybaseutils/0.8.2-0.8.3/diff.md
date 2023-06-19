# Comparing `tmp/pybaseutils-0.8.2.tar.gz` & `tmp/pybaseutils-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybaseutils-0.8.2.tar", last modified: Fri Jun  2 01:38:34 2023, max compression
+gzip compressed data, was "dist/pybaseutils-0.8.3.tar", last modified: Mon Jun 19 03:45:15 2023, max compression
```

## Comparing `pybaseutils-0.8.2.tar` & `pybaseutils-0.8.3.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.2/LICENCE
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/PKG-INFO
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/base64_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/base_audio/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4792 2023-05-16 07:29:26.000000 pybaseutils-0.8.2/pybaseutils/base_audio/audio_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.2/pybaseutils/base_audio/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/batch_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/cluster/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.2/pybaseutils/color_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.2/pybaseutils/config_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/coords_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/cvutils/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.2/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6101 2023-06-01 06:52:32.000000 pybaseutils-0.8.2/pybaseutils/cvutils/monitor.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     9695 2023-06-01 07:00:45.000000 pybaseutils-0.8.2/pybaseutils/cvutils/video_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.2/pybaseutils/cvutils/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/dataloader/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/dataloader/dataset.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/dataloader/parser_textdata.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    32583 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/file_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/font_style/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/font_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    97190 2023-06-02 01:38:12.000000 pybaseutils-0.8.2/pybaseutils/image_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/json_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/log.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.2/pybaseutils/logger.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/maker/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/convert_labelme2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/convert_voc2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/convert_voc2yolo.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/convert_yolo2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/maker_labelme.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/maker/maker_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/maker/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/metrics/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.2/pybaseutils/plot_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/pycpp/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.2/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/pycpp/main.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.2/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.2/pybaseutils/setup_config.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/thread_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/time_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.2/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/transforms/
--rwxrwxrwx   0 dm        (1000) dm        (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.2/pybaseutils/word_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.2/pybaseutils/worker.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.2/pybaseutils/yaml_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      137 2023-06-02 01:38:30.000000 pybaseutils-0.8.2/pybaseutils/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/
--rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.2/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3491 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)       20 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.2/README.md
--rwxrwxrwx   0 dm        (1000) dm        (1000)       38 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/setup.cfg
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2213 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/setup.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.2/test_py/class_names.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/converter/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.2/test_py/converter/AffectNet.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.2/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.2/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.2/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.2/test_py/converter/CCPD.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.2/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.2/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.2/test_py/converter/TT100K.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.2/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/converter/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1733 2023-05-11 03:26:39.000000 pybaseutils-0.8.2/test_py/demo1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1189 2023-05-30 10:27:09.000000 pybaseutils-0.8.2/test_py/demo2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.2/test_py/demo_async_await1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1194 2023-05-25 05:49:48.000000 pybaseutils-0.8.2/test_py/demo_async_await2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4664 2023-06-01 07:22:44.000000 pybaseutils-0.8.2/test_py/demo_copy_files.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.2/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1342 2023-05-16 02:22:22.000000 pybaseutils-0.8.2/test_py/demo_ffmpy.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.2/test_py/demo_for_trt.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2877 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/demo_get_file_list.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/demo_gif.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1745 2023-05-24 03:16:30.000000 pybaseutils-0.8.2/test_py/demo_gif_video.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/demo_metrics.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/demo_mouse.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/demo_pandas.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.2/test_py/demo_plot.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.2/test_py/demo_standard_image .py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.2/test_py/demo_standard_video .py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/demo_taichi.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      778 2023-06-01 07:11:31.000000 pybaseutils-0.8.2/test_py/demo_video.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.2/test_py/demo_voc_crop.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2374 2023-04-18 03:49:38.000000 pybaseutils-0.8.2/test_py/demo_voc_vis.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.2/test_py/demo_word_similar.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/demo_worker1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/demo_worker2.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/detector/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6671 2023-05-04 08:11:18.000000 pybaseutils-0.8.2/test_py/detector/detect_face_person.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.2/test_py/detector/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/flask_demo/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.2/test_py/flask_demo/func.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.2/test_py/flask_demo/server.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.2/test_py/flask_demo/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/image_correction/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.2/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.2/test_py/image_correction/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.2/test_py/kafka_worker.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.2/test_py/men_tracemalloc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.2/test_py/performance.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.513464 pybaseutils-0.8.3/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.3/LICENCE
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-06-19 03:45:15.513141 pybaseutils-0.8.3/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.3/README.md
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.469735 pybaseutils-0.8.3/pybaseutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2023-06-19 03:45:11.000000 pybaseutils-0.8.3/pybaseutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/base64_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.472683 pybaseutils-0.8.3/pybaseutils/base_audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.3/pybaseutils/base_audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4792 2023-05-16 07:29:26.000000 pybaseutils-0.8.3/pybaseutils/base_audio/audio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/batch_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.474600 pybaseutils-0.8.3/pybaseutils/cluster/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.3/pybaseutils/color_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.3/pybaseutils/config_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/coords_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.476933 pybaseutils-0.8.3/pybaseutils/cvutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.3/pybaseutils/cvutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.3/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6101 2023-06-01 06:52:32.000000 pybaseutils-0.8.3/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9722 2023-06-07 03:32:53.000000 pybaseutils-0.8.3/pybaseutils/cvutils/video_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.479453 pybaseutils-0.8.3/pybaseutils/dataloader/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/dataloader/dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/dataloader/parser_textdata.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    32586 2023-06-19 03:44:02.000000 pybaseutils-0.8.3/pybaseutils/file_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.480002 pybaseutils-0.8.3/pybaseutils/font_style/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/font_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    97190 2023-06-14 03:03:27.000000 pybaseutils-0.8.3/pybaseutils/image_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/json_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/log.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.3/pybaseutils/logger.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.483197 pybaseutils-0.8.3/pybaseutils/maker/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/maker/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/convert_voc2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/convert_voc2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/convert_yolo2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/maker_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/maker/maker_voc.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.486149 pybaseutils-0.8.3/pybaseutils/metrics/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.3/pybaseutils/plot_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.487406 pybaseutils-0.8.3/pybaseutils/pycpp/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.3/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.3/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/pycpp/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.3/pybaseutils/setup_config.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/time_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.3/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.488263 pybaseutils-0.8.3/pybaseutils/transforms/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.3/pybaseutils/word_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.3/pybaseutils/worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.3/pybaseutils/yaml_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.471917 pybaseutils-0.8.3/pybaseutils.egg-info/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-06-19 03:45:15.000000 pybaseutils-0.8.3/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3491 2023-06-19 03:45:15.000000 pybaseutils-0.8.3/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2023-06-19 03:45:15.000000 pybaseutils-0.8.3/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.3/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2023-06-19 03:45:15.000000 pybaseutils-0.8.3/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2023-06-19 03:45:15.513545 pybaseutils-0.8.3/setup.cfg
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-0.8.3/setup.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.501545 pybaseutils-0.8.3/test_py/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.3/test_py/class_names.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.507081 pybaseutils-0.8.3/test_py/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.3/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.3/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.3/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.3/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.3/test_py/converter/CCPD.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.3/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.3/test_py/converter/TT100K.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.3/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.3/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      544 2023-06-16 03:40:08.000000 pybaseutils-0.8.3/test_py/demo1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1189 2023-05-30 10:27:09.000000 pybaseutils-0.8.3/test_py/demo2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.3/test_py/demo_async_await1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-0.8.3/test_py/demo_async_await2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4664 2023-06-01 07:22:44.000000 pybaseutils-0.8.3/test_py/demo_copy_files.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.3/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1342 2023-05-16 02:22:22.000000 pybaseutils-0.8.3/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.3/test_py/demo_for_trt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2943 2023-06-15 00:54:20.000000 pybaseutils-0.8.3/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/demo_gif.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1745 2023-05-24 03:16:30.000000 pybaseutils-0.8.3/test_py/demo_gif_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/demo_metrics.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/demo_mouse.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/demo_pandas.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.3/test_py/demo_plot.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.3/test_py/demo_standard_image .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.3/test_py/demo_standard_video .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/demo_taichi.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      779 2023-06-05 05:36:00.000000 pybaseutils-0.8.3/test_py/demo_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.3/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2440 2023-06-15 00:55:49.000000 pybaseutils-0.8.3/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.3/test_py/demo_word_similar.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/demo_worker1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/demo_worker2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.508115 pybaseutils-0.8.3/test_py/detector/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.3/test_py/detector/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6671 2023-05-04 08:11:18.000000 pybaseutils-0.8.3/test_py/detector/detect_face_person.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.509747 pybaseutils-0.8.3/test_py/flask_demo/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.3/test_py/flask_demo/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.3/test_py/flask_demo/func.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.3/test_py/flask_demo/server.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.512319 pybaseutils-0.8.3/test_py/image_correction/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.3/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.3/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.3/test_py/kafka_worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.3/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.3/test_py/performance.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pybaseutils-0.8.2/LICENCE` & `pybaseutils-0.8.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/PKG-INFO` & `pybaseutils-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,140 +1,139 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.2
+Version: 0.8.3
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
-Platform: UNKNOWN
 License-File: LICENCE
 
 base-utils
 ==========
 
 -  开源不易,麻烦给个【Star】
 -  源码 ： https://github.com/PanJinquan/base-utils
 -  安装包： https://pypi.org/project/pybaseutils/
 
-base\_utils(C++)
-----------------
+base_utils(C++)
+---------------
 
-base\_util是个人开发常用的C++库，集成了C/C++ OpenCV等常用的算法
+base_util是个人开发常用的C++库，集成了C/C++ OpenCV等常用的算法
 
 -  增加了debug测试宏定义，如时间测试，LOG信息等
 -  针对目标坐标点的卡尔曼滤波，加权平均滤波
 -  常用的文件处理函数
 -  常用的OpenCV图像处理函数
 
 pybaseutils(Python)
 -------------------
 
 pybaseutils是个人开发常用的python库，集成了python等常用的算法
 
 -  安装方法1：pip install pybaseutils (有延时，可能不是最新版本)
--  安装方法2：pip install --upgrade pybaseutils -i
+-  安装方法2：pip install –upgrade pybaseutils -i
    https://pypi.org/simple (从pypi源下载最新版本)
 
 一些问题修复说明
 ----------------
 
 -  `问题修复说明 <./docs/README.md>`__
 
 目录结构
 --------
 
 ::
 
-    ├── base_utils         # base_utils的C++源代码
-    ├── pybaseutils        # pybaseutils的python源代码
-    ├── data               # 相关测试数据
-    ├── test               # base_utils的测试代码
-    │   ├── build.sh
-    │   ├── CMakeLists.txt
-    │   ├── kalman_test.cpp
-    │   └── main.cpp
-    └── README.md
+   ├── base_utils         # base_utils的C++源代码
+   ├── pybaseutils        # pybaseutils的python源代码
+   ├── data               # 相关测试数据
+   ├── test               # base_utils的测试代码
+   │   ├── build.sh
+   │   ├── CMakeLists.txt
+   │   ├── kalman_test.cpp
+   │   └── main.cpp
+   └── README.md
+
+.. _base_utilsc-1:
 
-base\_utils(C++)
-================
+base_utils(C++)
+===============
 
 1.相关配置
 ----------
 
 -  OpenCV配置方法
 
 .. code:: cmake
 
-    # opencv set
-    find_package(OpenCV REQUIRED)
-    include_directories(${OpenCV_INCLUDE_DIRS} ./src/)
-    MESSAGE(STATUS "OpenCV_INCLUDE_DIRS = ${OpenCV_INCLUDE_DIRS}")
+   # opencv set
+   find_package(OpenCV REQUIRED)
+   include_directories(${OpenCV_INCLUDE_DIRS} ./src/)
+   MESSAGE(STATUS "OpenCV_INCLUDE_DIRS = ${OpenCV_INCLUDE_DIRS}")
 
 -  base-utils库的配置方法
 
 .. code:: cmake
 
-    # base-utils
-    set(BASE_ROOT ../) # 设置base-utils所在的根目录
-    add_subdirectory(${BASE_ROOT}/base_utils/ base_build) # 添加子目录到build中
-    include_directories(${BASE_ROOT}/base_utils/include)
-    include_directories(${BASE_ROOT}/base_utils/src)
-    MESSAGE(STATUS "BASE_ROOT = ${BASE_ROOT}")
+   # base-utils
+   set(BASE_ROOT ../) # 设置base-utils所在的根目录
+   add_subdirectory(${BASE_ROOT}/base_utils/ base_build) # 添加子目录到build中
+   include_directories(${BASE_ROOT}/base_utils/include)
+   include_directories(${BASE_ROOT}/base_utils/src)
+   MESSAGE(STATUS "BASE_ROOT = ${BASE_ROOT}")
 
 -  配置OpenCL（可选）
 
    1. OpenCL:
       https://software.intel.com/content/www/us/en/develop/tools/opencl-sdk/choose-download.html
    2. Android系统一般都支持OpenCL，Linux系统可参考如下配置：
 
 .. code:: bash
 
-    # 参考安装OpenCL： https://blog.csdn.net/qq_28483731/article/details/68235383，作为测试，安装`intel cpu版本的OpenCL`即可
-    # 安装clinfo，clinfo是一个显示OpenCL平台和设备的软件
-    sudo apt-get install clinfo
-    # 安装依赖
-    sudo apt install dkms xz-utils openssl libnuma1 libpciaccess0 bc curl libssl-dev lsb-core libicu-dev
-    sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
-    echo "deb http://download.mono-project.com/repo/debian wheezy main" | sudo tee /etc/apt/sources.list.d/mono-xamarin.list
-    sudo apt-get update
-    sudo apt-get install mono-complete
-    # 在intel官网上下载了intel SDK的tgz文件，并且解压
-    sudo sh install.sh
+   # 参考安装OpenCL： https://blog.csdn.net/qq_28483731/article/details/68235383，作为测试，安装`intel cpu版本的OpenCL`即可
+   # 安装clinfo，clinfo是一个显示OpenCL平台和设备的软件
+   sudo apt-get install clinfo
+   # 安装依赖
+   sudo apt install dkms xz-utils openssl libnuma1 libpciaccess0 bc curl libssl-dev lsb-core libicu-dev
+   sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
+   echo "deb http://download.mono-project.com/repo/debian wheezy main" | sudo tee /etc/apt/sources.list.d/mono-xamarin.list
+   sudo apt-get update
+   sudo apt-get install mono-complete
+   # 在intel官网上下载了intel SDK的tgz文件，并且解压
+   sudo sh install.sh
 
 2.Demo测试
 ----------
 
 -  ``build``
 
 .. code:: bash
 
-    cd test
-    bash build.sh
+   cd test
+   bash build.sh
 
 -  ``test/main.cpp``\ 测试样例
 
 .. code:: cpp
 
-    #include<opencv2/opencv.hpp>
-    #include<string>
-    #include "debug.h"
-    using namespace std;
-
-    int main() {
-        string path = "../../data/test_image/test1.jpg";
-        DEBUG_TIME(t1);
-        cv::Mat image = cv::imread(path);
-        LOGI("image:%s", path.c_str());
-        LOGD("image:%s", path.c_str());
-        LOGW("image:%s", path.c_str());
-        LOGE("image:%s", path.c_str());
-        LOGF("image:%s", path.c_str());
-        DEBUG_TIME(t2);
-        LOGI("rum time:%3.3fms", RUN_TIME(t2 - t1));
-        cv::waitKey(0);
-        DEBUG_IMSHOW("image", image);
-        return 0;
-    }
-
-
+   #include<opencv2/opencv.hpp>
+   #include<string>
+   #include "debug.h"
+   using namespace std;
+
+   int main() {
+       string path = "../../data/test_image/test1.jpg";
+       DEBUG_TIME(t1);
+       cv::Mat image = cv::imread(path);
+       LOGI("image:%s", path.c_str());
+       LOGD("image:%s", path.c_str());
+       LOGW("image:%s", path.c_str());
+       LOGE("image:%s", path.c_str());
+       LOGF("image:%s", path.c_str());
+       DEBUG_TIME(t2);
+       LOGI("rum time:%3.3fms", RUN_TIME(t2 - t1));
+       cv::waitKey(0);
+       DEBUG_IMSHOW("image", image);
+       return 0;
+   }
```

### Comparing `pybaseutils-0.8.2/pybaseutils/base64_utils.py` & `pybaseutils-0.8.3/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/base_audio/audio_utils.py` & `pybaseutils-0.8.3/pybaseutils/base_audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/batch_utils.py` & `pybaseutils-0.8.3/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/cluster/kmean.py` & `pybaseutils-0.8.3/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-0.8.3/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/cluster/similarity.py` & `pybaseutils-0.8.3/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/color_utils.py` & `pybaseutils-0.8.3/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/config_utils.py` & `pybaseutils-0.8.3/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/coords_utils.py` & `pybaseutils-0.8.3/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-0.8.3/pybaseutils/cvutils/corner_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/cvutils/monitor.py` & `pybaseutils-0.8.3/pybaseutils/cvutils/monitor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-0.8.3/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/cvutils/video_utils.py` & `pybaseutils-0.8.3/pybaseutils/cvutils/video_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
             isSuccess, frame = video_cap.read()
             if not isSuccess:
                 break
             if vis: image_utils.cv_show_image("frame", frame, use_rgb=False, delay=delay)
             video_writer.write(frame)
         count += 1
     video_cap.release()
+    video_writer.release()
 
 
 def write_video(self, frame):
     self.video_writer.write(frame)
 
 
 class CVVideo():
```

### Comparing `pybaseutils-0.8.2/pybaseutils/dataloader/dataset.py` & `pybaseutils-0.8.3/pybaseutils/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-0.8.3/pybaseutils/dataloader/parser_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/dataloader/parser_textdata.py` & `pybaseutils-0.8.3/pybaseutils/dataloader/parser_textdata.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-0.8.3/pybaseutils/dataloader/parser_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/file_utils.py` & `pybaseutils-0.8.3/pybaseutils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 def read_json_data(json_path):
     """
     读取数据
     :param json_path:
     :return:
     """
-    with open(json_path, 'r') as f:
+    with open(json_path, 'rb') as f:
         json_data = json.load(f)
     return json_data
 
 
 def write_json_path(out_json_path, json_data):
     """
     写入 JSON 数据
@@ -184,15 +184,15 @@
     :return: txt的数据列表
     Python中有三个去除头尾字符、空白符的函数，它们依次为:
     strip： 用来去除头尾字符、空白符(包括\n、\r、\t、' '，即：换行、回车、制表符、空格)
     lstrip：用来去除开头字符、空白符(包括\n、\r、\t、' '，即：换行、回车、制表符、空格)
     rstrip：用来去除结尾字符、空白符(包括\n、\r、\t、' '，即：换行、回车、制表符、空格)
     注意：这些函数都只会删除头和尾的字符，中间的不会删除。
     """
-    with open(filename, mode="r", encoding='utf-8') as f:
+    with open(filename, mode="rb", encoding='utf-8') as f:
         content_list = f.readlines()
         if split is None:
             content_list = [content.rstrip() for content in content_list]
             return content_list
         else:
             content_list = [content.rstrip().split(split) for content in content_list]
         if convertNum:
@@ -907,15 +907,15 @@
     '''
     想要获取linux设备网卡接口，并用列表进行保存
     :return:
     '''
     eth_list = []
     os.system("ls -l /sys/class/net/ | grep -v virtual | sed '1d' | awk 'BEGIN {FS=\"/\"} {print $NF}' > eth.yaml")
     try:
-        with open('./eth.yaml', "r") as f:
+        with open('./eth.yaml', "rb") as f:
             for line in f.readlines():
                 line = line.strip()
                 eth_list.append(line.lower())
     except Exception as e:
         print(e)
         eth_list = []
     return eth_list
```

### Comparing `pybaseutils-0.8.2/pybaseutils/font_style/__init__.py` & `pybaseutils-0.8.3/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/font_utils.py` & `pybaseutils-0.8.3/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/geometry_tools.py` & `pybaseutils-0.8.3/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/heatmap_utils.py` & `pybaseutils-0.8.3/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/image_utils.py` & `pybaseutils-0.8.3/pybaseutils/image_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1472,18 +1472,18 @@
 def draw_image_lines(image, points, pointline=[], color=(0, 0, 255), thickness=2):
     # points = np.asarray(points, dtype=np.int32)
     if pointline == "auto" or pointline == []:
         pointline = circle_line(len(points), iscircle=True)
     for point_index in pointline:
         point1 = tuple(points[point_index[0]])
         point2 = tuple(points[point_index[1]])
-        point1 = (int(point1[0]), int(point1[1]))
-        point2 = (int(point2[0]), int(point2[1]))
         if (not check_point(point1)) or (not check_point(point2)):
             continue
+        point1 = (int(point1[0]), int(point1[1]))
+        point2 = (int(point2[0]), int(point2[1]))
         cv2.line(image, point1, point2, color, thickness)  # 绿色，3个像素宽度
     return image
 
 
 def draw_image_arrowed_lines(image,
                              points,
                              pointline=[],
```

### Comparing `pybaseutils-0.8.2/pybaseutils/json_utils.py` & `pybaseutils-0.8.3/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/log.py` & `pybaseutils-0.8.3/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/logger.py` & `pybaseutils-0.8.3/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/maker/convert_labelme2voc.py` & `pybaseutils-0.8.3/pybaseutils/maker/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/maker/convert_voc2voc.py` & `pybaseutils-0.8.3/pybaseutils/maker/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/maker/convert_voc2yolo.py` & `pybaseutils-0.8.3/pybaseutils/maker/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/maker/convert_yolo2voc.py` & `pybaseutils-0.8.3/pybaseutils/maker/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/maker/maker_labelme.py` & `pybaseutils-0.8.3/pybaseutils/maker/maker_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/maker/maker_voc.py` & `pybaseutils-0.8.3/pybaseutils/maker/maker_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/metrics/accuracy.py` & `pybaseutils-0.8.3/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/metrics/average_meter.py` & `pybaseutils-0.8.3/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/metrics/class_report.py` & `pybaseutils-0.8.3/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/metrics/plot_pr.py` & `pybaseutils-0.8.3/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/metrics/plot_roc.py` & `pybaseutils-0.8.3/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/numpy_utils.py` & `pybaseutils-0.8.3/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/pandas_utils.py` & `pybaseutils-0.8.3/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/plot_utils.py` & `pybaseutils-0.8.3/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/pycpp/demo.py` & `pybaseutils-0.8.3/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/pycpp/main.py` & `pybaseutils-0.8.3/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/setup_config.py` & `pybaseutils-0.8.3/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/thread_utils.py` & `pybaseutils-0.8.3/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/time_utils.py` & `pybaseutils-0.8.3/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/tracemalloc_utils.py` & `pybaseutils-0.8.3/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-0.8.3/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/transforms/affine_transform.py` & `pybaseutils-0.8.3/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/word_utils.py` & `pybaseutils-0.8.3/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/worker.py` & `pybaseutils-0.8.3/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils/yaml_utils.py` & `pybaseutils-0.8.3/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-0.8.3/pybaseutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,140 +1,139 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.2
+Version: 0.8.3
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
-Platform: UNKNOWN
 License-File: LICENCE
 
 base-utils
 ==========
 
 -  开源不易,麻烦给个【Star】
 -  源码 ： https://github.com/PanJinquan/base-utils
 -  安装包： https://pypi.org/project/pybaseutils/
 
-base\_utils(C++)
-----------------
+base_utils(C++)
+---------------
 
-base\_util是个人开发常用的C++库，集成了C/C++ OpenCV等常用的算法
+base_util是个人开发常用的C++库，集成了C/C++ OpenCV等常用的算法
 
 -  增加了debug测试宏定义，如时间测试，LOG信息等
 -  针对目标坐标点的卡尔曼滤波，加权平均滤波
 -  常用的文件处理函数
 -  常用的OpenCV图像处理函数
 
 pybaseutils(Python)
 -------------------
 
 pybaseutils是个人开发常用的python库，集成了python等常用的算法
 
 -  安装方法1：pip install pybaseutils (有延时，可能不是最新版本)
--  安装方法2：pip install --upgrade pybaseutils -i
+-  安装方法2：pip install –upgrade pybaseutils -i
    https://pypi.org/simple (从pypi源下载最新版本)
 
 一些问题修复说明
 ----------------
 
 -  `问题修复说明 <./docs/README.md>`__
 
 目录结构
 --------
 
 ::
 
-    ├── base_utils         # base_utils的C++源代码
-    ├── pybaseutils        # pybaseutils的python源代码
-    ├── data               # 相关测试数据
-    ├── test               # base_utils的测试代码
-    │   ├── build.sh
-    │   ├── CMakeLists.txt
-    │   ├── kalman_test.cpp
-    │   └── main.cpp
-    └── README.md
+   ├── base_utils         # base_utils的C++源代码
+   ├── pybaseutils        # pybaseutils的python源代码
+   ├── data               # 相关测试数据
+   ├── test               # base_utils的测试代码
+   │   ├── build.sh
+   │   ├── CMakeLists.txt
+   │   ├── kalman_test.cpp
+   │   └── main.cpp
+   └── README.md
+
+.. _base_utilsc-1:
 
-base\_utils(C++)
-================
+base_utils(C++)
+===============
 
 1.相关配置
 ----------
 
 -  OpenCV配置方法
 
 .. code:: cmake
 
-    # opencv set
-    find_package(OpenCV REQUIRED)
-    include_directories(${OpenCV_INCLUDE_DIRS} ./src/)
-    MESSAGE(STATUS "OpenCV_INCLUDE_DIRS = ${OpenCV_INCLUDE_DIRS}")
+   # opencv set
+   find_package(OpenCV REQUIRED)
+   include_directories(${OpenCV_INCLUDE_DIRS} ./src/)
+   MESSAGE(STATUS "OpenCV_INCLUDE_DIRS = ${OpenCV_INCLUDE_DIRS}")
 
 -  base-utils库的配置方法
 
 .. code:: cmake
 
-    # base-utils
-    set(BASE_ROOT ../) # 设置base-utils所在的根目录
-    add_subdirectory(${BASE_ROOT}/base_utils/ base_build) # 添加子目录到build中
-    include_directories(${BASE_ROOT}/base_utils/include)
-    include_directories(${BASE_ROOT}/base_utils/src)
-    MESSAGE(STATUS "BASE_ROOT = ${BASE_ROOT}")
+   # base-utils
+   set(BASE_ROOT ../) # 设置base-utils所在的根目录
+   add_subdirectory(${BASE_ROOT}/base_utils/ base_build) # 添加子目录到build中
+   include_directories(${BASE_ROOT}/base_utils/include)
+   include_directories(${BASE_ROOT}/base_utils/src)
+   MESSAGE(STATUS "BASE_ROOT = ${BASE_ROOT}")
 
 -  配置OpenCL（可选）
 
    1. OpenCL:
       https://software.intel.com/content/www/us/en/develop/tools/opencl-sdk/choose-download.html
    2. Android系统一般都支持OpenCL，Linux系统可参考如下配置：
 
 .. code:: bash
 
-    # 参考安装OpenCL： https://blog.csdn.net/qq_28483731/article/details/68235383，作为测试，安装`intel cpu版本的OpenCL`即可
-    # 安装clinfo，clinfo是一个显示OpenCL平台和设备的软件
-    sudo apt-get install clinfo
-    # 安装依赖
-    sudo apt install dkms xz-utils openssl libnuma1 libpciaccess0 bc curl libssl-dev lsb-core libicu-dev
-    sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
-    echo "deb http://download.mono-project.com/repo/debian wheezy main" | sudo tee /etc/apt/sources.list.d/mono-xamarin.list
-    sudo apt-get update
-    sudo apt-get install mono-complete
-    # 在intel官网上下载了intel SDK的tgz文件，并且解压
-    sudo sh install.sh
+   # 参考安装OpenCL： https://blog.csdn.net/qq_28483731/article/details/68235383，作为测试，安装`intel cpu版本的OpenCL`即可
+   # 安装clinfo，clinfo是一个显示OpenCL平台和设备的软件
+   sudo apt-get install clinfo
+   # 安装依赖
+   sudo apt install dkms xz-utils openssl libnuma1 libpciaccess0 bc curl libssl-dev lsb-core libicu-dev
+   sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
+   echo "deb http://download.mono-project.com/repo/debian wheezy main" | sudo tee /etc/apt/sources.list.d/mono-xamarin.list
+   sudo apt-get update
+   sudo apt-get install mono-complete
+   # 在intel官网上下载了intel SDK的tgz文件，并且解压
+   sudo sh install.sh
 
 2.Demo测试
 ----------
 
 -  ``build``
 
 .. code:: bash
 
-    cd test
-    bash build.sh
+   cd test
+   bash build.sh
 
 -  ``test/main.cpp``\ 测试样例
 
 .. code:: cpp
 
-    #include<opencv2/opencv.hpp>
-    #include<string>
-    #include "debug.h"
-    using namespace std;
-
-    int main() {
-        string path = "../../data/test_image/test1.jpg";
-        DEBUG_TIME(t1);
-        cv::Mat image = cv::imread(path);
-        LOGI("image:%s", path.c_str());
-        LOGD("image:%s", path.c_str());
-        LOGW("image:%s", path.c_str());
-        LOGE("image:%s", path.c_str());
-        LOGF("image:%s", path.c_str());
-        DEBUG_TIME(t2);
-        LOGI("rum time:%3.3fms", RUN_TIME(t2 - t1));
-        cv::waitKey(0);
-        DEBUG_IMSHOW("image", image);
-        return 0;
-    }
-
-
+   #include<opencv2/opencv.hpp>
+   #include<string>
+   #include "debug.h"
+   using namespace std;
+
+   int main() {
+       string path = "../../data/test_image/test1.jpg";
+       DEBUG_TIME(t1);
+       cv::Mat image = cv::imread(path);
+       LOGI("image:%s", path.c_str());
+       LOGD("image:%s", path.c_str());
+       LOGW("image:%s", path.c_str());
+       LOGE("image:%s", path.c_str());
+       LOGF("image:%s", path.c_str());
+       DEBUG_TIME(t2);
+       LOGI("rum time:%3.3fms", RUN_TIME(t2 - t1));
+       cv::waitKey(0);
+       DEBUG_IMSHOW("image", image);
+       return 0;
+   }
```

### Comparing `pybaseutils-0.8.2/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-0.8.3/pybaseutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/README.md` & `pybaseutils-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/setup.py` & `pybaseutils-0.8.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 import os
 import pybaseutils
 import pypandoc
 from setuptools import setup, find_packages
 
 root = os.path.dirname(__file__)
-long_description = pypandoc.convert('README.md', 'rst')
+long_description = pypandoc.convert_file('README.md', 'rst')
 setup(name='pybaseutils',
       version=pybaseutils.__version__,
       description='pybaseutils',
       long_description=long_description,
       url='https://github.com/PanJinquan/base-utils',
       author='PanJinquan',
       author_email='390737991@qq.com',
@@ -46,11 +46,11 @@
         source：源文件
         to：目标文件的格式，比如html、rst、md等
         format：源文件的格式，比如html、rst、md等。默认为None，则会自动检测
         encoding：指定编码集
         outputfile：目标文件，比如test.html（注意outputfile的后缀要和to一致）
     """
     # 修复中文乱码问题： <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
-    pypandoc.convert(in_file, 'html', format='md', outputfile="README.html", encoding='utf-8')
-    pypandoc.convert(in_file, 'rst', format='md', outputfile="README.rst", encoding='utf-8')
+    pypandoc.convert_file(in_file, 'html', format='md', outputfile="README.html", encoding='utf-8')
+    pypandoc.convert_file(in_file, 'rst', format='md', outputfile="README.rst", encoding='utf-8')
 
 # readme2rst()
```

### Comparing `pybaseutils-0.8.2/test_py/class_names.py` & `pybaseutils-0.8.3/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/AffectNet.py` & `pybaseutils-0.8.3/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/AsianMovie.py` & `pybaseutils-0.8.3/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/BITVehicle2voc.py` & `pybaseutils-0.8.3/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/BSTLD2voc.py` & `pybaseutils-0.8.3/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/CCPD.py` & `pybaseutils-0.8.3/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/CCPD2voc.py` & `pybaseutils-0.8.3/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-0.8.3/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/TT100K.py` & `pybaseutils-0.8.3/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/tt100k_utils.py` & `pybaseutils-0.8.3/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/converter/ua_detrac2voc.py` & `pybaseutils-0.8.3/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo2.py` & `pybaseutils-0.8.3/test_py/demo2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_async_await2.py` & `pybaseutils-0.8.3/test_py/demo_async_await2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,67 @@
 # -*-coding: utf-8 -*-
 """
     @Author : 
     @E-mail : 
     @Date   : 2023-05-25 11:47:17
     @Brief  : <Python — 异步async/await> https://blog.csdn.net/weixin_45804031/article/details/124579021
 """
+import os
 import asyncio
 import requests
+from typing import Callable
 import time
 import asyncio
 import requests
 from concurrent import futures
-
+from pybaseutils import time_utils
 executor = futures.ThreadPoolExecutor(max_workers=5)
 
 
-def task(params):
+def task_process(params):
     time.sleep(1)
     print(params)
+    params["data"] = params["data"] + "/1"
     time.sleep(1)
     return params
 
 
-async def async_upload_image(params):
-    # 将content字段中所有的文件和图片资源都上传到服务器，返回url代替
+async def async_task(params, task: Callable):
     def run_in_executor(params):
         params = task(params)
         return params
 
     loop = asyncio.get_event_loop()
     return await loop.run_in_executor(executor, run_in_executor, params)
 
 
-async def http_api(params):
-    result = await async_upload_image(params)
+async def http_api(params, task: Callable):
+    result = await async_task(params, task=task)
     return result
 
 
-if __name__ == "__main__":
-    tasks = []
+@time_utils.performance("test_time")
+def test_time():
     url = 'https://www.baidu.com'
     for i in range(0, 3):
         params = {"data": url, "n": i}
-        r = http_api(params)
-        tasks.append(r)
+        r = task_process(params)
+
+
+@time_utils.performance("async_test_time")
+def async_test_time():
+    tasks = []
+    url = 'https://www.baidu.com'
+    for i in range(0, 3):
+        params = {"data": url, "id": i}
+        t = http_api(params, task=task_process)
+        tasks.append(t)
     loop = asyncio.get_event_loop()
-    loop.run_until_complete(asyncio.wait(tasks))
+    rs, s = loop.run_until_complete(asyncio.wait(tasks))
+    result = [r.result() for r in rs]
     loop.close()
-    print(tasks)
+    print(result)
+
+
+if __name__ == "__main__":
+    async_test_time()
+    # test_time()
```

### Comparing `pybaseutils-0.8.2/test_py/demo_copy_files.py` & `pybaseutils-0.8.3/test_py/demo_copy_files.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_copy_files_for_voc.py` & `pybaseutils-0.8.3/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_ffmpy.py` & `pybaseutils-0.8.3/test_py/demo_ffmpy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_get_file_list.py` & `pybaseutils-0.8.3/test_py/demo_get_file_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,10 +63,10 @@
         max_num = min(max_num, len(file_list))
         file_list = file_list[0:max_num]
     file_utils.write_list_data(filename, file_list)
     print("num files:{},out_path:{}".format(len(file_list), filename))
 
 
 if __name__ == "__main__":
-    file_dir = "/home/dm/nasdata/dataset/tmp/fall/Fall-Down-Det-v3/JPEGImages"
+    file_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/标注数据/岗评项目_室内电力操作检测-22labels/JPEGImages"
     save_file_list(file_dir, prefix="", postfix=file_utils.IMG_POSTFIX + ["*.JPG"], only_id=False, shuffle=False,
                    max_num=None)
```

### Comparing `pybaseutils-0.8.2/test_py/demo_gif.py` & `pybaseutils-0.8.3/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_gif_video.py` & `pybaseutils-0.8.3/test_py/demo_gif_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_metrics.py` & `pybaseutils-0.8.3/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_mouse.py` & `pybaseutils-0.8.3/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_pandas.py` & `pybaseutils-0.8.3/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_plot.py` & `pybaseutils-0.8.3/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_standard_image .py` & `pybaseutils-0.8.3/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_standard_video .py` & `pybaseutils-0.8.3/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_taichi.py` & `pybaseutils-0.8.3/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_video.py` & `pybaseutils-0.8.3/test_py/demo_video.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pybaseutils.cvutils import video_utils
 
 
 def video2frames_demo(root, out):
     files = file_utils.get_files_list(root, postfix=["*.avi", "*.mp4"])
     for video_file in files:
         print(video_file)
-        video_utils.video2frames_similarity(video_file, out_dir=out, func=None, interval=50, vis=True)
+        video_utils.video2frames_similarity(video_file, out_dir=out, func=None, interval=100, vis=True)
         # video_utils.video2frames(video_file, out_dir=out, func=None, interval=50, vis=True)
 
 
 if __name__ == "__main__":
     root = "/home/dm/nasdata/release/CSG/南方电网视频/videos"
     out = root + "-frame"
     video2frames_demo(root, out)
```

### Comparing `pybaseutils-0.8.2/test_py/demo_voc_crop.py` & `pybaseutils-0.8.3/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_voc_vis.py` & `pybaseutils-0.8.3/test_py/demo_voc_vis.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     # from models.transforms import data_transforms
     # filename = "/home/dm/nasdata/dataset/csdn/traffic light/VOC/train.txt"
     # class_name = "/home/dm/nasdata/dataset/csdn/traffic light/VOC/class_name.txt"
     # filename = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-v1/train.txt"
     # filename = "/home/dm/nasdata/dataset/csdn/face_person/MPII/test.txt"
     # filename = "/home/dm/nasdata/dataset/csdn/Eyeglasses/dataset/face-eyeglasses/trainval.txt"
     # filename = "/home/dm/nasdata/dataset/tmp/insects/VOC2/VOC/VOCdevkit/trainval.txt"
-    filename = "/home/dm/cv/panjinquan/dataset/tmp/fall/Fall-Down-Det-v2/train.txt"
+    filename = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/标注数据/岗评项目_室内电力操作检测-22labels/file_list.txt"
     # filename = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-old/train.txt"
     # class_name = ["face", "face-eyeglasses"]
     # class_name = "/home/dm/nasdata/dataset/tmp/traffic-sign/TT100K/VOC/train/class_name.txt"
     # class_name = ["unique"]
     # class_name =None
     # class_name =['10+', 'dog', 'down', 'person']
     use_rgb = False
@@ -32,15 +32,15 @@
                                     transform=None,
                                     use_rgb=use_rgb,
                                     check=False,
                                     shuffle=False)
     print("have num:{}".format(len(dataset)))
     class_name = dataset.class_name
     for i in range(len(dataset)):
-        i=113
+        # i=113
         print(i)
         data = dataset.__getitem__(i)
         image, targets, image_id = data["image"], data["target"], data["image_id"]
         print(image_id)
         bboxes, labels = targets[:, 0:4], targets[:, 4:5]
         image = parser_voc.show_target_image(image, bboxes, labels, normal=False, transpose=False,
                                              class_name=class_name, use_rgb=use_rgb,thickness=2, fontScale=1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybaseutils-0.8.2/test_py/demo_word_similar.py` & `pybaseutils-0.8.3/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_worker1.py` & `pybaseutils-0.8.3/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/demo_worker2.py` & `pybaseutils-0.8.3/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/detector/detect_face_person.py` & `pybaseutils-0.8.3/test_py/detector/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/flask_demo/server.py` & `pybaseutils-0.8.3/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-0.8.3/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-0.8.3/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-0.8.3/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/kafka_worker.py` & `pybaseutils-0.8.3/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/men_tracemalloc.py` & `pybaseutils-0.8.3/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.2/test_py/performance.py` & `pybaseutils-0.8.3/test_py/performance.py`

 * *Files identical despite different names*

