# Comparing `tmp/pywaclient-1.3.5.tar.gz` & `tmp/pywaclient-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywaclient-1.3.5.tar", last modified: Tue Jun  6 09:45:52 2023, max compression
+gzip compressed data, was "dist/pywaclient-1.3.6.tar", last modified: Mon Jun 19 18:25:56 2023, max compression
```

## Comparing `pywaclient-1.3.5.tar` & `pywaclient-1.3.6.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:45:52.000000 pywaclient-1.3.5/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-06 09:45:41.000000 pywaclient-1.3.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-06-06 09:45:41.000000 pywaclient-1.3.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-06-06 09:45:41.000000 pywaclient-1.3.5/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2208 2023-06-06 09:45:52.000000 pywaclient-1.3.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1759 2023-06-06 09:45:41.000000 pywaclient-1.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)     7013 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/articles.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/block_templates.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/canvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/categories.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/chronicles.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/histories.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/images.py
--rw-rw-rw-   0 root         (0) root         (0)     6023 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/manuscripts.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/map_marker_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/maps.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/notebooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/rpg_system.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/subscriber_groups.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/timelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/users.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/variables.py
--rw-rw-rw-   0 root         (0) root         (0)    14182 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/endpoints/worlds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)     2905 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/exceptions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6892 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/article.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/block.py
--rw-rw-rw-   0 root         (0) root         (0)     3532 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/category.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/entity.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     5558 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/manuscript.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/secret.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-06-06 09:45:41.000000 pywaclient-1.3.5/pywaclient/models/world.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2208 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-06 09:45:52.000000 pywaclient-1.3.5/pywaclient.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-06 09:45:41.000000 pywaclient-1.3.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 09:45:52.000000 pywaclient-1.3.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-06 09:45:41.000000 pywaclient-1.3.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:45:52.000000 pywaclient-1.3.5/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:45:52.000000 pywaclient-1.3.5/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/data/block.json
--rw-rw-rw-   0 root         (0) root         (0)     2469 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/data/form_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/init_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_article_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_block_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_block_template_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_block_template_part_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_canvas_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_category_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_chronicle_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_history_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_image_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3772 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_manuscript_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_map_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_notebook_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_parse_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_rpg_system_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_secret_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1873 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_subscriber_group_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_timeline_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_user_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_variable_collection_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_variable_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     4530 2023-06-06 09:45:41.000000 pywaclient-1.3.5/tests/test_world_endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:25:56.000000 pywaclient-1.3.6/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-19 18:25:46.000000 pywaclient-1.3.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-06-19 18:25:46.000000 pywaclient-1.3.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-06-19 18:25:46.000000 pywaclient-1.3.6/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-06-19 18:25:56.000000 pywaclient-1.3.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2023-06-19 18:25:46.000000 pywaclient-1.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)     7013 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/articles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/block_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/canvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/chronicles.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/eras.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/histories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/images.py
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/manuscripts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/map_marker_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/notebooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/rpg_system.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/subscriber_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/timelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/variables.py
+-rw-rw-rw-   0 root         (0) root         (0)    14182 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/endpoints/worlds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)     2905 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/exceptions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6892 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/article.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/block.py
+-rw-rw-rw-   0 root         (0) root         (0)     3532 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/category.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     5558 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/manuscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-06-19 18:25:46.000000 pywaclient-1.3.6/pywaclient/models/world.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-19 18:25:56.000000 pywaclient-1.3.6/pywaclient.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-19 18:25:46.000000 pywaclient-1.3.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 18:25:56.000000 pywaclient-1.3.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-19 18:25:46.000000 pywaclient-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:25:56.000000 pywaclient-1.3.6/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:25:56.000000 pywaclient-1.3.6/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/data/block.json
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/data/form_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/init_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_article_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_block_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_block_template_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_block_template_part_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_canvas_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_category_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_chronicle_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_history_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_image_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_manuscript_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_map_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_notebook_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_parse_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_rpg_system_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_secret_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_subscriber_group_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3542 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_timeline_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_user_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_variable_collection_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_variable_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4530 2023-06-19 18:25:46.000000 pywaclient-1.3.6/tests/test_world_endpoint.py
```

### Comparing `pywaclient-1.3.5/LICENCE` & `pywaclient-1.3.6/LICENCE`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/PKG-INFO` & `pywaclient-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.3.5
+Version: 1.3.6
 Summary: A small wrapper library around the World Anvil Aragorn API: https://www.worldanvil.com/api/aragorn/documentation.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.3.5/README.md` & `pywaclient-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/__init__.py` & `pywaclient-1.3.6/pywaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/api.py` & `pywaclient-1.3.6/pywaclient/api.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/__init__.py` & `pywaclient-1.3.6/pywaclient/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/articles.py` & `pywaclient-1.3.6/pywaclient/endpoints/chronicles.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from pywaclient.endpoints import CrudEndpoint
 
 
-class ArticleCrudEndpoint(CrudEndpoint):
+class ChronicleCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
-        super().__init__(client, 'article')
+    def __init__(self, client: 'BoromirApiClient'):
+        super().__init__(client, 'chronicle')
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/block_templates.py` & `pywaclient-1.3.6/pywaclient/endpoints/block_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from typing import Dict, Any, Iterable
 
 from pywaclient.endpoints import CrudEndpoint
 
 
 class BlockTemplatePartCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'blocktemplatepart')
 
 class BlockTemplateCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'blocktemplate')
         self.path_block_template_parts = f'{self.path}/blocktemplateparts'
         self.block_template_part = BlockTemplatePartCrudEndpoint(client)
 
     def block_template_parts(self, block_template_id: str, complete: bool = True, limit: int = 50,
                              offset: int = 0) -> Iterable[Dict[str, Any]]:
         """
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/blocks.py` & `pywaclient-1.3.6/pywaclient/endpoints/blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 #    limitations under the License.
 from typing import Dict, Any, Iterable
 from pywaclient.endpoints import CrudEndpoint
 
 
 class BlockCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'block')
 
 class BlockFolderCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'blockfolder')
         self.path_blocks = f'{self.path}/blocks'
         self.block = BlockCrudEndpoint(client)
 
     def blocks(self, folder_id: str, complete: bool = True, limit: int = 50, offset: int = 0) -> Iterable[Dict[str, Any]]:
         """
         A complete list of the statblocks within a folder.
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/canvas.py` & `pywaclient-1.3.6/pywaclient/endpoints/canvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 #    limitations under the License.
 
 from pywaclient.endpoints import CrudEndpoint
 
 
 class CanvasCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'canvas')
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/categories.py` & `pywaclient-1.3.6/pywaclient/endpoints/categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #    limitations under the License.
 from typing import Dict, Any, Iterable
 from pywaclient.endpoints import CrudEndpoint
 
 
 class CategoryCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'category')
         self.path_articles = f'{self.path}/articles'
 
     def articles(self, world_id: str, category_id: str, complete: bool = True, limit: int = 50, offset: int = 0) -> Iterable[Dict[str, Any]]:
         """
         List all articles by a category given, filtered with a limit of entities shown and an offset.
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/chronicles.py` & `pywaclient-1.3.6/pywaclient/endpoints/subscriber_groups.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-
 from pywaclient.endpoints import CrudEndpoint
 
 
-class ChronicleCrudEndpoint(CrudEndpoint):
+class SubscriberGroupCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
-        super().__init__(client, 'chronicle')
+    def __init__(self, client: 'BoromirApiClient'):
+        super().__init__(client, 'subscribergroup')
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/histories.py` & `pywaclient-1.3.6/pywaclient/endpoints/eras.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 from pywaclient.endpoints import CrudEndpoint
 
 
-class HistoryCrudEndpoint(CrudEndpoint):
+class EraCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
-        super().__init__(client, 'history')
+    def __init__(self, client: 'BoromirApiClient'):
+        super().__init__(client, 'era')
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/images.py` & `pywaclient-1.3.6/pywaclient/endpoints/images.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from typing import Iterable
 
 from pywaclient.endpoints import CrudEndpoint, download_binary
 
 
 class ImageCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'image')
 
     def get_binary(self, identifier: str) -> Iterable[bytes]:
         """Get the image binary by identifier
 
         :param identifier: Identifier of the image.
         :return: Iterable of image binary chunks.
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/manuscripts.py` & `pywaclient-1.3.6/pywaclient/endpoints/manuscripts.py`

 * *Files 14% similar despite different names*

