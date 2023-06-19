# Comparing `tmp/django-anarticle-0.1.0rc1.tar.gz` & `tmp/django-anarticle-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-anarticle-0.1.0rc1.tar", last modified: Wed Feb  8 04:15:15 2023, max compression
+gzip compressed data, was "django-anarticle-0.1.0rc3.tar", last modified: Mon Jun 19 03:56:04 2023, max compression
```

## Comparing `django-anarticle-0.1.0rc1.tar` & `django-anarticle-0.1.0rc3.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-08 04:15:15.772184 django-anarticle-0.1.0rc1/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3257 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/.gitignore
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      556 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/LICENSE
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)       63 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2313 2023-02-08 04:15:15.772184 django-anarticle-0.1.0rc1/PKG-INFO
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1222 2023-02-07 04:01:02.000000 django-anarticle-0.1.0rc1/README.rst
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-08 04:15:15.768184 django-anarticle-0.1.0rc1/anarticle/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/__init__.py
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-08 04:15:15.768184 django-anarticle-0.1.0rc1/anarticle/admin/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/admin/__init__.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      968 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/admin/mixins.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      231 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/apps.py
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-08 04:15:15.768184 django-anarticle-0.1.0rc1/anarticle/graphqls/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      551 2023-02-02 05:54:08.000000 django-anarticle-0.1.0rc1/anarticle/graphqls/article.graphql
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      347 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/graphqls/category.graphql
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      303 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/graphqls/tag.graphql
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-08 04:15:15.768184 django-anarticle-0.1.0rc1/anarticle/migrations/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     4699 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/migrations/0001_initial.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/migrations/__init__.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     4990 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/models.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3573 2023-02-07 01:49:13.000000 django-anarticle-0.1.0rc1/anarticle/resolvers.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      129 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/tests.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      854 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/anarticle/utils.py
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-08 04:15:15.768184 django-anarticle-0.1.0rc1/django_anarticle.egg-info/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2313 2023-02-08 04:15:15.000000 django-anarticle-0.1.0rc1/django_anarticle.egg-info/PKG-INFO
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      653 2023-02-08 04:15:15.000000 django-anarticle-0.1.0rc1/django_anarticle.egg-info/SOURCES.txt
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)        1 2023-02-08 04:15:15.000000 django-anarticle-0.1.0rc1/django_anarticle.egg-info/dependency_links.txt
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      207 2023-02-08 04:15:15.000000 django-anarticle-0.1.0rc1/django_anarticle.egg-info/requires.txt
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)       21 2023-02-08 04:15:15.000000 django-anarticle-0.1.0rc1/django_anarticle.egg-info/top_level.txt
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1739 2023-02-08 04:03:34.000000 django-anarticle-0.1.0rc1/pyproject.toml
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)       38 2023-02-08 04:15:15.772184 django-anarticle-0.1.0rc1/setup.cfg
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)       86 2023-02-02 02:49:22.000000 django-anarticle-0.1.0rc1/setup.py
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-08 04:15:15.772184 django-anarticle-0.1.0rc1/tests/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      467 2023-02-07 01:49:13.000000 django-anarticle-0.1.0rc1/tests/conftest.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     4195 2023-02-07 01:49:13.000000 django-anarticle-0.1.0rc1/tests/test_resolvers.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-19 03:56:04.823765 django-anarticle-0.1.0rc3/
+-rwxr-xr-x   0 cchiut    (1000) cchiut    (1000)      464 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/.editorconfig
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3257 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/.gitignore
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      556 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/LICENSE
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)       63 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/MANIFEST.in
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3938 2023-06-19 03:56:04.823765 django-anarticle-0.1.0rc3/PKG-INFO
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2703 2023-06-19 03:32:53.000000 django-anarticle-0.1.0rc3/README.rst
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-19 03:56:04.819766 django-anarticle-0.1.0rc3/anarticle/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/__init__.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      231 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/apps.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-19 03:56:04.823765 django-anarticle-0.1.0rc3/anarticle/graphqls/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2056 2023-06-19 03:43:09.000000 django-anarticle-0.1.0rc3/anarticle/graphqls/__init__.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      551 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/graphqls/article.graphql
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2638 2023-06-19 03:07:30.000000 django-anarticle-0.1.0rc3/anarticle/graphqls/bindables.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2245 2023-06-19 03:07:28.000000 django-anarticle-0.1.0rc3/anarticle/graphqls/bindables_sync.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      347 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/graphqls/category.graphql
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      303 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/graphqls/tag.graphql
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3495 2023-06-19 03:06:55.000000 django-anarticle-0.1.0rc3/anarticle/graphqls/type_defs.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-19 03:56:04.823765 django-anarticle-0.1.0rc3/anarticle/migrations/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3524 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/migrations/0001_initial.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/migrations/__init__.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1064 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/mixins.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3687 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/models.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3607 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/resolvers.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      108 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/tests.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      878 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/anarticle/utils.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-19 03:56:04.823765 django-anarticle-0.1.0rc3/django_anarticle.egg-info/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3938 2023-06-19 03:56:04.000000 django-anarticle-0.1.0rc3/django_anarticle.egg-info/PKG-INFO
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      783 2023-06-19 03:56:04.000000 django-anarticle-0.1.0rc3/django_anarticle.egg-info/SOURCES.txt
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)        1 2023-06-19 03:56:04.000000 django-anarticle-0.1.0rc3/django_anarticle.egg-info/dependency_links.txt
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      207 2023-06-19 03:56:04.000000 django-anarticle-0.1.0rc3/django_anarticle.egg-info/requires.txt
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)       21 2023-06-19 03:56:04.000000 django-anarticle-0.1.0rc3/django_anarticle.egg-info/top_level.txt
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1857 2023-06-19 03:45:22.000000 django-anarticle-0.1.0rc3/pyproject.toml
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)       38 2023-06-19 03:56:04.823765 django-anarticle-0.1.0rc3/setup.cfg
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)       86 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/setup.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-19 03:56:04.823765 django-anarticle-0.1.0rc3/tests/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-06-19 03:44:03.000000 django-anarticle-0.1.0rc3/tests/__init__.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      453 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/tests/conftest.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     4195 2023-06-17 03:57:20.000000 django-anarticle-0.1.0rc3/tests/test_resolvers.py
```

### Comparing `django-anarticle-0.1.0rc1/.gitignore` & `django-anarticle-0.1.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `django-anarticle-0.1.0rc1/LICENSE` & `django-anarticle-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-anarticle-0.1.0rc1/anarticle/admin/mixins.py` & `django-anarticle-0.1.0rc3/anarticle/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 """
 Copyright (c) 2014-present, aglean Inc.
 """
 from django.contrib import admin
 
-from anarticle.models import Paragraph
+from .models import Paragraph
 
 
 class TagAdminMixin():
+    ordering = ('name',)
     list_display = ('id', 'name', 'image', 'image_url', 'article_count')
     search_fields = ('name',)
 
 
 class CategoryAdminMixin():
+    ordering = ('name',)
     list_display = ('id', 'name', 'description', 'image', 'image_url',
                     'tag_count')
     list_filter = ('tags',)
     search_fields = ('name',)
     autocomplete_fields = ('tags',)
 
 
 class ParagraphInline(admin.StackedInline):
+    ordering = ('id',)
     model = Paragraph
 
 
 class ArticleAdminMixin():
+    ordering = ('-created_at',)
     list_display = ('id', 'title', 'author', 'image', 'image_url',
                     'is_published', 'published_at', 'updated_at', 'created_at')
     list_filter = ('tags', 'tags__category')
     search_fields = ('title',)
     inlines = (ParagraphInline,)
     autocomplete_fields = ('tags', 'author')
```

