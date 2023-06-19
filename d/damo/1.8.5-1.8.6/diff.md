# Comparing `tmp/damo-1.8.5.tar.gz` & `tmp/damo-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.5.tar", last modified: Mon Jun 12 17:22:53 2023, max compression
+gzip compressed data, was "damo-1.8.6.tar", last modified: Mon Jun 19 21:07:26 2023, max compression
```

## Comparing `damo-1.8.5.tar` & `damo-1.8.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:53.175708 damo-1.8.5/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-12 17:22:53.175708 damo-1.8.5/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7641 2023-06-12 17:22:49.000000 damo-1.8.5/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.5/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-06-12 17:22:53.175708 damo-1.8.5/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.5/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:53.159708 damo-1.8.5/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:53.171708 damo-1.8.5/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:49.000000 damo-1.8.5/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-04 17:35:27.000000 damo-1.8.5/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.5/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34675 2023-06-04 19:34:22.000000 damo-1.8.5/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-05-29 19:08:47.000000 damo-1.8.5/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17097 2023-06-04 19:28:36.000000 damo-1.8.5/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    22589 2023-06-04 19:06:02.000000 damo-1.8.5/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19134 2023-06-04 19:28:46.000000 damo-1.8.5/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3880 2023-06-10 21:05:04.000000 damo-1.8.5/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2002 2023-06-03 19:10:51.000000 damo-1.8.5/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      891 2023-06-03 18:38:32.000000 damo-1.8.5/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13295 2023-06-03 19:10:58.000000 damo-1.8.5/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2749 2023-06-03 19:10:58.000000 damo-1.8.5/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5615 2023-06-04 19:26:26.000000 damo-1.8.5/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4132 2023-06-11 18:10:19.000000 damo-1.8.5/src/damo/damo_record_info.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-04 19:50:04.000000 damo-1.8.5/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3195 2023-06-11 19:00:48.000000 damo-1.8.5/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1582 2023-06-04 19:26:37.000000 damo-1.8.5/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      974 2023-06-11 18:40:28.000000 damo-1.8.5/src/damo/damo_show.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1653 2023-06-11 19:01:29.000000 damo-1.8.5/src/damo/damo_show_accesses.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      837 2023-06-11 18:26:23.000000 damo-1.8.5/src/damo/damo_show_snapshot.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-11 17:45:41.000000 damo-1.8.5/src/damo/damo_show_status.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-10 19:35:18.000000 damo-1.8.5/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1073 2023-06-10 21:05:04.000000 damo-1.8.5/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3056 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1016 2023-06-10 21:05:04.000000 damo-1.8.5/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.5/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3943 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-06-12 17:21:48.000000 damo-1.8.5/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5553 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:53.171708 damo-1.8.5/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1316 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:26.797932 damo-1.8.6/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-19 21:07:26.797932 damo-1.8.6/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7641 2023-06-19 21:07:22.000000 damo-1.8.6/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.6/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-06-19 21:07:26.797932 damo-1.8.6/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.6/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:26.781932 damo-1.8.6/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:26.797932 damo-1.8.6/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:22.000000 damo-1.8.6/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-04 17:35:27.000000 damo-1.8.6/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.6/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34675 2023-06-17 18:34:52.000000 damo-1.8.6/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-05-29 19:08:47.000000 damo-1.8.6/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17097 2023-06-04 19:28:36.000000 damo-1.8.6/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    22860 2023-06-18 18:09:23.000000 damo-1.8.6/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19134 2023-06-04 19:28:46.000000 damo-1.8.6/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3880 2023-06-10 21:05:04.000000 damo-1.8.6/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.8.6/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.8.6/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13386 2023-06-18 17:39:30.000000 damo-1.8.6/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.8.6/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5615 2023-06-04 19:26:26.000000 damo-1.8.6/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-06-18 17:31:57.000000 damo-1.8.6/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-04 19:50:04.000000 damo-1.8.6/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3376 2023-06-18 17:35:15.000000 damo-1.8.6/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.8.6/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      974 2023-06-11 18:40:28.000000 damo-1.8.6/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1653 2023-06-11 19:01:29.000000 damo-1.8.6/src/damo/damo_show_accesses.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      837 2023-06-11 18:26:23.000000 damo-1.8.6/src/damo/damo_show_snapshot.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-11 17:45:41.000000 damo-1.8.6/src/damo/damo_show_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-10 19:35:18.000000 damo-1.8.6/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1073 2023-06-10 21:05:04.000000 damo-1.8.6/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2956 2023-06-18 18:12:17.000000 damo-1.8.6/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1016 2023-06-10 21:05:04.000000 damo-1.8.6/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.6/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.6/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3930 2023-06-18 17:35:51.000000 damo-1.8.6/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-06-19 21:06:16.000000 damo-1.8.6/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5551 2023-06-18 17:22:23.000000 damo-1.8.6/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-19 21:07:26.797932 damo-1.8.6/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1316 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-06-19 21:07:26.000000 damo-1.8.6/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.5/PKG-INFO` & `damo-1.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.5
+Version: 1.8.6
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +87,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.5/README.md` & `damo-1.8.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -72,19 +72,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.5/setup.py` & `damo-1.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damo_deprecated.py` & `damo-1.8.6/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damo_deprecation_notice.py` & `damo-1.8.6/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damo_dist.py` & `damo-1.8.6/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damo_fmt_str.py` & `damo-1.8.6/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damo_fs.py` & `damo-1.8.6/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damo_paddr_layout.py` & `damo-1.8.6/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damo_subcmds.py` & `damo-1.8.6/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damon.py` & `damo-1.8.6/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damon_args.py` & `damo-1.8.6/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damon_dbgfs.py` & `damo-1.8.6/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/_damon_result.py` & `damo-1.8.6/src/damo/_damon_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,60 +45,56 @@
                 self.end_time, raw)),
             ('regions', [r.to_kvpairs() for r in self.regions])])
 
 class DamonRecord:
     '''
     Contains data access monitoring results for single target
     '''