```diff
@@ -85,33 +85,33 @@
         :return:            Iterable dictionary of the entities.
         """
         return self._scroll_collection(self.path_stats, {'id': identifier}, 'entities')
 
 
 class ManuscriptBookmarkCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'manuscript_bookmark')
 
 
 class ManuscriptTagCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'manuscript_tag')
 
 
 class ManuscriptLabelCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'manuscript_label')
 
 
 class ManuscriptCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'manuscript')
         self.bookmark = ManuscriptBookmarkCrudEndpoint(client)
         self._path_bookmarks = f'{self.path}/manuscript_bookmarks'
         self.tag = ManuscriptTagCrudEndpoint(client)
         self._path_tags = f'{self.path}/manuscript_tags'
         self.label = ManuscriptLabelCrudEndpoint(client)
         self._path_labels = f'{self.path}/manuscript_labels'
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/map_marker_types.py` & `pywaclient-1.3.6/pywaclient/endpoints/map_marker_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from typing import Dict, Any, Iterable
 
 from pywaclient.endpoints import CrudEndpoint
 
 
 class MapMarkerTypeCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'markertype')
         self.path_list = 'markertypes'
 
     def list(self) -> Iterable[Dict[str, Any]]:
         """Iterate over all map marker types.
         """
         return self._scroll_collection(self.path_list, {}, 'entities')
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/maps.py` & `pywaclient-1.3.6/pywaclient/endpoints/maps.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 from typing import Dict, Any, Iterable
 
 from pywaclient.endpoints import CrudEndpoint
 
 
 class MapMarkerCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'marker')
 
 
 class MapMarkerGroupCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'markergroup')
         self.marker = MapMarkerCrudEndpoint(client)
         self.path_markers = 'markergroup/markers'
 
     def markers(self, map_maker_group_id: str) -> Iterable[Dict[str, Any]]:
         """Iterate over all map markers in a map marker group.
         """
         return self._scroll_collection(self.path_markers, {'id': map_maker_group_id}, 'entities')
 
 
 class MapLayerCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'layer')
 
 
 class MapCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'map')
         self.path_layers = f'{self.path}/layers'
         self.layer = MapLayerCrudEndpoint(client)
         self.path_groups = f'{self.path}/markergroups'
         self.marker_group = MapMarkerGroupCrudEndpoint(client)
 
     def marker_groups(self, map_id: str) -> Iterable[Dict[str, Any]]:
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/notebooks.py` & `pywaclient-1.3.6/pywaclient/endpoints/notebooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 #    limitations under the License.
 from typing import Dict, Any, Iterable
 
 from pywaclient.endpoints import CrudEndpoint
 
 class NoteCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'note')
 
 
 
 class NoteSectionCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'notesection')
         self.note = NoteCrudEndpoint(client)
         self.note_sections_path = f'{self.path}/notes'
 
     def notes(self, note_section_id: str, complete: bool = True, limit: int = 50, offset: int = 0) -> Iterable[Dict[str, Any]]:
         """
         Retrieve an iterable of all the note references within one section.
@@ -44,15 +44,15 @@
         assert offset >= 0
         assert 1 <= limit <= 50
         return self._post_request(self.note_sections_path, {'id': note_section_id}, {'limit': limit, 'offset': offset})['entities']
 
 
 class NotebookCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'notebook')
         self.note_section = NoteSectionCrudEndpoint(client)
         self.path_notebook_sections = f'{self.path}/notesections'
 
     def note_sections(self, notebook_id: str, complete: bool = True, limit: int = 50, offset: int = 0) -> Iterable[Dict[str, Any]]:
         """
         Retrieve an iterable of all the note section references from one notebook.
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/rpg_system.py` & `pywaclient-1.3.6/tests/init_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-#    Copyright 2020 Jonas Waeber
+#    Copyright 2020 - present Jonas Waeber
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-from typing import Dict, Any, Iterable
+import os
 
-from pywaclient.endpoints import BasicEndpoint
+from api import BoromirApiClient
+from models.user import User
 
-
-class RpgSystemCrudEndpoint(BasicEndpoint):
-
-    def __init__(self, client: 'AragornApiClient'):
-        super().__init__(client, 'rpgsystem')
-        self.list_path = 'rpgsystems'
-
-    def list(self) -> Iterable[Dict[str, Any]]:
-        """Iterate over all RPG systems.
-        """
-        return self._scroll_collection(self.list_path, {}, 'entities')
+world_id = 'daae0a12-f3c3-4978-b571-b5313e3c1741'
+client = BoromirApiClient(
+    name='TEST APPLICATION',
+    url='https://gitlab.com/SoulLink/world-anvil-api-client',
+    application_key=os.environ.get('WA_APPLICATION_KEY'),
+    authentication_token=os.environ.get('WA_AUTH_TOKEN'),
+    version='0.1.0'
+)
+user = User(client, client.user.identity()['id'])
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/secrets.py` & `pywaclient-1.3.6/pywaclient/endpoints/secrets.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 from pywaclient.endpoints import CrudEndpoint
 
 
 class SecretCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'secret')
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/subscriber_groups.py` & `pywaclient-1.3.6/tests/test_image_endpoint.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,12 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-from pywaclient.endpoints import CrudEndpoint
 
+if __name__ == '__main__':
+    pass
 
-class SubscriberGroupCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
-        super().__init__(client, 'subscribergroup')
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/timelines.py` & `pywaclient-1.3.6/pywaclient/endpoints/articles.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
+
 from pywaclient.endpoints import CrudEndpoint
 
 
-class TimelineCrudEndpoint(CrudEndpoint):
+class ArticleCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
-        super().__init__(client, 'timeline')
+    def __init__(self, client: 'BoromirApiClient'):
+        super().__init__(client, 'article')
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/users.py` & `pywaclient-1.3.6/pywaclient/endpoints/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from typing import Dict, Any, Iterable
 
 from pywaclient.endpoints import BasicEndpoint
 
 
 class UserCrudEndpoint(BasicEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'user')
         self.identity_path = 'identity'
         self.path_blocktemplates = f'{self.path}/blocktemplates'
         self.path_worlds = f'{self.path}/worlds'
 
     def identity(self):
         """Get the user that is associated with the authentication token provided."""
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/variables.py` & `pywaclient-1.3.6/pywaclient/endpoints/variables.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 from typing import Dict, Any, Iterable
 
 from pywaclient.endpoints import CrudEndpoint
 
 
 class VariableCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'variable')
 
 
 class VariableCollectionCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'variablecollection')
         self.variable = VariableCrudEndpoint(client)
         self.path_variables = f"{self.path}/variables"
 
     def variables(self, world_id: str, variable_collection_id: str, complete: bool = True, limit: int = 50,
                   offset: int = 0) -> Iterable[Dict[str, Any]]:
         """
```

