# Comparing `tmp/oarepo-model-builder-multilingual-3.0.5.tar.gz` & `tmp/oarepo-model-builder-multilingual-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-multilingual-3.0.5.tar", last modified: Mon Jun 19 10:48:20 2023, max compression
+gzip compressed data, was "oarepo-model-builder-multilingual-3.0.6.tar", last modified: Mon Jun 19 12:40:12 2023, max compression
```

## Comparing `oarepo-model-builder-multilingual-3.0.5.tar` & `oarepo-model-builder-multilingual-3.0.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.817660 oarepo-model-builder-multilingual-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-19 10:48:20.817660 oarepo-model-builder-multilingual-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.809660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.809660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.809660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/builtin_models/i18n.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.809660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.809660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.809660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/facets/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.813660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.813660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.813660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/model/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.813660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/multilings.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/faker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.813660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.813660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.813660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/utils/supported_langs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.817660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.809660 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-19 10:48:20.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-19 10:48:20.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:48:20.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-19 10:48:20.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-19 10:48:20.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-19 10:48:20.000000 oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-19 10:48:20.817660 oarepo-model-builder-multilingual-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:48:20.817660 oarepo-model-builder-multilingual-3.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/mock_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/model.json5
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/multilingual_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/test_build_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/test_i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/test_marshmallow_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/test_multi_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-19 10:47:43.000000 oarepo-model-builder-multilingual-3.0.5/tests/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.714549 oarepo-model-builder-multilingual-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-19 12:40:12.714549 oarepo-model-builder-multilingual-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.702549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builtin_models/i18n.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/multilings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/faker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.710549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.710549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.710549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/utils/supported_langs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.710549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.702549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-19 12:40:12.714549 oarepo-model-builder-multilingual-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.714549 oarepo-model-builder-multilingual-3.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/mock_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/model.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/multilingual_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_build_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_i18nStr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_marshmallow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_multi_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_ui.py
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/LICENSE` & `oarepo-model-builder-multilingual-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 3.0.5
+Version: 3.0.6
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
@@ -13,14 +13,15 @@
 ## Usage
 
 Within this plugin, two data types are added: multilingual and i18nstr. They can be added to the data model
 using `type: multilingual` or `type: i18nstr`.
 Values containing language tags must be in IETF [format](https://www.w3.org/International/articles/language-tags/).
 The structure of both data types can be changed using the `multilingual` field
 
+
 ## i18nStr
 
 An object that contains the language of the item and the actual value of the item.
 
 ### Example
 
 #### Model
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/README.md` & `oarepo-model-builder-multilingual-3.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ## Usage
 
 Within this plugin, two data types are added: multilingual and i18nstr. They can be added to the data model
 using `type: multilingual` or `type: i18nstr`.
 Values containing language tags must be in IETF [format](https://www.w3.org/International/articles/language-tags/).
 The structure of both data types can be changed using the `multilingual` field
 
+
 ## i18nStr
 
 An object that contains the language of the item and the actual value of the item.
 
 ### Example
 
 #### Model
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/__init__.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 from typing import List
 
 from oarepo_model_builder.datatypes import DataType, Import, datatypes
 from oarepo_model_builder.datatypes.components import (
     ObjectMarshmallowComponent,
     RegularMarshmallowComponent,
 )
-from oarepo_model_builder.datatypes.components.marshmallow import (
-    MarshmallowField,
-)
+from oarepo_model_builder.datatypes.components.marshmallow import MarshmallowField
 from oarepo_model_builder.datatypes.components.marshmallow.graph import MarshmallowClass
 from oarepo_model_builder.utils.absolute_class import convert_to_absolute_class_name
-from oarepo_model_builder.utils.python_name import (
-    qualified_name,
-)
+from oarepo_model_builder.utils.python_name import qualified_name
 
-from oarepo_model_builder_multilingual.datatypes import (
-    I18nDataType,
-)
+from oarepo_model_builder_multilingual.datatypes import I18nDataType
 
 
 class I18nMarshmallowMixin:
     def _register_class_name(
         self, datatype, marshmallow_config, classes, marshmallow_module
     ):
         schema_class = marshmallow_config.get("class")
@@ -51,15 +45,14 @@
                 definition_marshmallow["class"] = qualified_schema_class
                 schema_class = qualified_schema_class
             if not generate:
                 if fingerprint not in classes:
                     classes[fingerprint] = schema_class
                 return
 
-
     def _build_class(
         self, datatype, marshmallow, children, field_generator, classes  # NOSONAR
     ):
         fields = []
         for _, c in sorted(children.items()):
             datatypes.call_components(c, field_generator, fields=fields)
         extra_fields = [
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 from typing import List
 
 from oarepo_model_builder.datatypes import DataType, Import, datatypes
 from oarepo_model_builder.datatypes.components import (
     UIMarshmallowComponent,
     UIObjectMarshmallowComponent,
 )
-from oarepo_model_builder.datatypes.components.marshmallow import (
-    MarshmallowField,
-)
+from oarepo_model_builder.datatypes.components.marshmallow import MarshmallowField
 from oarepo_model_builder.datatypes.components.marshmallow.graph import MarshmallowClass
 from oarepo_model_builder.utils.absolute_class import convert_to_absolute_class_name
-from oarepo_model_builder.utils.python_name import (
-    qualified_name,
-)
+from oarepo_model_builder.utils.python_name import qualified_name
 
-from oarepo_model_builder_multilingual.datatypes import (
-    I18nDataType,
-)
+from oarepo_model_builder_multilingual.datatypes import I18nDataType
 
 
 class I18nMarshmallowMixin:
     def _register_class_name(
         self, datatype, marshmallow_config, classes, marshmallow_module
     ):
         schema_class = marshmallow_config.get("class")
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/datatypes/multilings.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/multilings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-
-
 from oarepo_model_builder.datatypes import DataType
 from oarepo_model_builder.datatypes.containers import ArrayDataType, NestedDataType
 from oarepo_model_builder.utils.deepmerge import deepmerge
-
 from oarepo_model_builder.utils.facet_helpers import facet_name
 
 
 class MultilingualDataType(ArrayDataType):
     schema_type = "array"
     mapping_type = "multilingual"
     marshmallow_field = "ma_fields.List"
     model_type = "multilingual"
 
     class ModelSchema(DataType.ModelSchema):
         pass
 
-
     def prepare(self, context):
         definition = self.definition
 
         definition["type"] = "array"
         definition["items"] = {"type": "i18nStr"}
         definition_marsh = definition.get("marshmallow", {})
         if "field-class" not in definition_marsh:
@@ -161,8 +157,7 @@
         definition["sample"] = {"skip": False}
 
         def_properties[lang] = {"type": "keyword"}
         def_properties[value] = {"type": "fulltext+keyword"}
         definition["properties"] = def_properties
 
         super().prepare(context)
-
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/faker.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/faker.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/utils/supported_langs.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/utils/supported_langs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual/validation/__init__.py` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/validation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     @validates_schema
     def validate_schema(self, data, **kwargs):
         for lang in data:
             if not langcodes.Language.get(lang).is_valid():
                 raise ValidationError("Invalid language code")
 
 
-
 class LanguagesSettingsSchema(ExtendablePartSchema):
-
     supported_langs = fields.Raw(data_key="supported-langs", required=False)
 
 
 validators = {
     "settings": LanguagesSettingsSchema,
-
 }
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 3.0.5
+Version: 3.0.6
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
@@ -13,14 +13,15 @@
 ## Usage
 
 Within this plugin, two data types are added: multilingual and i18nstr. They can be added to the data model
 using `type: multilingual` or `type: i18nstr`.
 Values containing language tags must be in IETF [format](https://www.w3.org/International/articles/language-tags/).
 The structure of both data types can be changed using the `multilingual` field
 
+
 ## i18nStr
 
 An object that contains the language of the item and the actual value of the item.
 
 ### Example
 
 #### Model
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/SOURCES.txt` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/oarepo_model_builder_multilingual.egg-info/entry_points.txt` & `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/setup.cfg` & `oarepo-model-builder-multilingual-3.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-multilingual
-version = 3.0.5
+version = 3.0.6
 description = 
 authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>"]
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/mock_filesystem.py` & `oarepo-model-builder-multilingual-3.0.6/tests/mock_filesystem.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/multilingual_schema.py` & `oarepo-model-builder-multilingual-3.0.6/tests/multilingual_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/test_build_from_entrypoints.py` & `oarepo-model-builder-multilingual-3.0.6/tests/test_build_from_entrypoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -111,28 +111,31 @@
 
 
 def test_mapping2():
     schema = load_model(
         "test.yaml",
         model_content={
             "settings": {
-                "supported-langs": {"cs": {"keyword":
-                                               {"type": "keyword"},
-                                           "text":
-                                               {"analyzer": "czech"}}, "en": {}},
+                "supported-langs": {
+                    "cs": {
+                        "keyword": {"type": "keyword"},
+                        "text": {"analyzer": "czech"},
+                    },
+                    "en": {},
+                },
             },
             "record": {
                 "module": {"qualified": "test"},
                 "properties": {
                     "b[]": {"properties": {"c": "multilingual"}},
                     "notes[]": "fulltext",
                     "keywords[]": "multilingual",
-                    "abstract": 'multilingual',
-                    "methods": 'multilingual',
-                    "technicalInfo": 'multilingual',
+                    "abstract": "multilingual",
+                    "methods": "multilingual",
+                    "technicalInfo": "multilingual",
                 },
             },
         },
         isort=False,
         black=False,
         autoflake=False,
     )
@@ -411,7 +414,106 @@
             print(data)
             assert isinstance(data["a"], list)
             for i18n in data["a"]:
                 assert i18n["lang"] in ("cs", "en")
 
             assert isinstance(data["b"], dict)
             assert data["b"]["lang"] in ("cs", "en")
+
+
+def test_non_i18n_mapping():
+    schema = load_model(
+        "test.yaml",
+        model_content={
+            "settings": {"supported-langs": {"cs": {}, "en": {}}},
+            "record": {
+                "module": {"qualified": "test"},
+                "properties": {
+                    "a": {"type": "fulltext", "multilingual": {"i18n": True}},
+                    "b[]": {"type": "keyword", "multilingual": {"i18n": True}},
+                    "c":{"properties":{"d": {"type":"keyword", "multilingual": {"i18n": True} }  } }
+                },
+            },
+        },
+        isort=False,
+        black=False,
+        autoflake=False,
+    )
+
+    filesystem = MockFilesystem()
+    builder = create_builder_from_entrypoints(filesystem=filesystem)
+
+    builder.build(schema, "record", ["record"], "")
+
+    data = builder.filesystem.open(
+        os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
+    ).read()
+    print(data)
+    data = json.loads(data)
+    assert data == {
+    "mappings": {
+        "properties": {
+            "a_cs": {
+                "type": "text",
+                "fields": {
+                    "keyword": {
+                        "type": "keyword"
+                    }
+                }
+            },
+            "a_en": {
+                "type": "text",
+                "fields": {
+                    "keyword": {
+                        "type": "keyword"
+                    }
+                }
+            },
+            "b_cs": {
+                "type": "text",
+                "fields": {
+                    "keyword": {
+                        "type": "keyword"
+                    }
+                }
+            },
+            "b_en": {
+                "type": "text",
+                "fields": {
+                    "keyword": {
+                        "type": "keyword"
+                    }
+                }
+            },
+            "a": {
+                "type": "text"
+            },
+            "b": {
+                "type": "keyword"
+            },
+            "c": {
+                "type": "object",
+                "properties": {
+                    "d_cs": {
+                        "type": "text",
+                        "fields": {
+                            "keyword": {
+                                "type": "keyword"
+                            }
+                        }
+                    },
+                    "d_en": {
+                        "type": "text",
+                        "fields": {
+                            "keyword": {
+                                "type": "keyword"
+                            }
+                        }
+                    },
+                    "d": {
+                        "type": "keyword"
+                    }
+                }
+            }
+        }
+    }
+}
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/test_cfg.py` & `oarepo-model-builder-multilingual-3.0.6/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/test_helper.py` & `oarepo-model-builder-multilingual-3.0.6/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/test_i18nStr.py` & `oarepo-model-builder-multilingual-3.0.6/tests/test_i18nStr.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                     "a": {"type": "i18nStr"},
                     "b": {
                         "type": "i18nStr",
                         "multilingual": {
                             "lang-field": "language",
                             "value-field": "val",
                         },
-                    }
+                    },
                 },
             },
         },
         isort=False,
         black=False,
         autoflake=False,
     )
