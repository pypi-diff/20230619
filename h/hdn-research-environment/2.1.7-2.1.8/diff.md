# Comparing `tmp/hdn-research-environment-2.1.7.tar.gz` & `tmp/hdn-research-environment-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.1.7.tar", last modified: Thu Jun 15 15:57:28 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.1.8.tar", last modified: Mon Jun 19 11:06:09 2023, max compression
```

## Comparing `hdn-research-environment-2.1.7.tar` & `hdn-research-environment-2.1.8.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.7/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.7/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.7/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.7/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.7/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.7/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-05 16:43:26.000000 hdn-research-environment-2.1.7/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.7/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.7/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.7/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    19730 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.7/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.1.7/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.7/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.7/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      291 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.7/environment/static/environment/js/forms.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.7/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     8010 2023-06-09 09:47:58.000000 hdn-research-environment-2.1.7/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.1.7/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.7/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1073 2023-06-09 13:14:55.000000 hdn-research-environment-2.1.7/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4417 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.7/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1149 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.7/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.7/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.7/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.1.7/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.7/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.7/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3870 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.7/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.7/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.7/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.7/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.7/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.7/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    14044 2023-06-15 15:38:02.000000 hdn-research-environment-2.1.7/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     3143 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.7/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-15 15:57:28.000000 hdn-research-environment-2.1.7/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.7/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.8/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.8/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.8/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.8/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.8/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.8/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-06-18 19:04:20.000000 hdn-research-environment-2.1.8/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    20237 2023-06-19 11:01:13.000000 hdn-research-environment-2.1.8/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.8/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.8/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      291 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/static/environment/js/forms.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6839 2023-06-19 11:01:13.000000 hdn-research-environment-2.1.8/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1537 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3305 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/_environment_tabs.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1073 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4417 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1149 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1163 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1649 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-19 10:22:33.000000 hdn-research-environment-2.1.8/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.8/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.8/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.8/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    14586 2023-06-19 11:01:13.000000 hdn-research-environment-2.1.8/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3200 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.8/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-19 11:06:09.000000 hdn-research-environment-2.1.8/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.8/setup.py
```

### Comparing `hdn-research-environment-2.1.7/LICENSE` & `hdn-research-environment-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/PKG-INFO` & `hdn-research-environment-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.7
+Version: 2.1.8
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.7/environment/api/v1/__init__.py` & `hdn-research-environment-2.1.8/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/api/v1/auth.py` & `hdn-research-environment-2.1.8/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/api/v1/decorators.py` & `hdn-research-environment-2.1.8/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/api/v2/__init__.py` & `hdn-research-environment-2.1.8/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/api/v2/decorators.py` & `hdn-research-environment-2.1.8/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/constants.py` & `hdn-research-environment-2.1.8/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/decorators.py` & `hdn-research-environment-2.1.8/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/deserializers.py` & `hdn-research-environment-2.1.8/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/entities.py` & `hdn-research-environment-2.1.8/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/exceptions.py` & `hdn-research-environment-2.1.8/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/forms.py` & `hdn-research-environment-2.1.8/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/mailers.py` & `hdn-research-environment-2.1.8/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/migrations/0001_initial.py` & `hdn-research-environment-2.1.8/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.1.8/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.1.8/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.1.8/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.1.8/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/models.py` & `hdn-research-environment-2.1.8/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/services.py` & `hdn-research-environment-2.1.8/environment/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,7 +592,19 @@
     running_workspaces = get_workspaces_list(user)
     if len(running_workspaces) >= constants.MAX_RUNNING_WORKSPACES:
         quotas_exceeded.append(
             f"You can only have {constants.MAX_RUNNING_WORKSPACES} running workspaces."
         )
 
     return quotas_exceeded
