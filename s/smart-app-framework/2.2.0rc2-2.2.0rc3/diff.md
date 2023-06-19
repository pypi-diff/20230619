# Comparing `tmp/smart_app_framework-2.2.0rc2-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.2.0rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 307110 bytes, number of entries: 334
+Zip file size: 305757 bytes, number of entries: 333
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -219,21 +219,21 @@
 -rw-r--r--  2.0 unx      997 b- defN 80-Jan-01 00:00 smart_kit/handlers/handle_take_runtime_permissions.py
 -rw-r--r--  2.0 unx      764 b- defN 80-Jan-01 00:00 smart_kit/handlers/handler_base.py
 -rw-r--r--  2.0 unx     1429 b- defN 80-Jan-01 00:00 smart_kit/handlers/handler_run_app.py
 -rw-r--r--  2.0 unx      917 b- defN 80-Jan-01 00:00 smart_kit/handlers/handler_take_profile_data.py
 -rw-r--r--  2.0 unx     1700 b- defN 80-Jan-01 00:00 smart_kit/handlers/handler_text.py
 -rw-r--r--  2.0 unx     1631 b- defN 80-Jan-01 00:00 smart_kit/handlers/handler_timeout.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/management/__init__.py
--rw-r--r--  2.0 unx     3642 b- defN 80-Jan-01 00:00 smart_kit/management/app_manager.py
--rw-r--r--  2.0 unx     1392 b- defN 80-Jan-01 00:00 smart_kit/management/base.py
+-rw-r--r--  2.0 unx     3252 b- defN 80-Jan-01 00:00 smart_kit/management/app_manager.py
+-rw-r--r--  2.0 unx     1798 b- defN 80-Jan-01 00:00 smart_kit/management/base.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 smart_kit/management/cache.py
 -rw-r--r--  2.0 unx     3050 b- defN 80-Jan-01 00:00 smart_kit/management/get_bundles_from_pps.py
 -rw-r--r--  2.0 unx      721 b- defN 80-Jan-01 00:00 smart_kit/management/plugins.py
 -rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 smart_kit/management/smart_kit_manager.py
--rw-r--r--  2.0 unx     7748 b- defN 80-Jan-01 00:00 smart_kit/management/tests.py
+-rw-r--r--  2.0 unx     7798 b- defN 80-Jan-01 00:00 smart_kit/management/tests.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/message/__init__.py
 -rw-r--r--  2.0 unx      765 b- defN 80-Jan-01 00:00 smart_kit/message/app_info.py
 -rw-r--r--  2.0 unx      398 b- defN 80-Jan-01 00:00 smart_kit/message/as_is_to_message.py
 -rw-r--r--  2.0 unx      259 b- defN 80-Jan-01 00:00 smart_kit/message/get_to_message.py
 -rw-r--r--  2.0 unx     3105 b- defN 80-Jan-01 00:00 smart_kit/message/smartapp_to_message.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/models/__init__.py
 -rw-r--r--  2.0 unx     3369 b- defN 80-Jan-01 00:00 smart_kit/models/dialogue_manager.py
@@ -248,15 +248,14 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/start_points/__init__.py
 -rw-r--r--  2.0 unx     1198 b- defN 80-Jan-01 00:00 smart_kit/start_points/app.py
 -rw-r--r--  2.0 unx     6735 b- defN 80-Jan-01 00:00 smart_kit/start_points/base_main_loop.py
 -rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 smart_kit/start_points/constants.py
 -rw-r--r--  2.0 unx     7976 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_async_http.py
 -rw-r--r--  2.0 unx     7147 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_http.py
 -rw-r--r--  2.0 unx    36715 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_kafka.py
