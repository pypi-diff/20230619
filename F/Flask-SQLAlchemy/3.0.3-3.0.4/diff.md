# Comparing `tmp/Flask-SQLAlchemy-3.0.3.tar.gz` & `tmp/flask_sqlalchemy-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SQLAlchemy-3.0.3.tar", last modified: Tue Jan 31 16:07:30 2023, max compression
+gzip compressed data, was "flask_sqlalchemy-3.0.4.tar", last modified: Mon Jun 19 17:31:22 2023, max compression
```

## Comparing `Flask-SQLAlchemy-3.0.3.tar` & `flask_sqlalchemy-3.0.4.tar`

### file list

```diff
@@ -1,79 +1,61 @@
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/_static/flask-sqlalchemy-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/_static/flask-sqlalchemy-title.png
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/binds.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/customizing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/legacy-query.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/pagination.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/queries.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-01-31 16:07:22.866726 Flask-SQLAlchemy-3.0.3/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/docs/record-queries.rst
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/docs/track-modifications.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/auth/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/auth/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/blog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/blog/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/blog/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/templates/auth/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/templates/auth/register.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/templates/blog/create.html
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/templates/blog/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/flaskr/templates/blog/update.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/flaskr/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/todo/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/todo/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/todo/templates/new.html
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/examples/todo/templates/show_all.html
--rw-r--r--   0 runner    (1001) docker     (123)   140769 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    38220 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/record_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/track_modifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_legacy_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_model_bind.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_model_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_record_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_table_bind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tests/test_track_modifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 16:07:22.870726 Flask-SQLAlchemy-3.0.3/tox.ini
--rw-------   0 runner    (1001) docker     (123)     3338 2023-01-31 16:07:30.158702 Flask-SQLAlchemy-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0    14114 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/CHANGES.rst
+-rw-r--r--   0        0        0     1475 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/LICENSE.rst
+-rw-r--r--   0        0        0     2210 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/README.rst
+-rw-r--r--   0        0        0      634 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/Makefile
+-rw-r--r--   0        0        0    16397 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/_static/flask-sqlalchemy-logo.png
+-rw-r--r--   0        0        0    11109 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/_static/flask-sqlalchemy-title.png
+-rw-r--r--   0        0        0     2276 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/api.rst
+-rw-r--r--   0        0        0     3463 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/binds.rst
+-rw-r--r--   0        0        0       45 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/changes.rst
+-rw-r--r--   0        0        0     1902 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/conf.py
+-rw-r--r--   0        0        0     7369 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/config.rst
+-rw-r--r--   0        0        0     2744 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/contexts.rst
+-rw-r--r--   0        0        0     7548 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/customizing.rst
+-rw-r--r--   0        0        0     1171 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/index.rst
+-rw-r--r--   0        0        0     2314 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/legacy-query.rst
+-rw-r--r--   0        0        0       71 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/license.rst
+-rw-r--r--   0        0        0      765 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/make.bat
+-rw-r--r--   0        0        0     3487 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/models.rst
+-rw-r--r--   0        0        0     2655 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/pagination.rst
+-rw-r--r--   0        0        0     3116 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/queries.rst
+-rw-r--r--   0        0        0     7503 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/quickstart.rst
+-rw-r--r--   0        0        0     1150 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/record-queries.rst
+-rw-r--r--   0        0        0      962 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/docs/track-modifications.rst
+-rw-r--r--   0        0        0     1917 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/dev.in
+-rw-r--r--   0        0        0     1310 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/dev.txt
+-rw-r--r--   0        0        0       69 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/docs.in
+-rw-r--r--   0        0        0     1281 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/docs.txt
+-rw-r--r--   0        0        0       23 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/mypy.in
+-rw-r--r--   0        0        0      532 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/mypy.txt
+-rw-r--r--   0        0        0       45 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/tests-min.in
+-rw-r--r--   0        0        0      524 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/tests-min.txt
+-rw-r--r--   0        0        0       15 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/tests.in
+-rw-r--r--   0        0        0      342 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/requirements/tests.txt
+-rw-r--r--   0        0        0     1250 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      484 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/cli.py
+-rw-r--r--   0        0        0    38305 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/extension.py
+-rw-r--r--   0        0        0     7112 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/model.py
+-rw-r--r--   0        0        0    10963 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/py.typed
+-rw-r--r--   0        0        0     3748 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/query.py
+-rw-r--r--   0        0        0     4306 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/record_queries.py
+-rw-r--r--   0        0        0     3189 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/session.py
+-rw-r--r--   0        0        0      859 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/table.py
+-rw-r--r--   0        0        0     2755 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/track_modifications.py
+-rw-r--r--   0        0        0     1047 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      365 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_cli.py
+-rw-r--r--   0        0        0     3919 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_engine.py
+-rw-r--r--   0        0        0     3727 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_legacy_query.py
+-rw-r--r--   0        0        0     4032 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_metadata.py
+-rw-r--r--   0        0        0     1612 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_model.py
+-rw-r--r--   0        0        0     2579 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_model_bind.py
+-rw-r--r--   0        0        0     7793 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_model_name.py
+-rw-r--r--   0        0        0     5356 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_pagination.py
+-rw-r--r--   0        0        0      931 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_record_queries.py
+-rw-r--r--   0        0        0     2523 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_session.py
+-rw-r--r--   0        0        0     1203 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_table_bind.py
+-rw-r--r--   0        0        0     1966 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_track_modifications.py
+-rw-r--r--   0        0        0     2356 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tests/test_view_query.py
+-rw-r--r--   0        0        0      918 2023-06-19 17:31:22.000000 flask_sqlalchemy-3.0.4/tox.ini
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 flask_sqlalchemy-3.0.4/PKG-INFO
```

### Comparing `Flask-SQLAlchemy-3.0.3/CHANGES.rst` & `flask_sqlalchemy-3.0.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Version 3.0.4
+-------------
+
+Released 2023-06-19
+
+-   Fix type hint for ``get_or_404`` return value. :pr:`1208`
+-   Fix type hints for pyright (used by VS Code Pylance extension). :issue:`1205`
+
+
 Version 3.0.3
 -------------
 
 Released 2023-01-31
 
 -   Show helpful errors when mistakenly using multiple ``SQLAlchemy`` instances for the
     same app, or without calling ``init_app``. :pr:`1151`
