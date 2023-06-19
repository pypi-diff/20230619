# Comparing `tmp/xiaobaisaf-1.8.tar.gz` & `tmp/xiaobaisaf-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaobaisaf-1.8.tar", last modified: Fri Jan 13 17:47:54 2023, max compression
+gzip compressed data, was "xiaobaisaf-2.1.tar", last modified: Mon Jun 19 17:16:22 2023, max compression
```

## Comparing `xiaobaisaf-1.8.tar` & `xiaobaisaf-2.1.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.229393 xiaobaisaf-1.8/
--rw-rw-rw-   0        0        0    35181 2022-08-20 10:21:11.000000 xiaobaisaf-1.8/LICENSE
--rw-rw-rw-   0        0        0    10373 2023-01-13 17:47:54.229393 xiaobaisaf-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     9665 2023-01-13 17:45:41.000000 xiaobaisaf-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.202386 xiaobaisaf-1.8/saf/
--rw-rw-rw-   0        0        0     1438 2022-08-28 16:12:42.000000 xiaobaisaf-1.8/saf/__init__.py
--rw-rw-rw-   0        0        0      149 2023-01-13 17:45:41.000000 xiaobaisaf-1.8/saf/__version__.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.203386 xiaobaisaf-1.8/saf/data/
--rw-rw-rw-   0        0        0      225 2022-08-23 20:01:48.000000 xiaobaisaf-1.8/saf/data/__init__.py
--rw-rw-rw-   0        0        0     2943 2023-01-11 16:41:44.000000 xiaobaisaf-1.8/saf/data/config.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.204387 xiaobaisaf-1.8/saf/example/
--rw-rw-rw-   0        0        0      105 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.205386 xiaobaisaf-1.8/saf/example/api/
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.206386 xiaobaisaf-1.8/saf/example/api/Config/
--rw-rw-rw-   0        0        0      131 2023-01-13 16:05:35.000000 xiaobaisaf-1.8/saf/example/api/Config/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-01-13 17:38:57.000000 xiaobaisaf-1.8/saf/example/api/Config/config.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.207386 xiaobaisaf-1.8/saf/example/api/TestCases/
--rw-rw-rw-   0        0        0      129 2023-01-13 15:48:21.000000 xiaobaisaf-1.8/saf/example/api/TestCases/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-01-13 17:27:45.000000 xiaobaisaf-1.8/saf/example/api/TestCases/test_one_html_case_template.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.209386 xiaobaisaf-1.8/saf/example/api/Utils/
--rw-rw-rw-   0        0        0      131 2023-01-13 15:48:21.000000 xiaobaisaf-1.8/saf/example/api/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-01-13 16:05:35.000000 xiaobaisaf-1.8/saf/example/api/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-01-13 16:05:35.000000 xiaobaisaf-1.8/saf/example/api/Utils/__init__.py
--rw-rw-rw-   0        0        0      250 2023-01-13 15:48:21.000000 xiaobaisaf-1.8/saf/example/api/Utils/myRequest.py
--rw-rw-rw-   0        0        0      129 2023-01-13 15:52:50.000000 xiaobaisaf-1.8/saf/example/api/__init__.py
--rw-rw-rw-   0        0        0     1211 2023-01-13 17:41:51.000000 xiaobaisaf-1.8/saf/example/api/run.py
--rw-rw-rw-   0        0        0      549 2023-01-13 17:41:51.000000 xiaobaisaf-1.8/saf/example/api/send_email_script.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.209386 xiaobaisaf-1.8/saf/example/web/
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.213387 xiaobaisaf-1.8/saf/example/web/Cases/
--rw-rw-rw-   0        0        0      140 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/Cases/__init__.py
--rw-rw-rw-   0        0        0     2447 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/Cases/conftest.py
--rw-rw-rw-   0        0        0      930 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/Cases/test_xiaobai_case_allure.py
--rw-rw-rw-   0        0        0      962 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/Cases/test_xiaobai_case_submitBug.py
--rw-rw-rw-   0        0        0      320 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/Cases/test_xiaobai_case_v1.py
--rw-rw-rw-   0        0        0     1192 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/Cases/test_xiaobai_case_v2.py
--rw-rw-rw-   0        0        0      228 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/Cases/test_xiaobai_case_v3.py
--rw-rw-rw-   0        0        0      435 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.214388 xiaobaisaf-1.8/saf/example/web/pageObject/
--rw-rw-rw-   0        0        0      166 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/pageObject/__init__.py
--rw-rw-rw-   0        0        0      152 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/example/web/pageObject/register_page_element.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.219386 xiaobaisaf-1.8/saf/utils/
--rw-rw-rw-   0        0        0     8132 2023-01-11 16:41:44.000000 xiaobaisaf-1.8/saf/utils/BugUtils.py
--rw-rw-rw-   0        0        0     4987 2023-01-11 16:41:44.000000 xiaobaisaf-1.8/saf/utils/PageObjectGenerator.py
--rw-rw-rw-   0        0        0     2099 2023-01-13 16:05:35.000000 xiaobaisaf-1.8/saf/utils/YamlUtils.py
--rw-rw-rw-   0        0        0      201 2022-08-21 10:03:39.000000 xiaobaisaf-1.8/saf/utils/__init__.py
--rw-rw-rw-   0        0        0      129 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/utils/downloadUtils.py
--rw-rw-rw-   0        0        0     1271 2022-08-28 16:12:42.000000 xiaobaisaf-1.8/saf/utils/elementUtils.py
--rw-rw-rw-   0        0        0      660 2022-08-28 15:59:39.000000 xiaobaisaf-1.8/saf/utils/imageUtils.py
--rw-rw-rw-   0        0        0     1369 2022-08-28 16:52:51.000000 xiaobaisaf-1.8/saf/utils/networkSpeedUtils.py
--rw-rw-rw-   0        0        0      166 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/saf/utils/osEnvUtils.py
--rw-rw-rw-   0        0        0     2694 2022-08-28 15:34:31.000000 xiaobaisaf-1.8/saf/utils/sendMsgUtils.py
--rw-rw-rw-   0        0        0     1529 2023-01-11 16:43:52.000000 xiaobaisaf-1.8/saf/utils/xiaobaicmd.py
--rw-rw-rw-   0        0        0       42 2023-01-13 17:47:54.229393 xiaobaisaf-1.8/setup.cfg
--rw-rw-rw-   0        0        0     2164 2023-01-11 16:41:45.000000 xiaobaisaf-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-13 17:47:54.228393 xiaobaisaf-1.8/xiaobaisaf.egg-info/
--rw-rw-rw-   0        0        0    10373 2023-01-13 17:47:54.000000 xiaobaisaf-1.8/xiaobaisaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-01-13 17:47:54.000000 xiaobaisaf-1.8/xiaobaisaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 17:47:54.000000 xiaobaisaf-1.8/xiaobaisaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-01-13 17:47:54.000000 xiaobaisaf-1.8/xiaobaisaf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-01-13 17:47:54.000000 xiaobaisaf-1.8/xiaobaisaf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-01-13 17:47:54.000000 xiaobaisaf-1.8/xiaobaisaf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.707762 xiaobaisaf-2.1/
+-rw-rw-rw-   0        0        0    35181 2022-08-20 10:21:11.000000 xiaobaisaf-2.1/LICENSE
+-rw-rw-rw-   0        0        0    11342 2023-06-19 17:16:22.707762 xiaobaisaf-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10673 2023-06-19 16:27:20.000000 xiaobaisaf-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.681832 xiaobaisaf-2.1/saf/
+-rw-rw-rw-   0        0        0     1438 2022-08-28 16:12:42.000000 xiaobaisaf-2.1/saf/__init__.py
+-rw-rw-rw-   0        0        0      149 2023-06-19 16:06:24.000000 xiaobaisaf-2.1/saf/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.682829 xiaobaisaf-2.1/saf/data/
+-rw-rw-rw-   0        0        0      225 2022-08-23 20:01:48.000000 xiaobaisaf-2.1/saf/data/__init__.py
+-rw-rw-rw-   0        0        0     2943 2023-01-11 16:41:44.000000 xiaobaisaf-2.1/saf/data/config.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.683826 xiaobaisaf-2.1/saf/example/
+-rw-rw-rw-   0        0        0      100 2023-06-14 16:17:05.000000 xiaobaisaf-2.1/saf/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.684825 xiaobaisaf-2.1/saf/example/api/
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.685822 xiaobaisaf-2.1/saf/example/api/Config/
+-rw-rw-rw-   0        0        0      131 2023-01-13 16:05:35.000000 xiaobaisaf-2.1/saf/example/api/Config/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-01-13 17:38:57.000000 xiaobaisaf-2.1/saf/example/api/Config/config.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.686819 xiaobaisaf-2.1/saf/example/api/TestCases/
+-rw-rw-rw-   0        0        0      129 2023-01-13 15:48:21.000000 xiaobaisaf-2.1/saf/example/api/TestCases/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-01-13 17:27:45.000000 xiaobaisaf-2.1/saf/example/api/TestCases/test_one_html_case_template.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.688814 xiaobaisaf-2.1/saf/example/api/Utils/
+-rw-rw-rw-   0        0        0      131 2023-01-13 15:48:21.000000 xiaobaisaf-2.1/saf/example/api/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-01-13 16:05:35.000000 xiaobaisaf-2.1/saf/example/api/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-01-13 16:05:35.000000 xiaobaisaf-2.1/saf/example/api/Utils/__init__.py
+-rw-rw-rw-   0        0        0      250 2023-01-13 15:48:21.000000 xiaobaisaf-2.1/saf/example/api/Utils/myRequest.py
+-rw-rw-rw-   0        0        0      129 2023-01-13 15:52:50.000000 xiaobaisaf-2.1/saf/example/api/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-01-13 17:41:51.000000 xiaobaisaf-2.1/saf/example/api/run.py
+-rw-rw-rw-   0        0        0      549 2023-01-13 17:41:51.000000 xiaobaisaf-2.1/saf/example/api/send_email_script.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.688814 xiaobaisaf-2.1/saf/example/web/
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.691805 xiaobaisaf-2.1/saf/example/web/Cases/
+-rw-rw-rw-   0        0        0      140 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/__init__.py
+-rw-rw-rw-   0        0        0     2441 2023-06-14 07:25:00.000000 xiaobaisaf-2.1/saf/example/web/Cases/conftest.py
+-rw-rw-rw-   0        0        0      930 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_allure.py
+-rw-rw-rw-   0        0        0      962 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_submitBug.py
+-rw-rw-rw-   0        0        0      320 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_v1.py
+-rw-rw-rw-   0        0        0     1192 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_v2.py
+-rw-rw-rw-   0        0        0      228 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_v3.py
+-rw-rw-rw-   0        0        0      435 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.692803 xiaobaisaf-2.1/saf/example/web/pageObject/
+-rw-rw-rw-   0        0        0      166 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/pageObject/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/pageObject/register_page_element.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.699784 xiaobaisaf-2.1/saf/utils/
+-rw-rw-rw-   0        0        0     8132 2023-01-11 16:41:44.000000 xiaobaisaf-2.1/saf/utils/BugUtils.py
+-rw-rw-rw-   0        0        0      126 2023-06-19 17:16:21.000000 xiaobaisaf-2.1/saf/utils/Demo.py
+-rw-rw-rw-   0        0        0     2042 2023-06-19 17:15:58.000000 xiaobaisaf-2.1/saf/utils/MonitorAndroidDeviceGUI.py
+-rw-rw-rw-   0        0        0     8917 2023-06-19 14:02:01.000000 xiaobaisaf-2.1/saf/utils/MonitorAndroidPackageCLI.py
+-rw-rw-rw-   0        0        0    14192 2023-06-19 14:02:01.000000 xiaobaisaf-2.1/saf/utils/MonitorAndroidPackageGUI.py
+-rw-rw-rw-   0        0        0     2099 2023-01-13 16:05:35.000000 xiaobaisaf-2.1/saf/utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      201 2022-08-21 10:03:39.000000 xiaobaisaf-2.1/saf/utils/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/utils/downloadUtils.py
+-rw-rw-rw-   0        0        0     1271 2022-08-28 16:12:42.000000 xiaobaisaf-2.1/saf/utils/elementUtils.py
+-rw-rw-rw-   0        0        0      660 2022-08-28 15:59:39.000000 xiaobaisaf-2.1/saf/utils/imageUtils.py
+-rw-rw-rw-   0        0        0     1369 2022-08-28 16:52:51.000000 xiaobaisaf-2.1/saf/utils/networkSpeedUtils.py
+-rw-rw-rw-   0        0        0      166 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/utils/osEnvUtils.py
+-rw-rw-rw-   0        0        0     8924 2023-06-14 07:25:00.000000 xiaobaisaf-2.1/saf/utils/selenium2POM.py
+-rw-rw-rw-   0        0        0     2694 2022-08-28 15:34:31.000000 xiaobaisaf-2.1/saf/utils/sendMsgUtils.py
+-rw-rw-rw-   0        0        0     2338 2023-06-19 16:27:20.000000 xiaobaisaf-2.1/saf/utils/xiaobaicmd.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 17:16:22.707762 xiaobaisaf-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2239 2023-06-15 15:15:26.000000 xiaobaisaf-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.706766 xiaobaisaf-2.1/xiaobaisaf.egg-info/
+-rw-rw-rw-   0        0        0    11342 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1556 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/top_level.txt
```

### Comparing `xiaobaisaf-1.8/LICENSE` & `xiaobaisaf-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/PKG-INFO` & `xiaobaisaf-2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 1.8
+Version: 2.1
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
-License: UNKNOWN
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
-Platform: UNKNOWN
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # simlpe_automation_framework
 
 ### 介绍
