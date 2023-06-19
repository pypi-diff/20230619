# Comparing `tmp/nqgreenapi-1.0.0a2.tar.gz` & `tmp/nqgreenapi-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nqgreenapi-1.0.0a2.tar", max compression
+gzip compressed data, was "nqgreenapi-1.0.0a3.tar", max compression
```

## Comparing `nqgreenapi-1.0.0a2.tar` & `nqgreenapi-1.0.0a3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      557 2023-05-15 11:41:54.752522 nqgreenapi-1.0.0a2/LICENSE
--rw-r--r--   0        0        0      348 2023-05-15 11:41:54.752522 nqgreenapi-1.0.0a2/README.md
--rw-r--r--   0        0        0      661 2023-05-20 13:59:37.932301 nqgreenapi-1.0.0a2/nqgreenapi/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-18 17:50:08.352808 nqgreenapi-1.0.0a2/nqgreenapi/callback.py
--rw-r--r--   0        0        0     1715 2023-05-18 09:21:41.441545 nqgreenapi-1.0.0a2/nqgreenapi/message.py
--rw-r--r--   0        0        0     4134 2023-05-30 13:56:48.628132 nqgreenapi-1.0.0a2/nqgreenapi/provider.py
--rw-r--r--   0        0        0      580 2023-05-15 11:41:54.756522 nqgreenapi-1.0.0a2/nqgreenapi/quotas.py
--rw-r--r--   0        0        0      331 2023-05-15 11:41:54.756522 nqgreenapi-1.0.0a2/nqgreenapi/resources/config_schema.json
--rw-r--r--   0        0        0      918 2023-05-18 09:21:41.441545 nqgreenapi-1.0.0a2/nqgreenapi/serializers.py
--rw-r--r--   0        0        0      854 2023-05-18 14:20:08.482922 nqgreenapi-1.0.0a2/nqgreenapi/utils.py
--rw-r--r--   0        0        0     1749 2023-05-30 14:03:18.825379 nqgreenapi-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 nqgreenapi-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-05-15 11:41:54.752522 nqgreenapi-1.0.0a3/LICENSE
+-rw-r--r--   0        0        0      358 2023-06-19 11:01:49.933710 nqgreenapi-1.0.0a3/README.md
+-rw-r--r--   0        0        0      661 2023-05-20 13:59:37.932301 nqgreenapi-1.0.0a3/nqgreenapi/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-18 17:50:08.352808 nqgreenapi-1.0.0a3/nqgreenapi/callback.py
+-rw-r--r--   0        0        0     1715 2023-05-18 09:21:41.441545 nqgreenapi-1.0.0a3/nqgreenapi/message.py
+-rw-r--r--   0        0        0     5093 2023-06-19 11:01:49.945710 nqgreenapi-1.0.0a3/nqgreenapi/provider.py
+-rw-r--r--   0        0        0      580 2023-05-15 11:41:54.756522 nqgreenapi-1.0.0a3/nqgreenapi/quotas.py
+-rw-r--r--   0        0        0      331 2023-05-15 11:41:54.756522 nqgreenapi-1.0.0a3/nqgreenapi/resources/config_schema.json
+-rw-r--r--   0        0        0     1380 2023-06-19 11:01:49.945710 nqgreenapi-1.0.0a3/nqgreenapi/serializers.py
+-rw-r--r--   0        0        0      854 2023-05-18 14:20:08.482922 nqgreenapi-1.0.0a3/nqgreenapi/utils.py
+-rw-r--r--   0        0        0     1759 2023-06-19 11:38:45.950126 nqgreenapi-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 nqgreenapi-1.0.0a3/PKG-INFO
```

### Comparing `nqgreenapi-1.0.0a2/LICENSE` & `nqgreenapi-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a2/nqgreenapi/__init__.py` & `nqgreenapi-1.0.0a3/nqgreenapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a2/nqgreenapi/callback.py` & `nqgreenapi-1.0.0a3/nqgreenapi/callback.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a2/nqgreenapi/message.py` & `nqgreenapi-1.0.0a3/nqgreenapi/message.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a2/nqgreenapi/provider.py` & `nqgreenapi-1.0.0a3/nqgreenapi/provider.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,56 +21,80 @@
 
 import pytz
 from pydantic import ValidationError
 from rest_framework.status import HTTP_204_NO_CONTENT
 from whatsapp_api_client_python import API
 
 from nqsdk.abstract.channel import Channel
-from nqsdk.abstract.provider import Provider, StaticCallbackHandleMixin
-from nqsdk.enums import CallbackEvent, CallbackStatus
+from nqsdk.abstract.provider import HealthCheckMixin, Provider, StaticCallbackHandleMixin
+from nqsdk.enums import CallbackEvent, CallbackStatus, CallbackUrl
 from nqsdk.exceptions import (
     CallbackHandlingException,
     SentException,
     UnsupportedCallbackEventException,
 )
 
 from .callback import GreenApiCallbackResponse
 from .message import GreenApiExtIdCallbackMeta, GreenApiSentMeta
-from .serializers import OutgoingMessageStatusModel
+from .serializers import (
+    InstanceState,
+    InstanceStateModel,
+    InstanceStatus,
+    InstanceStatusModel,
+    MessageStatus,
+    OutgoingMessageStatusModel,
+)
 from .utils import flatten_errors
 
 if TYPE_CHECKING:  # pragma: no cover
     from rest_framework.request import Request
 
     from nqsdk.abstract.message import Message
 
     from .callback import CallbackResponse
     from .message import ExtIdCallbackMeta
 
 
