# Comparing `tmp/je_api_testka_dev-0.0.94.tar.gz` & `tmp/je_api_testka_dev-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka_dev-0.0.94.tar", last modified: Tue Jun 13 08:04:36 2023, max compression
+gzip compressed data, was "je_api_testka_dev-0.0.95.tar", last modified: Mon Jun 19 05:31:17 2023, max compression
```

## Comparing `je_api_testka_dev-0.0.94.tar` & `je_api_testka_dev-0.0.95.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.802329 je_api_testka_dev-0.0.94/
--rw-rw-rw-   0        0        0     3074 2023-06-13 08:04:36.800084 je_api_testka_dev-0.0.94/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.94/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.480765 je_api_testka_dev-0.0.94/je_api_testka/
--rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.94/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.94/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.505652 je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     5734 2023-06-13 07:24:00.000000 je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     3116 2023-06-13 07:15:23.000000 je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.512529 je_api_testka_dev-0.0.94/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.523603 je_api_testka_dev-0.0.94/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.531758 je_api_testka_dev-0.0.94/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     3497 2023-05-29 03:22:33.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.542815 je_api_testka_dev-0.0.94/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.551925 je_api_testka_dev-0.0.94/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     5993 2023-06-13 07:58:24.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.561495 je_api_testka_dev-0.0.94/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.594701 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     9231 2023-06-13 07:24:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     4291 2023-06-13 07:30:18.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     2092 2023-06-13 07:34:49.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.607234 je_api_testka_dev-0.0.94/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.610774 je_api_testka_dev-0.0.94/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.619739 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.636553 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.643569 je_api_testka_dev-0.0.94/je_api_testka/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      563 2023-06-13 06:12:30.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.654741 je_api_testka_dev-0.0.94/je_api_testka/utils/mock_server/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/mock_server/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-06-13 08:03:10.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/mock_server/flask_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.670347 je_api_testka_dev-0.0.94/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3589 2023-06-13 08:01:42.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.684243 je_api_testka_dev-0.0.94/je_api_testka/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/__init__.py
--rw-rw-rw-   0        0        0     2982 2023-04-18 02:25:34.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.698253 je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.710058 je_api_testka_dev-0.0.94/je_api_testka/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0     6250 2023-05-31 06:04:47.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.722720 je_api_testka_dev-0.0.94/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2490 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.729638 je_api_testka_dev-0.0.94/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.732636 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.743568 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.754361 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.94/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:36.796565 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0     3074 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2636 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 08:04:36.000000 je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1170 2023-06-13 08:04:12.000000 je_api_testka_dev-0.0.94/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 08:04:36.803342 je_api_testka_dev-0.0.94/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.622179 je_api_testka_dev-0.0.95/
+-rw-rw-rw-   0        0        0     3074 2023-06-19 05:31:17.620180 je_api_testka_dev-0.0.95/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.95/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.368076 je_api_testka_dev-0.0.95/je_api_testka/
+-rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.95/je_api_testka/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.95/je_api_testka/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.380071 je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     6242 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     3116 2023-06-13 07:15:23.000000 je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.383069 je_api_testka_dev-0.0.95/je_api_testka/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.389591 je_api_testka_dev-0.0.95/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/assert_result/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/assert_result/result_check.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.398620 je_api_testka_dev-0.0.95/je_api_testka/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     3502 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.409589 je_api_testka_dev-0.0.95/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.417141 je_api_testka_dev-0.0.95/je_api_testka/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     5973 2023-06-19 03:34:10.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.424142 je_api_testka_dev-0.0.95/je_api_testka/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-06-19 03:15:40.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.443302 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     9239 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/html_report_generate.py
+-rw-rw-rw-   0        0        0     4289 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/json_report.py
+-rw-rw-rw-   0        0        0     2082 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/xml_report.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.449302 je_api_testka_dev-0.0.95/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1912 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.452302 je_api_testka_dev-0.0.95/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.459310 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-06-19 03:31:45.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.468306 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.476554 je_api_testka_dev-0.0.95/je_api_testka/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-06-13 06:12:30.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.490986 je_api_testka_dev-0.0.95/je_api_testka/utils/mock_server/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/mock_server/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-06-19 03:36:57.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/mock_server/flask_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.503077 je_api_testka_dev-0.0.95/je_api_testka/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3593 2023-06-19 03:43:06.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.513094 je_api_testka_dev-0.0.95/je_api_testka/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     3286 2023-06-19 03:59:54.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.525095 je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.540087 je_api_testka_dev-0.0.95/je_api_testka/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0    10629 2023-06-19 05:30:20.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.552089 je_api_testka_dev-0.0.95/je_api_testka/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2753 2023-06-19 03:55:58.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/socket_server/api_testka_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.559089 je_api_testka_dev-0.0.95/je_api_testka/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.562088 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.568086 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.576665 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.95/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:31:17.617261 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0     3074 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2636 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 05:31:17.000000 je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1172 2023-06-19 05:30:49.000000 je_api_testka_dev-0.0.95/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 05:31:17.623176 je_api_testka_dev-0.0.95/setup.cfg
```

### Comparing `je_api_testka_dev-0.0.94/PKG-INFO` & `je_api_testka_dev-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_api_testka_dev
-Version: 0.0.94
+Version: 0.0.95
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.94/README.md` & `je_api_testka_dev-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/__init__.py` & `je_api_testka_dev-0.0.95/je_api_testka/__init__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/__main__.py` & `je_api_testka_dev-0.0.95/je_api_testka/__main__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/request_method.py` & `je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/request_method.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import sys
 from datetime import datetime