--rw-r--r--  2.0 unx     3833 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_parallel_kafka.py
 -rw-r--r--  2.0 unx      612 b- defN 80-Jan-01 00:00 smart_kit/start_points/postprocess.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/system_answers/__init__.py
 -rw-r--r--  2.0 unx     1005 b- defN 80-Jan-01 00:00 smart_kit/system_answers/nothing_found_action.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/template/app/__init__.py-tpl
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/template/app/adapters/__init__.py-tpl
 -rw-r--r--  2.0 unx      969 b- defN 80-Jan-01 00:00 smart_kit/template/app/adapters/db_adapters.py-tpl
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/template/app/basic_entities/__init__.py-tpl
@@ -306,15 +305,15 @@
 -rw-r--r--  2.0 unx     5686 b- defN 80-Jan-01 00:00 smart_kit/template/static/references/tests/hello_scenario_tests.json
 -rw-r--r--  2.0 unx     1838 b- defN 80-Jan-01 00:00 smart_kit/template/wsgi.py-tpl
 -rw-r--r--  2.0 unx      337 b- defN 80-Jan-01 00:00 smart_kit/template/wsgi_config.py-tpl
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/testing/__init__.py
 -rw-r--r--  2.0 unx     7833 b- defN 80-Jan-01 00:00 smart_kit/testing/local.py
 -rw-r--r--  2.0 unx     1409 b- defN 80-Jan-01 00:00 smart_kit/testing/ssml_test/ssml_string_parser.py
 -rw-r--r--  2.0 unx     4067 b- defN 80-Jan-01 00:00 smart_kit/testing/ssml_test/suite.py
--rw-r--r--  2.0 unx    13068 b- defN 80-Jan-01 00:00 smart_kit/testing/suite.py
+-rw-r--r--  2.0 unx    13126 b- defN 80-Jan-01 00:00 smart_kit/testing/suite.py
 -rw-r--r--  2.0 unx     6630 b- defN 80-Jan-01 00:00 smart_kit/testing/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/__init__.py
 -rw-r--r--  2.0 unx      607 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/base_text_normalizer.py
 -rw-r--r--  2.0 unx     3718 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/http_text_normalizer.py
 -rw-r--r--  2.0 unx     6190 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/local_text_normalizer.py
 -rw-r--r--  2.0 unx     9894 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/nltk_tokenizer_binding.py
 -rw-r--r--  2.0 unx     6126 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/pymorphy2_morph_wrapper.py
@@ -326,11 +325,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     2899 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3322 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32375 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc2.dist-info/RECORD
-334 files, 987909 bytes uncompressed, 254328 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc3.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32268 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc3.dist-info/RECORD
+333 files, 984093 bytes uncompressed, 253151 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -753,17 +753,14 @@
 
 Filename: smart_kit/start_points/main_loop_http.py
 Comment: 
 
 Filename: smart_kit/start_points/main_loop_kafka.py
 Comment: 
 
-Filename: smart_kit/start_points/main_loop_parallel_kafka.py
-Comment: 
-
 Filename: smart_kit/start_points/postprocess.py
 Comment: 
 
 Filename: smart_kit/system_answers/__init__.py
 Comment: 
 
 Filename: smart_kit/system_answers/nothing_found_action.py
@@ -987,17 +984,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc2.dist-info/METADATA
+Filename: smart_app_framework-2.2.0rc3.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc2.dist-info/WHEEL
+Filename: smart_app_framework-2.2.0rc3.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc2.dist-info/RECORD
+Filename: smart_app_framework-2.2.0rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smart_kit/management/app_manager.py

```diff
@@ -1,28 +1,17 @@
-import logging.config
 from collections import namedtuple
 
-from smart_kit.configs.logger_config import LOGGING_CONFIG
-from smart_kit.configs.logger_config import LoggerConfig
-from smart_kit.management.base import HelpCommand
+from smart_kit.management.base import HelpCommand, init_logger
 from smart_kit.management.cache import CreateCacheCommand
 from smart_kit.management.tests import TestsCommand
 from smart_kit.management.plugins import activate_plugins
 from smart_kit.start_points.app import run as app_runner
 from smart_kit.management.get_bundles_from_pps import GetBundleCommand
 
 
-def init_logger(app_config):
-    logger_config = LoggerConfig(app_config.CONFIGS_PATH)
-    logger_config.init()
-    config = logger_config[LOGGING_CONFIG]
-    logging.log_store_for_map = config.get('log_store_for_map', None)
-    logging.config.dictConfig(config)
-
-
 class AppCommand:
     @classmethod
     def doc(cls):
         return cls.__doc__ or "No help provided"
 
     def execute(self, *args, **kwargs):
         raise NotImplementedError
```

## smart_kit/management/base.py