### Comparing `pywaclient-1.3.5/pywaclient/endpoints/worlds.py` & `pywaclient-1.3.6/pywaclient/endpoints/worlds.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Dict, Any, Iterable
 
 from pywaclient.endpoints import CrudEndpoint
 
 
 class WorldCrudEndpoint(CrudEndpoint):
 
-    def __init__(self, client: 'AragornApiClient'):
+    def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'world')
         self.path_categories = f'{self.path}/categories'
         self.path_block_folders = f'{self.path}/blockfolders'
         self.path_variable_collections = f'{self.path}/variablecollections'
         self.path_subscriber_groups = f'{self.path}/subscribergroups'
         self.path_secrets = f'{self.path}/secrets'
         self.path_manuscripts = f'{self.path}/manuscripts'
```

### Comparing `pywaclient-1.3.5/pywaclient/exceptions/__init__.py` & `pywaclient-1.3.6/pywaclient/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/article.py` & `pywaclient-1.3.6/pywaclient/models/article.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/block.py` & `pywaclient-1.3.6/pywaclient/models/block.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/category.py` & `pywaclient-1.3.6/pywaclient/models/category.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/entity.py` & `pywaclient-1.3.6/pywaclient/models/entity.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/genre.py` & `pywaclient-1.3.6/pywaclient/models/genre.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/manuscript.py` & `pywaclient-1.3.6/pywaclient/models/manuscript.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/secret.py` & `pywaclient-1.3.6/pywaclient/models/secret.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/user.py` & `pywaclient-1.3.6/pywaclient/models/user.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient/models/world.py` & `pywaclient-1.3.6/pywaclient/models/world.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/pywaclient.egg-info/PKG-INFO` & `pywaclient-1.3.6/pywaclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.3.5
+Version: 1.3.6
 Summary: A small wrapper library around the World Anvil Aragorn API: https://www.worldanvil.com/api/aragorn/documentation.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.3.5/pywaclient.egg-info/SOURCES.txt` & `pywaclient-1.3.6/pywaclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 pywaclient/endpoints/__init__.py
 pywaclient/endpoints/articles.py
 pywaclient/endpoints/block_templates.py
 pywaclient/endpoints/blocks.py
 pywaclient/endpoints/canvas.py
 pywaclient/endpoints/categories.py
 pywaclient/endpoints/chronicles.py
