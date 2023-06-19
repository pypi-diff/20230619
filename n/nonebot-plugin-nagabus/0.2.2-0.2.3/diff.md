# Comparing `tmp/nonebot_plugin_nagabus-0.2.2.tar.gz` & `tmp/nonebot_plugin_nagabus-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.2.3.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.2.2.tar` & `nonebot_plugin_nagabus-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.2/LICENSE
--rw-r--r--   0        0        0     1505 2023-06-18 15:16:39.550248 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-06-09 05:28:00.065113 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
--rw-r--r--   0        0        0     2872 2023-06-09 05:28:24.454277 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
--rw-r--r--   0        0        0     4650 2023-06-09 06:01:06.071925 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2420 2023-06-01 06:58:40.633672 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1617 2023-06-09 05:51:28.775960 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3709 2023-06-09 06:12:20.123461 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0      436 2023-06-09 05:28:00.075631 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/errors.py
--rw-r--r--   0        0        0     3415 2023-06-09 15:01:04.190237 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1248 2023-06-09 15:00:22.460735 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    21192 2023-06-09 14:41:10.459561 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0      347 2023-06-09 05:53:37.650409 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      997 2023-06-18 15:16:39.541668 nonebot_plugin_nagabus-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.2/README.md
--rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1379 2023-06-19 13:37:42.959252 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1364 2023-06-19 13:36:03.851200 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-06-09 05:28:00.065113 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      715 2023-06-19 13:36:03.860199 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-09 05:28:24.454277 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0     4650 2023-06-09 06:01:06.071925 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2420 2023-06-01 06:58:40.633672 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1617 2023-06-09 05:51:28.775960 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-19 13:36:03.827200 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3709 2023-06-09 06:12:20.123461 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0      436 2023-06-09 05:28:00.075631 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/errors.py
+-rw-r--r--   0        0        0     3415 2023-06-09 15:01:04.190237 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1248 2023-06-09 15:00:22.460735 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    21194 2023-06-19 13:36:03.846202 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0      347 2023-06-09 05:53:37.650409 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      997 2023-06-19 13:38:34.784589 nonebot_plugin_nagabus-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.3/README.md
+-rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.2.2/LICENSE` & `nonebot_plugin_nagabus-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,50 +2,49 @@
 nonebot-plugin-nagabus
 
 @Author         : ssttkkl
 @License        : AGPLv3
 @GitHub         : https://github.com/ssttkkl/nonebot-plugin-nagabus
 """
 
-from .errors import ConfigError
+from nonebot import require, logger
+from nonebot.plugin import PluginMetadata
 
-try:
-    from .config import Config
-    from .utils.nonebot import default_cmd_start
+from .errors import ConfigError
 
-    __usage__ = f"""
-    牌谱分析：
-    {default_cmd_start}naga <雀魂牌谱链接> <东/南x局x本场>：消耗10NP解析雀魂小局
-    {default_cmd_start}naga <天凤牌谱链接>：消耗50NP解析天凤半庄
-    
-    使用情况：
-    {default_cmd_start}naga本月使用情况
-    {default_cmd_start}naga上月使用情况
-    
-    以上命令格式中，以<>包裹的表示一个参数。
-    
-    详细说明：参见https://github.com/ssttkkl/nonebot-plugin-nagabus
-    """.strip()
-
-    from nonebot.plugin import PluginMetadata
-
-    __plugin_meta__ = PluginMetadata(
-        name='NAGA公交车',
-        description='为群友提供NAGA拼车服务',
-        usage=__usage__,
-        type="application",
-        homepage="https://github.com/ssttkkl/nonebot-plugin-nagabus",
-        config=Config
-    )
-
-    from nonebot import logger, require
-
-    require("nonebot_plugin_access_control")
-    require("nonebot_plugin_datastore")
-    require("nonebot_plugin_get_nickname")
-    require("nonebot_plugin_majsoul")
-    require("nonebot_plugin_saa")
-    require("nonebot_plugin_session")
+require("nonebot_plugin_access_control")
+require("nonebot_plugin_datastore")
+require("nonebot_plugin_get_nickname")
+require("nonebot_plugin_majsoul")
+require("nonebot_plugin_saa")
+require("nonebot_plugin_session")
+
+from .config import Config
+from .utils.nonebot import default_cmd_start
+
+__usage__ = f"""
+牌谱分析：
+{default_cmd_start}naga <雀魂牌谱链接> <东/南x局x本场>：消耗10NP解析雀魂小局
+{default_cmd_start}naga <天凤牌谱链接>：消耗50NP解析天凤半庄
+
+使用情况：
+{default_cmd_start}naga本月使用情况
+{default_cmd_start}naga上月使用情况
+
+以上命令格式中，以<>包裹的表示一个参数。
+
+详细说明：参见https://github.com/ssttkkl/nonebot-plugin-nagabus
+""".strip()
+
+__plugin_meta__ = PluginMetadata(
+    name='NAGA公交车',
+    description='为群友提供NAGA拼车服务',
+    usage=__usage__,
+    type="application",
+    homepage="https://github.com/ssttkkl/nonebot-plugin-nagabus",
+    config=Config
+)
 
+try:
     from . import matchers
 except ConfigError as e:
     logger.exception(e)
```

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,23 @@
 
         return values
 
     class Config:
         extra = "ignore"
 
 
-try:
-    conf = Config(**get_driver().config.dict())
-except ValidationError as e:
-    for err in e.errors():
-        if err["loc"] == ("naga_cookies",) and err["type"] == "value_error.missing":
-            raise ConfigError("Please configure naga_cookies in your .env file!") from e
-    else:
-        raise e
+_conf = None
+
+
+def conf() -> Config:
+    global _conf
+    if _conf is None:
+        try:
+            _conf = Config(**get_driver().config.dict())
+        except ValidationError as e:
+            for err in e.errors():
+                if err["loc"] == ("naga_cookies",) and err["type"] == "value_error.missing":
+                    raise ConfigError("Please configure naga_cookies in your .env file!") from e
+            else:
+                raise e
+
+    return _conf
```

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ...config import conf
 
-dialect = conf.datastore_database_dialect
+dialect = conf().datastore_database_dialect
 if dialect == 'sqlite':
     from sqlalchemy.dialects.sqlite import insert as _insert
     from sqlalchemy.dialects.sqlite import JSON as _JSON
     from sqlalchemy.dialects.sqlite import BLOB as _BLOB
 elif dialect == 'postgresql':
     from sqlalchemy.dialects.postgresql import insert as _insert
     from sqlalchemy.dialects.postgresql import JSONB as _JSON
```

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/naga/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             self._refresh_worker = asyncio.create_task(self._refresh())
 
 
 class NagaService:
     _tenhou_haihu_id_reg = re.compile(r"^20\d{8}gm-[a-f\d]{4}-[a-z\d]{4,5}-[a-zA-Z\d]{8}$")
 
     def __init__(self, cookies: Dict[str, str], timeout: float = 90.0):
-        if conf.naga_fake_api:
+        if conf().naga_fake_api:
             self.api = FakeNagaApi()
             logger.warning("using fake naga api")
         else:
             self.api = NagaApi(cookies)
 
         self._majsoul_order_mutex = Lock()
         self._tenhou_order_mutex = Lock()
```

### Comparing `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.2.3/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/pyproject.toml` & `nonebot_plugin_nagabus-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.2.2/README.md` & `nonebot_plugin_nagabus-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.2/PKG-INFO` & `nonebot_plugin_nagabus-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