```diff
@@ -1,7 +1,21 @@
+import logging.config
+
+from smart_kit.configs.logger_config import LOGGING_CONFIG
+from smart_kit.configs.logger_config import LoggerConfig
+
+
+def init_logger(app_config):
+    logger_config = LoggerConfig(app_config.CONFIGS_PATH)
+    logger_config.init()
+    config = logger_config[LOGGING_CONFIG]
+    logging.log_store_for_map = config.get('log_store_for_map', None)
+    logging.config.dictConfig(config)
+
+
 class AppCommand:
     @classmethod
     def doc(cls):
         return cls.__doc__ or "No help provided"
 
     def execute(self, *args, **kwargs):
         raise NotImplementedError
```

## smart_kit/management/tests.py

```diff
@@ -1,15 +1,15 @@
 import argparse
 import os
 import shutil
 import sys
 
 import smart_kit
 from core.descriptions.descriptions import Descriptions
-from smart_kit.management.base import AppCommand
+from smart_kit.management.base import AppCommand, init_logger
 from smart_kit.testing.ssml_test.suite import SsmlTestSuite
 from smart_kit.testing.suite import TestSuite
 
 
 def define_path(path):
     if os.path.exists(path):
         return path
@@ -52,14 +52,15 @@
         )
         gen_command = self.parser.add_argument_group("Generating")
         gen_command.add_argument(
             "--update", dest="update", help="Create missing template for scenarios", action="store_true",
         )
 
     def execute(self, *args, **kwargs) -> None:
+        init_logger(self.app_config)
         namespace = self.parser.parse_args(args)
         if namespace.gen:
             if not namespace.path:
                 self.parser.error("Tests generation utility require path")
             self.generate_tests_folder(namespace.path, namespace.update)
         elif namespace.run:
             if namespace.ssml_interactive:
```

## smart_kit/testing/suite.py

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 from csv import DictWriter, QUOTE_MINIMAL
 from functools import cached_property
 from typing import AnyStr, Optional, Tuple, Any, Dict, Callable
 
 from core.configs.global_constants import LINK_BEHAVIOR_FLAG
+from core.utils.utils import deep_update_dict
 from smart_kit.compatibility.commands import combine_commands
 from smart_kit.configs.settings import Settings
 from smart_kit.message.smartapp_to_message import SmartAppToMessage
 from smart_kit.models.smartapp_model import SmartAppModel
 from smart_kit.request.kafka_request import SmartKitKafkaRequest
 from smart_kit.testing.utils import Environment
 from smart_kit.utils.diff import partial_diff
@@ -294,18 +295,18 @@
     def apply_override_configs(self, override_configs):
         for repo_key, override_value in override_configs.items():
             if repo_key in self.settings.registered_repositories:
                 self._saved_configs_states[repo_key] = self.settings.registered_repositories[repo_key].data
                 if isinstance(override_value, list):
                     self.settings.registered_repositories[repo_key].data = override_value
                 elif isinstance(override_value, dict):
-                    self.settings.registered_repositories[repo_key].data = {
-                        **self._saved_configs_states[repo_key],
-                        **override_value,
-                    }
+                    self.settings.registered_repositories[repo_key].data = deep_update_dict(
+                        self._saved_configs_states[repo_key],
+                        override_value,
+                    )
                 else:
                     raise ValueError(
                         "Only list and dict types are supported for override_configs values! "
                         f"{type(override_value)=}; {override_value=}"
                     )
 
     def finalize(self):
```

## Comparing `smart_app_framework-2.2.0rc2.dist-info/METADATA` & `smart_app_framework-2.2.0rc3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.2.0rc2
+Version: 2.2.0rc3
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