+pywaclient/endpoints/eras.py
 pywaclient/endpoints/histories.py
 pywaclient/endpoints/images.py
 pywaclient/endpoints/manuscripts.py
 pywaclient/endpoints/map_marker_types.py
 pywaclient/endpoints/maps.py
 pywaclient/endpoints/notebooks.py
 pywaclient/endpoints/rpg_system.py
```

### Comparing `pywaclient-1.3.5/setup.py` & `pywaclient-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/data/block.json` & `pywaclient-1.3.6/tests/data/block.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/data/form_schema.json` & `pywaclient-1.3.6/tests/data/form_schema.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/init_client.py` & `pywaclient-1.3.6/tests/test_rpg_system_endpoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-#    Copyright 2020 - present Jonas Waeber
+#    Copyright 2020 Jonas Waeber
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-import os
+from init_client import client
 
-from api import BoromirApiClient
-from models.user import User
+if __name__ == '__main__':
+    full_list = client.rpg_system.list()
 
-world_id = 'daae0a12-f3c3-4978-b571-b5313e3c1741'
-client = BoromirApiClient(
-    name='TEST APPLICATION',
-    url='https://gitlab.com/SoulLink/world-anvil-api-client',
-    application_key=os.environ.get('WA_APPLICATION_KEY'),
-    authentication_token=os.environ.get('WA_AUTH_TOKEN'),
-    version='0.1.0'
-)
-user = User(client, client.user.identity()['id'])
+    print(len(full_list))
+    print(full_list[0])
+    value = client.rpg_system.get(full_list[0]['id'], 1)
+    print(value)
```

### Comparing `pywaclient-1.3.5/tests/test_article_endpoint.py` & `pywaclient-1.3.6/tests/test_article_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_block_endpoint.py` & `pywaclient-1.3.6/tests/test_block_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_block_template_endpoint.py` & `pywaclient-1.3.6/tests/test_block_template_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_block_template_part_endpoint.py` & `pywaclient-1.3.6/tests/test_block_template_part_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_canvas_endpoint.py` & `pywaclient-1.3.6/tests/test_canvas_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_category_endpoint.py` & `pywaclient-1.3.6/tests/test_category_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_chronicle_endpoint.py` & `pywaclient-1.3.6/tests/test_chronicle_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_history_endpoint.py` & `pywaclient-1.3.6/tests/test_history_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_image_endpoint.py` & `pywaclient-1.3.6/pywaclient/endpoints/histories.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,12 +7,14 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
+from pywaclient.endpoints import CrudEndpoint
 