+    kdamond_idx = None
+    context_idx = None
     intervals = None
+    scheme_idx = None
     target_id = None
     snapshots = None
 
-    def __init__(self, intervals, target_id):
+    def __init__(self, kd_idx, ctx_idx, intervals, scheme_idx, target_id):
+        self.kdamond_idx = kd_idx
+        self.context_idx = ctx_idx
         self.intervals = intervals
+        self.scheme_idx = scheme_idx
         self.target_id = target_id
         self.snapshots = []
 
     @classmethod
     def from_kvpairs(cls, kv):
-        intervals = None
-        if 'intervals' in kv:
-            intervals = _damon.DamonIntervals.from_kvpairs(kv['intervals'])
-
-        record = DamonRecord(intervals, kv['target_id'])
+        for keyword in ['kdamond_idx', 'context_idx', 'intervals',
+                'scheme_idx']:
+            if not keyword in kv:
+                kv[keyword] = None
+
+        record = DamonRecord(kv['kdamond_idx'], kv['context_idx'],
+                _damon.DamonIntervals.from_kvpairs(kv['intervals'])
+                if kv['intervals'] != None else None,
+                kv['scheme_idx'], kv['target_id'])
         record.snapshots = [DamonSnapshot.from_kvpairs(s)
                 for s in kv['snapshots']]
 
         return record
 
     def to_kvpairs(self, raw=False):
         ordered_dict = collections.OrderedDict()
-        if self.intervals != None:
-            ordered_dict['intervals'] = self.intervals.to_kvpairs(raw)
+        ordered_dict['kdamond_idx'] = self.kdamond_idx
+        ordered_dict['context_idx'] = self.context_idx
+        ordered_dict['intervals'] = (self.intervals.to_kvpairs(raw)
+                if self.intervals != None else None)
+        ordered_dict['scheme_idx'] = self.scheme_idx
         ordered_dict['target_id'] = self.target_id
         ordered_dict['snapshots'] = [s.to_kvpairs(raw) for s in self.snapshots]
         return ordered_dict
 
-class DamonResult:
-    '''
-    Contains data access monitoring results.
-    '''
-    records = None
-
-    def __init__(self):
-        self.records = []
-
-    def record_of(self, target_id, intervals):
-        for record in self.records:
-            if record.target_id == target_id:
-                return record
-        record = DamonRecord(intervals, target_id)
-        self.records.append(record)
-        return record
-
 # for monitoring results manipulation
 
 def regions_intersect(r1, r2):
     return not (r1.end <= r2.start or r2.end <= r1.start)
 
 def add_region(regions, region, nr_acc_to_add):
     for r in regions:
@@ -153,16 +149,16 @@
         to_aggregate.append(snapshot)
         interval_ns = to_aggregate[-1].end_time - to_aggregate[0].start_time
         if interval_ns >= aggregate_interval_us * 1000:
             adjusted.append(aggregate_snapshots(to_aggregate))
             to_aggregate = []
     return adjusted
 
-def adjust_result(result, aggregate_interval, nr_snapshots_to_skip):
-    for record in result.records:
+def adjust_records(records, aggregate_interval, nr_snapshots_to_skip):
+    for record in records:
         if record.intervals != None:
             record.intervals.aggr = aggregate_interval
         record.snapshots = adjusted_snapshots(
                 record.snapshots[nr_snapshots_to_skip:], aggregate_interval)
 
 # For reading monitoring results from a file
 
@@ -194,24 +190,24 @@
         region = _damon.DamonRegion(start_addr, end_addr,
                 nr_accesses, _damon.unit_samples,
                 None, _damon.unit_aggr_intervals)
         snapshot.regions.append(region)
     return snapshot
 
 # if number of snapshots is one and the file type is record or perf script,
-# write_damon_result() adds a fake snapshot for snapshot start time deduction.
+# write_damon_records() adds a fake snapshot for snapshot start time deduction.
 def is_fake_snapshot(snapshot):
     if len(snapshot.regions) != 1:
         return False
     r = snapshot.regions[0]
     return (r.start == 0 and r.end == 0 and
             r.nr_accesses.samples == -1 and r.age.aggr_intervals == -1)
 
-def set_first_snapshot_start_time(result):
-    for record in result.records:
+def set_first_snapshot_start_time(records):
+    for record in records:
         snapshots = record.snapshots
         if len(snapshots) < 2:
             break
         end_time = snapshots[-1].end_time
         start_time = snapshots[0].end_time
         nr_snapshots = len(snapshots) - 1
         snapshot_time = float(end_time - start_time) / nr_snapshots
@@ -222,47 +218,55 @@
 
 def warn_record_type_deprecation():
     _damo_deprecation_notice.will_be_deprecated(
             feature='\'record\' file type support',
             deadline='2023-Q3',
             additional_notice='use json_compressed type instead.')
 