## Comparing `smart_app_framework-2.2.0rc2.dist-info/RECORD` & `smart_app_framework-2.2.0rc3.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -218,21 +218,21 @@
 smart_kit/handlers/handle_take_runtime_permissions.py,sha256=0PTWl4uXh-ngWkZC0ZlTD0YZGsmITh39dc1vRshEb-s,997
 smart_kit/handlers/handler_base.py,sha256=vBZVsG0QDwm1qtKAAg4bWZfMdW-zo0StW7OteNrxAJ0,764
 smart_kit/handlers/handler_run_app.py,sha256=OIXTNrntk3y-W6j2huqrfasDQidtVSafH37ry1dpYtQ,1429
 smart_kit/handlers/handler_take_profile_data.py,sha256=9E7SbwResBG_Mmp7z07ilLovQ59_-m0xO2r4RZDQhmI,917
 smart_kit/handlers/handler_text.py,sha256=cOVGxdWVmBgHurajwBI4vFx-mfc5DN5sSP7LfkLCnPM,1700
 smart_kit/handlers/handler_timeout.py,sha256=UFanh8APLPsBp60-61SdNETK9eIYKrVgXozoZ_3iAoI,1631
 smart_kit/management/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-smart_kit/management/app_manager.py,sha256=5hYYGZ9SLsEosD61LqcC6Xyand_LgwQDdmqI0kOo23A,3642
-smart_kit/management/base.py,sha256=8GqY9vQ-19uR9SxYfc-V_wNbq-E9t18aHfgPNUptUBs,1392
+smart_kit/management/app_manager.py,sha256=VdaYCrGzl2FNJYDnnWeMAFj4wxhXRWoLbDibKMeeIYQ,3252
+smart_kit/management/base.py,sha256=MA9lxYJhpkcKw5hQfv4WkdSPok8GDMIagOg5DrLbsKY,1798
 smart_kit/management/cache.py,sha256=J73uFGk48YqaX2tTQNmBPUKOokX9PKs0ppgumD7uTXk,2550
 smart_kit/management/get_bundles_from_pps.py,sha256=wxmchkE6X9_rncLYN1EcgRXveBvGroeGJ-y-EU9crpc,3050
 smart_kit/management/plugins.py,sha256=5M-di2bkRLcWs1H2MsDv9hQPExs3BK43WkeCgEW8Juw,721
 smart_kit/management/smart_kit_manager.py,sha256=a2cK1gWrQ8GqFa4e_QdZHvoGSE2OBgeMaxM7iZQ1X3s,2072
-smart_kit/management/tests.py,sha256=wxubruqau-RfRXY6r7ZUH3oc7OFApHSQJm7YFbtg52g,7748
+smart_kit/management/tests.py,sha256=cMAuW7JQ3LsBzabhtS6jWFbFpPBYDD6K7q4M-u0qNoE,7798
 smart_kit/message/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/message/app_info.py,sha256=N35Q5NIuwi7CADWt8DqLcg97h0IVt9Up6WhQhwmdeZ4,765
 smart_kit/message/as_is_to_message.py,sha256=Nf71Oeez8ZkJHjQwTJ31-X3doj8j2XmkBQ7l4pQBHMI,398
 smart_kit/message/get_to_message.py,sha256=UzQzD7Z3FO9HHJKUzYzaXtsddfVjKKDPdI_-VUU03KM,259
 smart_kit/message/smartapp_to_message.py,sha256=8Ec7F3LcTGYEngvqwXBMjSTq60E25S2iwtoz6lZjpbo,3105
 smart_kit/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/models/dialogue_manager.py,sha256=SbZ_et_yeD9Mw_OPDE6zIfITMAkpaPBWcrir6kMHNFE,3369
@@ -247,15 +247,14 @@
 smart_kit/start_points/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/start_points/app.py,sha256=8lcZV7SiEBzFdcF7oe-54w7hmyHfK9PQ_IDa64_kVjM,1198
 smart_kit/start_points/base_main_loop.py,sha256=Kcedoy-rAhjk2HChcxb-sWY-XlE3ptMcB4VZT6HO6WY,6735
 smart_kit/start_points/constants.py,sha256=d_XQfL3YxYswZd5AFIwugqv8EimD18ZFfPRcPJpAgK0,56
 smart_kit/start_points/main_loop_async_http.py,sha256=o2tOOpkt-J0T3fJzS-cKVBqAEwEsmshWeACbudzzBfg,7976
 smart_kit/start_points/main_loop_http.py,sha256=TNNHuwrqbrg7fpLY1pY_J43dA2hbsNs-_MePOyqo_s8,7147
 smart_kit/start_points/main_loop_kafka.py,sha256=KNVMRXimJ4FY2cDMA06Y0Q6Prlba096S-Op9gU9dN4c,36715