@@ -42,14 +40,15 @@
         return 'https://open.feishu.cn/open-apis/bot/v2/hook/xxxx'
 
 class dingding(object):
     @staticmethod
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
+
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
 from saf.utils.sendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
@@ -61,14 +60,15 @@
     report = outcome.get_result()
     if report.outcome == 'failed':
         # 调用机器人发送执行结果
         robotSendMessage(robot_name='feishu', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='feishu,dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
 ```
+
 - 用例文件
 ```python
 # fielname = test_xiaobai_auto_script.py
 
 def setup_module():
     ''' 用例脚本执行之前需要准备的信息 '''
     ...
@@ -96,14 +96,15 @@
     ''' 用例函数
         需要针对业务场景的测试步骤的实现
             1、UI测试就是定位需要操作的界面节点然后执行操作
             2、API测试就是执行相关接口实现接口的功能
         需要针对每次的结果添加断言进行判断处理
     '''
 ```
+
 ```python
 # filename = test_xiaobai_shop_allure.py
 # JDK与Allure已安装且配置好环境变量（若不知道可以查看公众号：小白科技之窗）
 import pytest
 import allure
 
 @allure.feature('下单')
@@ -136,81 +137,85 @@
 allure open ../report
 '''
 ```
 
 ### saf>1.1 使用禅道API，测试失败自动提单
 - 需要在禅道后台>>二次开发>>应用>>添加应用>>创建开启免密的应用 
 - 需要将上一步所生成数据【代号】与【密钥】写入到`saf/data/config.py`中zenTao相关的参数位置
-  ```python
-  # filename = saf/data/config.py
-  import hashlib
-  import time
-  class zenTao(object):
-      '''
-      参考禅道接口文档：
-      https://www.zentao.net/book/zentaopmshelp/integration-287.html
-      '''
-      @staticmethod
-      def baseURL():
-          ''' 禅道的根路径 '''
-          return 'http://192.168.254.133/zentao'
-   
-      @staticmethod
-      def account():
-          ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
-          return '开启密钥的账户名称，例如管理员：admin'
-   
-      @staticmethod
-      def getCode():
-          ''' 后台-》二次开发-》应用-》创建-》代号 '''
-          return '复制生成应用的代号字符串'
-    
-      @staticmethod
-      def getKey():
-          ''' 后台-》二次开发-》应用-》创建-》密钥 '''
-          return '复制生成应用的密钥字符串'
-    
-      @staticmethod
-      def getTime():
-          ''' 获取时间戳 ，默认即可，无需修改'''
-          return int(time.time())
-    
-      @staticmethod
-      def getToken():
-          ''' 获取token： md5($code + $key + $time) ，默认即可，无需修改'''
-          _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
-          return _md5.hexdigest()
-  ```
+
+```python
+# filename = saf/data/config.py
+import hashlib
+import time
+class zenTao(object):
+    '''
+    参考禅道接口文档：
+    https://www.zentao.net/book/zentaopmshelp/integration-287.html
+    '''
+    @staticmethod
+    def baseURL():
+        ''' 禅道的根路径 '''
+        return 'http://192.168.254.133/zentao'
+ 
+    @staticmethod
+    def account():
+        ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
+        return '开启密钥的账户名称，例如管理员：admin'
+ 
+    @staticmethod
+    def getCode():
+        ''' 后台-》二次开发-》应用-》创建-》代号 '''
+        return '复制生成应用的代号字符串'
+  
+    @staticmethod
+    def getKey():
+        ''' 后台-》二次开发-》应用-》创建-》密钥 '''
+        return '复制生成应用的密钥字符串'
+  
+    @staticmethod
+    def getTime():
+        ''' 获取时间戳 ，默认即可，无需修改'''
+        return int(time.time())
+  
+    @staticmethod
+    def getToken():
+        ''' 获取token： md5($code + $key + $time) ，默认即可，无需修改'''
+        _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
+        return _md5.hexdigest()
+```
+
 - 用例同目录下创建`conftest.py`pytest的配置文件
-  ```python
-  # filename = conftest.py
-  from saf.utils.submitBugUtils import addZenTaoBUG
-  import pytest
-    
-  @pytest.mark.hookwrapper
-  def pytest_runtest_makereport(item, call):
-    """
-    :param item:
-    """
-    outcome = yield
-    report = outcome.get_result()
-    if report.outcome == 'failed':
-        doc = item.function.__doc__
-        doc = str(doc).replace('\n', '<br>')
-        addZenTaoBUG(title=item.function.__name__,
-                          steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
+```python
+# filename = conftest.py
+from saf.utils.BugUtils import addZenTaoBUG
+import pytest
+  
+@pytest.mark.hookwrapper
+def pytest_runtest_makereport(item, call):
+  """
+  :param item:
+  """
+  outcome = yield
+  report = outcome.get_result()
+  if report.outcome == 'failed':
+      doc = item.function.__doc__
+      doc = str(doc).replace('\n', '<br>')
+      addZenTaoBUG(title=item.function.__name__,
+                        steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
     
-  ```
+ ```
 - 用例文件正常编写，正常运行即可
 
 ### saf>1.0 拷贝web自动化模板到D:\autoProject目录下
-```commandline
+```bat
 
 xiaobaicmd -t web -d D:\autoProject
+xiaobaicmd --template web --dirname D:\autoProject
 xiaobaicmd -t api -d D:\autoProject
+xiaobaicmd --template api --dirname D:\autoProject
 xiaobaicmd -t app -d D:\autoProject[暂时不支持]
 ```
 
 ### saf>1.3 新增pytest参数多种样例，`web`中包含
 ```python
 # filename = test_xiaobai_case_v2.py
 import pytest
@@ -251,19 +256,40 @@
 ---
 test_login:
   keys: username,password,_assert
   values:
     - ('xiaobai', '12346', 200)
     - ('xiaohui', '123456', 200)
 ```
+
+### saf>1.8 基于selenium完成正常的页面操作，工具会自动在当前目录下生成Pages目录，目录内会自动生成当前打开的所有页面的PageObject代码，命令如下：
+```cmd
+xiaobaicmd -u URL 
+xiaobaicmd -url URL 
+```
+
+### saf>1.9  基于adb实现监控Android设备中APP操作时实时生成XPath表达式及坐标等数据
+```cmd
+xiaobaicmd -m gui             # 基于界面实时获取APP数据
+xiaobaicmd --monitor gui      # 基于界面实时获取APP数据
+xiaobaicmd -m cli             # 基于命令实时获取APP数据
+xiaobaicmd --monitor cli      # 基于命令实时获取APP数据
+```
+
+### saf>2.0   基础adb实现Android设备的界面监控功能
+```cmd
+xiaobaicmd -e [1]   # 默认值为1，可省略；表示打开界面监控第一个设备的实时界面
+xiaobaicmd --device 1
+```
+
 ### 环境检测[还未实现]
-```commandline
+```bat
 xiaobaicmd  --init
 
-检测内容：
+检测内容: 
 1、python版本及第三方库
 2、第三方工具及环境
 ```
 
 ### 参与贡献
 [selenium官网文档](https://www.selenium.dev/documentation/, "selenium官网文档")
 
@@ -283,19 +309,21 @@
 
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
-| version | info                 |
-|---------|----------------------|
-| 1.0     | 基本实现web自动化模板功能       |
-| 1.1     | fix上个版本的BUG          |
-| 1.2     | 新增allure报告库及封装禅道提单接口 |
-| 1.3     | 新增jira提单接口           |
-| 1.4     | 新增pytest参数化样例        |
-| 1.5     | 优化pytest样例内容         |
-| 1.6     | 优化                   |
-| 1.7     | 新增基础环境检测功能           |
-| 1.8     | 新增API自动化模板           |
-
+| version | info                    |
+|---------|-------------------------|
+| 1.0     | 基本实现web自动化模板功能          |
+| 1.1     | fix上个版本的BUG             |
+| 1.2     | 新增allure报告库及封装禅道提单接口    |
+| 1.3     | 新增jira提单接口              |
+| 1.4     | 新增pytest参数化样例           |
+| 1.5     | 优化pytest样例内容            |
+| 1.6     | 优化                      |
+| 1.7     | 新增基础环境检测功能              |
+| 1.8     | 新增API自动化模板              |
+| 1.9     | 新增xiaobaicmd -u命令       |
+| 2.0     | 新增xiaobaicmd -m命令       |
+| 2.1     | 新增xiaobaicmd --device命令 |
```

### Comparing `xiaobaisaf-1.8/README.md` & `xiaobaisaf-2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         return 'https://open.feishu.cn/open-apis/bot/v2/hook/xxxx'
 
 class dingding(object):
     @staticmethod
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
+
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
 from saf.utils.sendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
@@ -47,14 +48,15 @@
     report = outcome.get_result()
     if report.outcome == 'failed':
         # 调用机器人发送执行结果
         robotSendMessage(robot_name='feishu', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='feishu,dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
 ```
+
 - 用例文件
 ```python
 # fielname = test_xiaobai_auto_script.py
 
 def setup_module():
     ''' 用例脚本执行之前需要准备的信息 '''
     ...
@@ -82,14 +84,15 @@
     ''' 用例函数
         需要针对业务场景的测试步骤的实现
             1、UI测试就是定位需要操作的界面节点然后执行操作
             2、API测试就是执行相关接口实现接口的功能
         需要针对每次的结果添加断言进行判断处理
     '''
 ```
+
 ```python
 # filename = test_xiaobai_shop_allure.py
 # JDK与Allure已安装且配置好环境变量（若不知道可以查看公众号：小白科技之窗）
 import pytest
 import allure
 
 @allure.feature('下单')
@@ -122,81 +125,85 @@
 allure open ../report
 '''
 ```
 
 ### saf>1.1 使用禅道API，测试失败自动提单
 - 需要在禅道后台>>二次开发>>应用>>添加应用>>创建开启免密的应用 
 - 需要将上一步所生成数据【代号】与【密钥】写入到`saf/data/config.py`中zenTao相关的参数位置
-  ```python
-  # filename = saf/data/config.py
-  import hashlib
-  import time
-  class zenTao(object):
-      '''
-      参考禅道接口文档：
-      https://www.zentao.net/book/zentaopmshelp/integration-287.html
-      '''
-      @staticmethod
-      def baseURL():
-          ''' 禅道的根路径 '''
-          return 'http://192.168.254.133/zentao'
-   
-      @staticmethod
-      def account():
-          ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
-          return '开启密钥的账户名称，例如管理员：admin'
-   
-      @staticmethod
-      def getCode():
-          ''' 后台-》二次开发-》应用-》创建-》代号 '''
-          return '复制生成应用的代号字符串'
-    
-      @staticmethod
-      def getKey():
-          ''' 后台-》二次开发-》应用-》创建-》密钥 '''
-          return '复制生成应用的密钥字符串'
-    
-      @staticmethod
-      def getTime():
-          ''' 获取时间戳 ，默认即可，无需修改'''
-          return int(time.time())
-    
-      @staticmethod
-      def getToken():
-          ''' 获取token： md5($code + $key + $time) ，默认即可，无需修改'''
-          _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
-          return _md5.hexdigest()
-  ```
+
+```python
+# filename = saf/data/config.py
+import hashlib
+import time
+class zenTao(object):
+    '''
+    参考禅道接口文档：
+    https://www.zentao.net/book/zentaopmshelp/integration-287.html
+    '''
+    @staticmethod
+    def baseURL():
+        ''' 禅道的根路径 '''
+        return 'http://192.168.254.133/zentao'
+ 
+    @staticmethod
+    def account():
+        ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
+        return '开启密钥的账户名称，例如管理员：admin'
+ 
+    @staticmethod
+    def getCode():
+        ''' 后台-》二次开发-》应用-》创建-》代号 '''
+        return '复制生成应用的代号字符串'
+  
+    @staticmethod
+    def getKey():
+        ''' 后台-》二次开发-》应用-》创建-》密钥 '''
+        return '复制生成应用的密钥字符串'
+  
+    @staticmethod
+    def getTime():
+        ''' 获取时间戳 ，默认即可，无需修改'''
+        return int(time.time())
+  
+    @staticmethod
+    def getToken():
+        ''' 获取token： md5($code + $key + $time) ，默认即可，无需修改'''
+        _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
+        return _md5.hexdigest()
+```
+
 - 用例同目录下创建`conftest.py`pytest的配置文件
-  ```python
-  # filename = conftest.py
-  from saf.utils.submitBugUtils import addZenTaoBUG
-  import pytest
-    
-  @pytest.mark.hookwrapper
-  def pytest_runtest_makereport(item, call):
-    """
-    :param item:
-    """
-    outcome = yield
-    report = outcome.get_result()
-    if report.outcome == 'failed':
-        doc = item.function.__doc__
-        doc = str(doc).replace('\n', '<br>')
-        addZenTaoBUG(title=item.function.__name__,
-                          steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
+```python
+# filename = conftest.py
+from saf.utils.BugUtils import addZenTaoBUG
+import pytest
+  
+@pytest.mark.hookwrapper
+def pytest_runtest_makereport(item, call):
+  """
+  :param item:
+  """
+  outcome = yield
+  report = outcome.get_result()
+  if report.outcome == 'failed':
+      doc = item.function.__doc__
+      doc = str(doc).replace('\n', '<br>')
+      addZenTaoBUG(title=item.function.__name__,
+                        steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
     
-  ```
+ ```
 - 用例文件正常编写，正常运行即可
 
 ### saf>1.0 拷贝web自动化模板到D:\autoProject目录下
-```commandline
+```bat
 
 xiaobaicmd -t web -d D:\autoProject
+xiaobaicmd --template web --dirname D:\autoProject
 xiaobaicmd -t api -d D:\autoProject
+xiaobaicmd --template api --dirname D:\autoProject
 xiaobaicmd -t app -d D:\autoProject[暂时不支持]
 ```
 
 ### saf>1.3 新增pytest参数多种样例，`web`中包含
 ```python
 # filename = test_xiaobai_case_v2.py
 import pytest
@@ -237,19 +244,40 @@
 ---
 test_login:
   keys: username,password,_assert
   values:
     - ('xiaobai', '12346', 200)
     - ('xiaohui', '123456', 200)
 ```
+
+### saf>1.8 基于selenium完成正常的页面操作，工具会自动在当前目录下生成Pages目录，目录内会自动生成当前打开的所有页面的PageObject代码，命令如下：
+```cmd
+xiaobaicmd -u URL 
+xiaobaicmd -url URL 
+```
+
+### saf>1.9  基于adb实现监控Android设备中APP操作时实时生成XPath表达式及坐标等数据
+```cmd
+xiaobaicmd -m gui             # 基于界面实时获取APP数据
+xiaobaicmd --monitor gui      # 基于界面实时获取APP数据
+xiaobaicmd -m cli             # 基于命令实时获取APP数据
+xiaobaicmd --monitor cli      # 基于命令实时获取APP数据
+```
+
+### saf>2.0   基础adb实现Android设备的界面监控功能
+```cmd
+xiaobaicmd -e [1]   # 默认值为1，可省略；表示打开界面监控第一个设备的实时界面
+xiaobaicmd --device 1
+```
+
 ### 环境检测[还未实现]
-```commandline
+```bat
 xiaobaicmd  --init
 
-检测内容：
+检测内容: 
 1、python版本及第三方库
 2、第三方工具及环境
 ```
 
 ### 参与贡献
 [selenium官网文档](https://www.selenium.dev/documentation/, "selenium官网文档")
 
@@ -269,18 +297,21 @@
 
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
-| version | info                 |
-|---------|----------------------|
-| 1.0     | 基本实现web自动化模板功能       |
-| 1.1     | fix上个版本的BUG          |
-| 1.2     | 新增allure报告库及封装禅道提单接口 |
-| 1.3     | 新增jira提单接口           |
-| 1.4     | 新增pytest参数化样例        |
-| 1.5     | 优化pytest样例内容         |
-| 1.6     | 优化                   |
-| 1.7     | 新增基础环境检测功能           |
-| 1.8     | 新增API自动化模板           |
+| version | info                    |
+|---------|-------------------------|
+| 1.0     | 基本实现web自动化模板功能          |
+| 1.1     | fix上个版本的BUG             |
+| 1.2     | 新增allure报告库及封装禅道提单接口    |
+| 1.3     | 新增jira提单接口              |
+| 1.4     | 新增pytest参数化样例           |
+| 1.5     | 优化pytest样例内容            |
+| 1.6     | 优化                      |
+| 1.7     | 新增基础环境检测功能              |
+| 1.8     | 新增API自动化模板              |
+| 1.9     | 新增xiaobaicmd -u命令       |
+| 2.0     | 新增xiaobaicmd -m命令       |
+| 2.1     | 新增xiaobaicmd --device命令 |
```

### Comparing `xiaobaisaf-1.8/saf/__init__.py` & `xiaobaisaf-2.1/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/data/config.py` & `xiaobaisaf-2.1/saf/data/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/example/api/Config/config.py` & `xiaobaisaf-2.1/saf/example/api/Config/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/example/api/TestCases/test_one_html_case_template.py` & `xiaobaisaf-2.1/saf/example/api/TestCases/test_one_html_case_template.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/example/api/Utils/YamlUtils.py` & `xiaobaisaf-2.1/saf/example/api/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/example/api/run.py` & `xiaobaisaf-2.1/saf/example/api/run.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/example/api/send_email_script.py` & `xiaobaisaf-2.1/saf/example/api/send_email_script.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/example/web/Cases/conftest.py` & `xiaobaisaf-2.1/saf/example/web/Cases/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 '''
 @Author: xiaobaiTser
 @Time  : 2022/8/21 0:23
 @File  : conftest.py
 '''
-from saf.utils.submitBugUtils import addZenTaoBUG
+from saf.utils.BugUtils import addZenTaoBUG
 from saf.utils.sendMsgUtils import robotSendMessage
 import pytest
 
 TESTTYPE = ['sendMsg', 'submitBug'][0]
 
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item, call):
```

### Comparing `xiaobaisaf-1.8/saf/example/web/Cases/test_xiaobai_case_allure.py` & `xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_allure.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/example/web/Cases/test_xiaobai_case_submitBug.py` & `xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_submitBug.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/example/web/Cases/test_xiaobai_case_v2.py` & `xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_v2.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/utils/BugUtils.py` & `xiaobaisaf-2.1/saf/utils/BugUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/utils/YamlUtils.py` & `xiaobaisaf-2.1/saf/utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/utils/elementUtils.py` & `xiaobaisaf-2.1/saf/utils/elementUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/utils/imageUtils.py` & `xiaobaisaf-2.1/saf/utils/imageUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/utils/networkSpeedUtils.py` & `xiaobaisaf-2.1/saf/utils/networkSpeedUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/saf/utils/sendMsgUtils.py` & `xiaobaisaf-2.1/saf/utils/sendMsgUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-1.8/setup.py` & `xiaobaisaf-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,19 +30,23 @@
     # 指定包名，即你需要打包的包名称，要实际在你本地存在哟，它会将指定包名下的所有"*.py"文件进行打包哟，但不会递归去拷贝所有的子包内容。
     # 综上所述，我们如果想要把一个包的所有"*.py"文件进行打包，应该在packages列表写下所有包的层级关系哟~这样就开源将指定包路径的所有".py"文件进行打包!
     keywords="saf test auto automation xiaobai xiaobaiauto2 test framework",
     packages=find_packages(),
     # 指定Python的版本
     python_requires='>=3.6, <3.10',
     install_requires=[
+        'adbutils',
         'allure-pytest',
         'ddddocr',
         'loguru',
         'httpx',
         'jira',
+        'bs4',
+        'lxml',
+        'pypinyin',
         'webdriver_manager',
         'xiaobaiauto2',
     ],
     entry_points={
         'console_scripts': [
             'xiaobaicmd = saf.utils.xiaobaicmd:main'
         ]
```

### Comparing `xiaobaisaf-1.8/xiaobaisaf.egg-info/PKG-INFO` & `xiaobaisaf-2.1/xiaobaisaf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 1.8
+Version: 2.1
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
-License: UNKNOWN
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
-Platform: UNKNOWN
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # simlpe_automation_framework
 
 ### 介绍
@@ -42,14 +40,15 @@
         return 'https://open.feishu.cn/open-apis/bot/v2/hook/xxxx'
 
 class dingding(object):
     @staticmethod
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
+
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
 from saf.utils.sendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
@@ -61,14 +60,15 @@
     report = outcome.get_result()
     if report.outcome == 'failed':
         # 调用机器人发送执行结果
         robotSendMessage(robot_name='feishu', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='feishu,dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
 ```
+
 - 用例文件
 ```python
 # fielname = test_xiaobai_auto_script.py
 
 def setup_module():
     ''' 用例脚本执行之前需要准备的信息 '''
     ...
@@ -96,14 +96,15 @@
     ''' 用例函数
         需要针对业务场景的测试步骤的实现
             1、UI测试就是定位需要操作的界面节点然后执行操作
             2、API测试就是执行相关接口实现接口的功能
         需要针对每次的结果添加断言进行判断处理
     '''
 ```
+
 ```python
 # filename = test_xiaobai_shop_allure.py
 # JDK与Allure已安装且配置好环境变量（若不知道可以查看公众号：小白科技之窗）
 import pytest
 import allure
 
 @allure.feature('下单')
@@ -136,81 +137,85 @@
 allure open ../report
 '''
 ```
 
 ### saf>1.1 使用禅道API，测试失败自动提单
 - 需要在禅道后台>>二次开发>>应用>>添加应用>>创建开启免密的应用 
 - 需要将上一步所生成数据【代号】与【密钥】写入到`saf/data/config.py`中zenTao相关的参数位置
-  ```python
-  # filename = saf/data/config.py
-  import hashlib
-  import time
-  class zenTao(object):
-      '''
-      参考禅道接口文档：
-      https://www.zentao.net/book/zentaopmshelp/integration-287.html
-      '''
-      @staticmethod
-      def baseURL():
-          ''' 禅道的根路径 '''
-          return 'http://192.168.254.133/zentao'
-   
-      @staticmethod
-      def account():
-          ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
-          return '开启密钥的账户名称，例如管理员：admin'
-   
-      @staticmethod
-      def getCode():
-          ''' 后台-》二次开发-》应用-》创建-》代号 '''
-          return '复制生成应用的代号字符串'
-    
-      @staticmethod
-      def getKey():
-          ''' 后台-》二次开发-》应用-》创建-》密钥 '''
-          return '复制生成应用的密钥字符串'
-    
-      @staticmethod
-      def getTime():
-          ''' 获取时间戳 ，默认即可，无需修改'''
-          return int(time.time())
-    
-      @staticmethod
-      def getToken():
-          ''' 获取token： md5($code + $key + $time) ，默认即可，无需修改'''
-          _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
-          return _md5.hexdigest()
-  ```
+
+```python
+# filename = saf/data/config.py
+import hashlib
+import time
+class zenTao(object):
+    '''
+    参考禅道接口文档：
+    https://www.zentao.net/book/zentaopmshelp/integration-287.html
+    '''
+    @staticmethod
+    def baseURL():
+        ''' 禅道的根路径 '''
+        return 'http://192.168.254.133/zentao'
+ 
+    @staticmethod
+    def account():
+        ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
+        return '开启密钥的账户名称，例如管理员：admin'
+ 
+    @staticmethod
+    def getCode():
+        ''' 后台-》二次开发-》应用-》创建-》代号 '''
+        return '复制生成应用的代号字符串'
+  
+    @staticmethod
+    def getKey():
+        ''' 后台-》二次开发-》应用-》创建-》密钥 '''
+        return '复制生成应用的密钥字符串'
+  
+    @staticmethod
+    def getTime():
+        ''' 获取时间戳 ，默认即可，无需修改'''
+        return int(time.time())
+  
+    @staticmethod
+    def getToken():
+        ''' 获取token： md5($code + $key + $time) ，默认即可，无需修改'''
+        _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
+        return _md5.hexdigest()
+```
+
 - 用例同目录下创建`conftest.py`pytest的配置文件
-  ```python
-  # filename = conftest.py
-  from saf.utils.submitBugUtils import addZenTaoBUG
-  import pytest
-    
-  @pytest.mark.hookwrapper
-  def pytest_runtest_makereport(item, call):
-    """
-    :param item:
-    """
-    outcome = yield
-    report = outcome.get_result()
-    if report.outcome == 'failed':
-        doc = item.function.__doc__
-        doc = str(doc).replace('\n', '<br>')
-        addZenTaoBUG(title=item.function.__name__,
-                          steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
+```python
+# filename = conftest.py
+from saf.utils.BugUtils import addZenTaoBUG
+import pytest
+  
+@pytest.mark.hookwrapper
+def pytest_runtest_makereport(item, call):
+  """
+  :param item:
+  """
+  outcome = yield
+  report = outcome.get_result()
+  if report.outcome == 'failed':
+      doc = item.function.__doc__
+      doc = str(doc).replace('\n', '<br>')
+      addZenTaoBUG(title=item.function.__name__,
+                        steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
     
-  ```
+ ```
 - 用例文件正常编写，正常运行即可
 
 ### saf>1.0 拷贝web自动化模板到D:\autoProject目录下
-```commandline
+```bat
 
 xiaobaicmd -t web -d D:\autoProject
+xiaobaicmd --template web --dirname D:\autoProject
 xiaobaicmd -t api -d D:\autoProject
+xiaobaicmd --template api --dirname D:\autoProject
 xiaobaicmd -t app -d D:\autoProject[暂时不支持]
 ```
 
 ### saf>1.3 新增pytest参数多种样例，`web`中包含
 ```python
 # filename = test_xiaobai_case_v2.py
 import pytest
@@ -251,19 +256,40 @@
 ---
 test_login:
   keys: username,password,_assert
   values:
     - ('xiaobai', '12346', 200)
     - ('xiaohui', '123456', 200)
 ```
+
+### saf>1.8 基于selenium完成正常的页面操作，工具会自动在当前目录下生成Pages目录，目录内会自动生成当前打开的所有页面的PageObject代码，命令如下：
+```cmd
+xiaobaicmd -u URL 
+xiaobaicmd -url URL 
+```
+
+### saf>1.9  基于adb实现监控Android设备中APP操作时实时生成XPath表达式及坐标等数据
+```cmd
+xiaobaicmd -m gui             # 基于界面实时获取APP数据
+xiaobaicmd --monitor gui      # 基于界面实时获取APP数据
+xiaobaicmd -m cli             # 基于命令实时获取APP数据
+xiaobaicmd --monitor cli      # 基于命令实时获取APP数据
+```
+
+### saf>2.0   基础adb实现Android设备的界面监控功能
+```cmd
+xiaobaicmd -e [1]   # 默认值为1，可省略；表示打开界面监控第一个设备的实时界面
+xiaobaicmd --device 1
+```
+
 ### 环境检测[还未实现]
-```commandline
+```bat
 xiaobaicmd  --init
 
-检测内容：
+检测内容: 
 1、python版本及第三方库
 2、第三方工具及环境
 ```
 
 ### 参与贡献
 [selenium官网文档](https://www.selenium.dev/documentation/, "selenium官网文档")
 
@@ -283,19 +309,21 @@
 
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
-| version | info                 |
-|---------|----------------------|
-| 1.0     | 基本实现web自动化模板功能       |
-| 1.1     | fix上个版本的BUG          |
-| 1.2     | 新增allure报告库及封装禅道提单接口 |
-| 1.3     | 新增jira提单接口           |
-| 1.4     | 新增pytest参数化样例        |
-| 1.5     | 优化pytest样例内容         |
-| 1.6     | 优化                   |
-| 1.7     | 新增基础环境检测功能           |
-| 1.8     | 新增API自动化模板           |
-
+| version | info                    |
+|---------|-------------------------|
+| 1.0     | 基本实现web自动化模板功能          |
+| 1.1     | fix上个版本的BUG             |
+| 1.2     | 新增allure报告库及封装禅道提单接口    |
+| 1.3     | 新增jira提单接口              |
+| 1.4     | 新增pytest参数化样例           |
+| 1.5     | 优化pytest样例内容            |
+| 1.6     | 优化                      |
+| 1.7     | 新增基础环境检测功能              |
+| 1.8     | 新增API自动化模板              |
+| 1.9     | 新增xiaobaicmd -u命令       |
+| 2.0     | 新增xiaobaicmd -m命令       |
+| 2.1     | 新增xiaobaicmd --device命令 |
```

### Comparing `xiaobaisaf-1.8/xiaobaisaf.egg-info/SOURCES.txt` & `xiaobaisaf-2.1/xiaobaisaf.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,22 +24,26 @@
 saf/example/web/Cases/test_xiaobai_case_submitBug.py
 saf/example/web/Cases/test_xiaobai_case_v1.py
 saf/example/web/Cases/test_xiaobai_case_v2.py
 saf/example/web/Cases/test_xiaobai_case_v3.py
 saf/example/web/pageObject/__init__.py
 saf/example/web/pageObject/register_page_element.py
 saf/utils/BugUtils.py
-saf/utils/PageObjectGenerator.py
+saf/utils/Demo.py
+saf/utils/MonitorAndroidDeviceGUI.py
+saf/utils/MonitorAndroidPackageCLI.py
+saf/utils/MonitorAndroidPackageGUI.py
 saf/utils/YamlUtils.py
 saf/utils/__init__.py
 saf/utils/downloadUtils.py
 saf/utils/elementUtils.py
 saf/utils/imageUtils.py
 saf/utils/networkSpeedUtils.py
 saf/utils/osEnvUtils.py
+saf/utils/selenium2POM.py
 saf/utils/sendMsgUtils.py
 saf/utils/xiaobaicmd.py
 xiaobaisaf.egg-info/PKG-INFO
 xiaobaisaf.egg-info/SOURCES.txt
 xiaobaisaf.egg-info/dependency_links.txt
 xiaobaisaf.egg-info/entry_points.txt
 xiaobaisaf.egg-info/requires.txt
```