+def record_of(target_id, records, intervals):
+    for record in records:
+        if record.target_id == target_id:
+            return record
+    record = DamonRecord(None, None, intervals, None, target_id)
+    records.append(record)
+    return record
+
 def parse_binary_format_record(file_path, monitoring_intervals):
     warn_record_type_deprecation()
     with open(file_path, 'rb') as f:
         fmt_version = read_record_format_version(f)
-        result = DamonResult()
+        records = []
         while True:
             end_time = read_end_time_from_record_file(f)
             if end_time == None:
                 break
 
             nr_tasks = struct.unpack('I', f.read(4))[0]
             for t in range(nr_tasks):
                 if fmt_version == 1:
                     target_id = struct.unpack('i', f.read(4))[0]
                 else:
                     target_id = struct.unpack('L', f.read(8))[0]
 
-                record = result.record_of(target_id, monitoring_intervals)
+                record = record_of(target_id, records, monitoring_intervals)
                 if len(record.snapshots) == 0:
                     start_time = None
                 else:
                     start_time = record.snapshots[-1].end_time
                     if end_time < start_time:
                         return None, 'snapshot is not sorted by time'
                 try:
                     snapshot = read_snapshot_from_record_file(f,
                             start_time, end_time)
                 except Exception as e:
                     return None, 'snapshot reading failead: %s' % e
                 record.snapshots.append(snapshot)
 
-    set_first_snapshot_start_time(result)
-    return result, None
+    set_first_snapshot_start_time(records)
+    return records, None
 
 def parse_perf_script_line(line):
         '''
         example line is as below:
 
         kdamond.0  4452 [000] 82877.315633: damon:damon_aggregated: \
                 target_id=18446623435582458880 nr_regions=17 \
@@ -291,23 +295,23 @@
         region = _damon.DamonRegion(start_addr, end_addr,
                 nr_accesses, _damon.unit_samples,
                 age, _damon.unit_aggr_intervals)
 
         return region, end_time, target_id, nr_regions
 
 def parse_perf_script(script_output, monitoring_intervals):
-    result = DamonResult()
+    records = []
     snapshot = None
 
     for line in script_output.split('\n'):
         region, end_time, target_id, nr_regions = parse_perf_script_line(line)
         if region == None:
             continue
 
-        record = result.record_of(target_id, monitoring_intervals)
+        record = record_of(target_id, records, monitoring_intervals)
         if len(record.snapshots) == 0:
             start_time = None
         else:
             start_time = record.snapshots[-1].end_time
             if start_time > end_time:
                 return None, 'trace is not time-sorted'
 
@@ -316,16 +320,16 @@
             record.snapshots.append(snapshot)
         snapshot = record.snapshots[-1]
         snapshot.regions.append(region)
 
         if len(snapshot.regions) == nr_regions:
             snapshot = None
 
-    set_first_snapshot_start_time(result)
-    return result, None
+    set_first_snapshot_start_time(records)
+    return records, None
 
 def set_perf_path(perf_path):
     global PERF
     PERF = perf_path
 
     # Test perf record for damon event
     err = None
@@ -337,33 +341,31 @@
                     stderr=subprocess.PIPE)
         except:
             err = 'perf record not working with "%s"' % PERF
     except:
         err = 'perf not found at "%s"' % PERF
     return err
 
-def parse_damon_record_json_compressed(result_file):
+def parse_json_compressed(result_file):
     with open(result_file, 'rb') as f:
         compressed = f.read()
     decompressed = zlib.decompress(compressed).decode()
     kvpairs = json.loads(decompressed)
-    result = DamonResult()
-    result.records = [DamonRecord.from_kvpairs(kvp) for kvp in kvpairs]
-    return result
+    return [DamonRecord.from_kvpairs(kvp) for kvp in kvpairs]
 
-def parse_damon_result(result_file, monitoring_intervals=None):
+def parse_records_file(result_file, monitoring_intervals=None):
     '''
