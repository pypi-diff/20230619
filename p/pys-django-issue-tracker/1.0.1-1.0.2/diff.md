# Comparing `tmp/pys-django-issue-tracker-1.0.1.tar.gz` & `tmp/pys-django-issue-tracker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pys-django-issue-tracker-1.0.1.tar", last modified: Thu Jun 15 05:48:22 2023, max compression
+gzip compressed data, was "pys-django-issue-tracker-1.0.2.tar", last modified: Mon Jun 19 10:58:09 2023, max compression
```

## Comparing `pys-django-issue-tracker-1.0.1.tar` & `pys-django-issue-tracker-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/
--rw-rw-r--   0 pys       (1000) pys       (1000)     1063 2023-06-14 13:33:04.000000 pys-django-issue-tracker-1.0.1/LICENSE.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)     5848 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/PKG-INFO
--rw-rw-r--   0 pys       (1000) pys       (1000)     4490 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/README.md
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.219771 pys-django-issue-tracker-1.0.1/issue_tracker/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/__init__.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      117 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/admin.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      207 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/app_settings.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      157 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/apps.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.219771 pys-django-issue-tracker-1.0.1/issue_tracker/channels/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/__init__.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.219771 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/__init__.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1931 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/db.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1809 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/discord.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1644 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/email.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1327 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/slack.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     2288 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/teams.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      634 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/channel.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     2830 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/channels_factory.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     2621 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/middleware.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.219771 pys-django-issue-tracker-1.0.1/issue_tracker/migrations/
--rw-rw-r--   0 pys       (1000) pys       (1000)     1525 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/migrations/0001_initial.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      428 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/migrations/0002_remove_issue_content_type_remove_issue_user.py
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/migrations/__init__.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      784 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/models.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/issue_tracker/tests/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/__init__.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/__init__.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/__init__.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     2512 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/test_discord.py
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/test_teams.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1685 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_app_settings.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      881 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_channel.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     3415 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_middleware.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      984 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/conftest.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      460 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/test_channels_factory.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/
--rw-rw-r--   0 pys       (1000) pys       (1000)     5848 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 pys       (1000) pys       (1000)     1396 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)        1 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)      538 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/requires.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)       14 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/top_level.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)       78 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/setup.cfg
--rw-rw-r--   0 pys       (1000) pys       (1000)     1712 2023-06-15 05:45:00.000000 pys-django-issue-tracker-1.0.1/setup.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.704335 pys-django-issue-tracker-1.0.2/
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1063 2023-06-14 13:33:04.000000 pys-django-issue-tracker-1.0.2/LICENSE.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)     6196 2023-06-19 10:58:09.704335 pys-django-issue-tracker-1.0.2/PKG-INFO
+-rw-rw-r--   0 pys       (1000) pys       (1000)     4795 2023-06-19 10:57:30.000000 pys-django-issue-tracker-1.0.2/README.md
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.696335 pys-django-issue-tracker-1.0.2/issue_tracker/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/__init__.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      117 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/admin.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      486 2023-06-19 10:57:30.000000 pys-django-issue-tracker-1.0.2/issue_tracker/app_settings.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      157 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/apps.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.700335 pys-django-issue-tracker-1.0.2/issue_tracker/channels/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/__init__.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.700335 pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/__init__.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1931 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/db.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1809 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/discord.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1644 2023-06-16 09:16:42.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/email.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1327 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/slack.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     2288 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/teams.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      634 2023-06-15 07:15:15.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/channel.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     2830 2023-06-19 09:14:42.000000 pys-django-issue-tracker-1.0.2/issue_tracker/channels/channels_factory.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     2621 2023-06-19 08:41:56.000000 pys-django-issue-tracker-1.0.2/issue_tracker/middleware.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.700335 pys-django-issue-tracker-1.0.2/issue_tracker/migrations/
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1525 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/migrations/0001_initial.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      428 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/migrations/0002_remove_issue_content_type_remove_issue_user.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/migrations/__init__.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      784 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/models.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.700335 pys-django-issue-tracker-1.0.2/issue_tracker/templates/
+-rw-rw-r--   0 pys       (1000) pys       (1000)     6140 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/templates/issue_notifire.html
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.700335 pys-django-issue-tracker-1.0.2/issue_tracker/tests/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/__init__.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.700335 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/__init__.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.700335 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/backends/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/backends/__init__.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     2512 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/backends/test_discord.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/backends/test_teams.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1685 2023-06-19 09:55:28.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/test_app_settings.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      881 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/test_channel.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     3415 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/test_middleware.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      984 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/conftest.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      460 2023-06-19 09:56:03.000000 pys-django-issue-tracker-1.0.2/issue_tracker/tests/test_channels_factory.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-19 10:58:09.704335 pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/
+-rw-rw-r--   0 pys       (1000) pys       (1000)     6196 2023-06-19 10:58:09.000000 pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1440 2023-06-19 10:58:09.000000 pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)        1 2023-06-19 10:58:09.000000 pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)      538 2023-06-19 10:58:09.000000 pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/requires.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)       14 2023-06-19 10:58:09.000000 pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)       78 2023-06-19 10:58:09.704335 pys-django-issue-tracker-1.0.2/setup.cfg
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1859 2023-06-19 10:57:30.000000 pys-django-issue-tracker-1.0.2/setup.py
```

### Comparing `pys-django-issue-tracker-1.0.1/LICENSE.txt` & `pys-django-issue-tracker-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/PKG-INFO` & `pys-django-issue-tracker-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pys-django-issue-tracker
-Version: 1.0.1
+Version: 1.0.2
 Summary: Django Issue tracker
 Home-page: https://github.com/pys-info/pys-issue-tracker
 Author: Pysquad
 Author-email: vh@pysquad.com