+from typing import Dict
 
 import requests
 from requests.structures import CaseInsensitiveDict
 
 from je_api_testka.requests_wrapper.requests_http_method_wrapper import api_tester_method
 from je_api_testka.utils.assert_result.result_check import check_result
 from je_api_testka.utils.exception.exception_tags import delete_error_message
@@ -11,15 +11,14 @@
 from je_api_testka.utils.exception.exception_tags import get_error_message
 from je_api_testka.utils.exception.exception_tags import head_error_message
 from je_api_testka.utils.exception.exception_tags import options_error_message
 from je_api_testka.utils.exception.exception_tags import patch_error_message
 from je_api_testka.utils.exception.exception_tags import post_error_message
 from je_api_testka.utils.exception.exception_tags import put_error_message
 from je_api_testka.utils.exception.exception_tags import session_error_message
-from je_api_testka.utils.exception.exceptions import APITesterExecuteException
 from je_api_testka.utils.exception.exceptions import APITesterGetDataException
 from je_api_testka.utils.get_data_strcture.get_api_data import get_api_response_data
 from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.test_record.test_record_class import test_record_instance
 
 exception_message_dict = {
     "get": get_error_message,
@@ -38,15 +37,29 @@
     "session_options": session_error_message,
 
 }
 
 
 def get_response(response: requests.Response,
                  start_time: [str, float, int],
-                 end_time: [str, float, int]) -> dict:
+                 end_time: [str, float, int]) \
+        -> Dict[
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str
+        ]:
     """
     use requests response to create data dict
     :param response: requests response
     :param start_time: test start time
     :param end_time: test end time
     :return: data dict include [status_code, text, content, headers, history, encoding, cookies,
     elapsed, request_time_sec, request_method, request_url, request_body, start_time, end_time]
@@ -58,15 +71,27 @@
 
 
 def test_api_method(http_method: str, test_url: str,
                     soap: bool = False, record_request_info: bool = True,
                     clean_record: bool = False, result_check_dict: dict = None
                     , verify: bool = False, timeout: int = 5, allow_redirects: bool = False,
                     **kwargs) \
-        -> (requests.Response, dict):
+        -> (requests.Response, Dict[
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str,
+            str, str]):
     """
     set requests http_method url headers and record response and record report
     :param http_method:
     :param test_url:
     :param soap:
     :param record_request_info:
     :param clean_record:
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/requests_wrapper/requests_http_method_wrapper.py` & `je_api_testka_dev-0.0.95/je_api_testka/requests_wrapper/requests_http_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/assert_result/result_check.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/assert_result/result_check.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/callback/callback_function_executor.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/callback/callback_function_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import typing
 from sys import stderr
+from typing import Any, Callable
 
 from je_api_testka.requests_wrapper.request_method import test_api_method
 from je_api_testka.utils.exception.exception_tags import get_bad_trigger_function, get_bad_trigger_method
 from je_api_testka.utils.exception.exceptions import CallbackExecutorException
 from je_api_testka.utils.generate_report.html_report_generate import generate_html
 from je_api_testka.utils.generate_report.html_report_generate import generate_html_report
 from je_api_testka.utils.generate_report.json_report import generate_json