-smart_kit/start_points/main_loop_parallel_kafka.py,sha256=rRJAFfVAHMo4v1oBvoQGs7g-AHxcadAo0vXThJIqV3s,3833
 smart_kit/start_points/postprocess.py,sha256=rUfh8Wl3rJ0Tbaoce5EtckG87_nCg5KYo8y_O2UpclQ,612
 smart_kit/system_answers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/system_answers/nothing_found_action.py,sha256=yW0_X34v4UEuPFlR2jTdBk7wJ9elSu-MezLVcNS-jJY,1005
 smart_kit/template/app/__init__.py-tpl,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/template/app/adapters/__init__.py-tpl,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/template/app/adapters/db_adapters.py-tpl,sha256=yocQSahj8Kgw2Odi9XUlO7E7Y2DXCxe1Tq6bgP2tJnQ,969
 smart_kit/template/app/basic_entities/__init__.py-tpl,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -305,15 +304,15 @@
 smart_kit/template/static/references/tests/hello_scenario_tests.json,sha256=WPZ08Jui9H5WVasMrWcgzb9ls9sv83kMj0hirxXOkcM,5686
 smart_kit/template/wsgi.py-tpl,sha256=Y5mMuIvtpPlg07HrmGotuJ5ezB7modw7T7jZamJVtko,1838
 smart_kit/template/wsgi_config.py-tpl,sha256=nQOOf4builgRYfnOo_2cCWak3hKNzjGQU5kXeAZTCzk,337
 smart_kit/testing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/testing/local.py,sha256=xCzBCEdbWVHKYKakygPdspKVKfQBwFc3FD605jeaKbo,7833
 smart_kit/testing/ssml_test/ssml_string_parser.py,sha256=Ro8UbPGsaO86RBi9EbkEf8jn3wzTVH26OHXBmdAvHSg,1409
 smart_kit/testing/ssml_test/suite.py,sha256=6-XgovyY2jlz6N0v-HwkdBMtCkvVwslFP2QEWZcyKY4,4067
-smart_kit/testing/suite.py,sha256=ktOfaQK7au_ascnkA5R_CHkCyoGba4zHx-ZihcouumY,13068
+smart_kit/testing/suite.py,sha256=9VGcT56_QwHXeiB696GgusK0K3vvGvHnxL8ibOtD4Kc,13126
 smart_kit/testing/utils.py,sha256=eQT3UXz0YSmAyGcBqinS0LMeFP_dszPNum29jfLdRDU,6630
 smart_kit/text_preprocessing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/text_preprocessing/base_text_normalizer.py,sha256=516_iatoGuJDVOJILwzuGavdLxqaGjuhAWCOxdeGwHc,607
 smart_kit/text_preprocessing/http_text_normalizer.py,sha256=D9BN7JxOXn1AepAfLOCNex4tZbsMlDBtgmW7NNpcNBA,3718
 smart_kit/text_preprocessing/local_text_normalizer.py,sha256=xuaxK0gFX6MsMdg-SREPcu5TqlkGuKvzgBp000j09B4,6190
 smart_kit/text_preprocessing/nltk_tokenizer_binding.py,sha256=pN7thYgSnks55n_44ZIcDJHxInN0QFgkH8aWT2XFHgY,9894
 smart_kit/text_preprocessing/pymorphy2_morph_wrapper.py,sha256=0SBv6IzvZT_SDiwRIroHa28d8Tdps1Kgq2q0a3-SJjo,6126
@@ -325,10 +324,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=rUdzi6f8mtXacNL6HvVYVoOnXD_M3FEMHFsMhPo0YL0,2899
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=n5N4FHjXyeZAASjVB2zhoOMsbnWiixI0OQsk4KkcDFg,3322
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.2.0rc2.dist-info/METADATA,sha256=z9izWwgeVNoE0kvQOJOmyIDrRKS5rW8TeFHl9XmL9LY,10823
-smart_app_framework-2.2.0rc2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-smart_app_framework-2.2.0rc2.dist-info/RECORD,,
+smart_app_framework-2.2.0rc3.dist-info/METADATA,sha256=ZLHaV1HPQ6OtpphFSCKhWHpmhnKmaQ3bK3DeAD_M3Q0,10823
+smart_app_framework-2.2.0rc3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.2.0rc3.dist-info/RECORD,,
```

