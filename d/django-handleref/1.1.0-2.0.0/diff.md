# Comparing `tmp/django-handleref-1.1.0.tar.gz` & `tmp/django-handleref-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-handleref-1.1.0.tar", max compression
+gzip compressed data, was "django-handleref-2.0.0.tar", max compression
```

## Comparing `django-handleref-1.1.0.tar` & `django-handleref-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11358 2022-11-08 11:34:24.270045 django-handleref-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3564 2022-11-08 11:34:24.270045 django-handleref-1.1.0/README.md
--rw-r--r--   0        0        0     1480 2022-11-08 11:34:49.306819 django-handleref-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-08 11:34:24.270045 django-handleref-1.1.0/src/django_handleref/__init__.py
--rw-r--r--   0        0        0    13789 2022-11-08 11:34:24.270045 django-handleref-1.1.0/src/django_handleref/admin.py
--rw-r--r--   0        0        0     2638 2022-11-08 11:34:24.270045 django-handleref-1.1.0/src/django_handleref/manager.py
--rw-r--r--   0        0        0     4313 2022-11-08 11:34:24.270045 django-handleref-1.1.0/src/django_handleref/models.py
--rw-r--r--   0        0        0        0 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/rest/__init__.py
--rw-r--r--   0        0        0      330 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/rest/serializers.py
--rw-r--r--   0        0        0     3031 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/templates/handleref/grappelli/object_history.html
--rw-r--r--   0        0        0     3580 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/templates/handleref/grappelli/version_details.html
--rw-r--r--   0        0        0     4308 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/templates/handleref/grappelli/version_revert.html
--rw-r--r--   0        0        0     3379 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/templates/handleref/grappelli/version_rollback.html
--rw-r--r--   0        0        0     2352 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/templates/handleref/object_history.html
--rw-r--r--   0        0        0     3348 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/templates/handleref/version_details.html
--rw-r--r--   0        0        0     4087 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/templates/handleref/version_revert.html
--rw-r--r--   0        0        0     3197 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/templates/handleref/version_rollback.html
--rw-r--r--   0        0        0      306 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/util.py
--rw-r--r--   0        0        0    13565 2022-11-08 11:34:24.273378 django-handleref-1.1.0/src/django_handleref/version.py
--rw-r--r--   0        0        0     4524 2022-11-08 11:35:49.796697 django-handleref-1.1.0/setup.py
--rw-r--r--   0        0        0     4355 2022-11-08 11:35:49.797642 django-handleref-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-11-08 11:34:24.270045 django-handleref-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1231 2023-06-19 11:57:34.841752 django-handleref-2.0.0/README.md
+-rw-r--r--   0        0        0     1403 2023-06-19 11:57:42.711797 django-handleref-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-08 11:34:24.270045 django-handleref-2.0.0/src/django_handleref/__init__.py
+-rw-r--r--   0        0        0    13771 2023-06-19 11:57:34.845085 django-handleref-2.0.0/src/django_handleref/admin.py
+-rw-r--r--   0        0        0     2634 2023-06-19 11:57:34.845085 django-handleref-2.0.0/src/django_handleref/manager.py
+-rw-r--r--   0        0        0     4312 2023-06-19 11:57:34.845085 django-handleref-2.0.0/src/django_handleref/models.py
+-rw-r--r--   0        0        0        0 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/rest/__init__.py
+-rw-r--r--   0        0        0      330 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/rest/serializers.py
+-rw-r--r--   0        0        0     3031 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/templates/handleref/grappelli/object_history.html
+-rw-r--r--   0        0        0     3580 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/templates/handleref/grappelli/version_details.html
+-rw-r--r--   0        0        0     4308 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/templates/handleref/grappelli/version_revert.html
+-rw-r--r--   0        0        0     3379 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/templates/handleref/grappelli/version_rollback.html
+-rw-r--r--   0        0        0     2352 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/templates/handleref/object_history.html
+-rw-r--r--   0        0        0     3348 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/templates/handleref/version_details.html
+-rw-r--r--   0        0        0     4087 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/templates/handleref/version_revert.html
+-rw-r--r--   0        0        0     3197 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/templates/handleref/version_rollback.html
+-rw-r--r--   0        0        0      306 2022-11-08 11:34:24.273378 django-handleref-2.0.0/src/django_handleref/util.py
+-rw-r--r--   0        0        0    13555 2023-06-19 11:57:34.845085 django-handleref-2.0.0/src/django_handleref/version.py
+-rw-r--r--   0        0        0     1999 2023-06-19 12:04:46.417212 django-handleref-2.0.0/setup.py
+-rw-r--r--   0        0        0     2044 2023-06-19 12:04:46.417889 django-handleref-2.0.0/PKG-INFO
```

### Comparing `django-handleref-1.1.0/LICENSE.txt` & `django-handleref-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/pyproject.toml` & `django-handleref-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 [tool.poetry]
 name = "django-handleref"