-License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/pys-info/pys-issue-tracker/issues
 Project-URL: Source, https://github.com/pys-info/pys-issue-tracker
 Keywords: django,issue,tracker,development
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
@@ -76,29 +75,36 @@
     "TEAMS": {
         "BACKEND": "issue_tracker.channels.backends.teams.TeamsChannel",
         "WEBHOOK_URL": <"TEAMS_WEBHOOK_URL">,
     },
     "EMAIL": {
         "BACKEND": "issue_tracker.channels.backends.email.EmailChannel",
     },
+    # If you are using EMAIL in above configuration you must need to configure EMAIL Configuration with EMAIL_ADMIN_USER and EMAIL_HOST_USER in settings.py
     "DB": {
         "BACKEND": "issue_tracker.channels.backends.db.DBChannel",
     },
-    "SLACk": {
+    "SLACK": {
         "BACKEND": "issue_tracker.channels.backends.slack.SlackChannel",
         "WEBHOOK_URL": <"SLACK_WEBHOOK_URL">,
     }
     ...
 }
 
     INSTALLED_APPS = [
         ...
         # The following apps is required:
        issue_tracker,
     ]
+
+    MIDDLEWARE = [
+        ...
+        # The following middleware is required:
+        'issue_tracker.middleware.ErrorNotificationMiddleware'
+    ]
 ## Acknowledgements
  - We would like to express our gratitude to the following individuals and organizations for their contributions, support, and inspiration:
    - PySquad Informatics LLP(https://pysquad.com/)
 
  - We also want to extend our thanks to the open-source community for their continuous efforts and contributions to the Python ecosystem. We greatly appreciate the work of all the developers, contributors, and maintainers of the libraries and frameworks that this package relies on.
  - Finally, we would like to thank our users for their feedback, bug reports, and feature requests. Your input has been invaluable in shaping the evolution of this package.
  - We are grateful to everyone who has played a part in making this package what it is today, and we look forward to continued collaboration and improvement in the future.
@@ -112,8 +118,7 @@
 -  Release version related information you can get inside the release-notes documents.See details information inside `docs/release-notes.rst`
 
 ## License
 *MIT License:* <https://choosealicense.com/licenses/mit/>
 
 ## Contact
 For any inquiries or feedback, you can reach us at xyz@example.com or join our community channel.
-
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: pys-django-issue-tracker Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: pys-django-issue-tracker Version: 1.0.2 Summary:
 Django Issue tracker Home-page: https://github.com/pys-info/pys-issue-tracker
-Author: Pysquad Author-email: vh@pysquad.com License: UNKNOWN Project-URL:
-Source, https://github.com/pys-info/pys-issue-tracker Keywords:
-django,issue,tracker,development Platform: UNKNOWN Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
-OSI Approved :: MIT License Classifier: Environment :: Web Environment
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Framework :: Django Classifier: Framework ::
-Django :: 3.0 Classifier: Framework :: Django :: 3.1 Classifier: Framework ::
-Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework ::
-Django :: 4.1 Classifier: Framework :: Django :: 4.2 Requires-Python: >=3.5
-Description-Content-Type: text/markdown License-File: LICENSE.txt
+Author: Pysquad Author-email: vh@pysquad.com Project-URL: Bug Reports, https://
+github.com/pys-info/pys-issue-tracker/issues Project-URL: Source, https://
+github.com/pys-info/pys-issue-tracker Keywords:
+django,issue,tracker,development Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
+:: Software Development :: Build Tools Classifier: License :: OSI Approved ::
+MIT License Classifier: Environment :: Web Environment Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Framework :: Django Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2 Requires-Python: >=3.5 Description-
+Content-Type: text/markdown License-File: LICENSE.txt
 ****** django-issue-tracker ******
 **[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/)** [Made_with_Django.] ## Project
 description Django Issue Tracker is a robust package designed to streamline
 issue tracking within Django web applications.The package supports various
 notification channels, allowing teams to receive updates through their
 preferred communication methods.By integrating this package, teams can
@@ -37,39 +38,42 @@
 install django-issue-tracker settings.py (Please note that below settings is
 required as INSTALLED_APPS):: # Specify channels configuration as follows:
 ISSUE_TRACKER_CHANNELS_CONFIGURATION = { "DISCORD": { "BACKEND":
 "issue_tracker.channels.backends.discord.DiscordChannel", "WEBHOOK_URL":
 <"DISCORD_WEBHOOK_URL">, }, "TEAMS": { "BACKEND":
 "issue_tracker.channels.backends.teams.TeamsChannel", "WEBHOOK_URL":
 <"TEAMS_WEBHOOK_URL">, }, "EMAIL": { "BACKEND":
-"issue_tracker.channels.backends.email.EmailChannel", }, "DB": { "BACKEND":
-"issue_tracker.channels.backends.db.DBChannel", }, "SLACk": { "BACKEND":
+"issue_tracker.channels.backends.email.EmailChannel", }, # If you are using
+EMAIL in above configuration you must need to configure EMAIL Configuration
+with EMAIL_ADMIN_USER and EMAIL_HOST_USER in settings.py "DB": { "BACKEND":
+"issue_tracker.channels.backends.db.DBChannel", }, "SLACK": { "BACKEND":
 "issue_tracker.channels.backends.slack.SlackChannel", "WEBHOOK_URL":
 <"SLACK_WEBHOOK_URL">, } ... } INSTALLED_APPS = [ ... # The following apps is
-required: issue_tracker, ] ## Acknowledgements - We would like to express our
-gratitude to the following individuals and organizations for their
-contributions, support, and inspiration: - PySquad Informatics LLP(https://
-pysquad.com/) - We also want to extend our thanks to the open-source community
-for their continuous efforts and contributions to the Python ecosystem. We
-greatly appreciate the work of all the developers, contributors, and
-maintainers of the libraries and frameworks that this package relies on. -
-Finally, we would like to thank our users for their feedback, bug reports, and
-feature requests. Your input has been invaluable in shaping the evolution of
-this package. - We are grateful to everyone who has played a part in making
-this package what it is today, and we look forward to continued collaboration
-and improvement in the future. ## Configuration - The package can be configured
-using configuration file or enviroment variable.Refer to the configuration
-documentation for details information on available setting and customization
-options.See details information inside `docs/configuration.rst`. -
-Troubleshooting and Support If you encounter any issues or have questions,
-please visit our support page or check out the FAQs for common troubleshooting
-steps and answers to frequently asked questions. See details information inside
-`docs/faq.rst`. - Changelog to see the full history of changes made to the
-package.please refer to the changlog.See details information inside
-`ChangLog.rst`. - This packages is licenced under the MIT Licence.See details
-information inside`License`. - Refer to the Channels documentation for details
-information on available channels.See details information inside `docs/
-channels.rst` - Release version related information you can get inside the
-release-notes documents.See details information inside `docs/release-notes.rst`
-## License *MIT License:*
+required: issue_tracker, ] MIDDLEWARE = [ ... # The following middleware is
+required: 'issue_tracker.middleware.ErrorNotificationMiddleware' ] ##
+Acknowledgements - We would like to express our gratitude to the following
+individuals and organizations for their contributions, support, and
+inspiration: - PySquad Informatics LLP(https://pysquad.com/) - We also want to
+extend our thanks to the open-source community for their continuous efforts and
+contributions to the Python ecosystem. We greatly appreciate the work of all
+the developers, contributors, and maintainers of the libraries and frameworks
+that this package relies on. - Finally, we would like to thank our users for
+their feedback, bug reports, and feature requests. Your input has been
+invaluable in shaping the evolution of this package. - We are grateful to
+everyone who has played a part in making this package what it is today, and we
+look forward to continued collaboration and improvement in the future. ##
+Configuration - The package can be configured using configuration file or
+enviroment variable.Refer to the configuration documentation for details
+information on available setting and customization options.See details
+information inside `docs/configuration.rst`. - Troubleshooting and Support If
+you encounter any issues or have questions, please visit our support page or
+check out the FAQs for common troubleshooting steps and answers to frequently
+asked questions. See details information inside `docs/faq.rst`. - Changelog to
+see the full history of changes made to the package.please refer to the
+changlog.See details information inside `ChangLog.rst`. - This packages is
+licenced under the MIT Licence.See details information inside`License`. - Refer
+to the Channels documentation for details information on available channels.See
+details information inside `docs/channels.rst` - Release version related
+information you can get inside the release-notes documents.See details
+information inside `docs/release-notes.rst` ## License *MIT License:*
 choosealicense.com/licenses/mit/> ## Contact For any inquiries or feedback, you
 can reach us at xyz@example.com or join our community channel.
```

### Comparing `pys-django-issue-tracker-1.0.1/README.md` & `pys-django-issue-tracker-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,29 +41,36 @@
     "TEAMS": {
         "BACKEND": "issue_tracker.channels.backends.teams.TeamsChannel",
         "WEBHOOK_URL": <"TEAMS_WEBHOOK_URL">,
     },
     "EMAIL": {
         "BACKEND": "issue_tracker.channels.backends.email.EmailChannel",
     },
+    # If you are using EMAIL in above configuration you must need to configure EMAIL Configuration with EMAIL_ADMIN_USER and EMAIL_HOST_USER in settings.py
     "DB": {
         "BACKEND": "issue_tracker.channels.backends.db.DBChannel",
     },
-    "SLACk": {
+    "SLACK": {
         "BACKEND": "issue_tracker.channels.backends.slack.SlackChannel",
         "WEBHOOK_URL": <"SLACK_WEBHOOK_URL">,
     }
     ...
 }
 
     INSTALLED_APPS = [
         ...
         # The following apps is required:
        issue_tracker,
     ]
+
+    MIDDLEWARE = [
+        ...
+        # The following middleware is required:
+        'issue_tracker.middleware.ErrorNotificationMiddleware'
+    ]
 ## Acknowledgements
  - We would like to express our gratitude to the following individuals and organizations for their contributions, support, and inspiration:
    - PySquad Informatics LLP(https://pysquad.com/)
 
  - We also want to extend our thanks to the open-source community for their continuous efforts and contributions to the Python ecosystem. We greatly appreciate the work of all the developers, contributors, and maintainers of the libraries and frameworks that this package relies on.
  - Finally, we would like to thank our users for their feedback, bug reports, and feature requests. Your input has been invaluable in shaping the evolution of this package.
  - We are grateful to everyone who has played a part in making this package what it is today, and we look forward to continued collaboration and improvement in the future.
```

#### html2text {}

```diff
@@ -19,39 +19,42 @@
 install django-issue-tracker settings.py (Please note that below settings is
 required as INSTALLED_APPS):: # Specify channels configuration as follows:
 ISSUE_TRACKER_CHANNELS_CONFIGURATION = { "DISCORD": { "BACKEND":
 "issue_tracker.channels.backends.discord.DiscordChannel", "WEBHOOK_URL":
 <"DISCORD_WEBHOOK_URL">, }, "TEAMS": { "BACKEND":
 "issue_tracker.channels.backends.teams.TeamsChannel", "WEBHOOK_URL":
 <"TEAMS_WEBHOOK_URL">, }, "EMAIL": { "BACKEND":
-"issue_tracker.channels.backends.email.EmailChannel", }, "DB": { "BACKEND":
-"issue_tracker.channels.backends.db.DBChannel", }, "SLACk": { "BACKEND":
+"issue_tracker.channels.backends.email.EmailChannel", }, # If you are using
+EMAIL in above configuration you must need to configure EMAIL Configuration
+with EMAIL_ADMIN_USER and EMAIL_HOST_USER in settings.py "DB": { "BACKEND":
+"issue_tracker.channels.backends.db.DBChannel", }, "SLACK": { "BACKEND":
 "issue_tracker.channels.backends.slack.SlackChannel", "WEBHOOK_URL":
 <"SLACK_WEBHOOK_URL">, } ... } INSTALLED_APPS = [ ... # The following apps is
-required: issue_tracker, ] ## Acknowledgements - We would like to express our
-gratitude to the following individuals and organizations for their
-contributions, support, and inspiration: - PySquad Informatics LLP(https://
-pysquad.com/) - We also want to extend our thanks to the open-source community
-for their continuous efforts and contributions to the Python ecosystem. We
-greatly appreciate the work of all the developers, contributors, and
-maintainers of the libraries and frameworks that this package relies on. -
-Finally, we would like to thank our users for their feedback, bug reports, and
-feature requests. Your input has been invaluable in shaping the evolution of
-this package. - We are grateful to everyone who has played a part in making
-this package what it is today, and we look forward to continued collaboration
-and improvement in the future. ## Configuration - The package can be configured
-using configuration file or enviroment variable.Refer to the configuration
-documentation for details information on available setting and customization
-options.See details information inside `docs/configuration.rst`. -
-Troubleshooting and Support If you encounter any issues or have questions,
-please visit our support page or check out the FAQs for common troubleshooting
-steps and answers to frequently asked questions. See details information inside
-`docs/faq.rst`. - Changelog to see the full history of changes made to the
-package.please refer to the changlog.See details information inside
-`ChangLog.rst`. - This packages is licenced under the MIT Licence.See details
-information inside`License`. - Refer to the Channels documentation for details
-information on available channels.See details information inside `docs/
-channels.rst` - Release version related information you can get inside the
-release-notes documents.See details information inside `docs/release-notes.rst`
-## License *MIT License:*
+required: issue_tracker, ] MIDDLEWARE = [ ... # The following middleware is
+required: 'issue_tracker.middleware.ErrorNotificationMiddleware' ] ##
+Acknowledgements - We would like to express our gratitude to the following
+individuals and organizations for their contributions, support, and
+inspiration: - PySquad Informatics LLP(https://pysquad.com/) - We also want to
+extend our thanks to the open-source community for their continuous efforts and
+contributions to the Python ecosystem. We greatly appreciate the work of all
+the developers, contributors, and maintainers of the libraries and frameworks
+that this package relies on. - Finally, we would like to thank our users for
+their feedback, bug reports, and feature requests. Your input has been
+invaluable in shaping the evolution of this package. - We are grateful to
+everyone who has played a part in making this package what it is today, and we
+look forward to continued collaboration and improvement in the future. ##
+Configuration - The package can be configured using configuration file or
+enviroment variable.Refer to the configuration documentation for details
+information on available setting and customization options.See details
+information inside `docs/configuration.rst`. - Troubleshooting and Support If
+you encounter any issues or have questions, please visit our support page or
+check out the FAQs for common troubleshooting steps and answers to frequently
+asked questions. See details information inside `docs/faq.rst`. - Changelog to
+see the full history of changes made to the package.please refer to the
+changlog.See details information inside `ChangLog.rst`. - This packages is
+licenced under the MIT Licence.See details information inside`License`. - Refer
+to the Channels documentation for details information on available channels.See
+details information inside `docs/channels.rst` - Release version related
+information you can get inside the release-notes documents.See details
+information inside `docs/release-notes.rst` ## License *MIT License:*
 choosealicense.com/licenses/mit/> ## Contact For any inquiries or feedback, you
 can reach us at xyz@example.com or join our community channel.
```

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/db.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/db.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/discord.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/discord.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/email.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/email.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/slack.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/slack.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/teams.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/channels/backends/teams.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/channels/channel.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/channels/channel.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/channels/channels_factory.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/channels/channels_factory.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/middleware.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/middleware.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/migrations/0001_initial.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/models.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/models.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/test_discord.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/backends/test_discord.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_app_settings.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_channel.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/test_channel.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_middleware.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/tests/channels/test_middleware.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/issue_tracker/tests/conftest.py` & `pys-django-issue-tracker-1.0.2/issue_tracker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/PKG-INFO` & `pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pys-django-issue-tracker
-Version: 1.0.1
+Version: 1.0.2
 Summary: Django Issue tracker
 Home-page: https://github.com/pys-info/pys-issue-tracker
 Author: Pysquad
 Author-email: vh@pysquad.com
-License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/pys-info/pys-issue-tracker/issues
 Project-URL: Source, https://github.com/pys-info/pys-issue-tracker
 Keywords: django,issue,tracker,development
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
@@ -76,29 +75,36 @@
     "TEAMS": {
         "BACKEND": "issue_tracker.channels.backends.teams.TeamsChannel",
         "WEBHOOK_URL": <"TEAMS_WEBHOOK_URL">,
     },
     "EMAIL": {
         "BACKEND": "issue_tracker.channels.backends.email.EmailChannel",
     },
+    # If you are using EMAIL in above configuration you must need to configure EMAIL Configuration with EMAIL_ADMIN_USER and EMAIL_HOST_USER in settings.py
     "DB": {
         "BACKEND": "issue_tracker.channels.backends.db.DBChannel",
     },
-    "SLACk": {
+    "SLACK": {
         "BACKEND": "issue_tracker.channels.backends.slack.SlackChannel",
         "WEBHOOK_URL": <"SLACK_WEBHOOK_URL">,
     }
     ...
 }
 
     INSTALLED_APPS = [
         ...
         # The following apps is required:
        issue_tracker,
     ]
+
+    MIDDLEWARE = [
+        ...
+        # The following middleware is required:
+        'issue_tracker.middleware.ErrorNotificationMiddleware'
+    ]
 ## Acknowledgements
  - We would like to express our gratitude to the following individuals and organizations for their contributions, support, and inspiration:
    - PySquad Informatics LLP(https://pysquad.com/)
 
  - We also want to extend our thanks to the open-source community for their continuous efforts and contributions to the Python ecosystem. We greatly appreciate the work of all the developers, contributors, and maintainers of the libraries and frameworks that this package relies on.
  - Finally, we would like to thank our users for their feedback, bug reports, and feature requests. Your input has been invaluable in shaping the evolution of this package.
  - We are grateful to everyone who has played a part in making this package what it is today, and we look forward to continued collaboration and improvement in the future.
@@ -112,8 +118,7 @@
 -  Release version related information you can get inside the release-notes documents.See details information inside `docs/release-notes.rst`
 
 ## License
 *MIT License:* <https://choosealicense.com/licenses/mit/>
 
 ## Contact
 For any inquiries or feedback, you can reach us at xyz@example.com or join our community channel.
-
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: pys-django-issue-tracker Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: pys-django-issue-tracker Version: 1.0.2 Summary:
 Django Issue tracker Home-page: https://github.com/pys-info/pys-issue-tracker
-Author: Pysquad Author-email: vh@pysquad.com License: UNKNOWN Project-URL:
-Source, https://github.com/pys-info/pys-issue-tracker Keywords:
-django,issue,tracker,development Platform: UNKNOWN Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
-OSI Approved :: MIT License Classifier: Environment :: Web Environment
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Framework :: Django Classifier: Framework ::
-Django :: 3.0 Classifier: Framework :: Django :: 3.1 Classifier: Framework ::
-Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework ::
-Django :: 4.1 Classifier: Framework :: Django :: 4.2 Requires-Python: >=3.5
-Description-Content-Type: text/markdown License-File: LICENSE.txt
+Author: Pysquad Author-email: vh@pysquad.com Project-URL: Bug Reports, https://
+github.com/pys-info/pys-issue-tracker/issues Project-URL: Source, https://
+github.com/pys-info/pys-issue-tracker Keywords:
+django,issue,tracker,development Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
+:: Software Development :: Build Tools Classifier: License :: OSI Approved ::
+MIT License Classifier: Environment :: Web Environment Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Framework :: Django Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2 Requires-Python: >=3.5 Description-
+Content-Type: text/markdown License-File: LICENSE.txt
 ****** django-issue-tracker ******
 **[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/)** [Made_with_Django.] ## Project
 description Django Issue Tracker is a robust package designed to streamline
 issue tracking within Django web applications.The package supports various
 notification channels, allowing teams to receive updates through their
 preferred communication methods.By integrating this package, teams can
@@ -37,39 +38,42 @@
 install django-issue-tracker settings.py (Please note that below settings is
 required as INSTALLED_APPS):: # Specify channels configuration as follows:
 ISSUE_TRACKER_CHANNELS_CONFIGURATION = { "DISCORD": { "BACKEND":
 "issue_tracker.channels.backends.discord.DiscordChannel", "WEBHOOK_URL":
 <"DISCORD_WEBHOOK_URL">, }, "TEAMS": { "BACKEND":
 "issue_tracker.channels.backends.teams.TeamsChannel", "WEBHOOK_URL":
 <"TEAMS_WEBHOOK_URL">, }, "EMAIL": { "BACKEND":
-"issue_tracker.channels.backends.email.EmailChannel", }, "DB": { "BACKEND":
-"issue_tracker.channels.backends.db.DBChannel", }, "SLACk": { "BACKEND":
+"issue_tracker.channels.backends.email.EmailChannel", }, # If you are using
+EMAIL in above configuration you must need to configure EMAIL Configuration
+with EMAIL_ADMIN_USER and EMAIL_HOST_USER in settings.py "DB": { "BACKEND":
+"issue_tracker.channels.backends.db.DBChannel", }, "SLACK": { "BACKEND":
 "issue_tracker.channels.backends.slack.SlackChannel", "WEBHOOK_URL":
 <"SLACK_WEBHOOK_URL">, } ... } INSTALLED_APPS = [ ... # The following apps is
-required: issue_tracker, ] ## Acknowledgements - We would like to express our
-gratitude to the following individuals and organizations for their
-contributions, support, and inspiration: - PySquad Informatics LLP(https://
-pysquad.com/) - We also want to extend our thanks to the open-source community
-for their continuous efforts and contributions to the Python ecosystem. We
-greatly appreciate the work of all the developers, contributors, and
-maintainers of the libraries and frameworks that this package relies on. -
-Finally, we would like to thank our users for their feedback, bug reports, and
-feature requests. Your input has been invaluable in shaping the evolution of
-this package. - We are grateful to everyone who has played a part in making
-this package what it is today, and we look forward to continued collaboration
-and improvement in the future. ## Configuration - The package can be configured
-using configuration file or enviroment variable.Refer to the configuration
-documentation for details information on available setting and customization
-options.See details information inside `docs/configuration.rst`. -
-Troubleshooting and Support If you encounter any issues or have questions,
-please visit our support page or check out the FAQs for common troubleshooting
-steps and answers to frequently asked questions. See details information inside
-`docs/faq.rst`. - Changelog to see the full history of changes made to the
-package.please refer to the changlog.See details information inside
-`ChangLog.rst`. - This packages is licenced under the MIT Licence.See details
-information inside`License`. - Refer to the Channels documentation for details
-information on available channels.See details information inside `docs/
-channels.rst` - Release version related information you can get inside the
-release-notes documents.See details information inside `docs/release-notes.rst`
-## License *MIT License:*
+required: issue_tracker, ] MIDDLEWARE = [ ... # The following middleware is
+required: 'issue_tracker.middleware.ErrorNotificationMiddleware' ] ##
+Acknowledgements - We would like to express our gratitude to the following
+individuals and organizations for their contributions, support, and
+inspiration: - PySquad Informatics LLP(https://pysquad.com/) - We also want to
+extend our thanks to the open-source community for their continuous efforts and
+contributions to the Python ecosystem. We greatly appreciate the work of all
+the developers, contributors, and maintainers of the libraries and frameworks
+that this package relies on. - Finally, we would like to thank our users for
+their feedback, bug reports, and feature requests. Your input has been
+invaluable in shaping the evolution of this package. - We are grateful to
+everyone who has played a part in making this package what it is today, and we
+look forward to continued collaboration and improvement in the future. ##
+Configuration - The package can be configured using configuration file or
+enviroment variable.Refer to the configuration documentation for details
+information on available setting and customization options.See details
+information inside `docs/configuration.rst`. - Troubleshooting and Support If
+you encounter any issues or have questions, please visit our support page or
+check out the FAQs for common troubleshooting steps and answers to frequently
+asked questions. See details information inside `docs/faq.rst`. - Changelog to
+see the full history of changes made to the package.please refer to the
+changlog.See details information inside `ChangLog.rst`. - This packages is
+licenced under the MIT Licence.See details information inside`License`. - Refer
+to the Channels documentation for details information on available channels.See
+details information inside `docs/channels.rst` - Release version related
+information you can get inside the release-notes documents.See details
+information inside `docs/release-notes.rst` ## License *MIT License:*
 choosealicense.com/licenses/mit/> ## Contact For any inquiries or feedback, you
 can reach us at xyz@example.com or join our community channel.
```

### Comparing `pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/SOURCES.txt` & `pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 issue_tracker/channels/backends/discord.py
 issue_tracker/channels/backends/email.py
 issue_tracker/channels/backends/slack.py
 issue_tracker/channels/backends/teams.py
 issue_tracker/migrations/0001_initial.py
 issue_tracker/migrations/0002_remove_issue_content_type_remove_issue_user.py
 issue_tracker/migrations/__init__.py
+issue_tracker/templates/issue_notifire.html
 issue_tracker/tests/__init__.py
 issue_tracker/tests/conftest.py
 issue_tracker/tests/test_channels_factory.py
 issue_tracker/tests/channels/__init__.py
 issue_tracker/tests/channels/test_app_settings.py
 issue_tracker/tests/channels/test_channel.py
 issue_tracker/tests/channels/test_middleware.py
```

### Comparing `pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/requires.txt` & `pys-django-issue-tracker-1.0.2/pys_django_issue_tracker.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Django==4.2.1
-PyYAML==6.0
 asgiref==3.6.0
 certifi==2023.5.7
 cfgv==3.3.1
 charset-normalizer==3.1.0
 coverage==7.2.5
 discord-webhook==1.1.0
 distlib==0.3.6
+Django==4.2.1
 exceptiongroup==1.1.1
 filelock==3.12.0
 identify==2.5.24
 idna==3.4
 iniconfig==2.0.0
 mocker==1.1.1
 nodeenv==1.8.0
 packaging==23.1
 platformdirs==3.5.1
 pluggy==1.0.0
 pre-commit==3.3.2
 pymsteams==0.2.2
+pytest==7.3.1
 pytest-cov==4.0.0
 pytest-django==4.5.2
-pytest==7.3.1
 python-dotenv==1.0.0
+PyYAML==6.0
 requests==2.30.0
 slack-sdk==3.21.3
 sqlparse==0.4.4
 timestamp==0.0.1
 tomli==2.0.1
 urllib3==2.0.2
 virtualenv==20.23.0
```

### Comparing `pys-django-issue-tracker-1.0.1/setup.py` & `pys-django-issue-tracker-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pys-django-issue-tracker",
-    version="1.0.1",
+    version="1.0.2",
     author="Pysquad",
     author_email="vh@pysquad.com",
     description="Django Issue tracker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pys-info/pys-issue-tracker",
+    package_data={
+        'issue_tracker': ['templates/*'],
+    },
     install_requires=[line.strip() for line in open("requirements.txt")],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Environment :: Web Environment",
@@ -38,10 +41,11 @@
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
     ],
     keywords="django, issue, tracker, development",
     packages=find_packages(exclude=("example")),
     python_requires=">=3.5",
     project_urls={
+        "Bug Reports": "https://github.com/pys-info/pys-issue-tracker/issues",
         "Source": "https://github.com/pys-info/pys-issue-tracker",
     },
 )
```

