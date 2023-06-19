# Comparing `tmp/pytest-yaml-yoyo-1.2.6.tar.gz` & `tmp/pytest-yaml-yoyo-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.6.tar", last modified: Thu Jun  8 15:20:09 2023, max compression
+gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.7.tar", last modified: Mon Jun 19 13:56:14 2023, max compression
```

## Comparing `pytest-yaml-yoyo-1.2.6.tar` & `pytest-yaml-yoyo-1.2.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 15:20:09.360916 pytest-yaml-yoyo-1.2.6/
--rw-rw-rw-   0        0        0    25252 2023-06-08 15:20:09.359919 pytest-yaml-yoyo-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    24753 2023-06-08 15:19:36.000000 pytest-yaml-yoyo-1.2.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-08 15:20:09.360916 pytest-yaml-yoyo-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-06-08 15:20:07.000000 pytest-yaml-yoyo-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:20:09.326009 pytest-yaml-yoyo-1.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 15:20:09.349944 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/
--rw-rw-rw-   0        0        0       20 2023-06-07 14:28:14.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/create_funtion.py
--rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/db.py
--rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/exceptions.py
--rw-rw-rw-   0        0        0     4113 2023-05-30 00:16:10.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/extract.py
--rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/http_session.py
--rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/log.py
--rw-rw-rw-   0        0        0     3063 2023-06-07 14:30:58.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/my_builtins.py
--rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/parser.py
--rw-rw-rw-   0        0        0     9783 2023-06-08 07:14:20.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/plugin.py
--rw-rw-rw-   0        0        0     4690 2023-06-08 15:17:14.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/render_template_obj.py
--rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/report_notify.py
--rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/request_session.py
--rw-rw-rw-   0        0        0    28695 2023-05-30 00:24:02.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/runner.py
--rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/swagger_parser.py
--rw-rw-rw-   0        0        0     3803 2023-06-08 08:28:11.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:20:09.358924 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/
--rw-rw-rw-   0        0        0    25252 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 13:56:14.125193 pytest-yaml-yoyo-1.2.7/
+-rw-rw-rw-   0        0        0    25807 2023-06-19 13:56:14.125193 pytest-yaml-yoyo-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    25308 2023-06-19 13:56:10.000000 pytest-yaml-yoyo-1.2.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:56:14.125193 pytest-yaml-yoyo-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-06-19 13:44:52.000000 pytest-yaml-yoyo-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:56:13.955825 pytest-yaml-yoyo-1.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 13:56:14.100493 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/
+-rw-rw-rw-   0        0        0       20 2023-06-07 14:28:14.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/create_funtion.py
+-rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/db.py
+-rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/exceptions.py
+-rw-rw-rw-   0        0        0     4113 2023-05-30 00:16:10.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/extract.py
+-rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/http_session.py
+-rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/log.py
+-rw-rw-rw-   0        0        0     3063 2023-06-07 14:30:58.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/my_builtins.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/parser.py
+-rw-rw-rw-   0        0        0    10098 2023-06-19 13:47:34.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/plugin.py
+-rw-rw-rw-   0        0        0     4690 2023-06-08 15:17:14.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/render_template_obj.py
+-rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/report_notify.py
+-rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/request_session.py
+-rw-rw-rw-   0        0        0    28695 2023-05-30 00:24:02.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/runner.py
+-rw-rw-rw-   0        0        0     3524 2023-06-19 13:40:33.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/start_project.py
+-rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/swagger_parser.py
+-rw-rw-rw-   0        0        0     3803 2023-06-08 08:28:11.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:56:14.123200 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/
+-rw-rw-rw-   0        0        0    25807 2023-06-19 13:56:13.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      877 2023-06-19 13:56:13.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:56:13.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-19 13:56:13.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-06-19 13:56:13.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 13:56:13.000000 pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-yaml-yoyo-1.2.6/PKG-INFO` & `pytest-yaml-yoyo-1.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.6
+Version: 1.2.7
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -218,16 +218,20 @@
 
 v1.2.6 发布 2023-06-08
 
 优化以下问题
 
 - 1.优化断言方式 len_eq
 - 2.模板过滤器 filter 支持