-version = "1.1.0"
+version = "2.0.0"
 description = "django object tracking"
 readme = "README.md"
 repository = "https://github.com/20c/django-handleref"
 authors = ["20C <code@20c.com>"]
 license = "Apache-2.0"
 
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Topic :: Software Development",
   "License :: OSI Approved :: Apache Software License",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
 ]
 
 packages = [{ include = "django_handleref", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 # testing
 django-reversion = ">=3"
-codecov = "*"
 pytest = ">=6.0.1"
 pytest-django = ">=3.8.0"
 pytest-cov = "*"
 pytest-pythonpath = "*"
 tox = ">=3.24"
 tox-gh-actions = ">=2.9.1"
 
 # linting
-#bandit = ">=1.6.2"
 black = { version = ">=20", allow-prereleases = true }
 isort = "^5.7.0"
 flake8 = "^3.8.4"
 mypy = ">=0.950"
 pre-commit = "^2.13"
 pyupgrade = "^2.19.4"
 
-# docs
-markdown = "*"
-markdown-include = ">=0.5,<1"
-mkdocs = "^1"
-
 # ctl
 ctl = "^1"
-jinja2 = "^2.11.2"
+jinja2 = "^3.1.2"
 tmpl = "^1"
 twine = "^3.3.0"
 
-[tool.poetry.plugins."markdown.extensions"]
-pymdgen = "pymdgen.md:Extension"
+# docs
+markdown-include = ">=0.5"
+mkdocs = "^1.2.3"
+pymdgen = "^1.0.0"
+
+[tool.poetry.extras]
+docs = ["markdown-include", "mkdocs", "pymdgen"]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `django-handleref-1.1.0/src/django_handleref/admin.py` & `django-handleref-2.0.0/src/django_handleref/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import re
 import traceback
 
 from django import forms
-from django.conf.urls import re_path
 from django.contrib import admin
 from django.contrib.admin.views.main import ChangeList
 from django.core.exceptions import ValidationError
 from django.shortcuts import redirect
 from django.template.response import TemplateResponse
+from django.urls import re_path
 from django.utils.translation import gettext_lazy as _
 
 # soft import reversion - since it is not a hard
 # requirement for django-handleref
 try:
     import reversion
 except ImportError:
@@ -119,15 +119,14 @@
         # so it's ok for now
 
         history_qset = reversion.models.Version.objects.get_for_object(instance)
         history_qset = history_qset.order_by("-revision_id")
         return history_qset
 
     def history_entry(self, version, previous):
-
         """
         Compile object history list entry dict
 
         Argument(s):
 
             - version(handleref.Version.Version): newer version
             - previous(handleref.version.Version): older version
@@ -182,15 +181,14 @@
             version = self.version_cls(_version)
             history.insert(0, self.history_entry(version, previous))
             previous = version
 
         return history
 
     def history_view(self, request, object_id):
-
         """
         object history view
         """
 
         # require superuser
 
         if not request.user.is_superuser:
@@ -221,15 +219,14 @@
             field_count=len(self.version_list_fields),
             title=_("Version History"),
         )
 
         return super().history_view(request, object_id, context)
 
     def version_details_view(self, request, object_id, version_id, extra_context=None):
-
         """
         Show version details
         """
 
         # require superuser
 
         if not request.user.is_superuser:
@@ -247,15 +244,14 @@
             previous=previous,
             changes=version.changes(previous),
         )
         context.update(extra_context or {})
         return TemplateResponse(request, self.version_details_template, context)
 
     def version_revert_view(self, request, object_id, extra_context=None):
-
         """
         Show version revert preview / confiformation view
         """
 
         # require superuser
 
         if not request.user.is_superuser:
@@ -282,15 +278,14 @@
             count=len(versions),
             changes=changes,
         )
         context.update(extra_context or {})
         return TemplateResponse(request, self.version_revert_template, context)
 
     def version_revert_process(self, request, object_id, extra_context=None):
-
         """
         Process revert version(s)
         """
 
         # require superuser
 
         if not request.user.is_superuser:
@@ -308,29 +303,26 @@
                 continue
             if not int(value):
                 continue
             field_versions[m.group(1)] = self.version_cls(int(value))
 
         errors = {}
         try:
-
             # revert
 
             reverter = self.reverter_cls()
             instance = self.model.objects.get(pk=object_id)
             reverter.revert_fields(instance, field_versions, user=request.user)
 
         except ValidationError as exc:
-
             # validation errors are collected
 
             errors = exc.message_dict
 
         except Exception as exc:
-
             # any other errors are logged
 
             errors = {"non_field_errors": ["Internal Error (check server logs)"]}
             logger.error(traceback.format_exc(exc))
 
         # if there were errors we want to show the revert preview again
         # and include error information
@@ -348,15 +340,14 @@
             "{}:{}_{}_history".format(
                 self.admin_site.name, opts.app_label, opts.model_name
             ),
             instance.id,
         )
 
     def version_rollback_view(self, request, object_id, version_id, extra_context=None):
-
         """
         Version rollback preview / confirmation view
         """
 
         # require superuser
 
         if not request.user.is_superuser:
@@ -373,43 +364,39 @@
         )
         context.update(extra_context or {})
         return TemplateResponse(request, self.version_rollback_template, context)
 
     def version_rollback_process(
         self, request, object_id, version_id, extra_context=None
     ):
-
         """
         Version rollback process
         """
 
         # require super user
 
         if not request.user.is_superuser:
             return redirect("admin:login")
 
         version = self.version_cls(int(version_id))
 
         errors = {}
         try:
-
             # rollback
 
             reverter = self.reverter_cls()
             instance = self.model.objects.get(pk=object_id)
             reverter.rollback(instance, version, user=request.user)
 
         except ValidationError as exc:
-
             # collect validation errors
 
             errors = exc.message_dict
 
         except Exception as exc:
-
             # log any other errors
 
             errors = {"non_field_errors": ["Internal Error (check server logs)"]}
             logger.error(traceback.format_exc(exc))
 
         # if there were errors show the rollback preview / confirmation
         # view again with error information
```

### Comparing `django-handleref-1.1.0/src/django_handleref/manager.py` & `django-handleref-2.0.0/src/django_handleref/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,34 +43,30 @@
 
         Either timestamp or version needs to be provided
         """
 
         qset = self
 
         if timestamp is not None:
-
             if isinstance(timestamp, numbers.Real):
                 timestamp = datetime.datetime.fromtimestamp(timestamp)
 
             qset = qset.filter(
                 models.Q(created__gt=timestamp) | models.Q(updated__gt=timestamp)
             )
 
         if version is not None:
-
             qset = qset.filter(version__gt=version)
 
         if not deleted:
-
             qset = qset.undeleted()
 
         return qset
 
     def undeleted(self):
-
         """
         Only return objects that are not soft-deleted
         """
 
         return self.exclude(status="deleted")
```

### Comparing `django-handleref-1.1.0/src/django_handleref/models.py` & `django-handleref-2.0.0/src/django_handleref/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         if not hasattr(self, "name"):
             name = self.__class__.__name__
         else:
             name = self.name
         return name + "-" + self.handle
 
     def delete(self, hard=False):
-
         """
         Override the vanilla delete functionality to soft-delete
         instead. Soft-delete is accomplished by setting the
         status field to "deleted"
 
         Arguments:
```

### Comparing `django-handleref-1.1.0/src/django_handleref/templates/handleref/grappelli/object_history.html` & `django-handleref-2.0.0/src/django_handleref/templates/handleref/grappelli/object_history.html`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/src/django_handleref/templates/handleref/grappelli/version_details.html` & `django-handleref-2.0.0/src/django_handleref/templates/handleref/grappelli/version_details.html`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/src/django_handleref/templates/handleref/grappelli/version_revert.html` & `django-handleref-2.0.0/src/django_handleref/templates/handleref/grappelli/version_revert.html`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/src/django_handleref/templates/handleref/grappelli/version_rollback.html` & `django-handleref-2.0.0/src/django_handleref/templates/handleref/grappelli/version_rollback.html`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/src/django_handleref/templates/handleref/object_history.html` & `django-handleref-2.0.0/src/django_handleref/templates/handleref/object_history.html`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/src/django_handleref/templates/handleref/version_details.html` & `django-handleref-2.0.0/src/django_handleref/templates/handleref/version_details.html`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/src/django_handleref/templates/handleref/version_revert.html` & `django-handleref-2.0.0/src/django_handleref/templates/handleref/version_revert.html`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/src/django_handleref/templates/handleref/version_rollback.html` & `django-handleref-2.0.0/src/django_handleref/templates/handleref/version_rollback.html`

 * *Files identical despite different names*

### Comparing `django-handleref-1.1.0/src/django_handleref/version.py` & `django-handleref-2.0.0/src/django_handleref/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     """
     Object version interface - extend to support
     different types of django object versioning
     solutions
     """
 
     def __init__(self, version):
-
         """
         Argument(s):
 
             - version: version object instance, for example
                 django reversion Version object
 
         """
@@ -150,15 +149,14 @@
             - Diff
 
         """
 
         return Diff(previous, self).changes
 
     def changed_fields(self, previous):
-
         """
         Return a list of changed fields between
         this version and a previous version
 
         Argument(s):
 
             - previous(Version)
@@ -329,29 +327,27 @@
     diff_ignore_fields = [
         "version",
         "created",
         "updated",
     ]
 
     def __init__(self, version_a, version_b):
-
         """
         Argument(s):
 
             - version_a(Version): older version
             - version_b(Version): newer version
 
         """
 
         self.version_a = version_a
         self.version_b = version_b
 
     @property
     def changes(self):
-
         """
         Compile and return a dict describing changes between
         the two versions tracked in this diff
 
         Returns:
 
             - dict: dict mapping field names to a dict describing
@@ -405,15 +401,14 @@
 class Reverter:
 
     """
     Allows to revert / rollback changes
     """
 
     def revert_fields(self, instance, field_versions, **kwargs):
-
         """
         Revert a set of fields
 
         Argument(s):
 
             - instance(model instance): instance of django model
               to be reverted
@@ -430,15 +425,14 @@
             setattr(instance, field, version.data[field])
             if field == "status":
                 self.validate_status_change(instance, version.data[field])
         instance.full_clean()
         instance.save()
 
     def rollback(self, instance, version, **kwargs):
-
         """
         Rollback to a specific version
 
         Argument(s):
 
             - instance(model instance): instance of django model
               to be reverted
@@ -456,15 +450,14 @@
             if field == "status":
                 self.validate_status_change(instance, value)
             setattr(instance, field, value)
         instance.full_clean()
         instance.save()
 
     def validate_status_change(self, instance, status):
-
         """
         Validate a status value change - this will make sure
         an object cannot be undeleted if a parent relationship
         is still flagged as deleted
 
         Argument(s):
 
@@ -480,15 +473,14 @@
             try:
                 relation = getattr(instance, field.name)
             except Exception:
                 continue
             self.validate_parent_status(instance, relation, status)
 
     def validate_parent_status(self, instance, parent, status):
-
         if not hasattr(parent, "HandleRef"):
             return
 
         if parent.status == "deleted" and status != "deleted":
             raise ValidationError(
                 {
                     "non_field_errors": "Parent object {} is currently flagged as deleted."
@@ -501,15 +493,14 @@
 class ReversionReverter(Reverter):
 
     """
     Reverter abstraction for django-reversion
     """
 
     def revert_fields(self, instance, field_versions, user=None):
-
         """
         Revert a set of fields
 
         Argument(s):
 
             - instance(model instance): instance of django model
               to be reverted
@@ -536,15 +527,14 @@
             version_ids = list(set(version_ids))
             reversion.set_comment(
                 "reverted some fields via versions: {}".format(", ".join(version_ids))
             )
             super().revert_fields(instance, field_versions)
 
     def rollback(self, instance, version, user=None):
-
         """
         Rollback to a specific version
 
         Argument(s):
 
             - instance(model instance): instance of django model
               to be reverted
```