```

### Comparing `Flask-SQLAlchemy-3.0.3/LICENSE.rst` & `flask_sqlalchemy-3.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/README.rst` & `flask_sqlalchemy-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/Makefile` & `flask_sqlalchemy-3.0.4/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
-SPHINXBUILD   ?= pdm run sphinx-build
+SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `Flask-SQLAlchemy-3.0.3/docs/_static/flask-sqlalchemy-logo.png` & `flask_sqlalchemy-3.0.4/docs/_static/flask-sqlalchemy-logo.png`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/_static/flask-sqlalchemy-title.png` & `flask_sqlalchemy-3.0.4/docs/_static/flask-sqlalchemy-title.png`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/api.rst` & `flask_sqlalchemy-3.0.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/binds.rst` & `flask_sqlalchemy-3.0.4/docs/binds.rst`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,14 @@
 
 .. code-block:: python
 
     # create tables for all binds
     db.create_all()
 
     # create tables for the default and "auth" binds
-    db.create_all(bind=[None, "auth"])
+    db.create_all(bind_key=[None, "auth"])
 
     # create tables for the "meta" bind
-    db.create_all(bind="meta")
+    db.create_all(bind_key="meta")
 
     # drop tables for the default bind
-    db.drop_all(bind=None)
+    db.drop_all(bind_key=None)
```

### Comparing `Flask-SQLAlchemy-3.0.3/docs/conf.py` & `flask_sqlalchemy-3.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/config.rst` & `flask_sqlalchemy-3.0.4/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/contexts.rst` & `flask_sqlalchemy-3.0.4/docs/contexts.rst`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 If you find yourself writing many tests like that, you can use a pytest fixture to push
 a context for a specific test.
 
 .. code-block:: python
 
     import pytest
 
-    @pytest.mark.fixture
+    @pytest.fixture
     def app_ctx(app):
         with app.app_context():
             yield
 
     @pytest.mark.usefixtures("app_ctx")
-    def test_user_model(app):
+    def test_user_model():
         user = User()
         db.session.add(user)
         db.session.commit()
```

### Comparing `Flask-SQLAlchemy-3.0.3/docs/customizing.rst` & `flask_sqlalchemy-3.0.4/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/index.rst` & `flask_sqlalchemy-3.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/legacy-query.rst` & `flask_sqlalchemy-3.0.4/docs/legacy-query.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/make.bat` & `flask_sqlalchemy-3.0.4/docs/make.bat`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 @ECHO OFF
 
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=pdm run sphinx-build
+	set SPHINXBUILD=sphinx-build
 )
 set SOURCEDIR=.
 set BUILDDIR=_build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
```

### Comparing `Flask-SQLAlchemy-3.0.3/docs/models.rst` & `flask_sqlalchemy-3.0.4/docs/models.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/pagination.rst` & `flask_sqlalchemy-3.0.4/docs/pagination.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/queries.rst` & `flask_sqlalchemy-3.0.4/docs/queries.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/quickstart.rst` & `flask_sqlalchemy-3.0.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/record-queries.rst` & `flask_sqlalchemy-3.0.4/docs/record-queries.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/docs/track-modifications.rst` & `flask_sqlalchemy-3.0.4/docs/track-modifications.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/pyproject.toml` & `flask_sqlalchemy-3.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,132 +1,76 @@
 [project]
 name = "Flask-SQLAlchemy"
 description = "Add SQLAlchemy support to your Flask application."
 readme = "README.rst"
-authors = [
-    { name = "Armin Ronacher", email = "armin.ronacher@active-4.com" },
-]
-maintainers = [
-    { name = "Pallets", email = "contact@palletsprojects.com" },
-]
+license = { file = "LICENSE.rst" }
+maintainers = [{name = "Pallets", email = "contact@palletsprojects.com"},]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
-dynamic = []
 requires-python = ">=3.7"
 dependencies = [
-    "Flask>=2.2",
-    "SQLAlchemy>=1.4.18",
+    "flask>=2.2.5",
+    "sqlalchemy>=1.4.18",
 ]
-version = "3.0.3"
-
-[project.license]
-text = "BSD-3-Clause"
+dynamic = ["version"]
 
 [project.urls]
 Donate = "https://palletsprojects.com/donate"
-Documentation = "https://flask-sqlalchemy.palletsprojects.com/"
+Documentation = "https://flask-sqlalchemy.palletsprojects.com"
 Changes = "https://flask-sqlalchemy.palletsprojects.com/changes/"
 "Source Code" = "https://github.com/pallets-eco/flask-sqlalchemy/"
 "Issue Tracker" = "https://github.com/pallets-eco/flask-sqlalchemy/issues/"
-Twitter = "https://twitter.com/PalletsTeam"
 Chat = "https://discord.gg/pallets"
 
-[project.optional-dependencies]
-
 [build-system]
-requires = [
-    "pdm-pep517>=1.0.0",
-]
-build-backend = "pdm.pep517.api"
+requires = ["flit_core<4"]
+build-backend = "flit_core.buildapi"
 