### Comparing `django-anarticle-0.1.0rc1/anarticle/graphqls/article.graphql` & `django-anarticle-0.1.0rc3/anarticle/graphqls/article.graphql`

 * *Files identical despite different names*

### Comparing `django-anarticle-0.1.0rc1/anarticle/migrations/0001_initial.py` & `django-anarticle-0.1.0rc3/anarticle/migrations/0001_initial.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.4 on 2022-12-28 02:43
+# Generated by Django 4.1.6 on 2023-02-22 08:17
 
 import anarticle.utils
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
@@ -15,72 +15,52 @@
     ]
 
     operations = [
         migrations.CreateModel(
             name='Article',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('title', models.CharField(max_length=255, verbose_name='Title')),
-                ('slug', models.SlugField(allow_unicode=True, blank=True, help_text='Characters combine with numbers, underscores or hyphens.Ex: today1_news-headline', verbose_name='Slug')),
-                ('summary', models.TextField(verbose_name='Summary')),
-                ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anarticle.utils.image_path, verbose_name='Cover image')),
-                ('is_published', models.BooleanField(default=True, help_text='Designates whether the item is published on the site.', verbose_name='Publish')),
-                ('published_at', models.DateTimeField(blank=True, null=True, verbose_name='Published at')),
-                ('created_at', models.DateTimeField(auto_now_add=True, verbose_name='Created at')),
-                ('updated_at', models.DateTimeField(auto_now=True, verbose_name='Updated at')),
-                ('author', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL, verbose_name='Author')),
+                ('title', models.CharField(max_length=255)),
+                ('slug', models.SlugField(allow_unicode=True, blank=True, help_text='Characters combine with numbers, underscores or hyphens.Ex: today1_news-headline')),
+                ('summary', models.TextField()),
+                ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anarticle.utils.image_path)),
+                ('is_published', models.BooleanField(default=True, help_text='Designates whether the item is published on the site.', verbose_name='Published')),
+                ('published_at', models.DateTimeField(blank=True, null=True)),
+                ('created_at', models.DateTimeField(auto_now_add=True)),
+                ('updated_at', models.DateTimeField(auto_now=True)),
+                ('author', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL)),
             ],
