# Comparing `tmp/feincms3_cookiecontrol-1.3.0.tar.gz` & `tmp/feincms3_cookiecontrol-1.3.1.tar.gz`

## Comparing `feincms3_cookiecontrol-1.3.0.tar` & `feincms3_cookiecontrol-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,49 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/admin.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/apps.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/embedding.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/models.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/views.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/migrations/0001_rework.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/migrations/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/static/f3cc.js
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templatetags/__init__.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/LICENSE
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/README.rst
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.editorconfig
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.eslintrc.js
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/esbuild.js
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/main.css
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/main.js
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tox.ini
+-rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/yarn.lock
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0    45516 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/docs/banner.png
+-rwxr-xr-x   0        0        0    41563 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/docs/embed.png
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/admin.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/apps.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/embedding.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/models.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/views.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/migrations/0001_rework.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/migrations/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/static/f3cc.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templatetags/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/settings.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/test_cookiecontrol.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/test_embed.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/urls.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/LICENSE
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/README.rst
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/PKG-INFO
```

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/embedding.py` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,17 @@
     return ""
 
 
 def wrap(provider, html, **kwargs):
     return _render(html, provider, _providers[provider], **kwargs)
 
 
-def oembed(url):
-    from feincms3.plugins.external import oembed_json
+def oembed(url, *, oembed_json=None):
+    if oembed_json is None:
+        from feincms3.plugins.external import oembed_json
 
     if (data := oembed_json(url)) and (html := data.get("html")):
         provider_name = data.get("provider_name", "")
         return render_to_string(
             "feincms3_cookiecontrol/embed.html",
             {
                 "embedded_html": f'<div class="responsive-embed widescreen {slugify(provider_name)}">{html}</div>',
```

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/models.py` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/models.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/views.py` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/views.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/migrations/0001_rework.py` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/migrations/0001_rework.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/static/f3cc.js` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/static/f3cc.js`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py` & `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/LICENSE` & `feincms3_cookiecontrol-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/README.rst` & `feincms3_cookiecontrol-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.0/pyproject.toml` & `feincms3_cookiecontrol-1.3.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -43,21 +43,70 @@
 
 [project.urls]
 Homepage = "https://github.com/feinheit/feincms3-cookiecontrol/"
 
 [tool.hatch.version]
 path = "feincms3_cookiecontrol/__init__.py"
 
-[tool.hatch.build.targets.sdist]
-include = [
-    "/feincms3_cookiecontrol",
-]
-
 [tool.ruff]
-extend-select = ["B", "E", "F", "W", "C90", "I", "N", "UP", "FBT", "C4", "DJ", "PIE"]
-extend-ignore = ["E501"]
+extend-select = [
+  # pyflakes, pycodestyle
+  "F", "E", "W",
+  # mmcabe
+  "C90",
+  # isort
+  "I",
+  # pep8-naming
+  "N",
+  # pyupgrade
+  "UP",
+  # flake8-2020
+  "YTT",
+  # flake8-boolean-trap
+  "FBT",
+  # flake8-bugbear
+  "B",
+  # flake8-builtins
+  "A",
+  # flake8-comprehensions
+  "C4",
+  # flake8-django
+  "DJ",
+  # flake8-logging-format
+  "G",
+  # flake8-pie
+  "PIE",
+  # flake8-simplify
+  "SIM",
+  # flake8-gettext
+  "INT",
+  # pygrep-hooks
+  "PGH",
+  # pylint
+  "PL",
+  # unused noqa
+  "RUF100",
+]
+extend-ignore = [
+  # Allow zip() without strict=
+  "B905",
+  # No line length errors
+  "E501",
+]
 fix = true
+show-fixes = true
 target-version = "py39"
 
 [tool.ruff.isort]
 combine-as-imports = true
 lines-after-imports = 2
+
+[tool.ruff.mccabe]
+max-complexity = 15
+
+[tool.ruff.per-file-ignores]
+"*/migrat*/*" = [
+  # Allow using PascalCase model names in migrations
+  "N806",
+  # Ignore the fact that migration files are invalid module names
+  "N999",
+]
```

### Comparing `feincms3_cookiecontrol-1.3.0/PKG-INFO` & `feincms3_cookiecontrol-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feincms3-cookiecontrol
-Version: 1.3.0
+Version: 1.3.1
 Summary: Cookie Control Panel for GDPR compliant feincms3 websites
 Project-URL: Homepage, https://github.com/feinheit/feincms3-cookiecontrol/
 Author-email: York Schickl <ys@feinheit.ch>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

