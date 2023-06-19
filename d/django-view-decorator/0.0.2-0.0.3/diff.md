# Comparing `tmp/django_view_decorator-0.0.2.tar.gz` & `tmp/django_view_decorator-0.0.3.tar.gz`

## Comparing `django_view_decorator-0.0.2.tar` & `django_view_decorator-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/__about__.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/__init__.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/apps.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/conf.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/decorators.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/urls.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/urls_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/management/commands/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/django_view_decorator/management/commands/list_views.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/README.md
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 django_view_decorator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/__about__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/__init__.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/apps.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/conf.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/decorators.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/urls.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/urls_utils.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/django_view_decorator/management/commands/list_views.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/README.md
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 django_view_decorator-0.0.3/PKG-INFO
```

### Comparing `django_view_decorator-0.0.2/django_view_decorator/apps.py` & `django_view_decorator-0.0.3/django_view_decorator/apps.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from typing import TypeVarTuple
 else:
     from typing_extensions import TypeVarTuple
 
 from django.apps import AppConfig
 from django.http import HttpRequest
 from django.http import HttpResponse
-from django.urls import path, URLPattern, include
+from django.urls import path, URLResolver, include, URLPattern
 
 from .conf import conf
 
 
 ViewType: TypeAlias = Callable[[HttpRequest, TypeVarTuple], HttpResponse]
 
 
@@ -40,16 +40,16 @@
         namespace: str | None = None,
     ) -> None:
         cls.views.setdefault(namespace, defaultdict(list))[name].append(
             View(paths=paths, view=view_func),
         )
 
     @classmethod
