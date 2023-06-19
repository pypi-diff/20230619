# Comparing `tmp/django-grainy-1.9.1.tar.gz` & `tmp/django-grainy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-grainy-1.9.1.tar", last modified: Wed Jan  6 21:10:37 2021, max compression
+gzip compressed data, was "django-grainy-2.0.0.tar", max compression
```

## Comparing `django-grainy-1.9.1.tar` & `django-grainy-2.0.0.tar`

### file list

```diff
@@ -1,62 +1,27 @@
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.276280 django-grainy-1.9.1/
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.259614 django-grainy-1.9.1/Ctl/
--rw-rw-r--   0 dev       (1012) dev       (1012)        5 2021-01-06 21:10:36.000000 django-grainy-1.9.1/Ctl/VERSION
--rw-rw-r--   0 dev       (1012) dev       (1012)       40 2020-10-06 10:16:43.000000 django-grainy-1.9.1/Ctl/requirements-docs.txt
--rw-rw-r--   0 dev       (1012) dev       (1012)       89 2020-04-23 16:04:09.000000 django-grainy-1.9.1/Ctl/requirements-test.txt
--rw-rw-r--   0 dev       (1012) dev       (1012)       37 2021-01-06 21:09:15.000000 django-grainy-1.9.1/Ctl/requirements.txt
--rw-rw-r--   0 dev       (1012) dev       (1012)    11357 2020-04-23 16:04:09.000000 django-grainy-1.9.1/LICENSE
--rw-rw-r--   0 dev       (1012) dev       (1012)      235 2020-10-06 10:16:43.000000 django-grainy-1.9.1/MANIFEST.in
--rw-rw-r--   0 dev       (1012) dev       (1012)      608 2021-01-06 21:10:37.276280 django-grainy-1.9.1/PKG-INFO
--rw-rw-r--   0 dev       (1012) dev       (1012)      754 2020-11-19 15:42:46.000000 django-grainy-1.9.1/README.md
--rw-rw-r--   0 dev       (1012) dev       (1012)      102 2021-01-06 21:10:37.276280 django-grainy-1.9.1/setup.cfg
--rw-rw-r--   0 dev       (1012) dev       (1012)     1073 2020-11-19 15:42:46.000000 django-grainy-1.9.1/setup.py
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.256281 django-grainy-1.9.1/src/
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.269614 django-grainy-1.9.1/src/django_grainy/
--rw-rw-r--   0 dev       (1012) dev       (1012)        0 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/__init__.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     1518 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy/admin.py
--rw-rw-r--   0 dev       (1012) dev       (1012)      100 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/apps.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     1372 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/backends.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     1201 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy/conf.py
--rw-rw-r--   0 dev       (1012) dev       (1012)      414 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/const.py
--rw-rw-r--   0 dev       (1012) dev       (1012)    14673 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy/decorators.py
--rw-rw-r--   0 dev       (1012) dev       (1012)      342 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy/exceptions.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     1348 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/fields.py
--rw-rw-r--   0 dev       (1012) dev       (1012)      693 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/forms.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     2869 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy/handlers.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     3747 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/helpers.py
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.269614 django-grainy-1.9.1/src/django_grainy/migrations/
--rw-rw-r--   0 dev       (1012) dev       (1012)     2980 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1012) dev       (1012)        0 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/migrations/__init__.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     4202 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy/models.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     7532 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/remote.py
--rw-rw-r--   0 dev       (1012) dev       (1012)      942 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy/rest.py
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.256281 django-grainy-1.9.1/src/django_grainy/static/
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.269614 django-grainy-1.9.1/src/django_grainy/static/grainy/
--rw-rw-r--   0 dev       (1012) dev       (1012)     8277 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/static/grainy/grainy.js
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.256281 django-grainy-1.9.1/src/django_grainy/templates/
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.256281 django-grainy-1.9.1/src/django_grainy/templates/django_grainy/
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.256281 django-grainy-1.9.1/src/django_grainy/templates/django_grainy/forms/
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.272947 django-grainy-1.9.1/src/django_grainy/templates/django_grainy/forms/widgets/
--rw-rw-r--   0 dev       (1012) dev       (1012)      474 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/templates/django_grainy/forms/widgets/bitmask_select.html
--rw-rw-r--   0 dev       (1012) dev       (1012)       60 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/tests.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     6660 2021-01-06 21:09:15.000000 django-grainy-1.9.1/src/django_grainy/util.py
--rw-rw-r--   0 dev       (1012) dev       (1012)       63 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy/views.py
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.269614 django-grainy-1.9.1/src/django_grainy.egg-info/
--rw-rw-r--   0 dev       (1012) dev       (1012)      608 2021-01-06 21:10:37.000000 django-grainy-1.9.1/src/django_grainy.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1012) dev       (1012)     1443 2021-01-06 21:10:37.000000 django-grainy-1.9.1/src/django_grainy.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1012) dev       (1012)        1 2021-01-06 21:10:37.000000 django-grainy-1.9.1/src/django_grainy.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1012) dev       (1012)       37 2021-01-06 21:10:37.000000 django-grainy-1.9.1/src/django_grainy.egg-info/requires.txt
--rw-rw-r--   0 dev       (1012) dev       (1012)       33 2021-01-06 21:10:37.000000 django-grainy-1.9.1/src/django_grainy.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1012) dev       (1012)        1 2020-10-06 10:18:20.000000 django-grainy-1.9.1/src/django_grainy.egg-info/zip-safe
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.276280 django-grainy-1.9.1/src/django_grainy_test/
--rw-rw-r--   0 dev       (1012) dev       (1012)        0 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy_test/__init__.py
--rw-rw-r--   0 dev       (1012) dev       (1012)      196 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy_test/admin.py
--rw-rw-r--   0 dev       (1012) dev       (1012)      109 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy_test/apps.py
-drwxrwxr-x   0 dev       (1012) dev       (1012)        0 2021-01-06 21:10:37.276280 django-grainy-1.9.1/src/django_grainy_test/migrations/
--rw-rw-r--   0 dev       (1012) dev       (1012)     7363 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy_test/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1012) dev       (1012)        0 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy_test/migrations/__init__.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     1595 2020-11-19 15:42:46.000000 django-grainy-1.9.1/src/django_grainy_test/models.py
--rw-rw-r--   0 dev       (1012) dev       (1012)      394 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy_test/serializers.py
--rw-rw-r--   0 dev       (1012) dev       (1012)       60 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy_test/tests.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     1108 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy_test/urls.py
--rw-rw-r--   0 dev       (1012) dev       (1012)     3478 2020-10-06 10:16:43.000000 django-grainy-1.9.1/src/django_grainy_test/views.py
+-rw-r--r--   0        0        0    11357 2023-06-19 12:06:02.361508 django-grainy-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1118 2023-06-19 12:06:02.361508 django-grainy-2.0.0/README.md
+-rw-r--r--   0        0        0     1400 2023-06-19 12:06:57.141850 django-grainy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 12:06:02.364841 django-grainy-2.0.0/src/django_grainy/__init__.py
+-rw-r--r--   0        0        0     1534 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/admin.py
+-rw-r--r--   0        0        0      100 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/apps.py
+-rw-r--r--   0        0        0     1252 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/backends.py
+-rw-r--r--   0        0        0     1202 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/conf.py
+-rw-r--r--   0        0        0      413 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/const.py
+-rw-r--r--   0        0        0    14499 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/decorators.py
+-rw-r--r--   0        0        0      321 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/exceptions.py
+-rw-r--r--   0        0        0     1338 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/fields.py
+-rw-r--r--   0        0        0      675 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/forms.py
+-rw-r--r--   0        0        0     2855 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/handlers.py
+-rw-r--r--   0        0        0     3728 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/helpers.py
+-rw-r--r--   0        0        0     2917 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/migrations/__init__.py
+-rw-r--r--   0        0        0     4054 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/models.py
+-rw-r--r--   0        0        0     7564 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/remote.py
+-rw-r--r--   0        0        0      889 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/rest.py
+-rw-r--r--   0        0        0     8313 2023-06-19 12:06:02.368175 django-grainy-2.0.0/src/django_grainy/static/grainy/grainy.js
+-rw-r--r--   0        0        0      474 2023-06-19 12:06:02.371508 django-grainy-2.0.0/src/django_grainy/templates/django_grainy/forms/widgets/bitmask_select.html
+-rw-r--r--   0        0        0       62 2023-06-19 12:06:02.371508 django-grainy-2.0.0/src/django_grainy/tests.py
+-rw-r--r--   0        0        0     6691 2023-06-19 12:06:02.371508 django-grainy-2.0.0/src/django_grainy/util.py
+-rw-r--r--   0        0        0       26 2023-06-19 12:06:02.371508 django-grainy-2.0.0/src/django_grainy/views.py
+-rw-r--r--   0        0        0     2194 2023-06-19 12:07:23.446048 django-grainy-2.0.0/setup.py
+-rw-r--r--   0        0        0     2068 2023-06-19 12:07:23.446697 django-grainy-2.0.0/PKG-INFO
```

### Comparing `django-grainy-1.9.1/LICENSE` & `django-grainy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-grainy-1.9.1/src/django_grainy/admin.py` & `django-grainy-2.0.0/src/django_grainy/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.contrib import admin
-from django.contrib.auth.admin import UserAdmin, GroupAdmin
 from django.contrib.auth import get_user_model
