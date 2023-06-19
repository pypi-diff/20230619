# Comparing `tmp/je_api_testka_dev-0.0.95.tar.gz` & `tmp/je_api_testka_dev-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka_dev-0.0.95.tar", last modified: Mon Jun 19 05:31:17 2023, max compression
+gzip compressed data, was "je_api_testka_dev-0.0.96.tar", last modified: Mon Jun 19 05:44:21 2023, max compression
```

## Comparing `je_api_testka_dev-0.0.95.tar` & `je_api_testka_dev-0.0.96.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.622179 je_api_testka_dev-0.0.95/
--rw-rw-rw-   0        0        0     3074 2023-06-19 05:31:17.620180 je_api_testka_dev-0.0.95/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.95/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.368076 je_api_testka_dev-0.0.95/je_api_testka/
--rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.95/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.95/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.380071 je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     6242 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     3116 2023-06-13 07:15:23.000000 je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.383069 je_api_testka_dev-0.0.95/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.389591 je_api_testka_dev-0.0.95/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.398620 je_api_testka_dev-0.0.95/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     3502 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.409589 je_api_testka_dev-0.0.95/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.417141 je_api_testka_dev-0.0.95/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     5973 2023-06-19 03:34:10.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.424142 je_api_testka_dev-0.0.95/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      734 2023-06-19 03:15:40.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.443302 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     9239 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     4289 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     2082 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.449302 je_api_testka_dev-0.0.95/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1912 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.452302 je_api_testka_dev-0.0.95/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.459310 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-06-19 03:31:45.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.468306 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.476554 je_api_testka_dev-0.0.95/je_api_testka/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      563 2023-06-13 06:12:30.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.490986 je_api_testka_dev-0.0.95/je_api_testka/utils/mock_server/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/mock_server/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-06-19 03:36:57.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/mock_server/flask_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.503077 je_api_testka_dev-0.0.95/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3593 2023-06-19 03:43:06.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.513094 je_api_testka_dev-0.0.95/je_api_testka/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/__init__.py
--rw-rw-rw-   0        0        0     3286 2023-06-19 03:59:54.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.525095 je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.540087 je_api_testka_dev-0.0.95/je_api_testka/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0    10629 2023-06-19 05:30:20.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.552089 je_api_testka_dev-0.0.95/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2753 2023-06-19 03:55:58.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.559089 je_api_testka_dev-0.0.95/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.562088 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.568086 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.576665 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.617261 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0     3074 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2636 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1172 2023-06-19 05:30:49.000000 je_api_testka_dev-0.0.95/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 05:31:17.623176 je_api_testka_dev-0.0.95/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.137398 je_api_testka_dev-0.0.96/
+-rw-rw-rw-   0        0        0     3074 2023-06-19 05:44:21.136399 je_api_testka_dev-0.0.96/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.96/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.903618 je_api_testka_dev-0.0.96/je_api_testka/
+-rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.96/je_api_testka/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.96/je_api_testka/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.918300 je_api_testka_dev-0.0.96/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     5676 2023-06-19 05:42:57.000000 je_api_testka_dev-0.0.96/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     3116 2023-06-13 07:15:23.000000 je_api_testka_dev-0.0.96/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.921438 je_api_testka_dev-0.0.96/je_api_testka/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.928430 je_api_testka_dev-0.0.96/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/assert_result/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/assert_result/result_check.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.934430 je_api_testka_dev-0.0.96/je_api_testka/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     3502 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.943427 je_api_testka_dev-0.0.96/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.951438 je_api_testka_dev-0.0.96/je_api_testka/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     5973 2023-06-19 03:34:10.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.960293 je_api_testka_dev-0.0.96/je_api_testka/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-06-19 03:15:40.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.975378 je_api_testka_dev-0.0.96/je_api_testka/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     9239 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/generate_report/html_report_generate.py
+-rw-rw-rw-   0        0        0     4289 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/generate_report/json_report.py
+-rw-rw-rw-   0        0        0     2082 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/generate_report/xml_report.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.992249 je_api_testka_dev-0.0.96/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-06-19 05:44:00.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:20.995857 je_api_testka_dev-0.0.96/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.002993 je_api_testka_dev-0.0.96/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-06-19 03:31:45.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.010941 je_api_testka_dev-0.0.96/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.017466 je_api_testka_dev-0.0.96/je_api_testka/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-06-13 06:12:30.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.024119 je_api_testka_dev-0.0.96/je_api_testka/utils/mock_server/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/mock_server/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-06-19 03:36:57.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/mock_server/flask_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.033144 je_api_testka_dev-0.0.96/je_api_testka/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3593 2023-06-19 03:43:06.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.040143 je_api_testka_dev-0.0.96/je_api_testka/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     3286 2023-06-19 03:59:54.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.055141 je_api_testka_dev-0.0.96/je_api_testka/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.062144 je_api_testka_dev-0.0.96/je_api_testka/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0    10629 2023-06-19 05:30:20.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.069146 je_api_testka_dev-0.0.96/je_api_testka/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2753 2023-06-19 03:55:58.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/socket_server/api_testka_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.075524 je_api_testka_dev-0.0.96/je_api_testka/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.079488 je_api_testka_dev-0.0.96/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.087484 je_api_testka_dev-0.0.96/je_api_testka/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.095758 je_api_testka_dev-0.0.96/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.96/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:44:21.133399 je_api_testka_dev-0.0.96/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0     3074 2023-06-19 05:44:20.000000 je_api_testka_dev-0.0.96/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2636 2023-06-19 05:44:20.000000 je_api_testka_dev-0.0.96/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 05:44:20.000000 je_api_testka_dev-0.0.96/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-19 05:44:20.000000 je_api_testka_dev-0.0.96/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 05:44:20.000000 je_api_testka_dev-0.0.96/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1172 2023-06-19 05:44:00.000000 je_api_testka_dev-0.0.96/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 05:44:21.138401 je_api_testka_dev-0.0.96/setup.cfg
```

### Comparing `je_api_testka_dev-0.0.95/PKG-INFO` & `je_api_testka_dev-0.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_api_testka_dev
-Version: 0.0.95
+Version: 0.0.96
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.95/README.md` & `je_api_testka_dev-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/__init__.py` & `je_api_testka_dev-0.0.96/je_api_testka/__init__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/__main__.py` & `je_api_testka_dev-0.0.96/je_api_testka/__main__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/request_method.py` & `je_api_testka_dev-0.0.96/je_api_testka/requests_wrapper/request_method.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,29 +37,15 @@
     "session_options": session_error_message,
 
 }
 
 
 def get_response(response: requests.Response,
                  start_time: [str, float, int],
-                 end_time: [str, float, int]) \
-        -> Dict[
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str
-        ]:
+                 end_time: [str, float, int]) -> Dict[str, str]:
     """
     use requests response to create data dict
     :param response: requests response
     :param start_time: test start time
     :param end_time: test end time
     :return: data dict include [status_code, text, content, headers, history, encoding, cookies,
     elapsed, request_time_sec, request_method, request_url, request_body, start_time, end_time]
@@ -70,28 +56,15 @@
         raise APITesterGetDataException(get_data_error_message)
 
 
 def test_api_method(http_method: str, test_url: str,
                     soap: bool = False, record_request_info: bool = True,
                     clean_record: bool = False, result_check_dict: dict = None
                     , verify: bool = False, timeout: int = 5, allow_redirects: bool = False,
-                    **kwargs) \
-        -> (requests.Response, Dict[
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str,
-            str, str]):
+                    **kwargs) -> (requests.Response, Dict[str, str]):
     """
     set requests http_method url headers and record response and record report
     :param http_method:
     :param test_url:
     :param soap:
     :param record_request_info:
     :param clean_record:
```

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/requests_http_method_wrapper.py` & `je_api_testka_dev-0.0.96/je_api_testka/requests_wrapper/requests_http_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/assert_result/result_check.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/assert_result/result_check.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/callback/callback_function_executor.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/exception/exception_tags.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/exception/exceptions.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/executor/action_executor.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/executor/action_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/file_process/get_dir_file_list.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/html_report_generate.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/generate_report/html_report_generate.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/json_report.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/generate_report/json_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/xml_report.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/generate_report/xml_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_format/json_process.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/logging/loggin_instance.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/mock_server/flask_mock_server.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/mock_server/flask_mock_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/package_manager/package_manager_class.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/project/create_project_structure.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/project/create_project_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/template_executor.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/template_keyword.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/project/template/template_keyword.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/scheduler/extend_apscheduler.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/scheduler/extend_apscheduler.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/socket_server/api_testka_socket_server.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/socket_server/api_testka_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.96/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/PKG-INFO` & `je_api_testka_dev-0.0.96/je_api_testka_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-api-testka-dev
-Version: 0.0.95
+Version: 0.0.96
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/SOURCES.txt` & `je_api_testka_dev-0.0.96/je_api_testka_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.95/pyproject.toml` & `je_api_testka_dev-0.0.96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_api_testka_dev"
-version = "0.0.95"
+version = "0.0.96"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Requests Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