-    def urlpatterns(cls) -> list[URLPattern]:
-        urlpatterns = []
+    def urlpatterns(cls) -> list[URLPattern | URLResolver]:
+        urlpatterns: list[URLPattern | URLResolver] = []
         for namespace, views in cls.views.items():
             _patterns = []
             for name, _views in views.items():
                 for _view in _views:
                     if isinstance(_view.paths, str):
                         _patterns.append(
                             path(_view.paths, _view.view, name=name),
@@ -75,9 +75,9 @@
     verbose_name = "Django View Decorator"
 
     def ready(self) -> None:
         if conf.DJANGO_VIEW_DECORATOR_AUTODISCOVER_VIEWS:
             from django.utils.module_loading import autodiscover_modules
 
             autodiscover_modules(
-                conf.DJANGO_VIEW_DECORATOR_AUTODISCOVER_MODULE
+                conf.DJANGO_VIEW_DECORATOR_AUTODISCOVER_MODULE,
             )
```

### Comparing `django_view_decorator-0.0.2/django_view_decorator/decorators.py` & `django_view_decorator-0.0.3/django_view_decorator/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     :param login_required: Whether the view requires the user to be logged in.
     :param staff_required: Whether the view requires the user to be staff.
     :param permissions: List of permissions required for the view.
     """
     from django.contrib.auth.views import redirect_to_login
 
     def decorator(
-        view_func: Callable[[HttpRequest], HttpResponse],
+        view_func: Callable[[HttpRequest], HttpResponse] | type[View],
     ) -> Callable[[HttpRequest], HttpResponse]:
         @wraps(view_func)
         def wrapper(
             request: HttpRequest,
             *args: TypeVarTuple,
             **kwargs: Any,
         ) -> HttpResponse:
@@ -60,16 +60,14 @@
             if staff_required and not request.user.is_staff:
                 return HttpResponseForbidden()
 
             if permissions and not request.user.has_perms(permissions):
                 return HttpResponseForbidden()
 
             if isinstance(view_func, type) and issubclass(view_func, View):
-                print(args)
-                print(kwargs)
                 return view_func.as_view()(request, *args, **kwargs)
 
             return view_func(request, *args, **kwargs)
 
         ViewRegistry.register(
             name=name,
             paths=paths,
@@ -78,34 +76,40 @@
         )
 
         return wrapper
 
     return decorator
 
 
-def namespaced_decorator_factory(*, namespace: str | None = None) -> Callable:
+def namespaced_decorator_factory(
+    *,
+    namespace: str | None = None,
+    base_path: str | None = None,
+) -> Callable:
     """
     Decorator factory to create namespaced view decorators.
 
     :param namespace: Namespace of the view decorator.
     """
 
     def decorator(
         paths: str | list[str],
         name: str,
-        login_required: bool = False,
-        staff_required: bool = False,
-        permissions: str | list[str] | None = None,
+        **kwargs,
     ) -> Callable[
         [Callable[[HttpRequest], HttpResponse]],
         Callable[[HttpRequest], HttpResponse],
     ]:
+        if base_path:
+            if isinstance(paths, str):
+                paths = [paths]
+
+            paths = list(map(lambda path: f"{base_path}/{path}", paths))
+
         return view(
             paths=paths,
             name=name,
             namespace=namespace,
-            login_required=login_required,
-            staff_required=staff_required,
-            permissions=permissions,
+            **kwargs,
         )
 
     return decorator
```

### Comparing `django_view_decorator-0.0.2/django_view_decorator/urls_utils.py` & `django_view_decorator-0.0.3/django_view_decorator/urls_utils.py`

 * *Files identical despite different names*

### Comparing `django_view_decorator-0.0.2/django_view_decorator/management/commands/list_views.py` & `django_view_decorator-0.0.3/django_view_decorator/management/commands/list_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from django.core.management.base import BaseCommand
 
 from django_view_decorator.apps import ViewRegistry
 
 
-
 class Command(BaseCommand):
     help = "List all views in the project."
 
     def handle(self, *args, **options):
         for namespace, view in ViewRegistry.views.items():
             for name, views in view.items():
                 for _view in views:
-                    meta_data = f"name: {name}, view: {_view.view.__module__}.{_view.view.__name__}"
+                    meta_data = (
+                        f"name: {name}, view: "
+                        f"{_view.view.__module__}.{_view.view.__name__}"
+                    )
                     if isinstance(_view.paths, str):
                         self.stdout.write(f"{_view.paths} ({meta_data})")
                     else:
                         for path in _view.paths:
                             self.stdout.write(f"{path} ({meta_data})")
```

### Comparing `django_view_decorator-0.0.2/LICENSE.txt` & `django_view_decorator-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_view_decorator-0.0.2/README.md` & `django_view_decorator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_view_decorator-0.0.2/pyproject.toml` & `django_view_decorator-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-view-decorator"
-description = ''
+description = 'django-view-decorator is decorator aimed at bringing locality of behaviour to the connection between a URL and a view in Django.'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Víðir Valberg Guðmundsson", email = "valberg@orn.li" },
 ]
@@ -22,15 +22,15 @@
 ]
 dependencies = [
   "Django>=3.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Documentation = "https://github.com/valberg/django-view-decorator#readme"
+Documentation = "https://django-view-decorator.readthedocs.io/"
 Issues = "https://github.com/valberg/django-view-decorator/issues"
 Source = "https://github.com/valberg/django-view-decorator"
 
 [tool.hatch.version]
 path = "django_view_decorator/__about__.py"
 
 [tool.hatch.build.targets.sdist]
@@ -41,20 +41,20 @@
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]==7.2.1",
   "pytest==7.2.2",
   "pytest-cov",
   "pytest-django==4.5.2",
   "mypy==1.1.1",
-  "django-stubs==1.15.0",
+  "django-stubs==1.16.0",
 ]
 
 [[tool.hatch.envs.tests.matrix]]
 python = ["3.10", "3.11"]
-django = ["3.2", "4.0", "4.1", "4.2rc1"]
+django = ["3.2", "4.0", "4.1", "4.2"]
 
 [tool.hatch.envs.tests.overrides]
 matrix.django.dependencies = [
     { value = "django~={matrix:django}" },
 ]
 matrix.python.dependencies = [
     { value = "typing_extensions==4.5.0", if = ["3.10"]},
@@ -98,16 +98,25 @@
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.mypy]
 mypy_path = "django_view_decorator/"
-exclude = "venv/"
+exclude = [
+    "venv/",
+    "dist/",
+    "docs/",
+]
 namespace_packages = false
 show_error_codes = true
 strict = true
 warn_unreachable = true
+follow_imports = "normal"
+#plugins = ["mypy_django_plugin.main"]
+
+[tool.django-stubs]
+#django_settings_module = "tests.settings"
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 allow_untyped_defs = true
```

### Comparing `django_view_decorator-0.0.2/PKG-INFO` & `django_view_decorator-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: django-view-decorator
-Version: 0.0.2
-Project-URL: Documentation, https://github.com/valberg/django-view-decorator#readme
+Version: 0.0.3
+Summary: django-view-decorator is decorator aimed at bringing locality of behaviour to the connection between a URL and a view in Django.
+Project-URL: Documentation, https://django-view-decorator.readthedocs.io/
 Project-URL: Issues, https://github.com/valberg/django-view-decorator/issues
 Project-URL: Source, https://github.com/valberg/django-view-decorator
 Author-email: Víðir Valberg Guðmundsson <valberg@orn.li>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