+from django.contrib.auth.admin import GroupAdmin, UserAdmin
 from django.contrib.auth.models import Group
 
 from .conf import ADMIN_REMOVE_DEFAULT_FORMS
-from .models import UserPermission, GroupPermission
-from .forms import UserPermissionForm, GroupPermissionForm
+from .forms import GroupPermissionForm, UserPermissionForm
+from .models import GroupPermission, UserPermission
 
 # Register your models here.
 
 
 class UserPermissionInlineAdmin(admin.TabularInline):
     model = UserPermission
     form = UserPermissionForm
@@ -43,19 +43,19 @@
         lst.remove("user_permissions")
         info["fields"] = lst
 
 
 @admin.register(get_user_model())
 class GrainyUserAdmin(UserAdmin):
     fieldsets = _fieldsets
-    inlines = UserAdmin.inlines + [UserPermissionInlineAdmin]
+    inlines = tuple(UserAdmin.inlines) + (UserPermissionInlineAdmin,)
 
 
 _exclude = []
 if ADMIN_REMOVE_DEFAULT_FORMS:
     _exclude.append("permissions")
 
 
 @admin.register(Group)
 class GrainyGroupAdmin(GroupAdmin):
-    inlines = GroupAdmin.inlines + [GroupPermissionInlineAdmin]
+    inlines = tuple(GroupAdmin.inlines) + (GroupPermissionInlineAdmin,)
     exclude = _exclude