+
+
+def workflow_finished_message(workflow: Workflow) -> Optional[str]:
+    if workflow.status == Workflow.SUCCESS:
+        return None
+
+    workflow_type_failure_messages = {
+        Workflow.WORKSPACE_CREATE: "Please retry the action. If the error persists, it's likely that the billing account quota was exceeded.",
+        Workflow.CREATE: "This is likely caused by insufficient cloud resources at the moment. Please retry the action.",
+    }
+
+    return workflow_type_failure_messages.get(workflow.type)
```

### Comparing `hdn-research-environment-2.1.7/environment/signals.py` & `hdn-research-environment-2.1.8/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.1.8/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.1.8/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.1.8/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.1.8/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tasks.py` & `hdn-research-environment-2.1.8/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.1.8/environment/templates/environment/_available_environments_list.html`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 {% if recent_workflow %}
     {% if recent_workflow_failed %}
     <div class="alert alert-danger" role="alert">
             {{ recent_workflow.get_type_display }}
             {% if recent_workflow.project %}
                 {{ recent_workflow.project }}
             {% endif %}
-            failed! Try again later.
+            failed! {{ workflow_finished_message }}
         </div>
     {% elif recent_workflow_succeeded %}
         <div class="alert alert-success" role="alert">
             {{ recent_workflow.get_type_display }}
             {% if recent_workflow.project %}
                 {{ recent_workflow.project }}
             {% endif %}
-            finished!
+            finished! {{ workflow_finished_message }}
         </div>
     {% endif %}
 {% endif %}
 
 <div class="d-flex flex-column align-items-end px-4 mb-3">
     <a class="btn btn-primary btn-sm" href="{% url 'create_workspace' %}">
       + Workspace
@@ -117,42 +117,7 @@
                         {% endif %}
                     </div>
                 </div>
             </div>
         {% endwith %}
     {% endfor %}
 </div>
-
-<script>
-    function refreshEnvironmentsCard(executionId) {
-        fetchNewEnvironmentsCard(executionId)
-        .then(html => $("#environments").html(html));
-    }
-
-    function pollExecutionStatus(executionId) {
-        const pollUrl = `{% url "check_execution_status" %}?execution_resource_name=${executionId}`;
-        fetch(pollUrl)
-        .then(response => response.json())
-        .then(({ finished }) => {
-            if (finished) {
-                refreshEnvironmentsCard(executionId);
-            } else {
-                scheduleExecutionPolling(executionId);
-            }
-        });
-    }
-
-    function scheduleExecutionPolling(executionId, immediate=false) {
-        const timeout = immediate ? 0 : 30000;
-        setTimeout(() => pollExecutionStatus(executionId), timeout);
-    }
-
-    {% for environment, project, workflows in environment_project_workflow_triplets %}
-        {% for workflow in workflows %}
-            scheduleExecutionPolling("{{ workflow.execution_resource_name }}", true);
-        {% endfor %}
-    {% endfor %}
-
-    {% for workflow in workspace_creation_workflows %}
-        scheduleExecutionPolling("{{ workflow.execution_resource_name }}", true);
-    {% endfor %}
-</script>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 {% load action_buttons %} {% if recent_workflow %} {% if recent_workflow_failed
 %}
 {{ recent_workflow.get_type_display }} {% if recent_workflow.project %} {
-{ recent_workflow.project }} {% endif %} failed! Try again later.
+{ recent_workflow.project }} {% endif %} failed! {{ workflow_finished_message
+}}
 {% elif recent_workflow_succeeded %}
 {{ recent_workflow.get_type_display }} {% if recent_workflow.project %} {
-{ recent_workflow.project }} {% endif %} finished!
+{ recent_workflow.project }} {% endif %} finished! {{ workflow_finished_message
+}}
 {% endif %} {% endif %}
 +_Workspace
 {% for workflow in workspace_creation_workflows %}
 {{ heading }}">
 Provisioning
 Loading...
 {% endfor %} {% for workspace, environments_project_workflow_triplets in
@@ -39,8 +41,7 @@
       endif %}
     * {% endfor %}
 {% else %}
 You don't have any workbenches in this workspace.
 Create one in the "Projects" tab.
 {% endif %}
 {% endwith %} {% endfor %}
-
```

### Comparing `hdn-research-environment-2.1.7/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.1.8/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.1.8/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.1.8/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.1.8/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.1.8/environment/templates/environment/identity_provisioning.html`

 * *Files 22% similar despite different names*