-- 3.变量取值优化, 所有的取值，数字类型默认int
-- 4.取值结果数字转字符串，可以用`${str(取值表达式)} 或者过滤器方式 `${取值表达式 | str}`
+- 3.变量取值优化, 所有的取值，数字类型默认 int
+- 4.取值结果数字转字符串，可以用 `${str(取值表达式)}` 或者过滤器方式 `${取值表达式 | str}`
+
+v1.2.7 发布 2023-06-19
+
+- 1.添加 `--start-project` 命令创建项目 demo
 
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
@@ -236,19 +240,46 @@
 pip 安装插件
 
 ::
 
     pip install pytest-yaml-yoyo
 
 
+Usage / 快速创建 demo 项目
+--------------------------
+
+使用 `--start-project` 命令快速创建 demo 项目
+
+::
+
+    pytest --start-project
+
+执行后会生成如下项目结构
+
+::
+
+    D:\demo\
+    ├── case_demo/
+    │   ├── test_extract.yml
+    │   ├── test_get.yml
+    │   ├── test_post.yml
+    ├── config.py
+    ├── pytest.ini
+
+通过 pytest 命令可以执行用例
+
+::
+
+  pytest
+
 
 Usage / 第一个 hello world
 --------------------------
 
-yaml 用例编写规则，跟pytest识别默认规则一样，必须是test 开头的，以`.yml` 结尾的文件才会被识别
+yaml 用例编写规则，跟 pytest 识别默认规则一样，必须是 test 开头的，以`.yml` 结尾的文件才会被识别
 
 新建一个`test_hello.yml`文件
 
 ::
 
     config:
       name: yy
```

### Comparing `pytest-yaml-yoyo-1.2.6/README.rst` & `pytest-yaml-yoyo-1.2.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -203,16 +203,20 @@
 
 v1.2.6 发布 2023-06-08
 
 优化以下问题
 
 - 1.优化断言方式 len_eq
 - 2.模板过滤器 filter 支持
-- 3.变量取值优化, 所有的取值，数字类型默认int
-- 4.取值结果数字转字符串，可以用`${str(取值表达式)} 或者过滤器方式 `${取值表达式 | str}`
+- 3.变量取值优化, 所有的取值，数字类型默认 int
+- 4.取值结果数字转字符串，可以用 `${str(取值表达式)}` 或者过滤器方式 `${取值表达式 | str}`
+
+v1.2.7 发布 2023-06-19
+
+- 1.添加 `--start-project` 命令创建项目 demo
 
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
@@ -221,19 +225,46 @@
 pip 安装插件
 
 ::
 
     pip install pytest-yaml-yoyo
 
 
+Usage / 快速创建 demo 项目
+--------------------------
+
+使用 `--start-project` 命令快速创建 demo 项目
+
+::
+
+    pytest --start-project
+
+执行后会生成如下项目结构
+
+::
+
+    D:\demo\
+    ├── case_demo/
+    │   ├── test_extract.yml
+    │   ├── test_get.yml
+    │   ├── test_post.yml
+    ├── config.py
+    ├── pytest.ini
+
+通过 pytest 命令可以执行用例
+
+::
+
+  pytest
+
 
 Usage / 第一个 hello world
 --------------------------
 
-yaml 用例编写规则，跟pytest识别默认规则一样，必须是test 开头的，以`.yml` 结尾的文件才会被识别
+yaml 用例编写规则，跟 pytest 识别默认规则一样，必须是 test 开头的，以`.yml` 结尾的文件才会被识别
 
 新建一个`test_hello.yml`文件
 
 ::
 
     config:
       name: yy
```

### Comparing `pytest-yaml-yoyo-1.2.6/setup.py` & `pytest-yaml-yoyo-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-yaml-yoyo',
     url='https://github.com/yoyoketang/pytest-yaml-yoyo',