@@ -143,19 +143,15 @@
                     "b": {
                         "type": "i18nStr",
                         "multilingual": {
                             "lang-field": "language",
                             "value-field": "val",
                         },
                     },
-                    "c":{
-                        "properties": {
-                            "d" : "keyword"
-                        }
-                    }
+                    "c": {"properties": {"d": "keyword"}},
                 },
             },
         },
         isort=False,
         black=False,
         autoflake=False,
     )
@@ -228,17 +224,15 @@
                         },
                     },
                     "c": {
                         "type": "object",
                         "properties": {
                             "f": {"type": "array", "items": {"type": "i18nStr"}},
                             "d": {"type": "array", "items": {"type": "multilingual"}},
-
                         },
-
                     },
                 },
             },
         },
         isort=False,
         black=False,
         autoflake=False,
@@ -249,8 +243,7 @@
 
     builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
     ).read()
     print(data)
-
```

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/test_marshmallow_ui.py` & `oarepo-model-builder-multilingual-3.0.6/tests/test_marshmallow_ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/test_multi_facets.py` & `oarepo-model-builder-multilingual-3.0.6/tests/test_multi_facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/test_schema.py` & `oarepo-model-builder-multilingual-3.0.6/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.5/tests/test_ui.py` & `oarepo-model-builder-multilingual-3.0.6/tests/test_ui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import json
+import os
+
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 
 from tests.mock_filesystem import MockFilesystem
 
 
 def test_validity():
     schema = load_model(
@@ -13,19 +16,22 @@
                         "text": {"analyzer": "czech"},
                         "sort": {"type": "icu_collation_keyword"},
                     }
                 }
             },
             "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {"a": {"type": "multilingual", "ui": {}}},
             },
         },
         isort=False,
         black=False,
         autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "record", ["record"], "")
+
+
```