@@ -32,19 +32,19 @@
             # Package manager
             "add_package_to_callback_executor": package_manager.add_package_to_callback_executor,
         }
 
     def callback_function(
             self,
             trigger_function_name: str,
-            callback_function: typing.Callable,
+            callback_function: Callable,
             callback_function_param: [dict, None] = None,
             callback_param_method: [str, None] = "kwargs",
             **kwargs
-    ) -> typing.Any:
+    ) -> Any:
         """
         :param trigger_function_name: what function we want to trigger only accept function in event_dict
         :param callback_function: what function we want to callback
         :param callback_function_param: callback function's param only accept dict
         :param callback_param_method: what type param will use on callback function only accept kwargs and args
         :param kwargs: trigger_function's param
         :return:
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/exception/exception_tags.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/exception/exceptions.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/executor/action_executor.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/executor/action_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import builtins
-import sys
 import types
-import typing
 from inspect import getmembers, isbuiltin
+from typing import Dict, Callable, Any, List
 
 from je_api_testka.requests_wrapper.request_method import test_api_method
 from je_api_testka.utils.exception.exception_tags import add_command_exception_tag
 from je_api_testka.utils.exception.exception_tags import executor_data_error, executor_list_error
 from je_api_testka.utils.exception.exceptions import APITesterExecuteException, APIAddCommandException
 from je_api_testka.utils.generate_report.html_report_generate import generate_html
 from je_api_testka.utils.generate_report.html_report_generate import generate_html_report
@@ -42,29 +41,29 @@
             "flask_mock_server_add_router": flask_mock_server_instance.add_router,
             "start_flask_mock_server": flask_mock_server_instance.start_mock_server,
         }
         # get all builtin function and add to event dict
         for function in getmembers(builtins, isbuiltin):
             self.event_dict.update({str(function[0]): function[1]})
 
-    def _execute_event(self, action: list) -> typing.Any:
+    def _execute_event(self, action: list) -> Any:
         """
         :param action: execute action
         :return: what event return
         """
-        event: typing.Callable = self.event_dict.get(action[0])
+        event: Callable = self.event_dict.get(action[0])
         if len(action) == 2:
             if isinstance(action[1], dict):
                 return event(**action[1])
             else:
                 return event(*action[1])
         else:
             raise APITesterExecuteException(executor_data_error + " " + str(action))
 
-    def execute_action(self, action_list: [list, dict]) -> dict:
+    def execute_action(self, action_list: [list, dict]) -> Dict[str, str]:
         """
         :param action_list: like this structure
         [
             ["method on event_dict", {"param": params}],
             ["method on event_dict", {"param": params}]
         ]
         for loop and use execute_event function to execute
@@ -96,15 +95,15 @@
                 execute_record = "execute: " + str(action)
                 execute_record_dict.update({execute_record: repr(error)})
         for key, value in execute_record_dict.items():
             print(key)
             print(value)
         return execute_record_dict
 
-    def execute_files(self, execute_files_list: list) -> typing.List[typing.Any]:
+    def execute_files(self, execute_files_list: list) -> List[Any]:
         """
         :param execute_files_list: list include execute files path
         :return: every execute detail as list
         """
         apitestka_logger.info(f"execute_files, execute_files_list: {execute_files_list}")
         execute_detail_list: list = list()
         for file in execute_files_list:
@@ -120,13 +119,13 @@
     for command_name, command in command_dict.items():
         if isinstance(command, (types.MethodType, types.FunctionType)):
             executor.event_dict.update({command_name: command})
         else:
             raise APIAddCommandException(add_command_exception_tag)
 
 
-def execute_action(action_list: list) -> typing.Any:
+def execute_action(action_list: list) -> Any:
     return executor.execute_action(action_list)
 
 
-def execute_files(execute_files_list: list) -> typing.List[typing.Any]:
+def execute_files(execute_files_list: list) -> List[Any]:
     return executor.execute_files(execute_files_list)
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/file_process/get_dir_file_list.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/file_process/get_dir_file_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from os import getcwd
 from os import walk
 from os.path import abspath
 from os.path import join