```diff
@@ -11,81 +11,63 @@
 000000a0: 2072 656c 3d22 7374 796c 6573 6865 6574   rel="stylesheet
 000000b0: 2220 7479 7065 3d22 7465 7874 2f63 7373  " type="text/css
 000000c0: 2220 6872 6566 3d22 7b25 2073 7461 7469  " href="{% stati
 000000d0: 6320 2765 6e76 6972 6f6e 6d65 6e74 2f63  c 'environment/c
 000000e0: 7373 2f65 6e76 6972 6f6e 6d65 6e74 2d62  ss/environment-b
 000000f0: 6173 652e 6373 7327 2025 7d22 3e0a 7b25  ase.css' %}">.{%
 00000100: 2065 6e64 626c 6f63 6b20 257d 0a0a 7b25   endblock %}..{%
-00000110: 2062 6c6f 636b 2063 6f6e 7465 6e74 2025   block content %
-00000120: 7d0a 3c64 6976 2063 6c61 7373 3d22 636f  }.<div class="co
-00000130: 6e74 6169 6e65 7222 3e0a 2020 7b25 2069  ntainer">.  {% i
-00000140: 6e63 6c75 6465 2022 6d65 7373 6167 655f  nclude "message_
-00000150: 736e 6970 7065 742e 6874 6d6c 2220 257d  snippet.html" %}
-00000160: 0a20 2020 203c 6832 2063 6c61 7373 3d22  .    <h2 class="
-00000170: 6d62 2d34 223e 5265 7365 6172 6368 2045  mb-4">Research E
-00000180: 6e76 6972 6f6e 6d65 6e74 733c 2f68 323e  nvironments</h2>
-00000190: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
-000001a0: 2263 6172 6422 2073 7479 6c65 3d22 7769  "card" style="wi
-000001b0: 6474 683a 2033 3672 656d 3b22 3e0a 2020  dth: 36rem;">.  
-000001c0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000001d0: 6361 7264 2d62 6f64 7922 3e0a 2020 2020  card-body">.    
-000001e0: 2020 2020 3c70 2063 6c61 7373 3d22 6361      <p class="ca
-000001f0: 7264 2d74 6578 7420 666f 6e74 2d77 6569  rd-text font-wei
-00000200: 6768 742d 626f 6c64 223e 596f 7520 646f  ght-bold">You do
-00000210: 6e27 7420 6861 7665 2061 6e79 2072 6573  n't have any res
-00000220: 6561 7263 6820 656e 7669 726f 6e6d 656e  earch environmen
-00000230: 7473 2079 6574 2e3c 2f70 3e0a 2020 2020  ts yet.</p>.    
-00000240: 2020 2020 3c70 2063 6c61 7373 3d22 6361      <p class="ca
-00000250: 7264 2d74 6578 7422 3e50 726f 7669 6465  rd-text">Provide
-00000260: 2061 2070 6173 7377 6f72 6420 616e 6420   a password and 
-00000270: 636c 6963 6b20 7468 6520 6275 7474 6f6e  click the button
-00000280: 2062 656c 6f77 2074 6f20 6372 6561 7465   below to create
-00000290: 2079 6f75 7220 476f 6f67 6c65 2043 6c6f   your Google Clo
-000002a0: 7564 2049 6465 6e74 6974 792e 3c2f 703e  ud Identity.</p>
-000002b0: 0a20 2020 2020 2020 203c 666f 726d 2069  .        <form i
-000002c0: 643d 2265 6e76 6972 6f6e 6d65 6e74 5f69  d="environment_i
-000002d0: 6465 6e74 6974 795f 7072 6f76 6973 696f  dentity_provisio
-000002e0: 6e69 6e67 5f66 6f72 6d22 2061 6374 696f  ning_form" actio
-000002f0: 6e3d 227b 2520 7572 6c20 2769 6465 6e74  n="{% url 'ident
-00000300: 6974 795f 7072 6f76 6973 696f 6e69 6e67  ity_provisioning
-00000310: 2720 257d 2220 6d65 7468 6f64 3d22 706f  ' %}" method="po
-00000320: 7374 223e 0a20 2020 2020 2020 2020 207b  st">.          {
-00000330: 2520 6373 7266 5f74 6f6b 656e 2025 7d0a  % csrf_token %}.
-00000340: 2020 2020 2020 2020 2020 7b7b 2066 6f72            {{ for
-00000350: 6d20 7d7d 0a20 2020 2020 2020 2020 203c  m }}.          <
-00000360: 6275 7474 6f6e 2063 6c61 7373 3d22 6274  button class="bt
-00000370: 6e20 6274 6e2d 7072 696d 6172 7920 6d74  n btn-primary mt
-00000380: 2d33 2220 7479 7065 3d22 7375 626d 6974  -3" type="submit
-00000390: 223e 0a20 2020 2020 2020 2020 2020 2043  ">.            C
-000003a0: 7265 6174 6520 436c 6f75 6420 4964 656e  reate Cloud Iden
-000003b0: 7469 7479 0a20 2020 2020 2020 2020 203c  tity.          <
-000003c0: 2f62 7574 746f 6e3e 0a20 2020 2020 2020  /button>.       
-000003d0: 203c 2f66 6f72 6d3e 0a20 2020 2020 203c   </form>.      <
-000003e0: 2f64 6976 3e0a 2020 2020 3c2f 6469 763e  /div>.    </div>
-000003f0: 0a3c 2f64 6976 3e0a 7b25 2065 6e64 626c  .</div>.{% endbl
-00000400: 6f63 6b20 257d 0a0a 7b25 2062 6c6f 636b  ock %}..{% block
-00000410: 206c 6f63 616c 5f6a 735f 626f 7474 6f6d   local_js_bottom
-00000420: 2025 7d0a 3c73 6372 6970 743e 0a20 2028   %}.<script>.  (
-00000430: 6675 6e63 7469 6f6e 2829 207b 0a20 2020  function() {.   
-00000440: 2063 6f6e 7374 2066 6f72 6d20 3d20 646f   const form = do
-00000450: 6375 6d65 6e74 2e67 6574 456c 656d 656e  cument.getElemen
-00000460: 7442 7949 6428 2265 6e76 6972 6f6e 6d65  tById("environme
-00000470: 6e74 5f69 6465 6e74 6974 795f 7072 6f76  nt_identity_prov
-00000480: 6973 696f 6e69 6e67 5f66 6f72 6d22 293b  isioning_form");
-00000490: 0a20 2020 206c 6574 2061 6c6c 6f77 5375  .    let allowSu
-000004a0: 626d 6974 203d 2074 7275 653b 0a0a 2020  bmit = true;..  
-000004b0: 2020 666f 726d 2e6f 6e73 7562 6d69 7420    form.onsubmit 
-000004c0: 3d20 6675 6e63 7469 6f6e 2829 207b 0a20  = function() {. 
-000004d0: 2020 2020 2069 6620 2861 6c6c 6f77 5375       if (allowSu
-000004e0: 626d 6974 2920 7b0a 2020 2020 2020 2020  bmit) {.        
-000004f0: 666f 726d 2e71 7565 7279 5365 6c65 6374  form.querySelect
-00000500: 6f72 2822 6275 7474 6f6e 2229 2e63 6c61  or("button").cla
-00000510: 7373 4c69 7374 2e61 6464 2822 6469 7361  ssList.add("disa
-00000520: 626c 6564 2229 3b0a 2020 2020 2020 2020  bled");.        
-00000530: 616c 6c6f 7753 7562 6d69 7420 3d20 6661  allowSubmit = fa
-00000540: 6c73 653b 0a20 2020 2020 2020 2072 6574  lse;.        ret
-00000550: 7572 6e20 7472 7565 3b0a 2020 2020 2020  urn true;.      
-00000560: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
-00000570: 2072 6574 7572 6e20 6661 6c73 653b 0a20   return false;. 
-00000580: 2020 2020 207d 0a20 2020 207d 3b0a 2020       }.    };.  
-00000590: 7d29 2829 3b0a 3c2f 7363 7269 7074 3e0a  })();.</script>.
-000005a0: 7b25 2065 6e64 626c 6f63 6b20 257d 0a    {% endblock %}.
+00000110: 2062 6c6f 636b 206c 6f63 616c 5f6a 735f   block local_js_
+00000120: 746f 7020 257d 0a3c 7363 7269 7074 2073  top %}.<script s
+00000130: 7263 3d22 7b25 2073 7461 7469 6320 2765  rc="{% static 'e
+00000140: 6e76 6972 6f6e 6d65 6e74 2f6a 732f 666f  nvironment/js/fo
+00000150: 726d 732e 6a73 2720 257d 223e 3c2f 7363  rms.js' %}"></sc
+00000160: 7269 7074 3e0a 7b25 2065 6e64 626c 6f63  ript>.{% endbloc
+00000170: 6b20 257d 0a0a 7b25 2062 6c6f 636b 2063  k %}..{% block c
+00000180: 6f6e 7465 6e74 2025 7d0a 3c64 6976 2063  ontent %}.<div c
+00000190: 6c61 7373 3d22 636f 6e74 6169 6e65 7222  lass="container"
+000001a0: 3e0a 2020 7b25 2069 6e63 6c75 6465 2022  >.  {% include "
+000001b0: 6d65 7373 6167 655f 736e 6970 7065 742e  message_snippet.
+000001c0: 6874 6d6c 2220 257d 0a20 2020 203c 6832  html" %}.    <h2
+000001d0: 2063 6c61 7373 3d22 6d62 2d34 223e 5265   class="mb-4">Re
+000001e0: 7365 6172 6368 2045 6e76 6972 6f6e 6d65  search Environme
+000001f0: 6e74 733c 2f68 323e 0a20 2020 203c 6469  nts</h2>.    <di
+00000200: 7620 636c 6173 733d 2263 6172 6422 2073  v class="card" s
+00000210: 7479 6c65 3d22 7769 6474 683a 2033 3672  tyle="width: 36r
+00000220: 656d 3b22 3e0a 2020 2020 2020 3c64 6976  em;">.      <div
+00000230: 2063 6c61 7373 3d22 6361 7264 2d62 6f64   class="card-bod
+00000240: 7922 3e0a 2020 2020 2020 2020 3c70 2063  y">.        <p c
+00000250: 6c61 7373 3d22 6361 7264 2d74 6578 7420  lass="card-text 
+00000260: 666f 6e74 2d77 6569 6768 742d 626f 6c64  font-weight-bold
+00000270: 223e 596f 7520 646f 6e27 7420 6861 7665  ">You don't have
+00000280: 2061 6e79 2072 6573 6561 7263 6820 656e   any research en
+00000290: 7669 726f 6e6d 656e 7473 2079 6574 2e3c  vironments yet.<
+000002a0: 2f70 3e0a 2020 2020 2020 2020 3c70 2063  /p>.        <p c
+000002b0: 6c61 7373 3d22 6361 7264 2d74 6578 7422  lass="card-text"
+000002c0: 3e50 726f 7669 6465 2061 2070 6173 7377  >Provide a passw
+000002d0: 6f72 6420 616e 6420 636c 6963 6b20 7468  ord and click th
+000002e0: 6520 6275 7474 6f6e 2062 656c 6f77 2074  e button below t
+000002f0: 6f20 6372 6561 7465 2079 6f75 7220 476f  o create your Go
+00000300: 6f67 6c65 2043 6c6f 7564 2049 6465 6e74  ogle Cloud Ident
+00000310: 6974 792e 3c2f 703e 0a20 2020 2020 2020  ity.</p>.       
+00000320: 203c 666f 726d 2069 643d 2265 6e76 6972   <form id="envir
+00000330: 6f6e 6d65 6e74 5f69 6465 6e74 6974 795f  onment_identity_
+00000340: 7072 6f76 6973 696f 6e69 6e67 5f66 6f72  provisioning_for
+00000350: 6d22 2063 6c61 7373 3d22 7369 6e67 6c65  m" class="single
+00000360: 2d73 7562 6d69 742d 666f 726d 2220 6163  -submit-form" ac
+00000370: 7469 6f6e 3d22 7b25 2075 726c 2027 6964  tion="{% url 'id
+00000380: 656e 7469 7479 5f70 726f 7669 7369 6f6e  entity_provision
+00000390: 696e 6727 2025 7d22 206d 6574 686f 643d  ing' %}" method=
+000003a0: 2270 6f73 7422 3e0a 2020 2020 2020 2020  "post">.        
+000003b0: 2020 7b25 2063 7372 665f 746f 6b65 6e20    {% csrf_token 
+000003c0: 257d 0a20 2020 2020 2020 2020 207b 7b20  %}.          {{ 
+000003d0: 666f 726d 207d 7d0a 2020 2020 2020 2020  form }}.        
+000003e0: 2020 3c62 7574 746f 6e20 636c 6173 733d    <button class=
+000003f0: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
+00000400: 206d 742d 3322 2074 7970 653d 2273 7562   mt-3" type="sub
+00000410: 6d69 7422 3e0a 2020 2020 2020 2020 2020  mit">.          
+00000420: 2020 4372 6561 7465 2043 6c6f 7564 2049    Create Cloud I
+00000430: 6465 6e74 6974 790a 2020 2020 2020 2020  dentity.        
+00000440: 2020 3c2f 6275 7474 6f6e 3e0a 2020 2020    </button>.    
+00000450: 2020 2020 3c2f 666f 726d 3e0a 2020 2020      </form>.    
+00000460: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
+00000470: 6976 3e0a 3c2f 6469 763e 0a7b 2520 656e  iv>.</div>.{% en
+00000480: 6462 6c6f 636b 2025 7d0a 0a              dblock %}..
```