-class GreenApiProvider(StaticCallbackHandleMixin, Provider):
+class GreenApiProvider(StaticCallbackHandleMixin, HealthCheckMixin, Provider):
     label = "Green Api provider"
 
     WEBHOOK_TYPE_MAP = {"outgoingMessageStatus": "outgoing_message_status"}
 
+    def __init__(self, *, config: dict, callback_urls: dict[CallbackUrl | str, str]):
+        super().__init__(config=config, callback_urls=callback_urls)
+        self._green_api = API.GreenApi(
+            self.config["id_instance"], self.config["api_token_instance"]
+        )
+
     @classmethod
     def get_config_schema(cls) -> dict:
         return json.loads(
             resources.files("nqgreenapi").joinpath("resources/config_schema.json").read_text()
         )
 
     @classmethod
     def get_channels(cls) -> list[type[Channel]]:
         return [Channel.create(label="whatsapp", is_ack_supported=True, is_delivery_supported=True)]
 
-    def send(self, *, message: Message) -> GreenApiSentMeta:
-        green_api = API.GreenApi(self.config["id_instance"], self.config["api_token_instance"])
+    def check_health(self) -> bool:
+        """Checks provider health."""
+
+        state_model = InstanceStateModel(**self._green_api.account.getStateInstance().data)
+        status_model = InstanceStatusModel(**self._green_api.account.getStatusInstance().data)
 
-        result = green_api.sending.sendMessage(
-            chatId=f"{message.get_recipient_id()}@c.us", message=message.get_content()
+        return (
+            state_model.stateInstance == InstanceState.authorized
+            and status_model.statusInstance == InstanceStatus.online
+        )
+
+    def send(self, *, message: Message) -> GreenApiSentMeta:
+        result = self._green_api.sending.sendMessage(
+            chatId=f"{message.get_recipient_id()}@c.us",
+            message=message.get_content(),
+            linkPreview=False,
         )
 
         if result.error:
             raise SentException(result.error)
 
         return GreenApiSentMeta(
             attempt_uid=message.attempt_uid,
@@ -97,18 +121,21 @@
         except ValidationError as e:
             raise CallbackHandlingException(
                 response=GreenApiCallbackResponse(
                     status=CallbackStatus.FAILED, error=flatten_errors(e.errors())
                 )
             )
 
+        if not model.sendByApi:
+            raise UnsupportedCallbackEventException(code=HTTP_204_NO_CONTENT)
+
         status = model.status
-        if status == "delivered":
+        if status == MessageStatus.delivered:
             event = CallbackEvent.DELIVERY
-        elif status == "read":
+        elif status == MessageStatus.read:
             event = CallbackEvent.ACK
         else:
             raise UnsupportedCallbackEventException(code=HTTP_204_NO_CONTENT)
 
         ext_id = model.idMessage
         dt_updated = datetime.fromtimestamp(model.timestamp, tz=pytz.UTC)
```

### Comparing `nqgreenapi-1.0.0a2/nqgreenapi/quotas.py` & `nqgreenapi-1.0.0a3/nqgreenapi/quotas.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a2/nqgreenapi/serializers.py` & `nqgreenapi-1.0.0a3/nqgreenapi/serializers.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,20 +13,43 @@
 # limitations under the License.
 
 from enum import Enum
 
 from pydantic import BaseModel
 
 
-class StatusEnum(str, Enum):
+class MessageStatus(str, Enum):
     sent = "sent"
     delivered = "delivered"
     read = "read"
     failed = "failed"
     noAccount = "noAccount"
     notInGroup = "notInGroup"
 
 
+class InstanceState(str, Enum):
+    notAuthorized = "notAuthorized"
+    authorized = "authorized"
+    blocked = "blocked"
+    sleepMode = "sleepMode"
+    starting = "starting"
+    yellowCard = "yellowCard"
+
+
+class InstanceStatus(str, Enum):
+    online = "online"
+    offline = "offline"
+
+
 class OutgoingMessageStatusModel(BaseModel):
     timestamp: int
-    status: StatusEnum
+    status: MessageStatus
     idMessage: str
+    sendByApi: bool
+
+
+class InstanceStateModel(BaseModel):
+    stateInstance: InstanceState
+
+
+class InstanceStatusModel(BaseModel):
+    statusInstance: InstanceStatus
```

### Comparing `nqgreenapi-1.0.0a2/nqgreenapi/utils.py` & `nqgreenapi-1.0.0a3/nqgreenapi/utils.py`

 * *Files identical despite different names*

### Comparing `nqgreenapi-1.0.0a2/pyproject.toml` & `nqgreenapi-1.0.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "poetry_core >= 1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nqgreenapi"
-version = "1.0.0-alpha-2"
-description = "NqGreenApi"
+version = "1.0.0-alpha-3"
+description = "NQ GreenApi Provider"
 authors = [ "Inqana Ltd. <develop@inqana.com>",]
 readme = "README.md"
 classifiers = [ "Development Status :: 3 - Alpha", "Intended Audience :: Developers", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 
 [tool.setuptools]
 zip-safe = true
 include-package-data = true
```

### Comparing `nqgreenapi-1.0.0a2/PKG-INFO` & `nqgreenapi-1.0.0a3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nqgreenapi
-Version: 1.0.0a2
-Summary: NqGreenApi
+Version: 1.0.0a3
+Summary: NQ GreenApi Provider
 Author: Inqana Ltd.
 Author-email: develop@inqana.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nqsdk (==1.0.0a16)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: whatsapp-api-client-python
 Description-Content-Type: text/markdown
 
-# NqGreenApi
+# NQ GreenApi Provider
 
 Part of NQ suite by [Inqana](https://inqana.com). Built with [NQ SDK](https://pypi.org/project/nqsdk/).
 
 ## Tests
 
 Run tests locally:
```

