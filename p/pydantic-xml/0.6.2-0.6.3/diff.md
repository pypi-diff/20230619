# Comparing `tmp/pydantic_xml-0.6.2.tar.gz` & `tmp/pydantic_xml-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-0.6.2.tar", max compression
+gzip compressed data, was "pydantic_xml-0.6.3.tar", max compression
```

## Comparing `pydantic_xml-0.6.2.tar` & `pydantic_xml-0.6.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1211 2023-06-10 07:20:25.015874 pydantic_xml-0.6.2/LICENSE
--rw-r--r--   0        0        0     3182 2023-06-10 07:20:25.015874 pydantic_xml-0.6.2/README.rst
--rw-r--r--   0        0        0      599 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    12576 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      364 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      569 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/errors.py
--rw-r--r--   0        0        0    11299 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/py.typed
--rw-r--r--   0        0        0       73 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0     1445 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/encoder.py
--rw-r--r--   0        0        0      342 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     4246 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     4074 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     4732 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0     6781 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     4220 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     6019 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     2933 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0     6415 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0       48 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1849 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 pydantic_xml-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-19 19:13:40.945762 pydantic_xml-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3182 2023-06-19 19:13:40.945762 pydantic_xml-0.6.3/README.rst
+-rw-r--r--   0        0        0      599 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    12576 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      364 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      569 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    11526 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       73 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0     1445 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/encoder.py
+-rw-r--r--   0        0        0      394 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     1898 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/forwardref.py
+-rw-r--r--   0        0        0     4612 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     4337 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     4732 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0     7057 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     4220 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     6555 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     3292 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0     7364 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0       48 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1849 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 pydantic_xml-0.6.3/PKG-INFO
```

### Comparing `pydantic_xml-0.6.2/LICENSE` & `pydantic_xml-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/README.rst` & `pydantic_xml-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/__init__.py` & `pydantic_xml-0.6.3/pydantic_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/element/element.py` & `pydantic_xml-0.6.3/pydantic_xml/element/element.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/element/native/lxml.py` & `pydantic_xml-0.6.3/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/element/native/std.py` & `pydantic_xml-0.6.3/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/errors.py` & `pydantic_xml-0.6.3/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/model.py` & `pydantic_xml-0.6.3/pydantic_xml/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,21 @@
     def __init_serializer__(cls) -> None:
         if config.REGISTER_NS_PREFIXES and cls.__xml_nsmap__:
             register_nsmap(cls.__xml_nsmap__)
 
         cls.__xml_serializer__ = ModelSerializerFactory.build_root(cls)
 
     @classmethod
+    def update_forward_refs(cls, **kwargs: Any) -> None:
+        super().update_forward_refs(**kwargs)
+
+        if cls.__xml_serializer__ is not None:
+            cls.__xml_serializer__.resolve_forward_refs()
+
+    @classmethod
     def from_xml_tree(cls, root: etree.Element) -> Optional['BaseXmlModel']:
         """
         Deserializes an xml element tree to an object of `cls` type.
 
         :param root: xml element to deserialize the object from
         :return: deserialized object
         """
```

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/encoder.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/encoder.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import dataclasses as dc
-from copy import deepcopy
+import typing
 from typing import Any, List, Optional, Type
 
 import pydantic as pd
 
 import pydantic_xml as pxml
 from pydantic_xml import errors
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.encoder import XmlEncoder
-from pydantic_xml.serializers.serializer import Location, PydanticShapeType, Serializer
+from pydantic_xml.serializers.serializer import Location, PydanticShapeType, Serializer, SubFieldWrapper
 from pydantic_xml.utils import QName, merge_nsmaps
 
 
 class HeterogeneousSerializerFactory:
     """
     Heterogeneous collection type serializer factory.
     """
@@ -28,32 +28,45 @@
             ns = ns or ctx.parent_ns
             nsmap = merge_nsmaps(nsmap, ctx.parent_nsmap)
 
             self._element_name = QName.from_alias(tag=name, ns=ns, nsmap=nsmap).uri
 
             self._inner_serializers = []
             for sub_field in model_field.sub_fields:
-                sub_field = deepcopy(sub_field)
-                sub_field.name = model_field.name
-                sub_field.alias = model_field.alias
-                sub_field.field_info = model_field.field_info
+                sub_field = typing.cast(
+                    pd.fields.ModelField,
+                    SubFieldWrapper(
+                        model_field.name,
+                        model_field.alias,
+                        model_field.field_info,
+                        sub_field,
+                    ),
+                )
 
                 self._inner_serializers.append(
                     self._build_field_serializer(
                         model,
                         sub_field,
                         dc.replace(
                             ctx,
                             parent_is_root=False,
                             parent_ns=ns,
                             parent_nsmap=nsmap,
                         ),
                     ),
                 )
 
+        def resolve_forward_refs(self) -> 'Serializer':
+            self._inner_serializers = [
+                serializer.resolve_forward_refs()
+                for serializer in self._inner_serializers
+            ]
+
+            return self
+
         def serialize(
                 self, element: XmlElementWriter, value: List[Any], *, encoder: XmlEncoder, skip_empty: bool = False,
         ) -> Optional[XmlElementWriter]:
             if value is None:
                 return element
 
             if skip_empty and len(value) == 0:
```

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import dataclasses as dc
-from copy import deepcopy
+import typing
 from typing import Any, List, Optional, Type
 
 import pydantic as pd
 
 import pydantic_xml as pxml
 from pydantic_xml import errors
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.encoder import XmlEncoder
-from pydantic_xml.serializers.serializer import Location, PydanticShapeType, Serializer
+from pydantic_xml.serializers.serializer import Location, PydanticShapeType, Serializer, SubFieldWrapper
 from pydantic_xml.utils import QName, merge_nsmaps
 
 
 class HomogeneousSerializerFactory:
     """
     Homogeneous collection type serializer factory.
     """