-            options={
-                'verbose_name': 'Article',
-                'verbose_name_plural': 'Articles',
-                'ordering': ['-created_at'],
-            },
         ),
         migrations.CreateModel(
             name='Tag',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=255, unique=True, verbose_name='Name')),
-                ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anarticle.utils.image_path, verbose_name='Cover image')),
+                ('name', models.CharField(max_length=255)),
+                ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anarticle.utils.image_path)),
             ],
-            options={
-                'verbose_name': 'Tag',
-                'verbose_name_plural': 'Tags',
-                'ordering': ['name'],
-            },
         ),
         migrations.CreateModel(
             name='Paragraph',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('content', models.TextField(blank=True, verbose_name='Content')),
-                ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anarticle.utils.image_path, verbose_name='Image')),
-                ('image_text', models.CharField(blank=True, help_text='Descripe the image content', max_length=255, verbose_name='Image description')),
-                ('article', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='anarticle.article', verbose_name='Article')),
+                ('content', models.TextField(blank=True)),
+                ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anarticle.utils.image_path)),
+                ('image_text', models.CharField(blank=True, help_text='Descripe the image content', max_length=255)),
+                ('article', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='anarticle.article')),
             ],
-            options={
-                'verbose_name': 'Paragraph',
-                'verbose_name_plural': 'Paragraphs',
-                'ordering': ['id'],
-            },
         ),
         migrations.CreateModel(
             name='Category',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=255, unique=True, verbose_name='Name')),
-                ('description', models.TextField(blank=True, verbose_name='Description')),
-                ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anarticle.utils.image_path, verbose_name='Cover image')),
-                ('tags', models.ManyToManyField(to='anarticle.tag', verbose_name='Tags')),
+                ('name', models.CharField(max_length=255)),
+                ('description', models.TextField(blank=True)),
+                ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anarticle.utils.image_path)),
+                ('tags', models.ManyToManyField(to='anarticle.tag')),
             ],
-            options={
-                'verbose_name': 'Category',
-                'verbose_name_plural': 'Categories',
-                'ordering': ['name'],
-            },
         ),
         migrations.AddField(
             model_name='article',
             name='tags',
-            field=models.ManyToManyField(to='anarticle.tag', verbose_name='Tags'),
+            field=models.ManyToManyField(to='anarticle.tag'),
         ),
     ]
```

### Comparing `django-anarticle-0.1.0rc1/anarticle/resolvers.py` & `django-anarticle-0.1.0rc3/anarticle/resolvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     queryset = []
     filters = []
 
     if name:
         filters.append(Q(name__icontains=name))
 
     if filters:
-        queryset = queryset.filter(reduce(operator.and_, filters)) \
+        queryset = obj.filter(reduce(operator.and_, filters)) \
                 if isinstance(obj, QuerySet) \
                 else Tag.objects.filter(reduce(operator.and_, filters))
     else:
         queryset = obj if isinstance(obj, QuerySet) \
                 else Tag.objects.all()
 
     return queryset
@@ -71,15 +71,15 @@
     if name:
         filters.append(Q(name__icontains=name))
 
     if description:
         filters.append(Q(description__icontains=description))
 
     if filters:
-        queryset = queryset.filter(reduce(operator.and_, filters)) \
+        queryset = obj.filter(reduce(operator.and_, filters)) \
                 if isinstance(obj, QuerySet) \
                 else Category.objects.filter(reduce(operator.and_, filters))
     else:
         queryset = obj if isinstance(obj, QuerySet) \
                 else Category.objects.all()
 
     return queryset
@@ -102,33 +102,35 @@
 @anarticle.connection('tags')
 def resolve_anarticle_tag_connection(obj, info, **kwargs):
     return resolve_anarticle_tags(obj.tags.all(), info, kwargs)
 
 
 @convert_kwargs_to_snake_case
 def resolve_anarticles(obj, info, **kwargs):