-    Return monitoring results and error string
+    Return monitoring results records and error string
     '''
 
     file_type = subprocess.check_output(
             ['file', '-b', result_file]).decode().strip()
     if file_type == 'zlib compressed data':
         try:
-            return parse_damon_record_json_compressed(result_file), None
+            return parse_json_compressed(result_file), None
         except Exception as e:
             return None, 'failed parsing json compressed file (%s)' % e
 
     perf_script_output = None
     if file_type == 'ASCII text':
         with open(result_file, 'r') as f:
             perf_script_output = f.read()
@@ -375,54 +377,53 @@
                         [PERF, 'script', '-i', result_file],
                         stderr=fnull).decode()
         except:
             # Should be record format file
             pass
     if perf_script_output != None:
         return parse_perf_script(perf_script_output, monitoring_intervals)
-
     return parse_binary_format_record(result_file, monitoring_intervals)
 
 # for writing monitoring results to a file
 
-def write_damon_record_json_compressed(result, file_path):
-    json_str = json.dumps([r.to_kvpairs(r) for r in result.records], indent=4)
+def write_json_compressed(records, file_path):
+    json_str = json.dumps([r.to_kvpairs(raw=True) for r in records], indent=4)
     compressed = zlib.compress(json_str.encode())
     with open(file_path, 'wb') as f:
         f.write(compressed)
 
-def add_fake_snapshot_if_needed(result):
+def add_fake_snapshot_if_needed(records):
     '''
     perf and record file format stores only snapshot end time.  For a record
     having only single snapshot, hence, the reader of the files cannot knwo the
     start time of the snapshot.  Add a fake snapshot for the case.
     '''
 
-    for record in result.records:
+    for record in records:
         snapshots = record.snapshots
         if len(snapshots) != 1:
             continue
         snapshot = snapshots[0]
         snap_duration = snapshot.end_time - snapshot.start_time
         fake_snapshot = DamonSnapshot(snapshot.end_time,
                 snapshot.end_time + snap_duration)
         # -1 nr_accesses.samples / -1 age.aggr_intervals means fake
         fake_snapshot.regions = [_damon.DamonRegion(0, 0,
             -1, _damon.unit_samples, -1, _damon.unit_aggr_intervals)]
         snapshots.append(fake_snapshot)
 
-def write_damon_record(result, file_path, format_version):
+def write_binary(records, file_path, format_version):
     warn_record_type_deprecation()
-    add_fake_snapshot_if_needed(result)
+    add_fake_snapshot_if_needed(records)
 
     with open(file_path, 'wb') as f:
         f.write(b'damon_recfmt_ver')
         f.write(struct.pack('i', format_version))
 
-        for record in result.records:
+        for record in records:
             snapshots = record.snapshots
             for snapshot in snapshots:
                 f.write(struct.pack('l', snapshot.end_time // 1000000000))
                 f.write(struct.pack('l', snapshot.end_time % 1000000000))
 
                 f.write(struct.pack('I', 1))
 
@@ -433,26 +434,26 @@
 
                 f.write(struct.pack('I', len(snapshot.regions)))
                 for region in snapshot.regions:
                     f.write(struct.pack('L', region.start))
                     f.write(struct.pack('L', region.end))
                     f.write(struct.pack('I', region.nr_accesses.samples))
 
-def write_damon_perf_script(result, file_path):
+def write_perf_script(records, file_path):
     '''
     Example of the normal perf script output:
 
     kdamond.0  4452 [000] 82877.315633: damon:damon_aggregated: \
             target_id=18446623435582458880 nr_regions=17 \
             140731667070976-140731668037632: 0 3
     '''
 
-    add_fake_snapshot_if_needed(result)
+    add_fake_snapshot_if_needed(records)
     with open(file_path, 'w') as f:
-        for record in result.records:
+        for record in records:
             snapshots = record.snapshots
             for snapshot in snapshots:
                 for region in snapshot.regions:
                     f.write(' '.join(['kdamond.x', 'xxxx', 'xxxx',
                         '%f:' % (snapshot.end_time / 1000000000.0),
                         'damon:damon_aggregated:',
                         'target_id=%s' % record.target_id,
@@ -476,36 +477,37 @@
 file_type_json_compressed = 'json_compressed'
 
 file_types = [file_type_json_compressed, file_type_perf_script,
         file_type_perf_data, file_type_record]
 self_write_supported_file_types = [file_type_json_compressed,
         file_type_perf_script, file_type_record]
 
-def write_damon_result(result, file_path, file_type, file_permission=None):
+def write_damon_records(records, file_path, file_type, file_permission=None):
     '''Returns None if success, an error string otherwise'''
     if not file_type in self_write_supported_file_types:
         return 'write unsupported file type: %s' % file_type
 
     if file_type == file_type_json_compressed:
-        write_damon_record_json_compressed(result, file_path)
+        write_json_compressed(records, file_path)
     elif file_type == file_type_perf_script:
-        write_damon_perf_script(result, file_path)
+        write_perf_script(records, file_path)
     elif file_type == file_type_record:
-        write_damon_record(result, file_path, 2)
+        write_binary(records, file_path, 2)
 
     if file_permission != None:
         os.chmod(file_path, file_permission)
     return None
 
-def update_result_file(file_path, file_format, file_permission=None,
+def update_records_file(file_path, file_format, file_permission=None,
         monitoring_intervals=None):
-    result, err = parse_damon_result(file_path, monitoring_intervals)
+    records, err = parse_records_file(file_path, monitoring_intervals)
     if err:
         return err
-    return write_damon_result(result, file_path, file_format, file_permission)
+    return write_damon_records(records, file_path, file_format,
+            file_permission)
 
 # for recording
 
 record_requests = {}
 '''
 Start recording DAMON's monitoring results using perf.
 
@@ -530,15 +532,15 @@
         # perf might already finished
         pass
 
     if file_format == file_type_perf_data:
         os.chmod(file_path, file_permission)
         return
 