-if __name__ == '__main__':
-    pass
 
+class HistoryCrudEndpoint(CrudEndpoint):
 
+    def __init__(self, client: 'BoromirApiClient'):
+        super().__init__(client, 'history')
```

### Comparing `pywaclient-1.3.5/tests/test_manuscript_endpoint.py` & `pywaclient-1.3.6/tests/test_manuscript_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_map_endpoint.py` & `pywaclient-1.3.6/tests/test_map_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_notebook_endpoint.py` & `pywaclient-1.3.6/tests/test_notebook_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_parse_response.py` & `pywaclient-1.3.6/tests/test_parse_response.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_secret_endpoint.py` & `pywaclient-1.3.6/tests/test_secret_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_subscriber_group_endpoint.py` & `pywaclient-1.3.6/tests/test_subscriber_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_timeline_endpoint.py` & `pywaclient-1.3.6/tests/test_timeline_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         {
             'title': 'A Secret Subscriber Group',
             'world': {
                 'id': world_id
             }
         })
 
+
+
     test_timelines_1 = client.timeline.put(
         {
             'title': 'Test Timelines Creation',
             'state': 'private',
             'world': {
                 'id': world_id
             },
@@ -77,22 +79,30 @@
             ],
             'description': 'Test Description',
             'utdOffset': 0,
             'type': 'parallel',
             'showInToC': True,
             'calendar': {
                 'id': '102144'
+            }
+        }
+    )
+
+    test_era = client.timeline.era.put(
+        {
+            'title': 'Test Era Creation #1',
+            'world': {
+                'id': world_id
             },
-            # 'eras': [
-            #     {
-            #         'id': '79289b23-3efb-45f8-8f69-4cb4ff6ee3b'
-            #     }
-            # ],
+            'timeline': {
+                'id': test_timelines_1['id']
+            }
         }
     )
+    print(test_era)
     test_timelines_2 = client.timeline.put(
         {
             'title': 'Test Timelines Creation 2',
             'world': {
                 'id': world_id
             }
         }
```

### Comparing `pywaclient-1.3.5/tests/test_user_endpoint.py` & `pywaclient-1.3.6/tests/test_user_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_variable_collection_endpoint.py` & `pywaclient-1.3.6/tests/test_variable_collection_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_variable_endpoint.py` & `pywaclient-1.3.6/tests/test_variable_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.5/tests/test_world_endpoint.py` & `pywaclient-1.3.6/tests/test_world_endpoint.py`

 * *Files identical despite different names*