+from typing import List
 
 
-def get_dir_files_as_list(dir_path: str = getcwd(), default_search_file_extension: str = ".json") -> list:
+def get_dir_files_as_list(dir_path: str = getcwd(), default_search_file_extension: str = ".json") -> List:
     """
     get dir file when end with default_search_file_extension
     :param dir_path: which dir we want to walk and get file list
     :param default_search_file_extension: which extension we want to search
     :return: [] if nothing searched or [file1, file2.... files] file was searched
     """
     return [
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/html_report_generate.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/html_report_generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
-import typing
 from threading import Lock
+from typing import List, Tuple
 
 from je_api_testka.utils.exception.exception_tags import html_generate_no_data_tag
 from je_api_testka.utils.exception.exceptions import APIHTMLException
 from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.test_record.test_record_class import test_record_instance
 
 lock = Lock()
@@ -195,15 +195,15 @@
     </tr>
     </tbody>
 </table>
 <br>
     """.strip()
 
 
-def generate_html() -> typing.Tuple[list, list]:
+def generate_html() -> Tuple[List, List]:
     """
     :return: test success_list & test failure_list
     """
     apitestka_logger.info(f"generate_html")
     if len(test_record_instance.test_record_list) == 0 and len(test_record_instance.error_record_list) == 0:
         raise APIHTMLException(html_generate_no_data_tag)
     else:
@@ -266,8 +266,7 @@
             file_to_write.writelines(
                 _html_string_bottom
             )
     except Exception as error:
         print(repr(error), file=sys.stderr)
     finally:
         lock.release()
-
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/json_report.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/json_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import json
-import sys
-import typing
 from threading import Lock
+from typing import Tuple, Dict
 
-from je_api_testka.utils.logging.loggin_instance import apitestka_logger
-from je_api_testka.utils.test_record.test_record_class import test_record_instance
 from je_api_testka.utils.exception.exception_tags import cant_save_json_report_record_us_null
 from je_api_testka.utils.exception.exceptions import APIJsonReportException
+from je_api_testka.utils.logging.loggin_instance import apitestka_logger
+from je_api_testka.utils.test_record.test_record_class import test_record_instance
 
 
-def generate_json() -> typing.Tuple[dict, dict]:
+def generate_json() -> Tuple[Dict, Dict]:
     """
     :return: test success_dict test failure_dict
     """
     apitestka_logger.info("generate_json")
     if len(test_record_instance.test_record_list) == 0 and len(test_record_instance.error_record_list) == 0:
         raise APIJsonReportException(cant_save_json_report_record_us_null)
     else:
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/generate_report/xml_report.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/generate_report/xml_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import sys
-import typing
 from threading import Lock
+from typing import Tuple
 from xml.dom.minidom import parseString
 
 from je_api_testka.utils.generate_report.json_report import generate_json
 from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.xml.change_xml_structure.change_xml_structure import dict_to_elements_tree
 
 
-def generate_xml() -> typing.Tuple[str, str]:
+def generate_xml() -> Tuple[str, str]:
     """
     :return: success_xml_string, failure_xml_string
     """
     apitestka_logger.info("generate_xml")
     success_dict, failure_dict = generate_json()
     success_dict = dict({"xml_data": success_dict})
     failure_dict = dict({"xml_data": failure_dict})
@@ -47,8 +46,7 @@
             file_to_write.write(success_xml)
             pass
     except Exception as error:
         apitestka_logger.error(f"generate_xml_report, xml_file_name: {xml_file_name}, "
                                f"failed: {repr(error)}")
     finally:
         lock.release()
-
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_file/json_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 from pathlib import Path
 from threading import Lock
+from typing import Dict
 
 from je_api_testka.utils.exception.exception_tags import cant_find_json_error
 from je_api_testka.utils.exception.exception_tags import cant_save_json_error
 from je_api_testka.utils.exception.exceptions import APITesterJsonException
 
 lock = Lock()
 
 
-def read_action_json(json_file_path: str) -> dict:
+def read_action_json(json_file_path: str) -> Dict:
     """
     read the action json
     :param json_file_path json file's path to read
     """
     try:
         lock.acquire()
         file_path = Path(json_file_path)
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/json/json_format/json_process.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/logging/loggin_instance.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/mock_server/flask_mock_server.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/mock_server/flask_mock_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import typing
+from typing import Callable
 
 from flask.app import Flask
 
 from je_api_testka.utils.exception.exception_tags import get_bad_api_router_setting
 from je_api_testka.utils.exception.exceptions import MockServerException
 from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 
@@ -29,15 +29,15 @@
         :param kwargs: use to set methods or another param
         :return:
         """
         apitestka_logger.info(
             f"add_router, rule_and_function_dict: {rule_and_function_dict}, params: {kwargs}"
         )
         for rule, function in rule_and_function_dict.items():
-            if isinstance(rule, str) and isinstance(function, typing.Callable):
+            if isinstance(rule, str) and isinstance(function, Callable):
                 self.app.route(rule, **kwargs)(function)
             else:
                 apitestka_logger.error(
                     f"add_router, rule_and_function_dict: {rule_and_function_dict}, params: {kwargs}, "
                     f"failed: {MockServerException(get_bad_api_router_setting)}"
                 )
                 raise MockServerException(get_bad_api_router_setting)
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/package_manager/package_manager_class.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/package_manager/package_manager_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import typing
+from typing import Union
 from importlib import import_module
 from importlib.util import find_spec
 from inspect import getmembers, isfunction, isbuiltin, isclass
 from sys import stderr
 
 from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 
@@ -11,15 +11,15 @@
 
     def __init__(self):
         self.installed_package_dict = {
         }
         self.executor = None
         self.callback_executor = None
 
-    def check_package(self, package: str) -> typing.Union[str, None]:
+    def check_package(self, package: str) -> Union[str, None]:
         """
         :param package: package to check exists or not
         :return: package if find else None
         """
         if self.installed_package_dict.get(package, None) is None:
             found_spec = find_spec(package)
             if found_spec is not None:
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/project/create_project_structure.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/project/create_project_structure.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,31 @@
     executor_template_2, bad_executor_template_1
 from je_api_testka.utils.project.template.template_keyword import template_keyword_1, \
     template_keyword_2, bad_template_1
 
 
 def create_dir(dir_name: str) -> None:
     """
+    Create dir.
     :param dir_name: create dir use dir name
     :return: None
     """
     Path(dir_name).mkdir(
         parents=True,
         exist_ok=True
     )
 
 
 def create_template(parent_name: str, project_path: str = None) -> None:
+    """
+    Create template on dir {parent_name} with path {project_path}
+    :param parent_name: Project folder name.
+    :param project_path: Path use to create project dir if None set cwd as default.
+    :return:
+    """
     if project_path is None:
         project_path = getcwd()
     keyword_dir_path = Path(project_path + "/" + parent_name + "/keyword")
     executor_dir_path = Path(project_path + "/" + parent_name + "/executor")
     lock = Lock()
     if keyword_dir_path.exists() and keyword_dir_path.is_dir():
         write_action_json(project_path + "/" + parent_name + "/keyword/keyword1.json", template_keyword_1)
@@ -56,16 +63,17 @@
                 )
         finally:
             lock.release()
 
 
 def create_project_dir(project_path: str = None, parent_name: str = "APITestka") -> None:
     """
-    :param project_path: path used to create project dir
-    :param parent_name: project folder name
+    Use to create project.
+    :param project_path: Path used to create project dir if None set cwd as default.
+    :param parent_name: Project folder name.
     :return: None
     """
     if project_path is None:
         project_path = getcwd()
     create_dir(project_path + "/" + parent_name + "/keyword")
     create_dir(project_path + "/" + parent_name + "/executor")
     create_template(parent_name)
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/template_executor.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/project/template/template_keyword.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/project/template/template_keyword.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/socket_server/api_testka_socket_server.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/socket_server/api_testka_socket_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 from je_api_testka.utils.executor.action_executor import execute_action
 
 
 class TCPServerHandler(socketserver.BaseRequestHandler):
 
     def handle(self) -> None:
+        """
+        Receive message and try to execute message
+        :return: None
+        """
         command_string = str(self.request.recv(8192).strip(), encoding="utf-8")
         socket = self.request
         print("command is: " + command_string, flush=True)
         if command_string == "quit_server":
             self.server.shutdown()
             self.server.close_flag = True
             print("Now quit server", flush=True)
@@ -41,14 +45,20 @@
 
     def __init__(self, server_address, request_handler_class):
         super().__init__(server_address, request_handler_class)
         self.close_flag: bool = False
 
 
 def start_apitestka_socket_server(host: str = "localhost", port: int = 9939) -> TCPServer:
+    """
+    Start TCP socket server on host with port
+    :param host: Server host.
+    :param port: Server port.
+    :return: TCP server instance.
+    """
     if len(sys.argv) == 2:
         host = sys.argv[1]
     elif len(sys.argv) == 3:
         host = sys.argv[1]
         port = int(sys.argv[2])
     server = TCPServer((host, port), TCPServerHandler)
     server_thread = threading.Thread(target=server.serve_forever)
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.95/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/PKG-INFO` & `je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-api-testka-dev
-Version: 0.0.94
+Version: 0.0.95
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.94/je_api_testka_dev.egg-info/SOURCES.txt` & `je_api_testka_dev-0.0.95/je_api_testka_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.94/pyproject.toml` & `je_api_testka_dev-0.0.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_api_testka_dev"
-version = "0.0.94"
+version = "0.0.95"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Requests Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
@@ -37,8 +37,8 @@
 file = "README.md"
 content-type = "text/markdown"
 
 [tool.setuptools]
 license-files = ["LICENSE"]
 
 [tool.setuptools.packages]
-find = { namespaces = false }
+find = { namespaces = false }
```