-    err = update_result_file(file_path, file_format, file_permission,
+    err = update_records_file(file_path, file_format, file_permission,
             monitoring_intervals)
     if err != None:
         print('converting format from perf_data to %s failed (%s)' %
                 (file_format, err))
 
 # for snapshot
 
@@ -573,34 +575,36 @@
     snapshot_start_time_ns = snapshot_end_time_ns - intervals.aggr * 1000
     snapshot = DamonSnapshot(snapshot_start_time_ns, snapshot_end_time_ns)
 
     for tried_region in tried_regions:
         snapshot.regions.append(tried_region)
     return snapshot
 
-def tried_regions_to_snapshots(monitor_scheme):
-    snapshots = {} # {kdamond idx: {ctx idx: [Snapshot, intervals]}}
+def tried_regions_to_records(monitor_scheme):
+    records = []
     for kdamond_idx, kdamond in enumerate(_damon.current_kdamonds()):
         if kdamond.state != 'on':
             continue
         # TODO: Make a cleaner way for passing the index
         for ctx_idx, ctx in enumerate(kdamond.contexts):
             for scheme in ctx.schemes:
                 if not scheme.effectively_equal(monitor_scheme, ctx.intervals):
                     continue
+
                 snapshot = tried_regions_to_snapshot(scheme.tried_regions,
                         ctx.intervals)
-                if not kdamond_idx in snapshots:
-                    snapshots[kdamond_idx] = {}
-                snapshots[kdamond_idx][ctx_idx] = [snapshot, ctx.intervals]
+
+                records.append(DamonRecord(kdamond_idx, ctx_idx, ctx.intervals,
+                    None, None))
+                records[-1].snapshots.append(snapshot)
                 break
-    return snapshots
+    return records
 
-def get_snapshots(access_pattern):
-    'return DamonSnapshots and an error'
+def get_snapshot_records(access_pattern):
+    'return DamonRecord objects each having single DamonSnapshot and an error'
     running_kdamond_idxs = _damon.running_kdamond_idxs()
     if len(running_kdamond_idxs) == 0:
         return None, 'no kdamond running'
 
     orig_kdamonds = _damon.current_kdamonds()
 
     monitor_scheme = _damon.Damos(access_pattern=access_pattern)
@@ -612,14 +616,14 @@
     if err != None:
         if installed:
             err = _damon.commit(orig_kdamonds)
             if err:
                 return None, 'monitoring scheme uninstall failed: %s' % err
         return None, 'updating schemes tried regions fail: %s' % err
 
-    snapshots = tried_regions_to_snapshots(monitor_scheme)
+    records = tried_regions_to_records(monitor_scheme)
 
     if installed:
         err = _damon.commit(orig_kdamonds)
         if err:
-            return snapshots, 'monitoring scheme uninstall failed: %s' % err
-    return snapshots, None
+            return records, 'monitoring scheme uninstall failed: %s' % err
+    return records, None
```

### Comparing `damo-1.8.5/src/damo/_damon_sysfs.py` & `damo-1.8.6/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo.py` & `damo-1.8.6/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_adjust.py` & `damo-1.8.6/src/damo/damo_adjust.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,23 +33,24 @@
     output_permission, err = _damon_result.parse_file_permission_str(
             args.output_permission)
     if err != None:
         print('wrong --output_permission (%s) (%s)' %
                 (args.output_permission, err))
         exit(1)
 
-    result, err = _damon_result.parse_damon_result(file_path)
+    records, err = _damon_result.parse_records_file(file_path)
     if err:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (file_path, err))
         exit(1)
 
     if args.aggregate_interval != None:
-        _damon_result.adjust_result(result, args.aggregate_interval, args.skip)
-    err = _damon_result.write_damon_result(result, args.output, args.output_type,
-            output_permission)
+        _damon_result.adjust_records(records, args.aggregate_interval,
+                args.skip)
+    err = _damon_result.write_damon_records(records, args.output,
+            args.output_type, output_permission)
     if err != None:
         print('writing adjusted result failed (%s)' % err)
         exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.5/src/damo/damo_convert_record_format.py` & `damo-1.8.6/src/damo/damo_convert_record_format.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,14 @@
         set_argparser(parser)
         args = parser.parse_args()
 
     if not os.path.isfile(args.record_file):
         print('record file (%s) is not exist' % args.record_file)
         exit(1)
 