### Comparing `hdn-research-environment-2.1.7/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.1.8/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-2.1.8/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.1.8/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.1.8/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tests/helpers.py` & `hdn-research-environment-2.1.8/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tests/mocks.py` & `hdn-research-environment-2.1.8/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tests/test_decorators.py` & `hdn-research-environment-2.1.8/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tests/test_services.py` & `hdn-research-environment-2.1.8/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tests/test_signals.py` & `hdn-research-environment-2.1.8/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tests/test_utilities.py` & `hdn-research-environment-2.1.8/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tests/test_validators.py` & `hdn-research-environment-2.1.8/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/tests/test_views.py` & `hdn-research-environment-2.1.8/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/urls.py` & `hdn-research-environment-2.1.8/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/utilities.py` & `hdn-research-environment-2.1.8/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.7/environment/views.py` & `hdn-research-environment-2.1.8/environment/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,21 @@
     with concurrent.futures.ThreadPoolExecutor() as executor:
         workspaces_list_future = executor.submit(
             services.get_workspaces_list, request.user
         )
         billing_accounts_list_future = executor.submit(
             services.get_billing_accounts_list, request.user
         )
+        workspace_creation_workflows_future = executor.submit(
+            services.get_workspace_creation_workflows, request.user
+        )
 
     workspaces_list = workspaces_list_future.result()
     billing_accounts_list = billing_accounts_list_future.result()