```

### Comparing `django-grainy-1.9.1/src/django_grainy/backends.py` & `django-grainy-2.0.0/src/django_grainy/backends.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,50 @@
 import re
-import logging
-
 
 from django.contrib.auth.backends import ModelBackend
-from django.contrib.auth import get_user_model
 
-from .helpers import (
-    django_op_to_flag,
-)
-
-from .models import (
-    namespace,
-)
-
-from .util import (
-    Permissions,
-)
+from .helpers import django_op_to_flag
+from .models import namespace
+from .util import Permissions
 
 
 class GrainyBackend(ModelBackend):
 
     """
     Authenticate actions using grainy permissions
     """
 
     def has_module_perms(self, user, obj=None):
-
         # superusers have access to everything
         if user.is_superuser:
             return True
 
         return Permissions(user).check(obj, django_op_to_flag("view"))
 
     def has_perm(self, user, perm, obj=None):
-
         # superusers have access to everything
         if user.is_superuser:
             return True
 
         ns = None
         if obj:
             try:
                 ns = namespace(obj)
-            except TypeError as inst:
+            except TypeError:
                 ns = None
 
         try:
             label, action = tuple(perm.split("."))
             a = re.match("(add|delete|change|view)_(.+)", action)
-        except ValueError as inst:
+        except ValueError:
             a = None
 
         if a:
             flag = django_op_to_flag(a.group(1))
             if not ns:
-                ns = "{}.{}".format(label, a.group(2))
+                ns = f"{label}.{a.group(2)}"
         else:
             flag = django_op_to_flag("view")
             if not ns:
                 ns = perm
 
         return Permissions(user).check(ns, flag)
```

### Comparing `django-grainy-1.9.1/src/django_grainy/conf.py` & `django-grainy-2.0.0/src/django_grainy/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import grainy.const
 from django.conf import settings