-    err = _damon_result.update_result_file(args.record_file, args.format)
+    err = _damon_result.update_records_file(args.record_file, args.format)
     if err != None:
         print('converting format failed (%s)' % err)
         exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.5/src/damo/damo_features.py` & `damo-1.8.6/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_fmt_json.py` & `damo-1.8.6/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_heats.py` & `damo-1.8.6/src/damo/damo_heats.py`

 * *Files 7% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     print('# resolution: %dx%d (%s and %s for each character)' % (
         len(pixels[1]), len(pixels),
         _damo_fmt_str.format_sz(
             float(addr_range[1] - addr_range[0]) / len(pixels[1]), False),
         _damo_fmt_str.format_time_ns(
             float(time_range[1] - time_range[0]) / len(pixels), False)))
 
-def pr_heats(args, damon_result):
+def pr_heats(args, __records):
     tid = args.tid
     tres = args.resol[0]
     tmin = args.time_range[0]
     tmax = args.time_range[1]
     ares = args.resol[1]
     amin = args.address_range[0]
     amax = args.address_range[1]
@@ -146,33 +146,38 @@
 
     # Compensate the values so that those fit with the resolution
     tmax = tmin + tunit * tres
     amax = amin + aunit * ares
 
     # __pr_heats(damon_result, tid, tunit, tmin, tmax, aunit, amin, amax)
 
-    snapshots = damon_result.record_of(tid, None).snapshots
-    pixels = heat_pixels_from_snapshots(snapshots, [tmin, tmax], [amin, amax],
-            [tres, ares])
-
-    if args.heatmap == 'stdout':
-        heatmap_plot_ascii(pixels, [tmin, tmax], [amin, amax], [tres, ares],
-                args.stdout_heatmap_color)
-        return
-
-    for row in pixels:
-        for pixel in row:
-            time = pixel.time
-            addr = pixel.addr
-            if not args.abs_time:
-                time -= tmin
-            if not args.abs_addr:
-                addr -= amin
+    records = []
+    for record in __records:
+        if record.target_id == tid:
+            records.append(record)
+
+    for record in records:
+        pixels = heat_pixels_from_snapshots(record.snapshots,
+                [tmin, tmax], [amin, amax], [tres, ares])
+
+        if args.heatmap == 'stdout':
+            heatmap_plot_ascii(pixels, [tmin, tmax], [amin, amax],
+                    [tres, ares], args.stdout_heatmap_color)
+            return
+
+        for row in pixels:
+            for pixel in row:
+                time = pixel.time
+                addr = pixel.addr
+                if not args.abs_time:
+                    time -= tmin
+                if not args.abs_addr:
+                    addr -= amin
 
-            print('%s\t%s\t%s' % (time, addr, pixel.heat))
+                print('%s\t%s\t%s' % (time, addr, pixel.heat))
 
 class GuideInfo:
     tid = None
     start_time = None
     end_time = None
     lowest_addr = None
     highest_addr = None
@@ -230,18 +235,18 @@
         for r2 in regions2:
             if is_overlap(r1, r2):
                 r1 = overlap_region_of(r1, r2)
         if r1:
             overlap_regions.append(r1)
     return overlap_regions
 
-def get_guide_info(damon_result):
+def get_guide_info(records):
     "return the set of guide information for the moitoring result"
     guides = {}
-    for record in damon_result.records:
+    for record in records:
         for snapshot in record.snapshots:
             monitor_time = snapshot.end_time
             tid = record.target_id
             if not tid in guides:
                 guides[tid] = GuideInfo(tid, monitor_time)
             guide = guides[tid]
             guide.end_time = monitor_time
@@ -268,25 +273,25 @@
                 guide.gaps = gaps
             else:
                 guide.gaps = overlapping_regions(guide.gaps, gaps)
 
     return sorted(list(guides.values()), key=lambda x: x.total_space(),
                     reverse=True)
 
-def pr_guide(damon_result):
-    for guide in get_guide_info(damon_result):
+def pr_guide(records):
+    for guide in get_guide_info(records):
         print(guide)
 
 def region_sort_key(region):
     return region[1] - region[0]
 
-def set_missed_args(args, damon_result):
+def set_missed_args(args, records):
     if args.tid and args.time_range and args.address_range:
         return
-    guides = get_guide_info(damon_result)
+    guides = get_guide_info(records)
     guide = guides[0]
     if not args.tid:
         args.tid = guide.tid
     for g in guides:
         if g.tid == args.tid:
             guide = g
             break
@@ -356,35 +361,35 @@
 
 def main(args=None):
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
-    damon_result, err = _damon_result.parse_damon_result(args.input)
+    records, err = _damon_result.parse_records_file(args.input)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (args.input, err))
         exit(1)
 
     # Use 80x40 resolution as default for ascii plot
     if args.heatmap == 'stdout' and args.resol == [500, 500]:
         args.resol = [40, 80]
 
     if args.guide:
-        pr_guide(damon_result)
+        pr_guide(records)
     else:
-        set_missed_args(args, damon_result)
+        set_missed_args(args, records)
         orig_stdout = sys.stdout
         if args.heatmap and args.heatmap != 'stdout':
             tmp_path = tempfile.mkstemp()[1]
             tmp_file = open(tmp_path, 'w')
             sys.stdout = tmp_file
 
-        pr_heats(args, damon_result)
+        pr_heats(args, records)
 
         if args.heatmap and args.heatmap != 'stdout':
             sys.stdout = orig_stdout
             tmp_file.flush()
             tmp_file.close()
             plot_heatmap(tmp_path, args.heatmap, args)
```

### Comparing `damo-1.8.5/src/damo/damo_lru_sort.py` & `damo-1.8.6/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_monitor.py` & `damo-1.8.6/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_nr_regions.py` & `damo-1.8.6/src/damo/damo_nr_regions.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,29 +31,29 @@
     file_path = args.input
     if args.range:
         percentiles = range(args.range[0], args.range[1], args.range[2])
     nr_regions_sort = True
     if args.sortby == 'time':
         nr_regions_sort = False
 
-    result, err = _damon_result.parse_damon_result(file_path)
+    records, err = _damon_result.parse_records_file(file_path)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (file_path, err))
         exit(1)
 
     orig_stdout = sys.stdout
     if args.plot:
         tmp_path = tempfile.mkstemp()[1]
         tmp_file = open(tmp_path, 'w')
         sys.stdout = tmp_file
 
     print('# <percentile> <# regions>')
 
-    for record in result.records:
+    for record in records:
         nr_regions_dist = []
         # Skip firs 20 regions as those would not adaptively adjusted
         for snapshot in record.snapshots[20:]:
             nr_regions_dist.append(len(snapshot.regions))
         if nr_regions_sort:
             nr_regions_dist.sort(reverse=False)
```

### Comparing `damo-1.8.5/src/damo/damo_reclaim.py` & `damo-1.8.6/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_record.py` & `damo-1.8.6/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_record_info.py` & `damo-1.8.6/src/damo/damo_record_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,18 +69,18 @@
         for r2 in regions2:
             if is_overlap(r1, r2):
                 r1 = overlap_region_of(r1, r2)
         if r1:
             overlap_regions.append(r1)
     return overlap_regions
 