-    version='v1.2.6',
+    version='v1.2.7',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_yaml_yoyo"],
     classifiers=[
```

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/create_funtion.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/create_funtion.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/db.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/db.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/extract.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/extract.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/http_session.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/http_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/log.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/log.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/my_builtins.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/my_builtins.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/plugin.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .log import set_log_format
 from .report_notify import ding_ding_notify
 from .create_funtion import import_from_file
 import os
 import platform
 import time
 from . import g  # 全局 g 对象，获取项目配置
+from .start_project import create_start_project
 
 
 @pytest.fixture(scope="session")
 def requests_session(request):
     """全局session 全部用例仅执行一次"""
     s = http_session.HttpSession()
     # max_retries=2 重试2次
@@ -155,14 +156,19 @@
     # proxies_ip
     parser.addini("proxies_ip", default=None, help="proxies_ip for the  test.")
     parser.addoption(
         "--proxies-ip",
         action="store", default=None,
         help="proxies_ip for the  test.",
     )
+    # 创建 demo
+    parser.addoption(
+        "--start-project", action="store_true", help="start demo project"
+    )
+
 
 def pytest_configure(config):  # noqa
     # 配置日志文件和格式
     g['root_path'] = config.rootpath  # 项目根路径
     set_log_format(config)
     config.addinivalue_line(
         "filterwarnings", "ignore::DeprecationWarning"
@@ -216,15 +222,15 @@
     """收集测试结果"""
     total = terminalreporter._numcollected  # noqa
     if total > 0:
         passed = len([i for i in terminalreporter.stats.get('passed', []) if i.when != 'teardown'])
         failed = len([i for i in terminalreporter.stats.get('failed', []) if i.when != 'teardown'])
         error = len([i for i in terminalreporter.stats.get('error', []) if i.when != 'teardown'])
         skipped = len([i for i in terminalreporter.stats.get('skipped', []) if i.when != 'teardown'])
-        if terminalreporter._numcollected- skipped == 0:
+        if terminalreporter._numcollected - skipped == 0:  # noqa
             successful = 0
         else:
             successful = len(terminalreporter.stats.get('passed', [])) / terminalreporter._numcollected * 100  # noqa
         duration = time.time() - terminalreporter._sessionstarttime  # noqa
         markdown_text = f"""### 执行结果:
 - 运行环境: {g.get('env_name')}
 - 运行base_url: {g.get('base_url')}
@@ -242,7 +248,13 @@
             if hasattr(g["env"], 'DING_TALK'):
                 ding_talk = g["env"].DING_TALK
                 if ding_talk.get('text'):
                     ding_talk['text'] = markdown_text+ding_talk['text']
                 else:
                     ding_talk['text'] = markdown_text
                 ding_ding_notify(**ding_talk)
+
+
+def pytest_cmdline_main(config):
+    if config.option.start_project:
+        create_start_project(config)
+        return 0
```

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/render_template_obj.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/render_template_obj.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/report_notify.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/report_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/request_session.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/request_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/runner.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/swagger_parser.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/validate.py` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo/validate.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/PKG-INFO` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.6
+Version: 1.2.7
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -218,16 +218,20 @@
 
 v1.2.6 发布 2023-06-08
 
 优化以下问题
 
 - 1.优化断言方式 len_eq
 - 2.模板过滤器 filter 支持
-- 3.变量取值优化, 所有的取值，数字类型默认int
-- 4.取值结果数字转字符串，可以用`${str(取值表达式)} 或者过滤器方式 `${取值表达式 | str}`
+- 3.变量取值优化, 所有的取值，数字类型默认 int
+- 4.取值结果数字转字符串，可以用 `${str(取值表达式)}` 或者过滤器方式 `${取值表达式 | str}`
+
+v1.2.7 发布 2023-06-19
+
+- 1.添加 `--start-project` 命令创建项目 demo
 
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
@@ -236,19 +240,46 @@
 pip 安装插件
 
 ::
 
     pip install pytest-yaml-yoyo
 
 
+Usage / 快速创建 demo 项目
+--------------------------
+
+使用 `--start-project` 命令快速创建 demo 项目
+
+::
+
+    pytest --start-project
+
+执行后会生成如下项目结构
+
+::
+
+    D:\demo\
+    ├── case_demo/
+    │   ├── test_extract.yml
+    │   ├── test_get.yml
+    │   ├── test_post.yml
+    ├── config.py
+    ├── pytest.ini
+
+通过 pytest 命令可以执行用例
+
+::
+
+  pytest
+
 
 Usage / 第一个 hello world
 --------------------------
 
-yaml 用例编写规则，跟pytest识别默认规则一样，必须是test 开头的，以`.yml` 结尾的文件才会被识别
+yaml 用例编写规则，跟 pytest 识别默认规则一样，必须是 test 开头的，以`.yml` 结尾的文件才会被识别
 
 新建一个`test_hello.yml`文件
 
 ::
 
     config:
       name: yy
```

### Comparing `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/SOURCES.txt` & `pytest-yaml-yoyo-1.2.7/src/pytest_yaml_yoyo.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/pytest_yaml_yoyo/my_builtins.py
 src/pytest_yaml_yoyo/parser.py
 src/pytest_yaml_yoyo/plugin.py
 src/pytest_yaml_yoyo/render_template_obj.py
 src/pytest_yaml_yoyo/report_notify.py
 src/pytest_yaml_yoyo/request_session.py
 src/pytest_yaml_yoyo/runner.py
+src/pytest_yaml_yoyo/start_project.py
 src/pytest_yaml_yoyo/swagger_parser.py
 src/pytest_yaml_yoyo/validate.py
 src/pytest_yaml_yoyo.egg-info/PKG-INFO
 src/pytest_yaml_yoyo.egg-info/SOURCES.txt
 src/pytest_yaml_yoyo.egg-info/dependency_links.txt
 src/pytest_yaml_yoyo.egg-info/entry_points.txt
 src/pytest_yaml_yoyo.egg-info/requires.txt
```