-[tool.pdm.version]
-source = "file"
-path = "src/flask_sqlalchemy/__init__.py"
-
-[tool.pdm.dev-dependencies]
-tests = [
-    "pytest",
-    "blinker",
-]
-coverage = [
-    "pytest-cov",
-    "coverage[toml]",
-]
-mypy = [
-    "mypy",
-    "pytest",
-    "sqlalchemy",
-]
-docs = [
-    "sphinx",
-    "pallets-sphinx-themes",
-    "sphinx-issues",
-    "sphinxcontrib-log-cabinet",
-]
-pre-commit = [
-    "pre-commit",
-]
-tox = [
-    "tox",
-    "tox-pdm",
-]
+[tool.flit.module]
+name = "flask_sqlalchemy"
 
-[tool.pdm.build]
-source-includes = [
+[tool.flit.sdist]
+include = [
     "docs/",
-    "examples/",
+    "requirements/",
     "tests/",
     "CHANGES.rst",
-    "pdm.lock",
     "tox.ini",
 ]
-excludes = [
-    "docs/_build",
+exclude = [
+    "docs/_build/",
 ]
 
 [tool.pytest.ini_options]
-testpaths = [
-    "tests",
-]
-filterwarnings = [
-    "error",
-]
+testpaths = ["tests"]
+filterwarnings = ["error"]
 
 [tool.coverage.run]
 branch = true
-source = [
-    "flask_sqlalchemy",
-    "tests",
-]
+source = ["flask_sqlalchemy", "tests"]
 
 [tool.coverage.paths]
-source = [
-    "src",
-    "*/site-packages",
-]
+source = ["src", "*/site-packages"]
 
 [tool.mypy]
 python_version = "3.7"
-files = [
-    "src/flask_sqlalchemy",
-    "tests",
-]
+files = ["src/flask_sqlalchemy", "tests"]
 show_error_codes = true
 pretty = true
 strict = true
-disable_error_code = [
-    "name-defined",
-]
+# db.Model attribute doesn't recognize subclassing
+disable_error_code = ["name-defined"]
+# db.Model is Any
 disallow_subclassing_any = false
 
 [[tool.mypy.overrides]]
 module = [
     "cryptography.*",
     "importlib_metadata.*",
 ]
```

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/__init__.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing as t
 
 from .extension import SQLAlchemy
 
-__version__ = "3.0.3"
+__version__ = "3.0.4"
 
 __all__ = [
     "SQLAlchemy",
 ]
 
 _deprecated_map = {
     "Model": ".model.Model",
```

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/extension.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import os
 import typing as t
 from weakref import WeakKeyDictionary
 
 import sqlalchemy as sa
-import sqlalchemy.event
-import sqlalchemy.exc
-import sqlalchemy.orm
+import sqlalchemy.event as sa_event
+import sqlalchemy.exc as sa_exc
+import sqlalchemy.orm as sa_orm
 from flask import abort
 from flask import current_app
 from flask import Flask
 from flask import has_app_context
 
 from .model import _QueryProperty
 from .model import DefaultMeta
@@ -19,14 +19,16 @@
 from .pagination import Pagination
 from .pagination import SelectPagination
 from .query import Query
 from .session import _app_ctx_id
 from .session import Session
 from .table import _Table
 
+_O = t.TypeVar("_O", bound=object)  # Based on sqlalchemy.orm._typing.py
+
 
 class SQLAlchemy:
     """Integrates SQLAlchemy with Flask. This handles setting up one or more engines,
     associating tables and models with specific engines, and cleaning up connections and
     sessions after each request.
 
     Only the engine configuration is specific to each application, other things like
@@ -123,15 +125,15 @@
     def __init__(
         self,
         app: Flask | None = None,
         *,
         metadata: sa.MetaData | None = None,
         session_options: dict[str, t.Any] | None = None,
         query_class: type[Query] = Query,
-        model_class: type[Model] | sa.orm.DeclarativeMeta = Model,
+        model_class: type[Model] | sa_orm.DeclarativeMeta = Model,
         engine_options: dict[str, t.Any] | None = None,
         add_models_to_shell: bool = True,
     ):
         if session_options is None:
             session_options = {}
 
         self.Query = query_class
@@ -265,14 +267,15 @@
         if app.config.get("SQLALCHEMY_COMMIT_ON_TEARDOWN", False):
             import warnings
 
             warnings.warn(
                 "'SQLALCHEMY_COMMIT_ON_TEARDOWN' is deprecated and will be removed in"
                 " Flask-SQAlchemy 3.1. Call 'db.session.commit()'` directly instead.",
                 DeprecationWarning,
+                stacklevel=2,
             )
             app.teardown_appcontext(self._teardown_commit)
         else:
             app.teardown_appcontext(self._teardown_session)
 
         basic_uri: str | sa.engine.URL | None = app.config.setdefault(
             "SQLALCHEMY_DATABASE_URI", None
@@ -334,15 +337,15 @@
         if app.config.setdefault("SQLALCHEMY_TRACK_MODIFICATIONS", False):
             from . import track_modifications
 
             track_modifications._listen(self.session)
 
     def _make_scoped_session(
         self, options: dict[str, t.Any]
-    ) -> sa.orm.scoped_session[Session]:
+    ) -> sa_orm.scoped_session[Session]:
         """Create a :class:`sqlalchemy.orm.scoping.scoped_session` around the factory
         from :meth:`_make_session_factory`. The result is available as :attr:`session`.
 
         The scope function can be customized using the ``scopefunc`` key in the
         ``session_options`` parameter to the extension. By default it uses the current
         thread or greenlet id.
 
@@ -357,19 +360,19 @@
             The session is scoped to the current app context.
 
         .. versionchanged:: 3.0
             Renamed from ``create_scoped_session``, this method is internal.
         """
         scope = options.pop("scopefunc", _app_ctx_id)
         factory = self._make_session_factory(options)
-        return sa.orm.scoped_session(factory, scope)
+        return sa_orm.scoped_session(factory, scope)
 
     def _make_session_factory(
         self, options: dict[str, t.Any]
-    ) -> sa.orm.sessionmaker[Session]:
+    ) -> sa_orm.sessionmaker[Session]:
         """Create the SQLAlchemy :class:`sqlalchemy.orm.sessionmaker` used by
         :meth:`_make_scoped_session`.
 
         To customize, pass the ``session_options`` parameter to :class:`SQLAlchemy`. To
         customize the session class, subclass :class:`.Session` and pass it as the
         ``class_`` key.
 
@@ -384,15 +387,15 @@
             The session class can be customized.
 
         .. versionchanged:: 3.0
             Renamed from ``create_session``, this method is internal.
         """
         options.setdefault("class_", Session)
         options.setdefault("query_cls", self.Query)
-        return sa.orm.sessionmaker(db=self, **options)
+        return sa_orm.sessionmaker(db=self, **options)
 
     def _teardown_commit(self, exc: BaseException | None) -> None:
         """Commit the session at the end of the request if there was not an unhandled
         exception during the request.
 
         :meta private:
 
@@ -478,15 +481,15 @@
 
                 metadata = self._make_metadata(bind_key)
                 return super().__new__(cls, *[args[0], metadata, *args[1:]], **kwargs)
 
         return Table
 
     def _make_declarative_base(
-        self, model: type[Model] | sa.orm.DeclarativeMeta
+        self, model: type[Model] | sa_orm.DeclarativeMeta
     ) -> type[t.Any]:
         """Create a SQLAlchemy declarative model class. The result is available as
         :attr:`Model`.
 
         To customize, subclass :class:`.Model` and pass it as ``model_class`` to
         :class:`SQLAlchemy`. To customize at the metaclass level, pass an already
         created declarative model class as ``model_class``.
@@ -499,17 +502,17 @@
 
         .. versionchanged:: 3.0
             Renamed with a leading underscore, this method is internal.
 
         .. versionchanged:: 2.3
             ``model`` can be an already created declarative model class.
         """
-        if not isinstance(model, sa.orm.DeclarativeMeta):
+        if not isinstance(model, sa_orm.DeclarativeMeta):
             metadata = self._make_metadata(None)
-            model = sa.orm.declarative_base(
+            model = sa_orm.declarative_base(
                 metadata=metadata, cls=model, name="Model", metaclass=DefaultMeta
             )
 
         if None not in self.metadatas:
             # Use the model's metadata as the default metadata.
             model.metadata.info["bind_key"] = None  # type: ignore[union-attr]
             self.metadatas[None] = model.metadata  # type: ignore[union-attr]
@@ -726,16 +729,16 @@
         return {
             table: engine
             for bind_key, engine in self.engines.items()
             for table in self.metadatas[bind_key].tables.values()
         }
 
     def get_or_404(
-        self, entity: type[t.Any], ident: t.Any, *, description: str | None = None
-    ) -> t.Any:
+        self, entity: type[_O], ident: t.Any, *, description: str | None = None
+    ) -> t.Optional[_O]:
         """Like :meth:`session.get() <sqlalchemy.orm.Session.get>` but aborts with a
         ``404 Not Found`` error instead of returning ``None``.
 
         :param entity: The model class to query.
         :param ident: The primary key to query.
         :param description: A custom message to show on the error page.
 
@@ -776,15 +779,15 @@
         :param statement: The ``select`` statement to execute.
         :param description: A custom message to show on the error page.
 
         .. versionadded:: 3.0
         """
         try:
             return self.session.execute(statement).scalar_one()
-        except (sa.exc.NoResultFound, sa.exc.MultipleResultsFound):
+        except (sa_exc.NoResultFound, sa_exc.MultipleResultsFound):
             abort(404, description=description)
 
     def paginate(
         self,
         select: sa.sql.Select[t.Any],
         *,
         page: int | None = None,
@@ -855,15 +858,15 @@
                 engine = self.engines[key]
             except KeyError:
                 message = f"Bind key '{key}' is not in 'SQLALCHEMY_BINDS' config."
 
                 if key is None:
                     message = f"'SQLALCHEMY_DATABASE_URI' config is not set. {message}"
 
-                raise sa.exc.UnboundExecutionError(message) from None
+                raise sa_exc.UnboundExecutionError(message) from None
 
             metadata = self.metadatas[key]
             getattr(metadata, op_name)(bind=engine)
 
     def create_all(self, bind_key: str | None | list[str | None] = "__all__") -> None:
         """Create tables that do not exist in the database by calling
         ``metadata.create_all()`` for all or some bind keys. This does not
@@ -932,53 +935,53 @@
             if isinstance(backref, str):
                 backref = (backref, {})
 
             backref[1].setdefault("query_class", self.Query)
 
     def relationship(
         self, *args: t.Any, **kwargs: t.Any
-    ) -> sa.orm.RelationshipProperty[t.Any]:
+    ) -> sa_orm.RelationshipProperty[t.Any]:
         """A :func:`sqlalchemy.orm.relationship` that applies this extension's
         :attr:`Query` class for dynamic relationships and backrefs.
 
         .. versionchanged:: 3.0
             The :attr:`Query` class is set on ``backref``.
         """
         self._set_rel_query(kwargs)
-        return sa.orm.relationship(*args, **kwargs)
+        return sa_orm.relationship(*args, **kwargs)
 
     def dynamic_loader(
         self, argument: t.Any, **kwargs: t.Any
-    ) -> sa.orm.RelationshipProperty[t.Any]:
+    ) -> sa_orm.RelationshipProperty[t.Any]:
         """A :func:`sqlalchemy.orm.dynamic_loader` that applies this extension's
         :attr:`Query` class for relationships and backrefs.
 
         .. versionchanged:: 3.0
             The :attr:`Query` class is set on ``backref``.
         """
         self._set_rel_query(kwargs)
-        return sa.orm.dynamic_loader(argument, **kwargs)
+        return sa_orm.dynamic_loader(argument, **kwargs)
 
     def _relation(
         self, *args: t.Any, **kwargs: t.Any
-    ) -> sa.orm.RelationshipProperty[t.Any]:
+    ) -> sa_orm.RelationshipProperty[t.Any]:
         """A :func:`sqlalchemy.orm.relationship` that applies this extension's
         :attr:`Query` class for dynamic relationships and backrefs.
 
         SQLAlchemy 2.0 removes this name, use ``relationship`` instead.
 
         :meta private:
 
         .. versionchanged:: 3.0
             The :attr:`Query` class is set on ``backref``.
         """
         # Deprecated, removed in SQLAlchemy 2.0. Accessed through ``__getattr__``.
         self._set_rel_query(kwargs)
-        f = sa.orm.relation  # type: ignore[attr-defined]
-        return f(*args, **kwargs)  # type: ignore[no-any-return]
+        f = sa_orm.relationship
+        return f(*args, **kwargs)
 
     def __getattr__(self, name: str) -> t.Any:
         if name == "db":
             import warnings
 
             warnings.warn(
                 "The 'db' attribute is deprecated and will be removed in"
@@ -989,17 +992,17 @@
             )
             return self
 
         if name == "relation":
             return self._relation
 
         if name == "event":
-            return sa.event
+            return sa_event
 
         if name.startswith("_"):
             raise AttributeError(name)
 
-        for mod in (sa, sa.orm):
+        for mod in (sa, sa_orm):
             if hasattr(mod, name):
                 return getattr(mod, name)
 
         raise AttributeError(name)
```

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/model.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import re
 import typing as t
 
 import sqlalchemy as sa
-import sqlalchemy.orm
+import sqlalchemy.orm as sa_orm
 
 from .query import Query
 
 if t.TYPE_CHECKING:
     from .extension import SQLAlchemy
 
 
@@ -178,37 +178,37 @@
         should be generated.
     -   Abstract models should not have one generated.
 
     Later, ``__table_cls__`` will determine if the model looks like single or
     joined-table inheritance. If no primary key is found, the name will be unset.
     """
     if cls.__dict__.get("__abstract__", False) or not any(
-        isinstance(b, sa.orm.DeclarativeMeta) for b in cls.__mro__[1:]
+        isinstance(b, sa_orm.DeclarativeMeta) for b in cls.__mro__[1:]
     ):
         return False
 
     for base in cls.__mro__:
         if "__tablename__" not in base.__dict__:
             continue
 
-        if isinstance(base.__dict__["__tablename__"], sa.orm.declared_attr):
+        if isinstance(base.__dict__["__tablename__"], sa_orm.declared_attr):
             return False
 
         return not (
             base is cls
             or base.__dict__.get("__abstract__", False)
-            or not isinstance(base, sa.orm.DeclarativeMeta)
+            or not isinstance(base, sa_orm.DeclarativeMeta)
         )
 
     return True
 
 
 def camel_to_snake_case(name: str) -> str:
     """Convert a ``CamelCase`` name to ``snake_case``."""
     name = re.sub(r"((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))", r"_\1", name)
     return name.lower().lstrip("_")
 
 
-class DefaultMeta(BindMetaMixin, NameMetaMixin, sa.orm.DeclarativeMeta):
+class DefaultMeta(BindMetaMixin, NameMetaMixin, sa_orm.DeclarativeMeta):
     """SQLAlchemy declarative metaclass that provides ``__bind_key__`` and
     ``__tablename__`` support.
     """
```

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/pagination.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing as t
 from math import ceil
 
 import sqlalchemy as sa
-import sqlalchemy.orm
+import sqlalchemy.orm as sa_orm
 from flask import abort
 from flask import request
 
 
 class Pagination:
     """Apply an offset and limit to the query based on the current page and number of
     items per page.
@@ -332,15 +332,15 @@
         select = self._query_args["select"]
         select = select.limit(self.per_page).offset(self._query_offset)
         session = self._query_args["session"]
         return list(session.execute(select).unique().scalars())
 
     def _query_count(self) -> int:
         select = self._query_args["select"]
-        sub = select.options(sa.orm.lazyload("*")).order_by(None).subquery()
+        sub = select.options(sa_orm.lazyload("*")).order_by(None).subquery()
         session = self._query_args["session"]
         out = session.execute(sa.select(sa.func.count()).select_from(sub)).scalar()
         return out  # type: ignore[no-any-return]
 
 
 class QueryPagination(Pagination):
     """Returned by :meth:`.Query.paginate`. Takes a ``query`` argument in addition to
```

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/query.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import typing as t
 
-import sqlalchemy as sa
-import sqlalchemy.exc
-import sqlalchemy.orm
+import sqlalchemy.exc as sa_exc
+import sqlalchemy.orm as sa_orm
 from flask import abort
 
 from .pagination import Pagination
 from .pagination import QueryPagination
 
 
-class Query(sa.orm.Query):  # type: ignore[type-arg]
+class Query(sa_orm.Query):  # type: ignore[type-arg]
     """SQLAlchemy :class:`~sqlalchemy.orm.query.Query` subclass with some extra methods
     useful for querying in a web application.
 
     This is the default query class for :attr:`.Model.query`.
 
     .. versionchanged:: 3.0
         Renamed to ``Query`` from ``BaseQuery``.
@@ -54,15 +53,15 @@
 
         :param description: A custom message to show on the error page.
 
         .. versionadded:: 3.0
         """
         try:
             return self.one()
-        except (sa.exc.NoResultFound, sa.exc.MultipleResultsFound):
+        except (sa_exc.NoResultFound, sa_exc.MultipleResultsFound):
             abort(404, description=description)
 
     def paginate(
         self,
         *,
         page: int | None = None,
         per_page: int | None = None,
```

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/record_queries.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/record_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import dataclasses
 import inspect
 import typing as t
 from time import perf_counter
 
 import sqlalchemy as sa
-import sqlalchemy.event
+import sqlalchemy.event as sa_event
 from flask import current_app
 from flask import g
 from flask import has_app_context
 
 
 def get_recorded_queries() -> list[_QueryInfo]:
     """Get the list of recorded query information for the current session. Queries are
@@ -92,16 +92,16 @@
             DeprecationWarning,
             stacklevel=2,
         )
         return getattr(self, name)
 
 
 def _listen(engine: sa.engine.Engine) -> None:
-    sa.event.listen(engine, "before_cursor_execute", _record_start, named=True)
-    sa.event.listen(engine, "after_cursor_execute", _record_end, named=True)
+    sa_event.listen(engine, "before_cursor_execute", _record_start, named=True)
+    sa_event.listen(engine, "after_cursor_execute", _record_end, named=True)
 
 
 def _record_start(context: sa.engine.ExecutionContext, **kwargs: t.Any) -> None:
     if not has_app_context():
         return
 
     context._fsa_start_time = perf_counter()  # type: ignore[attr-defined]
```

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/session.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import typing as t
 
 import sqlalchemy as sa
-import sqlalchemy.exc
-import sqlalchemy.orm
+import sqlalchemy.exc as sa_exc
+import sqlalchemy.orm as sa_orm
 from flask.globals import app_ctx
 
 if t.TYPE_CHECKING:
     from .extension import SQLAlchemy
 
 
-class Session(sa.orm.Session):
+class Session(sa_orm.Session):
     """A SQLAlchemy :class:`~sqlalchemy.orm.Session` class that chooses what engine to
     use based on the bind key associated with the metadata associated with the thing
     being queried.
 
     To customize ``db.session``, subclass this and pass it as the ``class_`` key in the
     ``session_options`` to :class:`.SQLAlchemy`.
 
@@ -51,17 +51,17 @@
             return bind
 
         engines = self._db.engines
 
         if mapper is not None:
             try:
                 mapper = sa.inspect(mapper)
-            except sa.exc.NoInspectionAvailable as e:
+            except sa_exc.NoInspectionAvailable as e:
                 if isinstance(mapper, type):
-                    raise sa.orm.exc.UnmappedClassError(mapper) from e
+                    raise sa_orm.exc.UnmappedClassError(mapper) from e
 
                 raise
 
             engine = _clause_to_engine(mapper.local_table, engines)
 
             if engine is not None:
                 return engine
@@ -84,15 +84,15 @@
     """If the clause is a table, return the engine associated with the table's
     metadata's bind key.
     """
     if isinstance(clause, sa.Table) and "bind_key" in clause.metadata.info:
         key = clause.metadata.info["bind_key"]
 
         if key not in engines:
-            raise sa.exc.UnboundExecutionError(
+            raise sa_exc.UnboundExecutionError(
                 f"Bind key '{key}' is not in 'SQLALCHEMY_BINDS' config."
             )
 
         return engines[key]
 
     return None
```

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/table.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/table.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/src/flask_sqlalchemy/track_modifications.py` & `flask_sqlalchemy-3.0.4/src/flask_sqlalchemy/track_modifications.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing as t
 
 import sqlalchemy as sa
-import sqlalchemy.event
-import sqlalchemy.orm
+import sqlalchemy.event as sa_event
+import sqlalchemy.orm as sa_orm
 from flask import current_app
 from flask import has_app_context
 from flask.signals import Namespace  # type: ignore[attr-defined]
 
 if t.TYPE_CHECKING:
     from .session import Session
 
@@ -25,20 +25,20 @@
 
 before_models_committed = _signals.signal("before-models-committed")
 """This signal works exactly like :data:`models_committed` but is emitted before the
 commit takes place.
 """
 
 
-def _listen(session: sa.orm.scoped_session[Session]) -> None:
-    sa.event.listen(session, "before_flush", _record_ops, named=True)
-    sa.event.listen(session, "before_commit", _record_ops, named=True)
-    sa.event.listen(session, "before_commit", _before_commit)
-    sa.event.listen(session, "after_commit", _after_commit)
-    sa.event.listen(session, "after_rollback", _after_rollback)
+def _listen(session: sa_orm.scoped_session[Session]) -> None:
+    sa_event.listen(session, "before_flush", _record_ops, named=True)
+    sa_event.listen(session, "before_commit", _record_ops, named=True)
+    sa_event.listen(session, "before_commit", _before_commit)
+    sa_event.listen(session, "after_commit", _after_commit)
+    sa_event.listen(session, "after_rollback", _after_rollback)
 
 
 def _record_ops(session: Session, **kwargs: t.Any) -> None:
     if not has_app_context():
         return
 
     if not current_app.config["SQLALCHEMY_TRACK_MODIFICATIONS"]:
```

### Comparing `Flask-SQLAlchemy-3.0.3/tests/conftest.py` & `flask_sqlalchemy-3.0.4/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 @pytest.fixture
 def db(app: Flask) -> SQLAlchemy:
     return SQLAlchemy(app)
 
 
 @pytest.fixture
-def Todo(app: Flask, db: SQLAlchemy) -> t.Any:
+def Todo(app: Flask, db: SQLAlchemy) -> t.Generator[t.Any, None, None]:
     class Todo(db.Model):
         id = sa.Column(sa.Integer, primary_key=True)
         title = sa.Column(sa.String)
 
     with app.app_context():
         db.create_all()
```

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_engine.py` & `flask_sqlalchemy-3.0.4/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_legacy_query.py` & `flask_sqlalchemy-3.0.4/tests/test_legacy_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 import typing as t
 import warnings
 
 import pytest
 import sqlalchemy as sa
-import sqlalchemy.exc
+import sqlalchemy.exc as sa_exc
 from flask import Flask
 from werkzeug.exceptions import NotFound
 
 from flask_sqlalchemy import SQLAlchemy
 from flask_sqlalchemy.query import Query
 
 
 @pytest.fixture(autouse=True)
 def ignore_query_warning() -> t.Generator[None, None, None]:
-    if hasattr(sa.exc, "LegacyAPIWarning"):
+    if hasattr(sa_exc, "LegacyAPIWarning"):
         with warnings.catch_warnings():
-            exc = sa.exc.LegacyAPIWarning
+            exc = sa_exc.LegacyAPIWarning
             warnings.simplefilter("ignore", exc)
             yield
     else:
         yield
 
 
 @pytest.mark.usefixtures("app_ctx")
```

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_metadata.py` & `flask_sqlalchemy-3.0.4/tests/test_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import pytest
 import sqlalchemy as sa
-import sqlalchemy.exc
-import sqlalchemy.orm
+import sqlalchemy.exc as sa_exc
+import sqlalchemy.orm as sa_orm
 from flask import Flask
 
 from flask_sqlalchemy import SQLAlchemy
 from flask_sqlalchemy.model import DefaultMeta
 from flask_sqlalchemy.model import Model
 
 
@@ -22,23 +22,23 @@
     db = SQLAlchemy(metadata=metadata)
     assert db.metadata is metadata
     assert db.metadata.info["bind_key"] is None
     assert db.Model.metadata is db.metadata
 
 
 def test_metadata_from_custom_model() -> None:
-    base = sa.orm.declarative_base(cls=Model, metaclass=DefaultMeta)
+    base = sa_orm.declarative_base(cls=Model, metaclass=DefaultMeta)
     metadata = base.metadata
     db = SQLAlchemy(model_class=base)
     assert db.Model.metadata is metadata
     assert db.Model.metadata is db.metadata
 
 
 def test_custom_metadata_overrides_custom_model() -> None:
-    base = sa.orm.declarative_base(cls=Model, metaclass=DefaultMeta)
+    base = sa_orm.declarative_base(cls=Model, metaclass=DefaultMeta)
     metadata = sa.MetaData()
     db = SQLAlchemy(model_class=base, metadata=metadata)
     assert db.Model.metadata is metadata
     assert db.Model.metadata is db.metadata
 
 
 def test_metadata_per_bind(app: Flask) -> None:
@@ -65,29 +65,29 @@
     class User(db.Model):
         id = sa.Column(sa.Integer, primary_key=True)
 
     class Post(db.Model):
         __bind_key__ = "a"
         id = sa.Column(sa.Integer, primary_key=True)
 
-    with pytest.raises(sa.exc.OperationalError):
+    with pytest.raises(sa_exc.OperationalError):
         db.session.execute(sa.select(User)).scalars()
 
-    with pytest.raises(sa.exc.OperationalError):
+    with pytest.raises(sa_exc.OperationalError):
         db.session.execute(sa.select(Post)).scalars()
 
     db.create_all()
     db.session.execute(sa.select(User)).scalars()
     db.session.execute(sa.select(Post)).scalars()
     db.drop_all()
 
-    with pytest.raises(sa.exc.OperationalError):
+    with pytest.raises(sa_exc.OperationalError):
         db.session.execute(sa.select(User)).scalars()
 
-    with pytest.raises(sa.exc.OperationalError):
+    with pytest.raises(sa_exc.OperationalError):
         db.session.execute(sa.select(Post)).scalars()
 
 
 @pytest.mark.usefixtures("app_ctx")
 @pytest.mark.parametrize("bind_key", ["a", ["a"]])
 def test_create_key_spec(app: Flask, bind_key: str | list[str | None]) -> None:
     app.config["SQLALCHEMY_BINDS"] = {"a": "sqlite://"}
@@ -99,15 +99,15 @@
     class Post(db.Model):
         __bind_key__ = "a"
         id = sa.Column(sa.Integer, primary_key=True)
 
     db.create_all(bind_key=bind_key)
     db.session.execute(sa.select(Post)).scalars()
 
-    with pytest.raises(sa.exc.OperationalError):
+    with pytest.raises(sa_exc.OperationalError):
         db.session.execute(sa.select(User)).scalars()
 
 
 @pytest.mark.usefixtures("app_ctx")
 def test_reflect(app: Flask) -> None:
     app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///user.db"
     app.config["SQLALCHEMY_BINDS"] = {"post": "sqlite:///post.db"}
```

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_model.py` & `flask_sqlalchemy-3.0.4/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing as t
 
 import pytest
 import sqlalchemy as sa
-import sqlalchemy.orm
+import sqlalchemy.orm as sa_orm
 from flask import Flask
 
 from flask_sqlalchemy import SQLAlchemy
 from flask_sqlalchemy.model import DefaultMeta
 from flask_sqlalchemy.model import Model
 
 
@@ -30,15 +30,15 @@
 
 @pytest.mark.usefixtures("app_ctx")
 @pytest.mark.parametrize("base", [Model, object])
 def test_custom_declarative_class(app: Flask, base: t.Any) -> None:
     class CustomMeta(DefaultMeta):
         pass
 
-    CustomModel = sa.orm.declarative_base(cls=base, name="Model", metaclass=CustomMeta)
+    CustomModel = sa_orm.declarative_base(cls=base, name="Model", metaclass=CustomMeta)
     db = SQLAlchemy(app, model_class=CustomModel)
     assert db.Model is CustomModel
     assert db.Model.query_class is db.Query
     assert "query" in db.Model.__dict__
 
 
 @pytest.mark.usefixtures("app_ctx")
```

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_model_bind.py` & `flask_sqlalchemy-3.0.4/tests/test_model_bind.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_model_name.py` & `flask_sqlalchemy-3.0.4/tests/test_model_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import inspect
 import typing as t
 
 import pytest
 import sqlalchemy as sa
-import sqlalchemy.exc
-import sqlalchemy.orm
+import sqlalchemy.exc as sa_exc
+import sqlalchemy.orm as sa_orm
 
 from flask_sqlalchemy import SQLAlchemy
 from flask_sqlalchemy.model import camel_to_snake_case
 
 
 @pytest.mark.parametrize(
     ("name", "expect"),
@@ -106,15 +106,15 @@
 
 def test_mixin_attr(db: SQLAlchemy) -> None:
     """A declared attr tablename will be used down multiple levels of
     inheritance.
     """
 
     class Mixin:
-        @sa.orm.declared_attr  # type: ignore[arg-type]
+        @sa_orm.declared_attr  # type: ignore[arg-type]
         def __tablename__(cls) -> str:  # noqa: B902
             return cls.__name__.upper()  # type: ignore[attr-defined,no-any-return]
 
     class Bird(Mixin, db.Model):
         id = sa.Column(sa.Integer, primary_key=True)
 
     class Duck(Bird):
@@ -149,15 +149,15 @@
     mixin, not directly on the class.
     """
 
     class Duck(db.Model):
         id = sa.Column(sa.Integer, primary_key=True)
 
     class IdMixin:
-        @sa.orm.declared_attr
+        @sa_orm.declared_attr
         def id(cls):  # type: ignore[no-untyped-def]  # noqa: B902
             return sa.Column(sa.Integer, sa.ForeignKey(Duck.id), primary_key=True)
 
     class RubberDuck(IdMixin, Duck):  # type: ignore[misc]
         pass
 
     assert RubberDuck.__tablename__ == "rubber_duck"
@@ -217,15 +217,15 @@
         id = sa.Column(sa.Integer, primary_key=True)
 
     class ns:
         is_duck = False
         floats = False
 
     class Witch(Duck):
-        @sa.orm.declared_attr  # type: ignore[arg-type]
+        @sa_orm.declared_attr  # type: ignore[arg-type]
         def is_duck(self) -> None:
             # declared attrs will be accessed during mapper configuration,
             # but make sure they're not accessed before that
             info = inspect.getouterframes(inspect.currentframe())[2]
             assert info[3] != "_should_set_tablename"
             ns.is_duck = True
 
@@ -243,15 +243,15 @@
     class User(db.Model):
         pass
 
     assert User.__table__ is user
 
 
 def test_correct_error_for_no_primary_key(db: SQLAlchemy) -> None:
-    with pytest.raises(sa.exc.ArgumentError) as info:
+    with pytest.raises(sa_exc.ArgumentError) as info:
 
         class User(db.Model):
             pass
 
     assert "could not assemble any primary key" in str(info.value)
```

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_pagination.py` & `flask_sqlalchemy-3.0.4/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_record_queries.py` & `flask_sqlalchemy-3.0.4/tests/test_record_queries.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import os
+
 import pytest
 import sqlalchemy as sa
 from flask import Flask
 
 from flask_sqlalchemy import SQLAlchemy
 from flask_sqlalchemy.record_queries import get_recorded_queries
 
@@ -20,9 +22,9 @@
     db.session.execute(sa.select(Example).filter(Example.id < 5)).scalars()
     info = get_recorded_queries()[-1]
     assert info.statement is not None
     assert "SELECT" in info.statement
     assert "FROM example" in info.statement
     assert info.parameters[0][0] == 5
     assert info.duration == info.end_time - info.start_time
-    assert "tests/test_record_queries.py:" in info.location
+    assert os.path.join("tests", "test_record_queries.py:") in info.location
     assert "(test_query_info)" in info.location
```

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_session.py` & `flask_sqlalchemy-3.0.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_table_bind.py` & `flask_sqlalchemy-3.0.4/tests/test_table_bind.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/tests/test_track_modifications.py` & `flask_sqlalchemy-3.0.4/tests/test_track_modifications.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-3.0.3/PKG-INFO` & `flask_sqlalchemy-3.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: Flask-SQLAlchemy
-Version: 3.0.3
+Version: 3.0.4
 Summary: Add SQLAlchemy support to your Flask application.
-License: BSD-3-Clause
-Author-email: Armin Ronacher <armin.ronacher@active-4.com>
 Maintainer-email: Pallets <contact@palletsprojects.com>
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Dist: flask>=2.2.5
+Requires-Dist: sqlalchemy>=1.4.18
 Project-URL: Changes, https://flask-sqlalchemy.palletsprojects.com/changes/
 Project-URL: Chat, https://discord.gg/pallets
-Project-URL: Documentation, https://flask-sqlalchemy.palletsprojects.com/
+Project-URL: Documentation, https://flask-sqlalchemy.palletsprojects.com
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Issue Tracker, https://github.com/pallets-eco/flask-sqlalchemy/issues/
 Project-URL: Source Code, https://github.com/pallets-eco/flask-sqlalchemy/
-Project-URL: Twitter, https://twitter.com/PalletsTeam
-Description-Content-Type: text/x-rst
 
 Flask-SQLAlchemy
 ================
 
 Flask-SQLAlchemy is an extension for `Flask`_ that adds support for
 `SQLAlchemy`_ to your application. It aims to simplify using SQLAlchemy
 with Flask by providing useful defaults and extra helpers that make it
```

