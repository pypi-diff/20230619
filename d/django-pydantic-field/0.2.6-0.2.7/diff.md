# Comparing `tmp/django-pydantic-field-0.2.6.tar.gz` & `tmp/django-pydantic-field-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pydantic-field-0.2.6.tar", last modified: Fri Jun 16 13:07:53 2023, max compression
+gzip compressed data, was "django-pydantic-field-0.2.7.tar", last modified: Mon Jun 19 17:43:59 2023, max compression
```

## Comparing `django-pydantic-field-0.2.6.tar` & `django-pydantic-field-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:07:53.319105 django-pydantic-field-0.2.6/django_pydantic_field/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/_migration_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/django_pydantic_field/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:07:53.000000 django-pydantic-field-0.2.6/django_pydantic_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:07:53.323105 django-pydantic-field-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_base_marshalling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_django_model_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_drf_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_e2e_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_form_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-16 13:07:43.000000 django-pydantic-field-0.2.6/tests/test_sample_app_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:43:59.605579 django-pydantic-field-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-19 17:43:59.605579 django-pydantic-field-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:43:59.601579 django-pydantic-field-0.2.7/django_pydantic_field/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/_migration_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/django_pydantic_field/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:43:59.601579 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 17:43:59.000000 django-pydantic-field-0.2.7/django_pydantic_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:43:59.605579 django-pydantic-field-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:43:59.605579 django-pydantic-field-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_base_marshalling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_django_model_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_drf_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_e2e_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_form_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-19 17:43:49.000000 django-pydantic-field-0.2.7/tests/test_sample_app_migrations.py
```

### Comparing `django-pydantic-field-0.2.6/LICENSE` & `django-pydantic-field-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/PKG-INFO` & `django-pydantic-field-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.6
+Version: 0.2.7
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-pydantic-field-0.2.6/README.md` & `django-pydantic-field-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/django_pydantic_field/_migration_serializers.py` & `django-pydantic-field-0.2.7/django_pydantic_field/_migration_serializers.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/django_pydantic_field/base.py` & `django-pydantic-field-0.2.7/django_pydantic_field/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,29 @@
     exclude_fields = extractor(ctx, "exclude", None)
     if exclude_fields is not None:
         export_ctx["exclude"] = {"__root__": exclude_fields}
 
     return {k: v for k, v in export_ctx.items() if v is not None}
 
 
+def deconstruct_export_kwargs(ctx: t.Dict[str, t.Any]) -> t.Dict[str, t.Any]:
+    # We want to invert the work that was done in extract_export_kwargs
+    export_ctx = dict(ctx)
+
+    include_fields = ctx.get("include")
+    if include_fields is not None:
+        export_ctx["include"] = include_fields["__root__"]
+
+    exclude_fields = ctx.get("exclude")
+    if exclude_fields is not None:
+        export_ctx["exclude"] = exclude_fields["__root__"]
+
+    return export_ctx
+
+
 def _get_field_schema_name(schema) -> str:
     return f"FieldSchema[{display_as_type(schema)}]"
 
 
 def _get_field_schema_params(schema, config=None, allow_null=False, **kwargs) -> dict:
     root_model = t.Optional[schema] if allow_null else schema
     params: t.Dict[str, t.Any] = dict(kwargs, __root__=(root_model, ...))
```

### Comparing `django-pydantic-field-0.2.6/django_pydantic_field/fields.py` & `django-pydantic-field-0.2.7/django_pydantic_field/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,16 @@
         schema = self.schema
         if isinstance(schema, GenericTypes):
             schema = GenericContainer.from_generic(self.schema)
 
         kwargs.update(schema=schema)
 
     def _deconstruct_config(self, kwargs):
-        kwargs.update(self.export_params, config=self.config)
+        kwargs.update(base.deconstruct_export_kwargs(self.export_params))
+        kwargs.update(config=self.config)
 
 
 if t.TYPE_CHECKING:
     OptSchemaT = t.Optional[base.SchemaT]
 
 
 @t.overload
```

### Comparing `django-pydantic-field-0.2.6/django_pydantic_field/forms.py` & `django-pydantic-field-0.2.7/django_pydantic_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/django_pydantic_field/rest_framework.py` & `django-pydantic-field-0.2.7/django_pydantic_field/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/django_pydantic_field/utils.py` & `django-pydantic-field-0.2.7/django_pydantic_field/utils.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/django_pydantic_field.egg-info/PKG-INFO` & `django-pydantic-field-0.2.7/django_pydantic_field.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.6
+Version: 0.2.7
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-pydantic-field-0.2.6/django_pydantic_field.egg-info/SOURCES.txt` & `django-pydantic-field-0.2.7/django_pydantic_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/pyproject.toml` & `django-pydantic-field-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-pydantic-field"
-version = "0.2.6"
+version = "0.2.7"
 description = "Django JSONField with Pydantic models as a Schema"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Savva Surenkov", email = "savva@surenkov.space" },
 ]
```

### Comparing `django-pydantic-field-0.2.6/tests/test_base_marshalling.py` & `django-pydantic-field-0.2.7/tests/test_base_marshalling.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/tests/test_django_model_field.py` & `django-pydantic-field-0.2.7/tests/test_django_model_field.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/tests/test_drf_adapters.py` & `django-pydantic-field-0.2.7/tests/test_drf_adapters.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/tests/test_form_field.py` & `django-pydantic-field-0.2.7/tests/test_form_field.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.6/tests/test_sample_app_migrations.py` & `django-pydantic-field-0.2.7/tests/test_sample_app_migrations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from contextlib import contextmanager
 
 import pytest
 from django.core.management import call_command
 
-pytestmark = pytest.mark.django_db
+pytestmark = pytest.mark.django_db(databases="__all__")
 
 MIGRATIONS_DIR = "tests/sample_app/migrations/"
 
 
 def test_makemigrations_not_failing():
     call_command("makemigrations", "sample_app", "--noinput", "--dry-run")
 
@@ -17,15 +17,15 @@
     with clean_dir(MIGRATIONS_DIR):
         call_command("makemigrations", "sample_app", "--noinput")
         capfd.readouterr()
 
         call_command("makemigrations", "sample_app", "--noinput", "--dry-run")
         out, _ = capfd.readouterr()
 
-    assert "No changes detected in app 'sample_app'" in out
+    assert "No changes detected in app 'sample_app'" in out, out
 
 
 @contextmanager
 def clean_dir(path):
     initial_files = dir_files(path)
 
     try:
```

