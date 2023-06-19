# Comparing `tmp/django_rq_scheduler-2023.6.1.tar.gz` & `tmp/django_rq_scheduler-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rq_scheduler-2023.6.1.tar", max compression
+gzip compressed data, was "django_rq_scheduler-2023.6.2.tar", max compression
```

## Comparing `django_rq_scheduler-2023.6.1.tar` & `django_rq_scheduler-2023.6.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1107 2023-06-03 14:51:51.030081 django_rq_scheduler-2023.6.1/LICENSE
--rw-r--r--   0        0        0     1366 2023-06-03 14:51:51.030081 django_rq_scheduler-2023.6.1/README.md
--rw-r--r--   0        0        0     1860 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/__init__.py
--rw-r--r--   0        0        0      104 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/admin/__init__.py
--rw-r--r--   0        0        0     5613 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/admin/job.py
--rw-r--r--   0        0        0     1468 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/admin/redis_models.py
--rw-r--r--   0        0        0      281 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/apps.py
--rw-r--r--   0        0        0     1214 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/decorators.py
--rw-r--r--   0        0        0        0 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/__init__.py
--rw-r--r--   0        0        0     1303 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/delete_failed_executions.py
--rw-r--r--   0        0        0     1907 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/export.py
--rw-r--r--   0        0        0     3835 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/import.py
--rw-r--r--   0        0        0     3438 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/rqstats.py
--rw-r--r--   0        0        0     3176 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/rqworker.py
--rw-r--r--   0        0        0     1374 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/run_job.py
--rw-r--r--   0        0        0     6402 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
--rw-r--r--   0        0        0      898 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
--rw-r--r--   0        0        0     4196 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0003_auto_20220329_2107.py
--rw-r--r--   0        0        0      791 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      896 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      728 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0006_auto_20230118_1640.py
--rw-r--r--   0        0        0     1302 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0007_add_result_ttl.py
--rw-r--r--   0        0        0     1982 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
--rw-r--r--   0        0        0     1362 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
--rw-r--r--   0        0        0      661 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0010_queue.py
--rw-r--r--   0        0        0     7643 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
--rw-r--r--   0        0        0      934 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
--rw-r--r--   0        0        0     1320 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py
--rw-r--r--   0        0        0        0 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/__init__.py
--rw-r--r--   0        0        0      187 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/models/__init__.py
--rw-r--r--   0        0        0     3113 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/models/args.py
--rw-r--r--   0        0        0      364 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/models/queue.py
--rw-r--r--   0        0        0    14803 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/models/scheduled_job.py
--rw-r--r--   0        0        0      366 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/models/worker.py
--rw-r--r--   0        0        0        0 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/py.typed
--rw-r--r--   0        0        0     5056 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/queues.py
--rw-r--r--   0        0        0     9124 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/rq_classes.py
--rw-r--r--   0        0        0     1073 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/settings.py
--rw-r--r--   0        0        0      163 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/change_form.html
--rw-r--r--   0        0        0      127 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/change_list.html
--rw-r--r--   0        0        0     1595 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/confirm_action.html
--rw-r--r--   0        0        0     7823 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/job_detail.html
--rw-r--r--   0        0        0     2697 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/jobs-list.partial.html
--rw-r--r--   0        0        0     6360 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/jobs.html
--rw-r--r--   0        0        0      915 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/queue_workers.html
--rw-r--r--   0        0        0      568 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/scheduler_base.html
--rw-r--r--   0        0        0     1324 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/single_job_action.html
--rw-r--r--   0        0        0     4224 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/stats.html
--rw-r--r--   0        0        0     3032 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/worker_details.html
--rw-r--r--   0        0        0     1879 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/workers-list.partial.html
--rw-r--r--   0        0        0      935 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/workers.html
--rw-r--r--   0        0        0        0 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templatetags/__init__.py
--rw-r--r--   0        0        0     1652 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templatetags/scheduler_tags.py
--rw-r--r--   0        0        0        0 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/__init__.py
--rw-r--r--   0        0        0      502 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/jobs.py
--rw-r--r--   0        0        0      668 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_internals.py
--rw-r--r--   0        0        0     5887 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_job_arg_models.py
--rw-r--r--   0        0        0     2349 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_job_decorator.py
--rw-r--r--   0        0        0    10967 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_mgmt_cmds.py
--rw-r--r--   0        0        0    27724 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_models.py
--rw-r--r--   0        0        0      807 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_redis_models.py
--rw-r--r--   0        0        0     2317 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_settings.py
--rw-r--r--   0        0        0    20065 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_views.py
--rw-r--r--   0        0        0     1577 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_worker.py
--rw-r--r--   0        0        0     3399 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/testtools.py
--rw-r--r--   0        0        0     2742 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tools.py
--rw-r--r--   0        0        0     1121 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/urls.py
--rw-r--r--   0        0        0    16239 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/views.py
--rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1107 2023-06-19 16:30:23.124128 django_rq_scheduler-2023.6.2/LICENSE
+-rw-r--r--   0        0        0     1366 2023-06-19 16:30:23.124128 django_rq_scheduler-2023.6.2/README.md
+-rw-r--r--   0        0        0     1860 2023-06-19 16:30:23.128128 django_rq_scheduler-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-19 16:30:23.128128 django_rq_scheduler-2023.6.2/scheduler/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-19 16:30:23.128128 django_rq_scheduler-2023.6.2/scheduler/admin/__init__.py
+-rw-r--r--   0        0        0     5613 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/admin/job.py
+-rw-r--r--   0        0        0     1468 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/admin/redis_models.py
+-rw-r--r--   0        0        0      281 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/apps.py
+-rw-r--r--   0        0        0     1214 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/decorators.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/management/commands/__init__.py
+-rw-r--r--   0        0        0     1303 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/management/commands/delete_failed_executions.py
+-rw-r--r--   0        0        0     1907 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/management/commands/export.py
+-rw-r--r--   0        0        0     3835 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/management/commands/import.py
+-rw-r--r--   0        0        0     3438 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/management/commands/rqstats.py
+-rw-r--r--   0        0        0     3176 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/management/commands/rqworker.py
+-rw-r--r--   0        0        0     1374 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/management/commands/run_job.py
+-rw-r--r--   0        0        0     6402 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
+-rw-r--r--   0        0        0      898 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
+-rw-r--r--   0        0        0     4196 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0003_auto_20220329_2107.py
+-rw-r--r--   0        0        0      791 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      896 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      728 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0006_auto_20230118_1640.py
+-rw-r--r--   0        0        0     1302 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0007_add_result_ttl.py
+-rw-r--r--   0        0        0     1982 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
+-rw-r--r--   0        0        0     1362 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
+-rw-r--r--   0        0        0      661 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0010_queue.py
+-rw-r--r--   0        0        0     7643 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
+-rw-r--r--   0        0        0      934 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
+-rw-r--r--   0        0        0     1320 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/migrations/__init__.py
+-rw-r--r--   0        0        0      187 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3113 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/models/args.py
+-rw-r--r--   0        0        0      364 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/models/queue.py
+-rw-r--r--   0        0        0    14803 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/models/scheduled_job.py
+-rw-r--r--   0        0        0      366 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/models/worker.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/py.typed
+-rw-r--r--   0        0        0     5056 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/queues.py
+-rw-r--r--   0        0        0     9124 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/rq_classes.py
+-rw-r--r--   0        0        0     1073 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/settings.py
+-rw-r--r--   0        0        0      163 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/change_form.html
+-rw-r--r--   0        0        0      127 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/change_list.html
+-rw-r--r--   0        0        0     1595 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/confirm_action.html
+-rw-r--r--   0        0        0     7823 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/job_detail.html
+-rw-r--r--   0        0        0     2697 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/jobs-list.partial.html
+-rw-r--r--   0        0        0     6360 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/jobs.html
+-rw-r--r--   0        0        0      915 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/queue_workers.html
+-rw-r--r--   0        0        0      568 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/scheduler_base.html
+-rw-r--r--   0        0        0     1324 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/single_job_action.html
+-rw-r--r--   0        0        0     4224 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/stats.html
+-rw-r--r--   0        0        0     3032 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/worker_details.html
+-rw-r--r--   0        0        0     1879 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/workers-list.partial.html
+-rw-r--r--   0        0        0      935 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/workers.html
+-rw-r--r--   0        0        0        0 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templatetags/__init__.py
+-rw-r--r--   0        0        0     1652 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/templatetags/scheduler_tags.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/jobs.py
+-rw-r--r--   0        0        0      668 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_internals.py
+-rw-r--r--   0        0        0     5887 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_job_arg_models.py
+-rw-r--r--   0        0        0     2349 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_job_decorator.py
+-rw-r--r--   0        0        0    10967 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_mgmt_cmds.py
+-rw-r--r--   0        0        0    27724 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_models.py
+-rw-r--r--   0        0        0      807 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_redis_models.py
+-rw-r--r--   0        0        0     2317 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_settings.py
+-rw-r--r--   0        0        0    20065 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_views.py
+-rw-r--r--   0        0        0     1577 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/test_worker.py
+-rw-r--r--   0        0        0     3399 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tests/testtools.py
+-rw-r--r--   0        0        0     2742 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/tools.py
+-rw-r--r--   0        0        0     1121 2023-06-19 16:30:23.132128 django_rq_scheduler-2023.6.2/scheduler/urls.py
+-rw-r--r--   0        0        0    16239 2023-06-19 16:30:23.136128 django_rq_scheduler-2023.6.2/scheduler/views.py
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.6.2/PKG-INFO
```

### Comparing `django_rq_scheduler-2023.6.1/LICENSE` & `django_rq_scheduler-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/README.md` & `django_rq_scheduler-2023.6.2/README.md`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/pyproject.toml` & `django_rq_scheduler-2023.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-rq-scheduler"
 packages = [
     { include = "scheduler" },
 ]
-version = "2023.6.1"
+version = "2023.6.2"
 description = "An async job scheduler for django using redis"
 readme = "README.md"
 keywords = ["redis", "django", "background-jobs", "job-queue", "task-queue", "redis-queue", "scheduled-jobs"]
 authors = [
     "Daniel Moran <daniel@moransoftware.ca>",
 ]
 maintainers = [
@@ -50,15 +50,15 @@
 click = "^8.1"
 rq = "^1.15"
 pyyaml = { version = "^6.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 poetry = "^1.5"
 coverage = "^7"
-fakeredis = { version = "^2.13", extras = ['lua'] }
+fakeredis = { version = "^2.15", extras = ['lua'] }
 Flake8-pyproject = "^1.2"
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
 
 [tool.flake8]
 max-line-length = 119
```