-    is_published = kwargs.get('is_published', True)
+    is_published = kwargs.get('is_published', None)
     published_at = kwargs.get('published_at', timezone.now())
     tags = kwargs.get('tags', '')
     title = kwargs.get('title', '')
 
     queryset = []
     filters = [
-        Q(is_published=is_published),
         Q(published_at__lt=published_at)
     ]
 
+    if is_published is not None:
+        filters.append(Q(is_published=is_published))
+
     if tags:
         values = [t.strip() for t in tags.split(',')]
         filters.append(Q(tags__name__in=values))
 
     if title:
         filters.append(Q(title__icontains=title))
 
-    queryset = queryset.filter(reduce(operator.and_, filters)) \
+    queryset = obj.filter(reduce(operator.and_, filters)) \
         if isinstance(obj, QuerySet) \
         else Article.objects.filter(reduce(operator.and_, filters))
 
     return queryset
 
 
 types = [anarticle, anarticle_paragraph, anarticle_tag, anarticle_category]
```

### Comparing `django-anarticle-0.1.0rc1/anarticle/utils.py` & `django-anarticle-0.1.0rc3/anarticle/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,19 +13,19 @@
             if len(PurePath(filename).stem) > 8 else PurePath(filename).stem
 
     cleaned_filename = (
         f"{timezone.now().strftime('%Y%m%d%H%M%S%f')}-"
         f'{fixed_filename}{PurePath(filename).suffix}'
     )
 
-    if getattr(settings, 'PUBLICATION_USE_TOKEN_FILENAME', False):
-        return PurePath('anarticle').joinpath(
+    if getattr(settings, 'ANARTICLE_USE_TOKEN_FILENAME', False):
+        return PurePath(instance._meta.app_label).joinpath(
                 f'{token_urlsafe()}{PurePath(filename).suffix}')
     else:
-        return PurePath('anarticle').joinpath(cleaned_filename)
+        return PurePath(instance._meta.app_label).joinpath(cleaned_filename)
 
 
 def image_url(instance):
     url = ''
     if instance.image:
         url = instance.image.url
```

### Comparing `django-anarticle-0.1.0rc1/django_anarticle.egg-info/SOURCES.txt` & `django-anarticle-0.1.0rc3/django_anarticle.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+.editorconfig
 .gitignore
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
 anarticle/__init__.py
 anarticle/apps.py
+anarticle/mixins.py
 anarticle/models.py
 anarticle/resolvers.py
 anarticle/tests.py
 anarticle/utils.py
-anarticle/admin/__init__.py
-anarticle/admin/mixins.py
+anarticle/graphqls/__init__.py
 anarticle/graphqls/article.graphql
+anarticle/graphqls/bindables.py
+anarticle/graphqls/bindables_sync.py
 anarticle/graphqls/category.graphql
 anarticle/graphqls/tag.graphql
+anarticle/graphqls/type_defs.py
 anarticle/migrations/0001_initial.py
 anarticle/migrations/__init__.py
 django_anarticle.egg-info/PKG-INFO
 django_anarticle.egg-info/SOURCES.txt
 django_anarticle.egg-info/dependency_links.txt
 django_anarticle.egg-info/requires.txt
 django_anarticle.egg-info/top_level.txt
+tests/__init__.py
 tests/conftest.py
 tests/test_resolvers.py
```

### Comparing `django-anarticle-0.1.0rc1/pyproject.toml` & `django-anarticle-0.1.0rc3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,48 +2,51 @@
 
 [build-system]
 requires = ["setuptools>=66.1.1", "setuptools_scm[toml]>=7.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-anarticle"
-authors = [{ name = "cchiut", email = "chiutung.chen@aglean.com"}]
-description = "App for publish articles with tags and categories"
-keywords = ["django", "aglean", "article"]
+authors = [{ name = "Chiu", email = "chiutung.chen@aglean.com"}]
+description = "App for publishing articles with tags and categories"
+keywords = ["django", "graphql", "ariadne", "aglean", "article", "tag", "category"]
 readme = "README.rst"
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"
 ]
-requires-python = ">= 3.11"
+requires-python = ">= 3.10"
 dependencies = [
     "django >= 4.0",
-    "ariadne >= 0.16.0",
-    "ariadne-relay >= 0.1.0a8",
     "pillow >= 9.4.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
+graphql = [
+    "ariadne >= 0.16.0",
+    "ariadne-relay >= 0.1.0a8",
+]
 dev = [
     "python-lsp-server[rope,pyflakes,mccabe,pycodestyle,autopep8]",
     "pylsp-rope",
-    "autoimport",
 ]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-mock",
     "pytest-django",
 ]
```

### Comparing `django-anarticle-0.1.0rc1/tests/test_resolvers.py` & `django-anarticle-0.1.0rc3/tests/test_resolvers.py`

 * *Files identical despite different names*