-def get_guide_info(damon_result):
+def get_guide_info(records):
     "return the set of guide information for the moitoring result"
     guides = {}
-    for record in damon_result.records:
+    for record in records:
         for snapshot in record.snapshots:
             monitor_time = snapshot.end_time
             tid = record.target_id
             if not tid in guides:
                 guides[tid] = GuideInfo(tid, monitor_time)
             guide = guides[tid]
             guide.end_time = monitor_time
@@ -107,16 +107,16 @@
                 guide.gaps = gaps
             else:
                 guide.gaps = overlapping_regions(guide.gaps, gaps)
 
     return sorted(list(guides.values()), key=lambda x: x.total_space(),
                     reverse=True)
 
-def pr_guide(damon_result):
-    for guide in get_guide_info(damon_result):
+def pr_guide(records):
+    for guide in get_guide_info(records):
         print(guide)
 
 def region_sort_key(region):
     return region[1] - region[0]
 
 def set_argparser(parser):
     parser.add_argument('--input', '-i', type=str, metavar='<file>',
@@ -124,16 +124,16 @@
 
 def main(args=None):
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
-    damon_result, err = _damon_result.parse_damon_result(args.input)
+    records, err = _damon_result.parse_records_file(args.input)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (args.input, err))
         exit(1)
-    pr_guide(damon_result)
+    pr_guide(records)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.5/src/damo/damo_report.py` & `damo-1.8.6/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_report_raw.py` & `damo-1.8.6/src/damo/damo_report_raw.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,52 +4,21 @@
 import json
 import os
 import sys
 
 import _damon_result
 import _damo_fmt_str
 
-def set_argparser(parser):
-    parser.add_argument('--input', '-i', type=str, metavar='<file>',
-            default='damon.data', help='input file name')
-    parser.add_argument('--duration', type=float, metavar='<seconds>', nargs=2,
-            help='start and end time offset for record to parse')
-    parser.add_argument('--raw_number', action='store_true',
-            help='use machine-friendly raw numbers')
-    parser.add_argument('--json', action='store_true',
-            help='print in json format')
-
-def main(args=None):
-    if not args:
-        parser = argparse.ArgumentParser()
-        set_argparser(parser)
-        args = parser.parse_args()
-
-    file_path = args.input
-
-    if not os.path.isfile(file_path):
-        print('input file (%s) is not exist' % file_path)
-        exit(1)
-
-    result, err = _damon_result.parse_damon_result(file_path)
-    if err:
-        print('parsing damon result file (%s) failed (%s)' %
-                (file_path, err))
-        exit(1)
-
-    if not result:
-        print('no monitoring result in the file')
-        exit(1)
-
+def pr_records(args, records):
     if args.json:
         print(json.dumps([r.to_kvpairs(args.raw_number)
-            for r in result.records], indent=4))
+            for r in records], indent=4))
         exit(0)
 
-    for record in result.records:
+    for record in records:
         snapshots = record.snapshots
         if len(snapshots) == 0:
             continue
 
         base_time = snapshots[0].start_time
         print('base_time_absolute: %s\n' %
                 _damo_fmt_str.format_time_ns(base_time, args.raw_number))
@@ -80,9 +49,48 @@
                         (r.start, r.end,
                             _damo_fmt_str.format_sz(r.end - r.start,
                                 args.raw_number), r.nr_accesses.samples,
                                 r.age.aggr_intervals
                                 if r.age.aggr_intervals != None else -1))
             print('')
 
+def set_argparser(parser):
+    parser.add_argument('--input', '-i', type=str, metavar='<file>',
+            default='damon.data', help='input file name')
+    parser.add_argument('--duration', type=float, metavar='<seconds>', nargs=2,
+            help='start and end time offset for record to parse')
+    parser.add_argument('--raw_number', action='store_true',
+            help='use machine-friendly raw numbers')
+    parser.add_argument('--json', action='store_true',
+            help='print in json format')
+
+def main(args=None):
+    if not args:
+        parser = argparse.ArgumentParser()
+        set_argparser(parser)
+        args = parser.parse_args()
+
+    file_path = args.input
+
+    if not os.path.isfile(file_path):
+        print('input file (%s) is not exist' % file_path)
+        exit(1)
+
+    records, err = _damon_result.parse_records_file(file_path)
+    if err:
+        print('parsing damon result file (%s) failed (%s)' %
+                (file_path, err))
+        exit(1)
+
+    if len(records) == 0:
+        print('no monitoring result in the file')
+        exit(1)
+
+    try:
+        pr_records(args, records)
+    except BrokenPipeError as e:
+        # maybe user piped to 'less' like pager and quit from it
+        pass
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.5/src/damo/damo_schemes.py` & `damo-1.8.6/src/damo/damo_schemes.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 import signal
 
 import _damon
 import _damon_args
 
 def cleanup_exit(exit_code):
     # ignore returning error, as kdamonds may already finished
-    err = _damon.turn_damon_off(kdamonds_idxs)
-    if err:
-        print('failed to turn damon off (%s)' % err)
+    _damon.turn_damon_off(kdamonds_idxs)
     err = _damon.stage_kdamonds(orig_kdamonds)
     if err:
         print('failed restoring previous kdamonds setup (%s)' % err)
     exit(exit_code)
 
 def sighandler(signum, frame):
     print('\nsignal %s received' % signum)