@@ -25,19 +25,23 @@
 
             name, ns, nsmap = self._get_entity_info(model_field)
             name = name or model_field.alias
             ns = ns or ctx.parent_ns
             nsmap = merge_nsmaps(nsmap, ctx.parent_nsmap)
 
             self._element_name = QName.from_alias(tag=name, ns=ns, nsmap=nsmap).uri
-
-            item_field = deepcopy(model_field.sub_fields[0])
-            item_field.name = model_field.name
-            item_field.alias = model_field.alias
-            item_field.field_info = model_field.field_info
+            item_field = typing.cast(
+                pd.fields.ModelField,
+                SubFieldWrapper(
+                    model_field.name,
+                    model_field.alias,
+                    model_field.field_info,
+                    model_field.sub_fields[0],
+                ),
+            )
 
             self._inner_serializer = self._build_field_serializer(
                 model,
                 item_field,
                 dc.replace(
                     ctx,
                     parent_is_root=False,
@@ -69,14 +73,19 @@
 
             result = []
             while (value := self._inner_serializer.deserialize(element)) is not None:
                 result.append(value)
 
             return result or None
 
+        def resolve_forward_refs(self) -> 'Serializer':
+            self._inner_serializer = self._inner_serializer.resolve_forward_refs()
+
+            return self
+
     @classmethod
     def build(
             cls,
             model: Type['pxml.BaseXmlModel'],
             model_field: pd.fields.ModelField,
             field_location: Location,
             ctx: Serializer.Context,
```

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,22 @@
             if self._is_root:
                 obj = result.get('__root__')
             else:
                 obj = result
 
             return self._model.parse_obj(obj)
 
+        def resolve_forward_refs(self) -> 'Serializer':
+            self._field_serializers = {
+                field_name: serializer.resolve_forward_refs()
+                for field_name, serializer in self._field_serializers.items()
+            }
+
+            return self
+
     class DeferredSerializer(ModelSerializer):
 
         def __init__(self, model_field: pd.fields.ModelField):
             assert is_xml_model(model_field.type_), "unexpected model field type"
             self._model: Type[pxml.BaseXmlModel] = model_field.type_
 
         @property
```

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/primitive.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/union.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from copy import deepcopy
+import typing
 from typing import Any, List, Optional, Type
 
 import pydantic as pd
 
 import pydantic_xml as pxml
 from pydantic_xml import errors
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.encoder import XmlEncoder
 from pydantic_xml.serializers.factories.model import ModelSerializerFactory
-from pydantic_xml.serializers.serializer import Location, PydanticShapeType, Serializer, is_xml_model
+from pydantic_xml.serializers.serializer import Location, PydanticShapeType, Serializer, SubFieldWrapper, is_xml_model
 
 
 class UnionSerializerFactory:
     """
     Union type serializer factory.
     """
 
@@ -21,18 +21,23 @@
                 self, model: Type['pxml.BaseXmlModel'], model_field: pd.fields.ModelField, ctx: Serializer.Context,
         ):
             assert model_field.sub_fields is not None, "unexpected model field subfields type"
             assert len(model_field.sub_fields) > 1, "unexpected model field subfields number"
 
             inner_serializers: List[Serializer] = []
             for sub_field in model_field.sub_fields:
-                sub_field = deepcopy(sub_field)
-                sub_field.name = model_field.name
-                sub_field.alias = model_field.alias
-                sub_field.field_info = model_field.field_info
+                sub_field = typing.cast(
+                    pd.fields.ModelField,
+                    SubFieldWrapper(
+                        model_field.name,
+                        model_field.alias,
+                        model_field.field_info,
+                        sub_field,
+                    ),
+                )
 
                 inner_serializers.append(self._build_field_serializer(model, sub_field, ctx))
 
             # all union types serializers must be of the same type
             if len(set(type(s) for s in inner_serializers)) > 1:
                 raise TypeError("unions of different primitive types are not supported")
 
@@ -51,18 +56,23 @@
                 self, model: Type['pxml.BaseXmlModel'], model_field: pd.fields.ModelField, ctx: Serializer.Context,
         ):
             assert model_field.sub_fields is not None, "unexpected model field subfields type"
             assert len(model_field.sub_fields) > 1, "unexpected model field subfields number"
 
             inner_serializers: List[ModelSerializerFactory.ModelSerializer] = []
             for sub_field in model_field.sub_fields:
-                sub_field = deepcopy(sub_field)
-                sub_field.name = model_field.name
-                sub_field.alias = model_field.alias
-                sub_field.field_info = model_field.field_info
+                sub_field = typing.cast(
+                    pd.fields.ModelField,
+                    SubFieldWrapper(
+                        model_field.name,
+                        model_field.alias,
+                        model_field.field_info,
+                        sub_field,
+                    ),
+                )
 
                 serializer = self._build_field_serializer(model, sub_field, ctx)
                 assert isinstance(serializer, ModelSerializerFactory.ModelSerializer), "unexpected serializer type"
 
                 inner_serializers.append(serializer)
 
             self._inner_serializers = inner_serializers
@@ -99,14 +109,22 @@
                     last_error = e
 
             if last_error is not None:
                 raise last_error
 
             return result
 
+        def resolve_forward_refs(self) -> 'Serializer':
+            self._inner_serializers = [
+                typing.cast(ModelSerializerFactory.ModelSerializer, serializer.resolve_forward_refs())
+                for serializer in self._inner_serializers
+            ]
+
+            return self
+
     @classmethod
     def build(
             cls,
             model: Type['pxml.BaseXmlModel'],
             model_field: pd.fields.ModelField,
             field_location: Location,
             ctx: Serializer.Context,
```

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import dataclasses as dc
-from copy import deepcopy
+import typing
 from typing import Any, Optional, Sized, Type
 
 import pydantic as pd
 
 import pydantic_xml as pxml
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.encoder import XmlEncoder
-from pydantic_xml.serializers.serializer import Serializer
+from pydantic_xml.serializers.serializer import Serializer, SubFieldWrapper
 from pydantic_xml.utils import QName, merge_nsmaps
 
 
 class WrappedSerializerFactory:
     """
     Wrapped serializer factory.
     """
@@ -21,22 +21,29 @@
                 self, model: Type['pxml.BaseXmlModel'], model_field: pd.fields.ModelField, ctx: Serializer.Context,
         ):
             path, ns, nsmap = self._get_entity_info(model_field)
             ns = ns or ctx.parent_ns
             self._nsmap = nsmap = merge_nsmaps(nsmap, ctx.parent_nsmap)
             self._search_mode = ctx.search_mode
 
-            model_field = deepcopy(model_field)
             field_info = model_field.field_info
 
             assert path is not None, "path is not provided"
             assert isinstance(field_info, pxml.XmlWrapperInfo), "unexpected field info type"
 
             # copy field_info from wrapped entity
-            model_field.field_info = field_info.entity or pd.fields.FieldInfo()
+            model_field = typing.cast(
+                pd.fields.ModelField,
+                SubFieldWrapper(
+                    model_field.name,
+                    model_field.alias,
+                    field_info.entity or pd.fields.FieldInfo(),
+                    model_field,
+                ),
+            )
 
             self._path = tuple(QName.from_alias(tag=part, ns=ns, nsmap=nsmap).uri for part in path.split('/'))
             self._inner_serializer = self._build_field_serializer(
                 model,
                 model_field,
                 ctx=dc.replace(
                     ctx,
@@ -65,14 +72,19 @@
         def deserialize(self, element: Optional[XmlElementReader]) -> Optional[Any]:
             if element is not None and \
                     (sub_element := element.find_sub_element(self._path, self._search_mode)) is not None:
                 return self._inner_serializer.deserialize(sub_element)
             else:
                 return None
 
+        def resolve_forward_refs(self) -> 'Serializer':
+            self._inner_serializer = self._inner_serializer.resolve_forward_refs()
+
+            return self
+
     @classmethod
     def build(
             cls,
             model: Type['pxml.BaseXmlModel'],
             model_field: pd.fields.ModelField,
             ctx: Serializer.Context,
     ) -> 'Serializer':
```

### Comparing `pydantic_xml-0.6.2/pydantic_xml/serializers/serializer.py` & `pydantic_xml-0.6.3/pydantic_xml/serializers/serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import dataclasses as dc
 import sys
 import typing
 from enum import IntEnum
 from inspect import isclass
-from typing import Any, Dict, Optional, Tuple, Type, Union
+from typing import Any, Dict, ForwardRef, Optional, Tuple, Type, Union
 
 if sys.version_info < (3, 10):
     UnionTypes = (Union,)
 else:
     from types import UnionType
     UnionTypes = (Union, UnionType)
 
@@ -18,14 +18,25 @@
 from pydantic_xml.element import SearchMode, XmlElementReader, XmlElementWriter
 from pydantic_xml.typedefs import NsMap
 
 from . import factories
 from .encoder import XmlEncoder
 
 
+class SubFieldWrapper:
+    def __init__(self, name: str, alias: str, field_info: pd.fields.FieldInfo, model_field: pd.fields.ModelField):
+        self.model_field = model_field
+        self.name = name
+        self.alias = alias
+        self.field_info = field_info
+
+    def __getattr__(self, item: str) -> Any:
+        return getattr(self.model_field, item)
+
+
 class Location(IntEnum):
     """
     Field data location.
     """
 
     MISSING = 0  # field location is not provided
     ELEMENT = 1  # field data is located at xml element
@@ -116,14 +127,23 @@
         """
         Deserializes a value from an xml element.
 
         :param element: element deserialized value should be fetched from
         :return: deserialized value
         """
 
+    def resolve_forward_refs(self) -> 'Serializer':
+        """
+        Resolve forward references if exist
+
+        :return: resolved serializer
+        """
+
+        return self
+
     @classmethod
     def _get_field_location(cls, field_info: pd.fields.FieldInfo) -> Location:
         if isinstance(field_info, pxml.XmlElementInfo):
             field_location = Location.ELEMENT
         elif isinstance(field_info, pxml.XmlAttributeInfo):
             field_location = Location.ATTRIBUTE
         elif isinstance(field_info, pxml.XmlWrapperInfo):
@@ -152,29 +172,29 @@
     @classmethod
     def _build_field_serializer(
             cls,
             model: Type['pxml.BaseXmlModel'],
             model_field: pd.fields.ModelField,
             ctx: Context,
     ) -> 'Serializer':
-        field_type = model_field.type_
-        field_info = model_field.field_info
+        if cls._has_forward_refs(model_field):
+            return factories.ForwardRefSerializerFactory.build(model, model_field, ctx)
 
         shape_type = PydanticShapeType.from_shape(model_field.shape)
         if shape_type is PydanticShapeType.UNKNOWN:
             raise TypeError(f"fields of type {model_field.type_} are not supported")
 
-        if is_xml_model(field_type):
+        if is_xml_model(model_field.type_):
             is_model_field = True
         else:
             is_model_field = False
 
         is_union_type = is_union(model_field.outer_type_) and not is_optional(model_field.outer_type_)
 
-        field_location = cls._get_field_location(field_info)
+        field_location = cls._get_field_location(model_field.field_info)
 
         if field_location is Location.WRAPPED:
             return factories.WrappedSerializerFactory.build(model, model_field, ctx)
         elif is_union_type:
             return factories.UnionSerializerFactory.build(model, model_field, field_location, ctx)
         elif shape_type is PydanticShapeType.SCALAR and not is_model_field:
             return factories.PrimitiveTypeSerializerFactory.build(model, model_field, field_location, ctx)
@@ -184,7 +204,18 @@
             return factories.MappingSerializerFactory.build(model, model_field, field_location, ctx)
         elif shape_type is PydanticShapeType.HOMOGENEOUS:
             return factories.HomogeneousSerializerFactory.build(model, model_field, field_location, ctx)
         elif shape_type is PydanticShapeType.HETEROGENEOUS:
             return factories.HeterogeneousSerializerFactory.build(model, model_field, field_location, ctx)
         else:
             raise AssertionError("unreachable")
+
+    @classmethod
+    def _has_forward_refs(cls, model_field: pd.fields.ModelField) -> bool:
+        if isinstance(model_field.type_, ForwardRef):
+            return True
+
+        for field in model_field.sub_fields or []:
+            if isinstance(field.type_, ForwardRef):
+                return True
+
+        return False
```

### Comparing `pydantic_xml-0.6.2/pydantic_xml/utils.py` & `pydantic_xml-0.6.3/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.2/pyproject.toml` & `pydantic_xml-0.6.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "0.6.2"
+version = "0.6.3"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
```

### Comparing `pydantic_xml-0.6.2/PKG-INFO` & `pydantic_xml-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 0.6.2
+Version: 0.6.3
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8,<4.0
```