+    workspace_creation_workflows = workspace_creation_workflows_future.result()
 
     environment_project_workflow_triplets = services.get_environments_with_projects(user=request.user)
 
     environments = map(lambda pair: pair[0], environment_project_workflow_triplets)
     available_project_environment_workflow_triplets = (
         services.get_available_projects_with_environments(
             request.user,
@@ -148,31 +152,35 @@
             environment_projects_pairs_with_creating,
             workspaces_list,
             billing_accounts_list,
         )
     )
 
     context = {
-        "environment_project_workflow_triplets": environment_project_workflow_triplets,
+        "available_project_environment_workflow_triplets": available_project_environment_workflow_triplets,
+        "environment_project_workflow_triplets": environment_projects_pairs_with_creating,
         "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_dict,
+        "workspace_creation_workflows": workspace_creation_workflows,
+        "billing_accounts_list": billing_accounts_list,
     }
 
     execution_resource_name = request.GET.get("execution_resource_name")
     if execution_resource_name:
         workflow = Workflow.objects.get(execution_resource_name=execution_resource_name)
         workflow_state_context = {
             "recent_workflow": workflow,
             "recent_workflow_failed": workflow.status == Workflow.FAILED,
             "recent_workflow_succeeded": workflow.status == Workflow.SUCCESS,
+            "workflow_finished_message": services.workflow_finished_message(workflow=workflow)
         }
         context = {**context, **workflow_state_context}
 
     return render(
         request,
-        "environment/_available_environments_list.html",
+        "environment/_environment_tabs.html",
         context,
     )
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 @cloud_identity_required
```

### Comparing `hdn-research-environment-2.1.7/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.1.8/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.7
+Version: 2.1.8
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.7/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.1.8/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 environment/static/environment/js/cookie.js
 environment/static/environment/js/forms.js
 environment/static/environment/js/gpu_disabling.js
 environment/static/environment/js/pricing_change.js
 environment/templates/environment/_available_environments_list.html
 environment/templates/environment/_available_projects_list.html
 environment/templates/environment/_billing_accounts_list.html
+environment/templates/environment/_environment_tabs.html
 environment/templates/environment/base_environment_home.html
 environment/templates/environment/create_research_environment.html
 environment/templates/environment/create_workspace.html
 environment/templates/environment/identity_provisioning.html
 environment/templates/environment/manage_billing_account.html
 environment/templates/environment/manage_shared_billing_invitation.html
 environment/templates/environment/research_environments.html
```

### Comparing `hdn-research-environment-2.1.7/setup.cfg` & `hdn-research-environment-2.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.1.7
+version = 2.1.8
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