```

### Comparing `damo-1.8.5/src/damo/damo_show.py` & `damo-1.8.6/src/damo/damo_show.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_show_accesses.py` & `damo-1.8.6/src/damo/damo_show_accesses.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_show_snapshot.py` & `damo-1.8.6/src/damo/damo_show_snapshot.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_show_status.py` & `damo-1.8.6/src/damo/damo_show_status.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_start.py` & `damo-1.8.6/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_stat.py` & `damo-1.8.6/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_stat_kdamonds.py` & `damo-1.8.6/src/damo/damo_stat_kdamonds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_stat_regions.py` & `damo-1.8.6/src/damo/damo_stat_regions.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,25 +28,24 @@
         else:
             total_sz += (region.end - region.start)
     if size_only:
         print('%s' % _damo_fmt_str.format_sz(total_sz, raw_nr))
 
 def update_pr_schemes_tried_regions(access_pattern, size_only, sortby,
         prio_weights, raw_nr):
-    snapshots, err = _damon_result.get_snapshots(access_pattern)
-    if snapshots == None:
+    records, err = _damon_result.get_snapshot_records(access_pattern)
+    if err != None:
         print(err)
+    if records == None:
         return
 
-    for kdamond_idx, ctx_snapshot in snapshots.items():
-        for ctx_idx, snapshot_intervals in ctx_snapshot.items():
-            snapshot, intervals = snapshot_intervals
-            print('kdamond %s ctx %s' % (kdamond_idx, ctx_idx))
-            __pr_schemes_tried_regions(snapshot.regions, intervals, size_only,
-                    sortby, prio_weights, raw_nr)
+    for record in records:
+        print('kdamond %s ctx %s' % (record.kdamond_idx, record.context_idx))
+        __pr_schemes_tried_regions(record.snapshots[0].regions,
+                record.intervals, size_only, sortby, prio_weights, raw_nr)
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
     parser.add_argument('--sz_region', metavar=('<min>', '<max>'), nargs=2,
             default=['min', 'max'],
             help='min/max size of regions (bytes)')
     parser.add_argument('--access_rate', metavar=('<min>', '<max>'), nargs=2,
```

### Comparing `damo-1.8.5/src/damo/damo_stat_schemes.py` & `damo-1.8.6/src/damo/damo_stat_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_stop.py` & `damo-1.8.6/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_translate_damos.py` & `damo-1.8.6/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_tune.py` & `damo-1.8.6/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.5/src/damo/damo_validate.py` & `damo-1.8.6/src/damo/damo_validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,24 +64,24 @@
     if args.regions_boundary:
         for boundary in args.regions_boundary:
             parsed_boundary = [int(x) for x in boundary.split('-')]
             if not len(parsed_boundary) == 2:
                 print('wrong boundary input %s' % boundary)
             regions_boundary.append(parsed_boundary)
 
-    result, err = _damon_result.parse_damon_result(args.input)
+    records, err = _damon_result.parse_records_file(args.input)
     if err != None:
         print('parsing failed (%s)' % err)
         exit(1)
 
-    if len(result.records) == 0:
+    if len(records) == 0:
         print('target snapshots is zero')
         exit(1)
 
-    for record in result.records:
+    for record in records:
         target = record.target_id
         nr_snapshots = len(record.snapshots)
         nr_allowed_errors = nr_snapshots * args.allow_error / 100.0
         nr_aggr_interval_errors = 0
         nr_nr_regions_erros = 0
         for snapshot in record.snapshots:
             aggr_interval_us = (snapshot.end_time - snapshot.start_time) / 1000
```

### Comparing `damo-1.8.5/src/damo/damo_wss.py` & `damo-1.8.6/src/damo/damo_wss.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import sys
 import tempfile
 
 import _damo_dist
 import _damon_result
 import _damo_fmt_str
 
-def get_wss_dists(result, acc_thres, sz_thres, do_sort):
+def get_wss_dists(records, acc_thres, sz_thres, do_sort):
     wss_dists = {}
-    for record in result.records:
+    for record in records:
         wss_dist = []
         for snapshot in record.snapshots:
             wss = 0
             for r in snapshot.regions:
                 # Ignore regions not fulfill working set conditions
                 if r.nr_accesses.samples < acc_thres:
                     continue
@@ -110,22 +110,22 @@
     file_path = args.input
     percentiles = range(args.range[0], args.range[1], args.range[2])
     wss_sort = True
     if args.sortby == 'time':
         wss_sort = False
     raw_number = args.raw_number
 
-    result, err = _damon_result.parse_damon_result(file_path)
+    records, err = _damon_result.parse_records_file(file_path)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (file_path, err))
         exit(1)
 
-    _damon_result.adjust_result(result, args.work_time, args.exclude_samples)
-    wss_dists = get_wss_dists(result, args.acc_thres, args.sz_thres, wss_sort)
+    _damon_result.adjust_records(records, args.work_time, args.exclude_samples)
+    wss_dists = get_wss_dists(records, args.acc_thres, args.sz_thres, wss_sort)
 
     if args.plot:
         orig_stdout = sys.stdout
         tmp_path = tempfile.mkstemp()[1]
         tmp_file = open(tmp_path, 'w')
         sys.stdout = tmp_file
         raw_number = True
```

### Comparing `damo-1.8.5/src/damo.egg-info/PKG-INFO` & `damo-1.8.6/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.5
+Version: 1.8.6
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +87,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.6/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.5/src/damo.egg-info/SOURCES.txt` & `damo-1.8.6/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