### Comparing `django_rq_scheduler-2023.6.1/scheduler/admin/job.py` & `django_rq_scheduler-2023.6.2/scheduler/admin/job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/admin/redis_models.py` & `django_rq_scheduler-2023.6.2/scheduler/admin/redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/decorators.py` & `django_rq_scheduler-2023.6.2/scheduler/decorators.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/management/commands/delete_failed_executions.py` & `django_rq_scheduler-2023.6.2/scheduler/management/commands/delete_failed_executions.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/management/commands/export.py` & `django_rq_scheduler-2023.6.2/scheduler/management/commands/export.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/management/commands/import.py` & `django_rq_scheduler-2023.6.2/scheduler/management/commands/import.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/management/commands/rqstats.py` & `django_rq_scheduler-2023.6.2/scheduler/management/commands/rqstats.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/management/commands/rqworker.py` & `django_rq_scheduler-2023.6.2/scheduler/management/commands/rqworker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/management/commands/run_job.py` & `django_rq_scheduler-2023.6.2/scheduler/management/commands/run_job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0003_auto_20220329_2107.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0003_auto_20220329_2107.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0006_auto_20230118_1640.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0006_auto_20230118_1640.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0007_add_result_ttl.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0007_add_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0010_queue.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0010_queue.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py` & `django_rq_scheduler-2023.6.2/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/models/args.py` & `django_rq_scheduler-2023.6.2/scheduler/models/args.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/models/scheduled_job.py` & `django_rq_scheduler-2023.6.2/scheduler/models/scheduled_job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/queues.py` & `django_rq_scheduler-2023.6.2/scheduler/queues.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/rq_classes.py` & `django_rq_scheduler-2023.6.2/scheduler/rq_classes.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/settings.py` & `django_rq_scheduler-2023.6.2/scheduler/settings.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/confirm_action.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/job_detail.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/job_detail.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/jobs-list.partial.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/jobs-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/jobs.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/jobs.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/queue_workers.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/queue_workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/scheduler_base.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/scheduler_base.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/single_job_action.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/single_job_action.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/stats.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/stats.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/worker_details.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/worker_details.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/workers-list.partial.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/workers-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/workers.html` & `django_rq_scheduler-2023.6.2/scheduler/templates/admin/scheduler/workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/templatetags/scheduler_tags.py` & `django_rq_scheduler-2023.6.2/scheduler/templatetags/scheduler_tags.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_internals.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_job_arg_models.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_job_arg_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_job_decorator.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_job_decorator.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_mgmt_cmds.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_mgmt_cmds.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_models.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_redis_models.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_settings.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_views.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/test_worker.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tests/testtools.py` & `django_rq_scheduler-2023.6.2/scheduler/tests/testtools.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/tools.py` & `django_rq_scheduler-2023.6.2/scheduler/tools.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/urls.py` & `django_rq_scheduler-2023.6.2/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/scheduler/views.py` & `django_rq_scheduler-2023.6.2/scheduler/views.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.1/PKG-INFO` & `django_rq_scheduler-2023.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rq-scheduler
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: An async job scheduler for django using redis
 Home-page: https://github.com/dsoftwareinc/django-rq-scheduler
 License: MIT
 Keywords: redis,django,background-jobs,job-queue,task-queue,redis-queue,scheduled-jobs
 Author: Daniel Moran
 Author-email: daniel@moransoftware.ca
 Maintainer: Daniel Moran
```

