# Comparing `tmp/nonebot_plugin_appinsights-0.1.0.tar.gz` & `tmp/nonebot_plugin_appinsights-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_appinsights-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_appinsights-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_appinsights-0.1.0.tar` & `nonebot_plugin_appinsights-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35182 2023-04-22 07:05:38.354550 nonebot_plugin_appinsights-0.1.0/LICENSE
--rw-r--r--   0        0        0      752 2023-04-22 07:16:37.963718 nonebot_plugin_appinsights-0.1.0/nonebot_plugin_appinsights/__init__.py
--rw-r--r--   0        0        0      211 2023-04-22 06:32:07.938169 nonebot_plugin_appinsights-0.1.0/nonebot_plugin_appinsights/config.py
--rw-r--r--   0        0        0      608 2023-04-22 07:17:27.927010 nonebot_plugin_appinsights-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1372 2023-04-22 07:16:37.965665 nonebot_plugin_appinsights-0.1.0/README.md
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 nonebot_plugin_appinsights-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35182 2023-04-22 07:05:38.354550 nonebot_plugin_appinsights-0.2.0/LICENSE
+-rw-r--r--   0        0        0      896 2023-06-19 16:52:57.484717 nonebot_plugin_appinsights-0.2.0/nonebot_plugin_appinsights/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-22 06:32:07.938169 nonebot_plugin_appinsights-0.2.0/nonebot_plugin_appinsights/config.py
+-rw-r--r--   0        0        0      622 2023-06-19 17:04:41.148147 nonebot_plugin_appinsights-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1368 2023-06-19 16:54:18.838868 nonebot_plugin_appinsights-0.2.0/README.md
+-rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 nonebot_plugin_appinsights-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_appinsights-0.1.0/LICENSE` & `nonebot_plugin_appinsights-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_appinsights-0.1.0/nonebot_plugin_appinsights/__init__.py` & `nonebot_plugin_appinsights-0.2.0/nonebot_plugin_appinsights/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import nonebot
 from nonebot.log import logger
 from opencensus.ext.azure.log_exporter import AzureLogHandler
+from .config import Config
 
 from .config import Config
 
 config = Config.parse_obj(nonebot.get_driver().config)
 
 appinsights_con_str = config.applicationinsights_connection_string
 
@@ -15,9 +16,12 @@
 else:
     logger.warning("Application insights connection string is not loaded, ignore connecting.")
 
 __plugin_meta__ = nonebot.plugin.PluginMetadata(
     name='Nonebot2 AppInsights',
     description='Nonebot2 Application Insights 日志连接插件',
     usage='在.env内配置applicationinsights_connection_string以使用',
-    extra={'version': '0.1.0'}
+    type='application',
+    homepage='https://github.com/xzhouqd/nonebot-plugin-appinsights',
+    config=Config,
+    extra={'version': '0.2.0'}
 )
```

### Comparing `nonebot_plugin_appinsights-0.1.0/pyproject.toml` & `nonebot_plugin_appinsights-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "nonebot-plugin-appinsights"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["XZhouQD <X.Zhou.QD@hotmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_appinsights"}]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
-nonebot2 = "^2.0.0-beta.4"
+nonebot2 = "^2.0.0"
 opencensus-ext-azure = "^1.1.9"
+requests = "< 2.30.0"
 
 [tool.poetry.dev-dependencies]
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
 default = true
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_appinsights-0.1.0/README.md` & `nonebot_plugin_appinsights-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 <a href="https://pypi.python.org/pypi/nonebot-plugin-appinsights">
     <img src="https://img.shields.io/pypi/dm/nonebot-plugin-appinsights?style=for-the-badge" alt="pypi download">
 </a>
 <img src="https://img.shields.io/badge/require_python-3.8+-blue?style=for-the-badge" alt="python">
 <br />
 <img src="https://img.shields.io/badge/tested_python-3.10.6-blue?style=for-the-badge" alt="python">
 <img src="https://img.shields.io/badge/tested_env-go_cqhttp_1.0.0-blue?style=for-the-badge" alt="python">
-<img src="https://img.shields.io/badge/tested_Nonebot-2.0.0_rc4-red?style=for-the-badge" alt="nonebot">
+<img src="https://img.shields.io/badge/tested_Nonebot-2.0.0-red?style=for-the-badge" alt="nonebot">
 </div>
 
 ## 配置 Application Insights Connection String
 用户需在.env配置文件内通过配置项`applicationinsights_connection_string`进行配置
 ```
 applicationinsights_connection_string = "InstrumentationKey=***"
 ```
```

### Comparing `nonebot_plugin_appinsights-0.1.0/PKG-INFO` & `nonebot_plugin_appinsights-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-appinsights
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: AGPLv3
 Author: XZhouQD
 Author-email: X.Zhou.QD@hotmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: opencensus-ext-azure (>=1.1.9,<2.0.0)
+Requires-Dist: requests (<2.30.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # nonebot-plugin-appinsights
 ### Nonebot2 Application Insights 日志连接插件
 
@@ -30,15 +31,15 @@
 <a href="https://pypi.python.org/pypi/nonebot-plugin-appinsights">
     <img src="https://img.shields.io/pypi/dm/nonebot-plugin-appinsights?style=for-the-badge" alt="pypi download">
 </a>
 <img src="https://img.shields.io/badge/require_python-3.8+-blue?style=for-the-badge" alt="python">
 <br />
 <img src="https://img.shields.io/badge/tested_python-3.10.6-blue?style=for-the-badge" alt="python">
 <img src="https://img.shields.io/badge/tested_env-go_cqhttp_1.0.0-blue?style=for-the-badge" alt="python">
-<img src="https://img.shields.io/badge/tested_Nonebot-2.0.0_rc4-red?style=for-the-badge" alt="nonebot">
+<img src="https://img.shields.io/badge/tested_Nonebot-2.0.0-red?style=for-the-badge" alt="nonebot">
 </div>
 
 ## 配置 Application Insights Connection String
 用户需在.env配置文件内通过配置项`applicationinsights_connection_string`进行配置
 ```
 applicationinsights_connection_string = "InstrumentationKey=***"
 ```
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-appinsights Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-appinsights Version: 0.2.0 Summary:
 License: AGPLv3 Author: XZhouQD Author-email: X.Zhou.QD@hotmail.com Requires-
 Python: >=3.8.0,<4.0.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0)
-Requires-Dist: opencensus-ext-azure (>=1.1.9,<2.0.0) Description-Content-Type:
-text/markdown
+Language :: Python :: 3.11 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-
+Dist: opencensus-ext-azure (>=1.1.9,<2.0.0) Requires-Dist: requests (<2.30.0)
+Description-Content-Type: text/markdown
         # nonebot-plugin-appinsights ### Nonebot2 Application Insights
          æ¥å¿è¿æ¥æä»¶ [license] [pypi] [pypi_download] [python]
                           [python] [python] [nonebot]
 ## éç½® Application Insights Connection String
 ç¨æ·éå¨.envéç½®æä»¶åéè¿éç½®é¡¹`applicationinsights_connection_string`è¿è¡éç½®
 ``` applicationinsights_connection_string = "InstrumentationKey=***" ```
```