+
 from .const import PERM_CHOICES_CRUD
 
 DJANGO_OP_TO_FLAG = getattr(
     settings,
     "GRAINY_DJANGO_OP_TO_FLAG",
     {
         "add": grainy.const.PERM_CREATE,
```

### Comparing `django-grainy-1.9.1/src/django_grainy/decorators.py` & `django-grainy-2.0.0/src/django_grainy/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 import inspect
 import json
 
-from types import MethodType
-
-from django.http import HttpResponse, JsonResponse
-from django.utils.translation import ugettext_lazy as _
 from django.core.serializers.json import DjangoJSONEncoder
-
-from django.views import View
-from django.http import HttpRequest
-
+from django.http import HttpRequest, HttpResponse, JsonResponse
 from grainy.core import Namespace
 
+from .exceptions import DecoratorRequiresNamespace
 from .handlers import GrainyHandler, GrainyModelHandler
+from .helpers import dict_get_namespace, namespace, request_to_flag
 from .util import Permissions
-from .exceptions import (
-    DecoratorRequiresNamespace,
-)
-from .helpers import namespace, dict_get_namespace, request_to_flag
 
 
 class grainy_decorator:
 
     """
     base decorator that all the other grainy_* decorators
     extend from
@@ -143,15 +134,14 @@
     # a view class or function, so a manual namespace always
     # needs to be set in decorator
     require_namespace = True
 
     view = None
 
     def __call__(self, view_function):
-
         get_object = self.get_object
         apply_perms = self.apply_perms
         extra = self.extra
         permissions_cls = self.permissions_cls
         decorator = self
 
         grainy_handler = self.make_grainy_handler(view_function)
@@ -243,34 +233,35 @@
         - safe <bool>: passed to DjangoJSONEncoder
         - json_dumps_params <dict>: passed to DjangoJSONEncoder
     """
 
     def _apply_perms(self, request, data, view_function, view):
         perms = self.permissions_cls(request.user)
         try:
-            obj = self.get_object(view)
-        except AssertionError as inst:
-            obj = None
+            self.get_object(view)
+        except AssertionError:
+            pass
+
         namespace = Namespace(
             self.Grainy.namespace(**request.nsparam).replace("?", "*")
         )
 
         if isinstance(data, list):
             prefix = f"{namespace}.*"
         else:
             prefix = namespace
-        for ns, p in self.extra.get("handlers", {}).items():
+        for ns, p in list(self.extra.get("handlers", {}).items()):
             perms.applicator.handler(f"{prefix}.{ns}", **p)
 
         data, tail = namespace.container(data)
 
         data = perms.apply(data)
         try:
             return dict_get_namespace(data, namespace)
-        except KeyError as inst:
+        except KeyError:
             pass
         if isinstance(tail, list):
             return []
         else:
             return {}
 
     def apply_perms(self, request, response, view_function, view):
@@ -306,15 +297,15 @@
     """
 
     require_namespace = True
 
     def get_object(self, view):
         try:
             return super().get_object(view)
-        except AssertionError as inst:
+        except AssertionError:
             return None
 
     def apply_perms(self, request, response, view_function, view):
         response.data = self._apply_perms(request, response.data, view_function, view)
         return response
 
     def augment_request(self, request):
@@ -331,15 +322,14 @@
         decorator = self
         namespace = Namespace(
             self.Grainy.namespace(**request.nsparam).replace("?", "*")
         )
         perms = decorator.permissions_cls(request.user)
 
         def grainy_data(request, defaults):
-
             """
             Returns a cleaned up dict for request.data
 
             Any fields that are permissioned to be writeable by
             the request will have their values applied to the
             result.
 
@@ -353,15 +343,15 @@
             elif request.method == "POST":
                 op = "c"
             else:
                 return request.data
 
             data = defaults
 
-            for field, value in request.data.items():
+            for field, value in list(request.data.items()):
                 if perms.check([f"{namespace}", field], op):
                     data[field] = value
 
             return data
 
         def grainy_update_serializer(serializer_cls, instance, **kwargs):
             """
@@ -401,29 +391,28 @@
 
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
         super().__init__(*args, **kwargs)
 
     def __call__(self, view):
-
         view.Grainy = self.make_grainy_handler(view)
 
         if inspect.isclass(view):
             self.kwargs["view"] = view
             for rh in self.response_handlers:
                 if hasattr(view, rh):
                     view_function = getattr(view, rh)
                     if (
                         not hasattr(view_function, "Grainy")
                         or view_function.Grainy.view
                     ):
                         setattr(view, rh, self.decorate(view_function))
                     else:
-                        print(view_function, view_function.Grainy)
+                        print((view_function, view_function.Grainy))
             return view
         else:
             return self.decorate(view)
 
     def decorate(self, view):
         return self.decorator(*self.args, **self.kwargs)(view)
```

### Comparing `django-grainy-1.9.1/src/django_grainy/fields.py` & `django-grainy-2.0.0/src/django_grainy/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import six
-from django.db import models
 from django import forms
+from django.db import models
+
 from .conf import PERM_CHOICES
 
 
 class PermissionFormField(forms.IntegerField):
     def prepare_value(self, value):
         # if the form field is passed a bitmask we
         # need to convert it to a list, where each
```

### Comparing `django-grainy-1.9.1/src/django_grainy/forms.py` & `django-grainy-2.0.0/src/django_grainy/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from django import forms
 
-from .models import UserPermission, GroupPermission
-from .conf import (
-    PERM_CHOICES_FOR_FIELD,
-)
-from .fields import (
-    PermissionFormField,
-)
+from .conf import PERM_CHOICES_FOR_FIELD
+from .fields import PermissionFormField
+from .models import GroupPermission, UserPermission
 
 
 class BitmaskSelect(forms.widgets.CheckboxSelectMultiple):
     template_name = "django_grainy/forms/widgets/bitmask_select.html"
 
 
 class UserPermissionForm(forms.ModelForm):
```

### Comparing `django-grainy-1.9.1/src/django_grainy/handlers.py` & `django-grainy-2.0.0/src/django_grainy/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from grainy.core import PermissionSet, Namespace
+from grainy.core import Namespace
+
 
 class GrainyHandler:
     """
     The base class to use for the Grainy Meta class
     """
 
     parent = None
@@ -29,19 +30,18 @@
         if not isinstance(cls.namespace_base, Namespace):
             raise ValueError("`namespace_base` needs to be a Namespace instance")
         template = cls.namespace_instance_template
 
         if instance == "*":
             if "id" not in kwargs:
                 kwargs.update(id="*")
-            template = template.replace("{instance.","{")
+            template = template.replace("{instance.", "{")
         if kwargs.get("pk") is None:
             kwargs.update(pk=kwargs.get("id"))
 
-
         return template.format(
             namespace=str(cls.namespace_base).format(**kwargs),
             instance=instance,
             **kwargs,
         ).lower()
 
     @classmethod
```

### Comparing `django-grainy-1.9.1/src/django_grainy/helpers.py` & `django-grainy-2.0.0/src/django_grainy/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import six
 import inspect
-from grainy.core import (
-    Namespace,
-)
-from .conf import PERM_CHOICES, REQUEST_METHOD_TO_FLAG, DJANGO_OP_TO_FLAG
 
+from grainy.core import Namespace
+
+from .conf import DJANGO_OP_TO_FLAG, PERM_CHOICES, REQUEST_METHOD_TO_FLAG
 
-def namespace(target, **kwargs):
 
+def namespace(target, **kwargs):
     """
     Convert `target` to permissioning namespace
 
     Any keyword arguments will be used for formatting of the
     namespace (as applicable)
 
     Arguments:
```

### Comparing `django-grainy-1.9.1/src/django_grainy/migrations/0001_initial.py` & `django-grainy-2.0.0/src/django_grainy/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# -*- coding: utf-8 -*-
 # Generated by Django 1.11.7 on 2017-11-30 14:40
-from __future__ import unicode_literals
 
+
+import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
+
 import django_grainy.fields
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("auth", "0008_alter_user_username_max_length"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
```

### Comparing `django-grainy-1.9.1/src/django_grainy/models.py` & `django-grainy-2.0.0/src/django_grainy/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-import six
-import inspect
-
-from django.db import models
-from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group
-from django.utils.translation import ugettext_lazy as _
-
+from django.db import models
+from django.utils.translation import gettext_lazy as _
 from grainy.const import PERM_READ
-from grainy.core import PermissionSet, Namespace
+from grainy.core import PermissionSet
 
 from .fields import PermissionField
-from .conf import PERM_CHOICES
-from .helpers import namespace, int_flags
-from .handlers import GrainyHandler, GrainyModelHandler
+from .helpers import int_flags, namespace
 
 
 class PermissionQuerySet(models.QuerySet):
     """
     Queryset that offers additional utilities for UserPermission and
     GroupPermission queries
     """
@@ -53,22 +46,22 @@
             - pset <grainy.PermissionSet|dict>: if passed as `dict` permission
                 values may be passed as string flags
         """
 
         _pset = self.permission_set()
 
         if not isinstance(pset, PermissionSet) and isinstance(pset, dict):
-            pset = PermissionSet({ns: int_flags(f) for ns, f in pset.items()})
+            pset = PermissionSet({ns: int_flags(f) for ns, f in list(pset.items())})
 
-        for namespace, permission in pset.permissions.items():
-            _pset[namespace] = permission
+        for _namespace, permission in list(pset.permissions.items()):
+            _pset[_namespace] = permission
 
-        for namespace, permission in _pset.permissions.items():
-            perm = self.update_or_create(
-                namespace=namespace, defaults={"permission": permission.value}
+        for _namespace, permission in list(_pset.permissions.items()):
+            self.update_or_create(
+                namespace=_namespace, defaults={"permission": permission.value}
             )
 
     def add_permission(self, target, permission):
         """
         Add permission for the specified target
 
         Arguments:
@@ -149,10 +142,7 @@
         verbose_name_plural = _("Group Permissions")
         base_manager_name = "objects"
 
     group = models.ForeignKey(
         Group, related_name="grainy_permissions", on_delete=models.CASCADE
     )
     objects = PermissionManager()
-
-
-
```

### Comparing `django-grainy-1.9.1/src/django_grainy/remote.py` & `django-grainy-2.0.0/src/django_grainy/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,21 @@
 views.
 
 Requesting django instance can than use the remote.Permissions utility
 to request and check permissions from the provider.
 """
 import json
 
-from grainy.core import PermissionSet
+from django.core.cache import cache
 from django.http import HttpResponse, JsonResponse
 from django.views import View
-from django.core.cache import cache
-
-from grainy.core import Permission
+from grainy.core import Permission, PermissionSet
 
 import django_grainy.util
 
-from .conf import ANONYMOUS_PERMS
-
-
 # Soft requirement import of requests module
 # Error will be raised if remote Permissions
 # are instantiated and it is missing
 
 try:
     import requests
 except ImportError:
@@ -86,15 +81,17 @@
     namespace
     """
 
     def get(self, request, namespace):
         self.authenticate(request)
         as_string = bool(request.GET.get("as_string", 0))
         explicit = bool(request.GET.get("explicit", 0))
-        return HttpResponse(self.permissions.get(namespace))
+        return HttpResponse(
+            self.permissions.get(namespace), as_string=as_string, explicit=explicit
+        )
 
 
 class ProvideLoad(Provider):
 
     """
     Provide full permission set (dict)
     """
@@ -142,15 +139,14 @@
         self.loaded = False
         self.grant_all = (
             isinstance(obj, django_grainy.util.get_user_model()) and obj.is_superuser
         )
         self.cache = cache
 
     def fetch(self, url, cache_key, **params):
-
         """
         Retrieve grainy permissions from remote endpoint
 
         Arguments:
         - url (`str`)
         - cache_key (`str`)
 
@@ -216,15 +212,15 @@
 
         Returns:
         - (`int`): permission flags
         - (`str`): permission flags, if as_string=True
         """
         if self.url_load:
             self.load()
-            return super().get(*args, **kwargs)
+            return super().get(target, as_string=as_string, explicit=explicit)
         else:
             target = django_grainy.util.namespace(target)
             cache_key = f"grainy:get:{self.obj.id}:{target}"
             r = self.fetch(
                 self.url_get.format(namespace=target),
                 cache_key,
                 as_string=as_string,
```

### Comparing `django-grainy-1.9.1/src/django_grainy/rest.py` & `django-grainy-2.0.0/src/django_grainy/rest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from rest_framework.permissions import BasePermission
 
 from .helpers import request_method_to_flag
-from .util import check_permissions, namespace
-from .exceptions import PermissionDenied
+from .util import check_permissions
 
 
 class ModelViewSetPermissions(BasePermission):
 
     """
     Use as a permission class on a ModelRestViewSet
     to automatically wire up the following views
@@ -28,8 +27,7 @@
         # view has not been grainy decorated
 
         return True
 
     def has_object_permission(self, request, view, obj):
         flag = request_method_to_flag(request.method)
         return check_permissions(request.user, obj, flag)
-
```

### Comparing `django-grainy-1.9.1/src/django_grainy/static/grainy/grainy.js` & `django-grainy-2.0.0/src/django_grainy/static/grainy/grainy.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,22 +2,24 @@
 
     /* javascript implementation of grainy permissioning logic
      */
 
 
     // permission flags
 
-    GRAINY_CONST = {
+    window.GRAINY_CONST = {
         PERM_DENY: 0,
         PERM_READ: 0x01,
         PERM_UPDATE: 0x02,
         PERM_CREATE: 0x04,
         PERM_DELETE: 0x08
     }
 
+    var GRAINY_CONST = window.GRAINY_CONST;
+
 
     GRAINY_CONST.PERM_WRITE = GRAINY_CONST.PERM_UPDATE |
         GRAINY_CONST.PERM_CREATE |
         GRAINY_CONST.PERM_DELETE
 
 
     GRAINY_CONST.PERM_RW = GRAINY_CONST.PERM_READ |
@@ -340,15 +342,15 @@
          *
          * @method update_index
          * @private
          */
 
         update_index: function() {
 
-            var parent_p, branch, i, namespace, k, p, idx = {}
+            var parent_p, branch, i, namespace, idx = {}
             var value, keys, key;
 
             for (namespace in this.rules) {
                 branch = idx
                 value = this.rules[namespace]
                 parent_p = GRAINY_CONST.PERM_DENY
                 keys = this.namespace_keys(namespace)
@@ -379,15 +381,15 @@
          *
          * @method int_flags
          * @param {String} flags
          * @returns {Number}
          */
 
         int_flags: function(flags) {
-            var i, int_flag, str_flag, flag, r = 0;
+            var i, int_flag, str_flag, r = 0;
 
             if (!flags)
                 return r
 
             if (typeof flags == "number")
                 return flags
```

### Comparing `django-grainy-1.9.1/src/django_grainy/util.py` & `django-grainy-2.0.0/src/django_grainy/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from grainy.core import PermissionSet, Applicator
-
-from django.db.models import QuerySet
 from django.contrib.auth import get_user_model
-from django.contrib.auth.models import Group, AnonymousUser
+from django.contrib.auth.models import AnonymousUser, Group
+from django.db.models import QuerySet
+from grainy.core import Applicator, PermissionSet
+
+from .conf import ANONYMOUS_GROUP, ANONYMOUS_PERMS
+from .helpers import int_flags, namespace, str_flags
 
-from .helpers import namespace, int_flags, str_flags
-from .conf import ANONYMOUS_PERMS, ANONYMOUS_GROUP
 
 def check_permissions(obj, target, permissions, **kwargs):
     if not hasattr(obj, "_permissions_util"):
         obj._permissions_util = Permissions(obj)
 
     return obj._permissions_util.check(target, permissions, **kwargs)
 
 
 def get_permissions(obj, target, **kwargs):
     if not hasattr(obj, "_permissions_util"):
         obj._permissions_util = Permissions(obj)
     return obj._permissions_util.get(target, **kwargs)
 
 
-
 class Permissions:
 
     """
     A utility class that will allow you to perform permission checks
     for a user or group on cached permission sets
     """
 
@@ -40,15 +39,15 @@
             raise ValueError(
                 "`obj` needs to be have a `grainy_permissions` relationship"
             )
         self.obj = obj
         self.pset = PermissionSet()
         self.applicator = Applicator(self.pset)
         self.loaded = False
-        self.load()
+        self.load()  # lgtm[py/init-calls-subclass]
 
         self.grant_all = isinstance(obj, get_user_model()) and obj.is_superuser
 
     def load(self, refresh=False):
         """
         Loads the permission set for the user or group specified in
         `self.obj`
```

