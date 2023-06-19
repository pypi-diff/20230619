# Comparing `tmp/deepfos-celery-1.0.2.tar.gz` & `tmp/deepfos-celery-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfos-celery-1.0.2.tar", last modified: Fri Mar 31 10:07:42 2023, max compression
+gzip compressed data, was "deepfos-celery-1.0.3.tar", last modified: Mon Jun 19 06:39:44 2023, max compression
```

## Comparing `deepfos-celery-1.0.2.tar` & `deepfos-celery-1.0.3.tar`

### file list

```diff
@@ -1,425 +1,426 @@
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.692958 deepfos-celery-1.0.2/
--rw-rw-r--   0 wei       (1000) wei       (1000)     7841 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/CONTRIBUTORS.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)     5060 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/Changelog.rst
--rw-rw-r--   0 wei       (1000) wei       (1000)     2631 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/LICENSE
--rw-rw-r--   0 wei       (1000) wei       (1000)      709 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/MANIFEST.in
--rw-rw-r--   0 wei       (1000) wei       (1000)     4154 2023-03-31 10:07:42.692958 deepfos-celery-1.0.2/PKG-INFO
--rw-rw-r--   0 wei       (1000) wei       (1000)     2099 2023-03-24 03:41:36.000000 deepfos-celery-1.0.2/README.rst
--rw-rw-r--   0 wei       (1000) wei       (1000)       84 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/TODO
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.640955 deepfos-celery-1.0.2/celery/
--rw-rw-r--   0 wei       (1000) wei       (1000)     6020 2023-03-31 09:58:37.000000 deepfos-celery-1.0.2/celery/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      401 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/__main__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5049 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/_state.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.644955 deepfos-celery-1.0.2/celery/aio/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2023-01-11 02:40:53.000000 deepfos-celery-1.0.2/celery/aio/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7167 2023-02-22 10:43:53.000000 deepfos-celery-1.0.2/celery/aio/amqp.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    24011 2023-03-20 10:54:12.000000 deepfos-celery-1.0.2/celery/aio/backend.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2919 2023-03-20 08:55:51.000000 deepfos-celery-1.0.2/celery/aio/canvas.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6460 2023-03-20 08:58:55.000000 deepfos-celery-1.0.2/celery/aio/common.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    12260 2023-03-15 09:14:16.000000 deepfos-celery-1.0.2/celery/aio/connection.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8648 2023-03-31 03:56:36.000000 deepfos-celery-1.0.2/celery/aio/control.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5352 2023-02-22 10:43:53.000000 deepfos-celery-1.0.2/celery/aio/dispatcher.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4277 2023-03-16 10:02:14.000000 deepfos-celery-1.0.2/celery/aio/entity.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      140 2023-02-22 09:41:26.000000 deepfos-celery-1.0.2/celery/aio/events.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3353 2023-03-15 06:42:40.000000 deepfos-celery-1.0.2/celery/aio/exchange.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8578 2023-03-31 02:44:01.000000 deepfos-celery-1.0.2/celery/aio/messaging.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7448 2023-02-08 03:43:28.000000 deepfos-celery-1.0.2/celery/aio/pool.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1939 2023-02-17 08:34:40.000000 deepfos-celery-1.0.2/celery/aio/pools.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    32065 2023-03-17 02:09:55.000000 deepfos-celery-1.0.2/celery/aio/redis.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    12906 2023-03-21 06:12:52.000000 deepfos-celery-1.0.2/celery/aio/result.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2946 2023-02-17 03:23:43.000000 deepfos-celery-1.0.2/celery/aio/task.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1606 2023-02-08 07:56:00.000000 deepfos-celery-1.0.2/celery/aio/transport.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6414 2023-03-31 05:30:15.000000 deepfos-celery-1.0.2/celery/aio/utils.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.644955 deepfos-celery-1.0.2/celery/app/
--rw-rw-r--   0 wei       (1000) wei       (1000)     2459 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    23402 2023-02-08 02:56:41.000000 deepfos-celery-1.0.2/celery/app/amqp.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1445 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/app/annotations.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2288 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/autoretry.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2765 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/backends.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    56783 2023-03-31 02:49:38.000000 deepfos-celery-1.0.2/celery/app/base.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6673 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/app/builtins.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    16748 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/control.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    14257 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/defaults.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1326 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/app/events.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9169 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/log.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2002 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/registry.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4685 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/routes.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    39948 2023-02-07 10:03:29.000000 deepfos-celery-1.0.2/celery/app/task.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    25909 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/trace.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    13160 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/app/utils.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.644955 deepfos-celery-1.0.2/celery/apps/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/apps/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5161 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/apps/beat.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    16418 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/apps/multi.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    13474 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/apps/worker.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.648955 deepfos-celery-1.0.2/celery/backends/
--rw-rw-r--   0 wei       (1000) wei       (1000)       23 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/backends/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7651 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/arangodb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9464 2023-03-20 08:35:23.000000 deepfos-celery-1.0.2/celery/backends/asynchronous.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4470 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/azureblockblob.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    37380 2023-02-16 03:06:09.000000 deepfos-celery-1.0.2/celery/backends/base.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4818 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/cache.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7899 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/cassandra.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3113 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/consul.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6847 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/cosmosdbsql.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3173 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/couchbase.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2919 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/couchdb.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.648955 deepfos-celery-1.0.2/celery/backends/database/
--rw-rw-r--   0 wei       (1000) wei       (1000)     7771 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/backends/database/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3351 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/backends/database/models.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2866 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/database/session.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    17262 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/dynamodb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8469 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/elasticsearch.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2925 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/filesystem.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    11189 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/backends/mongodb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    22564 2023-02-21 08:28:09.000000 deepfos-celery-1.0.2/celery/backends/redis.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    12077 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/backends/rpc.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2752 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/backends/s3.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    24135 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/beat.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.652955 deepfos-celery-1.0.2/celery/bin/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/bin/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9960 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/bin/amqp.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7715 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/base.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2583 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/beat.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2338 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/call.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6684 2022-10-13 09:04:11.000000 deepfos-celery-1.0.2/celery/bin/celery.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6679 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/bin/control.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2835 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/events.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5791 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/bin/graph.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1035 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/bin/list.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4244 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/bin/logtool.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2139 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/migrate.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    15363 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/multi.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2578 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/purge.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1007 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/result.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4809 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/bin/shell.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3072 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/bin/upgrade.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    11751 2022-10-13 09:23:40.000000 deepfos-celery-1.0.2/celery/bin/worker.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    12297 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/bootsteps.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    58315 2023-03-20 08:36:56.000000 deepfos-celery-1.0.2/celery/canvas.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.652955 deepfos-celery-1.0.2/celery/concurrency/
--rw-rw-r--   0 wei       (1000) wei       (1000)      852 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/concurrency/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    50516 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/concurrency/asynpool.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4373 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/concurrency/base.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4156 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/concurrency/eventlet.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3415 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/concurrency/gevent.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5680 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/concurrency/prefork.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      693 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/concurrency/solo.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1248 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/concurrency/thread.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.652955 deepfos-celery-1.0.2/celery/contrib/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/contrib/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5091 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/contrib/abortable.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    14163 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/contrib/migrate.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6507 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/contrib/pytest.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5021 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/contrib/rdb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3410 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/contrib/sphinx.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.652955 deepfos-celery-1.0.2/celery/contrib/testing/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/contrib/testing/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3017 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/contrib/testing/app.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7646 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/contrib/testing/manager.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3394 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/contrib/testing/mocks.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      208 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/contrib/testing/tasks.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5040 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/contrib/testing/worker.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.656956 deepfos-celery-1.0.2/celery/events/
--rw-rw-r--   0 wei       (1000) wei       (1000)      477 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/events/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    18050 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/events/cursesmon.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8987 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/events/dispatcher.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3116 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/events/dumper.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1736 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/events/event.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4998 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/events/receiver.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3274 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/events/snapshot.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    25773 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/events/state.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8601 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/celery/exceptions.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.656956 deepfos-celery-1.0.2/celery/fixups/
--rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/fixups/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6596 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/fixups/django.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.656956 deepfos-celery-1.0.2/celery/loaders/
--rw-rw-r--   0 wei       (1000) wei       (1000)      490 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/loaders/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      199 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/loaders/app.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8731 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/loaders/base.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1520 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/loaders/default.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    17016 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/local.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    24279 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/platforms.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    34176 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/result.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    29259 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/schedules.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.656956 deepfos-celery-1.0.2/celery/security/
--rw-rw-r--   0 wei       (1000) wei       (1000)     2278 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/security/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2993 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/security/certificate.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1042 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/security/key.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4206 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/security/serialization.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      845 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/security/utils.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4273 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/signals.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3260 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/states.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.660956 deepfos-celery-1.0.2/celery/utils/
--rw-rw-r--   0 wei       (1000) wei       (1000)      935 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2874 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/abstract.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    25648 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/collections.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4717 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/debug.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3620 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/deprecated.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.660956 deepfos-celery-1.0.2/celery/utils/dispatch/
--rw-rw-r--   0 wei       (1000) wei       (1000)       74 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/dispatch/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    17231 2023-02-22 06:13:24.000000 deepfos-celery-1.0.2/celery/utils/dispatch/signal.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10550 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/functional.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9041 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/graph.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4826 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/imports.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2776 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/iso8601.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8626 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/log.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2858 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/nodenames.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5940 2023-01-11 03:00:52.000000 deepfos-celery-1.0.2/celery/utils/objects.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9084 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/saferepr.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8069 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/serialization.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.660956 deepfos-celery-1.0.2/celery/utils/static/
--rw-rw-r--   0 wei       (1000) wei       (1000)      299 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/static/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2556 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/static/celery_128.png
--rw-rw-r--   0 wei       (1000) wei       (1000)     1093 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/sysinfo.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4568 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/utils/term.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5779 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/text.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9626 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/threads.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    12375 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/time.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4533 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/utils/timer2.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.664956 deepfos-celery-1.0.2/celery/worker/
--rw-rw-r--   0 wei       (1000) wei       (1000)       95 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4593 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/autoscale.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7517 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/components.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.664956 deepfos-celery-1.0.2/celery/worker/consumer/
--rw-rw-r--   0 wei       (1000) wei       (1000)      391 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/consumer/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      525 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/consumer/agent.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1026 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/consumer/connection.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    21497 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/worker/consumer/consumer.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      946 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/consumer/control.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2054 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/consumer/events.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6833 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/consumer/gossip.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      930 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/consumer/heart.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2519 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/consumer/mingle.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1959 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/worker/consumer/tasks.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    16771 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/worker/control.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2107 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/heartbeat.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3857 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/worker/loops.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3630 2022-09-23 05:23:46.000000 deepfos-celery-1.0.2/celery/worker/pidbox.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    22670 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/worker/request.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7639 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/worker/state.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6893 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/celery/worker/strategy.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    14521 2022-10-13 11:56:05.000000 deepfos-celery-1.0.2/celery/worker/worker.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.668957 deepfos-celery-1.0.2/deepfos_celery.egg-info/
--rw-rw-r--   0 wei       (1000) wei       (1000)     4154 2023-03-31 10:07:42.000000 deepfos-celery-1.0.2/deepfos_celery.egg-info/PKG-INFO
--rw-rw-r--   0 wei       (1000) wei       (1000)    10231 2023-03-31 10:07:42.000000 deepfos-celery-1.0.2/deepfos_celery.egg-info/SOURCES.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        1 2023-03-31 10:07:42.000000 deepfos-celery-1.0.2/deepfos_celery.egg-info/dependency_links.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       48 2023-03-31 10:07:42.000000 deepfos-celery-1.0.2/deepfos_celery.egg-info/entry_points.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        1 2023-03-24 03:47:52.000000 deepfos-celery-1.0.2/deepfos_celery.egg-info/not-zip-safe
--rw-rw-r--   0 wei       (1000) wei       (1000)     1302 2023-03-31 10:07:42.000000 deepfos-celery-1.0.2/deepfos_celery.egg-info/requires.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        7 2023-03-31 10:07:42.000000 deepfos-celery-1.0.2/deepfos_celery.egg-info/top_level.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        1 2023-02-17 09:55:35.000000 deepfos-celery-1.0.2/pyproject.toml
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.668957 deepfos-celery-1.0.2/requirements/
--rw-rw-r--   0 wei       (1000) wei       (1000)     1454 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/README.rst
--rw-rw-r--   0 wei       (1000) wei       (1000)      145 2023-03-28 04:07:03.000000 deepfos-celery-1.0.2/requirements/default.txt
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.668957 deepfos-celery-1.0.2/requirements/deps/
--rw-rw-r--   0 wei       (1000) wei       (1000)       10 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/deps/mock.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      145 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/dev.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      150 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/docs.txt
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.672957 deepfos-celery-1.0.2/requirements/extras/
--rw-rw-r--   0 wei       (1000) wei       (1000)       15 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/arangodb.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/auth.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       70 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/azureblockblob.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      111 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/brotli.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       24 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/cassandra.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/consul.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       20 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/cosmosdbsql.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       17 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/couchbase.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       10 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/couchdb.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/django.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       15 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/dynamodb.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/elasticsearch.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       17 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/eventlet.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/gevent.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       19 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/librabbitmq.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       36 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/lzma.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       38 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/memcache.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       20 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/mongodb.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        8 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/msgpack.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       17 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/pymemcache.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        6 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/pyro.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/pytest.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/redis.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       15 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/s3.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       27 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/slmq.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        6 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/solar.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       11 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/sqlalchemy.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       82 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/sqs.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       73 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/tblib.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       39 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/thread.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/yaml.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/zeromq.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/extras/zookeeper.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       10 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/extras/zstd.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      266 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/pkgutils.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       19 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/security.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      148 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/test-ci-base.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      550 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/test-ci-default.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      128 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/requirements/test-integration.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       17 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/requirements/test-pypy3.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      170 2023-01-11 03:07:23.000000 deepfos-celery-1.0.2/requirements/test.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      932 2023-03-31 10:07:42.692958 deepfos-celery-1.0.2/setup.cfg
--rw-rw-r--   0 wei       (1000) wei       (1000)     5003 2023-03-24 03:49:30.000000 deepfos-celery-1.0.2/setup.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.672957 deepfos-celery-1.0.2/t/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1855 2023-03-14 11:11:18.000000 deepfos-celery-1.0.2/t/base.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.672957 deepfos-celery-1.0.2/t/benchmarks/
--rw-rw-r--   0 wei       (1000) wei       (1000)     2841 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/benchmarks/bench_worker.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.672957 deepfos-celery-1.0.2/t/distro/
--rw-rw-r--   0 wei       (1000) wei       (1000)      873 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/distro/test_CI_reqs.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.672957 deepfos-celery-1.0.2/t/integration/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/integration/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3596 2023-03-14 10:51:31.000000 deepfos-celery-1.0.2/t/integration/conftest.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4033 2023-03-14 09:53:46.000000 deepfos-celery-1.0.2/t/integration/redissrv.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9524 2023-02-17 09:07:30.000000 deepfos-celery-1.0.2/t/integration/tasks.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3483 2023-03-20 10:35:30.000000 deepfos-celery-1.0.2/t/integration/test_aiocanvas.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10744 2023-03-14 10:47:07.000000 deepfos-celery-1.0.2/t/integration/test_aiotasks.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3681 2023-03-14 11:02:00.000000 deepfos-celery-1.0.2/t/integration/test_auto_recovery.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1120 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/integration/test_backend.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    44519 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/integration/test_canvas.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3459 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/integration/test_security.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9446 2023-02-20 09:32:07.000000 deepfos-celery-1.0.2/t/integration/test_tasks.py
--rw-rw-r--   0 wei       (1000) wei       (1000)       91 2023-03-14 10:22:23.000000 deepfos-celery-1.0.2/t/integration/test_tmp.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2435 2023-02-20 09:08:26.000000 deepfos-celery-1.0.2/t/integration/test_tmp2.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      226 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/skip.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.676957 deepfos-celery-1.0.2/t/unit/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/__init__.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.676957 deepfos-celery-1.0.2/t/unit/aio/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2023-02-16 09:50:39.000000 deepfos-celery-1.0.2/t/unit/aio/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    18500 2023-03-31 03:59:44.000000 deepfos-celery-1.0.2/t/unit/aio/test_aio_control.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.676957 deepfos-celery-1.0.2/t/unit/app/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/app/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    13048 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_amqp.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1331 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/app/test_annotations.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    39009 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/t/unit/app/test_app.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1294 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_backends.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    27400 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_beat.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5475 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_builtins.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      356 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/app/test_celery.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    17367 2023-03-31 03:05:26.000000 deepfos-celery-1.0.2/t/unit/app/test_control.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1627 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_defaults.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      692 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_exceptions.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8637 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_loaders.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10946 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_log.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2342 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/app/test_registry.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7829 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_routes.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    30264 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/app/test_schedules.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1790 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/app/test_utils.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.676957 deepfos-celery-1.0.2/t/unit/apps/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/apps/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    16253 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/apps/test_multi.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.680957 deepfos-celery-1.0.2/t/unit/backends/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/backends/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4266 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_arangodb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6338 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_asynchronous.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3355 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_azureblockblob.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    40815 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_base.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10297 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_cache.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6982 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_cassandra.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      940 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_consul.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4987 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/backends/test_cosmosdbsql.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4847 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_couchbase.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3972 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_couchdb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    14924 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_database.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    19265 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_dynamodb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    32594 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/backends/test_elasticsearch.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3021 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_filesystem.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    25643 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_mongodb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    43068 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/backends/test_redis.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3685 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/backends/test_rpc.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     6654 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/backends/test_s3.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.680957 deepfos-celery-1.0.2/t/unit/bin/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/bin/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)       18 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/bin/celery.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.680957 deepfos-celery-1.0.2/t/unit/bin/proj/
--rw-rw-r--   0 wei       (1000) wei       (1000)       64 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/bin/proj/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)       62 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/bin/proj/app.py
--rw-rw-r--   0 wei       (1000) wei       (1000)       28 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/bin/proj/app2.py
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/bin/test_multi.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.680957 deepfos-celery-1.0.2/t/unit/concurrency/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/concurrency/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     4620 2022-09-23 05:35:24.000000 deepfos-celery-1.0.2/t/unit/concurrency/test_concurrency.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3625 2023-02-17 02:14:28.000000 deepfos-celery-1.0.2/t/unit/concurrency/test_eventlet.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3132 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/concurrency/test_gevent.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1830 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/concurrency/test_pool.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    14713 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/concurrency/test_prefork.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      848 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/concurrency/test_solo.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      728 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/concurrency/test_thread.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10358 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/conftest.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.680957 deepfos-celery-1.0.2/t/unit/contrib/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/__init__.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.684958 deepfos-celery-1.0.2/t/unit/contrib/proj/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/proj/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      183 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/proj/conf.py
--rw-rw-r--   0 wei       (1000) wei       (1000)       93 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/proj/contents.rst
--rw-rw-r--   0 wei       (1000) wei       (1000)      249 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/proj/foo.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      113 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/proj/xyzzy.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1387 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/test_abortable.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10713 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/contrib/test_migrate.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      785 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/test_pytest.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3146 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/contrib/test_rdb.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      767 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/contrib/test_sphinx.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.684958 deepfos-celery-1.0.2/t/unit/events/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/events/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2297 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/events/test_cursesmon.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    11372 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/events/test_events.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3378 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/events/test_snapshot.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    22295 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/events/test_state.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.684958 deepfos-celery-1.0.2/t/unit/fixups/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/fixups/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10834 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/fixups/test_django.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.684958 deepfos-celery-1.0.2/t/unit/security/
--rw-rw-r--   0 wei       (1000) wei       (1000)     3584 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/security/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      102 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/security/case.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3226 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/security/test_certificate.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1069 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/security/test_key.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5492 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/security/test_security.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2218 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/security/test_serialization.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.684958 deepfos-celery-1.0.2/t/unit/tasks/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/tasks/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    43214 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/tasks/test_canvas.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10978 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/tasks/test_chord.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2334 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/tasks/test_context.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    34926 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/tasks/test_result.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1085 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/tasks/test_states.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    50867 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/tasks/test_tasks.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    15374 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/tasks/test_trace.py
--rw-rw-r--   0 wei       (1000) wei       (1000)       78 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/tasks/unit_tasks.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      989 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/test_canvas.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.688958 deepfos-celery-1.0.2/t/unit/utils/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/utils/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    12877 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_collections.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2357 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/utils/test_debug.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1737 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_deprecated.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    11705 2023-02-22 06:16:25.000000 deepfos-celery-1.0.2/t/unit/utils/test_dispatcher.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7456 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_functional.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1935 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/utils/test_graph.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3308 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_imports.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     8161 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_local.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      202 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/utils/test_nodenames.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1293 2023-02-07 10:10:18.000000 deepfos-celery-1.0.2/t/unit/utils/test_objects.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1394 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_pickle.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    26066 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_platforms.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5565 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_saferepr.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     3427 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_serialization.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      751 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/utils/test_sysinfo.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1734 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/utils/test_term.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     1968 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_text.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2453 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_threads.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    11730 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_time.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2744 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/utils/test_timer2.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      624 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/utils/test_utils.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-03-31 10:07:42.692958 deepfos-celery-1.0.2/t/unit/worker/
--rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/worker/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     7221 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/worker/test_autoscale.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9401 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/worker/test_bootsteps.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2454 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/worker/test_components.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    21360 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/worker/test_consumer.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    23385 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/worker/test_control.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     2384 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/worker/test_heartbeat.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    16236 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/worker/test_loops.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    41778 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/worker/test_request.py
--rw-rw-r--   0 wei       (1000) wei       (1000)      238 2022-09-23 05:23:47.000000 deepfos-celery-1.0.2/t/unit/worker/test_revoke.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     5268 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/worker/test_state.py
--rw-rw-r--   0 wei       (1000) wei       (1000)     9760 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/worker/test_strategy.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    39836 2022-09-23 05:35:05.000000 deepfos-celery-1.0.2/t/unit/worker/test_worker.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.138571 deepfos-celery-1.0.3/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7841 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/CONTRIBUTORS.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5060 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/Changelog.rst
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2631 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/LICENSE
+-rw-rw-r--   0 wei       (1000) wei       (1000)      709 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/MANIFEST.in
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4234 2023-06-19 06:39:44.138571 deepfos-celery-1.0.3/PKG-INFO
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2179 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/README.rst
+-rw-rw-r--   0 wei       (1000) wei       (1000)       84 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/TODO
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.082569 deepfos-celery-1.0.3/celery/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6193 2023-06-19 06:33:07.000000 deepfos-celery-1.0.3/celery/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      401 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/__main__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5049 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/_state.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.086569 deepfos-celery-1.0.3/celery/aio/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7340 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/amqp.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    24678 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/backend.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2998 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/canvas.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6656 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/common.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    12587 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/connection.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8876 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/control.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5489 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/dispatcher.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4396 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/entity.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      145 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/events.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3461 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/exchange.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8805 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/messaging.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7448 2023-02-08 03:43:28.000000 deepfos-celery-1.0.3/celery/aio/pool.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2011 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/pools.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    32969 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/redis.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    13291 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/result.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3030 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/task.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1606 2023-02-08 07:56:00.000000 deepfos-celery-1.0.3/celery/aio/transport.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6623 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/aio/utils.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.086569 deepfos-celery-1.0.3/celery/app/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2459 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    23402 2023-02-08 02:56:41.000000 deepfos-celery-1.0.3/celery/app/amqp.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1445 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/app/annotations.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2288 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/autoretry.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2765 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/backends.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    58322 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/app/base.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6673 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/app/builtins.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    16748 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/control.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    14257 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/defaults.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1326 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/app/events.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9169 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/log.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2002 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/registry.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4685 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/routes.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    41027 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/app/task.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    25909 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/trace.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    13160 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/app/utils.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.090569 deepfos-celery-1.0.3/celery/apps/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/apps/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5161 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/apps/beat.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    16418 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/apps/multi.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    13474 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/apps/worker.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.090569 deepfos-celery-1.0.3/celery/backends/
+-rw-rw-r--   0 wei       (1000) wei       (1000)       23 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/backends/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7651 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/arangodb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9464 2023-03-20 08:35:23.000000 deepfos-celery-1.0.3/celery/backends/asynchronous.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4470 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/azureblockblob.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    37380 2023-02-16 03:06:09.000000 deepfos-celery-1.0.3/celery/backends/base.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4818 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/cache.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7899 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/cassandra.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3113 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/consul.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6847 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/cosmosdbsql.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3173 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/couchbase.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2919 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/couchdb.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.094569 deepfos-celery-1.0.3/celery/backends/database/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7771 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/backends/database/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3351 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/backends/database/models.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2866 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/database/session.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    17262 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/dynamodb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8469 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/elasticsearch.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2925 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/filesystem.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    11189 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/backends/mongodb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    23158 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/backends/redis.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    12077 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/backends/rpc.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2752 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/backends/s3.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    24135 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/beat.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.094569 deepfos-celery-1.0.3/celery/bin/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/bin/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9960 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/bin/amqp.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7715 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/base.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2583 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/beat.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2338 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/call.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6684 2022-10-13 09:04:11.000000 deepfos-celery-1.0.3/celery/bin/celery.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6679 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/bin/control.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2835 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/events.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5791 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/bin/graph.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1035 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/bin/list.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4244 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/bin/logtool.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2139 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/migrate.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    15363 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/multi.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2578 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/purge.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1007 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/result.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4809 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/bin/shell.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3072 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/bin/upgrade.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    11751 2022-10-13 09:23:40.000000 deepfos-celery-1.0.3/celery/bin/worker.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    12297 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/bootsteps.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    58315 2023-03-20 08:36:56.000000 deepfos-celery-1.0.3/celery/canvas.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.098569 deepfos-celery-1.0.3/celery/concurrency/
+-rw-rw-r--   0 wei       (1000) wei       (1000)      852 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/concurrency/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    52581 2023-06-19 06:33:07.000000 deepfos-celery-1.0.3/celery/concurrency/asynpool.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4373 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/concurrency/base.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4156 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/concurrency/eventlet.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3415 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/concurrency/gevent.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5947 2023-06-19 06:33:07.000000 deepfos-celery-1.0.3/celery/concurrency/prefork.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      693 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/concurrency/solo.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1248 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/concurrency/thread.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.098569 deepfos-celery-1.0.3/celery/contrib/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/contrib/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5091 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/contrib/abortable.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    14163 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/contrib/migrate.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6507 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/contrib/pytest.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5021 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/contrib/rdb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3410 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/contrib/sphinx.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.098569 deepfos-celery-1.0.3/celery/contrib/testing/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/contrib/testing/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3017 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/contrib/testing/app.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7646 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/contrib/testing/manager.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3394 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/contrib/testing/mocks.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      208 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/contrib/testing/tasks.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5040 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/contrib/testing/worker.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.102570 deepfos-celery-1.0.3/celery/events/
+-rw-rw-r--   0 wei       (1000) wei       (1000)      477 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/events/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    18050 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/events/cursesmon.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8987 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/events/dispatcher.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3116 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/events/dumper.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1736 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/events/event.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4998 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/events/receiver.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3274 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/events/snapshot.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    25773 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/events/state.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8601 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/celery/exceptions.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.102570 deepfos-celery-1.0.3/celery/fixups/
+-rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/fixups/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6596 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/fixups/django.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.102570 deepfos-celery-1.0.3/celery/loaders/
+-rw-rw-r--   0 wei       (1000) wei       (1000)      490 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/loaders/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      199 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/loaders/app.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8731 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/loaders/base.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1520 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/loaders/default.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    17016 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/local.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    24279 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/platforms.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    34176 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/result.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    29259 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/schedules.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.102570 deepfos-celery-1.0.3/celery/security/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2278 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/security/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2993 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/security/certificate.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1042 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/security/key.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4206 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/security/serialization.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      845 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/security/utils.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4273 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/signals.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3260 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/states.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.106570 deepfos-celery-1.0.3/celery/utils/
+-rw-rw-r--   0 wei       (1000) wei       (1000)      935 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2874 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/abstract.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    25648 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/collections.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4717 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/debug.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3620 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/deprecated.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.106570 deepfos-celery-1.0.3/celery/utils/dispatch/
+-rw-rw-r--   0 wei       (1000) wei       (1000)       74 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/dispatch/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    17697 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/utils/dispatch/signal.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10550 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/functional.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9041 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/graph.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4826 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/imports.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2776 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/iso8601.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8626 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/log.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2858 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/nodenames.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6136 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/celery/utils/objects.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6788 2023-06-19 06:33:07.000000 deepfos-celery-1.0.3/celery/utils/psutil.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9084 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/saferepr.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8069 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/serialization.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.106570 deepfos-celery-1.0.3/celery/utils/static/
+-rw-rw-r--   0 wei       (1000) wei       (1000)      299 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/static/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2556 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/static/celery_128.png
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1093 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/sysinfo.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4568 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/utils/term.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5779 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/text.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9626 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/threads.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    12375 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/time.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4533 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/utils/timer2.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.106570 deepfos-celery-1.0.3/celery/worker/
+-rw-rw-r--   0 wei       (1000) wei       (1000)       95 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4593 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/autoscale.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7517 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/components.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.110570 deepfos-celery-1.0.3/celery/worker/consumer/
+-rw-rw-r--   0 wei       (1000) wei       (1000)      391 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/consumer/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      525 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/consumer/agent.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1026 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/consumer/connection.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    21497 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/worker/consumer/consumer.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      946 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/consumer/control.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2054 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/consumer/events.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6833 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/consumer/gossip.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      930 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/consumer/heart.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2519 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/consumer/mingle.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1959 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/worker/consumer/tasks.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    16771 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/worker/control.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2107 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/heartbeat.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3857 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/worker/loops.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3630 2022-09-23 05:23:46.000000 deepfos-celery-1.0.3/celery/worker/pidbox.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    22670 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/worker/request.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7639 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/worker/state.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6893 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/celery/worker/strategy.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    14521 2022-10-13 11:56:05.000000 deepfos-celery-1.0.3/celery/worker/worker.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.110570 deepfos-celery-1.0.3/deepfos_celery.egg-info/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4234 2023-06-19 06:39:44.000000 deepfos-celery-1.0.3/deepfos_celery.egg-info/PKG-INFO
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10254 2023-06-19 06:39:44.000000 deepfos-celery-1.0.3/deepfos_celery.egg-info/SOURCES.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        1 2023-06-19 06:39:44.000000 deepfos-celery-1.0.3/deepfos_celery.egg-info/dependency_links.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       48 2023-06-19 06:39:44.000000 deepfos-celery-1.0.3/deepfos_celery.egg-info/entry_points.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        1 2023-03-24 03:47:52.000000 deepfos-celery-1.0.3/deepfos_celery.egg-info/not-zip-safe
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1302 2023-06-19 06:39:44.000000 deepfos-celery-1.0.3/deepfos_celery.egg-info/requires.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        7 2023-06-19 06:39:44.000000 deepfos-celery-1.0.3/deepfos_celery.egg-info/top_level.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        1 2023-02-17 09:55:35.000000 deepfos-celery-1.0.3/pyproject.toml
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.114570 deepfos-celery-1.0.3/requirements/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1454 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/README.rst
+-rw-rw-r--   0 wei       (1000) wei       (1000)      153 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/requirements/default.txt
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.114570 deepfos-celery-1.0.3/requirements/deps/
+-rw-rw-r--   0 wei       (1000) wei       (1000)       10 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/deps/mock.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      145 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/dev.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      150 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/docs.txt
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.118570 deepfos-celery-1.0.3/requirements/extras/
+-rw-rw-r--   0 wei       (1000) wei       (1000)       15 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/arangodb.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/auth.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       70 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/azureblockblob.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      111 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/brotli.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       24 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/cassandra.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/consul.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       20 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/cosmosdbsql.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       17 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/couchbase.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       10 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/couchdb.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/django.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       15 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/dynamodb.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/elasticsearch.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       17 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/eventlet.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/gevent.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       19 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/librabbitmq.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       36 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/lzma.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       38 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/memcache.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       20 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/mongodb.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        8 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/msgpack.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       17 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/pymemcache.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        6 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/pyro.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/pytest.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/redis.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       15 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/s3.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       27 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/slmq.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        6 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/solar.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       11 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/sqlalchemy.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       82 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/sqs.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       73 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/tblib.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       39 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/thread.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/yaml.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       14 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/zeromq.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       13 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/extras/zookeeper.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       10 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/extras/zstd.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      266 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/pkgutils.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       19 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/security.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      148 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/test-ci-base.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      550 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/test-ci-default.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      128 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/requirements/test-integration.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       17 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/requirements/test-pypy3.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      181 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/requirements/test.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      932 2023-06-19 06:39:44.138571 deepfos-celery-1.0.3/setup.cfg
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5202 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/setup.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.118570 deepfos-celery-1.0.3/t/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1939 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/base.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.118570 deepfos-celery-1.0.3/t/benchmarks/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2841 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/benchmarks/bench_worker.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.118570 deepfos-celery-1.0.3/t/distro/
+-rw-rw-r--   0 wei       (1000) wei       (1000)      873 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/distro/test_CI_reqs.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.118570 deepfos-celery-1.0.3/t/integration/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/integration/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3745 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/integration/conftest.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4181 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/integration/redissrv.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9890 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/integration/tasks.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3582 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/integration/test_aiocanvas.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    11040 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/integration/test_aiotasks.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3792 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/integration/test_auto_recovery.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1120 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/integration/test_backend.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    44519 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/integration/test_canvas.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3459 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/integration/test_security.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9728 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/integration/test_tasks.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)       91 2023-03-14 10:22:23.000000 deepfos-celery-1.0.3/t/integration/test_tmp.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2435 2023-02-20 09:08:26.000000 deepfos-celery-1.0.3/t/integration/test_tmp2.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      226 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/skip.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.122570 deepfos-celery-1.0.3/t/unit/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/__init__.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.122570 deepfos-celery-1.0.3/t/unit/aio/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2023-02-16 09:50:39.000000 deepfos-celery-1.0.3/t/unit/aio/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    19025 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/unit/aio/test_aio_control.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.122570 deepfos-celery-1.0.3/t/unit/app/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/app/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    13048 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_amqp.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1331 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/app/test_annotations.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    39009 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/t/unit/app/test_app.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1294 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_backends.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    27400 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_beat.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5475 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_builtins.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      356 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/app/test_celery.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    17367 2023-03-31 03:05:26.000000 deepfos-celery-1.0.3/t/unit/app/test_control.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1627 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_defaults.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      692 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_exceptions.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8637 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_loaders.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10946 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_log.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2342 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/app/test_registry.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7829 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_routes.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    30264 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/app/test_schedules.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1790 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/app/test_utils.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.126570 deepfos-celery-1.0.3/t/unit/apps/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/apps/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    16253 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/apps/test_multi.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.126570 deepfos-celery-1.0.3/t/unit/backends/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/backends/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4266 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_arangodb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6338 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_asynchronous.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3355 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_azureblockblob.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    40815 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_base.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10297 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_cache.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6982 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_cassandra.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      940 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_consul.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4987 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/backends/test_cosmosdbsql.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4847 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_couchbase.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3972 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_couchdb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    14924 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_database.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    19265 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_dynamodb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    32594 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/backends/test_elasticsearch.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3021 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_filesystem.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    25643 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_mongodb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    43068 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/backends/test_redis.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3685 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/backends/test_rpc.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     6654 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/backends/test_s3.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.126570 deepfos-celery-1.0.3/t/unit/bin/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/bin/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)       18 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/bin/celery.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.130571 deepfos-celery-1.0.3/t/unit/bin/proj/
+-rw-rw-r--   0 wei       (1000) wei       (1000)       64 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/bin/proj/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)       62 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/bin/proj/app.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)       28 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/bin/proj/app2.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/bin/test_multi.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.130571 deepfos-celery-1.0.3/t/unit/concurrency/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/concurrency/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     4620 2022-09-23 05:35:24.000000 deepfos-celery-1.0.3/t/unit/concurrency/test_concurrency.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3625 2023-02-17 02:14:28.000000 deepfos-celery-1.0.3/t/unit/concurrency/test_eventlet.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3132 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/concurrency/test_gevent.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1830 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/concurrency/test_pool.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    14713 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/concurrency/test_prefork.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      848 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/concurrency/test_solo.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      728 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/concurrency/test_thread.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10358 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/conftest.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.130571 deepfos-celery-1.0.3/t/unit/contrib/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/__init__.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.130571 deepfos-celery-1.0.3/t/unit/contrib/proj/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/proj/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      183 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/proj/conf.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)       93 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/proj/contents.rst
+-rw-rw-r--   0 wei       (1000) wei       (1000)      249 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/proj/foo.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      113 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/proj/xyzzy.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1387 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/test_abortable.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10713 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/contrib/test_migrate.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      785 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/test_pytest.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3146 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/contrib/test_rdb.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      767 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/contrib/test_sphinx.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.130571 deepfos-celery-1.0.3/t/unit/events/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/events/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2297 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/events/test_cursesmon.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    11372 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/events/test_events.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3378 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/events/test_snapshot.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    22295 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/events/test_state.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.130571 deepfos-celery-1.0.3/t/unit/fixups/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/fixups/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10834 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/fixups/test_django.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.130571 deepfos-celery-1.0.3/t/unit/security/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3584 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/security/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      102 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/security/case.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3226 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/security/test_certificate.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1069 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/security/test_key.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5492 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/security/test_security.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2218 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/security/test_serialization.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.134571 deepfos-celery-1.0.3/t/unit/tasks/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/tasks/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    43214 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/tasks/test_canvas.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10978 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/tasks/test_chord.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2334 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/tasks/test_context.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    34926 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/tasks/test_result.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1085 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/tasks/test_states.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    50867 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/tasks/test_tasks.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    15374 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/tasks/test_trace.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)       78 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/tasks/unit_tasks.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      989 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/test_canvas.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.134571 deepfos-celery-1.0.3/t/unit/utils/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/utils/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    12877 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_collections.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2357 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/utils/test_debug.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1737 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_deprecated.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    12101 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/unit/utils/test_dispatcher.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7456 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_functional.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1935 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/utils/test_graph.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3308 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_imports.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     8161 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_local.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      202 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/utils/test_nodenames.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1351 2023-04-11 10:12:13.000000 deepfos-celery-1.0.3/t/unit/utils/test_objects.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1394 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_pickle.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    26066 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_platforms.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5565 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_saferepr.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     3427 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_serialization.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      751 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/utils/test_sysinfo.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1734 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/utils/test_term.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1968 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_text.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2453 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_threads.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    11730 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_time.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2744 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/utils/test_timer2.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      624 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/utils/test_utils.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-19 06:39:44.138571 deepfos-celery-1.0.3/t/unit/worker/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        0 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/worker/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     7221 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/worker/test_autoscale.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9401 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/worker/test_bootsteps.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2454 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/worker/test_components.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    21360 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/worker/test_consumer.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    23385 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/worker/test_control.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2384 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/worker/test_heartbeat.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    16236 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/worker/test_loops.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    41778 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/worker/test_request.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)      238 2022-09-23 05:23:47.000000 deepfos-celery-1.0.3/t/unit/worker/test_revoke.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     5268 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/worker/test_state.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)     9760 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/worker/test_strategy.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    39836 2022-09-23 05:35:05.000000 deepfos-celery-1.0.3/t/unit/worker/test_worker.py
```

### Comparing `deepfos-celery-1.0.2/CONTRIBUTORS.txt` & `deepfos-celery-1.0.3/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/Changelog.rst` & `deepfos-celery-1.0.3/Changelog.rst`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/LICENSE` & `deepfos-celery-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/MANIFEST.in` & `deepfos-celery-1.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/PKG-INFO` & `deepfos-celery-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfos-celery
-Version: 1.0.2
+Version: 1.0.3
 Summary: Distributed Task Queue.
 Home-page: http://celeryproject.org
 Author: DeepFOS
 Author-email: python@deepfinance.com
 License: BSD
 Project-URL: Documentation, http://docs.celeryproject.org/en/latest/index.html
 Project-URL: Code, https://gitee.com/python-development-team/deepfos-celery/
@@ -22,121 +22,121 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6,
-Provides-Extra: pymemcache
-Provides-Extra: pyro
-Provides-Extra: sqs
-Provides-Extra: s3
+Provides-Extra: auth
 Provides-Extra: cassandra
+Provides-Extra: pyro
+Provides-Extra: gevent
 Provides-Extra: mongodb
-Provides-Extra: zookeeper
-Provides-Extra: azureblockblob
-Provides-Extra: eventlet
-Provides-Extra: solar
-Provides-Extra: tblib
-Provides-Extra: slmq
-Provides-Extra: sqlalchemy
-Provides-Extra: auth
-Provides-Extra: zstd
-Provides-Extra: brotli
 Provides-Extra: couchbase
-Provides-Extra: dynamodb
-Provides-Extra: elasticsearch
-Provides-Extra: gevent
-Provides-Extra: arangodb
+Provides-Extra: cosmosdbsql
 Provides-Extra: pytest
-Provides-Extra: lzma
+Provides-Extra: sqlalchemy
 Provides-Extra: yaml
+Provides-Extra: pymemcache
+Provides-Extra: consul
 Provides-Extra: msgpack
-Provides-Extra: cosmosdbsql
+Provides-Extra: brotli
 Provides-Extra: django
+Provides-Extra: zookeeper
+Provides-Extra: lzma
+Provides-Extra: sqs
 Provides-Extra: redis
-Provides-Extra: consul
+Provides-Extra: s3
+Provides-Extra: couchdb
+Provides-Extra: azureblockblob
+Provides-Extra: dynamodb
+Provides-Extra: arangodb
+Provides-Extra: slmq
+Provides-Extra: tblib
 Provides-Extra: librabbitmq
+Provides-Extra: solar
 Provides-Extra: memcache
-Provides-Extra: couchdb
+Provides-Extra: zstd
+Provides-Extra: eventlet
+Provides-Extra: elasticsearch
 License-File: LICENSE
 
-.. image:: http://docs.celeryproject.org/en/latest/_images/celery-banner-small.png
-
-|license| |wheel| |pyversion|
-
-:Version: 1.0.0
-:Web: http://celeryproject.org/
-:Download: https://pypi.org/project/celery/
-:Source: https://gitee.com/python-development-team/deepfos-celery/
-:Keywords: task, queue, job, async, rabbitmq, amqp, redis,
-  python, distributed, actors
-
-What is this?
-=============
-
-本项目基于 ``celery-5.0.5`` 开发，主要功能是添加 ``asyncio`` 支持，
-以更好地和 ``FastAPI`` 等异步web框架配合使用。
-
-项目是 ``celery`` 的超集，但并非所有功能都支持 ``asyncio`` ，
-并且目前仅完成了 ``redis`` 作为 ``broker`` 和 ``backend`` 的支持。
-
-
-Get Started
-===========
-
-创建任务和官方 ``celery`` 一样:
-
-.. code-block:: python
-
-    from celery import Celery
-
-    app = Celery('hello', broker='redis://:@localhost/')
-
-    @app.task(aio_variant=True)
-    def hello():
-        return 'hello world'
-
-
-但增加了 ``aio_variant`` 这一参数，相较于普通的任务发送和获取结果的方式：
-
-.. code-block:: python
-
-    task = hello.apply_async()
-    result = task.get()
-
-
-可以使用:
-
-.. code-block:: python
-
-    task = await hello.aio.apply_async()
-    result = await task.get()
-
-
-**注意**
-
-    这不只是一个简单的语法糖，而是确实使用 ``aioredis`` 替换了原有 ``redis-py`` 的同步网络请求。
-
-
-.. _license:
-
-License
-=======
-
-This software is licensed under the `New BSD License`. See the ``LICENSE``
-file in the top distribution directory for the full license text.
-
-.. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
-
-.. |license| image:: https://img.shields.io/pypi/l/celery.svg
-    :alt: BSD License
-    :target: https://opensource.org/licenses/BSD-3-Clause
-
-.. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
-    :alt: Celery can be installed via wheel
-    :target: https://pypi.org/project/celery/
-
-.. |pyversion| image:: https://img.shields.io/pypi/pyversions/celery.svg
-    :alt: Supported Python versions.
-    :target: https://pypi.org/project/celery/
-
+.. image:: http://docs.celeryproject.org/en/latest/_images/celery-banner-small.png
+
+|license| |wheel| |pyversion|
+
+:Version: 1.0.0
+:Web: http://celeryproject.org/
+:Download: https://pypi.org/project/celery/
+:Source: https://gitee.com/python-development-team/deepfos-celery/
+:Keywords: task, queue, job, async, rabbitmq, amqp, redis,
+  python, distributed, actors
+
+What is this?
+=============
+
+本项目基于 ``celery-5.0.5`` 开发，主要功能是添加 ``asyncio`` 支持，
+以更好地和 ``FastAPI`` 等异步web框架配合使用。
+
+项目是 ``celery`` 的超集，但并非所有功能都支持 ``asyncio`` ，
+并且目前仅完成了 ``redis`` 作为 ``broker`` 和 ``backend`` 的支持。
+
+
+Get Started
+===========
+
+创建任务和官方 ``celery`` 一样:
+
+.. code-block:: python
+
+    from celery import Celery
+
+    app = Celery('hello', broker='redis://:@localhost/')
+
+    @app.task(aio_variant=True)
+    def hello():
+        return 'hello world'
+
+
+但增加了 ``aio_variant`` 这一参数，相较于普通的任务发送和获取结果的方式：
+
+.. code-block:: python
+
+    task = hello.apply_async()
+    result = task.get()
+
+
+可以使用:
+
+.. code-block:: python
+
+    task = await hello.aio.apply_async()
+    result = await task.get()
+
+
+**注意**
+
+    这不只是一个简单的语法糖，而是确实使用 ``aioredis`` 替换了原有 ``redis-py`` 的同步网络请求。
+
+
+.. _license:
+
+License
+=======
+
+This software is licensed under the `New BSD License`. See the ``LICENSE``
+file in the top distribution directory for the full license text.
+
+.. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
+
+.. |license| image:: https://img.shields.io/pypi/l/celery.svg
+    :alt: BSD License
+    :target: https://opensource.org/licenses/BSD-3-Clause
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
+    :alt: Celery can be installed via wheel
+    :target: https://pypi.org/project/celery/
+
+.. |pyversion| image:: https://img.shields.io/pypi/pyversions/celery.svg
+    :alt: Supported Python versions.
+    :target: https://pypi.org/project/celery/
+
```

### Comparing `deepfos-celery-1.0.2/README.rst` & `deepfos-celery-1.0.3/README.rst`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-.. image:: http://docs.celeryproject.org/en/latest/_images/celery-banner-small.png
-
-|license| |wheel| |pyversion|
-
-:Version: 1.0.0
-:Web: http://celeryproject.org/
-:Download: https://pypi.org/project/celery/
-:Source: https://gitee.com/python-development-team/deepfos-celery/
-:Keywords: task, queue, job, async, rabbitmq, amqp, redis,
-  python, distributed, actors
-
-What is this?
-=============
-
-本项目基于 ``celery-5.0.5`` 开发，主要功能是添加 ``asyncio`` 支持，
-以更好地和 ``FastAPI`` 等异步web框架配合使用。
-
-项目是 ``celery`` 的超集，但并非所有功能都支持 ``asyncio`` ，
-并且目前仅完成了 ``redis`` 作为 ``broker`` 和 ``backend`` 的支持。
-
-
-Get Started
-===========
-
-创建任务和官方 ``celery`` 一样:
-
-.. code-block:: python
-
-    from celery import Celery
-
-    app = Celery('hello', broker='redis://:@localhost/')
-
-    @app.task(aio_variant=True)
-    def hello():
-        return 'hello world'
-
-
-但增加了 ``aio_variant`` 这一参数，相较于普通的任务发送和获取结果的方式：
-
-.. code-block:: python
-
-    task = hello.apply_async()
-    result = task.get()
-
-
-可以使用:
-
-.. code-block:: python
-
-    task = await hello.aio.apply_async()
-    result = await task.get()
-
-
-**注意**
-
-    这不只是一个简单的语法糖，而是确实使用 ``aioredis`` 替换了原有 ``redis-py`` 的同步网络请求。
-
-
-.. _license:
-
-License
-=======
-
-This software is licensed under the `New BSD License`. See the ``LICENSE``
-file in the top distribution directory for the full license text.
-
-.. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
-
-.. |license| image:: https://img.shields.io/pypi/l/celery.svg
-    :alt: BSD License
-    :target: https://opensource.org/licenses/BSD-3-Clause
-
-.. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
-    :alt: Celery can be installed via wheel
-    :target: https://pypi.org/project/celery/
-
-.. |pyversion| image:: https://img.shields.io/pypi/pyversions/celery.svg
-    :alt: Supported Python versions.
-    :target: https://pypi.org/project/celery/
-
+.. image:: http://docs.celeryproject.org/en/latest/_images/celery-banner-small.png
+
+|license| |wheel| |pyversion|
+
+:Version: 1.0.0
+:Web: http://celeryproject.org/
+:Download: https://pypi.org/project/celery/
+:Source: https://gitee.com/python-development-team/deepfos-celery/
+:Keywords: task, queue, job, async, rabbitmq, amqp, redis,
+  python, distributed, actors
+
+What is this?
+=============
+
+本项目基于 ``celery-5.0.5`` 开发，主要功能是添加 ``asyncio`` 支持，
+以更好地和 ``FastAPI`` 等异步web框架配合使用。
+
+项目是 ``celery`` 的超集，但并非所有功能都支持 ``asyncio`` ，
+并且目前仅完成了 ``redis`` 作为 ``broker`` 和 ``backend`` 的支持。
+
+
+Get Started
+===========
+
+创建任务和官方 ``celery`` 一样:
+
+.. code-block:: python
+
+    from celery import Celery
+
+    app = Celery('hello', broker='redis://:@localhost/')
+
+    @app.task(aio_variant=True)
+    def hello():
+        return 'hello world'
+
+
+但增加了 ``aio_variant`` 这一参数，相较于普通的任务发送和获取结果的方式：
+
+.. code-block:: python
+
+    task = hello.apply_async()
+    result = task.get()
+
+
+可以使用:
+
+.. code-block:: python
+
+    task = await hello.aio.apply_async()
+    result = await task.get()
+
+
+**注意**
+
+    这不只是一个简单的语法糖，而是确实使用 ``aioredis`` 替换了原有 ``redis-py`` 的同步网络请求。
+
+
+.. _license:
+
+License
+=======
+
+This software is licensed under the `New BSD License`. See the ``LICENSE``
+file in the top distribution directory for the full license text.
+
+.. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
+
+.. |license| image:: https://img.shields.io/pypi/l/celery.svg
+    :alt: BSD License
+    :target: https://opensource.org/licenses/BSD-3-Clause
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
+    :alt: Celery can be installed via wheel
+    :target: https://pypi.org/project/celery/
+
+.. |pyversion| image:: https://img.shields.io/pypi/pyversions/celery.svg
+    :alt: Supported Python versions.
+    :target: https://pypi.org/project/celery/
+
```

### Comparing `deepfos-celery-1.0.2/celery/_state.py` & `deepfos-celery-1.0.3/celery/_state.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/aio/amqp.py` & `deepfos-celery-1.0.3/celery/aio/amqp.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-from kombu import Exchange
-from kombu.common import Broadcast
-from kombu.utils import cached_property
-
-from celery.app.amqp import AMQP
-from celery.aio import pools
-from celery.aio.messaging import Producer
-from celery.aio.connection import Connection
-from celery.aio.entity import Queue
-from celery import signals
-
-
-class AioAMQP(AMQP):
-    Producer = Producer
-    Connection = Connection
-
-    @property
-    def producer_pool(self):
-        if self._producer_pool is None:
-            self._producer_pool = pools.producers[
-                self.app.aconnection_for_write()]
-            self._producer_pool.limit = self.app.pool.limit
-        return self._producer_pool
-
-    def _create_task_sender(self):
-        default_retry = self.app.conf.task_publish_retry
-        default_policy = self.app.conf.task_publish_retry_policy
-        default_delivery_mode = self.app.conf.task_default_delivery_mode
-        default_queue = self.default_queue
-        queues = self.queues
-        send_before_publish = signals.before_task_publish.asend
-        before_receivers = signals.before_task_publish.areceivers
-        send_after_publish = signals.after_task_publish.asend
-        after_receivers = signals.after_task_publish.areceivers
-
-        send_task_sent = signals.task_sent.asend   # XXX compat
-        sent_receivers = signals.task_sent.areceivers
-
-        default_evd = self._event_dispatcher
-        default_exchange = self.default_exchange
-
-        default_rkey = self.app.conf.task_default_routing_key
-        default_serializer = self.app.conf.task_serializer
-        default_compressor = self.app.conf.result_compression
-
-        async def send_task_message(
-            producer, name, message,
-            exchange=None, routing_key=None, queue=None,
-            event_dispatcher=None,
-            retry=None, retry_policy=None,
-            serializer=None, delivery_mode=None,
-            compression=None, declare=None,
-            headers=None, exchange_type=None, **kwargs
-        ):
-            retry = default_retry if retry is None else retry
-            headers2, properties, body, sent_event = message
-            if headers:
-                headers2.update(headers)
-            if kwargs:
-                properties.update(kwargs)
-
-            qname = queue
-            if queue is None and exchange is None:
-                queue = default_queue
-            if queue is not None:
-                if isinstance(queue, str):
-                    qname, queue = queue, queues[queue]
-                else:
-                    qname = queue.name
-
-            if delivery_mode is None:
-                try:
-                    delivery_mode = queue.exchange.delivery_mode
-                except AttributeError:
-                    pass
-                delivery_mode = delivery_mode or default_delivery_mode
-
-            if exchange_type is None:
-                try:
-                    exchange_type = queue.exchange.type
-                except AttributeError:
-                    exchange_type = 'direct'
-
-            # convert to anon-exchange, when exchange not set and direct ex.
-            if (not exchange or not routing_key) and exchange_type == 'direct':
-                exchange, routing_key = '', qname
-            elif exchange is None:
-                # not topic exchange, and exchange not undefined
-                exchange = queue.exchange.name or default_exchange
-                routing_key = routing_key or queue.routing_key or default_rkey
-            if declare is None and queue and not isinstance(queue, Broadcast):
-                declare = [queue]
-
-            # merge default and custom policy
-            retry = default_retry if retry is None else retry
-            _rp = (dict(default_policy, **retry_policy) if retry_policy
-                   else default_policy)
-
-            if before_receivers:
-                await send_before_publish(
-                    sender=name, body=body,
-                    exchange=exchange, routing_key=routing_key,
-                    declare=declare, headers=headers2,
-                    properties=properties, retry_policy=retry_policy,
-                )
-            ret = await producer.publish(
-                body,
-                exchange=exchange,
-                routing_key=routing_key,
-                serializer=serializer or default_serializer,
-                compression=compression or default_compressor,
-                retry=retry, retry_policy=_rp,
-                delivery_mode=delivery_mode, declare=declare,
-                headers=headers2,
-                **properties
-            )
-            if after_receivers:
-                await send_after_publish(
-                    sender=name, body=body, headers=headers2,
-                    exchange=exchange, routing_key=routing_key
-                )
-            if sent_receivers:  # XXX deprecated
-                if isinstance(body, tuple):  # protocol version 2
-                    await send_task_sent(
-                        sender=name, task_id=headers2['id'], task=name,
-                        args=body[0], kwargs=body[1],
-                        eta=headers2['eta'], taskset=headers2['group'],
-                    )
-                else:  # protocol version 1
-                    await send_task_sent(
-                        sender=name, task_id=body['id'], task=name,
-                        args=body['args'], kwargs=body['kwargs'],
-                        eta=body['eta'], taskset=body['taskset'],
-                    )
-            if sent_event:
-                evd = event_dispatcher or default_evd
-                exname = exchange
-                if isinstance(exname, Exchange):
-                    exname = exname.name
-                sent_event.update({
-                    'queue': qname,
-                    'exchange': exname,
-                    'routing_key': routing_key,
-                })
-                await evd.publish('task-sent', sent_event,
-                            producer, retry=retry, retry_policy=retry_policy)
-            return ret
-        return send_task_message
-
-    def Queues(self, queues, create_missing=None,
-               autoexchange=None, max_priority=None):
-        # Create new :class:`Queues` instance, using queue defaults
-        # from the current configuration.
-        conf = self.app.conf
-        default_routing_key = conf.task_default_routing_key
-        if create_missing is None:
-            create_missing = conf.task_create_missing_queues
-        if max_priority is None:
-            max_priority = conf.task_queue_max_priority
-        if not queues and conf.task_default_queue:
-            queues = (Queue(conf.task_default_queue,
-                            exchange=self.default_exchange,
-                            routing_key=default_routing_key),)
-        autoexchange = (self.autoexchange if autoexchange is None
-                        else autoexchange)
-        return self.queues_cls(
-            queues, self.default_exchange, create_missing,
-            autoexchange, max_priority, default_routing_key,
-        )
-
-    @cached_property
-    def _event_dispatcher(self):
-        return self.app.aio_events.Dispatcher(enabled=False)
+from kombu import Exchange
+from kombu.common import Broadcast
+from kombu.utils import cached_property
+
+from celery.app.amqp import AMQP
+from celery.aio import pools
+from celery.aio.messaging import Producer
+from celery.aio.connection import Connection
+from celery.aio.entity import Queue
+from celery import signals
+
+
+class AioAMQP(AMQP):
+    Producer = Producer
+    Connection = Connection
+
+    @property
+    def producer_pool(self):
+        if self._producer_pool is None:
+            self._producer_pool = pools.producers[
+                self.app.aconnection_for_write()]
+            self._producer_pool.limit = self.app.pool.limit
+        return self._producer_pool
+
+    def _create_task_sender(self):
+        default_retry = self.app.conf.task_publish_retry
+        default_policy = self.app.conf.task_publish_retry_policy
+        default_delivery_mode = self.app.conf.task_default_delivery_mode
+        default_queue = self.default_queue
+        queues = self.queues
+        send_before_publish = signals.before_task_publish.asend
+        before_receivers = signals.before_task_publish.areceivers
+        send_after_publish = signals.after_task_publish.asend
+        after_receivers = signals.after_task_publish.areceivers
+
+        send_task_sent = signals.task_sent.asend   # XXX compat
+        sent_receivers = signals.task_sent.areceivers
+
+        default_evd = self._event_dispatcher
+        default_exchange = self.default_exchange
+
+        default_rkey = self.app.conf.task_default_routing_key
+        default_serializer = self.app.conf.task_serializer
+        default_compressor = self.app.conf.result_compression
+
+        async def send_task_message(
+            producer, name, message,
+            exchange=None, routing_key=None, queue=None,
+            event_dispatcher=None,
+            retry=None, retry_policy=None,
+            serializer=None, delivery_mode=None,
+            compression=None, declare=None,
+            headers=None, exchange_type=None, **kwargs
+        ):
+            retry = default_retry if retry is None else retry
+            headers2, properties, body, sent_event = message
+            if headers:
+                headers2.update(headers)
+            if kwargs:
+                properties.update(kwargs)
+
+            qname = queue
+            if queue is None and exchange is None:
+                queue = default_queue
+            if queue is not None:
+                if isinstance(queue, str):
+                    qname, queue = queue, queues[queue]
+                else:
+                    qname = queue.name
+
+            if delivery_mode is None:
+                try:
+                    delivery_mode = queue.exchange.delivery_mode
+                except AttributeError:
+                    pass
+                delivery_mode = delivery_mode or default_delivery_mode
+
+            if exchange_type is None:
+                try:
+                    exchange_type = queue.exchange.type
+                except AttributeError:
+                    exchange_type = 'direct'
+
+            # convert to anon-exchange, when exchange not set and direct ex.
+            if (not exchange or not routing_key) and exchange_type == 'direct':
+                exchange, routing_key = '', qname
+            elif exchange is None:
+                # not topic exchange, and exchange not undefined
+                exchange = queue.exchange.name or default_exchange
+                routing_key = routing_key or queue.routing_key or default_rkey
+            if declare is None and queue and not isinstance(queue, Broadcast):
+                declare = [queue]
+
+            # merge default and custom policy
+            retry = default_retry if retry is None else retry
+            _rp = (dict(default_policy, **retry_policy) if retry_policy
+                   else default_policy)
+
+            if before_receivers:
+                await send_before_publish(
+                    sender=name, body=body,
+                    exchange=exchange, routing_key=routing_key,
+                    declare=declare, headers=headers2,
+                    properties=properties, retry_policy=retry_policy,
+                )
+            ret = await producer.publish(
+                body,
+                exchange=exchange,
+                routing_key=routing_key,
+                serializer=serializer or default_serializer,
+                compression=compression or default_compressor,
+                retry=retry, retry_policy=_rp,
+                delivery_mode=delivery_mode, declare=declare,
+                headers=headers2,
+                **properties
+            )
+            if after_receivers:
+                await send_after_publish(
+                    sender=name, body=body, headers=headers2,
+                    exchange=exchange, routing_key=routing_key
+                )
+            if sent_receivers:  # XXX deprecated
+                if isinstance(body, tuple):  # protocol version 2
+                    await send_task_sent(
+                        sender=name, task_id=headers2['id'], task=name,
+                        args=body[0], kwargs=body[1],
+                        eta=headers2['eta'], taskset=headers2['group'],
+                    )
+                else:  # protocol version 1
+                    await send_task_sent(
+                        sender=name, task_id=body['id'], task=name,
+                        args=body['args'], kwargs=body['kwargs'],
+                        eta=body['eta'], taskset=body['taskset'],
+                    )
+            if sent_event:
+                evd = event_dispatcher or default_evd
+                exname = exchange
+                if isinstance(exname, Exchange):
+                    exname = exname.name
+                sent_event.update({
+                    'queue': qname,
+                    'exchange': exname,
+                    'routing_key': routing_key,
+                })
+                await evd.publish('task-sent', sent_event,
+                            producer, retry=retry, retry_policy=retry_policy)
+            return ret
+        return send_task_message
+
+    def Queues(self, queues, create_missing=None,
+               autoexchange=None, max_priority=None):
+        # Create new :class:`Queues` instance, using queue defaults
+        # from the current configuration.
+        conf = self.app.conf
+        default_routing_key = conf.task_default_routing_key
+        if create_missing is None:
+            create_missing = conf.task_create_missing_queues
+        if max_priority is None:
+            max_priority = conf.task_queue_max_priority
+        if not queues and conf.task_default_queue:
+            queues = (Queue(conf.task_default_queue,
+                            exchange=self.default_exchange,
+                            routing_key=default_routing_key),)
+        autoexchange = (self.autoexchange if autoexchange is None
+                        else autoexchange)
+        return self.queues_cls(
+            queues, self.default_exchange, create_missing,
+            autoexchange, max_priority, default_routing_key,
+        )
+
+    @cached_property
+    def _event_dispatcher(self):
+        return self.app.aio_events.Dispatcher(enabled=False)
```

### Comparing `deepfos-celery-1.0.2/celery/aio/backend.py` & `deepfos-celery-1.0.3/celery/aio/backend.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,667 +1,667 @@
-import asyncio
-from collections import deque
-from typing import *
-from functools import partial
-from contextlib import asynccontextmanager
-import time
-import socket
-
-import aioredis.connection
-
-from celery.backends.redis import (
-    RedisBackend as SyncRedisBackend,
-    SentinelBackend as SyncSentinelBackend,
-    ResultConsumer as SyncResultConsumer,
-    task_join_will_block,
-    states,
-    logger,
-    ImproperlyConfigured,
-    E_RETRY_LIMIT_EXCEEDED,
-    E_REDIS_SENTINEL_MISSING,
-)
-from celery.backends.asynchronous import (
-    Empty,
-    Drainer as SyncDrainer,
-    register_drainer,
-    drainers,
-    detect_environment
-)
-from celery.backends.base import (
-    bytes_to_str,
-    get_exponential_backoff_interval,
-    raise_with_context,
-    BackendGetMetaError,
-    BackendStoreError,
-)
-from celery.exceptions import TimeoutError
-from celery.result import GroupResult
-
-from celery.aio.redis import get_redis_error_classes
-from celery.aio.utils import retry_over_time
-from celery.aio.result import result_from_tuple
-
-
-@register_drainer('aio-default')
-class Drainer(SyncDrainer):
-    if TYPE_CHECKING:
-        result_consumer: 'ResultConsumer'
-
-    def __init__(self, result_consumer):
-        self.result_consumer = result_consumer
-        self._started = False
-        self._drainer: asyncio.Task = None
-
-    async def drain_events_until(self, r, timeout=None, interval=1, on_interval=None, wait=None):
-        wait = wait or self.result_consumer.drain_events
-        p = r.on_ready
-        time_start = time.monotonic()
-
-        while 1:
-            # Total time spent may exceed a single call to wait()
-            if timeout and time.monotonic() - time_start >= timeout:
-                raise socket.timeout()
-            try:
-                await wait(r, interval)
-            except socket.timeout:
-                pass
-            if on_interval:
-                await on_interval()
-            if p.ready:  # got event on the wanted channel.
-                break
-
-    async def start(self):
-        await self.result_consumer.spawn_drainer()
-
-    def stop(self):
-        self.result_consumer.stop_drainer()
-
-
-class ResultConsumer(SyncResultConsumer):
-    if TYPE_CHECKING:
-        from aioredis.client import PubSub
-
-        backend: 'RedisBackend'
-        _pubsub: PubSub
-        drainer: Drainer
-        _running_drainer: asyncio.Task
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.drainer = drainers['aio-' + detect_environment()](self)
-        self._running_drainer = None
-        self._pubsub_lock = asyncio.Lock()
-
-    async def on_after_fork(self):
-        try:
-            self.backend.client.connection_pool.reset()
-            if self._pubsub is not None:
-                await self._pubsub.close()
-        except KeyError as e:
-            logger.warning(str(e))
-
-    async def _reconnect_pubsub(self):
-        self._pubsub = None
-        self.backend.client.connection_pool.reset()
-        # task state might have changed when the connection was down so we
-        # retrieve meta for all subscribed tasks before going into pubsub mode
-        metas = await self.backend.client.mget(self.subscribed_to)
-        metas = [meta for meta in metas if meta]
-        for meta in metas:
-            await self.on_state_change(self._decode_result(meta), None)
-        self._pubsub = self.backend.client.pubsub(
-            ignore_subscribe_messages=True,
-        )
-        if self.subscribed_to:
-            async with self._pubsub_lock:
-                await self._pubsub.subscribe(*self.subscribed_to)
-
-    @asynccontextmanager
-    async def reconnect_on_error(self):
-        try:
-            yield
-        except self._connection_errors:
-            try:
-                await self._ensure(self._reconnect_pubsub, ())
-            except self._connection_errors:
-                logger.critical(E_RETRY_LIMIT_EXCEEDED)
-                raise
-
-    async def _maybe_cancel_ready_task(self, meta):
-        if meta['status'] in states.READY_STATES:
-            await self.cancel_for(meta['task_id'])
-
-    async def on_state_change(self, meta, message):
-        if self.on_message:
-            self.on_message(meta)
-        if meta['status'] in states.READY_STATES:
-            task_id = meta['task_id']
-            try:
-                result = self._get_pending_result(task_id)
-            except KeyError:
-                # send to buffer in case we received this result
-                # before it was added to _pending_results.
-                self._pending_messages.put(task_id, meta)
-            else:
-                await result._maybe_set_cache(meta)
-                buckets = self.buckets
-                try:
-                    # remove bucket for this result, since it's fulfilled
-                    bucket = buckets.pop(result)
-                except KeyError:
-                    pass
-                else:
-                    # send to waiter via bucket
-                    bucket.append(result)
-        await asyncio.sleep(0)
-        await self._maybe_cancel_ready_task(meta)
-
-    async def start(self, initial_task_id, **kwargs):
-        self._pubsub = self.backend.client.pubsub(
-            ignore_subscribe_messages=True,
-        )
-        await self._consume_from(initial_task_id)
-
-    async def on_wait_for_pending(self, result, **kwargs):
-        for meta in await result._iter_meta(**kwargs):
-            if meta is not None:
-                await self.on_state_change(meta, None)
-
-    async def stop(self):
-        if self._pubsub is not None:
-            await self._pubsub.close()
-
-    async def _drain_events(self):
-        logger.debug(f'start drainer on channel: [{self._pubsub.channels}]')
-        async with self.reconnect_on_error():
-            async for message in self._pubsub.listen():
-                if message and message['type'] == 'message':
-                    logger.info(f'got message: {message}')
-                    await self.on_state_change(
-                        self._decode_result(message['data']), message
-                    )
-
-        logger.debug(f'stoping drainer... | '
-                     f'subscribed: {self._pubsub.subscribed}')
-        self._running_drainer = None
-
-    async def spawn_drainer(self) -> Optional[asyncio.Task]:
-        if not self._pubsub:
-            return
-
-        if self._running_drainer is None:
-            self._running_drainer = asyncio.create_task(self._drain_events())
-            await asyncio.sleep(0)
-        return self._running_drainer
-
-    def stop_drainer(self):
-        if self._running_drainer is not None:
-            self._running_drainer.cancel()
-            self._running_drainer = None
-
-    async def drain_events(self, result, timeout=None):
-        await self.spawn_drainer()
-        await self.backend.wait_for_future(result, timeout)
-
-    async def consume_from(self, task_id):
-        if self._pubsub is None:
-            return await self.start(task_id)
-        await self._consume_from(task_id)
-
-    async def _consume_from(self, task_id):
-        key = self._get_key_for_task(task_id)
-        if key not in self.subscribed_to:
-            self.subscribed_to.add(key)
-            async with self.reconnect_on_error():
-                async with self._pubsub_lock:
-                    if self._pubsub:  # double check needed
-                        await self._pubsub.subscribe(key)
-
-    async def cancel_for(self, task_id):
-        key = self._get_key_for_task(task_id)
-        self.subscribed_to.discard(key)
-        if self._pubsub:
-            async with self.reconnect_on_error():
-                async with self._pubsub_lock:
-                    if self._pubsub:  # double check needed
-                        await self._pubsub.unsubscribe(key)
-
-    # -------------------------------------------------------
-    # celery.backends.asynchronou::BaseResultConsumer
-    async def _wait_for_pending(
-        self, result, timeout=None,
-        on_interval=None, on_message=None, **kwargs
-    ):
-        await self.on_wait_for_pending(result, timeout=timeout, **kwargs)
-        prev_on_m, self.on_message = self.on_message, on_message
-        try:
-            await self.drain_events_until(
-                result, timeout=timeout,
-                on_interval=on_interval
-            )
-        except socket.timeout:
-            raise TimeoutError('The operation timed out.')
-        finally:
-            self.on_message = prev_on_m
-
-    async def drain_events_until(self, r, timeout=None, on_interval=None):
-        return await self.drainer.drain_events_until(
-            r, timeout=timeout, on_interval=on_interval)
-
-
-class RedisBackend(SyncRedisBackend):
-    if TYPE_CHECKING:
-        @property
-        def client(self) -> aioredis.Redis: ...
-        result_consumer: ResultConsumer
-
-    ResultConsumer = ResultConsumer
-    redis = aioredis
-
-    def __init__(self, host=None, port=None, db=None, password=None,
-                 max_connections=None, url=None,
-                 connection_pool=None, **kwargs):
-        super().__init__(
-            host=host, port=port, db=db, password=password,
-            max_connections=max_connections, url=url,
-            connection_pool=connection_pool, **kwargs
-        )
-        self._pending_future: Dict[str, asyncio.Future] = {}
-
-    def get_redis_error_classes(self):
-        return get_redis_error_classes()
-
-    async def on_task_call(self, producer, task_id):
-        if not task_join_will_block():
-            await self.result_consumer.consume_from(task_id)
-
-    async def get(self, key):
-        return await self.client.get(key)
-
-    async def mget(self, keys):
-        return await self.client.mget(keys)
-
-    async def ensure(self, fun, args, **policy):
-        retry_policy = dict(self.retry_policy, **policy)
-        max_retries = retry_policy.get('max_retries')
-        return await retry_over_time(
-            fun, self.connection_errors, args, {},
-            partial(self.on_connection_error, max_retries),
-            **retry_policy
-        )
-
-    async def set(self, key, value, **retry_policy):
-        return await self.ensure(self._set, (key, value), **retry_policy)
-
-    async def _set(self, key, value):
-        async with self.client.pipeline() as pipe:
-            if self.expires:
-                pipe.setex(key, self.expires, value)
-            else:
-                pipe.set(key, value)
-            pipe.publish(key, value)
-            await pipe.execute()
-
-    async def remove_pending_result(self, result):
-        self._remove_pending_result(result.id)
-        await self.on_result_fulfilled(result)
-        return result
-
-    async def _forget(self, task_id):
-        await self.delete(self.get_key_for_task(task_id))
-
-    async def forget(self, task_id):
-        self._cache.pop(task_id, None)
-        await self._forget(task_id)
-        await self.result_consumer.cancel_for(task_id)
-
-    async def delete(self, key):
-        await self.client.delete(key)
-
-    async def incr(self, key):
-        return await self.client.incr(key)
-
-    async def expire(self, key, value):
-        return await self.client.expire(key, value)
-
-    async def add_to_chord(self, group_id, result):
-        await self.client.incr(self.get_key_for_group(group_id, '.t'), 1)
-
-    async def on_result_fulfilled(self, result):
-        await self.result_consumer.cancel_for(result.id)
-
-    async def add_pending_result(self, result, weak=False, start_drainer=True):
-        if start_drainer:
-            await self.result_consumer.drainer.start()
-        try:
-            await self._maybe_resolve_from_buffer(result)
-        except Empty:
-            await self._add_pending_result(result.id, result, weak=weak)
-        return result
-
-    async def _maybe_resolve_from_buffer(self, result):
-        await result._maybe_set_cache(self._pending_messages.take(result.id))
-
-    async def _add_pending_result(self, task_id, result, weak=False):
-        concrete, weak_ = self._pending_results
-        if task_id not in weak_ and result.id not in concrete:
-            (weak_ if weak else concrete)[task_id] = result
-            await self.result_consumer.consume_from(task_id)
-            self._pending_future[task_id] = \
-                asyncio.get_running_loop().create_future()
-        else:
-            ori_result = weak_.get(task_id, concrete.get(task_id))
-            await ori_result.on_ready.then(result.on_ready)
-
-    async def add_pending_results(self, results, weak=False):
-        await self.result_consumer.drainer.start()
-        return [
-            await self.add_pending_result(
-                result, weak=weak, start_drainer=False)
-            for result in results
-        ]
-
-    async def wait_for_pending(self, result,
-                         callback=None, propagate=True, **kwargs):
-        self._ensure_not_eager()
-        await self._wait_for_pending(result, **kwargs)
-        return await result.maybe_throw(callback=callback, propagate=propagate)
-
-    async def _wait_for_pending(
-        self, result, timeout=None, on_interval=None,
-        on_message=None, **kwargs
-    ):
-        return await self.result_consumer._wait_for_pending(
-            result, timeout=timeout,
-            on_interval=on_interval, on_message=on_message,
-            **kwargs
-        )
-
-    async def _get_task_meta_for(self, task_id):
-        """Get task meta-data for a task by id."""
-        meta = await self.get(self.get_key_for_task(task_id))
-        if not meta:
-            return {'status': states.PENDING, 'result': None}
-        return self.decode_result(meta)
-
-    async def _store_result(self, task_id, result, state,
-                      traceback=None, request=None, **kwargs):
-        meta = self._get_result_meta(result=result, state=state,
-                                     traceback=traceback, request=request)
-        meta['task_id'] = bytes_to_str(task_id)
-
-        # Retrieve metadata from the backend, if the status
-        # is a success then we ignore any following update to the state.
-        # This solves a task deduplication issue because of network
-        # partitioning or lost workers. This issue involved a race condition
-        # making a lost task overwrite the last successful result in the
-        # result backend.
-        current_meta = await self._get_task_meta_for(task_id)
-
-        if current_meta['status'] == states.SUCCESS:
-            return result
-
-        await self._set_with_state(
-            self.get_key_for_task(task_id),
-            self.encode(meta), state
-        )
-        return result
-
-    async def get_task_meta(self, task_id, cache=True):
-        """Get task meta from backend.
-
-        if always_retry_backend_operation is activated, in the event of a recoverable exception,
-        then retry operation with an exponential backoff until a limit has been reached.
-        """
-        self._ensure_not_eager()
-        if cache:
-            try:
-                return self._cache[task_id]
-            except KeyError:
-                pass
-        retries = 0
-        while True:
-            try:
-                meta = await self._get_task_meta_for(task_id)
-                break
-            except Exception as exc:
-                if self.always_retry and self.exception_safe_to_retry(exc):
-                    if retries < self.max_retries:
-                        retries += 1
-
-                        # get_exponential_backoff_interval computes integers
-                        # and time.sleep accept floats for sub second sleep
-                        sleep_amount = get_exponential_backoff_interval(
-                            self.base_sleep_between_retries_ms, retries,
-                            self.max_sleep_between_retries_ms, True) / 1000
-                        await self._sleep(sleep_amount)
-                    else:
-                        raise_with_context(
-                            BackendGetMetaError("failed to get meta", task_id=task_id),
-                        )
-                else:
-                    raise
-
-        if cache and meta.get('status') == states.SUCCESS:
-            self._cache[task_id] = meta
-        return meta
-
-    async def store_result(self, task_id, result, state,
-                     traceback=None, request=None, **kwargs):
-        """Update task state and result.
-
-        if always_retry_backend_operation is activated, in the event of a recoverable exception,
-        then retry operation with an exponential backoff until a limit has been reached.
-        """
-        result = self.encode_result(result, state)
-
-        retries = 0
-
-        while True:
-            try:
-                await self._store_result(
-                    task_id, result, state, traceback,
-                    request=request, **kwargs)
-                return result
-            except Exception as exc:
-                if self.always_retry and self.exception_safe_to_retry(exc):
-                    if retries < self.max_retries:
-                        retries += 1
-
-                        # get_exponential_backoff_interval computes integers
-                        # and time.sleep accept floats for sub second sleep
-                        sleep_amount = get_exponential_backoff_interval(
-                            self.base_sleep_between_retries_ms, retries,
-                            self.max_sleep_between_retries_ms, True) / 1000
-                        await self._sleep(sleep_amount)
-                    else:
-                        raise_with_context(
-                            BackendStoreError("failed to store result on the backend", task_id=task_id, state=state),
-                        )
-                else:
-                    raise
-
-    async def _sleep(self, amount):
-        await asyncio.sleep(amount)
-
-    async def _set_with_state(self, key, value, state):
-        return await self.set(key, value)
-
-    async def _wait_for_single_future(self, result, timeout):
-        future = self._pending_future[result.id]
-        try:
-            await asyncio.wait_for(asyncio.shield(future), timeout=timeout)
-        except asyncio.TimeoutError:
-            pass
-
-    async def wait_for_future(self, result, timeout):
-        if isinstance(result, GroupResult):
-            results = result.results
-        else:
-            results = [result]
-
-        await asyncio.gather(*[
-            self._wait_for_single_future(r, timeout)
-            for r in results
-        ])
-
-    def maybe_set_future(self, task_id, result):
-        if task_id not in self._pending_future:
-            future = asyncio.get_running_loop().create_future()
-            self._pending_future[task_id] = future
-        else:
-            future: asyncio.Future = self._pending_future[task_id]
-
-        if not future.done():
-            logger.debug(f'Set result for task[{task_id}]: {result}')
-            future.set_result(result)
-
-    def remove_pending_future(self, task_id):
-        self._pending_future.pop(task_id, None)
-
-    async def restore_group(self, group_id, cache=True):
-        meta = await self.get_group_meta(group_id, cache=cache)
-        if meta:
-            return meta['result']
-
-    async def get_group_meta(self, group_id, cache=True):
-        self._ensure_not_eager()
-        if cache:
-            try:
-                return self._cache[group_id]
-            except KeyError:
-                pass
-
-        meta = await self._restore_group(group_id)
-        if cache and meta is not None:
-            self._cache[group_id] = meta
-        return meta
-
-    async def _restore_group(self, group_id):
-        """Get task meta-data for a task by id."""
-        meta = await self.get(self.get_key_for_group(group_id))
-        # previously this was always pickled, but later this
-        # was extended to support other serializers, so the
-        # structure is kind of weird.
-        if meta:
-            meta = self.decode(meta)
-            result = meta['result']
-            meta['result'] = await result_from_tuple(result, self.app)
-            return meta
-
-    async def _save_group(self, group_id, result):
-        await self._set_with_state(
-            self.get_key_for_group(group_id),
-            self.encode({'result': result.as_tuple()}),
-            states.SUCCESS
-        )
-        return result
-
-    async def iter_native(self, result, no_ack=True, **kwargs):
-        self._ensure_not_eager()
-
-        results = result.results
-        if not results:
-            raise StopIteration()
-
-        # we tell the result consumer to put consumed results
-        # into these buckets.
-        bucket = deque()
-        for node in results:
-            if not hasattr(node, '_cache'):
-                bucket.append(node)
-            elif node._cache:
-                bucket.append(node)
-            else:
-                self._collect_into(node, bucket)
-
-        await self._wait_for_pending(result, no_ack=no_ack, **kwargs)
-        while bucket:
-            node = bucket.popleft()
-            if not hasattr(node, '_cache'):
-                yield node.id, node.children
-            else:
-                yield node.id, node._cache
-
-        while bucket:
-            node = bucket.popleft()
-            yield node.id, node._cache
-
-    async def get_many(
-        self, task_ids, timeout=None, interval=0.5, no_ack=True,
-        on_message=None, on_interval=None, max_iterations=None,
-        READY_STATES=states.READY_STATES
-    ):
-        interval = 0.5 if interval is None else interval
-        ids = task_ids if isinstance(task_ids, set) else set(task_ids)
-        cached_ids = set()
-        cache = self._cache
-        for task_id in ids:
-            try:
-                cached = cache[task_id]
-            except KeyError:
-                pass
-            else:
-                if cached['status'] in READY_STATES:
-                    yield bytes_to_str(task_id), cached
-                    cached_ids.add(task_id)
-
-        ids.difference_update(cached_ids)
-        iterations = 0
-        while ids:
-            keys = list(ids)
-            r = self._mget_to_results(
-                await self.mget(
-                    [self.get_key_for_task(k)
-                     for k in keys]
-                ), keys, READY_STATES
-            )
-            cache.update(r)
-            ids.difference_update({bytes_to_str(v) for v in r})
-            for key, value in r.items():
-                if on_message is not None:
-                    on_message(value)
-                yield bytes_to_str(key), value
-            if timeout and iterations * interval >= timeout:
-                raise TimeoutError(f'Operation timed out ({timeout})')
-            if on_interval:
-                on_interval()
-            time.sleep(interval)  # don't busy loop.
-            iterations += 1
-            if max_iterations and iterations >= max_iterations:
-                break
-
-
-class SentinelBackend(RedisBackend):
-    try:
-        from aioredis import sentinel
-    except ImportError:
-        sentinel = None
-
-    if TYPE_CHECKING:
-        from aioredis.sentinel import Sentinel
-        def _get_sentinel_instance(self, **params) -> Sentinel: ...
-
-    def __init__(self, *args, **kwargs):
-        if self.sentinel is None:
-            raise ImproperlyConfigured(E_REDIS_SENTINEL_MISSING.strip())
-
-        super().__init__(*args, **kwargs)
-
-    def _params_from_url(self, url, defaults):
-        chunks = url.split(";")
-        connparams = dict(defaults, hosts=[])
-        for chunk in chunks:
-            data = super()._params_from_url(
-                url=chunk, defaults=defaults)
-            connparams['hosts'].append(data)
-        for param in ("host", "port", "db", "password"):
-            connparams.pop(param)
-
-        # Adding db/password in connparams to connect to the correct instance
-        for param in ("db", "password"):
-            if connparams['hosts'] and param in connparams['hosts'][0]:
-                connparams[param] = connparams['hosts'][0].get(param)
-        return connparams
-
-    _get_sentinel_instance = SyncSentinelBackend._get_sentinel_instance # noqa
-    _get_pool = SyncSentinelBackend._get_pool # noqa
+import asyncio
+from collections import deque
+from typing import *
+from functools import partial
+from contextlib import asynccontextmanager
+import time
+import socket
+
+import aioredis.connection
+
+from celery.backends.redis import (
+    RedisBackend as SyncRedisBackend,
+    SentinelBackend as SyncSentinelBackend,
+    ResultConsumer as SyncResultConsumer,
+    task_join_will_block,
+    states,
+    logger,
+    ImproperlyConfigured,
+    E_RETRY_LIMIT_EXCEEDED,
+    E_REDIS_SENTINEL_MISSING,
+)
+from celery.backends.asynchronous import (
+    Empty,
+    Drainer as SyncDrainer,
+    register_drainer,
+    drainers,
+    detect_environment
+)
+from celery.backends.base import (
+    bytes_to_str,
+    get_exponential_backoff_interval,
+    raise_with_context,
+    BackendGetMetaError,
+    BackendStoreError,
+)
+from celery.exceptions import TimeoutError
+from celery.result import GroupResult
+
+from celery.aio.redis import get_redis_error_classes
+from celery.aio.utils import retry_over_time
+from celery.aio.result import result_from_tuple
+
+
+@register_drainer('aio-default')
+class Drainer(SyncDrainer):
+    if TYPE_CHECKING:
+        result_consumer: 'ResultConsumer'
+
+    def __init__(self, result_consumer):
+        self.result_consumer = result_consumer
+        self._started = False
+        self._drainer: asyncio.Task = None
+
+    async def drain_events_until(self, r, timeout=None, interval=1, on_interval=None, wait=None):
+        wait = wait or self.result_consumer.drain_events
+        p = r.on_ready
+        time_start = time.monotonic()
+
+        while 1:
+            # Total time spent may exceed a single call to wait()
+            if timeout and time.monotonic() - time_start >= timeout:
+                raise socket.timeout()
+            try:
+                await wait(r, interval)
+            except socket.timeout:
+                pass
+            if on_interval:
+                await on_interval()
+            if p.ready:  # got event on the wanted channel.
+                break
+
+    async def start(self):
+        await self.result_consumer.spawn_drainer()
+
+    def stop(self):
+        self.result_consumer.stop_drainer()
+
+
+class ResultConsumer(SyncResultConsumer):
+    if TYPE_CHECKING:
+        from aioredis.client import PubSub
+
+        backend: 'RedisBackend'
+        _pubsub: PubSub
+        drainer: Drainer
+        _running_drainer: asyncio.Task
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.drainer = drainers['aio-' + detect_environment()](self)
+        self._running_drainer = None
+        self._pubsub_lock = asyncio.Lock()
+
+    async def on_after_fork(self):
+        try:
+            self.backend.client.connection_pool.reset()
+            if self._pubsub is not None:
+                await self._pubsub.close()
+        except KeyError as e:
+            logger.warning(str(e))
+
+    async def _reconnect_pubsub(self):
+        self._pubsub = None
+        self.backend.client.connection_pool.reset()
+        # task state might have changed when the connection was down so we
+        # retrieve meta for all subscribed tasks before going into pubsub mode
+        metas = await self.backend.client.mget(self.subscribed_to)
+        metas = [meta for meta in metas if meta]
+        for meta in metas:
+            await self.on_state_change(self._decode_result(meta), None)
+        self._pubsub = self.backend.client.pubsub(
+            ignore_subscribe_messages=True,
+        )
+        if self.subscribed_to:
+            async with self._pubsub_lock:
+                await self._pubsub.subscribe(*self.subscribed_to)
+
+    @asynccontextmanager
+    async def reconnect_on_error(self):
+        try:
+            yield
+        except self._connection_errors:
+            try:
+                await self._ensure(self._reconnect_pubsub, ())
+            except self._connection_errors:
+                logger.critical(E_RETRY_LIMIT_EXCEEDED)
+                raise
+
+    async def _maybe_cancel_ready_task(self, meta):
+        if meta['status'] in states.READY_STATES:
+            await self.cancel_for(meta['task_id'])
+
+    async def on_state_change(self, meta, message):
+        if self.on_message:
+            self.on_message(meta)
+        if meta['status'] in states.READY_STATES:
+            task_id = meta['task_id']
+            try:
+                result = self._get_pending_result(task_id)
+            except KeyError:
+                # send to buffer in case we received this result
+                # before it was added to _pending_results.
+                self._pending_messages.put(task_id, meta)
+            else:
+                await result._maybe_set_cache(meta)
+                buckets = self.buckets
+                try:
+                    # remove bucket for this result, since it's fulfilled
+                    bucket = buckets.pop(result)
+                except KeyError:
+                    pass
+                else:
+                    # send to waiter via bucket
+                    bucket.append(result)
+        await asyncio.sleep(0)
+        await self._maybe_cancel_ready_task(meta)
+
+    async def start(self, initial_task_id, **kwargs):
+        self._pubsub = self.backend.client.pubsub(
+            ignore_subscribe_messages=True,
+        )
+        await self._consume_from(initial_task_id)
+
+    async def on_wait_for_pending(self, result, **kwargs):
+        for meta in await result._iter_meta(**kwargs):
+            if meta is not None:
+                await self.on_state_change(meta, None)
+
+    async def stop(self):
+        if self._pubsub is not None:
+            await self._pubsub.close()
+
+    async def _drain_events(self):
+        logger.debug(f'start drainer on channel: [{self._pubsub.channels}]')
+        async with self.reconnect_on_error():
+            async for message in self._pubsub.listen():
+                if message and message['type'] == 'message':
+                    logger.info(f'got message: {message}')
+                    await self.on_state_change(
+                        self._decode_result(message['data']), message
+                    )
+
+        logger.debug(f'stoping drainer... | '
+                     f'subscribed: {self._pubsub.subscribed}')
+        self._running_drainer = None
+
+    async def spawn_drainer(self) -> Optional[asyncio.Task]:
+        if not self._pubsub:
+            return
+
+        if self._running_drainer is None:
+            self._running_drainer = asyncio.create_task(self._drain_events())
+            await asyncio.sleep(0)
+        return self._running_drainer
+
+    def stop_drainer(self):
+        if self._running_drainer is not None:
+            self._running_drainer.cancel()
+            self._running_drainer = None
+
+    async def drain_events(self, result, timeout=None):
+        await self.spawn_drainer()
+        await self.backend.wait_for_future(result, timeout)
+
+    async def consume_from(self, task_id):
+        if self._pubsub is None:
+            return await self.start(task_id)
+        await self._consume_from(task_id)
+
+    async def _consume_from(self, task_id):
+        key = self._get_key_for_task(task_id)
+        if key not in self.subscribed_to:
+            self.subscribed_to.add(key)
+            async with self.reconnect_on_error():
+                async with self._pubsub_lock:
+                    if self._pubsub:  # double check needed
+                        await self._pubsub.subscribe(key)
+
+    async def cancel_for(self, task_id):
+        key = self._get_key_for_task(task_id)
+        self.subscribed_to.discard(key)
+        if self._pubsub:
+            async with self.reconnect_on_error():
+                async with self._pubsub_lock:
+                    if self._pubsub:  # double check needed
+                        await self._pubsub.unsubscribe(key)
+
+    # -------------------------------------------------------
+    # celery.backends.asynchronou::BaseResultConsumer
+    async def _wait_for_pending(
+        self, result, timeout=None,
+        on_interval=None, on_message=None, **kwargs
+    ):
+        await self.on_wait_for_pending(result, timeout=timeout, **kwargs)
+        prev_on_m, self.on_message = self.on_message, on_message
+        try:
+            await self.drain_events_until(
+                result, timeout=timeout,
+                on_interval=on_interval
+            )
+        except socket.timeout:
+            raise TimeoutError('The operation timed out.')
+        finally:
+            self.on_message = prev_on_m
+
+    async def drain_events_until(self, r, timeout=None, on_interval=None):
+        return await self.drainer.drain_events_until(
+            r, timeout=timeout, on_interval=on_interval)
+
+
+class RedisBackend(SyncRedisBackend):
+    if TYPE_CHECKING:
+        @property
+        def client(self) -> aioredis.Redis: ...
+        result_consumer: ResultConsumer
+
+    ResultConsumer = ResultConsumer
+    redis = aioredis
+
+    def __init__(self, host=None, port=None, db=None, password=None,
+                 max_connections=None, url=None,
+                 connection_pool=None, **kwargs):
+        super().__init__(
+            host=host, port=port, db=db, password=password,
+            max_connections=max_connections, url=url,
+            connection_pool=connection_pool, **kwargs
+        )
+        self._pending_future: Dict[str, asyncio.Future] = {}
+
+    def get_redis_error_classes(self):
+        return get_redis_error_classes()
+
+    async def on_task_call(self, producer, task_id):
+        if not task_join_will_block():
+            await self.result_consumer.consume_from(task_id)
+
+    async def get(self, key):
+        return await self.client.get(key)
+
+    async def mget(self, keys):
+        return await self.client.mget(keys)
+
+    async def ensure(self, fun, args, **policy):
+        retry_policy = dict(self.retry_policy, **policy)
+        max_retries = retry_policy.get('max_retries')
+        return await retry_over_time(
+            fun, self.connection_errors, args, {},
+            partial(self.on_connection_error, max_retries),
+            **retry_policy
+        )
+
+    async def set(self, key, value, **retry_policy):
+        return await self.ensure(self._set, (key, value), **retry_policy)
+
+    async def _set(self, key, value):
+        async with self.client.pipeline() as pipe:
+            if self.expires:
+                pipe.setex(key, self.expires, value)
+            else:
+                pipe.set(key, value)
+            pipe.publish(key, value)
+            await pipe.execute()
+
+    async def remove_pending_result(self, result):
+        self._remove_pending_result(result.id)
+        await self.on_result_fulfilled(result)
+        return result
+
+    async def _forget(self, task_id):
+        await self.delete(self.get_key_for_task(task_id))
+
+    async def forget(self, task_id):
+        self._cache.pop(task_id, None)
+        await self._forget(task_id)
+        await self.result_consumer.cancel_for(task_id)
+
+    async def delete(self, key):
+        await self.client.delete(key)
+
+    async def incr(self, key):
+        return await self.client.incr(key)
+
+    async def expire(self, key, value):
+        return await self.client.expire(key, value)
+
+    async def add_to_chord(self, group_id, result):
+        await self.client.incr(self.get_key_for_group(group_id, '.t'), 1)
+
+    async def on_result_fulfilled(self, result):
+        await self.result_consumer.cancel_for(result.id)
+
+    async def add_pending_result(self, result, weak=False, start_drainer=True):
+        if start_drainer:
+            await self.result_consumer.drainer.start()
+        try:
+            await self._maybe_resolve_from_buffer(result)
+        except Empty:
+            await self._add_pending_result(result.id, result, weak=weak)
+        return result
+
+    async def _maybe_resolve_from_buffer(self, result):
+        await result._maybe_set_cache(self._pending_messages.take(result.id))
+
+    async def _add_pending_result(self, task_id, result, weak=False):
+        concrete, weak_ = self._pending_results
+        if task_id not in weak_ and result.id not in concrete:
+            (weak_ if weak else concrete)[task_id] = result
+            await self.result_consumer.consume_from(task_id)
+            self._pending_future[task_id] = \
+                asyncio.get_running_loop().create_future()
+        else:
+            ori_result = weak_.get(task_id, concrete.get(task_id))
+            await ori_result.on_ready.then(result.on_ready)
+
+    async def add_pending_results(self, results, weak=False):
+        await self.result_consumer.drainer.start()
+        return [
+            await self.add_pending_result(
+                result, weak=weak, start_drainer=False)
+            for result in results
+        ]
+
+    async def wait_for_pending(self, result,
+                         callback=None, propagate=True, **kwargs):
+        self._ensure_not_eager()
+        await self._wait_for_pending(result, **kwargs)
+        return await result.maybe_throw(callback=callback, propagate=propagate)
+
+    async def _wait_for_pending(
+        self, result, timeout=None, on_interval=None,
+        on_message=None, **kwargs
+    ):
+        return await self.result_consumer._wait_for_pending(
+            result, timeout=timeout,
+            on_interval=on_interval, on_message=on_message,
+            **kwargs
+        )
+
+    async def _get_task_meta_for(self, task_id):
+        """Get task meta-data for a task by id."""
+        meta = await self.get(self.get_key_for_task(task_id))
+        if not meta:
+            return {'status': states.PENDING, 'result': None}
+        return self.decode_result(meta)
+
+    async def _store_result(self, task_id, result, state,
+                      traceback=None, request=None, **kwargs):
+        meta = self._get_result_meta(result=result, state=state,
+                                     traceback=traceback, request=request)
+        meta['task_id'] = bytes_to_str(task_id)
+
+        # Retrieve metadata from the backend, if the status
+        # is a success then we ignore any following update to the state.
+        # This solves a task deduplication issue because of network
+        # partitioning or lost workers. This issue involved a race condition
+        # making a lost task overwrite the last successful result in the
+        # result backend.
+        current_meta = await self._get_task_meta_for(task_id)
+
+        if current_meta['status'] == states.SUCCESS:
+            return result
+
+        await self._set_with_state(
+            self.get_key_for_task(task_id),
+            self.encode(meta), state
+        )
+        return result
+
+    async def get_task_meta(self, task_id, cache=True):
+        """Get task meta from backend.
+
+        if always_retry_backend_operation is activated, in the event of a recoverable exception,
+        then retry operation with an exponential backoff until a limit has been reached.
+        """
+        self._ensure_not_eager()
+        if cache:
+            try:
+                return self._cache[task_id]
+            except KeyError:
+                pass
+        retries = 0
+        while True:
+            try:
+                meta = await self._get_task_meta_for(task_id)
+                break
+            except Exception as exc:
+                if self.always_retry and self.exception_safe_to_retry(exc):
+                    if retries < self.max_retries:
+                        retries += 1
+
+                        # get_exponential_backoff_interval computes integers
+                        # and time.sleep accept floats for sub second sleep
+                        sleep_amount = get_exponential_backoff_interval(
+                            self.base_sleep_between_retries_ms, retries,
+                            self.max_sleep_between_retries_ms, True) / 1000
+                        await self._sleep(sleep_amount)
+                    else:
+                        raise_with_context(
+                            BackendGetMetaError("failed to get meta", task_id=task_id),
+                        )
+                else:
+                    raise
+
+        if cache and meta.get('status') == states.SUCCESS:
+            self._cache[task_id] = meta
+        return meta
+
+    async def store_result(self, task_id, result, state,
+                     traceback=None, request=None, **kwargs):
+        """Update task state and result.
+
+        if always_retry_backend_operation is activated, in the event of a recoverable exception,
+        then retry operation with an exponential backoff until a limit has been reached.
+        """
+        result = self.encode_result(result, state)
+
+        retries = 0
+
+        while True:
+            try:
+                await self._store_result(
+                    task_id, result, state, traceback,
+                    request=request, **kwargs)
+                return result
+            except Exception as exc:
+                if self.always_retry and self.exception_safe_to_retry(exc):
+                    if retries < self.max_retries:
+                        retries += 1
+
+                        # get_exponential_backoff_interval computes integers
+                        # and time.sleep accept floats for sub second sleep
+                        sleep_amount = get_exponential_backoff_interval(
+                            self.base_sleep_between_retries_ms, retries,
+                            self.max_sleep_between_retries_ms, True) / 1000
+                        await self._sleep(sleep_amount)
+                    else:
+                        raise_with_context(
+                            BackendStoreError("failed to store result on the backend", task_id=task_id, state=state),
+                        )
+                else:
+                    raise
+
+    async def _sleep(self, amount):
+        await asyncio.sleep(amount)
+
+    async def _set_with_state(self, key, value, state):
+        return await self.set(key, value)
+
+    async def _wait_for_single_future(self, result, timeout):
+        future = self._pending_future[result.id]
+        try:
+            await asyncio.wait_for(asyncio.shield(future), timeout=timeout)
+        except asyncio.TimeoutError:
+            pass
+
+    async def wait_for_future(self, result, timeout):
+        if isinstance(result, GroupResult):
+            results = result.results
+        else:
+            results = [result]
+
+        await asyncio.gather(*[
+            self._wait_for_single_future(r, timeout)
+            for r in results
+        ])
+
+    def maybe_set_future(self, task_id, result):
+        if task_id not in self._pending_future:
+            future = asyncio.get_running_loop().create_future()
+            self._pending_future[task_id] = future
+        else:
+            future: asyncio.Future = self._pending_future[task_id]
+
+        if not future.done():
+            logger.debug(f'Set result for task[{task_id}]: {result}')
+            future.set_result(result)
+
+    def remove_pending_future(self, task_id):
+        self._pending_future.pop(task_id, None)
+
+    async def restore_group(self, group_id, cache=True):
+        meta = await self.get_group_meta(group_id, cache=cache)
+        if meta:
+            return meta['result']
+
+    async def get_group_meta(self, group_id, cache=True):
+        self._ensure_not_eager()
+        if cache:
+            try:
+                return self._cache[group_id]
+            except KeyError:
+                pass
+
+        meta = await self._restore_group(group_id)
+        if cache and meta is not None:
+            self._cache[group_id] = meta
+        return meta
+
+    async def _restore_group(self, group_id):
+        """Get task meta-data for a task by id."""
+        meta = await self.get(self.get_key_for_group(group_id))
+        # previously this was always pickled, but later this
+        # was extended to support other serializers, so the
+        # structure is kind of weird.
+        if meta:
+            meta = self.decode(meta)
+            result = meta['result']
+            meta['result'] = await result_from_tuple(result, self.app)
+            return meta
+
+    async def _save_group(self, group_id, result):
+        await self._set_with_state(
+            self.get_key_for_group(group_id),
+            self.encode({'result': result.as_tuple()}),
+            states.SUCCESS
+        )
+        return result
+
+    async def iter_native(self, result, no_ack=True, **kwargs):
+        self._ensure_not_eager()
+
+        results = result.results
+        if not results:
+            raise StopIteration()
+
+        # we tell the result consumer to put consumed results
+        # into these buckets.
+        bucket = deque()
+        for node in results:
+            if not hasattr(node, '_cache'):
+                bucket.append(node)
+            elif node._cache:
+                bucket.append(node)
+            else:
+                self._collect_into(node, bucket)
+
+        await self._wait_for_pending(result, no_ack=no_ack, **kwargs)
+        while bucket:
+            node = bucket.popleft()
+            if not hasattr(node, '_cache'):
+                yield node.id, node.children
+            else:
+                yield node.id, node._cache
+
+        while bucket:
+            node = bucket.popleft()
+            yield node.id, node._cache
+
+    async def get_many(
+        self, task_ids, timeout=None, interval=0.5, no_ack=True,
+        on_message=None, on_interval=None, max_iterations=None,
+        READY_STATES=states.READY_STATES
+    ):
+        interval = 0.5 if interval is None else interval
+        ids = task_ids if isinstance(task_ids, set) else set(task_ids)
+        cached_ids = set()
+        cache = self._cache
+        for task_id in ids:
+            try:
+                cached = cache[task_id]
+            except KeyError:
+                pass
+            else:
+                if cached['status'] in READY_STATES:
+                    yield bytes_to_str(task_id), cached
+                    cached_ids.add(task_id)
+
+        ids.difference_update(cached_ids)
+        iterations = 0
+        while ids:
+            keys = list(ids)
+            r = self._mget_to_results(
+                await self.mget(
+                    [self.get_key_for_task(k)
+                     for k in keys]
+                ), keys, READY_STATES
+            )
+            cache.update(r)
+            ids.difference_update({bytes_to_str(v) for v in r})
+            for key, value in r.items():
+                if on_message is not None:
+                    on_message(value)
+                yield bytes_to_str(key), value
+            if timeout and iterations * interval >= timeout:
+                raise TimeoutError(f'Operation timed out ({timeout})')
+            if on_interval:
+                on_interval()
+            time.sleep(interval)  # don't busy loop.
+            iterations += 1
+            if max_iterations and iterations >= max_iterations:
+                break
+
+
+class SentinelBackend(RedisBackend):
+    try:
+        from aioredis import sentinel
+    except ImportError:
+        sentinel = None
+
+    if TYPE_CHECKING:
+        from aioredis.sentinel import Sentinel
+        def _get_sentinel_instance(self, **params) -> Sentinel: ...
+
+    def __init__(self, *args, **kwargs):
+        if self.sentinel is None:
+            raise ImproperlyConfigured(E_REDIS_SENTINEL_MISSING.strip())
+
+        super().__init__(*args, **kwargs)
+
+    def _params_from_url(self, url, defaults):
+        chunks = url.split(";")
+        connparams = dict(defaults, hosts=[])
+        for chunk in chunks:
+            data = super()._params_from_url(
+                url=chunk, defaults=defaults)
+            connparams['hosts'].append(data)
+        for param in ("host", "port", "db", "password"):
+            connparams.pop(param)
+
+        # Adding db/password in connparams to connect to the correct instance
+        for param in ("db", "password"):
+            if connparams['hosts'] and param in connparams['hosts'][0]:
+                connparams[param] = connparams['hosts'][0].get(param)
+        return connparams
+
+    _get_sentinel_instance = SyncSentinelBackend._get_sentinel_instance # noqa
+    _get_pool = SyncSentinelBackend._get_pool # noqa
```

### Comparing `deepfos-celery-1.0.2/celery/aio/canvas.py` & `deepfos-celery-1.0.3/celery/aio/canvas.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from celery.canvas import (
-    group as syncgroup,
-    Signature,
-    GroupResult
-)
-
-from celery.aio.common import abarrier
-
-
-@Signature.register_type()
-class group(syncgroup):
-    async def _apply_tasks(
-        self, tasks, producer=None, app=None, p=None,
-        add_to_parent=None, chord=None,
-        args=None, kwargs=None, **options
-    ):
-        # pylint: disable=redefined-outer-name
-        #   XXX chord is also a class in outer scope.
-        app = app or self.app
-        async with app.aio_producer_or_acquire(producer) as producer:
-            for sig, res in tasks:
-                await sig.apply_async(
-                    producer=producer, add_to_parent=False,
-                    chord=sig.options.get('chord') or chord,
-                    args=args, kwargs=kwargs,
-                    **options)
-
-                # adding callback to result, such that it will gradually
-                # fulfill the barrier.
-                #
-                # Using barrier.add would use result.then, but we need
-                # to add the weak argument here to only create a weak
-                # reference to the object.
-                if p and not p.cancelled and not p.ready:
-                    p.size += 1
-                    await res.then(p, weak=True)
-                yield res
-
-    async def apply_async(
-        self, args=None, kwargs=None, add_to_parent=True,
-        producer=None, link=None, link_error=None, **options
-    ):
-        args = args if args else ()
-        if link is not None:
-            raise TypeError('Cannot add link to group: use a chord')
-        if link_error is not None:
-            raise TypeError(
-                'Cannot add link to group: do that on individual tasks')
-        app = self.app
-        if app.conf.task_always_eager:
-            return self.apply(args, kwargs, **options)
-        if not self.tasks:
-            return self.freeze()
-
-        options, group_id, root_id = self._freeze_gid(options)
-        tasks = self._prepared(self.tasks, [], group_id, root_id, app)
-        p = await abarrier()
-        results = []
-        async for res in self._apply_tasks(
-            tasks, producer, app, p,
-            args=args, kwargs=kwargs, **options
-        ):
-            results.append(res)
-        result = await self.app.AioGroupResult(group_id, results, ready_barrier=p)
-        await p.finalize()
-
-        # - Special case of group(A.s() | group(B.s(), C.s()))
-        # That is, group with single item that's a chain but the
-        # last task in that chain is a group.
-        #
-        # We cannot actually support arbitrary GroupResults in chains,
-        # but this special case we can.
-        if len(result) == 1 and isinstance(result[0], GroupResult):
-            result = result[0]
-
-        parent_task = app.current_worker_task
-        if add_to_parent and parent_task:
-            parent_task.add_trail(result)
-        return result
+from celery.canvas import (
+    group as syncgroup,
+    Signature,
+    GroupResult
+)
+
+from celery.aio.common import abarrier
+
+
+@Signature.register_type()
+class group(syncgroup):
+    async def _apply_tasks(
+        self, tasks, producer=None, app=None, p=None,
+        add_to_parent=None, chord=None,
+        args=None, kwargs=None, **options
+    ):
+        # pylint: disable=redefined-outer-name
+        #   XXX chord is also a class in outer scope.
+        app = app or self.app
+        async with app.aio_producer_or_acquire(producer) as producer:
+            for sig, res in tasks:
+                await sig.apply_async(
+                    producer=producer, add_to_parent=False,
+                    chord=sig.options.get('chord') or chord,
+                    args=args, kwargs=kwargs,
+                    **options)
+
+                # adding callback to result, such that it will gradually
+                # fulfill the barrier.
+                #
+                # Using barrier.add would use result.then, but we need
+                # to add the weak argument here to only create a weak
+                # reference to the object.
+                if p and not p.cancelled and not p.ready:
+                    p.size += 1
+                    await res.then(p, weak=True)
+                yield res
+
+    async def apply_async(
+        self, args=None, kwargs=None, add_to_parent=True,
+        producer=None, link=None, link_error=None, **options
+    ):
+        args = args if args else ()
+        if link is not None:
+            raise TypeError('Cannot add link to group: use a chord')
+        if link_error is not None:
+            raise TypeError(
+                'Cannot add link to group: do that on individual tasks')
+        app = self.app
+        if app.conf.task_always_eager:
+            return self.apply(args, kwargs, **options)
+        if not self.tasks:
+            return self.freeze()
+
+        options, group_id, root_id = self._freeze_gid(options)
+        tasks = self._prepared(self.tasks, [], group_id, root_id, app)
+        p = await abarrier()
+        results = []
+        async for res in self._apply_tasks(
+            tasks, producer, app, p,
+            args=args, kwargs=kwargs, **options
+        ):
+            results.append(res)
+        result = await self.app.AioGroupResult(group_id, results, ready_barrier=p)
+        await p.finalize()
+
+        # - Special case of group(A.s() | group(B.s(), C.s()))
+        # That is, group with single item that's a chain but the
+        # last task in that chain is a group.
+        #
+        # We cannot actually support arbitrary GroupResults in chains,
+        # but this special case we can.
+        if len(result) == 1 and isinstance(result[0], GroupResult):
+            result = result[0]
+
+        parent_task = app.current_worker_task
+        if add_to_parent and parent_task:
+            parent_task.add_trail(result)
+        return result
```

### Comparing `deepfos-celery-1.0.2/celery/aio/common.py` & `deepfos-celery-1.0.3/celery/aio/common.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-from collections import deque
-
-from kombu.common import (
-    _ensure_channel_is_bound,
-    ChannelError,
-    RecoverableConnectionError,
-)
-from vine import promise, Thenable, barrier
-
-
-async def maybe_declare(entity, channel=None, retry=False, **retry_policy):
-    """Declare entity (cached)."""
-    if retry:
-        return await _imaybe_declare(entity, channel, **retry_policy)
-    return await _maybe_declare(entity, channel)
-
-
-async def _maybe_declare(entity, channel):
-    # _maybe_declare sets name on original for autogen queues
-    orig = entity
-
-    _ensure_channel_is_bound(entity, channel)
-
-    if channel is None:
-        if not entity.is_bound:
-            raise ChannelError(
-                f"channel is None and entity {entity} not bound.")
-        channel = entity.channel
-
-    declared = ident = None
-    if channel.connection and entity.can_cache_declaration:
-        declared = channel.connection.client.declared_entities
-        ident = hash(entity)
-        if ident in declared:
-            return False
-
-    if not channel.connection:
-        raise RecoverableConnectionError('channel disconnected')
-    await entity.declare(channel=channel)
-    if declared is not None and ident:
-        declared.add(ident)
-    if orig is not None:
-        orig.name = entity.name
-    return True
-
-
-async def _imaybe_declare(entity, channel, **retry_policy):
-    _ensure_channel_is_bound(entity, channel)
-
-    if not entity.channel.connection:
-        raise RecoverableConnectionError('channel disconnected')
-
-    return await entity.channel.connection.client.ensure(
-        entity, _maybe_declare, **retry_policy)(entity, channel)
-
-
-@Thenable.register
-class apromise(promise):
-    def __init__(self, fun=None, args=None, kwargs=None,
-                 callback=None, on_error=None, weak=False,
-                 ignore_result=False):
-        super().__init__(
-            fun=fun, args=args, kwargs=kwargs,
-            callback=None, on_error=on_error,
-            weak=weak, ignore_result=ignore_result
-        )
-
-        if callback is not None:
-            self._wrap_callback(callback)
-
-    async def then(self, callback, on_error=None):
-        if not isinstance(callback, Thenable):
-            callback = apromise(callback, on_error=on_error)
-        if self.cancelled:
-            callback.cancel()
-            return callback
-        if self.failed:
-            callback.throw(self.reason)
-        elif self.ready:
-            args, kwargs = self.value
-            await callback(*args, **kwargs)
-        return self._wrap_callback(callback)
-
-    def _wrap_callback(self, callback, on_error=None):
-        if not isinstance(callback, Thenable):
-            callback = apromise(callback, on_error=on_error)
-        if self._lvpending is None:
-            svpending = self._svpending
-            if svpending is not None:
-                self._svpending, self._lvpending = None, deque([svpending])
-            else:
-                self._svpending = callback
-                return callback
-        self._lvpending.append(callback)
-        return callback
-
-    async def __call__(self, *args, **kwargs):
-        retval = None
-        if self.cancelled:
-            return
-        final_args = self.args + args if args else self.args
-        final_kwargs = dict(self.kwargs, **kwargs) if kwargs else self.kwargs
-        # self.fun may be a weakref
-        fun = self._fun_is_alive(self.fun)
-        if fun is not None:
-            try:
-                if self.ignore_result:
-                    await fun(*final_args, **final_kwargs)
-                    ca = ()
-                    ck = {}
-                else:
-                    retval = await fun(*final_args, **final_kwargs)
-                    self.value = (ca, ck) = (retval,), {}
-            except Exception:
-                return self.throw()
-        else:
-            self.value = (ca, ck) = final_args, final_kwargs
-        self.ready = True
-        svpending = self._svpending
-        if svpending is not None:
-            try:
-                await svpending(*ca, **ck)
-            finally:
-                self._svpending = None
-        else:
-            lvpending = self._lvpending
-            try:
-                while lvpending:
-                    p = lvpending.popleft()
-                    await p(*ca, **ck)
-            finally:
-                self._lvpending = None
-        return retval
-
-
-@Thenable.register
-class abarrier(barrier):
-    def __init__(self, promises=None, args=None, kwargs=None,
-                 callback=None, size=None):
-        self.p = apromise()
-        self.args = args or ()
-        self.kwargs = kwargs or {}
-        self._value = 0
-        self.size = size or 0
-        if not self.size and promises:
-            # iter(l) calls len(l) so generator wrappers
-            # can only return NotImplemented in the case the
-            # generator is not fully consumed yet.
-            plen = promises.__len__()
-            if plen is not NotImplemented:
-                self.size = plen
-        self.ready = self.failed = False
-        self.reason = None
-        self.cancelled = False
-        self.finalized = False
-
-        self._promises = promises
-        self._callback = callback
-        self.finalized = False
-
-    async def _init_cb_and_promises(self):
-        promises = self._promises
-        [await self.add_noincr(p) for p in promises or []]
-        self.finalized = bool(promises or self.size)
-        if self._callback:
-            await self.then(self._callback)
-        return self
-
-    def __await__(self):
-        return self._init_cb_and_promises().__await__()
-
-    async def __call__(self, *args, **kwargs):
-        if not self.ready and not self.cancelled:
-            self._value += 1
-            if self.finalized and self._value >= self.size:
-                self.ready = True
-                await self.p(*self.args, **self.kwargs)
-
-    async def then(self, callback, errback=None):
-        await self.p.then(callback, errback)
-
-    async def finalize(self):
-        if not self.finalized and self._value >= self.size:
-            await self.p(*self.args, **self.kwargs)
-        self.finalized = True
-
-    async def add_noincr(self, p):
-        if not self.cancelled:
-            if self.ready:
-                raise ValueError('Cannot add promise to full barrier')
-            await p.then(self)
-
-    async def add(self, p):
-        if not self.cancelled:
-            await self.add_noincr(p)
-            self.size += 1
+from collections import deque
+
+from kombu.common import (
+    _ensure_channel_is_bound,
+    ChannelError,
+    RecoverableConnectionError,
+)
+from vine import promise, Thenable, barrier
+
+
+async def maybe_declare(entity, channel=None, retry=False, **retry_policy):
+    """Declare entity (cached)."""
+    if retry:
+        return await _imaybe_declare(entity, channel, **retry_policy)
+    return await _maybe_declare(entity, channel)
+
+
+async def _maybe_declare(entity, channel):
+    # _maybe_declare sets name on original for autogen queues
+    orig = entity
+
+    _ensure_channel_is_bound(entity, channel)
+
+    if channel is None:
+        if not entity.is_bound:
+            raise ChannelError(
+                f"channel is None and entity {entity} not bound.")
+        channel = entity.channel
+
+    declared = ident = None
+    if channel.connection and entity.can_cache_declaration:
+        declared = channel.connection.client.declared_entities
+        ident = hash(entity)
+        if ident in declared:
+            return False
+
+    if not channel.connection:
+        raise RecoverableConnectionError('channel disconnected')
+    await entity.declare(channel=channel)
+    if declared is not None and ident:
+        declared.add(ident)
+    if orig is not None:
+        orig.name = entity.name
+    return True
+
+
+async def _imaybe_declare(entity, channel, **retry_policy):
+    _ensure_channel_is_bound(entity, channel)
+
+    if not entity.channel.connection:
+        raise RecoverableConnectionError('channel disconnected')
+
+    return await entity.channel.connection.client.ensure(
+        entity, _maybe_declare, **retry_policy)(entity, channel)
+
+
+@Thenable.register
+class apromise(promise):
+    def __init__(self, fun=None, args=None, kwargs=None,
+                 callback=None, on_error=None, weak=False,
+                 ignore_result=False):
+        super().__init__(
+            fun=fun, args=args, kwargs=kwargs,
+            callback=None, on_error=on_error,
+            weak=weak, ignore_result=ignore_result
+        )
+
+        if callback is not None:
+            self._wrap_callback(callback)
+
+    async def then(self, callback, on_error=None):
+        if not isinstance(callback, Thenable):
+            callback = apromise(callback, on_error=on_error)
+        if self.cancelled:
+            callback.cancel()
+            return callback
+        if self.failed:
+            callback.throw(self.reason)
+        elif self.ready:
+            args, kwargs = self.value
+            await callback(*args, **kwargs)
+        return self._wrap_callback(callback)
+
+    def _wrap_callback(self, callback, on_error=None):
+        if not isinstance(callback, Thenable):
+            callback = apromise(callback, on_error=on_error)
+        if self._lvpending is None:
+            svpending = self._svpending
+            if svpending is not None:
+                self._svpending, self._lvpending = None, deque([svpending])
+            else:
+                self._svpending = callback
+                return callback
+        self._lvpending.append(callback)
+        return callback
+
+    async def __call__(self, *args, **kwargs):
+        retval = None
+        if self.cancelled:
+            return
+        final_args = self.args + args if args else self.args
+        final_kwargs = dict(self.kwargs, **kwargs) if kwargs else self.kwargs
+        # self.fun may be a weakref
+        fun = self._fun_is_alive(self.fun)
+        if fun is not None:
+            try:
+                if self.ignore_result:
+                    await fun(*final_args, **final_kwargs)
+                    ca = ()
+                    ck = {}
+                else:
+                    retval = await fun(*final_args, **final_kwargs)
+                    self.value = (ca, ck) = (retval,), {}
+            except Exception:
+                return self.throw()
+        else:
+            self.value = (ca, ck) = final_args, final_kwargs
+        self.ready = True
+        svpending = self._svpending
+        if svpending is not None:
+            try:
+                await svpending(*ca, **ck)
+            finally:
+                self._svpending = None
+        else:
+            lvpending = self._lvpending
+            try:
+                while lvpending:
+                    p = lvpending.popleft()
+                    await p(*ca, **ck)
+            finally:
+                self._lvpending = None
+        return retval
+
+
+@Thenable.register
+class abarrier(barrier):
+    def __init__(self, promises=None, args=None, kwargs=None,
+                 callback=None, size=None):
+        self.p = apromise()
+        self.args = args or ()
+        self.kwargs = kwargs or {}
+        self._value = 0
+        self.size = size or 0
+        if not self.size and promises:
+            # iter(l) calls len(l) so generator wrappers
+            # can only return NotImplemented in the case the
+            # generator is not fully consumed yet.
+            plen = promises.__len__()
+            if plen is not NotImplemented:
+                self.size = plen
+        self.ready = self.failed = False
+        self.reason = None
+        self.cancelled = False
+        self.finalized = False
+
+        self._promises = promises
+        self._callback = callback
+        self.finalized = False
+
+    async def _init_cb_and_promises(self):
+        promises = self._promises
+        [await self.add_noincr(p) for p in promises or []]
+        self.finalized = bool(promises or self.size)
+        if self._callback:
+            await self.then(self._callback)
+        return self
+
+    def __await__(self):
+        return self._init_cb_and_promises().__await__()
+
+    async def __call__(self, *args, **kwargs):
+        if not self.ready and not self.cancelled:
+            self._value += 1
+            if self.finalized and self._value >= self.size:
+                self.ready = True
+                await self.p(*self.args, **self.kwargs)
+
+    async def then(self, callback, errback=None):
+        await self.p.then(callback, errback)
+
+    async def finalize(self):
+        if not self.finalized and self._value >= self.size:
+            await self.p(*self.args, **self.kwargs)
+        self.finalized = True
+
+    async def add_noincr(self, p):
+        if not self.cancelled:
+            if self.ready:
+                raise ValueError('Cannot add promise to full barrier')
+            await p.then(self)
+
+    async def add(self, p):
+        if not self.cancelled:
+            await self.add_noincr(p)
+            self.size += 1
```

### Comparing `deepfos-celery-1.0.2/celery/aio/connection.py` & `deepfos-celery-1.0.3/celery/aio/connection.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,327 +1,327 @@
-import asyncio
-import os
-import socket
-from contextlib import asynccontextmanager
-from itertools import count
-
-from kombu.connection import (
-    Connection as SyncConnection,
-    exceptions,
-)
-from kombu.utils.collections import HashedSeq
-from kombu.utils.functional import lazy
-
-from celery.aio.utils import retry_over_time, Resource
-
-_log_channel = os.environ.get('KOMBU_LOG_CHANNEL', False)
-
-
-class Connection(SyncConnection):
-    def register_with_event_loop(self, loop):
-        return NotImplemented
-
-    def get_transport_cls(self):
-        if self.transport_cls == 'sentinel':
-            from celery.aio.redis import SentinelTransport
-            return SentinelTransport
-        else:
-            from celery.aio.redis import Transport
-            return Transport
-
-    async def connect(self):
-        return await self._ensure_connection(
-            max_retries=1, reraise_as_library_errors=False
-        )
-
-    def ensure(self, obj, fun, errback=None, max_retries=None,
-               interval_start=1, interval_step=1, interval_max=1,
-               on_revive=None):
-        """Ensure operation completes.
-
-        Regardless of any channel/connection errors occurring.
-
-        Retries by establishing the connection, and reapplying
-        the function.
-
-        Arguments:
-            obj: The object to ensure an action on.
-            fun (Callable): Method to apply.
-
-            errback (Callable): Optional callback called each time the
-                connection can't be established.  Arguments provided are
-                the exception raised and the interval that will
-                be slept ``(exc, interval)``.
-
-            max_retries (int): Maximum number of times to retry.
-                If this limit is exceeded the connection error
-                will be re-raised.
-
-            interval_start (float): The number of seconds we start
-                sleeping for.
-            interval_step (float): How many seconds added to the interval
-                for each retry.
-            interval_max (float): Maximum number of seconds to sleep between
-                each retry.
-            on_revive (Callable): Optional callback called whenever
-                revival completes successfully
-
-        Examples:
-            >>> from kombu import Connection, Producer
-            >>> conn = Connection('amqp://')
-            >>> producer = Producer(conn)
-
-            >>> def errback(exc, interval):
-            ...     logger.error('Error: %r', exc, exc_info=1)
-            ...     logger.info('Retry in %s seconds.', interval)
-
-            >>> publish = conn.ensure(producer, producer.publish,
-            ...                       errback=errback, max_retries=3)
-            >>> publish({'hello': 'world'}, routing_key='dest')
-        """
-
-        async def _ensured(*args, **kwargs):
-            got_connection = 0
-            conn_errors = self.recoverable_connection_errors
-            chan_errors = self.recoverable_channel_errors
-            has_modern_errors = hasattr(
-                self.transport, 'recoverable_connection_errors',
-            )
-            with self._reraise_as_library_errors():
-                for retries in count(0):  # for infinity
-                    try:
-                        return await fun(*args, **kwargs)
-                    except conn_errors as exc:
-                        if got_connection and not has_modern_errors:
-                            # transport can not distinguish between
-                            # recoverable/irrecoverable errors, so we propagate
-                            # the error if it persists after a new connection
-                            # was successfully established.
-                            raise
-                        if max_retries is not None and retries >= max_retries:
-                            raise
-                        self._debug(
-                            'ensure connection error: %r',
-                            exc, exc_info=1
-                        )
-                        await self.collect()
-                        errback and errback(exc, 0)
-                        remaining_retries = None
-                        if max_retries is not None:
-                            remaining_retries = max(max_retries - retries, 1)
-                        await self._ensure_connection(
-                            errback,
-                            remaining_retries,
-                            interval_start, interval_step, interval_max,
-                            reraise_as_library_errors=False,
-                        )
-                        channel = await self.default_channel()
-                        obj.revive(channel)
-                        if on_revive:
-                            on_revive(channel)
-                        got_connection += 1
-                    except chan_errors as exc:
-                        if max_retries is not None and retries > max_retries:
-                            raise
-                        self._debug(
-                            'ensure channel error: %r',
-                            exc, exc_info=1
-                        )
-                        errback and errback(exc, 0)
-
-        _ensured.__name__ = f'{fun.__name__}(ensured)'
-        _ensured.__doc__ = fun.__doc__
-        _ensured.__module__ = fun.__module__
-        return _ensured
-
-    async def _ensure_connection(
-        self, errback=None, max_retries=None,
-        interval_start=2, interval_step=2, interval_max=30,
-        callback=None, reraise_as_library_errors=True,
-        timeout=None
-    ):
-        """Ensure we have a connection to the server.
-
-        If not retry establishing the connection with the settings
-        specified.
-
-        Arguments:
-            errback (Callable): Optional callback called each time the
-                connection can't be established.  Arguments provided are
-                the exception raised and the interval that will be
-                slept ``(exc, interval)``.
-
-            max_retries (int): Maximum number of times to retry.
-                If this limit is exceeded the connection error
-                will be re-raised.
-
-            interval_start (float): The number of seconds we start
-                sleeping for.
-            interval_step (float): How many seconds added to the interval
-                for each retry.
-            interval_max (float): Maximum number of seconds to sleep between
-                each retry.
-            callback (Callable): Optional callback that is called for every
-                internal iteration (1 s).
-            timeout (int): Maximum amount of time in seconds to spend
-                waiting for connection
-        """
-        if self.connected:
-            return self._connection
-
-        def on_error(exc, intervals, retries, interval=0):
-            round = self.completes_cycle(retries)
-            if round:
-                interval = next(intervals)
-            if errback:
-                errback(exc, interval)
-            self.maybe_switch_next()  # select next host
-
-            return interval if round else 0
-
-        ctx = self._reraise_as_library_errors
-        if not reraise_as_library_errors:
-            ctx = self._dummy_context
-        with ctx():
-            return await retry_over_time(
-                self._connection_factory, self.recoverable_connection_errors,
-                (), {}, on_error, max_retries,
-                interval_start, interval_step, interval_max,
-                callback, timeout=timeout
-            )
-
-    async def _connection_factory(self):
-        self.declared_entities.clear()
-        self._default_channel = None
-        self._connection = await self._establish_connection()
-        self._closed = False
-        return self._connection
-
-    async def _establish_connection(self):
-        self._debug('establishing connection...')
-        conn = await self.transport.establish_connection()
-        self._debug('connection established: %r', self)
-        return conn
-
-    async def maybe_close_channel(self, channel):
-        """Close given channel, but ignore connection and channel errors."""
-        try:
-            await channel.close()
-        except (self.connection_errors + self.channel_errors):
-            pass
-
-    async def _do_close_self(self):
-        # Close only connection and channel(s), but not transport.
-        self.declared_entities.clear()
-        if self._default_channel:
-            await self.maybe_close_channel(self._default_channel)
-        if self._connection:
-            try:
-                await self.transport.close_connection(self._connection)
-            except self.connection_errors + (AttributeError, socket.error):
-                pass
-            self._connection = None
-
-    async def default_channel(self):
-        """Default channel.
-
-        Created upon access and closed when the connection is closed.
-
-        Note:
-            Can be used for automatic channel handling when you only need one
-            channel, and also it is the channel implicitly used if
-            a connection is passed instead of a channel, to functions that
-            require a channel.
-        """
-        # make sure we're still connected, and if not refresh.
-        conn_opts = self._extract_failover_opts()
-        await self._ensure_connection(**conn_opts)
-
-        if self._default_channel is None:
-            self._default_channel = self.channel()
-        return self._default_channel
-
-    async def _close(self):
-        """Really close connection, even if part of a connection pool."""
-        await self._do_close_self()
-        self._do_close_transport()
-        self._debug('closed')
-        self._closed = True
-
-    async def collect(self, socket_timeout=None):
-        # amqp requires communication to close, we don't need that just
-        # to clear out references, Transport._collect can also be implemented
-        # by other transports that want fast after fork
-        try:
-            gc_transport = self._transport._collect
-        except AttributeError:
-            _timeo = socket.getdefaulttimeout()
-            socket.setdefaulttimeout(socket_timeout)
-            try:
-                await self._do_close_self()
-            except socket.timeout:
-                pass
-            finally:
-                socket.setdefaulttimeout(_timeo)
-        else:
-            gc_transport(self._connection)
-
-        self._do_close_transport()
-        self.declared_entities.clear()
-        self._connection = None
-
-    def __eqhash__(self):
-        return HashedSeq('aio' + self.transport_cls, self.hostname, self.userid,
-                         self.password, self.virtual_host, self.port,
-                         repr(self.transport_options))
-
-    def Pool(self, limit=None, **kwargs):
-        return ConnectionPool(self, limit, **kwargs)
-
-    async def release(self):
-        """Close the connection (if open)."""
-        await self._close()
-
-    close = release
-
-    async def drain_events(self, **kwargs):
-        return await self.transport.drain_events(self.connection, **kwargs)
-
-
-class ConnectionPool(Resource):
-    """Pool of connections."""
-    LimitExceeded = exceptions.ConnectionLimitExceeded
-    close_after_fork = True
-
-    def __init__(self, connection: Connection, limit=None, **kwargs):
-        self.connection = connection
-        super().__init__(limit=limit)
-
-    def new(self):
-        return self.connection.clone()
-
-    async def release_resource(self, resource: Connection):
-        try:
-            resource._debug('released')
-        except AttributeError:
-            pass
-
-    async def close_resource(self, resource: Connection):
-        await resource._close()
-
-    @asynccontextmanager
-    async def acquire_channel(self, block=False):
-        connection: Connection
-        async with self.acquire(block=block) as connection:
-            yield connection, await connection.default_channel()
-
-    def setup(self):
-        if self.limit:
-            q = self._resource.queue
-            while len(q) < self.limit:
-                self._resource.put_nowait(lazy(self.new))
-
-    async def prepare(self, resource):
-        if callable(resource):
-            resource = resource()
-        resource._debug('acquired')
-        return resource
+import asyncio
+import os
+import socket
+from contextlib import asynccontextmanager
+from itertools import count
+
+from kombu.connection import (
+    Connection as SyncConnection,
+    exceptions,
+)
+from kombu.utils.collections import HashedSeq
+from kombu.utils.functional import lazy
+
+from celery.aio.utils import retry_over_time, Resource
+
+_log_channel = os.environ.get('KOMBU_LOG_CHANNEL', False)
+
+
+class Connection(SyncConnection):
+    def register_with_event_loop(self, loop):
+        return NotImplemented
+
+    def get_transport_cls(self):
+        if self.transport_cls == 'sentinel':
+            from celery.aio.redis import SentinelTransport
+            return SentinelTransport
+        else:
+            from celery.aio.redis import Transport
+            return Transport
+
+    async def connect(self):
+        return await self._ensure_connection(
+            max_retries=1, reraise_as_library_errors=False
+        )
+
+    def ensure(self, obj, fun, errback=None, max_retries=None,
+               interval_start=1, interval_step=1, interval_max=1,
+               on_revive=None):
+        """Ensure operation completes.
+
+        Regardless of any channel/connection errors occurring.
+
+        Retries by establishing the connection, and reapplying
+        the function.
+
+        Arguments:
+            obj: The object to ensure an action on.
+            fun (Callable): Method to apply.
+
+            errback (Callable): Optional callback called each time the
+                connection can't be established.  Arguments provided are
+                the exception raised and the interval that will
+                be slept ``(exc, interval)``.
+
+            max_retries (int): Maximum number of times to retry.
+                If this limit is exceeded the connection error
+                will be re-raised.
+
+            interval_start (float): The number of seconds we start
+                sleeping for.
+            interval_step (float): How many seconds added to the interval
+                for each retry.
+            interval_max (float): Maximum number of seconds to sleep between
+                each retry.
+            on_revive (Callable): Optional callback called whenever
+                revival completes successfully
+
+        Examples:
+            >>> from kombu import Connection, Producer
+            >>> conn = Connection('amqp://')
+            >>> producer = Producer(conn)
+
+            >>> def errback(exc, interval):
+            ...     logger.error('Error: %r', exc, exc_info=1)
+            ...     logger.info('Retry in %s seconds.', interval)
+
+            >>> publish = conn.ensure(producer, producer.publish,
+            ...                       errback=errback, max_retries=3)
+            >>> publish({'hello': 'world'}, routing_key='dest')
+        """
+
+        async def _ensured(*args, **kwargs):
+            got_connection = 0
+            conn_errors = self.recoverable_connection_errors
+            chan_errors = self.recoverable_channel_errors
+            has_modern_errors = hasattr(
+                self.transport, 'recoverable_connection_errors',
+            )
+            with self._reraise_as_library_errors():
+                for retries in count(0):  # for infinity
+                    try:
+                        return await fun(*args, **kwargs)
+                    except conn_errors as exc:
+                        if got_connection and not has_modern_errors:
+                            # transport can not distinguish between
+                            # recoverable/irrecoverable errors, so we propagate
+                            # the error if it persists after a new connection
+                            # was successfully established.
+                            raise
+                        if max_retries is not None and retries >= max_retries:
+                            raise
+                        self._debug(
+                            'ensure connection error: %r',
+                            exc, exc_info=1
+                        )
+                        await self.collect()
+                        errback and errback(exc, 0)
+                        remaining_retries = None
+                        if max_retries is not None:
+                            remaining_retries = max(max_retries - retries, 1)
+                        await self._ensure_connection(
+                            errback,
+                            remaining_retries,
+                            interval_start, interval_step, interval_max,
+                            reraise_as_library_errors=False,
+                        )
+                        channel = await self.default_channel()
+                        obj.revive(channel)
+                        if on_revive:
+                            on_revive(channel)
+                        got_connection += 1
+                    except chan_errors as exc:
+                        if max_retries is not None and retries > max_retries:
+                            raise
+                        self._debug(
+                            'ensure channel error: %r',
+                            exc, exc_info=1
+                        )
+                        errback and errback(exc, 0)
+
+        _ensured.__name__ = f'{fun.__name__}(ensured)'
+        _ensured.__doc__ = fun.__doc__
+        _ensured.__module__ = fun.__module__
+        return _ensured
+
+    async def _ensure_connection(
+        self, errback=None, max_retries=None,
+        interval_start=2, interval_step=2, interval_max=30,
+        callback=None, reraise_as_library_errors=True,
+        timeout=None
+    ):
+        """Ensure we have a connection to the server.
+
+        If not retry establishing the connection with the settings
+        specified.
+
+        Arguments:
+            errback (Callable): Optional callback called each time the
+                connection can't be established.  Arguments provided are
+                the exception raised and the interval that will be
+                slept ``(exc, interval)``.
+
+            max_retries (int): Maximum number of times to retry.
+                If this limit is exceeded the connection error
+                will be re-raised.
+
+            interval_start (float): The number of seconds we start
+                sleeping for.
+            interval_step (float): How many seconds added to the interval
+                for each retry.
+            interval_max (float): Maximum number of seconds to sleep between
+                each retry.
+            callback (Callable): Optional callback that is called for every
+                internal iteration (1 s).
+            timeout (int): Maximum amount of time in seconds to spend
+                waiting for connection
+        """
+        if self.connected:
+            return self._connection
+
+        def on_error(exc, intervals, retries, interval=0):
+            round = self.completes_cycle(retries)
+            if round:
+                interval = next(intervals)
+            if errback:
+                errback(exc, interval)
+            self.maybe_switch_next()  # select next host
+
+            return interval if round else 0
+
+        ctx = self._reraise_as_library_errors
+        if not reraise_as_library_errors:
+            ctx = self._dummy_context
+        with ctx():
+            return await retry_over_time(
+                self._connection_factory, self.recoverable_connection_errors,
+                (), {}, on_error, max_retries,
+                interval_start, interval_step, interval_max,
+                callback, timeout=timeout
+            )
+
+    async def _connection_factory(self):
+        self.declared_entities.clear()
+        self._default_channel = None
+        self._connection = await self._establish_connection()
+        self._closed = False
+        return self._connection
+
+    async def _establish_connection(self):
+        self._debug('establishing connection...')
+        conn = await self.transport.establish_connection()
+        self._debug('connection established: %r', self)
+        return conn
+
+    async def maybe_close_channel(self, channel):
+        """Close given channel, but ignore connection and channel errors."""
+        try:
+            await channel.close()
+        except (self.connection_errors + self.channel_errors):
+            pass
+
+    async def _do_close_self(self):
+        # Close only connection and channel(s), but not transport.
+        self.declared_entities.clear()
+        if self._default_channel:
+            await self.maybe_close_channel(self._default_channel)
+        if self._connection:
+            try:
+                await self.transport.close_connection(self._connection)
+            except self.connection_errors + (AttributeError, socket.error):
+                pass
+            self._connection = None
+
+    async def default_channel(self):
+        """Default channel.
+
+        Created upon access and closed when the connection is closed.
+
+        Note:
+            Can be used for automatic channel handling when you only need one
+            channel, and also it is the channel implicitly used if
+            a connection is passed instead of a channel, to functions that
+            require a channel.
+        """
+        # make sure we're still connected, and if not refresh.
+        conn_opts = self._extract_failover_opts()
+        await self._ensure_connection(**conn_opts)
+
+        if self._default_channel is None:
+            self._default_channel = self.channel()
+        return self._default_channel
+
+    async def _close(self):
+        """Really close connection, even if part of a connection pool."""
+        await self._do_close_self()
+        self._do_close_transport()
+        self._debug('closed')
+        self._closed = True
+
+    async def collect(self, socket_timeout=None):
+        # amqp requires communication to close, we don't need that just
+        # to clear out references, Transport._collect can also be implemented
+        # by other transports that want fast after fork
+        try:
+            gc_transport = self._transport._collect
+        except AttributeError:
+            _timeo = socket.getdefaulttimeout()
+            socket.setdefaulttimeout(socket_timeout)
+            try:
+                await self._do_close_self()
+            except socket.timeout:
+                pass
+            finally:
+                socket.setdefaulttimeout(_timeo)
+        else:
+            gc_transport(self._connection)
+
+        self._do_close_transport()
+        self.declared_entities.clear()
+        self._connection = None
+
+    def __eqhash__(self):
+        return HashedSeq('aio' + self.transport_cls, self.hostname, self.userid,
+                         self.password, self.virtual_host, self.port,
+                         repr(self.transport_options))
+
+    def Pool(self, limit=None, **kwargs):
+        return ConnectionPool(self, limit, **kwargs)
+
+    async def release(self):
+        """Close the connection (if open)."""
+        await self._close()
+
+    close = release
+
+    async def drain_events(self, **kwargs):
+        return await self.transport.drain_events(self.connection, **kwargs)
+
+
+class ConnectionPool(Resource):
+    """Pool of connections."""
+    LimitExceeded = exceptions.ConnectionLimitExceeded
+    close_after_fork = True
+
+    def __init__(self, connection: Connection, limit=None, **kwargs):
+        self.connection = connection
+        super().__init__(limit=limit)
+
+    def new(self):
+        return self.connection.clone()
+
+    async def release_resource(self, resource: Connection):
+        try:
+            resource._debug('released')
+        except AttributeError:
+            pass
+
+    async def close_resource(self, resource: Connection):
+        await resource._close()
+
+    @asynccontextmanager
+    async def acquire_channel(self, block=False):
+        connection: Connection
+        async with self.acquire(block=block) as connection:
+            yield connection, await connection.default_channel()
+
+    def setup(self):
+        if self.limit:
+            q = self._resource.queue
+            while len(q) < self.limit:
+                self._resource.put_nowait(lazy(self.new))
+
+    async def prepare(self, resource):
+        if callable(resource):
+            resource = resource()
+        resource._debug('acquired')
+        return resource
```

### Comparing `deepfos-celery-1.0.2/celery/aio/dispatcher.py` & `deepfos-celery-1.0.3/celery/aio/dispatcher.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import asyncio
-import os
-import time
-
-from collections import deque, defaultdict
-
-from celery.events.dispatcher import (
-    EventDispatcher as SyncEventDispatcher,
-    Event,
-    app_or_default,
-    anon_nodename,
-    utcoffset,
-    group_from,
-)
-from celery.aio.messaging import Producer
-from celery.aio.exchange import get_exchange
-
-
-class EventDispatcher(SyncEventDispatcher):
-    def __init__(self, connection=None, hostname=None, enabled=True,
-                 channel=None, buffer_while_offline=True, app=None,
-                 serializer=None, groups=None, delivery_mode=1,
-                 buffer_group=None, buffer_limit=24, on_send_buffered=None):
-        self.app = app_or_default(app or self.app)
-        self.connection = connection
-        self.channel = channel
-        self.hostname = hostname or anon_nodename()
-        self.buffer_while_offline = buffer_while_offline
-        self.buffer_group = buffer_group or frozenset()
-        self.buffer_limit = buffer_limit
-        self.on_send_buffered = on_send_buffered
-        self._group_buffer = defaultdict(list)
-        self.mutex = asyncio.Lock()
-        self.producer = None
-        self._outbound_buffer = deque()
-        self.serializer = serializer or self.app.conf.event_serializer
-        self.on_enabled = set()
-        self.on_disabled = set()
-        self.groups = set(groups or [])
-        self.tzoffset = [-time.timezone, -time.altzone]
-        self.clock = self.app.clock
-        self.delivery_mode = delivery_mode
-        if not connection and channel:
-            self.connection = channel.connection.client
-        self.enabled = enabled
-        conninfo = self.connection or self.app.aconnection_for_write()
-        self.exchange = get_exchange(conninfo,
-                                     name=self.app.conf.event_exchange)
-        if conninfo.transport.driver_type in self.DISABLED_TRANSPORTS:
-            self.enabled = False
-        if self.enabled:
-            self.enable()
-        self.headers = {'hostname': self.hostname}
-        self.pid = os.getpid()
-
-    def enable(self):
-        self.producer = Producer(self.channel or self.connection,
-                                 exchange=self.exchange,
-                                 serializer=self.serializer,
-                                 auto_declare=False)
-        self.enabled = True
-        for callback in self.on_enabled:
-            callback()
-
-    async def publish(self, type, fields, producer,
-                blind=False, Event=Event, **kwargs):
-        clock = None if blind else self.clock.forward()
-        event = Event(type, hostname=self.hostname, utcoffset=utcoffset(),
-                      pid=self.pid, clock=clock, **fields)
-        async with self.mutex:
-            return await self._publish(
-                event, producer,
-                routing_key=type.replace('-', '.'),
-                **kwargs
-            )
-
-    async def _publish(
-        self, event, producer, routing_key, retry=False,
-        retry_policy=None, utcoffset=utcoffset
-    ):
-        exchange = self.exchange
-        try:
-            await producer.publish(
-                event,
-                routing_key=routing_key,
-                exchange=exchange.name,
-                retry=retry,
-                retry_policy=retry_policy,
-                declare=[exchange],
-                serializer=self.serializer,
-                headers=self.headers,
-                delivery_mode=self.delivery_mode,
-            )
-        except Exception as exc:  # pylint: disable=broad-except
-            if not self.buffer_while_offline:
-                raise
-            self._outbound_buffer.append((event, routing_key, exc))
-
-
-    async def send(self, type, blind=False, utcoffset=utcoffset, retry=False,
-             retry_policy=None, Event=Event, **fields):
-        if self.enabled:
-            groups, group = self.groups, group_from(type)
-            if groups and group not in groups:
-                return
-            if group in self.buffer_group:
-                clock = self.clock.forward()
-                event = Event(type, hostname=self.hostname,
-                              utcoffset=utcoffset(),
-                              pid=self.pid, clock=clock, **fields)
-                buf = self._group_buffer[group]
-                buf.append(event)
-                if len(buf) >= self.buffer_limit:
-                    await self.flush()
-                elif self.on_send_buffered:
-                    self.on_send_buffered()
-            else:
-                return await self.publish(
-                    type, fields, self.producer,
-                    blind=blind, Event=Event, retry=retry,
-                    retry_policy=retry_policy)
-
-    async def flush(self, errors=True, groups=True):
-        if errors:
-            buf = list(self._outbound_buffer)
-            try:
-                async with self.mutex:
-                    for event, routing_key, _ in buf:
-                        await self._publish(event, self.producer, routing_key)
-            finally:
-                self._outbound_buffer.clear()
-        if groups:
-            async with self.mutex:
-                for group, events in self._group_buffer.items():
-                    await self._publish(
-                        events, self.producer, '%s.multi' % group)
-                    events[:] = []  # list.clear
+import asyncio
+import os
+import time
+
+from collections import deque, defaultdict
+
+from celery.events.dispatcher import (
+    EventDispatcher as SyncEventDispatcher,
+    Event,
+    app_or_default,
+    anon_nodename,
+    utcoffset,
+    group_from,
+)
+from celery.aio.messaging import Producer
+from celery.aio.exchange import get_exchange
+
+
+class EventDispatcher(SyncEventDispatcher):
+    def __init__(self, connection=None, hostname=None, enabled=True,
+                 channel=None, buffer_while_offline=True, app=None,
+                 serializer=None, groups=None, delivery_mode=1,
+                 buffer_group=None, buffer_limit=24, on_send_buffered=None):
+        self.app = app_or_default(app or self.app)
+        self.connection = connection
+        self.channel = channel
+        self.hostname = hostname or anon_nodename()
+        self.buffer_while_offline = buffer_while_offline
+        self.buffer_group = buffer_group or frozenset()
+        self.buffer_limit = buffer_limit
+        self.on_send_buffered = on_send_buffered
+        self._group_buffer = defaultdict(list)
+        self.mutex = asyncio.Lock()
+        self.producer = None
+        self._outbound_buffer = deque()
+        self.serializer = serializer or self.app.conf.event_serializer
+        self.on_enabled = set()
+        self.on_disabled = set()
+        self.groups = set(groups or [])
+        self.tzoffset = [-time.timezone, -time.altzone]
+        self.clock = self.app.clock
+        self.delivery_mode = delivery_mode
+        if not connection and channel:
+            self.connection = channel.connection.client
+        self.enabled = enabled
+        conninfo = self.connection or self.app.aconnection_for_write()
+        self.exchange = get_exchange(conninfo,
+                                     name=self.app.conf.event_exchange)
+        if conninfo.transport.driver_type in self.DISABLED_TRANSPORTS:
+            self.enabled = False
+        if self.enabled:
+            self.enable()
+        self.headers = {'hostname': self.hostname}
+        self.pid = os.getpid()
+
+    def enable(self):
+        self.producer = Producer(self.channel or self.connection,
+                                 exchange=self.exchange,
+                                 serializer=self.serializer,
+                                 auto_declare=False)
+        self.enabled = True
+        for callback in self.on_enabled:
+            callback()
+
+    async def publish(self, type, fields, producer,
+                blind=False, Event=Event, **kwargs):
+        clock = None if blind else self.clock.forward()
+        event = Event(type, hostname=self.hostname, utcoffset=utcoffset(),
+                      pid=self.pid, clock=clock, **fields)
+        async with self.mutex:
+            return await self._publish(
+                event, producer,
+                routing_key=type.replace('-', '.'),
+                **kwargs
+            )
+
+    async def _publish(
+        self, event, producer, routing_key, retry=False,
+        retry_policy=None, utcoffset=utcoffset
+    ):
+        exchange = self.exchange
+        try:
+            await producer.publish(
+                event,
+                routing_key=routing_key,
+                exchange=exchange.name,
+                retry=retry,
+                retry_policy=retry_policy,
+                declare=[exchange],
+                serializer=self.serializer,
+                headers=self.headers,
+                delivery_mode=self.delivery_mode,
+            )
+        except Exception as exc:  # pylint: disable=broad-except
+            if not self.buffer_while_offline:
+                raise
+            self._outbound_buffer.append((event, routing_key, exc))
+
+
+    async def send(self, type, blind=False, utcoffset=utcoffset, retry=False,
+             retry_policy=None, Event=Event, **fields):
+        if self.enabled:
+            groups, group = self.groups, group_from(type)
+            if groups and group not in groups:
+                return
+            if group in self.buffer_group:
+                clock = self.clock.forward()
+                event = Event(type, hostname=self.hostname,
+                              utcoffset=utcoffset(),
+                              pid=self.pid, clock=clock, **fields)
+                buf = self._group_buffer[group]
+                buf.append(event)
+                if len(buf) >= self.buffer_limit:
+                    await self.flush()
+                elif self.on_send_buffered:
+                    self.on_send_buffered()
+            else:
+                return await self.publish(
+                    type, fields, self.producer,
+                    blind=blind, Event=Event, retry=retry,
+                    retry_policy=retry_policy)
+
+    async def flush(self, errors=True, groups=True):
+        if errors:
+            buf = list(self._outbound_buffer)
+            try:
+                async with self.mutex:
+                    for event, routing_key, _ in buf:
+                        await self._publish(event, self.producer, routing_key)
+            finally:
+                self._outbound_buffer.clear()
+        if groups:
+            async with self.mutex:
+                for group, events in self._group_buffer.items():
+                    await self._publish(
+                        events, self.producer, '%s.multi' % group)
+                    events[:] = []  # list.clear
```

### Comparing `deepfos-celery-1.0.2/celery/aio/entity.py` & `deepfos-celery-1.0.3/celery/aio/entity.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from typing import *
-
-from kombu.entity import (
-    Queue as SyncQueue,
-    Exchange,
-    prepare_accept_content
-)
-from kombu.exceptions import NotBoundError
-from kombu.utils.functional import ChannelPromise
-
-
-class Queue(SyncQueue):
-    if TYPE_CHECKING:
-        binding_arguments = None
-        no_declare: bool
-
-    @property
-    def channel(self):
-        """Current channel if the object is bound."""
-        channel = self._channel
-        if channel is None:
-            raise NotBoundError(
-                "Can't call method on {} not bound to a channel".format(
-                    type(self).__name__))
-        if isinstance(channel, ChannelPromise):
-            channel = self._channel = channel()
-        return channel
-
-    async def queue_bind(self, nowait=False, channel=None):
-        return await self.bind_to(
-            self.exchange, self.routing_key, self.binding_arguments,
-            channel=channel, nowait=nowait)
-
-    async def bind_to(self, exchange='', routing_key='',
-            arguments=None, nowait=False, channel=None):
-        if isinstance(exchange, Exchange):
-            exchange = exchange.name
-
-        return await (channel or self.channel).queue_bind(
-            queue=self.name,
-            exchange=exchange,
-            routing_key=routing_key,
-            arguments=arguments,
-            nowait=nowait,
-        )
-
-    async def declare(self, nowait=False, channel=None):
-        if not self.no_declare:
-            # - declare main binding.
-            self._create_exchange(nowait=nowait, channel=channel)
-            await self._create_queue(nowait=nowait, channel=channel)
-            self._create_bindings(nowait=nowait, channel=channel)
-        return self.name
-
-    async def _create_queue(self, nowait=False, channel=None):
-        await self.queue_declare(nowait=nowait, passive=False, channel=channel)
-        if self.exchange and self.exchange.name:
-            await self.queue_bind(nowait=nowait, channel=channel)
-
-    async def get(self, no_ack=None, accept=None):
-        """Poll the server for a new message.
-
-        This method provides direct access to the messages in a
-        queue using a synchronous dialogue, designed for
-        specific types of applications where synchronous functionality
-        is more important than performance.
-
-        Returns:
-            ~kombu.Message: if a message was available,
-                or :const:`None` otherwise.
-
-        Arguments:
-            no_ack (bool): If enabled the broker will
-                automatically ack messages.
-            accept (Set[str]): Custom list of accepted content types.
-        """
-        no_ack = self.no_ack if no_ack is None else no_ack
-        message = await self.channel.basic_get(queue=self.name, no_ack=no_ack)
-        if message is not None:
-            m2p = getattr(self.channel, 'message_to_python', None)
-            if m2p:
-                message = m2p(message)
-            if message.errors:
-                message._reraise_error()
-            message.accept = prepare_accept_content(accept)
-        return message
-
-    async def queue_declare(self, nowait=False, passive=False, channel=None):
-        """Declare queue on the server.
-
-        Arguments:
-            nowait (bool): Do not wait for a reply.
-            passive (bool): If set, the server will not create the queue.
-                The client can use this to check whether a queue exists
-                without modifying the server state.
-        """
-        channel = channel or self.channel
-        queue_arguments = channel.prepare_queue_arguments(
-            self.queue_arguments or {},
-            expires=self.expires,
-            message_ttl=self.message_ttl,
-            max_length=self.max_length,
-            max_length_bytes=self.max_length_bytes,
-            max_priority=self.max_priority,
-        )
-        ret = await channel.queue_declare(
-            queue=self.name,
-            passive=passive,
-            durable=self.durable,
-            exclusive=self.exclusive,
-            auto_delete=self.auto_delete,
-            arguments=queue_arguments,
-            nowait=nowait,
-        )
-        if not self.name:
-            self.name = ret[0]
-        if self.on_declared:
-            self.on_declared(*ret)
-        return ret
+from typing import *
+
+from kombu.entity import (
+    Queue as SyncQueue,
+    Exchange,
+    prepare_accept_content
+)
+from kombu.exceptions import NotBoundError
+from kombu.utils.functional import ChannelPromise
+
+
+class Queue(SyncQueue):
+    if TYPE_CHECKING:
+        binding_arguments = None
+        no_declare: bool
+
+    @property
+    def channel(self):
+        """Current channel if the object is bound."""
+        channel = self._channel
+        if channel is None:
+            raise NotBoundError(
+                "Can't call method on {} not bound to a channel".format(
+                    type(self).__name__))
+        if isinstance(channel, ChannelPromise):
+            channel = self._channel = channel()
+        return channel
+
+    async def queue_bind(self, nowait=False, channel=None):
+        return await self.bind_to(
+            self.exchange, self.routing_key, self.binding_arguments,
+            channel=channel, nowait=nowait)
+
+    async def bind_to(self, exchange='', routing_key='',
+            arguments=None, nowait=False, channel=None):
+        if isinstance(exchange, Exchange):
+            exchange = exchange.name
+
+        return await (channel or self.channel).queue_bind(
+            queue=self.name,
+            exchange=exchange,
+            routing_key=routing_key,
+            arguments=arguments,
+            nowait=nowait,
+        )
+
+    async def declare(self, nowait=False, channel=None):
+        if not self.no_declare:
+            # - declare main binding.
+            self._create_exchange(nowait=nowait, channel=channel)
+            await self._create_queue(nowait=nowait, channel=channel)
+            self._create_bindings(nowait=nowait, channel=channel)
+        return self.name
+
+    async def _create_queue(self, nowait=False, channel=None):
+        await self.queue_declare(nowait=nowait, passive=False, channel=channel)
+        if self.exchange and self.exchange.name:
+            await self.queue_bind(nowait=nowait, channel=channel)
+
+    async def get(self, no_ack=None, accept=None):
+        """Poll the server for a new message.
+
+        This method provides direct access to the messages in a
+        queue using a synchronous dialogue, designed for
+        specific types of applications where synchronous functionality
+        is more important than performance.
+
+        Returns:
+            ~kombu.Message: if a message was available,
+                or :const:`None` otherwise.
+
+        Arguments:
+            no_ack (bool): If enabled the broker will
+                automatically ack messages.
+            accept (Set[str]): Custom list of accepted content types.
+        """
+        no_ack = self.no_ack if no_ack is None else no_ack
+        message = await self.channel.basic_get(queue=self.name, no_ack=no_ack)
+        if message is not None:
+            m2p = getattr(self.channel, 'message_to_python', None)
+            if m2p:
+                message = m2p(message)
+            if message.errors:
+                message._reraise_error()
+            message.accept = prepare_accept_content(accept)
+        return message
+
+    async def queue_declare(self, nowait=False, passive=False, channel=None):
+        """Declare queue on the server.
+
+        Arguments:
+            nowait (bool): Do not wait for a reply.
+            passive (bool): If set, the server will not create the queue.
+                The client can use this to check whether a queue exists
+                without modifying the server state.
+        """
+        channel = channel or self.channel
+        queue_arguments = channel.prepare_queue_arguments(
+            self.queue_arguments or {},
+            expires=self.expires,
+            message_ttl=self.message_ttl,
+            max_length=self.max_length,
+            max_length_bytes=self.max_length_bytes,
+            max_priority=self.max_priority,
+        )
+        ret = await channel.queue_declare(
+            queue=self.name,
+            passive=passive,
+            durable=self.durable,
+            exclusive=self.exclusive,
+            auto_delete=self.auto_delete,
+            arguments=queue_arguments,
+            nowait=nowait,
+        )
+        if not self.name:
+            self.name = ret[0]
+        if self.on_declared:
+            self.on_declared(*ret)
+        return ret
```

### Comparing `deepfos-celery-1.0.2/celery/aio/exchange.py` & `deepfos-celery-1.0.3/celery/aio/exchange.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-from typing import *
-from copy import copy
-
-from kombu.transport.virtual.exchange import (
-    ExchangeType as SyncExchangeType,
-    DirectExchange as SyncDirectExchange,
-    TopicExchange as SyncTopicExchange,
-    FanoutExchange as SyncFanoutExchange
-)
-from kombu.entity import (
-    Exchange as SyncExchange,
-)
-
-from celery.events.event import EVENT_EXCHANGE_NAME
-
-
-class ExchangeType(SyncExchangeType):
-    if TYPE_CHECKING:
-        from celery.aio.redis import Channel
-        channel: Channel
-
-    async def deliver(self, message, exchange, routing_key, **kwargs):
-        raise NotImplementedError('subclass responsibility')
-
-
-class DirectExchange(ExchangeType, SyncDirectExchange):
-    async def deliver(self, message, exchange, routing_key, **kwargs):
-        _lookup = self.channel._lookup
-        _put = self.channel._put
-        for queue in (await _lookup(exchange, routing_key)):
-            await _put(queue, message, **kwargs)
-
-
-class TopicExchange(ExchangeType, SyncTopicExchange):
-    async def deliver(self, message, exchange, routing_key, **kwargs):
-        _lookup = self.channel._lookup
-        _put = self.channel._put
-        deadletter = self.channel.deadletter_queue
-        queues = (
-            q for q in (await _lookup(exchange, routing_key))
-            if q and q != deadletter
-        )
-        for queue in queues:
-            await _put(queue, message, **kwargs)
-
-
-class FanoutExchange(ExchangeType, SyncFanoutExchange):
-    async def deliver(self, message, exchange, routing_key, **kwargs):
-        if self.channel.supports_fanout:
-            await self.channel._put_fanout(
-                exchange, message, routing_key, **kwargs)
-
-
-STANDARD_EXCHANGE_TYPES = {
-    'direct': DirectExchange,
-    'topic': TopicExchange,
-    'fanout': FanoutExchange,
-}
-
-
-class Exchange(SyncExchange):
-    if TYPE_CHECKING:
-        from celery.aio.redis import Channel
-        @property
-        def channel(self) -> Channel: ...
-
-    async def declare(self, nowait=False, passive=None, channel=None):
-        return super().declare(nowait, passive, channel)
-
-    async def publish(self, message, routing_key=None, mandatory=False,
-                immediate=False, exchange=None):
-        if isinstance(message, str):
-            message = self.Message(message)
-        exchange = exchange or self.name
-        return await self.channel.basic_publish(
-            message,
-            exchange=exchange,
-            routing_key=routing_key,
-            mandatory=mandatory,
-            immediate=immediate,
-        )
-
-    async def delete(self, if_unused=False, nowait=False):
-        return await self.channel.exchange_delete(
-            exchange=self.name, if_unused=if_unused, nowait=nowait)
-
-
-event_exchange = Exchange(EVENT_EXCHANGE_NAME, type='topic')
-
-
-def get_exchange(conn, name=EVENT_EXCHANGE_NAME):
-    """Get exchange used for sending events.
-
-    Arguments:
-        conn (kombu.Connection): Connection used for sending/receiving events.
-        name (str): Name of the exchange. Default is ``celeryev``.
-
-    Note:
-        The event type changes if Redis is used as the transport
-        (from topic -> fanout).
-    """
-    ex = copy(event_exchange)
-    if conn.transport.driver_type == 'redis':
-        # quick hack for Issue #436
-        ex.type = 'fanout'
-    if name != ex.name:
-        ex.name = name
-    return ex
+from typing import *
+from copy import copy
+
+from kombu.transport.virtual.exchange import (
+    ExchangeType as SyncExchangeType,
+    DirectExchange as SyncDirectExchange,
+    TopicExchange as SyncTopicExchange,
+    FanoutExchange as SyncFanoutExchange
+)
+from kombu.entity import (
+    Exchange as SyncExchange,
+)
+
+from celery.events.event import EVENT_EXCHANGE_NAME
+
+
+class ExchangeType(SyncExchangeType):
+    if TYPE_CHECKING:
+        from celery.aio.redis import Channel
+        channel: Channel
+
+    async def deliver(self, message, exchange, routing_key, **kwargs):
+        raise NotImplementedError('subclass responsibility')
+
+
+class DirectExchange(ExchangeType, SyncDirectExchange):
+    async def deliver(self, message, exchange, routing_key, **kwargs):
+        _lookup = self.channel._lookup
+        _put = self.channel._put
+        for queue in (await _lookup(exchange, routing_key)):
+            await _put(queue, message, **kwargs)
+
+
+class TopicExchange(ExchangeType, SyncTopicExchange):
+    async def deliver(self, message, exchange, routing_key, **kwargs):
+        _lookup = self.channel._lookup
+        _put = self.channel._put
+        deadletter = self.channel.deadletter_queue
+        queues = (
+            q for q in (await _lookup(exchange, routing_key))
+            if q and q != deadletter
+        )
+        for queue in queues:
+            await _put(queue, message, **kwargs)
+
+
+class FanoutExchange(ExchangeType, SyncFanoutExchange):
+    async def deliver(self, message, exchange, routing_key, **kwargs):
+        if self.channel.supports_fanout:
+            await self.channel._put_fanout(
+                exchange, message, routing_key, **kwargs)
+
+
+STANDARD_EXCHANGE_TYPES = {
+    'direct': DirectExchange,
+    'topic': TopicExchange,
+    'fanout': FanoutExchange,
+}
+
+
+class Exchange(SyncExchange):
+    if TYPE_CHECKING:
+        from celery.aio.redis import Channel
+        @property
+        def channel(self) -> Channel: ...
+
+    async def declare(self, nowait=False, passive=None, channel=None):
+        return super().declare(nowait, passive, channel)
+
+    async def publish(self, message, routing_key=None, mandatory=False,
+                immediate=False, exchange=None):
+        if isinstance(message, str):
+            message = self.Message(message)
+        exchange = exchange or self.name
+        return await self.channel.basic_publish(
+            message,
+            exchange=exchange,
+            routing_key=routing_key,
+            mandatory=mandatory,
+            immediate=immediate,
+        )
+
+    async def delete(self, if_unused=False, nowait=False):
+        return await self.channel.exchange_delete(
+            exchange=self.name, if_unused=if_unused, nowait=nowait)
+
+
+event_exchange = Exchange(EVENT_EXCHANGE_NAME, type='topic')
+
+
+def get_exchange(conn, name=EVENT_EXCHANGE_NAME):
+    """Get exchange used for sending events.
+
+    Arguments:
+        conn (kombu.Connection): Connection used for sending/receiving events.
+        name (str): Name of the exchange. Default is ``celeryev``.
+
+    Note:
+        The event type changes if Redis is used as the transport
+        (from topic -> fanout).
+    """
+    ex = copy(event_exchange)
+    if conn.transport.driver_type == 'redis':
+        # quick hack for Issue #436
+        ex.type = 'fanout'
+    if name != ex.name:
+        ex.name = name
+    return ex
```

### Comparing `deepfos-celery-1.0.2/celery/aio/messaging.py` & `deepfos-celery-1.0.3/celery/aio/messaging.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-import asyncio
-
-from typing import TYPE_CHECKING, Dict, List
-
-from kombu import Queue
-from kombu.messaging import (
-    Producer as SyncProducer,
-    Consumer as SyncConsumer,
-    is_connection,
-    maybe_channel
-)
-from kombu.utils.functional import ChannelPromise
-
-from celery.aio.common import maybe_declare
-from celery.aio.utils import AsyncChannelPromise
-
-
-class Producer(SyncProducer):
-    async def publish(self, body, routing_key=None, delivery_mode=None,
-                mandatory=False, immediate=False, priority=0,
-                content_type=None, content_encoding=None, serializer=None,
-                headers=None, compression=None, exchange=None, retry=False,
-                retry_policy=None, declare=None, expiration=None, timeout=None,
-                **properties):
-        """Publish message to the specified exchange.
-
-        Arguments:
-            body (Any): Message body.
-            routing_key (str): Message routing key.
-            delivery_mode (enum): See :attr:`delivery_mode`.
-            mandatory (bool): Currently not supported.
-            immediate (bool): Currently not supported.
-            priority (int): Message priority. A number between 0 and 9.
-            content_type (str): Content type. Default is auto-detect.
-            content_encoding (str): Content encoding. Default is auto-detect.
-            serializer (str): Serializer to use. Default is auto-detect.
-            compression (str): Compression method to use.  Default is none.
-            headers (Dict): Mapping of arbitrary headers to pass along
-                with the message body.
-            exchange (kombu.entity.Exchange, str): Override the exchange.
-                Note that this exchange must have been declared.
-            declare (Sequence[EntityT]): Optional list of required entities
-                that must have been declared before publishing the message.
-                The entities will be declared using
-                :func:`~kombu.common.maybe_declare`.
-            retry (bool): Retry publishing, or declaring entities if the
-                connection is lost.
-            retry_policy (Dict): Retry configuration, this is the keywords
-                supported by :meth:`~kombu.Connection.ensure`.
-            expiration (float): A TTL in seconds can be specified per message.
-                Default is no expiration.
-            timeout (float): Set timeout to wait maximum timeout second
-                for message to publish.
-            **properties (Any): Additional message properties, see AMQP spec.
-        """
-        _publish = self._publish
-
-        declare = [] if declare is None else declare
-        headers = {} if headers is None else headers
-        retry_policy = {} if retry_policy is None else retry_policy
-        routing_key = self.routing_key if routing_key is None else routing_key
-        compression = self.compression if compression is None else compression
-
-        exchange_name, properties['delivery_mode'] = self._delivery_details(
-            exchange or self.exchange, delivery_mode,
-        )
-
-        if expiration is not None:
-            properties['expiration'] = str(int(expiration * 1000))
-
-        body, content_type, content_encoding = self._prepare(
-            body, serializer, content_type, content_encoding,
-            compression, headers)
-
-        if self.auto_declare and self.exchange.name:
-            if self.exchange not in declare:
-                # XXX declare should be a Set.
-                declare.append(self.exchange)
-
-        if retry:
-            conn = await self.connection
-            _publish = conn.ensure(self, _publish, **retry_policy)
-        return await _publish(
-            body, priority, content_type, content_encoding,
-            headers, properties, routing_key, mandatory, immediate,
-            exchange_name, declare, timeout
-        )
-
-    async def _publish(self, body, priority, content_type, content_encoding,
-                 headers, properties, routing_key, mandatory,
-                 immediate, exchange, declare, timeout=None):
-        channel = await self.channel
-        message = channel.prepare_message(
-            body, priority, content_type,
-            content_encoding, headers, properties,
-        )
-        if declare:
-            maybe_declare = self.maybe_declare
-            await asyncio.gather(*(
-                maybe_declare(entity)
-                for entity in declare
-            ))
-
-        # handle autogenerated queue names for reply_to
-        reply_to = properties.get('reply_to')
-        if isinstance(reply_to, Queue):
-            properties['reply_to'] = reply_to.name
-        return await channel.basic_publish(
-            message,
-            exchange=exchange, routing_key=routing_key,
-            mandatory=mandatory, immediate=immediate,
-            timeout=timeout
-        )
-
-    async def maybe_declare(self, entity, retry=False, **retry_policy):
-        """Declare exchange if not already declared during this session."""
-        if entity:
-            return await maybe_declare(
-                entity, await self.channel, retry, **retry_policy)
-
-    async def _get_channel(self):
-        channel = self._channel
-        if isinstance(channel, AsyncChannelPromise):
-            channel = self._channel = await channel()
-            self.exchange.revive(channel)
-            if self.on_return:
-                channel.events['basic_return'].add(self.on_return)
-        return channel
-
-    def _set_channel(self, channel):
-        self._channel = channel
-
-    channel = property(_get_channel, _set_channel)
-
-    def revive(self, channel):
-        """Revive the producer after connection loss."""
-        if is_connection(channel):
-            connection = channel
-            self.__connection__ = connection
-            channel = AsyncChannelPromise(connection.default_channel)
-        if isinstance(channel, ChannelPromise):
-            self._channel = channel
-            self.exchange = self.exchange(channel)
-        else:
-            # Channel already concrete
-            self._channel = channel
-            if self.on_return:
-                self._channel.events['basic_return'].add(self.on_return)
-            self.exchange = self.exchange(channel)
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, *exc_info):
-        self.release()
-
-    def release(self):
-        pass
-
-    close = release
-
-    async def _get_connection(self):
-        if self.__connection__ is not None:
-            return self.__connection__
-        try:
-            channel = await self.channel
-            return channel.connection.client
-        except AttributeError:
-            pass
-
-    @property
-    def connection(self):
-        return self._get_connection()
-
-
-class Consumer(SyncConsumer):
-    if TYPE_CHECKING:
-        from celery.aio.entity import Queue
-
-        _queues: Dict[str, Queue]
-        @property
-        def queues(self) -> List[Queue]: ...  # noqa
-
-    def __init__(
-        self, channel, queues=None, no_ack=None, auto_declare=None,
-        callbacks=None, on_decode_error=None, on_message=None,
-        accept=None, prefetch_count=None, tag_prefix=None
-    ):
-        super().__init__(
-            None, queues, no_ack, auto_declare,
-            callbacks, on_decode_error, on_message,
-            accept, prefetch_count, tag_prefix
-        )
-        self.channel = channel
-
-    async def init(self):
-        if self.channel:
-            await self.revive(self.channel)
-
-    async def revive(self, channel):
-        self._active_tags.clear()
-        channel = self.channel = maybe_channel(channel)
-        # modify dict size while iterating over it is not allowed
-        for qname, queue in list(self._queues.items()):
-            # name may have changed after declare
-            self._queues.pop(qname, None)
-            queue = self._queues[queue.name] = queue(self.channel)
-            queue.revive(channel)
-
-        if self.auto_declare:
-            await self.declare()
-
-        if self.prefetch_count is not None:
-            self.qos(prefetch_count=self.prefetch_count)
-
-    async def declare(self):
-        for queue in self._queues.values():
-            await queue.declare()
-
-    def _basic_consume(self, queue: Queue, consumer_tag=None,
-                       no_ack=None, nowait=True):
-        tag = self._active_tags.get(queue.name)
-        if tag is None:
-            tag = self._add_tag(queue, consumer_tag)
-            queue.consume(tag, self._receive_callback,
-                          no_ack=no_ack, nowait=nowait)
-        return tag
+import asyncio
+
+from typing import TYPE_CHECKING, Dict, List
+
+from kombu import Queue
+from kombu.messaging import (
+    Producer as SyncProducer,
+    Consumer as SyncConsumer,
+    is_connection,
+    maybe_channel
+)
+from kombu.utils.functional import ChannelPromise
+
+from celery.aio.common import maybe_declare
+from celery.aio.utils import AsyncChannelPromise
+
+
+class Producer(SyncProducer):
+    async def publish(self, body, routing_key=None, delivery_mode=None,
+                mandatory=False, immediate=False, priority=0,
+                content_type=None, content_encoding=None, serializer=None,
+                headers=None, compression=None, exchange=None, retry=False,
+                retry_policy=None, declare=None, expiration=None, timeout=None,
+                **properties):
+        """Publish message to the specified exchange.
+
+        Arguments:
+            body (Any): Message body.
+            routing_key (str): Message routing key.
+            delivery_mode (enum): See :attr:`delivery_mode`.
+            mandatory (bool): Currently not supported.
+            immediate (bool): Currently not supported.
+            priority (int): Message priority. A number between 0 and 9.
+            content_type (str): Content type. Default is auto-detect.
+            content_encoding (str): Content encoding. Default is auto-detect.
+            serializer (str): Serializer to use. Default is auto-detect.
+            compression (str): Compression method to use.  Default is none.
+            headers (Dict): Mapping of arbitrary headers to pass along
+                with the message body.
+            exchange (kombu.entity.Exchange, str): Override the exchange.
+                Note that this exchange must have been declared.
+            declare (Sequence[EntityT]): Optional list of required entities
+                that must have been declared before publishing the message.
+                The entities will be declared using
+                :func:`~kombu.common.maybe_declare`.
+            retry (bool): Retry publishing, or declaring entities if the
+                connection is lost.
+            retry_policy (Dict): Retry configuration, this is the keywords
+                supported by :meth:`~kombu.Connection.ensure`.
+            expiration (float): A TTL in seconds can be specified per message.
+                Default is no expiration.
+            timeout (float): Set timeout to wait maximum timeout second
+                for message to publish.
+            **properties (Any): Additional message properties, see AMQP spec.
+        """
+        _publish = self._publish
+
+        declare = [] if declare is None else declare
+        headers = {} if headers is None else headers
+        retry_policy = {} if retry_policy is None else retry_policy
+        routing_key = self.routing_key if routing_key is None else routing_key
+        compression = self.compression if compression is None else compression
+
+        exchange_name, properties['delivery_mode'] = self._delivery_details(
+            exchange or self.exchange, delivery_mode,
+        )
+
+        if expiration is not None:
+            properties['expiration'] = str(int(expiration * 1000))
+
+        body, content_type, content_encoding = self._prepare(
+            body, serializer, content_type, content_encoding,
+            compression, headers)
+
+        if self.auto_declare and self.exchange.name:
+            if self.exchange not in declare:
+                # XXX declare should be a Set.
+                declare.append(self.exchange)
+
+        if retry:
+            conn = await self.connection
+            _publish = conn.ensure(self, _publish, **retry_policy)
+        return await _publish(
+            body, priority, content_type, content_encoding,
+            headers, properties, routing_key, mandatory, immediate,
+            exchange_name, declare, timeout
+        )
+
+    async def _publish(self, body, priority, content_type, content_encoding,
+                 headers, properties, routing_key, mandatory,
+                 immediate, exchange, declare, timeout=None):
+        channel = await self.channel
+        message = channel.prepare_message(
+            body, priority, content_type,
+            content_encoding, headers, properties,
+        )
+        if declare:
+            maybe_declare = self.maybe_declare
+            await asyncio.gather(*(
+                maybe_declare(entity)
+                for entity in declare
+            ))
+
+        # handle autogenerated queue names for reply_to
+        reply_to = properties.get('reply_to')
+        if isinstance(reply_to, Queue):
+            properties['reply_to'] = reply_to.name
+        return await channel.basic_publish(
+            message,
+            exchange=exchange, routing_key=routing_key,
+            mandatory=mandatory, immediate=immediate,
+            timeout=timeout
+        )
+
+    async def maybe_declare(self, entity, retry=False, **retry_policy):
+        """Declare exchange if not already declared during this session."""
+        if entity:
+            return await maybe_declare(
+                entity, await self.channel, retry, **retry_policy)
+
+    async def _get_channel(self):
+        channel = self._channel
+        if isinstance(channel, AsyncChannelPromise):
+            channel = self._channel = await channel()
+            self.exchange.revive(channel)
+            if self.on_return:
+                channel.events['basic_return'].add(self.on_return)
+        return channel
+
+    def _set_channel(self, channel):
+        self._channel = channel
+
+    channel = property(_get_channel, _set_channel)
+
+    def revive(self, channel):
+        """Revive the producer after connection loss."""
+        if is_connection(channel):
+            connection = channel
+            self.__connection__ = connection
+            channel = AsyncChannelPromise(connection.default_channel)
+        if isinstance(channel, ChannelPromise):
+            self._channel = channel
+            self.exchange = self.exchange(channel)
+        else:
+            # Channel already concrete
+            self._channel = channel
+            if self.on_return:
+                self._channel.events['basic_return'].add(self.on_return)
+            self.exchange = self.exchange(channel)
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *exc_info):
+        self.release()
+
+    def release(self):
+        pass
+
+    close = release
+
+    async def _get_connection(self):
+        if self.__connection__ is not None:
+            return self.__connection__
+        try:
+            channel = await self.channel
+            return channel.connection.client
+        except AttributeError:
+            pass
+
+    @property
+    def connection(self):
+        return self._get_connection()
+
+
+class Consumer(SyncConsumer):
+    if TYPE_CHECKING:
+        from celery.aio.entity import Queue
+
+        _queues: Dict[str, Queue]
+        @property
+        def queues(self) -> List[Queue]: ...  # noqa
+
+    def __init__(
+        self, channel, queues=None, no_ack=None, auto_declare=None,
+        callbacks=None, on_decode_error=None, on_message=None,
+        accept=None, prefetch_count=None, tag_prefix=None
+    ):
+        super().__init__(
+            None, queues, no_ack, auto_declare,
+            callbacks, on_decode_error, on_message,
+            accept, prefetch_count, tag_prefix
+        )
+        self.channel = channel
+
+    async def init(self):
+        if self.channel:
+            await self.revive(self.channel)
+
+    async def revive(self, channel):
+        self._active_tags.clear()
+        channel = self.channel = maybe_channel(channel)
+        # modify dict size while iterating over it is not allowed
+        for qname, queue in list(self._queues.items()):
+            # name may have changed after declare
+            self._queues.pop(qname, None)
+            queue = self._queues[queue.name] = queue(self.channel)
+            queue.revive(channel)
+
+        if self.auto_declare:
+            await self.declare()
+
+        if self.prefetch_count is not None:
+            self.qos(prefetch_count=self.prefetch_count)
+
+    async def declare(self):
+        for queue in self._queues.values():
+            await queue.declare()
+
+    def _basic_consume(self, queue: Queue, consumer_tag=None,
+                       no_ack=None, nowait=True):
+        tag = self._active_tags.get(queue.name)
+        if tag is None:
+            tag = self._add_tag(queue, consumer_tag)
+            queue.consume(tag, self._receive_callback,
+                          no_ack=no_ack, nowait=nowait)
+        return tag
```

### Comparing `deepfos-celery-1.0.2/celery/aio/pool.py` & `deepfos-celery-1.0.3/celery/aio/pool.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/aio/pools.py` & `deepfos-celery-1.0.3/celery/aio/pools.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from typing import *
-from kombu.pools import (
-    PoolGroup,
-    connections,
-    register_group,
-    use_global_limit,
-)
-
-from celery.aio.messaging import Producer
-from celery.aio.utils import Resource, async_lazy
-
-
-class AioProducerPool(Resource):
-    Producer = Producer
-    close_after_fork = True
-
-    if TYPE_CHECKING:
-        from .connection import ConnectionPool
-        connections: ConnectionPool
-
-    def __init__(self, connections, *args, **kwargs):
-        self.connections = connections
-        self.Producer = kwargs.pop('Producer', None) or self.Producer
-        super().__init__(*args, **kwargs)
-
-    async def _acquire_connection(self):
-        return await self.connections.get(block=True)
-
-    async def create_producer(self):
-        conn = await self._acquire_connection()
-        try:
-            return self.Producer(conn)
-        except BaseException:
-            await conn.release()
-            raise
-
-    def new(self):
-        return async_lazy(self.create_producer)
-
-    def setup(self):
-        if self.limit:
-            for _ in range(self.limit):
-                self._resource.put_nowait(self.new())
-
-    async def close_resource(self, resource):
-        pass
-
-    async def prepare(self, p):
-        if isinstance(p, async_lazy):
-            p = await p()
-        if p._channel is None:
-            conn = await self._acquire_connection()
-            try:
-                p.revive(conn)
-            except BaseException:
-                await conn.release()
-                raise
-        return p
-
-    async def release(self, resource):
-        if resource.__connection__:
-            await resource.__connection__.release()
-        resource.channel = None
-        await super().release(resource)
-
-
-class Producers(PoolGroup):
-    def create(self, connection, limit):
-        return AioProducerPool(connections[connection], limit=limit)
-
-
-producers = register_group(Producers(limit=use_global_limit))
+from typing import *
+from kombu.pools import (
+    PoolGroup,
+    connections,
+    register_group,
+    use_global_limit,
+)
+
+from celery.aio.messaging import Producer
+from celery.aio.utils import Resource, async_lazy
+
+
+class AioProducerPool(Resource):
+    Producer = Producer
+    close_after_fork = True
+
+    if TYPE_CHECKING:
+        from .connection import ConnectionPool
+        connections: ConnectionPool
+
+    def __init__(self, connections, *args, **kwargs):
+        self.connections = connections
+        self.Producer = kwargs.pop('Producer', None) or self.Producer
+        super().__init__(*args, **kwargs)
+
+    async def _acquire_connection(self):
+        return await self.connections.get(block=True)
+
+    async def create_producer(self):
+        conn = await self._acquire_connection()
+        try:
+            return self.Producer(conn)
+        except BaseException:
+            await conn.release()
+            raise
+
+    def new(self):
+        return async_lazy(self.create_producer)
+
+    def setup(self):
+        if self.limit:
+            for _ in range(self.limit):
+                self._resource.put_nowait(self.new())
+
+    async def close_resource(self, resource):
+        pass
+
+    async def prepare(self, p):
+        if isinstance(p, async_lazy):
+            p = await p()
+        if p._channel is None:
+            conn = await self._acquire_connection()
+            try:
+                p.revive(conn)
+            except BaseException:
+                await conn.release()
+                raise
+        return p
+
+    async def release(self, resource):
+        if resource.__connection__:
+            await resource.__connection__.release()
+        resource.channel = None
+        await super().release(resource)
+
+
+class Producers(PoolGroup):
+    def create(self, connection, limit):
+        return AioProducerPool(connections[connection], limit=limit)
+
+
+producers = register_group(Producers(limit=use_global_limit))
```

### Comparing `deepfos-celery-1.0.2/celery/aio/redis.py` & `deepfos-celery-1.0.3/celery/aio/redis.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,904 +1,904 @@
-import asyncio
-import socket
-import functools
-import warnings
-
-from itertools import count
-from contextlib import asynccontextmanager
-from time import monotonic, time
-from typing import *
-
-import aioredis
-import numbers
-
-from aioredis import sentinel
-from kombu.transport.redis import (
-    Transport as SyncTransport,
-    Channel as SyncChannel,
-    MultiChannelPoller as SyncMultiChannelPoller,
-    QoS as SyncQoS,
-    PrefixedStrictRedis,
-    error_classes_t,
-    virtual,
-    dumps,
-    loads,
-    cycle_by_name,
-    bytes_to_str,
-    InconsistencyError,
-    VersionMismatch,
-    Empty,
-    MutexHeld,
-
-    crit,
-    warn,
-    _parse_url,
-)
-from kombu.transport.virtual.base import (
-    UNDELIVERABLE_FMT,
-    queue_declare_ok_t,
-    uuid,
-    ChannelError,
-    UndeliverableWarning,
-    FairCycle,
-)
-from celery.aio.exchange import STANDARD_EXCHANGE_TYPES
-from celery.aio.utils import is_async_callable
-from celery.utils.log import get_logger
-
-
-logger = get_logger(__name__)
-
-
-@asynccontextmanager
-async def Mutex(client: aioredis.Redis, name, expire):
-    """Acquire redis lock in non blocking way.
-
-    Raise MutexHeld if not successful.
-    """
-    lock = client.lock(name, timeout=expire)
-    lock_acquired = False
-    try:
-        lock_acquired = await lock.acquire(blocking=False)
-        if lock_acquired:
-            yield
-        else:
-            raise MutexHeld()
-    finally:
-        if lock_acquired:
-            try:
-                await lock.release()
-            except aioredis.exceptions.LockNotOwnedError:
-                # when lock is expired
-                pass
-
-
-class QoS(SyncQoS):
-    @asynccontextmanager
-    async def pipe_or_acquire(self, pipe=None, client=None):
-        if pipe:
-            yield pipe
-        else:
-            with self.channel.conn_or_acquire(client) as client:
-                async with client.pipeline() as pipe:
-                    yield pipe
-
-    async def _remove_from_indices(self, delivery_tag, pipe=None):
-        async with self.pipe_or_acquire(pipe) as pipe:
-            return pipe.zrem(self.unacked_index_key, delivery_tag) \
-                       .hdel(self.unacked_key, delivery_tag)
-
-    async def append(self, message, delivery_tag):
-        delivery = message.delivery_info
-        EX, RK = delivery['exchange'], delivery['routing_key']
-        zadd_args = [{delivery_tag: time()}]
-
-        async with self.pipe_or_acquire() as pipe:
-            await (pipe
-                .zadd(self.unacked_index_key, *zadd_args)
-                .hset(self.unacked_key, delivery_tag,
-                      dumps([message._raw, EX, RK]))
-                .execute()
-            )
-            if self._dirty:
-                self._flush()
-            self._quick_append(delivery_tag, message)
-
-    async def restore_unacked(self, client=None):
-        with self.channel.conn_or_acquire(client) as client:
-            for tag in self._delivered:
-                await self.restore_by_tag(tag, client=client)
-        self._delivered.clear()
-
-    async def ack(self, delivery_tag):
-        pipe = await self._remove_from_indices(delivery_tag)
-        await pipe.execute()
-        self._quick_ack(delivery_tag)
-
-    async def reject(self, delivery_tag, requeue=False):
-        if requeue:
-            await self.restore_by_tag(delivery_tag, leftmost=True)
-        await self.ack(delivery_tag)
-
-    async def restore_visible(self, start=0, num=10, interval=10):
-        self._vrestore_count += 1
-        if (self._vrestore_count - 1) % interval:
-            return
-        with self.channel.conn_or_acquire() as client:
-            ceil = time() - self.visibility_timeout
-            try:
-                async with Mutex(client, self.unacked_mutex_key,
-                           self.unacked_mutex_expire):
-                    visible = await client.zrevrangebyscore(
-                        self.unacked_index_key, ceil, 0,
-                        start=num and start, num=num, withscores=True)
-                    for tag, score in visible or []:
-                        await self.restore_by_tag(tag, client)
-            except MutexHeld:
-                pass
-
-    async def restore_by_tag(self, tag, client=None, leftmost=False):
-
-        async def restore_transaction(pipe):
-            p = pipe.hget(self.unacked_key, tag)
-            pipe.multi()
-            pipe = await self._remove_from_indices(tag, pipe)
-            if p:
-                M, EX, RK = loads(bytes_to_str(p))  # json is unicode
-                await self.channel._do_restore_message(M, EX, RK, pipe, leftmost)
-
-        with self.channel.conn_or_acquire(client) as client:
-            await client.transaction(restore_transaction, self.unacked_key)
-
-
-class AsyncFairCycle(FairCycle):
-    async def get(self, callback, **kwargs):
-        """Get from next resource."""
-        for tried in count(0):  # for infinity
-            resource = self._next()
-            try:
-                return await self.fun(resource, callback, **kwargs)
-            except self.predicate:
-                # reraise when retries exchausted.
-                if tried >= len(self.resources) - 1:
-                    raise
-
-
-def get_redis_error_classes():
-    from aioredis import exceptions
-    # This exception suddenly changed name between redis-py versions
-    if hasattr(exceptions, 'InvalidData'):
-        DataError = exceptions.InvalidData
-    else:
-        DataError = exceptions.DataError
-
-    return error_classes_t(
-        (virtual.Transport.connection_errors + (
-            InconsistencyError,
-            socket.error,
-            IOError,
-            OSError,
-            exceptions.ConnectionError,
-            exceptions.AuthenticationError,
-            exceptions.TimeoutError)),
-        (virtual.Transport.channel_errors + (
-            DataError,
-            exceptions.InvalidResponse,
-            exceptions.ResponseError)),
-    )
-
-
-class Channel(SyncChannel):
-    QoS = QoS
-    connection_class = aioredis.Connection
-    connection_class_ssl = aioredis.SSLConnection
-    exchange_types = dict(STANDARD_EXCHANGE_TYPES)
-
-    if TYPE_CHECKING:
-        from aioredis.client import PubSub
-        @property
-        def subclient(self) -> PubSub: ...  # noqa
-
-    def __init__(self, *args, **kwargs):
-        virtual.Channel.__init__(self, *args, **kwargs)
-
-        if not self.ack_emulation:  # disable visibility timeout
-            self.QoS = virtual.QoS
-
-        self._queue_cycle = cycle_by_name(self.queue_order_strategy)()
-        self.Client = self._get_client()
-        self.ResponseError = self._get_response_error()
-        self.active_fanout_queues = set()
-        self.auto_delete_queues = set()
-        self._fanout_to_queue = {}
-        self.handlers = {'BRPOP': self._brpop_read, 'LISTEN': self._receive}
-
-        if self.fanout_prefix:
-            if isinstance(self.fanout_prefix, str):
-                self.keyprefix_fanout = self.fanout_prefix
-        else:
-            # previous versions did not set a fanout, so cannot enable
-            # by default.
-            self.keyprefix_fanout = ''
-
-        self.connection.cycle.add(self)  # add to channel poller.
-        # copy errors, in case channel closed but threads still
-        # are still waiting for data.
-        self.connection_errors = self.connection.connection_errors
-        self._conn_evaled = False
-
-        self._brpop_task: asyncio.Task = None
-        self._listen_task: asyncio.Task = None
-
-        # if register_after_fork is not None:
-        #     register_after_fork(self, _after_fork_cleanup_channel)
-
-    async def ping(self):
-        return await self.client.ping()
-
-    async def _after_fork(self):
-        await self._disconnect_pools()
-
-    async def _disconnect_pools(self):
-        pool = self._pool
-        async_pool = self._async_pool
-        is_same_pool = pool is async_pool
-
-        self._async_pool = self._pool = None
-
-        if pool is not None:
-            await pool.disconnect()
-
-        if not is_same_pool and async_pool is not None:
-            await async_pool.disconnect()
-
-    async def _do_restore_message(self, payload, exchange, routing_key,
-                            pipe, leftmost=False):
-        try:
-            try:
-                payload['headers']['redelivered'] = True
-                payload['properties']['delivery_info']['redelivered'] = True
-            except KeyError:
-                pass
-            for queue in await self._lookup(exchange, routing_key):
-                await (pipe.lpush if leftmost else pipe.rpush)(
-                    queue, dumps(payload),
-                )
-        except Exception:
-            crit('Could not restore message: %r', payload, exc_info=True)
-
-    async def _restore(self, message, leftmost=False):
-        if not self.ack_emulation:
-            delivery_info = message.delivery_info
-            message = message.serializable()
-            message['redelivered'] = True
-            for queue in await self._lookup(
-                delivery_info['exchange'], delivery_info['routing_key']
-            ):
-                await self._put(queue, message)
-            return
-
-        tag = message.delivery_tag
-
-        async def restore_transaction(pipe):
-            P = await pipe.hget(self.unacked_key, tag)
-            pipe.multi()
-            await pipe.hdel(self.unacked_key, tag)
-            if P:
-                M, EX, RK = loads(bytes_to_str(P))  # json is unicode
-                await self._do_restore_message(M, EX, RK, pipe, leftmost)
-
-        with self.conn_or_acquire() as client:
-            await client.transaction(restore_transaction, self.unacked_key)
-
-    async def _restore_at_beginning(self, message):
-        return await self._restore(message, leftmost=True)
-
-    def _get_response_error(self):
-        from aioredis import exceptions
-        return exceptions.ResponseError
-
-    async def _get(self, queue):
-        with self.conn_or_acquire() as client:
-            for pri in self.priority_steps:
-                item = await client.rpop(self._q_for_pri(queue, pri))
-                if item:
-                    return loads(bytes_to_str(item))
-            raise Empty()
-
-    async def _size(self, queue):
-        with self.conn_or_acquire() as client:
-            async with client.pipeline() as pipe:
-                for pri in self.priority_steps:
-                    pipe = pipe.llen(self._q_for_pri(queue, pri))
-                sizes = await pipe.execute()
-        return sum(size for size in sizes
-                   if isinstance(size, numbers.Integral))
-
-    async def _put(self, queue, message, **kwargs):
-        """Deliver message."""
-        pri = self._get_message_priority(message, reverse=False)
-
-        with self.conn_or_acquire() as client:
-            await client.lpush(self._q_for_pri(queue, pri), dumps(message))
-
-    async def _put_fanout(self, exchange, message, routing_key, **kwargs):
-        """Deliver fanout message."""
-        with self.conn_or_acquire() as client:
-            await client.publish(
-                self._get_publish_topic(exchange, routing_key),
-                dumps(message),
-            )
-
-    async def _queue_bind(self, exchange, routing_key, pattern, queue):
-        if self.typeof(exchange).type == 'fanout':
-            # Mark exchange as fanout.
-            self._fanout_queues[queue] = (
-                exchange, routing_key.replace('#', '*'),
-            )
-        with self.conn_or_acquire() as client:
-            await client.sadd(
-                self.keyprefix_queue % (exchange,),
-                self.sep.join([routing_key or '', pattern or '', queue or ''])
-            )
-
-    async def _delete(self, queue, exchange, routing_key, pattern, *args, **kwargs):
-        self.auto_delete_queues.discard(queue)
-        with self.conn_or_acquire(client=kwargs.get('client')) as client:
-            await client.srem(self.keyprefix_queue % (exchange,),
-                        self.sep.join([routing_key or '',
-                                       pattern or '',
-                                       queue or '']))
-            async with client.pipeline() as pipe:
-                for pri in self.priority_steps:
-                    pipe = pipe.delete(self._q_for_pri(queue, pri))
-                await pipe.execute()
-
-    async def _has_queue(self, queue, **kwargs):
-        with self.conn_or_acquire() as client:
-            async with client.pipeline() as pipe:
-                for pri in self.priority_steps:
-                    pipe = pipe.exists(self._q_for_pri(queue, pri))
-                return any(await pipe.execute())
-
-    async def get_table(self, exchange):
-        key = self.keyprefix_queue % exchange
-        with self.conn_or_acquire() as client:
-            values = await client.smembers(key)
-            if not values:
-                # table does not exists since all queues bound to the exchange
-                # were deleted. We need just return empty list.
-                return []
-            return [tuple(bytes_to_str(val).split(self.sep)) for val in values]
-
-    async def _purge(self, queue):
-        with self.conn_or_acquire() as client:
-            async with client.pipeline() as pipe:
-                for pri in self.priority_steps:
-                    priq = self._q_for_pri(queue, pri)
-                    pipe = pipe.llen(priq).delete(priq)
-                sizes = await pipe.execute()
-                return sum(sizes[::2])
-
-    async def close(self):
-        self._closing = True
-        if not self.closed:
-            # remove from channel poller.
-            self.connection.cycle.discard(self)
-
-            # delete fanout bindings
-            client = self.__dict__.get('client')  # only if property cached
-            if client is not None:
-                for queue in self._fanout_queues:
-                    if queue in self.auto_delete_queues:
-                        await self.queue_delete(queue, client=client)
-            await self._disconnect_pools()
-            await self._close_clients()
-
-            # --------------------------------------
-            # virtual.base::Channel
-            self.closed = True
-
-            for consumer in list(self._consumers):
-                self.basic_cancel(consumer)  # todo maybe await
-            if self._qos:
-                self._qos.restore_unacked_once()
-            if self._cycle is not None:
-                self._cycle.close()
-                self._cycle = None
-            if self.connection is not None:
-                self.connection.close_channel(self)  # todo maybe await
-        self.exchange_types = None
-
-    async def _close_clients(self):
-        for attr in 'client', 'subclient':
-            try:
-                client = self.__dict__[attr]
-                connection, client.connection = client.connection, None
-                await connection.disconnect()
-            except (KeyError, AttributeError, self.ResponseError):
-                pass
-
-    def _connparams(self, asynchronous=False):
-        params = super(Channel, self)._connparams(asynchronous)
-        channel = self
-
-        if asynchronous:
-            class Connection(self.connection_class):
-                async def disconnect(self):
-                    await super().disconnect()
-                    channel._on_connection_disconnect(self)
-
-            params['connection_class'] = Connection
-        return params
-
-    def _get_pool(self, asynchronous=True):
-        params = self._connparams(asynchronous=True)
-        self.keyprefix_fanout = self.keyprefix_fanout.format(db=params['db'])
-        return aioredis.ConnectionPool(**params)
-
-    def _get_client(self):
-        if getattr(aioredis, 'VERSION', (1, 0)) < (2, 0, 0):
-            raise VersionMismatch(
-                'Redis transport requires aioredis versions 2.0.0 or later. '
-                f'You have {aioredis.__version__}')
-
-        if self.global_keyprefix:
-            return functools.partial(
-                PrefixedStrictRedis,
-                global_keyprefix=self.global_keyprefix,
-            )
-        return aioredis.StrictRedis
-
-    # -----------------------------------------------------------------------------
-    # virtual.base::Channel method overload
-    async def queue_delete(self, queue, if_unused=False, if_empty=False, **kwargs):
-        """Delete queue."""
-        if if_empty and self._size(queue):
-            return
-        for exchange, routing_key, args in self.state.queue_bindings(queue):
-            meta = self.typeof(exchange).prepare_bind(
-                queue, exchange, routing_key, args,
-            )
-            await self._delete(queue, exchange, *meta, **kwargs)
-        self.state.queue_bindings_delete(queue)
-
-    async def after_reply_message_received(self, queue):
-        await self.queue_delete(queue)
-
-    async def queue_bind(self, queue, exchange=None, routing_key='',
-                   arguments=None, **kwargs):
-        """Bind `queue` to `exchange` with `routing key`."""
-        exchange = exchange or 'amq.direct'
-        if self.state.has_binding(queue, exchange, routing_key):
-            return
-        # Add binding:
-        self.state.binding_declare(queue, exchange, routing_key, arguments)
-        # Update exchange's routing table:
-        table = self.state.exchanges[exchange].setdefault('table', [])
-        meta = self.typeof(exchange).prepare_bind(
-            queue, exchange, routing_key, arguments,
-        )
-        table.append(meta)
-        if self.supports_fanout:
-            await self._queue_bind(exchange, *meta)
-
-    async def queue_unbind(self, queue, exchange=None, routing_key='',
-                     arguments=None, **kwargs):
-        # Remove queue binding:
-        self.state.binding_delete(queue, exchange, routing_key)
-        try:
-            table = await self.get_table(exchange)
-        except KeyError:
-            return
-        binding_meta = self.typeof(exchange).prepare_bind(
-            queue, exchange, routing_key, arguments,
-        )
-        # TODO: the complexity of this operation is O(number of bindings).
-        # Should be optimized.  Modifying table in place.
-        table[:] = [meta for meta in table if meta != binding_meta]
-
-    async def list_bindings(self):
-        return ((queue, exchange, rkey)
-                for exchange in self.state.exchanges
-                for rkey, pattern, queue in await self.get_table(exchange))
-
-    async def queue_declare(self, queue=None, passive=False, **kwargs):
-        """Declare queue."""
-        queue = queue or 'amq.gen-%s' % uuid()
-        if passive and not (await self._has_queue(queue, **kwargs)):
-            raise ChannelError(
-                'NOT_FOUND - no queue {!r} in vhost {!r}'.format(
-                    queue, self.connection.client.virtual_host or '/'),
-                (50, 10), 'Channel.queue_declare', '404',
-            )
-        else:
-            self._new_queue(queue, **kwargs)
-        return queue_declare_ok_t(queue, await self._size(queue), 0)
-
-    async def queue_purge(self, queue, **kwargs):
-        """Remove all ready messages from queue."""
-        return await self._purge(queue)
-
-    async def basic_publish(self, message, exchange, routing_key, **kwargs):
-        """Publish message."""
-        self._inplace_augment_message(message, exchange, routing_key)
-        if exchange:
-            return await self.typeof(exchange).deliver(
-                message, exchange, routing_key, **kwargs
-            )
-        # anon exchange: routing_key is the destination queue
-        return await self._put(routing_key, message, **kwargs)
-
-    async def basic_get(self, queue, no_ack=False, **kwargs):
-        """Get message by direct access (synchronous)."""
-        try:
-            message = self.Message((await self._get(queue)), channel=self)
-            if not no_ack:
-                self.qos.append(message, message.delivery_tag)
-            return message
-        except Empty:
-            pass
-
-    async def _lookup(self, exchange, routing_key, default=None):
-        """Find all queues matching `routing_key` for the given `exchange`.
-
-        Returns:
-            str: queue name -- must return the string `default`
-                if no queues matched.
-        """
-        if default is None:
-            default = self.deadletter_queue
-        if not exchange:  # anon exchange
-            return [routing_key or default]
-
-        try:
-            R = self.typeof(exchange).lookup(
-                await self.get_table(exchange),
-                exchange, routing_key, default,
-            )
-        except KeyError:
-            R = []
-
-        if not R and default is not None:
-            warnings.warn(UndeliverableWarning(UNDELIVERABLE_FMT.format(
-                exchange=exchange, routing_key=routing_key)),
-            )
-            self._new_queue(default)
-            R = [default]
-        return R
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.close()
-
-    def __enter__(self):
-        raise NotImplementedError
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        raise NotImplementedError
-
-    def _reset_cycle(self):
-        self._cycle = AsyncFairCycle(
-            self._get_and_deliver, self._active_queues, Empty)
-
-    async def _get_and_deliver(self, queue, callback):
-        message = await self._get(queue)
-        callback(message, queue)
-
-    # -----------------------------------------------------------------------------
-    # exchange
-    async def exchange_delete(self, exchange, if_unused=False, nowait=False):
-        """Delete `exchange` and all its bindings."""
-        for rkey, _, queue in (await self.get_table(exchange)):
-            await self.queue_delete(queue, if_unused=True, if_empty=True)
-        self.state.exchanges.pop(exchange, None)
-
-    # -----------------------------------------------------------------------------
-    # consumer
-    async def _brpop_start(self, timeout=1):
-        queues = self._queue_cycle.consume(len(self.active_queues))
-        if not queues:
-            return
-
-        keys = [self._q_for_pri(queue, pri) for pri in self.priority_steps
-                for queue in queues] + [timeout or 0]
-
-        command_args = ['BRPOP', *keys]
-        if self.global_keyprefix:
-            command_args = self.client._prefix_args(command_args)
-
-        async def brpop(conn):
-            await conn.send_command(*command_args)
-            return await self._brpop_read_impl()
-
-        self._in_poll = True
-        self._brpop_task = task = asyncio.create_task(
-            brpop(self.client.connection))
-
-        await asyncio.sleep(0)
-        return task
-
-    async def _brpop_read_impl(self, **options):
-        try:
-            dest__item = await self.client.parse_response(
-                self.client.connection,
-                'BRPOP',
-                **options
-            )
-        except self.connection_errors:
-            # if there's a ConnectionError, disconnect so the next
-            # iteration will reconnect automatically.
-            await self.client.connection.disconnect()
-            raise
-        if dest__item:
-            dest, item = dest__item
-            dest = bytes_to_str(dest).rsplit(self.sep, 1)[0]
-            self._queue_cycle.rotate(dest)
-            self.connection._deliver(loads(bytes_to_str(item)), dest)
-            return True
-        else:
-            raise Empty()
-
-    def _brpop_read(self, **options):
-        try:
-            return self._brpop_task.result()
-        finally:
-            self._brpop_task = None
-            self._in_poll = None
-
-    async def _subscribe(self):
-        keys = [self._get_subscribe_topic(queue)
-                for queue in self.active_fanout_queues]
-        if not keys:
-            return
-        c = self.subclient
-        if not c.connection.is_connected:
-            await c.connection.connect()
-        self._in_listen = c.connection
-        await c.psubscribe(keys)
-        self._listen_task = t = asyncio.create_task(c.parse_response())
-        await asyncio.sleep(0)
-        return t
-
-    async def _unsubscribe_from(self, queue):
-        topic = self._get_subscribe_topic(queue)
-        c = self.subclient
-        if c.connection and c.connection.is_connected:
-            await c.unsubscribe([topic])
-
-    def _receive_one(self, c):
-        try:
-            response = self._listen_task.result()
-        except self.connection_errors:
-            self._in_listen = None
-            raise
-        finally:
-            self._listen_task = None
-        if isinstance(response, (list, tuple)):
-            payload = self._handle_message(c, response)
-            if bytes_to_str(payload['type']).endswith('message'):
-                channel = bytes_to_str(payload['channel'])
-                if payload['data']:
-                    if channel[0] == '/':
-                        _, _, channel = channel.partition('.')
-                    try:
-                        message = loads(bytes_to_str(payload['data']))
-                    except (TypeError, ValueError):
-                        warn('Cannot process event on channel %r: %s',
-                             channel, repr(payload)[:4096], exc_info=1)
-                        raise Empty()
-                    exchange = channel.split('/', 1)[0]
-                    self.connection._deliver(
-                        message, self._fanout_to_queue[exchange])
-                    return True
-
-
-class MultiChannelPoller(SyncMultiChannelPoller):
-    def __init__(self):
-        self._channels = set()
-        self._pending_tasks = set()
-
-    @staticmethod
-    async def ensure_connection(client):
-        conn = getattr(client, 'connection', None)
-        if conn is None:
-            client.connection = await client.connection_pool.get_connection('_')
-        elif not conn.is_connected:
-            await client.connection.connect()
-
-    async def _register_BRPOP(self, channel):
-        """Enable BRPOP mode for channel."""
-        await self.ensure_connection(channel.client)
-
-        if not channel._in_poll:  # send BRPOP
-            task = await channel._brpop_start()
-            task.channel = channel
-            task.cmd = 'BRPOP'
-            self._pending_tasks.add(task)
-
-    async def _register_LISTEN(self, channel):
-        """Enable LISTEN mode for channel."""
-        await self.ensure_connection(channel.client)
-
-        if not channel._in_listen:
-            task = await channel._subscribe()  # send SUBSCR
-            task.channel = channel
-            task.cmd = 'LISTEN'
-            self._pending_tasks.add(task)
-
-    async def poll(self, timeout):
-        if not self._pending_tasks:
-            return
-
-        done, pending = await asyncio.wait(
-            self._pending_tasks,
-            timeout=timeout,
-            return_when=asyncio.FIRST_COMPLETED
-        )
-        for task in done:
-            self._pending_tasks.discard(task)
-        if not done:
-            return
-        else:
-            return done.pop()
-
-    @staticmethod
-    async def handle_task(task):
-        chan = task.channel  # noqa
-        type = task.cmd  # noqa
-
-        if chan.qos.can_consume():
-            hdlr = chan.handlers[type]
-            if is_async_callable(hdlr):
-                await hdlr()
-            else:
-                hdlr()
-
-        return True
-
-    async def get(self, callback, timeout=None):
-        self._in_protected_read = True
-        try:
-            for channel in self._channels:
-                if channel.active_queues:           # BRPOP mode?
-                    if channel.qos.can_consume():
-                        await self._register_BRPOP(channel)
-                if channel.active_fanout_queues:    # LISTEN mode?
-                    self._register_LISTEN(channel)
-
-            if (
-                (done_task := await self.poll(timeout))
-                and (await self.handle_task(done_task))
-            ):
-                return
-            # - no new data, so try to restore messages.
-            # - reset active redis commands.
-            await self.maybe_restore_messages()
-            raise Empty()
-        finally:
-            self._in_protected_read = False
-            while self.after_read:
-                try:
-                    fun = self.after_read.pop()
-                except KeyError:
-                    break
-                else:
-                    fun()
-
-    async def maybe_restore_messages(self):
-        for channel in self._channels:
-            if channel.active_queues:
-                # only need to do this once, as they are not local to channel.
-                return await channel.qos.restore_visible(
-                    num=channel.unacked_restore_limit,
-                )
-
-
-class Transport(SyncTransport):
-    Channel = Channel
-    connection_errors, channel_errors = get_redis_error_classes()
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # All channels share the same poller.
-        self.cycle = MultiChannelPoller()
-
-    async def establish_connection(self):
-        channel: Channel = self.create_channel(self)
-        await channel.ping()
-        self._avail_channels.append(channel)
-        return self     # for drain events
-
-    async def close_connection(self, connection):
-        self.cycle.close()
-        for chan_list in self._avail_channels, self.channels:
-            while chan_list:
-                try:
-                    channel = chan_list.pop()
-                except LookupError:  # pragma: no cover
-                    pass
-                else:
-                    await channel.close()
-
-    async def drain_events(self, connection, timeout=None):
-        time_start = monotonic()
-        get = self.cycle.get
-        polling_interval = self.polling_interval
-        if timeout and polling_interval and polling_interval > timeout:
-            polling_interval = timeout
-        while 1:
-            try:
-                await get(self._deliver, timeout=timeout)
-            except Empty:
-                if timeout is not None and monotonic() - time_start >= timeout:
-                    raise socket.timeout()
-                if polling_interval is not None:
-                    await asyncio.sleep(polling_interval)
-            else:
-                break
-
-
-class SentinelManagedSSLConnection(
-        sentinel.SentinelManagedConnection,
-        aioredis.SSLConnection):
-    pass
-
-
-class SentinelChannel(Channel):
-    from_transport_options = Channel.from_transport_options + (
-        'master_name',
-        'min_other_sentinels',
-        'sentinel_kwargs')
-
-    connection_class = sentinel.SentinelManagedConnection
-    connection_class_ssl = SentinelManagedSSLConnection
-
-    def _sentinel_managed_pool(self, asynchronous=False):
-        connparams = self._connparams(asynchronous)
-
-        additional_params = connparams.copy()
-
-        additional_params.pop('host', None)
-        additional_params.pop('port', None)
-
-        sentinels = []
-        for url in self.connection.client.alt:
-            url = _parse_url(url)
-            if url.scheme == 'sentinel':
-                port = url.port or self.connection.default_port
-                sentinels.append((url.hostname, port))
-
-        # Fallback for when only one sentinel is provided.
-        if not sentinels:
-            sentinels.append((connparams['host'], connparams['port']))
-
-        sentinel_inst = sentinel.Sentinel(
-            sentinels,
-            min_other_sentinels=getattr(self, 'min_other_sentinels', 0),
-            sentinel_kwargs=getattr(self, 'sentinel_kwargs', None),
-            **additional_params)
-
-        master_name = getattr(self, 'master_name', None)
-
-        if master_name is None:
-            raise ValueError(
-                "'master_name' transport option must be specified."
-            )
-
-        return sentinel_inst.master_for(
-            master_name,
-            self.Client,
-        ).connection_pool
-
-    def _get_pool(self, asynchronous=False):
-        return self._sentinel_managed_pool(asynchronous)
-
-
-class SentinelTransport(Transport):
-    """Redis Sentinel Transport."""
-
-    default_port = 26379
-    Channel = SentinelChannel
+import asyncio
+import socket
+import functools
+import warnings
+
+from itertools import count
+from contextlib import asynccontextmanager
+from time import monotonic, time
+from typing import *
+
+import aioredis
+import numbers
+
+from aioredis import sentinel
+from kombu.transport.redis import (
+    Transport as SyncTransport,
+    Channel as SyncChannel,
+    MultiChannelPoller as SyncMultiChannelPoller,
+    QoS as SyncQoS,
+    PrefixedStrictRedis,
+    error_classes_t,
+    virtual,
+    dumps,
+    loads,
+    cycle_by_name,
+    bytes_to_str,
+    InconsistencyError,
+    VersionMismatch,
+    Empty,
+    MutexHeld,
+
+    crit,
+    warn,
+    _parse_url,
+)
+from kombu.transport.virtual.base import (
+    UNDELIVERABLE_FMT,
+    queue_declare_ok_t,
+    uuid,
+    ChannelError,
+    UndeliverableWarning,
+    FairCycle,
+)
+from celery.aio.exchange import STANDARD_EXCHANGE_TYPES
+from celery.aio.utils import is_async_callable
+from celery.utils.log import get_logger
+
+
+logger = get_logger(__name__)
+
+
+@asynccontextmanager
+async def Mutex(client: aioredis.Redis, name, expire):
+    """Acquire redis lock in non blocking way.
+
+    Raise MutexHeld if not successful.
+    """
+    lock = client.lock(name, timeout=expire)
+    lock_acquired = False
+    try:
+        lock_acquired = await lock.acquire(blocking=False)
+        if lock_acquired:
+            yield
+        else:
+            raise MutexHeld()
+    finally:
+        if lock_acquired:
+            try:
+                await lock.release()
+            except aioredis.exceptions.LockNotOwnedError:
+                # when lock is expired
+                pass
+
+
+class QoS(SyncQoS):
+    @asynccontextmanager
+    async def pipe_or_acquire(self, pipe=None, client=None):
+        if pipe:
+            yield pipe
+        else:
+            with self.channel.conn_or_acquire(client) as client:
+                async with client.pipeline() as pipe:
+                    yield pipe
+
+    async def _remove_from_indices(self, delivery_tag, pipe=None):
+        async with self.pipe_or_acquire(pipe) as pipe:
+            return pipe.zrem(self.unacked_index_key, delivery_tag) \
+                       .hdel(self.unacked_key, delivery_tag)
+
+    async def append(self, message, delivery_tag):
+        delivery = message.delivery_info
+        EX, RK = delivery['exchange'], delivery['routing_key']
+        zadd_args = [{delivery_tag: time()}]
+
+        async with self.pipe_or_acquire() as pipe:
+            await (pipe
+                .zadd(self.unacked_index_key, *zadd_args)
+                .hset(self.unacked_key, delivery_tag,
+                      dumps([message._raw, EX, RK]))
+                .execute()
+            )
+            if self._dirty:
+                self._flush()
+            self._quick_append(delivery_tag, message)
+
+    async def restore_unacked(self, client=None):
+        with self.channel.conn_or_acquire(client) as client:
+            for tag in self._delivered:
+                await self.restore_by_tag(tag, client=client)
+        self._delivered.clear()
+
+    async def ack(self, delivery_tag):
+        pipe = await self._remove_from_indices(delivery_tag)
+        await pipe.execute()
+        self._quick_ack(delivery_tag)
+
+    async def reject(self, delivery_tag, requeue=False):
+        if requeue:
+            await self.restore_by_tag(delivery_tag, leftmost=True)
+        await self.ack(delivery_tag)
+
+    async def restore_visible(self, start=0, num=10, interval=10):
+        self._vrestore_count += 1
+        if (self._vrestore_count - 1) % interval:
+            return
+        with self.channel.conn_or_acquire() as client:
+            ceil = time() - self.visibility_timeout
+            try:
+                async with Mutex(client, self.unacked_mutex_key,
+                           self.unacked_mutex_expire):
+                    visible = await client.zrevrangebyscore(
+                        self.unacked_index_key, ceil, 0,
+                        start=num and start, num=num, withscores=True)
+                    for tag, score in visible or []:
+                        await self.restore_by_tag(tag, client)
+            except MutexHeld:
+                pass
+
+    async def restore_by_tag(self, tag, client=None, leftmost=False):
+
+        async def restore_transaction(pipe):
+            p = pipe.hget(self.unacked_key, tag)
+            pipe.multi()
+            pipe = await self._remove_from_indices(tag, pipe)
+            if p:
+                M, EX, RK = loads(bytes_to_str(p))  # json is unicode
+                await self.channel._do_restore_message(M, EX, RK, pipe, leftmost)
+
+        with self.channel.conn_or_acquire(client) as client:
+            await client.transaction(restore_transaction, self.unacked_key)
+
+
+class AsyncFairCycle(FairCycle):
+    async def get(self, callback, **kwargs):
+        """Get from next resource."""
+        for tried in count(0):  # for infinity
+            resource = self._next()
+            try:
+                return await self.fun(resource, callback, **kwargs)
+            except self.predicate:
+                # reraise when retries exchausted.
+                if tried >= len(self.resources) - 1:
+                    raise
+
+
+def get_redis_error_classes():
+    from aioredis import exceptions
+    # This exception suddenly changed name between redis-py versions
+    if hasattr(exceptions, 'InvalidData'):
+        DataError = exceptions.InvalidData
+    else:
+        DataError = exceptions.DataError
+
+    return error_classes_t(
+        (virtual.Transport.connection_errors + (
+            InconsistencyError,
+            socket.error,
+            IOError,
+            OSError,
+            exceptions.ConnectionError,
+            exceptions.AuthenticationError,
+            exceptions.TimeoutError)),
+        (virtual.Transport.channel_errors + (
+            DataError,
+            exceptions.InvalidResponse,
+            exceptions.ResponseError)),
+    )
+
+
+class Channel(SyncChannel):
+    QoS = QoS
+    connection_class = aioredis.Connection
+    connection_class_ssl = aioredis.SSLConnection
+    exchange_types = dict(STANDARD_EXCHANGE_TYPES)
+
+    if TYPE_CHECKING:
+        from aioredis.client import PubSub
+        @property
+        def subclient(self) -> PubSub: ...  # noqa
+
+    def __init__(self, *args, **kwargs):
+        virtual.Channel.__init__(self, *args, **kwargs)
+
+        if not self.ack_emulation:  # disable visibility timeout
+            self.QoS = virtual.QoS
+
+        self._queue_cycle = cycle_by_name(self.queue_order_strategy)()
+        self.Client = self._get_client()
+        self.ResponseError = self._get_response_error()
+        self.active_fanout_queues = set()
+        self.auto_delete_queues = set()
+        self._fanout_to_queue = {}
+        self.handlers = {'BRPOP': self._brpop_read, 'LISTEN': self._receive}
+
+        if self.fanout_prefix:
+            if isinstance(self.fanout_prefix, str):
+                self.keyprefix_fanout = self.fanout_prefix
+        else:
+            # previous versions did not set a fanout, so cannot enable
+            # by default.
+            self.keyprefix_fanout = ''
+
+        self.connection.cycle.add(self)  # add to channel poller.
+        # copy errors, in case channel closed but threads still
+        # are still waiting for data.
+        self.connection_errors = self.connection.connection_errors
+        self._conn_evaled = False
+
+        self._brpop_task: asyncio.Task = None
+        self._listen_task: asyncio.Task = None
+
+        # if register_after_fork is not None:
+        #     register_after_fork(self, _after_fork_cleanup_channel)
+
+    async def ping(self):
+        return await self.client.ping()
+
+    async def _after_fork(self):
+        await self._disconnect_pools()
+
+    async def _disconnect_pools(self):
+        pool = self._pool
+        async_pool = self._async_pool
+        is_same_pool = pool is async_pool
+
+        self._async_pool = self._pool = None
+
+        if pool is not None:
+            await pool.disconnect()
+
+        if not is_same_pool and async_pool is not None:
+            await async_pool.disconnect()
+
+    async def _do_restore_message(self, payload, exchange, routing_key,
+                            pipe, leftmost=False):
+        try:
+            try:
+                payload['headers']['redelivered'] = True
+                payload['properties']['delivery_info']['redelivered'] = True
+            except KeyError:
+                pass
+            for queue in await self._lookup(exchange, routing_key):
+                await (pipe.lpush if leftmost else pipe.rpush)(
+                    queue, dumps(payload),
+                )
+        except Exception:
+            crit('Could not restore message: %r', payload, exc_info=True)
+
+    async def _restore(self, message, leftmost=False):
+        if not self.ack_emulation:
+            delivery_info = message.delivery_info
+            message = message.serializable()
+            message['redelivered'] = True
+            for queue in await self._lookup(
+                delivery_info['exchange'], delivery_info['routing_key']
+            ):
+                await self._put(queue, message)
+            return
+
+        tag = message.delivery_tag
+
+        async def restore_transaction(pipe):
+            P = await pipe.hget(self.unacked_key, tag)
+            pipe.multi()
+            await pipe.hdel(self.unacked_key, tag)
+            if P:
+                M, EX, RK = loads(bytes_to_str(P))  # json is unicode
+                await self._do_restore_message(M, EX, RK, pipe, leftmost)
+
+        with self.conn_or_acquire() as client:
+            await client.transaction(restore_transaction, self.unacked_key)
+
+    async def _restore_at_beginning(self, message):
+        return await self._restore(message, leftmost=True)
+
+    def _get_response_error(self):
+        from aioredis import exceptions
+        return exceptions.ResponseError
+
+    async def _get(self, queue):
+        with self.conn_or_acquire() as client:
+            for pri in self.priority_steps:
+                item = await client.rpop(self._q_for_pri(queue, pri))
+                if item:
+                    return loads(bytes_to_str(item))
+            raise Empty()
+
+    async def _size(self, queue):
+        with self.conn_or_acquire() as client:
+            async with client.pipeline() as pipe:
+                for pri in self.priority_steps:
+                    pipe = pipe.llen(self._q_for_pri(queue, pri))
+                sizes = await pipe.execute()
+        return sum(size for size in sizes
+                   if isinstance(size, numbers.Integral))
+
+    async def _put(self, queue, message, **kwargs):
+        """Deliver message."""
+        pri = self._get_message_priority(message, reverse=False)
+
+        with self.conn_or_acquire() as client:
+            await client.lpush(self._q_for_pri(queue, pri), dumps(message))
+
+    async def _put_fanout(self, exchange, message, routing_key, **kwargs):
+        """Deliver fanout message."""
+        with self.conn_or_acquire() as client:
+            await client.publish(
+                self._get_publish_topic(exchange, routing_key),
+                dumps(message),
+            )
+
+    async def _queue_bind(self, exchange, routing_key, pattern, queue):
+        if self.typeof(exchange).type == 'fanout':
+            # Mark exchange as fanout.
+            self._fanout_queues[queue] = (
+                exchange, routing_key.replace('#', '*'),
+            )
+        with self.conn_or_acquire() as client:
+            await client.sadd(
+                self.keyprefix_queue % (exchange,),
+                self.sep.join([routing_key or '', pattern or '', queue or ''])
+            )
+
+    async def _delete(self, queue, exchange, routing_key, pattern, *args, **kwargs):
+        self.auto_delete_queues.discard(queue)
+        with self.conn_or_acquire(client=kwargs.get('client')) as client:
+            await client.srem(self.keyprefix_queue % (exchange,),
+                        self.sep.join([routing_key or '',
+                                       pattern or '',
+                                       queue or '']))
+            async with client.pipeline() as pipe:
+                for pri in self.priority_steps:
+                    pipe = pipe.delete(self._q_for_pri(queue, pri))
+                await pipe.execute()
+
+    async def _has_queue(self, queue, **kwargs):
+        with self.conn_or_acquire() as client:
+            async with client.pipeline() as pipe:
+                for pri in self.priority_steps:
+                    pipe = pipe.exists(self._q_for_pri(queue, pri))
+                return any(await pipe.execute())
+
+    async def get_table(self, exchange):
+        key = self.keyprefix_queue % exchange
+        with self.conn_or_acquire() as client:
+            values = await client.smembers(key)
+            if not values:
+                # table does not exists since all queues bound to the exchange
+                # were deleted. We need just return empty list.
+                return []
+            return [tuple(bytes_to_str(val).split(self.sep)) for val in values]
+
+    async def _purge(self, queue):
+        with self.conn_or_acquire() as client:
+            async with client.pipeline() as pipe:
+                for pri in self.priority_steps:
+                    priq = self._q_for_pri(queue, pri)
+                    pipe = pipe.llen(priq).delete(priq)
+                sizes = await pipe.execute()
+                return sum(sizes[::2])
+
+    async def close(self):
+        self._closing = True
+        if not self.closed:
+            # remove from channel poller.
+            self.connection.cycle.discard(self)
+
+            # delete fanout bindings
+            client = self.__dict__.get('client')  # only if property cached
+            if client is not None:
+                for queue in self._fanout_queues:
+                    if queue in self.auto_delete_queues:
+                        await self.queue_delete(queue, client=client)
+            await self._disconnect_pools()
+            await self._close_clients()
+
+            # --------------------------------------
+            # virtual.base::Channel
+            self.closed = True
+
+            for consumer in list(self._consumers):
+                self.basic_cancel(consumer)  # todo maybe await
+            if self._qos:
+                self._qos.restore_unacked_once()
+            if self._cycle is not None:
+                self._cycle.close()
+                self._cycle = None
+            if self.connection is not None:
+                self.connection.close_channel(self)  # todo maybe await
+        self.exchange_types = None
+
+    async def _close_clients(self):
+        for attr in 'client', 'subclient':
+            try:
+                client = self.__dict__[attr]
+                connection, client.connection = client.connection, None
+                await connection.disconnect()
+            except (KeyError, AttributeError, self.ResponseError):
+                pass
+
+    def _connparams(self, asynchronous=False):
+        params = super(Channel, self)._connparams(asynchronous)
+        channel = self
+
+        if asynchronous:
+            class Connection(self.connection_class):
+                async def disconnect(self):
+                    await super().disconnect()
+                    channel._on_connection_disconnect(self)
+
+            params['connection_class'] = Connection
+        return params
+
+    def _get_pool(self, asynchronous=True):
+        params = self._connparams(asynchronous=True)
+        self.keyprefix_fanout = self.keyprefix_fanout.format(db=params['db'])
+        return aioredis.ConnectionPool(**params)
+
+    def _get_client(self):
+        if getattr(aioredis, 'VERSION', (1, 0)) < (2, 0, 0):
+            raise VersionMismatch(
+                'Redis transport requires aioredis versions 2.0.0 or later. '
+                f'You have {aioredis.__version__}')
+
+        if self.global_keyprefix:
+            return functools.partial(
+                PrefixedStrictRedis,
+                global_keyprefix=self.global_keyprefix,
+            )
+        return aioredis.StrictRedis
+
+    # -----------------------------------------------------------------------------
+    # virtual.base::Channel method overload
+    async def queue_delete(self, queue, if_unused=False, if_empty=False, **kwargs):
+        """Delete queue."""
+        if if_empty and self._size(queue):
+            return
+        for exchange, routing_key, args in self.state.queue_bindings(queue):
+            meta = self.typeof(exchange).prepare_bind(
+                queue, exchange, routing_key, args,
+            )
+            await self._delete(queue, exchange, *meta, **kwargs)
+        self.state.queue_bindings_delete(queue)
+
+    async def after_reply_message_received(self, queue):
+        await self.queue_delete(queue)
+
+    async def queue_bind(self, queue, exchange=None, routing_key='',
+                   arguments=None, **kwargs):
+        """Bind `queue` to `exchange` with `routing key`."""
+        exchange = exchange or 'amq.direct'
+        if self.state.has_binding(queue, exchange, routing_key):
+            return
+        # Add binding:
+        self.state.binding_declare(queue, exchange, routing_key, arguments)
+        # Update exchange's routing table:
+        table = self.state.exchanges[exchange].setdefault('table', [])
+        meta = self.typeof(exchange).prepare_bind(
+            queue, exchange, routing_key, arguments,
+        )
+        table.append(meta)
+        if self.supports_fanout:
+            await self._queue_bind(exchange, *meta)
+
+    async def queue_unbind(self, queue, exchange=None, routing_key='',
+                     arguments=None, **kwargs):
+        # Remove queue binding:
+        self.state.binding_delete(queue, exchange, routing_key)
+        try:
+            table = await self.get_table(exchange)
+        except KeyError:
+            return
+        binding_meta = self.typeof(exchange).prepare_bind(
+            queue, exchange, routing_key, arguments,
+        )
+        # TODO: the complexity of this operation is O(number of bindings).
+        # Should be optimized.  Modifying table in place.
+        table[:] = [meta for meta in table if meta != binding_meta]
+
+    async def list_bindings(self):
+        return ((queue, exchange, rkey)
+                for exchange in self.state.exchanges
+                for rkey, pattern, queue in await self.get_table(exchange))
+
+    async def queue_declare(self, queue=None, passive=False, **kwargs):
+        """Declare queue."""
+        queue = queue or 'amq.gen-%s' % uuid()
+        if passive and not (await self._has_queue(queue, **kwargs)):
+            raise ChannelError(
+                'NOT_FOUND - no queue {!r} in vhost {!r}'.format(
+                    queue, self.connection.client.virtual_host or '/'),
+                (50, 10), 'Channel.queue_declare', '404',
+            )
+        else:
+            self._new_queue(queue, **kwargs)
+        return queue_declare_ok_t(queue, await self._size(queue), 0)
+
+    async def queue_purge(self, queue, **kwargs):
+        """Remove all ready messages from queue."""
+        return await self._purge(queue)
+
+    async def basic_publish(self, message, exchange, routing_key, **kwargs):
+        """Publish message."""
+        self._inplace_augment_message(message, exchange, routing_key)
+        if exchange:
+            return await self.typeof(exchange).deliver(
+                message, exchange, routing_key, **kwargs
+            )
+        # anon exchange: routing_key is the destination queue
+        return await self._put(routing_key, message, **kwargs)
+
+    async def basic_get(self, queue, no_ack=False, **kwargs):
+        """Get message by direct access (synchronous)."""
+        try:
+            message = self.Message((await self._get(queue)), channel=self)
+            if not no_ack:
+                self.qos.append(message, message.delivery_tag)
+            return message
+        except Empty:
+            pass
+
+    async def _lookup(self, exchange, routing_key, default=None):
+        """Find all queues matching `routing_key` for the given `exchange`.
+
+        Returns:
+            str: queue name -- must return the string `default`
+                if no queues matched.
+        """
+        if default is None:
+            default = self.deadletter_queue
+        if not exchange:  # anon exchange
+            return [routing_key or default]
+
+        try:
+            R = self.typeof(exchange).lookup(
+                await self.get_table(exchange),
+                exchange, routing_key, default,
+            )
+        except KeyError:
+            R = []
+
+        if not R and default is not None:
+            warnings.warn(UndeliverableWarning(UNDELIVERABLE_FMT.format(
+                exchange=exchange, routing_key=routing_key)),
+            )
+            self._new_queue(default)
+            R = [default]
+        return R
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.close()
+
+    def __enter__(self):
+        raise NotImplementedError
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        raise NotImplementedError
+
+    def _reset_cycle(self):
+        self._cycle = AsyncFairCycle(
+            self._get_and_deliver, self._active_queues, Empty)
+
+    async def _get_and_deliver(self, queue, callback):
+        message = await self._get(queue)
+        callback(message, queue)
+
+    # -----------------------------------------------------------------------------
+    # exchange
+    async def exchange_delete(self, exchange, if_unused=False, nowait=False):
+        """Delete `exchange` and all its bindings."""
+        for rkey, _, queue in (await self.get_table(exchange)):
+            await self.queue_delete(queue, if_unused=True, if_empty=True)
+        self.state.exchanges.pop(exchange, None)
+
+    # -----------------------------------------------------------------------------
+    # consumer
+    async def _brpop_start(self, timeout=1):
+        queues = self._queue_cycle.consume(len(self.active_queues))
+        if not queues:
+            return
+
+        keys = [self._q_for_pri(queue, pri) for pri in self.priority_steps
+                for queue in queues] + [timeout or 0]
+
+        command_args = ['BRPOP', *keys]
+        if self.global_keyprefix:
+            command_args = self.client._prefix_args(command_args)
+
+        async def brpop(conn):
+            await conn.send_command(*command_args)
+            return await self._brpop_read_impl()
+
+        self._in_poll = True
+        self._brpop_task = task = asyncio.create_task(
+            brpop(self.client.connection))
+
+        await asyncio.sleep(0)
+        return task
+
+    async def _brpop_read_impl(self, **options):
+        try:
+            dest__item = await self.client.parse_response(
+                self.client.connection,
+                'BRPOP',
+                **options
+            )
+        except self.connection_errors:
+            # if there's a ConnectionError, disconnect so the next
+            # iteration will reconnect automatically.
+            await self.client.connection.disconnect()
+            raise
+        if dest__item:
+            dest, item = dest__item
+            dest = bytes_to_str(dest).rsplit(self.sep, 1)[0]
+            self._queue_cycle.rotate(dest)
+            self.connection._deliver(loads(bytes_to_str(item)), dest)
+            return True
+        else:
+            raise Empty()
+
+    def _brpop_read(self, **options):
+        try:
+            return self._brpop_task.result()
+        finally:
+            self._brpop_task = None
+            self._in_poll = None
+
+    async def _subscribe(self):
+        keys = [self._get_subscribe_topic(queue)
+                for queue in self.active_fanout_queues]
+        if not keys:
+            return
+        c = self.subclient
+        if not c.connection.is_connected:
+            await c.connection.connect()
+        self._in_listen = c.connection
+        await c.psubscribe(keys)
+        self._listen_task = t = asyncio.create_task(c.parse_response())
+        await asyncio.sleep(0)
+        return t
+
+    async def _unsubscribe_from(self, queue):
+        topic = self._get_subscribe_topic(queue)
+        c = self.subclient
+        if c.connection and c.connection.is_connected:
+            await c.unsubscribe([topic])
+
+    def _receive_one(self, c):
+        try:
+            response = self._listen_task.result()
+        except self.connection_errors:
+            self._in_listen = None
+            raise
+        finally:
+            self._listen_task = None
+        if isinstance(response, (list, tuple)):
+            payload = self._handle_message(c, response)
+            if bytes_to_str(payload['type']).endswith('message'):
+                channel = bytes_to_str(payload['channel'])
+                if payload['data']:
+                    if channel[0] == '/':
+                        _, _, channel = channel.partition('.')
+                    try:
+                        message = loads(bytes_to_str(payload['data']))
+                    except (TypeError, ValueError):
+                        warn('Cannot process event on channel %r: %s',
+                             channel, repr(payload)[:4096], exc_info=1)
+                        raise Empty()
+                    exchange = channel.split('/', 1)[0]
+                    self.connection._deliver(
+                        message, self._fanout_to_queue[exchange])
+                    return True
+
+
+class MultiChannelPoller(SyncMultiChannelPoller):
+    def __init__(self):
+        self._channels = set()
+        self._pending_tasks = set()
+
+    @staticmethod
+    async def ensure_connection(client):
+        conn = getattr(client, 'connection', None)
+        if conn is None:
+            client.connection = await client.connection_pool.get_connection('_')
+        elif not conn.is_connected:
+            await client.connection.connect()
+
+    async def _register_BRPOP(self, channel):
+        """Enable BRPOP mode for channel."""
+        await self.ensure_connection(channel.client)
+
+        if not channel._in_poll:  # send BRPOP
+            task = await channel._brpop_start()
+            task.channel = channel
+            task.cmd = 'BRPOP'
+            self._pending_tasks.add(task)
+
+    async def _register_LISTEN(self, channel):
+        """Enable LISTEN mode for channel."""
+        await self.ensure_connection(channel.client)
+
+        if not channel._in_listen:
+            task = await channel._subscribe()  # send SUBSCR
+            task.channel = channel
+            task.cmd = 'LISTEN'
+            self._pending_tasks.add(task)
+
+    async def poll(self, timeout):
+        if not self._pending_tasks:
+            return
+
+        done, pending = await asyncio.wait(
+            self._pending_tasks,
+            timeout=timeout,
+            return_when=asyncio.FIRST_COMPLETED
+        )
+        for task in done:
+            self._pending_tasks.discard(task)
+        if not done:
+            return
+        else:
+            return done.pop()
+
+    @staticmethod
+    async def handle_task(task):
+        chan = task.channel  # noqa
+        type = task.cmd  # noqa
+
+        if chan.qos.can_consume():
+            hdlr = chan.handlers[type]
+            if is_async_callable(hdlr):
+                await hdlr()
+            else:
+                hdlr()
+
+        return True
+
+    async def get(self, callback, timeout=None):
+        self._in_protected_read = True
+        try:
+            for channel in self._channels:
+                if channel.active_queues:           # BRPOP mode?
+                    if channel.qos.can_consume():
+                        await self._register_BRPOP(channel)
+                if channel.active_fanout_queues:    # LISTEN mode?
+                    self._register_LISTEN(channel)
+
+            if (
+                (done_task := await self.poll(timeout))
+                and (await self.handle_task(done_task))
+            ):
+                return
+            # - no new data, so try to restore messages.
+            # - reset active redis commands.
+            await self.maybe_restore_messages()
+            raise Empty()
+        finally:
+            self._in_protected_read = False
+            while self.after_read:
+                try:
+                    fun = self.after_read.pop()
+                except KeyError:
+                    break
+                else:
+                    fun()
+
+    async def maybe_restore_messages(self):
+        for channel in self._channels:
+            if channel.active_queues:
+                # only need to do this once, as they are not local to channel.
+                return await channel.qos.restore_visible(
+                    num=channel.unacked_restore_limit,
+                )
+
+
+class Transport(SyncTransport):
+    Channel = Channel
+    connection_errors, channel_errors = get_redis_error_classes()
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # All channels share the same poller.
+        self.cycle = MultiChannelPoller()
+
+    async def establish_connection(self):
+        channel: Channel = self.create_channel(self)
+        await channel.ping()
+        self._avail_channels.append(channel)
+        return self     # for drain events
+
+    async def close_connection(self, connection):
+        self.cycle.close()
+        for chan_list in self._avail_channels, self.channels:
+            while chan_list:
+                try:
+                    channel = chan_list.pop()
+                except LookupError:  # pragma: no cover
+                    pass
+                else:
+                    await channel.close()
+
+    async def drain_events(self, connection, timeout=None):
+        time_start = monotonic()
+        get = self.cycle.get
+        polling_interval = self.polling_interval
+        if timeout and polling_interval and polling_interval > timeout:
+            polling_interval = timeout
+        while 1:
+            try:
+                await get(self._deliver, timeout=timeout)
+            except Empty:
+                if timeout is not None and monotonic() - time_start >= timeout:
+                    raise socket.timeout()
+                if polling_interval is not None:
+                    await asyncio.sleep(polling_interval)
+            else:
+                break
+
+
+class SentinelManagedSSLConnection(
+        sentinel.SentinelManagedConnection,
+        aioredis.SSLConnection):
+    pass
+
+
+class SentinelChannel(Channel):
+    from_transport_options = Channel.from_transport_options + (
+        'master_name',
+        'min_other_sentinels',
+        'sentinel_kwargs')
+
+    connection_class = sentinel.SentinelManagedConnection
+    connection_class_ssl = SentinelManagedSSLConnection
+
+    def _sentinel_managed_pool(self, asynchronous=False):
+        connparams = self._connparams(asynchronous)
+
+        additional_params = connparams.copy()
+
+        additional_params.pop('host', None)
+        additional_params.pop('port', None)
+
+        sentinels = []
+        for url in self.connection.client.alt:
+            url = _parse_url(url)
+            if url.scheme == 'sentinel':
+                port = url.port or self.connection.default_port
+                sentinels.append((url.hostname, port))
+
+        # Fallback for when only one sentinel is provided.
+        if not sentinels:
+            sentinels.append((connparams['host'], connparams['port']))
+
+        sentinel_inst = sentinel.Sentinel(
+            sentinels,
+            min_other_sentinels=getattr(self, 'min_other_sentinels', 0),
+            sentinel_kwargs=getattr(self, 'sentinel_kwargs', None),
+            **additional_params)
+
+        master_name = getattr(self, 'master_name', None)
+
+        if master_name is None:
+            raise ValueError(
+                "'master_name' transport option must be specified."
+            )
+
+        return sentinel_inst.master_for(
+            master_name,
+            self.Client,
+        ).connection_pool
+
+    def _get_pool(self, asynchronous=False):
+        return self._sentinel_managed_pool(asynchronous)
+
+
+class SentinelTransport(Transport):
+    """Redis Sentinel Transport."""
+
+    default_port = 26379
+    Channel = SentinelChannel
```

### Comparing `deepfos-celery-1.0.2/celery/aio/transport.py` & `deepfos-celery-1.0.3/celery/aio/transport.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/aio/utils.py` & `deepfos-celery-1.0.3/celery/aio/utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-import asyncio
-import collections
-
-from asyncio import sleep
-from time import time
-from itertools import count
-from contextlib import asynccontextmanager
-from inspect import isfunction, iscoroutinefunction, ismethod
-
-from kombu.utils.functional import (
-    fxrange,
-    lazy,
-    ChannelPromise
-)
-from kombu.resource import Resource as SyncResource
-
-
-def is_async_callable(fun):
-    if not callable(fun):
-        return False
-
-    if isfunction(fun) or ismethod(fun):
-        return iscoroutinefunction(fun)
-
-    return iscoroutinefunction(fun.__call__)
-
-
-class LifoQueue(asyncio.LifoQueue):
-    @property
-    def queue(self):
-        return self._queue
-
-    def _init(self, maxsize):
-        self._queue = collections.deque()
-
-
-async def retry_over_time(
-    fun, catch, args=None, kwargs=None, errback=None,
-    max_retries=None, interval_start=2, interval_step=2,
-    interval_max=30, callback=None, timeout=None
-):
-    """async version of kombu.util.functional: retry_over_time"""
-    kwargs = {} if not kwargs else kwargs
-    args = [] if not args else args
-    interval_range = fxrange(interval_start,
-                             interval_max + interval_start,
-                             interval_step, repeatlast=True)
-    end = time() + timeout if timeout else None
-    errback_is_coro = errback and is_async_callable(errback)
-    cb_is_coro = callback and is_async_callable(callback)
-
-    for retries in count():
-        try:
-            return await fun(*args, **kwargs)
-        except catch as exc:
-            if max_retries is not None and retries >= max_retries:
-                raise
-            if end and time() > end:
-                raise
-            if callback:
-                if cb_is_coro:
-                    await callback()
-                else:
-                    callback()
-
-            if errback:
-                if errback_is_coro:
-                    interval = await errback(exc, interval_range, retries)
-                else:
-                    interval = errback(exc, interval_range, retries)
-                tts = float(interval)
-            else:
-                tts = next(interval_range)
-
-            if tts:
-                for _ in range(int(tts)):
-                    if callback:
-                        if cb_is_coro:
-                            await callback()
-                        else:
-                            callback()
-                    await sleep(1.0)
-                # sleep remainder after int truncation above.
-                await sleep(abs(int(tts) - tts))
-
-
-class Resource(SyncResource):
-    def __init__(self, limit=None, preload=None, close_after_fork=None):
-        self._limit = limit
-        self.preload = preload or 0
-        self._closed = False
-        self.close_after_fork = (
-            close_after_fork
-            if close_after_fork is not None else self.close_after_fork
-        )
-
-        self._resource = LifoQueue()
-        self._dirty = set()
-        self.setup()
-
-    def new(self):
-        raise NotImplementedError
-
-    async def get(self, block=False, timeout=None):
-        """Acquire resource.
-
-        Arguments:
-            block (bool): If the limit is exceeded,
-                then block until there is an available item.
-            timeout (float): Timeout to wait
-                if ``block`` is true.  Default is :const:`None` (forever).
-
-        Raises:
-            LimitExceeded: if block is false and the limit has been exceeded.
-        """
-        if self._closed:
-            raise RuntimeError('Acquire on closed pool')
-        if self.limit:
-            while 1:
-                try:
-                    if not block:
-                        R = self._resource.get_nowait()
-                    elif timeout is not None:
-                        R = await asyncio.wait_for(
-                            self._resource.get(),
-                            timeout=timeout
-                        )
-                    else:
-                        R = await self._resource.get()
-                except asyncio.QueueEmpty:
-                    self._add_when_empty()
-                else:
-                    try:
-                        R = await self.prepare(R)
-                    except BaseException:
-                        if isinstance(R, async_lazy):
-                            # not evaluated yet, just put it back
-                            self._resource.put_nowait(R)
-                        else:
-                            # evaluted so must try to release/close first.
-                            await self.release(R)
-                        raise
-                    self._dirty.add(R)
-                    break
-        else:
-            R = await self.prepare(self.new())
-
-        async def release():
-            """Release resource so it can be used by another thread.
-
-            Warnings:
-                The caller is responsible for discarding the object,
-                and to never use the resource again.  A new resource must
-                be acquired if so needed.
-            """
-            await self.release(R)
-        R.release = release
-
-        return R
-
-    @asynccontextmanager
-    async def acquire(self, block=False, timeout=None):
-        R = await self.get(block, timeout)
-        try:
-            yield R
-        finally:
-            await self.release(R)
-
-    async def release_resource(self, resource):
-        pass
-
-    async def release(self, resource):
-        if self.limit:
-            self._dirty.discard(resource)
-            self._resource.put_nowait(resource)
-            await self.release_resource(resource)
-        else:
-            await self.close_resource(resource)
-
-    async def close_resource(self, resource):
-        await resource.close()
-
-    async def prepare(self, resource):
-        return resource
-
-
-class async_lazy(lazy):
-    async def __call__(self):
-        return await self.evaluate()
-
-    async def evaluate(self):
-        return await self._fun(*self._args, **self._kwargs)
-
-
-async def maybe_async_evaluate(value):
-    """Evaluate value only if value is a :class:`lazy` instance."""
-    if isinstance(value, async_lazy):
-        return await value.evaluate()
-    return value
-
-
-class AsyncChannelPromise(ChannelPromise):
-
-    async def __call__(self):
-        try:
-            return self.__value__
-        except AttributeError:
-            value = self.__value__ = await self.__contract__()
-            return value
+import asyncio
+import collections
+
+from asyncio import sleep
+from time import time
+from itertools import count
+from contextlib import asynccontextmanager
+from inspect import isfunction, iscoroutinefunction, ismethod
+
+from kombu.utils.functional import (
+    fxrange,
+    lazy,
+    ChannelPromise
+)
+from kombu.resource import Resource as SyncResource
+
+
+def is_async_callable(fun):
+    if not callable(fun):
+        return False
+
+    if isfunction(fun) or ismethod(fun):
+        return iscoroutinefunction(fun)
+
+    return iscoroutinefunction(fun.__call__)
+
+
+class LifoQueue(asyncio.LifoQueue):
+    @property
+    def queue(self):
+        return self._queue
+
+    def _init(self, maxsize):
+        self._queue = collections.deque()
+
+
+async def retry_over_time(
+    fun, catch, args=None, kwargs=None, errback=None,
+    max_retries=None, interval_start=2, interval_step=2,
+    interval_max=30, callback=None, timeout=None
+):
+    """async version of kombu.util.functional: retry_over_time"""
+    kwargs = {} if not kwargs else kwargs
+    args = [] if not args else args
+    interval_range = fxrange(interval_start,
+                             interval_max + interval_start,
+                             interval_step, repeatlast=True)
+    end = time() + timeout if timeout else None
+    errback_is_coro = errback and is_async_callable(errback)
+    cb_is_coro = callback and is_async_callable(callback)
+
+    for retries in count():
+        try:
+            return await fun(*args, **kwargs)
+        except catch as exc:
+            if max_retries is not None and retries >= max_retries:
+                raise
+            if end and time() > end:
+                raise
+            if callback:
+                if cb_is_coro:
+                    await callback()
+                else:
+                    callback()
+
+            if errback:
+                if errback_is_coro:
+                    interval = await errback(exc, interval_range, retries)
+                else:
+                    interval = errback(exc, interval_range, retries)
+                tts = float(interval)
+            else:
+                tts = next(interval_range)
+
+            if tts:
+                for _ in range(int(tts)):
+                    if callback:
+                        if cb_is_coro:
+                            await callback()
+                        else:
+                            callback()
+                    await sleep(1.0)
+                # sleep remainder after int truncation above.
+                await sleep(abs(int(tts) - tts))
+
+
+class Resource(SyncResource):
+    def __init__(self, limit=None, preload=None, close_after_fork=None):
+        self._limit = limit
+        self.preload = preload or 0
+        self._closed = False
+        self.close_after_fork = (
+            close_after_fork
+            if close_after_fork is not None else self.close_after_fork
+        )
+
+        self._resource = LifoQueue()
+        self._dirty = set()
+        self.setup()
+
+    def new(self):
+        raise NotImplementedError
+
+    async def get(self, block=False, timeout=None):
+        """Acquire resource.
+
+        Arguments:
+            block (bool): If the limit is exceeded,
+                then block until there is an available item.
+            timeout (float): Timeout to wait
+                if ``block`` is true.  Default is :const:`None` (forever).
+
+        Raises:
+            LimitExceeded: if block is false and the limit has been exceeded.
+        """
+        if self._closed:
+            raise RuntimeError('Acquire on closed pool')
+        if self.limit:
+            while 1:
+                try:
+                    if not block:
+                        R = self._resource.get_nowait()
+                    elif timeout is not None:
+                        R = await asyncio.wait_for(
+                            self._resource.get(),
+                            timeout=timeout
+                        )
+                    else:
+                        R = await self._resource.get()
+                except asyncio.QueueEmpty:
+                    self._add_when_empty()
+                else:
+                    try:
+                        R = await self.prepare(R)
+                    except BaseException:
+                        if isinstance(R, async_lazy):
+                            # not evaluated yet, just put it back
+                            self._resource.put_nowait(R)
+                        else:
+                            # evaluted so must try to release/close first.
+                            await self.release(R)
+                        raise
+                    self._dirty.add(R)
+                    break
+        else:
+            R = await self.prepare(self.new())
+
+        async def release():
+            """Release resource so it can be used by another thread.
+
+            Warnings:
+                The caller is responsible for discarding the object,
+                and to never use the resource again.  A new resource must
+                be acquired if so needed.
+            """
+            await self.release(R)
+        R.release = release
+
+        return R
+
+    @asynccontextmanager
+    async def acquire(self, block=False, timeout=None):
+        R = await self.get(block, timeout)
+        try:
+            yield R
+        finally:
+            await self.release(R)
+
+    async def release_resource(self, resource):
+        pass
+
+    async def release(self, resource):
+        if self.limit:
+            self._dirty.discard(resource)
+            self._resource.put_nowait(resource)
+            await self.release_resource(resource)
+        else:
+            await self.close_resource(resource)
+
+    async def close_resource(self, resource):
+        await resource.close()
+
+    async def prepare(self, resource):
+        return resource
+
+
+class async_lazy(lazy):
+    async def __call__(self):
+        return await self.evaluate()
+
+    async def evaluate(self):
+        return await self._fun(*self._args, **self._kwargs)
+
+
+async def maybe_async_evaluate(value):
+    """Evaluate value only if value is a :class:`lazy` instance."""
+    if isinstance(value, async_lazy):
+        return await value.evaluate()
+    return value
+
+
+class AsyncChannelPromise(ChannelPromise):
+
+    async def __call__(self):
+        try:
+            return self.__value__
+        except AttributeError:
+            value = self.__value__ = await self.__contract__()
+            return value
```

### Comparing `deepfos-celery-1.0.2/celery/app/__init__.py` & `deepfos-celery-1.0.3/celery/app/__init__.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/amqp.py` & `deepfos-celery-1.0.3/celery/app/amqp.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/annotations.py` & `deepfos-celery-1.0.3/celery/app/annotations.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/autoretry.py` & `deepfos-celery-1.0.3/celery/app/autoretry.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/backends.py` & `deepfos-celery-1.0.3/celery/app/backends.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/base.py` & `deepfos-celery-1.0.3/celery/app/base.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,1539 +1,1539 @@
-"""Actual App instance implementation."""
-import inspect
-import os
-import sys
-import threading
-import warnings
-from collections import UserDict, defaultdict, deque
-from contextlib import asynccontextmanager
-from datetime import datetime
-from operator import attrgetter
-
-from click.exceptions import Exit
-from kombu import pools
-from kombu.clocks import LamportClock
-from kombu.common import oid_from
-from kombu.utils.compat import register_after_fork
-from kombu.utils.objects import cached_property
-from kombu.utils.uuid import uuid
-from vine import starpromise
-
-from celery import platforms, signals
-from celery._state import (_announce_app_finalized, _deregister_app,
-                           _register_app, _set_current_app, _task_stack,
-                           connect_on_app_finalize, get_current_app,
-                           get_current_worker_task, set_default_app)
-from celery.exceptions import AlwaysEagerIgnored, ImproperlyConfigured
-from celery.loaders import get_loader_cls
-from celery.local import PromiseProxy, maybe_evaluate
-from celery.utils import abstract
-from celery.utils.collections import AttributeDictMixin
-from celery.utils.dispatch import Signal
-from celery.utils.functional import first, head_from_fun, maybe_list
-from celery.utils.imports import gen_task_name, instantiate, symbol_by_name
-from celery.utils.log import get_logger
-from celery.utils.objects import (FallbackContext,
-                                  mro_lookup,
-                                  AsyncFallbackContext)
-from celery.utils.time import timezone, to_utc
-
-# Load all builtin tasks
-from . import builtins  # noqa
-from . import backends
-from .annotations import prepare as prepare_annotations
-from .autoretry import add_autoretry_behaviour
-from .defaults import DEFAULT_SECURITY_DIGEST, find_deprecated_settings
-from .registry import TaskRegistry
-from .utils import (AppPickler, Settings, _new_key_to_old, _old_key_to_new,
-                    _unpickle_app, _unpickle_app_v2, appstr, bugreport,
-                    detect_settings)
-
-__all__ = ('Celery',)
-
-logger = get_logger(__name__)
-
-BUILTIN_FIXUPS = {
-    'celery.fixups.django:fixup',
-}
-USING_EXECV = os.environ.get('FORKED_BY_MULTIPROCESSING')
-
-ERR_ENVVAR_NOT_SET = """
-The environment variable {0!r} is not set,
-and as such the configuration could not be loaded.
-
-Please set this variable and make sure it points to
-a valid configuration module.
-
-Example:
-    {0}="proj.celeryconfig"
-"""
-
-
-def app_has_custom(app, attr):
-    """Return true if app has customized method `attr`.
-
-    Note:
-        This is used for optimizations in cases where we know
-        how the default behavior works, but need to account
-        for someone using inheritance to override a method/property.
-    """
-    return mro_lookup(app.__class__, attr, stop={Celery, object},
-                      monkey_patched=[__name__])
-
-
-def _unpickle_appattr(reverse_name, args):
-    """Unpickle app."""
-    # Given an attribute name and a list of args, gets
-    # the attribute from the current app and calls it.
-    return get_current_app()._rgetattr(reverse_name)(*args)
-
-
-def _after_fork_cleanup_app(app):
-    # This is used with multiprocessing.register_after_fork,
-    # so need to be at module level.
-    try:
-        app._after_fork()
-    except Exception as exc:  # pylint: disable=broad-except
-        logger.info('after forker raised exception: %r', exc, exc_info=1)
-
-
-class PendingConfiguration(UserDict, AttributeDictMixin):
-    # `app.conf` will be of this type before being explicitly configured,
-    # meaning the app can keep any configuration set directly
-    # on `app.conf` before the `app.config_from_object` call.
-    #
-    # accessing any key will finalize the configuration,
-    # replacing `app.conf` with a concrete settings object.
-
-    callback = None
-    _data = None
-
-    def __init__(self, conf, callback):
-        object.__setattr__(self, '_data', conf)
-        object.__setattr__(self, 'callback', callback)
-
-    def __setitem__(self, key, value):
-        self._data[key] = value
-
-    def clear(self):
-        self._data.clear()
-
-    def update(self, *args, **kwargs):
-        self._data.update(*args, **kwargs)
-
-    def setdefault(self, *args, **kwargs):
-        return self._data.setdefault(*args, **kwargs)
-
-    def __contains__(self, key):
-        # XXX will not show finalized configuration
-        # setdefault will cause `key in d` to happen,
-        # so for setdefault to be lazy, so does contains.
-        return key in self._data
-
-    def __len__(self):
-        return len(self.data)
-
-    def __repr__(self):
-        return repr(self.data)
-
-    @cached_property
-    def data(self):
-        return self.callback()
-
-
-class Celery:
-    """Celery application.
-
-    Arguments:
-        main (str): Name of the main module if running as `__main__`.
-            This is used as the prefix for auto-generated task names.
-
-    Keyword Arguments:
-        broker (str): URL of the default broker used.
-        backend (Union[str, Type[celery.backends.base.Backend]]):
-            The result store backend class, or the name of the backend
-            class to use.
-
-            Default is the value of the :setting:`result_backend` setting.
-        autofinalize (bool): If set to False a :exc:`RuntimeError`
-            will be raised if the task registry or tasks are used before
-            the app is finalized.
-        set_as_current (bool):  Make this the global current app.
-        include (List[str]): List of modules every worker should import.
-
-        amqp (Union[str, Type[AMQP]]): AMQP object or class name.
-        events (Union[str, Type[celery.app.events.Events]]): Events object or
-            class name.
-        log (Union[str, Type[Logging]]): Log object or class name.
-        control (Union[str, Type[celery.app.control.Control]]): Control object
-            or class name.
-        tasks (Union[str, Type[TaskRegistry]]): A task registry, or the name of
-            a registry class.
-        fixups (List[str]): List of fix-up plug-ins (e.g., see
-            :mod:`celery.fixups.django`).
-        config_source (Union[str, class]): Take configuration from a class,
-            or object.  Attributes may include any settings described in
-            the documentation.
-        task_cls (Union[str, Type[celery.app.task.Task]]): base task class to
-            use. See :ref:`this section <custom-task-cls-app-wide>` for usage.
-    """
-
-    #: This is deprecated, use :meth:`reduce_keys` instead
-    Pickler = AppPickler
-
-    SYSTEM = platforms.SYSTEM
-    IS_macOS, IS_WINDOWS = platforms.IS_macOS, platforms.IS_WINDOWS
-
-    #: Name of the `__main__` module.  Required for standalone scripts.
-    #:
-    #: If set this will be used instead of `__main__` when automatically
-    #: generating task names.
-    main = None
-
-    #: Custom options for command-line programs.
-    #: See :ref:`extending-commandoptions`
-    user_options = None
-
-    #: Custom bootsteps to extend and modify the worker.
-    #: See :ref:`extending-bootsteps`.
-    steps = None
-
-    builtin_fixups = BUILTIN_FIXUPS
-
-    amqp_cls = 'celery.app.amqp:AMQP'
-    backend_cls = None
-    events_cls = 'celery.app.events:Events'
-    loader_cls = None
-    log_cls = 'celery.app.log:Logging'
-    control_cls = 'celery.app.control:Control'
-    task_cls = 'celery.app.task:Task'
-    registry_cls = 'celery.app.registry:TaskRegistry'
-
-    #: Thread local storage.
-    _local = None
-    _fixups = None
-    _pool = None
-    _conf = None
-    _after_fork_registered = False
-
-    #: Signal sent when app is loading configuration.
-    on_configure = None
-
-    #: Signal sent after app has prepared the configuration.
-    on_after_configure = None
-
-    #: Signal sent after app has been finalized.
-    on_after_finalize = None
-
-    #: Signal sent by every new process after fork.
-    on_after_fork = None
-
-    def __init__(self, main=None, loader=None, backend=None,
-                 amqp=None, events=None, log=None, control=None,
-                 set_as_current=True, tasks=None, broker=None, include=None,
-                 changes=None, config_source=None, fixups=None, task_cls=None,
-                 autofinalize=True, namespace=None, strict_typing=True,
-                 aio_control=None,
-                 **kwargs):
-
-        self._local = threading.local()
-
-        self.clock = LamportClock()
-        self.main = main
-        self.amqp_cls = amqp or self.amqp_cls
-        self.events_cls = events or self.events_cls
-        self.loader_cls = loader or self._get_default_loader()
-        self.log_cls = log or self.log_cls
-        self.control_cls = control or self.control_cls
-        self.aio_control_cls = aio_control or self.aio_control_cls
-        self.task_cls = task_cls or self.task_cls
-        self.set_as_current = set_as_current
-        self.registry_cls = symbol_by_name(self.registry_cls)
-        self.user_options = defaultdict(set)
-        self.steps = defaultdict(set)
-        self.autofinalize = autofinalize
-        self.namespace = namespace
-        self.strict_typing = strict_typing
-
-        self.configured = False
-        self._config_source = config_source
-        self._pending_defaults = deque()
-        self._pending_periodic_tasks = deque()
-
-        self.finalized = False
-        self._finalize_mutex = threading.Lock()
-        self._pending = deque()
-        self._tasks = tasks
-        if not isinstance(self._tasks, TaskRegistry):
-            self._tasks = self.registry_cls(self._tasks or {})
-
-        # If the class defines a custom __reduce_args__ we need to use
-        # the old way of pickling apps: pickling a list of
-        # args instead of the new way that pickles a dict of keywords.
-        self._using_v1_reduce = app_has_custom(self, '__reduce_args__')
-
-        # these options are moved to the config to
-        # simplify pickling of the app object.
-        self._preconf = changes or {}
-        self._preconf_set_by_auto = set()
-        self.__autoset('broker_url', broker)
-        self.__autoset('result_backend', backend)
-        self.__autoset('include', include)
-        self.__autoset('broker_use_ssl', kwargs.get('broker_use_ssl'))
-        self.__autoset('redis_backend_use_ssl', kwargs.get('redis_backend_use_ssl'))
-        self._conf = Settings(
-            PendingConfiguration(
-                self._preconf, self._finalize_pending_conf),
-            prefix=self.namespace,
-            keys=(_old_key_to_new, _new_key_to_old),
-        )
-
-        # - Apply fix-ups.
-        self.fixups = set(self.builtin_fixups) if fixups is None else fixups
-        # ...store fixup instances in _fixups to keep weakrefs alive.
-        self._fixups = [symbol_by_name(fixup)(self) for fixup in self.fixups]
-
-        if self.set_as_current:
-            self.set_current()
-
-        # Signals
-        if self.on_configure is None:
-            # used to be a method pre 4.0
-            self.on_configure = Signal(name='app.on_configure')
-        self.on_after_configure = Signal(
-            name='app.on_after_configure',
-            providing_args={'source'},
-        )
-        self.on_after_finalize = Signal(name='app.on_after_finalize')
-        self.on_after_fork = Signal(name='app.on_after_fork')
-
-        self.on_init()
-        _register_app(self)
-
-    def _get_default_loader(self):
-        # the --loader command-line argument sets the environment variable.
-        return (
-            os.environ.get('CELERY_LOADER') or
-            self.loader_cls or
-            'celery.loaders.app:AppLoader'
-        )
-
-    def on_init(self):
-        """Optional callback called at init."""
-
-    def __autoset(self, key, value):
-        if value:
-            self._preconf[key] = value
-            self._preconf_set_by_auto.add(key)
-
-    def set_current(self):
-        """Make this the current app for this thread."""
-        _set_current_app(self)
-
-    def set_default(self):
-        """Make this the default app for all threads."""
-        set_default_app(self)
-
-    def _ensure_after_fork(self):
-        if not self._after_fork_registered:
-            self._after_fork_registered = True
-            if register_after_fork is not None:
-                register_after_fork(self, _after_fork_cleanup_app)
-
-    def close(self):
-        """Clean up after the application.
-
-        Only necessary for dynamically created apps, and you should
-        probably use the :keyword:`with` statement instead.
-
-        Example:
-            >>> with Celery(set_as_current=False) as app:
-            ...     with app.connection_for_write() as conn:
-            ...         pass
-        """
-        self._pool = None
-        self._aio_pool = None
-        _deregister_app(self)
-
-    def start(self, argv=None):
-        from celery.bin.celery import celery
-
-        celery.params[0].default = self
-
-        try:
-            celery.main(args=argv, standalone_mode=False)
-        except Exit as e:
-            return e.exit_code
-        finally:
-            celery.params[0].default = None
-
-    def worker_main(self, argv=None):
-        if argv is None:
-            argv = sys.argv
-
-        if 'worker' not in argv:
-            raise ValueError(
-                "The worker sub-command must be specified in argv.\n"
-                "Use app.start() to programmatically start other commands."
-            )
-
-        self.start(argv=argv)
-
-    def task(self, *args, **opts):
-        """Decorator to create a task class out of any callable.
-
-        See :ref:`Task options<task-options>` for a list of the
-        arguments that can be passed to this decorator.
-
-        Examples:
-            .. code-block:: python
-
-                @app.task
-                def refresh_feed(url):
-                    store_feed(feedparser.parse(url))
-
-            with setting extra options:
-
-            .. code-block:: python
-
-                @app.task(exchange='feeds')
-                def refresh_feed(url):
-                    return store_feed(feedparser.parse(url))
-
-        Note:
-            App Binding: For custom apps the task decorator will return
-            a proxy object, so that the act of creating the task is not
-            performed until the task is used or the task registry is accessed.
-
-            If you're depending on binding to be deferred, then you must
-            not access any attributes on the returned object until the
-            application is fully set up (finalized).
-        """
-        if USING_EXECV and opts.get('lazy', True):
-            # When using execv the task in the original module will point to a
-            # different app, so doing things like 'add.request' will point to
-            # a different task instance.  This makes sure it will always use
-            # the task instance from the current app.
-            # Really need a better solution for this :(
-            from . import shared_task
-            return shared_task(*args, lazy=False, **opts)
-
-        def inner_create_task_cls(shared=True, filter=None, lazy=True, **opts):
-            _filt = filter
-
-            def _create_task_cls(fun):
-                if shared:
-                    def cons(app):
-                        return app._task_from_fun(fun, **opts)
-                    cons.__name__ = fun.__name__
-                    connect_on_app_finalize(cons)
-                if not lazy or self.finalized:
-                    ret = self._task_from_fun(fun, **opts)
-                else:
-                    # return a proxy object that evaluates on first use
-                    ret = PromiseProxy(self._task_from_fun, (fun,), opts,
-                                       __doc__=fun.__doc__)
-                    self._pending.append(ret)
-                if _filt:
-                    return _filt(ret)
-                return ret
-
-            return _create_task_cls
-
-        if len(args) == 1:
-            if callable(args[0]):
-                return inner_create_task_cls(**opts)(*args)
-            raise TypeError('argument 1 to @task() must be a callable')
-        if args:
-            raise TypeError(
-                '@task() takes exactly 1 argument ({} given)'.format(
-                    sum([len(args), len(opts)])))
-        return inner_create_task_cls(**opts)
-
-    def _task_from_fun(self, fun, name=None, base=None, bind=False, aio_variant=False, **options):
-        if not self.finalized and not self.autofinalize:
-            raise RuntimeError('Contract breach: app not finalized')
-        name = name or self.gen_task_name(fun.__name__, fun.__module__)
-        base = base or self.Task
-
-        if name not in self._tasks:
-            run = fun if bind else staticmethod(fun)
-            attrs = dict({
-                'app': self,
-                'name': name,
-                'run': run,
-                '_decorated': True,
-                '__doc__': fun.__doc__,
-                '__module__': fun.__module__,
-                '__annotations__': fun.__annotations__,
-                '__header__': staticmethod(head_from_fun(fun, bound=bind)),
-                '__wrapped__': run
-            }, **options)
-            task = type(fun.__name__, (base,), attrs)()
-            if aio_variant:
-                aio_task = type(fun.__name__ + '@aio', (self.AioTask,), attrs)()
-                task.aio = aio_task
-
-            # for some reason __qualname__ cannot be set in type()
-            # so we have to set it here.
-            try:
-                task.__qualname__ = fun.__qualname__
-                if aio_variant:
-                    aio_task.__qualname__ = fun.__qualname__
-            except AttributeError:
-                pass
-            self._tasks[task.name] = task
-            task.bind(self)  # connects task to this app
-            add_autoretry_behaviour(task, **options)
-            if aio_variant:
-                aio_task.bind(self)
-                add_autoretry_behaviour(aio_task, **options)
-        else:
-            task = self._tasks[name]
-        return task
-
-    def register_task(self, task):
-        """Utility for registering a task-based class.
-
-        Note:
-            This is here for compatibility with old Celery 1.0
-            style task classes, you should not need to use this for
-            new projects.
-        """
-        task = inspect.isclass(task) and task() or task
-        if not task.name:
-            task_cls = type(task)
-            task.name = self.gen_task_name(
-                task_cls.__name__, task_cls.__module__)
-        add_autoretry_behaviour(task)
-        self.tasks[task.name] = task
-        task._app = self
-        task.bind(self)
-        return task
-
-    def gen_task_name(self, name, module):
-        return gen_task_name(self, name, module)
-
-    def finalize(self, auto=False):
-        """Finalize the app.
-
-        This loads built-in tasks, evaluates pending task decorators,
-        reads configuration, etc.
-        """
-        with self._finalize_mutex:
-            if not self.finalized:
-                if auto and not self.autofinalize:
-                    raise RuntimeError('Contract breach: app not finalized')
-                self.finalized = True
-                _announce_app_finalized(self)
-
-                pending = self._pending
-                while pending:
-                    maybe_evaluate(pending.popleft())
-
-                for task in self._tasks.values():
-                    task.bind(self)
-
-                self.on_after_finalize.send(sender=self)
-
-    def add_defaults(self, fun):
-        """Add default configuration from dict ``d``.
-
-        If the argument is a callable function then it will be regarded
-        as a promise, and it won't be loaded until the configuration is
-        actually needed.
-
-        This method can be compared to:
-
-        .. code-block:: pycon
-
-            >>> celery.conf.update(d)
-
-        with a difference that 1) no copy will be made and 2) the dict will
-        not be transferred when the worker spawns child processes, so
-        it's important that the same configuration happens at import time
-        when pickle restores the object on the other side.
-        """
-        if not callable(fun):
-            d, fun = fun, lambda: d
-        if self.configured:
-            return self._conf.add_defaults(fun())
-        self._pending_defaults.append(fun)
-
-    def config_from_object(self, obj,
-                           silent=False, force=False, namespace=None):
-        """Read configuration from object.
-
-        Object is either an actual object or the name of a module to import.
-
-        Example:
-            >>> celery.config_from_object('myapp.celeryconfig')
-
-            >>> from myapp import celeryconfig
-            >>> celery.config_from_object(celeryconfig)
-
-        Arguments:
-            silent (bool): If true then import errors will be ignored.
-            force (bool): Force reading configuration immediately.
-                By default the configuration will be read only when required.
-        """
-        self._config_source = obj
-        self.namespace = namespace or self.namespace
-        if force or self.configured:
-            self._conf = None
-            if self.loader.config_from_object(obj, silent=silent):
-                return self.conf
-
-    def config_from_envvar(self, variable_name, silent=False, force=False):
-        """Read configuration from environment variable.
-
-        The value of the environment variable must be the name
-        of a module to import.
-
-        Example:
-            >>> os.environ['CELERY_CONFIG_MODULE'] = 'myapp.celeryconfig'
-            >>> celery.config_from_envvar('CELERY_CONFIG_MODULE')
-        """
-        module_name = os.environ.get(variable_name)
-        if not module_name:
-            if silent:
-                return False
-            raise ImproperlyConfigured(
-                ERR_ENVVAR_NOT_SET.strip().format(variable_name))
-        return self.config_from_object(module_name, silent=silent, force=force)
-
-    def config_from_cmdline(self, argv, namespace='celery'):
-        self._conf.update(
-            self.loader.cmdline_config_parser(argv, namespace)
-        )
-
-    def setup_security(self, allowed_serializers=None, key=None, cert=None,
-                       store=None, digest=DEFAULT_SECURITY_DIGEST,
-                       serializer='json'):
-        """Setup the message-signing serializer.
-
-        This will affect all application instances (a global operation).
-
-        Disables untrusted serializers and if configured to use the ``auth``
-        serializer will register the ``auth`` serializer with the provided
-        settings into the Kombu serializer registry.
-
-        Arguments:
-            allowed_serializers (Set[str]): List of serializer names, or
-                content_types that should be exempt from being disabled.
-            key (str): Name of private key file to use.
-                Defaults to the :setting:`security_key` setting.
-            cert (str): Name of certificate file to use.
-                Defaults to the :setting:`security_certificate` setting.
-            store (str): Directory containing certificates.
-                Defaults to the :setting:`security_cert_store` setting.
-            digest (str): Digest algorithm used when signing messages.
-                Default is ``sha256``.
-            serializer (str): Serializer used to encode messages after
-                they've been signed.  See :setting:`task_serializer` for
-                the serializers supported.  Default is ``json``.
-        """
-        from celery.security import setup_security
-        return setup_security(allowed_serializers, key, cert,
-                              store, digest, serializer, app=self)
-
-    def autodiscover_tasks(self, packages=None,
-                           related_name='tasks', force=False):
-        """Auto-discover task modules.
-
-        Searches a list of packages for a "tasks.py" module (or use
-        related_name argument).
-
-        If the name is empty, this will be delegated to fix-ups (e.g., Django).
-
-        For example if you have a directory layout like this:
-
-        .. code-block:: text
-
-            foo/__init__.py
-               tasks.py
-               models.py
-
-            bar/__init__.py
-                tasks.py
-                models.py
-
-            baz/__init__.py
-                models.py
-
-        Then calling ``app.autodiscover_tasks(['foo', 'bar', 'baz'])`` will
-        result in the modules ``foo.tasks`` and ``bar.tasks`` being imported.
-
-        Arguments:
-            packages (List[str]): List of packages to search.
-                This argument may also be a callable, in which case the
-                value returned is used (for lazy evaluation).
-            related_name (Optional[str]): The name of the module to find.  Defaults
-                to "tasks": meaning "look for 'module.tasks' for every
-                module in ``packages``.".  If ``None`` will only try to import
-                the package, i.e. "look for 'module'".
-            force (bool): By default this call is lazy so that the actual
-                auto-discovery won't happen until an application imports
-                the default modules.  Forcing will cause the auto-discovery
-                to happen immediately.
-        """
-        if force:
-            return self._autodiscover_tasks(packages, related_name)
-        signals.import_modules.connect(starpromise(
-            self._autodiscover_tasks, packages, related_name,
-        ), weak=False, sender=self)
-
-    def _autodiscover_tasks(self, packages, related_name, **kwargs):
-        if packages:
-            return self._autodiscover_tasks_from_names(packages, related_name)
-        return self._autodiscover_tasks_from_fixups(related_name)
-
-    def _autodiscover_tasks_from_names(self, packages, related_name):
-        # packages argument can be lazy
-        return self.loader.autodiscover_tasks(
-            packages() if callable(packages) else packages, related_name,
-        )
-
-    def _autodiscover_tasks_from_fixups(self, related_name):
-        return self._autodiscover_tasks_from_names([
-            pkg for fixup in self._fixups
-            if hasattr(fixup, 'autodiscover_tasks')
-            for pkg in fixup.autodiscover_tasks()
-        ], related_name=related_name)
-
-    def send_task(self, name, args=None, kwargs=None, countdown=None,
-                  eta=None, task_id=None, producer=None, connection=None,
-                  router=None, result_cls=None, expires=None,
-                  publisher=None, link=None, link_error=None,
-                  add_to_parent=True, group_id=None, group_index=None,
-                  retries=0, chord=None,
-                  reply_to=None, time_limit=None, soft_time_limit=None,
-                  root_id=None, parent_id=None, route_name=None,
-                  shadow=None, chain=None, task_type=None, **options):
-        """Send task by name.
-
-        Supports the same arguments as :meth:`@-Task.apply_async`.
-
-        Arguments:
-            name (str): Name of task to call (e.g., `"tasks.add"`).
-            result_cls (AsyncResult): Specify custom result class.
-        """
-        parent = have_parent = None
-        amqp = self.amqp
-        task_id = task_id or uuid()
-        producer = producer or publisher  # XXX compat
-        router = router or amqp.router
-        conf = self.conf
-        if conf.task_always_eager:  # pragma: no cover
-            warnings.warn(AlwaysEagerIgnored(
-                'task_always_eager has no effect on send_task',
-            ), stacklevel=2)
-
-        ignored_result = options.pop('ignore_result', False)
-        options = router.route(
-            options, route_name or name, args, kwargs, task_type)
-
-        if not root_id or not parent_id:
-            parent = self.current_worker_task
-            if parent:
-                if not root_id:
-                    root_id = parent.request.root_id or parent.request.id
-                if not parent_id:
-                    parent_id = parent.request.id
-
-                if conf.task_inherit_parent_priority:
-                    options.setdefault('priority',
-                                       parent.request.delivery_info.get('priority'))
-
-        message = amqp.create_task_message(
-            task_id, name, args, kwargs, countdown, eta, group_id, group_index,
-            expires, retries, chord,
-            maybe_list(link), maybe_list(link_error),
-            reply_to or self.thread_oid, time_limit, soft_time_limit,
-            self.conf.task_send_sent_event,
-            root_id, parent_id, shadow, chain,
-            argsrepr=options.get('argsrepr'),
-            kwargsrepr=options.get('kwargsrepr'),
-        )
-
-        if connection:
-            producer = amqp.Producer(connection, auto_declare=False)
-
-        with self.producer_or_acquire(producer) as P:
-            with P.connection._reraise_as_library_errors():
-                if not ignored_result:
-                    self.backend.on_task_call(P, task_id)
-                amqp.send_task_message(P, name, message, **options)
-        result = (result_cls or self.AsyncResult)(task_id)
-        # We avoid using the constructor since a custom result class
-        # can be used, in which case the constructor may still use
-        # the old signature.
-        result.ignored = ignored_result
-
-        if add_to_parent:
-            if not have_parent:
-                parent, have_parent = self.current_worker_task, True
-            if parent:
-                parent.add_trail(result)
-        return result
-
-    def connection_for_read(self, url=None, **kwargs):
-        """Establish connection used for consuming.
-
-        See Also:
-            :meth:`connection` for supported arguments.
-        """
-        return self._connection(url or self.conf.broker_read_url, **kwargs)
-
-    def connection_for_write(self, url=None, **kwargs):
-        """Establish connection used for producing.
-
-        See Also:
-            :meth:`connection` for supported arguments.
-        """
-        return self._connection(url or self.conf.broker_write_url, **kwargs)
-
-    def connection(self, hostname=None, userid=None, password=None,
-                   virtual_host=None, port=None, ssl=None,
-                   connect_timeout=None, transport=None,
-                   transport_options=None, heartbeat=None,
-                   login_method=None, failover_strategy=None, **kwargs):
-        """Establish a connection to the message broker.
-
-        Please use :meth:`connection_for_read` and
-        :meth:`connection_for_write` instead, to convey the intent
-        of use for this connection.
-
-        Arguments:
-            url: Either the URL or the hostname of the broker to use.
-            hostname (str): URL, Hostname/IP-address of the broker.
-                If a URL is used, then the other argument below will
-                be taken from the URL instead.
-            userid (str): Username to authenticate as.
-            password (str): Password to authenticate with
-            virtual_host (str): Virtual host to use (domain).
-            port (int): Port to connect to.
-            ssl (bool, Dict): Defaults to the :setting:`broker_use_ssl`
-                setting.
-            transport (str): defaults to the :setting:`broker_transport`
-                setting.
-            transport_options (Dict): Dictionary of transport specific options.
-            heartbeat (int): AMQP Heartbeat in seconds (``pyamqp`` only).
-            login_method (str): Custom login method to use (AMQP only).
-            failover_strategy (str, Callable): Custom failover strategy.
-            **kwargs: Additional arguments to :class:`kombu.Connection`.
-
-        Returns:
-            kombu.Connection: the lazy connection instance.
-        """
-        return self.connection_for_write(
-            hostname or self.conf.broker_write_url,
-            userid=userid, password=password,
-            virtual_host=virtual_host, port=port, ssl=ssl,
-            connect_timeout=connect_timeout, transport=transport,
-            transport_options=transport_options, heartbeat=heartbeat,
-            login_method=login_method, failover_strategy=failover_strategy,
-            **kwargs
-        )
-
-    def _connection(self, url, userid=None, password=None,
-                    virtual_host=None, port=None, ssl=None,
-                    connect_timeout=None, transport=None,
-                    transport_options=None, heartbeat=None,
-                    login_method=None, failover_strategy=None, **kwargs):
-        conf = self.conf
-        return self.amqp.Connection(
-            url,
-            userid or conf.broker_user,
-            password or conf.broker_password,
-            virtual_host or conf.broker_vhost,
-            port or conf.broker_port,
-            transport=transport or conf.broker_transport,
-            ssl=self.either('broker_use_ssl', ssl),
-            heartbeat=heartbeat,
-            login_method=login_method or conf.broker_login_method,
-            failover_strategy=(
-                failover_strategy or conf.broker_failover_strategy
-            ),
-            transport_options=dict(
-                conf.broker_transport_options, **transport_options or {}
-            ),
-            connect_timeout=self.either(
-                'broker_connection_timeout', connect_timeout
-            ),
-        )
-    broker_connection = connection
-
-    def _acquire_connection(self, pool=True):
-        """Helper for :meth:`connection_or_acquire`."""
-        if pool:
-            return self.pool.acquire(block=True)
-        return self.connection_for_write()
-
-    def connection_or_acquire(self, connection=None, pool=True, *_, **__):
-        """Context used to acquire a connection from the pool.
-
-        For use within a :keyword:`with` statement to get a connection
-        from the pool if one is not already provided.
-
-        Arguments:
-            connection (kombu.Connection): If not provided, a connection
-                will be acquired from the connection pool.
-        """
-        return FallbackContext(connection, self._acquire_connection, pool=pool)
-    default_connection = connection_or_acquire  # XXX compat
-
-    def producer_or_acquire(self, producer=None):
-        """Context used to acquire a producer from the pool.
-
-        For use within a :keyword:`with` statement to get a producer
-        from the pool if one is not already provided
-
-        Arguments:
-            producer (kombu.Producer): If not provided, a producer
-                will be acquired from the producer pool.
-        """
-        return FallbackContext(
-            producer, self.producer_pool.acquire, block=True,
-        )
-    default_producer = producer_or_acquire  # XXX compat
-
-    def prepare_config(self, c):
-        """Prepare configuration before it is merged with the defaults."""
-        return find_deprecated_settings(c)
-
-    def now(self):
-        """Return the current time and date as a datetime."""
-        now_in_utc = to_utc(datetime.utcnow())
-        return now_in_utc.astimezone(self.timezone)
-
-    def select_queues(self, queues=None):
-        """Select subset of queues.
-
-        Arguments:
-            queues (Sequence[str]): a list of queue names to keep.
-        """
-        return self.amqp.queues.select(queues)
-
-    def either(self, default_key, *defaults):
-        """Get key from configuration or use default values.
-
-        Fallback to the value of a configuration key if none of the
-        `*values` are true.
-        """
-        return first(None, [
-            first(None, defaults), starpromise(self.conf.get, default_key),
-        ])
-
-    def bugreport(self):
-        """Return information useful in bug reports."""
-        return bugreport(self)
-
-    def _get_backend(self):
-        backend, url = backends.by_url(
-            self.backend_cls or self.conf.result_backend,
-            self.loader)
-        return backend(app=self, url=url)
-
-    def _finalize_pending_conf(self):
-        """Get config value by key and finalize loading the configuration.
-
-        Note:
-            This is used by PendingConfiguration:
-                as soon as you access a key the configuration is read.
-        """
-        conf = self._conf = self._load_config()
-        return conf
-
-    def _load_config(self):
-        if isinstance(self.on_configure, Signal):
-            self.on_configure.send(sender=self)
-        else:
-            # used to be a method pre 4.0
-            self.on_configure()
-        if self._config_source:
-            self.loader.config_from_object(self._config_source)
-        self.configured = True
-        settings = detect_settings(
-            self.prepare_config(self.loader.conf), self._preconf,
-            ignore_keys=self._preconf_set_by_auto, prefix=self.namespace,
-        )
-        if self._conf is not None:
-            # replace in place, as someone may have referenced app.conf,
-            # done some changes, accessed a key, and then try to make more
-            # changes to the reference and not the finalized value.
-            self._conf.swap_with(settings)
-        else:
-            self._conf = settings
-
-        # load lazy config dict initializers.
-        pending_def = self._pending_defaults
-        while pending_def:
-            self._conf.add_defaults(maybe_evaluate(pending_def.popleft()()))
-
-        # load lazy periodic tasks
-        pending_beat = self._pending_periodic_tasks
-        while pending_beat:
-            self._add_periodic_task(*pending_beat.popleft())
-
-        self.on_after_configure.send(sender=self, source=self._conf)
-        return self._conf
-
-    def _after_fork(self):
-        self._pool = None
-        try:
-            self.__dict__['amqp']._producer_pool = None
-        except (AttributeError, KeyError):
-            pass
-        self.on_after_fork.send(sender=self)
-
-    def signature(self, *args, **kwargs):
-        """Return a new :class:`~celery.Signature` bound to this app."""
-        kwargs['app'] = self
-        return self._canvas.signature(*args, **kwargs)
-
-    def add_periodic_task(self, schedule, sig,
-                          args=(), kwargs=(), name=None, **opts):
-        key, entry = self._sig_to_periodic_task_entry(
-            schedule, sig, args, kwargs, name, **opts)
-        if self.configured:
-            self._add_periodic_task(key, entry)
-        else:
-            self._pending_periodic_tasks.append((key, entry))
-        return key
-
-    def _sig_to_periodic_task_entry(self, schedule, sig,
-                                    args=(), kwargs=None, name=None, **opts):
-        kwargs = {} if not kwargs else kwargs
-        sig = (sig.clone(args, kwargs)
-               if isinstance(sig, abstract.CallableSignature)
-               else self.signature(sig.name, args, kwargs))
-        return name or repr(sig), {
-            'schedule': schedule,
-            'task': sig.name,
-            'args': sig.args,
-            'kwargs': sig.kwargs,
-            'options': dict(sig.options, **opts),
-        }
-
-    def _add_periodic_task(self, key, entry):
-        self._conf.beat_schedule[key] = entry
-
-    def create_task_cls(self):
-        """Create a base task class bound to this app."""
-        return self.subclass_with_self(
-            self.task_cls, name='Task', attribute='_app',
-            keep_reduce=True, abstract=True,
-        )
-
-    def subclass_with_self(self, Class, name=None, attribute='app',
-                           reverse=None, keep_reduce=False, **kw):
-        """Subclass an app-compatible class.
-
-        App-compatible means that the class has a class attribute that
-        provides the default app it should use, for example:
-        ``class Foo: app = None``.
-
-        Arguments:
-            Class (type): The app-compatible class to subclass.
-            name (str): Custom name for the target class.
-            attribute (str): Name of the attribute holding the app,
-                Default is 'app'.
-            reverse (str): Reverse path to this object used for pickling
-                purposes. For example, to get ``app.AsyncResult``,
-                use ``"AsyncResult"``.
-            keep_reduce (bool): If enabled a custom ``__reduce__``
-                implementation won't be provided.
-        """
-        Class = symbol_by_name(Class)
-        reverse = reverse if reverse else Class.__name__
-
-        def __reduce__(self):
-            return _unpickle_appattr, (reverse, self.__reduce_args__())
-
-        attrs = dict(
-            {attribute: self},
-            __module__=Class.__module__,
-            __doc__=Class.__doc__,
-            **kw)
-        if not keep_reduce:
-            attrs['__reduce__'] = __reduce__
-
-        return type(name or Class.__name__, (Class,), attrs)
-
-    def _rgetattr(self, path):
-        return attrgetter(path)(self)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *exc_info):
-        self.close()
-
-    def __repr__(self):
-        return '<{} {}>'.format(type(self).__name__, appstr(self))
-
-    def __reduce__(self):
-        if self._using_v1_reduce:
-            return self.__reduce_v1__()
-        return (_unpickle_app_v2, (self.__class__, self.__reduce_keys__()))
-
-    def __reduce_v1__(self):
-        # Reduce only pickles the configuration changes,
-        # so the default configuration doesn't have to be passed
-        # between processes.
-        return (
-            _unpickle_app,
-            (self.__class__, self.Pickler) + self.__reduce_args__(),
-        )
-
-    def __reduce_keys__(self):
-        """Keyword arguments used to reconstruct the object when unpickling."""
-        return {
-            'main': self.main,
-            'changes':
-                self._conf.changes if self.configured else self._preconf,
-            'loader': self.loader_cls,
-            'backend': self.backend_cls,
-            'amqp': self.amqp_cls,
-            'events': self.events_cls,
-            'log': self.log_cls,
-            'control': self.control_cls,
-            'fixups': self.fixups,
-            'config_source': self._config_source,
-            'task_cls': self.task_cls,
-            'namespace': self.namespace,
-        }
-
-    def __reduce_args__(self):
-        """Deprecated method, please use :meth:`__reduce_keys__` instead."""
-        return (self.main, self._conf.changes if self.configured else {},
-                self.loader_cls, self.backend_cls, self.amqp_cls,
-                self.events_cls, self.log_cls, self.control_cls,
-                False, self._config_source)
-
-    @cached_property
-    def Worker(self):
-        """Worker application.
-
-        See Also:
-            :class:`~@Worker`.
-        """
-        return self.subclass_with_self('celery.apps.worker:Worker')
-
-    @cached_property
-    def WorkController(self, **kwargs):
-        """Embeddable worker.
-
-        See Also:
-            :class:`~@WorkController`.
-        """
-        return self.subclass_with_self('celery.worker:WorkController')
-
-    @cached_property
-    def Beat(self, **kwargs):
-        """:program:`celery beat` scheduler application.
-
-        See Also:
-            :class:`~@Beat`.
-        """
-        return self.subclass_with_self('celery.apps.beat:Beat')
-
-    @cached_property
-    def Task(self):
-        """Base task class for this app."""
-        return self.create_task_cls()
-
-    @cached_property
-    def annotations(self):
-        return prepare_annotations(self.conf.task_annotations)
-
-    @cached_property
-    def AsyncResult(self):
-        """Create new result instance.
-
-        See Also:
-            :class:`celery.result.AsyncResult`.
-        """
-        return self.subclass_with_self('celery.result:AsyncResult')
-
-    @cached_property
-    def ResultSet(self):
-        return self.subclass_with_self('celery.result:ResultSet')
-
-    @cached_property
-    def GroupResult(self):
-        """Create new group result instance.
-
-        See Also:
-            :class:`celery.result.GroupResult`.
-        """
-        return self.subclass_with_self('celery.result:GroupResult')
-
-    @property
-    def pool(self):
-        """Broker connection pool: :class:`~@pool`.
-
-        Note:
-            This attribute is not related to the workers concurrency pool.
-        """
-        if self._pool is None:
-            self._ensure_after_fork()
-            limit = self.conf.broker_pool_limit
-            pools.set_limit(limit)
-            self._pool = pools.connections[self.connection_for_write()]
-        return self._pool
-
-    @property
-    def current_task(self):
-        """Instance of task being executed, or :const:`None`."""
-        return _task_stack.top
-
-    @property
-    def current_worker_task(self):
-        """The task currently being executed by a worker or :const:`None`.
-
-        Differs from :data:`current_task` in that it's not affected
-        by tasks calling other tasks directly, or eagerly.
-        """
-        return get_current_worker_task()
-
-    @cached_property
-    def oid(self):
-        """Universally unique identifier for this app."""
-        # since 4.0: thread.get_ident() is not included when
-        # generating the process id.  This is due to how the RPC
-        # backend now dedicates a single thread to receive results,
-        # which would not work if each thread has a separate id.
-        return oid_from(self, threads=False)
-
-    @property
-    def thread_oid(self):
-        """Per-thread unique identifier for this app."""
-        try:
-            return self._local.oid
-        except AttributeError:
-            self._local.oid = new_oid = oid_from(self, threads=True)
-            return new_oid
-
-    @cached_property
-    def amqp(self):
-        """AMQP related functionality: :class:`~@amqp`."""
-        return instantiate(self.amqp_cls, app=self)
-
-    @property
-    def backend(self):
-        """Current backend instance."""
-        try:
-            return self._local.backend
-        except AttributeError:
-            self._local.backend = new_backend = self._get_backend()
-            return new_backend
-
-    @property
-    def conf(self):
-        """Current configuration."""
-        if self._conf is None:
-            self._conf = self._load_config()
-        return self._conf
-
-    @conf.setter
-    def conf(self, d):  # noqa
-        self._conf = d
-
-    @cached_property
-    def control(self):
-        """Remote control: :class:`~@control`."""
-        return instantiate(self.control_cls, app=self)
-
-    @cached_property
-    def events(self):
-        """Consuming and sending events: :class:`~@events`."""
-        return instantiate(self.events_cls, app=self)
-
-    @cached_property
-    def loader(self):
-        """Current loader instance."""
-        return get_loader_cls(self.loader_cls)(app=self)
-
-    @cached_property
-    def log(self):
-        """Logging: :class:`~@log`."""
-        return instantiate(self.log_cls, app=self)
-
-    @cached_property
-    def _canvas(self):
-        from celery import canvas
-        return canvas
-
-    @cached_property
-    def tasks(self):
-        """Task registry.
-
-        Warning:
-            Accessing this attribute will also auto-finalize the app.
-        """
-        self.finalize(auto=True)
-        return self._tasks
-
-    @property
-    def producer_pool(self):
-        return self.amqp.producer_pool
-
-    def uses_utc_timezone(self):
-        """Check if the application uses the UTC timezone."""
-        return self.timezone == timezone.utc
-
-    @cached_property
-    def timezone(self):
-        """Current timezone for this app.
-
-        This is a cached property taking the time zone from the
-        :setting:`timezone` setting.
-        """
-        conf = self.conf
-        if not conf.timezone:
-            if conf.enable_utc:
-                return timezone.utc
-            else:
-                return timezone.local
-        return timezone.get_timezone(conf.timezone)
-
-    # -----------------------------------------------------------------------------
-    # asyncio support
-    _aio_pool = None
-
-    aio_task_cls = 'celery.aio.task:AioTask'
-    aio_amqp_cls = 'celery.aio.amqp:AioAMQP'
-    aio_events_cls = 'celery.aio.events:Events'
-    aio_control_cls = 'celery.aio.control:Control'
-
-    def create_aio_task_cls(self):
-        """Create a base task class bound to this app."""
-        return self.subclass_with_self(
-            self.aio_task_cls, name='AioTask', attribute='_app',
-            keep_reduce=True, abstract=True,
-        )
-
-    @cached_property
-    def AioTask(self):
-        """Base aio-task class for this app."""
-        return self.create_aio_task_cls()
-
-    @cached_property
-    def aio_amqp(self):
-        """AMQP related functionality: :class:`~@aio_amqp`."""
-        return instantiate(self.aio_amqp_cls, app=self)
-
-    @cached_property
-    def aio_events(self):
-        """Consuming and sending events: :class:`~@events`."""
-        return instantiate(self.aio_events_cls, app=self)
-
-    @property
-    def aio_producer_pool(self):
-        return self.aio_amqp.producer_pool
-
-    @property
-    def aio_pool(self):
-        if self._aio_pool is None:
-            self._ensure_after_fork()
-            limit = self.conf.broker_pool_limit
-            pools.set_limit(limit)
-            self._aio_pool = pools.connections[self.aconnection_for_write()]
-        return self._aio_pool
-
-    @cached_property
-    def aio_control(self):
-        """Remote control: :class:`~@control`."""
-        return instantiate(self.aio_control_cls, app=self)
-
-    @cached_property
-    def AioAsyncResult(self):
-        return self.subclass_with_self('celery.aio.result:AsyncResult')
-
-    @cached_property
-    def AioGroupResult(self):
-        return self.subclass_with_self('celery.aio.result:GroupResult')
-
-    def aio_producer_or_acquire(self, producer=None):
-        """Context used to acquire a producer from the pool.
-
-        For use within a :keyword:`with` statement to get a producer
-        from the pool if one is not already provided
-
-        Arguments:
-            producer (kombu.Producer): If not provided, a producer
-                will be acquired from the producer pool.
-        """
-        return AsyncFallbackContext(
-            producer, self.aio_producer_pool.acquire, block=True,
-        )
-
-    @asynccontextmanager
-    async def _aio_acquire_connection(self, pool=True):
-        """Helper for :meth:`connection_or_acquire`."""
-        if pool:
-            async with self.aio_pool.acquire(block=True) as conn:
-                yield conn
-        else:
-            yield self.aconnection_for_write()
-
-    def aio_connection_or_acquire(self, connection=None, pool=True, *_, **__):
-        return AsyncFallbackContext(
-            connection, self._aio_acquire_connection, pool=pool
-        )
-
-    async def asend_task(self, name, args=None, kwargs=None, countdown=None,
-                  eta=None, task_id=None, producer=None, connection=None,
-                  router=None, result_cls=None, expires=None,
-                  publisher=None, link=None, link_error=None,
-                  add_to_parent=True, group_id=None, group_index=None,
-                  retries=0, chord=None,
-                  reply_to=None, time_limit=None, soft_time_limit=None,
-                  root_id=None, parent_id=None, route_name=None,
-                  shadow=None, chain=None, task_type=None, **options):
-        """Send task by name.
-
-        Supports the same arguments as :meth:`@-Task.apply_async`.
-
-        Arguments:
-            name (str): Name of task to call (e.g., `"tasks.add"`).
-            result_cls (AsyncResult): Specify custom result class.
-        """
-        parent = have_parent = None
-        amqp = self.aio_amqp
-        task_id = task_id or uuid()
-        producer = producer or publisher  # XXX compat
-        router = router or amqp.router
-        conf = self.conf
-        if conf.task_always_eager:  # pragma: no cover
-            warnings.warn(AlwaysEagerIgnored(
-                'task_always_eager has no effect on send_task',
-            ), stacklevel=2)
-
-        ignored_result = options.pop('ignore_result', False)
-        options = router.route(
-            options, route_name or name, args, kwargs, task_type)
-
-        if not root_id or not parent_id:
-            parent = self.current_worker_task
-            if parent:
-                if not root_id:
-                    root_id = parent.request.root_id or parent.request.id
-                if not parent_id:
-                    parent_id = parent.request.id
-
-                if conf.task_inherit_parent_priority:
-                    options.setdefault('priority',
-                                       parent.request.delivery_info.get('priority'))
-
-        message = amqp.create_task_message(
-            task_id, name, args, kwargs, countdown, eta, group_id, group_index,
-            expires, retries, chord,
-            maybe_list(link), maybe_list(link_error),
-            reply_to or self.thread_oid, time_limit, soft_time_limit,
-            self.conf.task_send_sent_event,
-            root_id, parent_id, shadow, chain,
-            argsrepr=options.get('argsrepr'),
-            kwargsrepr=options.get('kwargsrepr'),
-        )
-
-        if connection:
-            producer = amqp.Producer(connection, auto_declare=False)
-
-        async with self.aio_producer_or_acquire(producer) as P:
-            with (await P.connection)._reraise_as_library_errors():
-                if not ignored_result:
-                    await self.aio_backend.on_task_call(P, task_id)
-                await amqp.send_task_message(P, name, message, **options)
-        result = (result_cls or self.AsyncResult)(task_id)
-        # We avoid using the constructor since a custom result class
-        # can be used, in which case the constructor may still use
-        # the old signature.
-        result.ignored = ignored_result
-
-        if add_to_parent:
-            if not have_parent:
-                parent, have_parent = self.current_worker_task, True
-            if parent:
-                parent.add_trail(result)
-        return result
-
-    def aconnection_for_read(self, url=None, **kwargs):
-        """Establish connection used for consuming.
-
-        See Also:
-            :meth:`connection` for supported arguments.
-        """
-        return self._aconnection(url or self.conf.broker_read_url, **kwargs)
-
-    def aconnection_for_write(self, url=None, **kwargs):
-        """Establish connection used for producing.
-
-        See Also:
-            :meth:`connection` for supported arguments.
-        """
-        return self._aconnection(url or self.conf.broker_write_url, **kwargs)
-
-    def _aconnection(self, url, userid=None, password=None,
-                    virtual_host=None, port=None, ssl=None,
-                    connect_timeout=None, transport=None,
-                    transport_options=None, heartbeat=None,
-                    login_method=None, failover_strategy=None, **kwargs):
-        conf = self.conf
-        return self.aio_amqp.Connection(
-            url,
-            userid or conf.broker_user,
-            password or conf.broker_password,
-            virtual_host or conf.broker_vhost,
-            port or conf.broker_port,
-            transport=transport or conf.broker_transport,
-            ssl=self.either('broker_use_ssl', ssl),
-            heartbeat=heartbeat,
-            login_method=login_method or conf.broker_login_method,
-            failover_strategy=(
-                failover_strategy or conf.broker_failover_strategy
-            ),
-            transport_options=dict(
-                conf.broker_transport_options, **transport_options or {}
-            ),
-            connect_timeout=self.either(
-                'broker_connection_timeout', connect_timeout
-            ),
-        )
-
-    @property
-    def aio_backend(self):
-        """Current backend instance."""
-        try:
-            return self._local.aio_backend
-        except AttributeError:
-            override_backends = self.loader.override_backends
-            ori_redis = override_backends.pop('redis', None)
-            ori_rediss = override_backends.pop('rediss', None)
-            ori_sentinel = override_backends.pop('sentinel', None)
-            override_backends['redis'] = override_backends['rediss'] \
-                = 'celery.aio.backend:RedisBackend'
-            override_backends['sentinel'] = 'celery.aio.backend:SentinelBackend'
-            try:
-                self._local.aio_backend = new_backend = self._get_backend()
-            finally:
-                if ori_redis is not None:
-                    override_backends['redis'] = ori_rediss
-                else:
-                    override_backends.pop('redis', None)
-
-                if ori_rediss is not None:
-                    override_backends['rediss'] = ori_rediss
-                else:
-                    override_backends.pop('rediss', None)
-
-                if ori_sentinel is not None:
-                    override_backends['sentinel'] = ori_sentinel
-                else:
-                    override_backends.pop('sentinel', None)
-            return new_backend
-
-
-App = Celery  # noqa: E305 XXX compat
+"""Actual App instance implementation."""
+import inspect
+import os
+import sys
+import threading
+import warnings
+from collections import UserDict, defaultdict, deque
+from contextlib import asynccontextmanager
+from datetime import datetime
+from operator import attrgetter
+
+from click.exceptions import Exit
+from kombu import pools
+from kombu.clocks import LamportClock
+from kombu.common import oid_from
+from kombu.utils.compat import register_after_fork
+from kombu.utils.objects import cached_property
+from kombu.utils.uuid import uuid
+from vine import starpromise
+
+from celery import platforms, signals
+from celery._state import (_announce_app_finalized, _deregister_app,
+                           _register_app, _set_current_app, _task_stack,
+                           connect_on_app_finalize, get_current_app,
+                           get_current_worker_task, set_default_app)
+from celery.exceptions import AlwaysEagerIgnored, ImproperlyConfigured
+from celery.loaders import get_loader_cls
+from celery.local import PromiseProxy, maybe_evaluate
+from celery.utils import abstract
+from celery.utils.collections import AttributeDictMixin
+from celery.utils.dispatch import Signal
+from celery.utils.functional import first, head_from_fun, maybe_list
+from celery.utils.imports import gen_task_name, instantiate, symbol_by_name
+from celery.utils.log import get_logger
+from celery.utils.objects import (FallbackContext,
+                                  mro_lookup,
+                                  AsyncFallbackContext)
+from celery.utils.time import timezone, to_utc
+
+# Load all builtin tasks
+from . import builtins  # noqa
+from . import backends
+from .annotations import prepare as prepare_annotations
+from .autoretry import add_autoretry_behaviour
+from .defaults import DEFAULT_SECURITY_DIGEST, find_deprecated_settings
+from .registry import TaskRegistry
+from .utils import (AppPickler, Settings, _new_key_to_old, _old_key_to_new,
+                    _unpickle_app, _unpickle_app_v2, appstr, bugreport,
+                    detect_settings)
+
+__all__ = ('Celery',)
+
+logger = get_logger(__name__)
+
+BUILTIN_FIXUPS = {
+    'celery.fixups.django:fixup',
+}
+USING_EXECV = os.environ.get('FORKED_BY_MULTIPROCESSING')
+
+ERR_ENVVAR_NOT_SET = """
+The environment variable {0!r} is not set,
+and as such the configuration could not be loaded.
+
+Please set this variable and make sure it points to
+a valid configuration module.
+
+Example:
+    {0}="proj.celeryconfig"
+"""
+
+
+def app_has_custom(app, attr):
+    """Return true if app has customized method `attr`.
+
+    Note:
+        This is used for optimizations in cases where we know
+        how the default behavior works, but need to account
+        for someone using inheritance to override a method/property.
+    """
+    return mro_lookup(app.__class__, attr, stop={Celery, object},
+                      monkey_patched=[__name__])
+
+
+def _unpickle_appattr(reverse_name, args):
+    """Unpickle app."""
+    # Given an attribute name and a list of args, gets
+    # the attribute from the current app and calls it.
+    return get_current_app()._rgetattr(reverse_name)(*args)
+
+
+def _after_fork_cleanup_app(app):
+    # This is used with multiprocessing.register_after_fork,
+    # so need to be at module level.
+    try:
+        app._after_fork()
+    except Exception as exc:  # pylint: disable=broad-except
+        logger.info('after forker raised exception: %r', exc, exc_info=1)
+
+
+class PendingConfiguration(UserDict, AttributeDictMixin):
+    # `app.conf` will be of this type before being explicitly configured,
+    # meaning the app can keep any configuration set directly
+    # on `app.conf` before the `app.config_from_object` call.
+    #
+    # accessing any key will finalize the configuration,
+    # replacing `app.conf` with a concrete settings object.
+
+    callback = None
+    _data = None
+
+    def __init__(self, conf, callback):
+        object.__setattr__(self, '_data', conf)
+        object.__setattr__(self, 'callback', callback)
+
+    def __setitem__(self, key, value):
+        self._data[key] = value
+
+    def clear(self):
+        self._data.clear()
+
+    def update(self, *args, **kwargs):
+        self._data.update(*args, **kwargs)
+
+    def setdefault(self, *args, **kwargs):
+        return self._data.setdefault(*args, **kwargs)
+
+    def __contains__(self, key):
+        # XXX will not show finalized configuration
+        # setdefault will cause `key in d` to happen,
+        # so for setdefault to be lazy, so does contains.
+        return key in self._data
+
+    def __len__(self):
+        return len(self.data)
+
+    def __repr__(self):
+        return repr(self.data)
+
+    @cached_property
+    def data(self):
+        return self.callback()
+
+
+class Celery:
+    """Celery application.
+
+    Arguments:
+        main (str): Name of the main module if running as `__main__`.
+            This is used as the prefix for auto-generated task names.
+
+    Keyword Arguments:
+        broker (str): URL of the default broker used.
+        backend (Union[str, Type[celery.backends.base.Backend]]):
+            The result store backend class, or the name of the backend
+            class to use.
+
+            Default is the value of the :setting:`result_backend` setting.
+        autofinalize (bool): If set to False a :exc:`RuntimeError`
+            will be raised if the task registry or tasks are used before
+            the app is finalized.
+        set_as_current (bool):  Make this the global current app.
+        include (List[str]): List of modules every worker should import.
+
+        amqp (Union[str, Type[AMQP]]): AMQP object or class name.
+        events (Union[str, Type[celery.app.events.Events]]): Events object or
+            class name.
+        log (Union[str, Type[Logging]]): Log object or class name.
+        control (Union[str, Type[celery.app.control.Control]]): Control object
+            or class name.
+        tasks (Union[str, Type[TaskRegistry]]): A task registry, or the name of
+            a registry class.
+        fixups (List[str]): List of fix-up plug-ins (e.g., see
+            :mod:`celery.fixups.django`).
+        config_source (Union[str, class]): Take configuration from a class,
+            or object.  Attributes may include any settings described in
+            the documentation.
+        task_cls (Union[str, Type[celery.app.task.Task]]): base task class to
+            use. See :ref:`this section <custom-task-cls-app-wide>` for usage.
+    """
+
+    #: This is deprecated, use :meth:`reduce_keys` instead
+    Pickler = AppPickler
+
+    SYSTEM = platforms.SYSTEM
+    IS_macOS, IS_WINDOWS = platforms.IS_macOS, platforms.IS_WINDOWS
+
+    #: Name of the `__main__` module.  Required for standalone scripts.
+    #:
+    #: If set this will be used instead of `__main__` when automatically
+    #: generating task names.
+    main = None
+
+    #: Custom options for command-line programs.
+    #: See :ref:`extending-commandoptions`
+    user_options = None
+
+    #: Custom bootsteps to extend and modify the worker.
+    #: See :ref:`extending-bootsteps`.
+    steps = None
+
+    builtin_fixups = BUILTIN_FIXUPS
+
+    amqp_cls = 'celery.app.amqp:AMQP'
+    backend_cls = None
+    events_cls = 'celery.app.events:Events'
+    loader_cls = None
+    log_cls = 'celery.app.log:Logging'
+    control_cls = 'celery.app.control:Control'
+    task_cls = 'celery.app.task:Task'
+    registry_cls = 'celery.app.registry:TaskRegistry'
+
+    #: Thread local storage.
+    _local = None
+    _fixups = None
+    _pool = None
+    _conf = None
+    _after_fork_registered = False
+
+    #: Signal sent when app is loading configuration.
+    on_configure = None
+
+    #: Signal sent after app has prepared the configuration.
+    on_after_configure = None
+
+    #: Signal sent after app has been finalized.
+    on_after_finalize = None
+
+    #: Signal sent by every new process after fork.
+    on_after_fork = None
+
+    def __init__(self, main=None, loader=None, backend=None,
+                 amqp=None, events=None, log=None, control=None,
+                 set_as_current=True, tasks=None, broker=None, include=None,
+                 changes=None, config_source=None, fixups=None, task_cls=None,
+                 autofinalize=True, namespace=None, strict_typing=True,
+                 aio_control=None,
+                 **kwargs):
+
+        self._local = threading.local()
+
+        self.clock = LamportClock()
+        self.main = main
+        self.amqp_cls = amqp or self.amqp_cls
+        self.events_cls = events or self.events_cls
+        self.loader_cls = loader or self._get_default_loader()
+        self.log_cls = log or self.log_cls
+        self.control_cls = control or self.control_cls
+        self.aio_control_cls = aio_control or self.aio_control_cls
+        self.task_cls = task_cls or self.task_cls
+        self.set_as_current = set_as_current
+        self.registry_cls = symbol_by_name(self.registry_cls)
+        self.user_options = defaultdict(set)
+        self.steps = defaultdict(set)
+        self.autofinalize = autofinalize
+        self.namespace = namespace
+        self.strict_typing = strict_typing
+
+        self.configured = False
+        self._config_source = config_source
+        self._pending_defaults = deque()
+        self._pending_periodic_tasks = deque()
+
+        self.finalized = False
+        self._finalize_mutex = threading.Lock()
+        self._pending = deque()
+        self._tasks = tasks
+        if not isinstance(self._tasks, TaskRegistry):
+            self._tasks = self.registry_cls(self._tasks or {})
+
+        # If the class defines a custom __reduce_args__ we need to use
+        # the old way of pickling apps: pickling a list of
+        # args instead of the new way that pickles a dict of keywords.
+        self._using_v1_reduce = app_has_custom(self, '__reduce_args__')
+
+        # these options are moved to the config to
+        # simplify pickling of the app object.
+        self._preconf = changes or {}
+        self._preconf_set_by_auto = set()
+        self.__autoset('broker_url', broker)
+        self.__autoset('result_backend', backend)
+        self.__autoset('include', include)
+        self.__autoset('broker_use_ssl', kwargs.get('broker_use_ssl'))
+        self.__autoset('redis_backend_use_ssl', kwargs.get('redis_backend_use_ssl'))
+        self._conf = Settings(
+            PendingConfiguration(
+                self._preconf, self._finalize_pending_conf),
+            prefix=self.namespace,
+            keys=(_old_key_to_new, _new_key_to_old),
+        )
+
+        # - Apply fix-ups.
+        self.fixups = set(self.builtin_fixups) if fixups is None else fixups
+        # ...store fixup instances in _fixups to keep weakrefs alive.
+        self._fixups = [symbol_by_name(fixup)(self) for fixup in self.fixups]
+
+        if self.set_as_current:
+            self.set_current()
+
+        # Signals
+        if self.on_configure is None:
+            # used to be a method pre 4.0
+            self.on_configure = Signal(name='app.on_configure')
+        self.on_after_configure = Signal(
+            name='app.on_after_configure',
+            providing_args={'source'},
+        )
+        self.on_after_finalize = Signal(name='app.on_after_finalize')
+        self.on_after_fork = Signal(name='app.on_after_fork')
+
+        self.on_init()
+        _register_app(self)
+
+    def _get_default_loader(self):
+        # the --loader command-line argument sets the environment variable.
+        return (
+            os.environ.get('CELERY_LOADER') or
+            self.loader_cls or
+            'celery.loaders.app:AppLoader'
+        )
+
+    def on_init(self):
+        """Optional callback called at init."""
+
+    def __autoset(self, key, value):
+        if value:
+            self._preconf[key] = value
+            self._preconf_set_by_auto.add(key)
+
+    def set_current(self):
+        """Make this the current app for this thread."""
+        _set_current_app(self)
+
+    def set_default(self):
+        """Make this the default app for all threads."""
+        set_default_app(self)
+
+    def _ensure_after_fork(self):
+        if not self._after_fork_registered:
+            self._after_fork_registered = True
+            if register_after_fork is not None:
+                register_after_fork(self, _after_fork_cleanup_app)
+
+    def close(self):
+        """Clean up after the application.
+
+        Only necessary for dynamically created apps, and you should
+        probably use the :keyword:`with` statement instead.
+
+        Example:
+            >>> with Celery(set_as_current=False) as app:
+            ...     with app.connection_for_write() as conn:
+            ...         pass
+        """
+        self._pool = None
+        self._aio_pool = None
+        _deregister_app(self)
+
+    def start(self, argv=None):
+        from celery.bin.celery import celery
+
+        celery.params[0].default = self
+
+        try:
+            celery.main(args=argv, standalone_mode=False)
+        except Exit as e:
+            return e.exit_code
+        finally:
+            celery.params[0].default = None
+
+    def worker_main(self, argv=None):
+        if argv is None:
+            argv = sys.argv
+
+        if 'worker' not in argv:
+            raise ValueError(
+                "The worker sub-command must be specified in argv.\n"
+                "Use app.start() to programmatically start other commands."
+            )
+
+        self.start(argv=argv)
+
+    def task(self, *args, **opts):
+        """Decorator to create a task class out of any callable.
+
+        See :ref:`Task options<task-options>` for a list of the
+        arguments that can be passed to this decorator.
+
+        Examples:
+            .. code-block:: python
+
+                @app.task
+                def refresh_feed(url):
+                    store_feed(feedparser.parse(url))
+
+            with setting extra options:
+
+            .. code-block:: python
+
+                @app.task(exchange='feeds')
+                def refresh_feed(url):
+                    return store_feed(feedparser.parse(url))
+
+        Note:
+            App Binding: For custom apps the task decorator will return
+            a proxy object, so that the act of creating the task is not
+            performed until the task is used or the task registry is accessed.
+
+            If you're depending on binding to be deferred, then you must
+            not access any attributes on the returned object until the
+            application is fully set up (finalized).
+        """
+        if USING_EXECV and opts.get('lazy', True):
+            # When using execv the task in the original module will point to a
+            # different app, so doing things like 'add.request' will point to
+            # a different task instance.  This makes sure it will always use
+            # the task instance from the current app.
+            # Really need a better solution for this :(
+            from . import shared_task
+            return shared_task(*args, lazy=False, **opts)
+
+        def inner_create_task_cls(shared=True, filter=None, lazy=True, **opts):
+            _filt = filter
+
+            def _create_task_cls(fun):
+                if shared:
+                    def cons(app):
+                        return app._task_from_fun(fun, **opts)
+                    cons.__name__ = fun.__name__
+                    connect_on_app_finalize(cons)
+                if not lazy or self.finalized:
+                    ret = self._task_from_fun(fun, **opts)
+                else:
+                    # return a proxy object that evaluates on first use
+                    ret = PromiseProxy(self._task_from_fun, (fun,), opts,
+                                       __doc__=fun.__doc__)
+                    self._pending.append(ret)
+                if _filt:
+                    return _filt(ret)
+                return ret
+
+            return _create_task_cls
+
+        if len(args) == 1:
+            if callable(args[0]):
+                return inner_create_task_cls(**opts)(*args)
+            raise TypeError('argument 1 to @task() must be a callable')
+        if args:
+            raise TypeError(
+                '@task() takes exactly 1 argument ({} given)'.format(
+                    sum([len(args), len(opts)])))
+        return inner_create_task_cls(**opts)
+
+    def _task_from_fun(self, fun, name=None, base=None, bind=False, aio_variant=False, **options):
+        if not self.finalized and not self.autofinalize:
+            raise RuntimeError('Contract breach: app not finalized')
+        name = name or self.gen_task_name(fun.__name__, fun.__module__)
+        base = base or self.Task
+
+        if name not in self._tasks:
+            run = fun if bind else staticmethod(fun)
+            attrs = dict({
+                'app': self,
+                'name': name,
+                'run': run,
+                '_decorated': True,
+                '__doc__': fun.__doc__,
+                '__module__': fun.__module__,
+                '__annotations__': fun.__annotations__,
+                '__header__': staticmethod(head_from_fun(fun, bound=bind)),
+                '__wrapped__': run
+            }, **options)
+            task = type(fun.__name__, (base,), attrs)()
+            if aio_variant:
+                aio_task = type(fun.__name__ + '@aio', (self.AioTask,), attrs)()
+                task.aio = aio_task
+
+            # for some reason __qualname__ cannot be set in type()
+            # so we have to set it here.
+            try:
+                task.__qualname__ = fun.__qualname__
+                if aio_variant:
+                    aio_task.__qualname__ = fun.__qualname__
+            except AttributeError:
+                pass
+            self._tasks[task.name] = task
+            task.bind(self)  # connects task to this app
+            add_autoretry_behaviour(task, **options)
+            if aio_variant:
+                aio_task.bind(self)
+                add_autoretry_behaviour(aio_task, **options)
+        else:
+            task = self._tasks[name]
+        return task
+
+    def register_task(self, task):
+        """Utility for registering a task-based class.
+
+        Note:
+            This is here for compatibility with old Celery 1.0
+            style task classes, you should not need to use this for
+            new projects.
+        """
+        task = inspect.isclass(task) and task() or task
+        if not task.name:
+            task_cls = type(task)
+            task.name = self.gen_task_name(
+                task_cls.__name__, task_cls.__module__)
+        add_autoretry_behaviour(task)
+        self.tasks[task.name] = task
+        task._app = self
+        task.bind(self)
+        return task
+
+    def gen_task_name(self, name, module):
+        return gen_task_name(self, name, module)
+
+    def finalize(self, auto=False):
+        """Finalize the app.
+
+        This loads built-in tasks, evaluates pending task decorators,
+        reads configuration, etc.
+        """
+        with self._finalize_mutex:
+            if not self.finalized:
+                if auto and not self.autofinalize:
+                    raise RuntimeError('Contract breach: app not finalized')
+                self.finalized = True
+                _announce_app_finalized(self)
+
+                pending = self._pending
+                while pending:
+                    maybe_evaluate(pending.popleft())
+
+                for task in self._tasks.values():
+                    task.bind(self)
+
+                self.on_after_finalize.send(sender=self)
+
+    def add_defaults(self, fun):
+        """Add default configuration from dict ``d``.
+
+        If the argument is a callable function then it will be regarded
+        as a promise, and it won't be loaded until the configuration is
+        actually needed.
+
+        This method can be compared to:
+
+        .. code-block:: pycon
+
+            >>> celery.conf.update(d)
+
+        with a difference that 1) no copy will be made and 2) the dict will
+        not be transferred when the worker spawns child processes, so
+        it's important that the same configuration happens at import time
+        when pickle restores the object on the other side.
+        """
+        if not callable(fun):
+            d, fun = fun, lambda: d
+        if self.configured:
+            return self._conf.add_defaults(fun())
+        self._pending_defaults.append(fun)
+
+    def config_from_object(self, obj,
+                           silent=False, force=False, namespace=None):
+        """Read configuration from object.
+
+        Object is either an actual object or the name of a module to import.
+
+        Example:
+            >>> celery.config_from_object('myapp.celeryconfig')
+
+            >>> from myapp import celeryconfig
+            >>> celery.config_from_object(celeryconfig)
+
+        Arguments:
+            silent (bool): If true then import errors will be ignored.
+            force (bool): Force reading configuration immediately.
+                By default the configuration will be read only when required.
+        """
+        self._config_source = obj
+        self.namespace = namespace or self.namespace
+        if force or self.configured:
+            self._conf = None
+            if self.loader.config_from_object(obj, silent=silent):
+                return self.conf
+
+    def config_from_envvar(self, variable_name, silent=False, force=False):
+        """Read configuration from environment variable.
+
+        The value of the environment variable must be the name
+        of a module to import.
+
+        Example:
+            >>> os.environ['CELERY_CONFIG_MODULE'] = 'myapp.celeryconfig'
+            >>> celery.config_from_envvar('CELERY_CONFIG_MODULE')
+        """
+        module_name = os.environ.get(variable_name)
+        if not module_name:
+            if silent:
+                return False
+            raise ImproperlyConfigured(
+                ERR_ENVVAR_NOT_SET.strip().format(variable_name))
+        return self.config_from_object(module_name, silent=silent, force=force)
+
+    def config_from_cmdline(self, argv, namespace='celery'):
+        self._conf.update(
+            self.loader.cmdline_config_parser(argv, namespace)
+        )
+
+    def setup_security(self, allowed_serializers=None, key=None, cert=None,
+                       store=None, digest=DEFAULT_SECURITY_DIGEST,
+                       serializer='json'):
+        """Setup the message-signing serializer.
+
+        This will affect all application instances (a global operation).
+
+        Disables untrusted serializers and if configured to use the ``auth``
+        serializer will register the ``auth`` serializer with the provided
+        settings into the Kombu serializer registry.
+
+        Arguments:
+            allowed_serializers (Set[str]): List of serializer names, or
+                content_types that should be exempt from being disabled.
+            key (str): Name of private key file to use.
+                Defaults to the :setting:`security_key` setting.
+            cert (str): Name of certificate file to use.
+                Defaults to the :setting:`security_certificate` setting.
+            store (str): Directory containing certificates.
+                Defaults to the :setting:`security_cert_store` setting.
+            digest (str): Digest algorithm used when signing messages.
+                Default is ``sha256``.
+            serializer (str): Serializer used to encode messages after
+                they've been signed.  See :setting:`task_serializer` for
+                the serializers supported.  Default is ``json``.
+        """
+        from celery.security import setup_security
+        return setup_security(allowed_serializers, key, cert,
+                              store, digest, serializer, app=self)
+
+    def autodiscover_tasks(self, packages=None,
+                           related_name='tasks', force=False):
+        """Auto-discover task modules.
+
+        Searches a list of packages for a "tasks.py" module (or use
+        related_name argument).
+
+        If the name is empty, this will be delegated to fix-ups (e.g., Django).
+
+        For example if you have a directory layout like this:
+
+        .. code-block:: text
+
+            foo/__init__.py
+               tasks.py
+               models.py
+
+            bar/__init__.py
+                tasks.py
+                models.py
+
+            baz/__init__.py
+                models.py
+
+        Then calling ``app.autodiscover_tasks(['foo', 'bar', 'baz'])`` will
+        result in the modules ``foo.tasks`` and ``bar.tasks`` being imported.
+
+        Arguments:
+            packages (List[str]): List of packages to search.
+                This argument may also be a callable, in which case the
+                value returned is used (for lazy evaluation).
+            related_name (Optional[str]): The name of the module to find.  Defaults
+                to "tasks": meaning "look for 'module.tasks' for every
+                module in ``packages``.".  If ``None`` will only try to import
+                the package, i.e. "look for 'module'".
+            force (bool): By default this call is lazy so that the actual
+                auto-discovery won't happen until an application imports
+                the default modules.  Forcing will cause the auto-discovery
+                to happen immediately.
+        """
+        if force:
+            return self._autodiscover_tasks(packages, related_name)
+        signals.import_modules.connect(starpromise(
+            self._autodiscover_tasks, packages, related_name,
+        ), weak=False, sender=self)
+
+    def _autodiscover_tasks(self, packages, related_name, **kwargs):
+        if packages:
+            return self._autodiscover_tasks_from_names(packages, related_name)
+        return self._autodiscover_tasks_from_fixups(related_name)
+
+    def _autodiscover_tasks_from_names(self, packages, related_name):
+        # packages argument can be lazy
+        return self.loader.autodiscover_tasks(
+            packages() if callable(packages) else packages, related_name,
+        )
+
+    def _autodiscover_tasks_from_fixups(self, related_name):
+        return self._autodiscover_tasks_from_names([
+            pkg for fixup in self._fixups
+            if hasattr(fixup, 'autodiscover_tasks')
+            for pkg in fixup.autodiscover_tasks()
+        ], related_name=related_name)
+
+    def send_task(self, name, args=None, kwargs=None, countdown=None,
+                  eta=None, task_id=None, producer=None, connection=None,
+                  router=None, result_cls=None, expires=None,
+                  publisher=None, link=None, link_error=None,
+                  add_to_parent=True, group_id=None, group_index=None,
+                  retries=0, chord=None,
+                  reply_to=None, time_limit=None, soft_time_limit=None,
+                  root_id=None, parent_id=None, route_name=None,
+                  shadow=None, chain=None, task_type=None, **options):
+        """Send task by name.
+
+        Supports the same arguments as :meth:`@-Task.apply_async`.
+
+        Arguments:
+            name (str): Name of task to call (e.g., `"tasks.add"`).
+            result_cls (AsyncResult): Specify custom result class.
+        """
+        parent = have_parent = None
+        amqp = self.amqp
+        task_id = task_id or uuid()
+        producer = producer or publisher  # XXX compat
+        router = router or amqp.router
+        conf = self.conf
+        if conf.task_always_eager:  # pragma: no cover
+            warnings.warn(AlwaysEagerIgnored(
+                'task_always_eager has no effect on send_task',
+            ), stacklevel=2)
+
+        ignored_result = options.pop('ignore_result', False)
+        options = router.route(
+            options, route_name or name, args, kwargs, task_type)
+
+        if not root_id or not parent_id:
+            parent = self.current_worker_task
+            if parent:
+                if not root_id:
+                    root_id = parent.request.root_id or parent.request.id
+                if not parent_id:
+                    parent_id = parent.request.id
+
+                if conf.task_inherit_parent_priority:
+                    options.setdefault('priority',
+                                       parent.request.delivery_info.get('priority'))
+
+        message = amqp.create_task_message(
+            task_id, name, args, kwargs, countdown, eta, group_id, group_index,
+            expires, retries, chord,
+            maybe_list(link), maybe_list(link_error),
+            reply_to or self.thread_oid, time_limit, soft_time_limit,
+            self.conf.task_send_sent_event,
+            root_id, parent_id, shadow, chain,
+            argsrepr=options.get('argsrepr'),
+            kwargsrepr=options.get('kwargsrepr'),
+        )
+
+        if connection:
+            producer = amqp.Producer(connection, auto_declare=False)
+
+        with self.producer_or_acquire(producer) as P:
+            with P.connection._reraise_as_library_errors():
+                if not ignored_result:
+                    self.backend.on_task_call(P, task_id)
+                amqp.send_task_message(P, name, message, **options)
+        result = (result_cls or self.AsyncResult)(task_id)
+        # We avoid using the constructor since a custom result class
+        # can be used, in which case the constructor may still use
+        # the old signature.
+        result.ignored = ignored_result
+
+        if add_to_parent:
+            if not have_parent:
+                parent, have_parent = self.current_worker_task, True
+            if parent:
+                parent.add_trail(result)
+        return result
+
+    def connection_for_read(self, url=None, **kwargs):
+        """Establish connection used for consuming.
+
+        See Also:
+            :meth:`connection` for supported arguments.
+        """
+        return self._connection(url or self.conf.broker_read_url, **kwargs)
+
+    def connection_for_write(self, url=None, **kwargs):
+        """Establish connection used for producing.
+
+        See Also:
+            :meth:`connection` for supported arguments.
+        """
+        return self._connection(url or self.conf.broker_write_url, **kwargs)
+
+    def connection(self, hostname=None, userid=None, password=None,
+                   virtual_host=None, port=None, ssl=None,
+                   connect_timeout=None, transport=None,
+                   transport_options=None, heartbeat=None,
+                   login_method=None, failover_strategy=None, **kwargs):
+        """Establish a connection to the message broker.
+
+        Please use :meth:`connection_for_read` and
+        :meth:`connection_for_write` instead, to convey the intent
+        of use for this connection.
+
+        Arguments:
+            url: Either the URL or the hostname of the broker to use.
+            hostname (str): URL, Hostname/IP-address of the broker.
+                If a URL is used, then the other argument below will
+                be taken from the URL instead.
+            userid (str): Username to authenticate as.
+            password (str): Password to authenticate with
+            virtual_host (str): Virtual host to use (domain).
+            port (int): Port to connect to.
+            ssl (bool, Dict): Defaults to the :setting:`broker_use_ssl`
+                setting.
+            transport (str): defaults to the :setting:`broker_transport`
+                setting.
+            transport_options (Dict): Dictionary of transport specific options.
+            heartbeat (int): AMQP Heartbeat in seconds (``pyamqp`` only).
+            login_method (str): Custom login method to use (AMQP only).
+            failover_strategy (str, Callable): Custom failover strategy.
+            **kwargs: Additional arguments to :class:`kombu.Connection`.
+
+        Returns:
+            kombu.Connection: the lazy connection instance.
+        """
+        return self.connection_for_write(
+            hostname or self.conf.broker_write_url,
+            userid=userid, password=password,
+            virtual_host=virtual_host, port=port, ssl=ssl,
+            connect_timeout=connect_timeout, transport=transport,
+            transport_options=transport_options, heartbeat=heartbeat,
+            login_method=login_method, failover_strategy=failover_strategy,
+            **kwargs
+        )
+
+    def _connection(self, url, userid=None, password=None,
+                    virtual_host=None, port=None, ssl=None,
+                    connect_timeout=None, transport=None,
+                    transport_options=None, heartbeat=None,
+                    login_method=None, failover_strategy=None, **kwargs):
+        conf = self.conf
+        return self.amqp.Connection(
+            url,
+            userid or conf.broker_user,
+            password or conf.broker_password,
+            virtual_host or conf.broker_vhost,
+            port or conf.broker_port,
+            transport=transport or conf.broker_transport,
+            ssl=self.either('broker_use_ssl', ssl),
+            heartbeat=heartbeat,
+            login_method=login_method or conf.broker_login_method,
+            failover_strategy=(
+                failover_strategy or conf.broker_failover_strategy
+            ),
+            transport_options=dict(
+                conf.broker_transport_options, **transport_options or {}
+            ),
+            connect_timeout=self.either(
+                'broker_connection_timeout', connect_timeout
+            ),
+        )
+    broker_connection = connection
+
+    def _acquire_connection(self, pool=True):
+        """Helper for :meth:`connection_or_acquire`."""
+        if pool:
+            return self.pool.acquire(block=True)
+        return self.connection_for_write()
+
+    def connection_or_acquire(self, connection=None, pool=True, *_, **__):
+        """Context used to acquire a connection from the pool.
+
+        For use within a :keyword:`with` statement to get a connection
+        from the pool if one is not already provided.
+
+        Arguments:
+            connection (kombu.Connection): If not provided, a connection
+                will be acquired from the connection pool.
+        """
+        return FallbackContext(connection, self._acquire_connection, pool=pool)
+    default_connection = connection_or_acquire  # XXX compat
+
+    def producer_or_acquire(self, producer=None):
+        """Context used to acquire a producer from the pool.
+
+        For use within a :keyword:`with` statement to get a producer
+        from the pool if one is not already provided
+
+        Arguments:
+            producer (kombu.Producer): If not provided, a producer
+                will be acquired from the producer pool.
+        """
+        return FallbackContext(
+            producer, self.producer_pool.acquire, block=True,
+        )
+    default_producer = producer_or_acquire  # XXX compat
+
+    def prepare_config(self, c):
+        """Prepare configuration before it is merged with the defaults."""
+        return find_deprecated_settings(c)
+
+    def now(self):
+        """Return the current time and date as a datetime."""
+        now_in_utc = to_utc(datetime.utcnow())
+        return now_in_utc.astimezone(self.timezone)
+
+    def select_queues(self, queues=None):
+        """Select subset of queues.
+
+        Arguments:
+            queues (Sequence[str]): a list of queue names to keep.
+        """
+        return self.amqp.queues.select(queues)
+
+    def either(self, default_key, *defaults):
+        """Get key from configuration or use default values.
+
+        Fallback to the value of a configuration key if none of the
+        `*values` are true.
+        """
+        return first(None, [
+            first(None, defaults), starpromise(self.conf.get, default_key),
+        ])
+
+    def bugreport(self):
+        """Return information useful in bug reports."""
+        return bugreport(self)
+
+    def _get_backend(self):
+        backend, url = backends.by_url(
+            self.backend_cls or self.conf.result_backend,
+            self.loader)
+        return backend(app=self, url=url)
+
+    def _finalize_pending_conf(self):
+        """Get config value by key and finalize loading the configuration.
+
+        Note:
+            This is used by PendingConfiguration:
+                as soon as you access a key the configuration is read.
+        """
+        conf = self._conf = self._load_config()
+        return conf
+
+    def _load_config(self):
+        if isinstance(self.on_configure, Signal):
+            self.on_configure.send(sender=self)
+        else:
+            # used to be a method pre 4.0
+            self.on_configure()
+        if self._config_source:
+            self.loader.config_from_object(self._config_source)
+        self.configured = True
+        settings = detect_settings(
+            self.prepare_config(self.loader.conf), self._preconf,
+            ignore_keys=self._preconf_set_by_auto, prefix=self.namespace,
+        )
+        if self._conf is not None:
+            # replace in place, as someone may have referenced app.conf,
+            # done some changes, accessed a key, and then try to make more
+            # changes to the reference and not the finalized value.
+            self._conf.swap_with(settings)
+        else:
+            self._conf = settings
+
+        # load lazy config dict initializers.
+        pending_def = self._pending_defaults
+        while pending_def:
+            self._conf.add_defaults(maybe_evaluate(pending_def.popleft()()))
+
+        # load lazy periodic tasks
+        pending_beat = self._pending_periodic_tasks
+        while pending_beat:
+            self._add_periodic_task(*pending_beat.popleft())
+
+        self.on_after_configure.send(sender=self, source=self._conf)
+        return self._conf
+
+    def _after_fork(self):
+        self._pool = None
+        try:
+            self.__dict__['amqp']._producer_pool = None
+        except (AttributeError, KeyError):
+            pass
+        self.on_after_fork.send(sender=self)
+
+    def signature(self, *args, **kwargs):
+        """Return a new :class:`~celery.Signature` bound to this app."""
+        kwargs['app'] = self
+        return self._canvas.signature(*args, **kwargs)
+
+    def add_periodic_task(self, schedule, sig,
+                          args=(), kwargs=(), name=None, **opts):
+        key, entry = self._sig_to_periodic_task_entry(
+            schedule, sig, args, kwargs, name, **opts)
+        if self.configured:
+            self._add_periodic_task(key, entry)
+        else:
+            self._pending_periodic_tasks.append((key, entry))
+        return key
+
+    def _sig_to_periodic_task_entry(self, schedule, sig,
+                                    args=(), kwargs=None, name=None, **opts):
+        kwargs = {} if not kwargs else kwargs
+        sig = (sig.clone(args, kwargs)
+               if isinstance(sig, abstract.CallableSignature)
+               else self.signature(sig.name, args, kwargs))
+        return name or repr(sig), {
+            'schedule': schedule,
+            'task': sig.name,
+            'args': sig.args,
+            'kwargs': sig.kwargs,
+            'options': dict(sig.options, **opts),
+        }
+
+    def _add_periodic_task(self, key, entry):
+        self._conf.beat_schedule[key] = entry
+
+    def create_task_cls(self):
+        """Create a base task class bound to this app."""
+        return self.subclass_with_self(
+            self.task_cls, name='Task', attribute='_app',
+            keep_reduce=True, abstract=True,
+        )
+
+    def subclass_with_self(self, Class, name=None, attribute='app',
+                           reverse=None, keep_reduce=False, **kw):
+        """Subclass an app-compatible class.
+
+        App-compatible means that the class has a class attribute that
+        provides the default app it should use, for example:
+        ``class Foo: app = None``.
+
+        Arguments:
+            Class (type): The app-compatible class to subclass.
+            name (str): Custom name for the target class.
+            attribute (str): Name of the attribute holding the app,
+                Default is 'app'.
+            reverse (str): Reverse path to this object used for pickling
+                purposes. For example, to get ``app.AsyncResult``,
+                use ``"AsyncResult"``.
+            keep_reduce (bool): If enabled a custom ``__reduce__``
+                implementation won't be provided.
+        """
+        Class = symbol_by_name(Class)
+        reverse = reverse if reverse else Class.__name__
+
+        def __reduce__(self):
+            return _unpickle_appattr, (reverse, self.__reduce_args__())
+
+        attrs = dict(
+            {attribute: self},
+            __module__=Class.__module__,
+            __doc__=Class.__doc__,
+            **kw)
+        if not keep_reduce:
+            attrs['__reduce__'] = __reduce__
+
+        return type(name or Class.__name__, (Class,), attrs)
+
+    def _rgetattr(self, path):
+        return attrgetter(path)(self)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *exc_info):
+        self.close()
+
+    def __repr__(self):
+        return '<{} {}>'.format(type(self).__name__, appstr(self))
+
+    def __reduce__(self):
+        if self._using_v1_reduce:
+            return self.__reduce_v1__()
+        return (_unpickle_app_v2, (self.__class__, self.__reduce_keys__()))
+
+    def __reduce_v1__(self):
+        # Reduce only pickles the configuration changes,
+        # so the default configuration doesn't have to be passed
+        # between processes.
+        return (
+            _unpickle_app,
+            (self.__class__, self.Pickler) + self.__reduce_args__(),
+        )
+
+    def __reduce_keys__(self):
+        """Keyword arguments used to reconstruct the object when unpickling."""
+        return {
+            'main': self.main,
+            'changes':
+                self._conf.changes if self.configured else self._preconf,
+            'loader': self.loader_cls,
+            'backend': self.backend_cls,
+            'amqp': self.amqp_cls,
+            'events': self.events_cls,
+            'log': self.log_cls,
+            'control': self.control_cls,
+            'fixups': self.fixups,
+            'config_source': self._config_source,
+            'task_cls': self.task_cls,
+            'namespace': self.namespace,
+        }
+
+    def __reduce_args__(self):
+        """Deprecated method, please use :meth:`__reduce_keys__` instead."""
+        return (self.main, self._conf.changes if self.configured else {},
+                self.loader_cls, self.backend_cls, self.amqp_cls,
+                self.events_cls, self.log_cls, self.control_cls,
+                False, self._config_source)
+
+    @cached_property
+    def Worker(self):
+        """Worker application.
+
+        See Also:
+            :class:`~@Worker`.
+        """
+        return self.subclass_with_self('celery.apps.worker:Worker')
+
+    @cached_property
+    def WorkController(self, **kwargs):
+        """Embeddable worker.
+
+        See Also:
+            :class:`~@WorkController`.
+        """
+        return self.subclass_with_self('celery.worker:WorkController')
+
+    @cached_property
+    def Beat(self, **kwargs):
+        """:program:`celery beat` scheduler application.
+
+        See Also:
+            :class:`~@Beat`.
+        """
+        return self.subclass_with_self('celery.apps.beat:Beat')
+
+    @cached_property
+    def Task(self):
+        """Base task class for this app."""
+        return self.create_task_cls()
+
+    @cached_property
+    def annotations(self):
+        return prepare_annotations(self.conf.task_annotations)
+
+    @cached_property
+    def AsyncResult(self):
+        """Create new result instance.
+
+        See Also:
+            :class:`celery.result.AsyncResult`.
+        """
+        return self.subclass_with_self('celery.result:AsyncResult')
+
+    @cached_property
+    def ResultSet(self):
+        return self.subclass_with_self('celery.result:ResultSet')
+
+    @cached_property
+    def GroupResult(self):
+        """Create new group result instance.
+
+        See Also:
+            :class:`celery.result.GroupResult`.
+        """
+        return self.subclass_with_self('celery.result:GroupResult')
+
+    @property
+    def pool(self):
+        """Broker connection pool: :class:`~@pool`.
+
+        Note:
+            This attribute is not related to the workers concurrency pool.
+        """
+        if self._pool is None:
+            self._ensure_after_fork()
+            limit = self.conf.broker_pool_limit
+            pools.set_limit(limit)
+            self._pool = pools.connections[self.connection_for_write()]
+        return self._pool
+
+    @property
+    def current_task(self):
+        """Instance of task being executed, or :const:`None`."""
+        return _task_stack.top
+
+    @property
+    def current_worker_task(self):
+        """The task currently being executed by a worker or :const:`None`.
+
+        Differs from :data:`current_task` in that it's not affected
+        by tasks calling other tasks directly, or eagerly.
+        """
+        return get_current_worker_task()
+
+    @cached_property
+    def oid(self):
+        """Universally unique identifier for this app."""
+        # since 4.0: thread.get_ident() is not included when
+        # generating the process id.  This is due to how the RPC
+        # backend now dedicates a single thread to receive results,
+        # which would not work if each thread has a separate id.
+        return oid_from(self, threads=False)
+
+    @property
+    def thread_oid(self):
+        """Per-thread unique identifier for this app."""
+        try:
+            return self._local.oid
+        except AttributeError:
+            self._local.oid = new_oid = oid_from(self, threads=True)
+            return new_oid
+
+    @cached_property
+    def amqp(self):
+        """AMQP related functionality: :class:`~@amqp`."""
+        return instantiate(self.amqp_cls, app=self)
+
+    @property
+    def backend(self):
+        """Current backend instance."""
+        try:
+            return self._local.backend
+        except AttributeError:
+            self._local.backend = new_backend = self._get_backend()
+            return new_backend
+
+    @property
+    def conf(self):
+        """Current configuration."""
+        if self._conf is None:
+            self._conf = self._load_config()
+        return self._conf
+
+    @conf.setter
+    def conf(self, d):  # noqa
+        self._conf = d
+
+    @cached_property
+    def control(self):
+        """Remote control: :class:`~@control`."""
+        return instantiate(self.control_cls, app=self)
+
+    @cached_property
+    def events(self):
+        """Consuming and sending events: :class:`~@events`."""
+        return instantiate(self.events_cls, app=self)
+
+    @cached_property
+    def loader(self):
+        """Current loader instance."""
+        return get_loader_cls(self.loader_cls)(app=self)
+
+    @cached_property
+    def log(self):
+        """Logging: :class:`~@log`."""
+        return instantiate(self.log_cls, app=self)
+
+    @cached_property
+    def _canvas(self):
+        from celery import canvas
+        return canvas
+
+    @cached_property
+    def tasks(self):
+        """Task registry.
+
+        Warning:
+            Accessing this attribute will also auto-finalize the app.
+        """
+        self.finalize(auto=True)
+        return self._tasks
+
+    @property
+    def producer_pool(self):
+        return self.amqp.producer_pool
+
+    def uses_utc_timezone(self):
+        """Check if the application uses the UTC timezone."""
+        return self.timezone == timezone.utc
+
+    @cached_property
+    def timezone(self):
+        """Current timezone for this app.
+
+        This is a cached property taking the time zone from the
+        :setting:`timezone` setting.
+        """
+        conf = self.conf
+        if not conf.timezone:
+            if conf.enable_utc:
+                return timezone.utc
+            else:
+                return timezone.local
+        return timezone.get_timezone(conf.timezone)
+
+    # -----------------------------------------------------------------------------
+    # asyncio support
+    _aio_pool = None
+
+    aio_task_cls = 'celery.aio.task:AioTask'
+    aio_amqp_cls = 'celery.aio.amqp:AioAMQP'
+    aio_events_cls = 'celery.aio.events:Events'
+    aio_control_cls = 'celery.aio.control:Control'
+
+    def create_aio_task_cls(self):
+        """Create a base task class bound to this app."""
+        return self.subclass_with_self(
+            self.aio_task_cls, name='AioTask', attribute='_app',
+            keep_reduce=True, abstract=True,
+        )
+
+    @cached_property
+    def AioTask(self):
+        """Base aio-task class for this app."""
+        return self.create_aio_task_cls()
+
+    @cached_property
+    def aio_amqp(self):
+        """AMQP related functionality: :class:`~@aio_amqp`."""
+        return instantiate(self.aio_amqp_cls, app=self)
+
+    @cached_property
+    def aio_events(self):
+        """Consuming and sending events: :class:`~@events`."""
+        return instantiate(self.aio_events_cls, app=self)
+
+    @property
+    def aio_producer_pool(self):
+        return self.aio_amqp.producer_pool
+
+    @property
+    def aio_pool(self):
+        if self._aio_pool is None:
+            self._ensure_after_fork()
+            limit = self.conf.broker_pool_limit
+            pools.set_limit(limit)
+            self._aio_pool = pools.connections[self.aconnection_for_write()]
+        return self._aio_pool
+
+    @cached_property
+    def aio_control(self):
+        """Remote control: :class:`~@control`."""
+        return instantiate(self.aio_control_cls, app=self)
+
+    @cached_property
+    def AioAsyncResult(self):
+        return self.subclass_with_self('celery.aio.result:AsyncResult')
+
+    @cached_property
+    def AioGroupResult(self):
+        return self.subclass_with_self('celery.aio.result:GroupResult')
+
+    def aio_producer_or_acquire(self, producer=None):
+        """Context used to acquire a producer from the pool.
+
+        For use within a :keyword:`with` statement to get a producer
+        from the pool if one is not already provided
+
+        Arguments:
+            producer (kombu.Producer): If not provided, a producer
+                will be acquired from the producer pool.
+        """
+        return AsyncFallbackContext(
+            producer, self.aio_producer_pool.acquire, block=True,
+        )
+
+    @asynccontextmanager
+    async def _aio_acquire_connection(self, pool=True):
+        """Helper for :meth:`connection_or_acquire`."""
+        if pool:
+            async with self.aio_pool.acquire(block=True) as conn:
+                yield conn
+        else:
+            yield self.aconnection_for_write()
+
+    def aio_connection_or_acquire(self, connection=None, pool=True, *_, **__):
+        return AsyncFallbackContext(
+            connection, self._aio_acquire_connection, pool=pool
+        )
+
+    async def asend_task(self, name, args=None, kwargs=None, countdown=None,
+                  eta=None, task_id=None, producer=None, connection=None,
+                  router=None, result_cls=None, expires=None,
+                  publisher=None, link=None, link_error=None,
+                  add_to_parent=True, group_id=None, group_index=None,
+                  retries=0, chord=None,
+                  reply_to=None, time_limit=None, soft_time_limit=None,
+                  root_id=None, parent_id=None, route_name=None,
+                  shadow=None, chain=None, task_type=None, **options):
+        """Send task by name.
+
+        Supports the same arguments as :meth:`@-Task.apply_async`.
+
+        Arguments:
+            name (str): Name of task to call (e.g., `"tasks.add"`).
+            result_cls (AsyncResult): Specify custom result class.
+        """
+        parent = have_parent = None
+        amqp = self.aio_amqp
+        task_id = task_id or uuid()
+        producer = producer or publisher  # XXX compat
+        router = router or amqp.router
+        conf = self.conf
+        if conf.task_always_eager:  # pragma: no cover
+            warnings.warn(AlwaysEagerIgnored(
+                'task_always_eager has no effect on send_task',
+            ), stacklevel=2)
+
+        ignored_result = options.pop('ignore_result', False)
+        options = router.route(
+            options, route_name or name, args, kwargs, task_type)
+
+        if not root_id or not parent_id:
+            parent = self.current_worker_task
+            if parent:
+                if not root_id:
+                    root_id = parent.request.root_id or parent.request.id
+                if not parent_id:
+                    parent_id = parent.request.id
+
+                if conf.task_inherit_parent_priority:
+                    options.setdefault('priority',
+                                       parent.request.delivery_info.get('priority'))
+
+        message = amqp.create_task_message(
+            task_id, name, args, kwargs, countdown, eta, group_id, group_index,
+            expires, retries, chord,
+            maybe_list(link), maybe_list(link_error),
+            reply_to or self.thread_oid, time_limit, soft_time_limit,
+            self.conf.task_send_sent_event,
+            root_id, parent_id, shadow, chain,
+            argsrepr=options.get('argsrepr'),
+            kwargsrepr=options.get('kwargsrepr'),
+        )
+
+        if connection:
+            producer = amqp.Producer(connection, auto_declare=False)
+
+        async with self.aio_producer_or_acquire(producer) as P:
+            with (await P.connection)._reraise_as_library_errors():
+                if not ignored_result:
+                    await self.aio_backend.on_task_call(P, task_id)
+                await amqp.send_task_message(P, name, message, **options)
+        result = (result_cls or self.AsyncResult)(task_id)
+        # We avoid using the constructor since a custom result class
+        # can be used, in which case the constructor may still use
+        # the old signature.
+        result.ignored = ignored_result
+
+        if add_to_parent:
+            if not have_parent:
+                parent, have_parent = self.current_worker_task, True
+            if parent:
+                parent.add_trail(result)
+        return result
+
+    def aconnection_for_read(self, url=None, **kwargs):
+        """Establish connection used for consuming.
+
+        See Also:
+            :meth:`connection` for supported arguments.
+        """
+        return self._aconnection(url or self.conf.broker_read_url, **kwargs)
+
+    def aconnection_for_write(self, url=None, **kwargs):
+        """Establish connection used for producing.
+
+        See Also:
+            :meth:`connection` for supported arguments.
+        """
+        return self._aconnection(url or self.conf.broker_write_url, **kwargs)
+
+    def _aconnection(self, url, userid=None, password=None,
+                    virtual_host=None, port=None, ssl=None,
+                    connect_timeout=None, transport=None,
+                    transport_options=None, heartbeat=None,
+                    login_method=None, failover_strategy=None, **kwargs):
+        conf = self.conf
+        return self.aio_amqp.Connection(
+            url,
+            userid or conf.broker_user,
+            password or conf.broker_password,
+            virtual_host or conf.broker_vhost,
+            port or conf.broker_port,
+            transport=transport or conf.broker_transport,
+            ssl=self.either('broker_use_ssl', ssl),
+            heartbeat=heartbeat,
+            login_method=login_method or conf.broker_login_method,
+            failover_strategy=(
+                failover_strategy or conf.broker_failover_strategy
+            ),
+            transport_options=dict(
+                conf.broker_transport_options, **transport_options or {}
+            ),
+            connect_timeout=self.either(
+                'broker_connection_timeout', connect_timeout
+            ),
+        )
+
+    @property
+    def aio_backend(self):
+        """Current backend instance."""
+        try:
+            return self._local.aio_backend
+        except AttributeError:
+            override_backends = self.loader.override_backends
+            ori_redis = override_backends.pop('redis', None)
+            ori_rediss = override_backends.pop('rediss', None)
+            ori_sentinel = override_backends.pop('sentinel', None)
+            override_backends['redis'] = override_backends['rediss'] \
+                = 'celery.aio.backend:RedisBackend'
+            override_backends['sentinel'] = 'celery.aio.backend:SentinelBackend'
+            try:
+                self._local.aio_backend = new_backend = self._get_backend()
+            finally:
+                if ori_redis is not None:
+                    override_backends['redis'] = ori_rediss
+                else:
+                    override_backends.pop('redis', None)
+
+                if ori_rediss is not None:
+                    override_backends['rediss'] = ori_rediss
+                else:
+                    override_backends.pop('rediss', None)
+
+                if ori_sentinel is not None:
+                    override_backends['sentinel'] = ori_sentinel
+                else:
+                    override_backends.pop('sentinel', None)
+            return new_backend
+
+
+App = Celery  # noqa: E305 XXX compat
```

### Comparing `deepfos-celery-1.0.2/celery/app/builtins.py` & `deepfos-celery-1.0.3/celery/app/builtins.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/control.py` & `deepfos-celery-1.0.3/celery/app/control.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/defaults.py` & `deepfos-celery-1.0.3/celery/app/defaults.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/events.py` & `deepfos-celery-1.0.3/celery/app/events.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/log.py` & `deepfos-celery-1.0.3/celery/app/log.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/registry.py` & `deepfos-celery-1.0.3/celery/app/registry.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/routes.py` & `deepfos-celery-1.0.3/celery/app/routes.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/task.py` & `deepfos-celery-1.0.3/celery/app/task.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1079 +1,1079 @@
-"""Task implementation: request context and the task base class."""
-import sys
-
-from billiard.einfo import ExceptionInfo
-from kombu import serialization
-from kombu.exceptions import OperationalError
-from kombu.utils.uuid import uuid
-
-from celery import current_app, group, states
-from celery._state import _task_stack
-from celery.canvas import _chain, signature
-from celery.exceptions import (Ignore, ImproperlyConfigured,
-                               MaxRetriesExceededError, Reject, Retry)
-from celery.local import class_property
-from celery.result import EagerResult, denied_join_result
-from celery.utils import abstract
-from celery.utils.functional import mattrgetter, maybe_list
-from celery.utils.imports import instantiate
-from celery.utils.nodenames import gethostname
-from celery.utils.serialization import raise_with_context
-
-from .annotations import resolve_all as resolve_all_annotations
-from .registry import _unpickle_task_v2
-from .utils import appstr
-
-__all__ = ('Context', 'Task')
-
-#: extracts attributes related to publishing a message from an object.
-extract_exec_options = mattrgetter(
-    'queue', 'routing_key', 'exchange', 'priority', 'expires',
-    'serializer', 'delivery_mode', 'compression', 'time_limit',
-    'soft_time_limit', 'immediate', 'mandatory',  # imm+man is deprecated
-)
-
-# We take __repr__ very seriously around here ;)
-R_BOUND_TASK = '<class {0.__name__} of {app}{flags}>'
-R_UNBOUND_TASK = '<unbound {0.__name__}{flags}>'
-R_INSTANCE = '<@task: {0.name} of {app}{flags}>'
-
-#: Here for backwards compatibility as tasks no longer use a custom meta-class.
-TaskType = type
-
-
-def _strflags(flags, default=''):
-    if flags:
-        return ' ({})'.format(', '.join(flags))
-    return default
-
-
-def _reprtask(task, fmt=None, flags=None):
-    flags = list(flags) if flags is not None else []
-    flags.append('v2 compatible') if task.__v2_compat__ else None
-    if not fmt:
-        fmt = R_BOUND_TASK if task._app else R_UNBOUND_TASK
-    return fmt.format(
-        task, flags=_strflags(flags),
-        app=appstr(task._app) if task._app else None,
-    )
-
-
-class Context:
-    """Task request variables (Task.request)."""
-
-    logfile = None
-    loglevel = None
-    hostname = None
-    id = None
-    args = None
-    kwargs = None
-    retries = 0
-    eta = None
-    expires = None
-    is_eager = False
-    headers = None
-    delivery_info = None
-    reply_to = None
-    root_id = None
-    parent_id = None
-    correlation_id = None
-    taskset = None   # compat alias to group
-    group = None
-    group_index = None
-    chord = None
-    chain = None
-    utc = None
-    called_directly = True
-    callbacks = None
-    errbacks = None
-    timelimit = None
-    origin = None
-    _children = None   # see property
-    _protected = 0
-
-    def __init__(self, *args, **kwargs):
-        self.update(*args, **kwargs)
-
-    def update(self, *args, **kwargs):
-        return self.__dict__.update(*args, **kwargs)
-
-    def clear(self):
-        return self.__dict__.clear()
-
-    def get(self, key, default=None):
-        return getattr(self, key, default)
-
-    def __repr__(self):
-        return '<Context: {!r}>'.format(vars(self))
-
-    def as_execution_options(self):
-        limit_hard, limit_soft = self.timelimit or (None, None)
-        return {
-            'task_id': self.id,
-            'root_id': self.root_id,
-            'parent_id': self.parent_id,
-            'group_id': self.group,
-            'group_index': self.group_index,
-            'chord': self.chord,
-            'chain': self.chain,
-            'link': self.callbacks,
-            'link_error': self.errbacks,
-            'expires': self.expires,
-            'soft_time_limit': limit_soft,
-            'time_limit': limit_hard,
-            'headers': self.headers,
-            'retries': self.retries,
-            'reply_to': self.reply_to,
-            'origin': self.origin,
-        }
-
-    @property
-    def children(self):
-        # children must be an empty list for every thread
-        if self._children is None:
-            self._children = []
-        return self._children
-
-
-@abstract.CallableTask.register
-class Task:
-    """Task base class.
-
-    Note:
-        When called tasks apply the :meth:`run` method.  This method must
-        be defined by all tasks (that is unless the :meth:`__call__` method
-        is overridden).
-    """
-
-    __trace__ = None
-    __v2_compat__ = False  # set by old base in celery.task.base
-
-    MaxRetriesExceededError = MaxRetriesExceededError
-    OperationalError = OperationalError
-
-    #: Execution strategy used, or the qualified name of one.
-    Strategy = 'celery.worker.strategy:default'
-
-    #: Request class used, or the qualified name of one.
-    Request = 'celery.worker.request:Request'
-
-    #: The application instance associated with this task class.
-    _app = None
-
-    #: Name of the task.
-    name = None
-
-    #: Enable argument checking.
-    #: You can set this to false if you don't want the signature to be
-    #: checked when calling the task.
-    #: Defaults to :attr:`app.strict_typing <@Celery.strict_typing>`.
-    typing = None
-
-    #: Maximum number of retries before giving up.  If set to :const:`None`,
-    #: it will **never** stop retrying.
-    max_retries = 3
-
-    #: Default time in seconds before a retry of the task should be
-    #: executed.  3 minutes by default.
-    default_retry_delay = 3 * 60
-
-    #: Rate limit for this task type.  Examples: :const:`None` (no rate
-    #: limit), `'100/s'` (hundred tasks a second), `'100/m'` (hundred tasks
-    #: a minute),`'100/h'` (hundred tasks an hour)
-    rate_limit = None
-
-    #: If enabled the worker won't store task state and return values
-    #: for this task.  Defaults to the :setting:`task_ignore_result`
-    #: setting.
-    ignore_result = None
-
-    #: If enabled the request will keep track of subtasks started by
-    #: this task, and this information will be sent with the result
-    #: (``result.children``).
-    trail = True
-
-    #: If enabled the worker will send monitoring events related to
-    #: this task (but only if the worker is configured to send
-    #: task related events).
-    #: Note that this has no effect on the task-failure event case
-    #: where a task is not registered (as it will have no task class
-    #: to check this flag).
-    send_events = True
-
-    #: When enabled errors will be stored even if the task is otherwise
-    #: configured to ignore results.
-    store_errors_even_if_ignored = None
-
-    #: The name of a serializer that are registered with
-    #: :mod:`kombu.serialization.registry`.  Default is `'json'`.
-    serializer = None
-
-    #: Hard time limit.
-    #: Defaults to the :setting:`task_time_limit` setting.
-    time_limit = None
-
-    #: Soft time limit.
-    #: Defaults to the :setting:`task_soft_time_limit` setting.
-    soft_time_limit = None
-
-    #: The result store backend used for this task.
-    backend = None
-
-    #: If disabled this task won't be registered automatically.
-    autoregister = True
-
-    #: If enabled the task will report its status as 'started' when the task
-    #: is executed by a worker.  Disabled by default as the normal behavior
-    #: is to not report that level of granularity.  Tasks are either pending,
-    #: finished, or waiting to be retried.
-    #:
-    #: Having a 'started' status can be useful for when there are long
-    #: running tasks and there's a need to report what task is currently
-    #: running.
-    #:
-    #: The application default can be overridden using the
-    #: :setting:`task_track_started` setting.
-    track_started = None
-
-    #: When enabled messages for this task will be acknowledged **after**
-    #: the task has been executed, and not *just before* (the
-    #: default behavior).
-    #:
-    #: Please note that this means the task may be executed twice if the
-    #: worker crashes mid execution.
-    #:
-    #: The application default can be overridden with the
-    #: :setting:`task_acks_late` setting.
-    acks_late = None
-
-    #: When enabled messages for this task will be acknowledged even if it
-    #: fails or times out.
-    #:
-    #: Configuring this setting only applies to tasks that are
-    #: acknowledged **after** they have been executed and only if
-    #: :setting:`task_acks_late` is enabled.
-    #:
-    #: The application default can be overridden with the
-    #: :setting:`task_acks_on_failure_or_timeout` setting.
-    acks_on_failure_or_timeout = None
-
-    #: Even if :attr:`acks_late` is enabled, the worker will
-    #: acknowledge tasks when the worker process executing them abruptly
-    #: exits or is signaled (e.g., :sig:`KILL`/:sig:`INT`, etc).
-    #:
-    #: Setting this to true allows the message to be re-queued instead,
-    #: so that the task will execute again by the same worker, or another
-    #: worker.
-    #:
-    #: Warning: Enabling this can cause message loops; make sure you know
-    #: what you're doing.
-    reject_on_worker_lost = None
-
-    #: Tuple of expected exceptions.
-    #:
-    #: These are errors that are expected in normal operation
-    #: and that shouldn't be regarded as a real error by the worker.
-    #: Currently this means that the state will be updated to an error
-    #: state, but the worker won't log the event as an error.
-    throws = ()
-
-    #: Default task expiry time.
-    expires = None
-
-    #: Default task priority.
-    priority = None
-
-    #: Max length of result representation used in logs and events.
-    resultrepr_maxsize = 1024
-
-    #: Task request stack, the current request will be the topmost.
-    request_stack = None
-
-    #: Some may expect a request to exist even if the task hasn't been
-    #: called.  This should probably be deprecated.
-    _default_request = None
-
-    #: Deprecated attribute ``abstract`` here for compatibility.
-    abstract = True
-
-    _exec_options = None
-
-    __bound__ = False
-
-    from_config = (
-        ('serializer', 'task_serializer'),
-        ('rate_limit', 'task_default_rate_limit'),
-        ('priority', 'task_default_priority'),
-        ('track_started', 'task_track_started'),
-        ('acks_late', 'task_acks_late'),
-        ('acks_on_failure_or_timeout', 'task_acks_on_failure_or_timeout'),
-        ('reject_on_worker_lost', 'task_reject_on_worker_lost'),
-        ('ignore_result', 'task_ignore_result'),
-        ('store_errors_even_if_ignored', 'task_store_errors_even_if_ignored'),
-    )
-
-    _backend = None  # set by backend property.
-
-    # - Tasks are lazily bound, so that configuration is not set
-    # - until the task is actually used
-
-    @classmethod
-    def bind(cls, app):
-        was_bound, cls.__bound__ = cls.__bound__, True
-        cls._app = app
-        conf = app.conf
-        cls._exec_options = None  # clear option cache
-
-        if cls.typing is None:
-            cls.typing = app.strict_typing
-
-        for attr_name, config_name in cls.from_config:
-            if getattr(cls, attr_name, None) is None:
-                setattr(cls, attr_name, conf[config_name])
-
-        # decorate with annotations from config.
-        if not was_bound:
-            cls.annotate()
-
-            from celery.utils.threads import LocalStack
-            cls.request_stack = LocalStack()
-
-        # PeriodicTask uses this to add itself to the PeriodicTask schedule.
-        cls.on_bound(app)
-
-        return app
-
-    @classmethod
-    def on_bound(cls, app):
-        """Called when the task is bound to an app.
-
-        Note:
-            This class method can be defined to do additional actions when
-            the task class is bound to an app.
-        """
-
-    @classmethod
-    def _get_app(cls):
-        if cls._app is None:
-            cls._app = current_app
-        if not cls.__bound__:
-            # The app property's __set__  method is not called
-            # if Task.app is set (on the class), so must bind on use.
-            cls.bind(cls._app)
-        return cls._app
-    app = class_property(_get_app, bind)
-
-    @classmethod
-    def annotate(cls):
-        for d in resolve_all_annotations(cls.app.annotations, cls):
-            for key, value in d.items():
-                if key.startswith('@'):
-                    cls.add_around(key[1:], value)
-                else:
-                    setattr(cls, key, value)
-
-    @classmethod
-    def add_around(cls, attr, around):
-        orig = getattr(cls, attr)
-        if getattr(orig, '__wrapped__', None):
-            orig = orig.__wrapped__
-        meth = around(orig)
-        meth.__wrapped__ = orig
-        setattr(cls, attr, meth)
-
-    def __call__(self, *args, **kwargs):
-        _task_stack.push(self)
-        self.push_request(args=args, kwargs=kwargs)
-        try:
-            return self.run(*args, **kwargs)
-        finally:
-            self.pop_request()
-            _task_stack.pop()
-
-    def __reduce__(self):
-        # - tasks are pickled into the name of the task only, and the receiver
-        # - simply grabs it from the local registry.
-        # - in later versions the module of the task is also included,
-        # - and the receiving side tries to import that module so that
-        # - it will work even if the task hasn't been registered.
-        mod = type(self).__module__
-        mod = mod if mod and mod in sys.modules else None
-        return (_unpickle_task_v2, (self.name, mod), None)
-
-    def run(self, *args, **kwargs):
-        """The body of the task executed by workers."""
-        raise NotImplementedError('Tasks must define the run method.')
-
-    def start_strategy(self, app, consumer, **kwargs):
-        return instantiate(self.Strategy, self, app, consumer, **kwargs)
-
-    def delay(self, *args, **kwargs):
-        """Star argument version of :meth:`apply_async`.
-
-        Does not support the extra options enabled by :meth:`apply_async`.
-
-        Arguments:
-            *args (Any): Positional arguments passed on to the task.
-            **kwargs (Any): Keyword arguments passed on to the task.
-        Returns:
-            celery.result.AsyncResult: Future promise.
-        """
-        return self.apply_async(args, kwargs)
-
-    def apply_async(self, args=None, kwargs=None, task_id=None, producer=None,
-                    link=None, link_error=None, shadow=None, **options):
-        """Apply tasks asynchronously by sending a message.
-
-        Arguments:
-            args (Tuple): The positional arguments to pass on to the task.
-
-            kwargs (Dict): The keyword arguments to pass on to the task.
-
-            countdown (float): Number of seconds into the future that the
-                task should execute.  Defaults to immediate execution.
-
-            eta (~datetime.datetime): Absolute time and date of when the task
-                should be executed.  May not be specified if `countdown`
-                is also supplied.
-
-            expires (float, ~datetime.datetime): Datetime or
-                seconds in the future for the task should expire.
-                The task won't be executed after the expiration time.
-
-            shadow (str): Override task name used in logs/monitoring.
-                Default is retrieved from :meth:`shadow_name`.
-
-            connection (kombu.Connection): Re-use existing broker connection
-                instead of acquiring one from the connection pool.
-
-            retry (bool): If enabled sending of the task message will be
-                retried in the event of connection loss or failure.
-                Default is taken from the :setting:`task_publish_retry`
-                setting.  Note that you need to handle the
-                producer/connection manually for this to work.
-
-            retry_policy (Mapping): Override the retry policy used.
-                See the :setting:`task_publish_retry_policy` setting.
-
-            queue (str, kombu.Queue): The queue to route the task to.
-                This must be a key present in :setting:`task_queues`, or
-                :setting:`task_create_missing_queues` must be
-                enabled.  See :ref:`guide-routing` for more
-                information.
-
-            exchange (str, kombu.Exchange): Named custom exchange to send the
-                task to.  Usually not used in combination with the ``queue``
-                argument.
-
-            routing_key (str): Custom routing key used to route the task to a
-                worker server.  If in combination with a ``queue`` argument
-                only used to specify custom routing keys to topic exchanges.
-
-            priority (int): The task priority, a number between 0 and 9.
-                Defaults to the :attr:`priority` attribute.
-
-            serializer (str): Serialization method to use.
-                Can be `pickle`, `json`, `yaml`, `msgpack` or any custom
-                serialization method that's been registered
-                with :mod:`kombu.serialization.registry`.
-                Defaults to the :attr:`serializer` attribute.
-
-            compression (str): Optional compression method
-                to use.  Can be one of ``zlib``, ``bzip2``,
-                or any custom compression methods registered with
-                :func:`kombu.compression.register`.
-                Defaults to the :setting:`task_compression` setting.
-
-            link (Signature): A single, or a list of tasks signatures
-                to apply if the task returns successfully.
-
-            link_error (Signature): A single, or a list of task signatures
-                to apply if an error occurs while executing the task.
-
-            producer (kombu.Producer): custom producer to use when publishing
-                the task.
-
-            add_to_parent (bool): If set to True (default) and the task
-                is applied while executing another task, then the result
-                will be appended to the parent tasks ``request.children``
-                attribute.  Trailing can also be disabled by default using the
-                :attr:`trail` attribute
-
-            publisher (kombu.Producer): Deprecated alias to ``producer``.
-
-            headers (Dict): Message headers to be included in the message.
-
-        Returns:
-            celery.result.AsyncResult: Promise of future evaluation.
-
-        Raises:
-            TypeError: If not enough arguments are passed, or too many
-                arguments are passed.  Note that signature checks may
-                be disabled by specifying ``@task(typing=False)``.
-            kombu.exceptions.OperationalError: If a connection to the
-               transport cannot be made, or if the connection is lost.
-
-        Note:
-            Also supports all keyword arguments supported by
-            :meth:`kombu.Producer.publish`.
-        """
-        if self.typing:
-            try:
-                check_arguments = self.__header__
-            except AttributeError:  # pragma: no cover
-                pass
-            else:
-                check_arguments(*(args or ()), **(kwargs or {}))
-
-        if self.__v2_compat__:
-            shadow = shadow or self.shadow_name(self(), args, kwargs, options)
-        else:
-            shadow = shadow or self.shadow_name(args, kwargs, options)
-
-        preopts = self._get_exec_options()
-        options = dict(preopts, **options) if options else preopts
-
-        options.setdefault('ignore_result', self.ignore_result)
-        if self.priority:
-            options.setdefault('priority', self.priority)
-
-        app = self._get_app()
-        if app.conf.task_always_eager:
-            with app.producer_or_acquire(producer) as eager_producer:
-                serializer = options.get('serializer')
-                if serializer is None:
-                    if eager_producer.serializer:
-                        serializer = eager_producer.serializer
-                    else:
-                        serializer = app.conf.task_serializer
-                body = args, kwargs
-                content_type, content_encoding, data = serialization.dumps(
-                    body, serializer,
-                )
-                args, kwargs = serialization.loads(
-                    data, content_type, content_encoding,
-                    accept=[content_type]
-                )
-            with denied_join_result():
-                return self.apply(args, kwargs, task_id=task_id or uuid(),
-                                  link=link, link_error=link_error, **options)
-        else:
-            return app.send_task(
-                self.name, args, kwargs, task_id=task_id, producer=producer,
-                link=link, link_error=link_error, result_cls=self.AsyncResult,
-                shadow=shadow, task_type=self,
-                **options
-            )
-
-    def shadow_name(self, args, kwargs, options):
-        """Override for custom task name in worker logs/monitoring.
-
-        Example:
-            .. code-block:: python
-
-                from celery.utils.imports import qualname
-
-                def shadow_name(task, args, kwargs, options):
-                    return qualname(args[0])
-
-                @app.task(shadow_name=shadow_name, serializer='pickle')
-                def apply_function_async(fun, *args, **kwargs):
-                    return fun(*args, **kwargs)
-
-        Arguments:
-            args (Tuple): Task positional arguments.
-            kwargs (Dict): Task keyword arguments.
-            options (Dict): Task execution options.
-        """
-
-    def signature_from_request(self, request=None, args=None, kwargs=None,
-                               queue=None, **extra_options):
-        request = self.request if request is None else request
-        args = request.args if args is None else args
-        kwargs = request.kwargs if kwargs is None else kwargs
-        options = request.as_execution_options()
-        delivery_info = request.delivery_info or {}
-        priority = delivery_info.get('priority')
-        if priority is not None:
-            options['priority'] = priority
-        if queue:
-            options['queue'] = queue
-        else:
-            exchange = delivery_info.get('exchange')
-            routing_key = delivery_info.get('routing_key')
-            if exchange == '' and routing_key:
-                # sent to anon-exchange
-                options['queue'] = routing_key
-            else:
-                options.update(delivery_info)
-        return self.signature(
-            args, kwargs, options, type=self, **extra_options
-        )
-    subtask_from_request = signature_from_request  # XXX compat
-
-    def retry(self, args=None, kwargs=None, exc=None, throw=True,
-              eta=None, countdown=None, max_retries=None, **options):
-        """Retry the task, adding it to the back of the queue.
-
-        Example:
-            >>> from imaginary_twitter_lib import Twitter
-            >>> from proj.celery import app
-
-            >>> @app.task(bind=True)
-            ... def tweet(self, auth, message):
-            ...     twitter = Twitter(oauth=auth)
-            ...     try:
-            ...         twitter.post_status_update(message)
-            ...     except twitter.FailWhale as exc:
-            ...         # Retry in 5 minutes.
-            ...         self.retry(countdown=60 * 5, exc=exc)
-
-        Note:
-            Although the task will never return above as `retry` raises an
-            exception to notify the worker, we use `raise` in front of the
-            retry to convey that the rest of the block won't be executed.
-
-        Arguments:
-            args (Tuple): Positional arguments to retry with.
-            kwargs (Dict): Keyword arguments to retry with.
-            exc (Exception): Custom exception to report when the max retry
-                limit has been exceeded (default:
-                :exc:`~@MaxRetriesExceededError`).
-
-                If this argument is set and retry is called while
-                an exception was raised (``sys.exc_info()`` is set)
-                it will attempt to re-raise the current exception.
-
-                If no exception was raised it will raise the ``exc``
-                argument provided.
-            countdown (float): Time in seconds to delay the retry for.
-            eta (~datetime.datetime): Explicit time and date to run the
-                retry at.
-            max_retries (int): If set, overrides the default retry limit for
-                this execution.  Changes to this parameter don't propagate to
-                subsequent task retry attempts.  A value of :const:`None`,
-                means "use the default", so if you want infinite retries you'd
-                have to set the :attr:`max_retries` attribute of the task to
-                :const:`None` first.
-            time_limit (int): If set, overrides the default time limit.
-            soft_time_limit (int): If set, overrides the default soft
-                time limit.
-            throw (bool): If this is :const:`False`, don't raise the
-                :exc:`~@Retry` exception, that tells the worker to mark
-                the task as being retried.  Note that this means the task
-                will be marked as failed if the task raises an exception,
-                or successful if it returns after the retry call.
-            **options (Any): Extra options to pass on to :meth:`apply_async`.
-
-        Raises:
-
-            celery.exceptions.Retry:
-                To tell the worker that the task has been re-sent for retry.
-                This always happens, unless the `throw` keyword argument
-                has been explicitly set to :const:`False`, and is considered
-                normal operation.
-        """
-        request = self.request
-        retries = request.retries + 1
-        if max_retries is not None:
-            self.override_max_retries = max_retries
-        max_retries = self.max_retries if max_retries is None else max_retries
-
-        # Not in worker or emulated by (apply/always_eager),
-        # so just raise the original exception.
-        if request.called_directly:
-            # raises orig stack if PyErr_Occurred,
-            # and augments with exc' if that argument is defined.
-            raise_with_context(exc or Retry('Task can be retried', None))
-
-        if not eta and countdown is None:
-            countdown = self.default_retry_delay
-
-        is_eager = request.is_eager
-        S = self.signature_from_request(
-            request, args, kwargs,
-            countdown=countdown, eta=eta, retries=retries,
-            **options
-        )
-
-        if max_retries is not None and retries > max_retries:
-            if exc:
-                # On Py3: will augment any current exception with
-                # the exc' argument provided (raise exc from orig)
-                raise_with_context(exc)
-            raise self.MaxRetriesExceededError(
-                "Can't retry {}[{}] args:{} kwargs:{}".format(
-                    self.name, request.id, S.args, S.kwargs
-                ), task_args=S.args, task_kwargs=S.kwargs
-            )
-
-        ret = Retry(exc=exc, when=eta or countdown, is_eager=is_eager, sig=S)
-
-        if is_eager:
-            # if task was executed eagerly using apply(),
-            # then the retry must also be executed eagerly in apply method
-            if throw:
-                raise ret
-            return ret
-
-        try:
-            S.apply_async()
-        except Exception as exc:
-            raise Reject(exc, requeue=False)
-        if throw:
-            raise ret
-        return ret
-
-    def apply(self, args=None, kwargs=None,
-              link=None, link_error=None,
-              task_id=None, retries=None, throw=None,
-              logfile=None, loglevel=None, headers=None, **options):
-        """Execute this task locally, by blocking until the task returns.
-
-        Arguments:
-            args (Tuple): positional arguments passed on to the task.
-            kwargs (Dict): keyword arguments passed on to the task.
-            throw (bool): Re-raise task exceptions.
-                Defaults to the :setting:`task_eager_propagates` setting.
-
-        Returns:
-            celery.result.EagerResult: pre-evaluated result.
-        """
-        # trace imports Task, so need to import inline.
-        from celery.app.trace import build_tracer
-
-        app = self._get_app()
-        args = args or ()
-        kwargs = kwargs or {}
-        task_id = task_id or uuid()
-        retries = retries or 0
-        if throw is None:
-            throw = app.conf.task_eager_propagates
-
-        # Make sure we get the task instance, not class.
-        task = app._tasks[self.name]
-
-        request = {
-            'id': task_id,
-            'retries': retries,
-            'is_eager': True,
-            'logfile': logfile,
-            'loglevel': loglevel or 0,
-            'hostname': gethostname(),
-            'callbacks': maybe_list(link),
-            'errbacks': maybe_list(link_error),
-            'headers': headers,
-            'delivery_info': {'is_eager': True},
-        }
-        tb = None
-        tracer = build_tracer(
-            task.name, task, eager=True,
-            propagate=throw, app=self._get_app(),
-        )
-        ret = tracer(task_id, args, kwargs, request)
-        retval = ret.retval
-        if isinstance(retval, ExceptionInfo):
-            retval, tb = retval.exception, retval.traceback
-        if isinstance(retval, Retry) and retval.sig is not None:
-            return retval.sig.apply(retries=retries + 1)
-        state = states.SUCCESS if ret.info is None else ret.info.state
-        return EagerResult(task_id, retval, state, traceback=tb)
-
-    def AsyncResult(self, task_id, **kwargs):
-        """Get AsyncResult instance for the specified task.
-
-        Arguments:
-            task_id (str): Task id to get result for.
-        """
-        return self._get_app().AsyncResult(task_id, backend=self.backend,
-                                           task_name=self.name, **kwargs)
-
-    def signature(self, args=None, *starargs, **starkwargs):
-        """Create signature.
-
-        Returns:
-            :class:`~celery.signature`:  object for
-                this task, wrapping arguments and execution options
-                for a single task invocation.
-        """
-        starkwargs.setdefault('app', self.app)
-        return signature(self, args, *starargs, **starkwargs)
-    subtask = signature
-
-    def s(self, *args, **kwargs):
-        """Create signature.
-
-        Shortcut for ``.s(*a, **k) -> .signature(a, k)``.
-        """
-        return self.signature(args, kwargs)
-
-    def si(self, *args, **kwargs):
-        """Create immutable signature.
-
-        Shortcut for ``.si(*a, **k) -> .signature(a, k, immutable=True)``.
-        """
-        return self.signature(args, kwargs, immutable=True)
-
-    def chunks(self, it, n):
-        """Create a :class:`~celery.canvas.chunks` task for this task."""
-        from celery import chunks
-        return chunks(self.s(), it, n, app=self.app)
-
-    def map(self, it):
-        """Create a :class:`~celery.canvas.xmap` task from ``it``."""
-        from celery import xmap
-        return xmap(self.s(), it, app=self.app)
-
-    def starmap(self, it):
-        """Create a :class:`~celery.canvas.xstarmap` task from ``it``."""
-        from celery import xstarmap
-        return xstarmap(self.s(), it, app=self.app)
-
-    def send_event(self, type_, retry=True, retry_policy=None, **fields):
-        """Send monitoring event message.
-
-        This can be used to add custom event types in :pypi:`Flower`
-        and other monitors.
-
-        Arguments:
-            type_ (str):  Type of event, e.g. ``"task-failed"``.
-
-        Keyword Arguments:
-            retry (bool):  Retry sending the message
-                if the connection is lost.  Default is taken from the
-                :setting:`task_publish_retry` setting.
-            retry_policy (Mapping): Retry settings.  Default is taken
-                from the :setting:`task_publish_retry_policy` setting.
-            **fields (Any): Map containing information about the event.
-                Must be JSON serializable.
-        """
-        req = self.request
-        if retry_policy is None:
-            retry_policy = self.app.conf.task_publish_retry_policy
-        with self.app.events.default_dispatcher(hostname=req.hostname) as d:
-            return d.send(
-                type_,
-                uuid=req.id, retry=retry, retry_policy=retry_policy, **fields)
-
-    def replace(self, sig):
-        """Replace this task, with a new task inheriting the task id.
-
-        Execution of the host task ends immediately and no subsequent statements
-        will be run.
-
-        .. versionadded:: 4.0
-
-        Arguments:
-            sig (~@Signature): signature to replace with.
-
-        Raises:
-            ~@Ignore: This is always raised when called in asynchronous context.
-            It is best to always use ``return self.replace(...)`` to convey
-            to the reader that the task won't continue after being replaced.
-        """
-        chord = self.request.chord
-        if 'chord' in sig.options:
-            raise ImproperlyConfigured(
-                "A signature replacing a task must not be part of a chord"
-            )
-
-        if isinstance(sig, group):
-            sig |= self.app.tasks['celery.accumulate'].s(index=0).set(
-                link=self.request.callbacks,
-                link_error=self.request.errbacks,
-            )
-        elif isinstance(sig, _chain):
-            if not sig.tasks:
-                raise ImproperlyConfigured(
-                    "Cannot replace with an empty chain"
-                )
-
-        if self.request.chain:
-            # We need to freeze the new signature with the current task's ID to
-            # ensure that we don't disassociate the new chain from the existing
-            # task IDs which would break previously constructed results
-            # objects.
-            sig.freeze(self.request.id)
-            if "link" in sig.options:
-                final_task_links = sig.tasks[-1].options.setdefault("link", [])
-                final_task_links.extend(maybe_list(sig.options["link"]))
-            # Construct the new remainder of the task by chaining the signature
-            # we're being replaced by with signatures constructed from the
-            # chain elements in the current request.
-            for t in reversed(self.request.chain):
-                sig |= signature(t, app=self.app)
-
-        sig.set(
-            chord=chord,
-            group_id=self.request.group,
-            group_index=self.request.group_index,
-            root_id=self.request.root_id,
-        )
-        sig.freeze(self.request.id)
-
-        if self.request.is_eager:
-            return sig.apply().get()
-        else:
-            sig.delay()
-            raise Ignore('Replaced by new task')
-
-    def add_to_chord(self, sig, lazy=False):
-        """Add signature to the chord the current task is a member of.
-
-        .. versionadded:: 4.0
-
-        Currently only supported by the Redis result backend.
-
-        Arguments:
-            sig (~@Signature): Signature to extend chord with.
-            lazy (bool): If enabled the new task won't actually be called,
-                and ``sig.delay()`` must be called manually.
-        """
-        if not self.request.chord:
-            raise ValueError('Current task is not member of any chord')
-        sig.set(
-            group_id=self.request.group,
-            group_index=self.request.group_index,
-            chord=self.request.chord,
-            root_id=self.request.root_id,
-        )
-        result = sig.freeze()
-        self.backend.add_to_chord(self.request.group, result)
-        return sig.delay() if not lazy else sig
-
-    def update_state(self, task_id=None, state=None, meta=None, **kwargs):
-        """Update task state.
-
-        Arguments:
-            task_id (str): Id of the task to update.
-                Defaults to the id of the current task.
-            state (str): New state.
-            meta (Dict): State meta-data.
-        """
-        if task_id is None:
-            task_id = self.request.id
-        self.backend.store_result(task_id, meta, state, request=self.request, **kwargs)
-
-    def on_success(self, retval, task_id, args, kwargs):
-        """Success handler.
-
-        Run by the worker if the task executes successfully.
-
-        Arguments:
-            retval (Any): The return value of the task.
-            task_id (str): Unique id of the executed task.
-            args (Tuple): Original arguments for the executed task.
-            kwargs (Dict): Original keyword arguments for the executed task.
-
-        Returns:
-            None: The return value of this handler is ignored.
-        """
-
-    def on_retry(self, exc, task_id, args, kwargs, einfo):
-        """Retry handler.
-
-        This is run by the worker when the task is to be retried.
-
-        Arguments:
-            exc (Exception): The exception sent to :meth:`retry`.
-            task_id (str): Unique id of the retried task.
-            args (Tuple): Original arguments for the retried task.
-            kwargs (Dict): Original keyword arguments for the retried task.
-            einfo (~billiard.einfo.ExceptionInfo): Exception information.
-
-        Returns:
-            None: The return value of this handler is ignored.
-        """
-
-    def on_failure(self, exc, task_id, args, kwargs, einfo):
-        """Error handler.
-
-        This is run by the worker when the task fails.
-
-        Arguments:
-            exc (Exception): The exception raised by the task.
-            task_id (str): Unique id of the failed task.
-            args (Tuple): Original arguments for the task that failed.
-            kwargs (Dict): Original keyword arguments for the task that failed.
-            einfo (~billiard.einfo.ExceptionInfo): Exception information.
-
-        Returns:
-            None: The return value of this handler is ignored.
-        """
-
-    def after_return(self, status, retval, task_id, args, kwargs, einfo):
-        """Handler called after the task returns.
-
-        Arguments:
-            status (str): Current task state.
-            retval (Any): Task return value/exception.
-            task_id (str): Unique id of the task.
-            args (Tuple): Original arguments for the task.
-            kwargs (Dict): Original keyword arguments for the task.
-            einfo (~billiard.einfo.ExceptionInfo): Exception information.
-
-        Returns:
-            None: The return value of this handler is ignored.
-        """
-
-    def add_trail(self, result):
-        if self.trail:
-            self.request.children.append(result)
-        return result
-
-    def push_request(self, *args, **kwargs):
-        self.request_stack.push(Context(*args, **kwargs))
-
-    def pop_request(self):
-        self.request_stack.pop()
-
-    def __repr__(self):
-        """``repr(task)``."""
-        return _reprtask(self, R_INSTANCE)
-
-    def _get_request(self):
-        """Get current request object."""
-        req = self.request_stack.top
-        if req is None:
-            # task was not called, but some may still expect a request
-            # to be there, perhaps that should be deprecated.
-            if self._default_request is None:
-                self._default_request = Context()
-            return self._default_request
-        return req
-    request = property(_get_request)
-
-    def _get_exec_options(self):
-        if self._exec_options is None:
-            self._exec_options = extract_exec_options(self)
-        return self._exec_options
-
-    @property
-    def backend(self):
-        backend = self._backend
-        if backend is None:
-            return self.app.backend
-        return backend
-
-    @backend.setter
-    def backend(self, value):  # noqa
-        self._backend = value
-
-    @property
-    def __name__(self):
-        return self.__class__.__name__
-
-    # -----------------------------------------------------------------------------
-    # asyncio support
-    _aio_variant = None
-
-    @property
-    def aio(self):
-        return self._aio_variant
-
-    @aio.setter
-    def aio(self, value):  # noqa
-        self._aio_variant = value
-
-
-BaseTask = Task  # noqa: E305 XXX compat alias
+"""Task implementation: request context and the task base class."""
+import sys
+
+from billiard.einfo import ExceptionInfo
+from kombu import serialization
+from kombu.exceptions import OperationalError
+from kombu.utils.uuid import uuid
+
+from celery import current_app, group, states
+from celery._state import _task_stack
+from celery.canvas import _chain, signature
+from celery.exceptions import (Ignore, ImproperlyConfigured,
+                               MaxRetriesExceededError, Reject, Retry)
+from celery.local import class_property
+from celery.result import EagerResult, denied_join_result
+from celery.utils import abstract
+from celery.utils.functional import mattrgetter, maybe_list
+from celery.utils.imports import instantiate
+from celery.utils.nodenames import gethostname
+from celery.utils.serialization import raise_with_context
+
+from .annotations import resolve_all as resolve_all_annotations
+from .registry import _unpickle_task_v2
+from .utils import appstr
+
+__all__ = ('Context', 'Task')
+
+#: extracts attributes related to publishing a message from an object.
+extract_exec_options = mattrgetter(
+    'queue', 'routing_key', 'exchange', 'priority', 'expires',
+    'serializer', 'delivery_mode', 'compression', 'time_limit',
+    'soft_time_limit', 'immediate', 'mandatory',  # imm+man is deprecated
+)
+
+# We take __repr__ very seriously around here ;)
+R_BOUND_TASK = '<class {0.__name__} of {app}{flags}>'
+R_UNBOUND_TASK = '<unbound {0.__name__}{flags}>'
+R_INSTANCE = '<@task: {0.name} of {app}{flags}>'
+
+#: Here for backwards compatibility as tasks no longer use a custom meta-class.
+TaskType = type
+
+
+def _strflags(flags, default=''):
+    if flags:
+        return ' ({})'.format(', '.join(flags))
+    return default
+
+
+def _reprtask(task, fmt=None, flags=None):
+    flags = list(flags) if flags is not None else []
+    flags.append('v2 compatible') if task.__v2_compat__ else None
+    if not fmt:
+        fmt = R_BOUND_TASK if task._app else R_UNBOUND_TASK
+    return fmt.format(
+        task, flags=_strflags(flags),
+        app=appstr(task._app) if task._app else None,
+    )
+
+
+class Context:
+    """Task request variables (Task.request)."""
+
+    logfile = None
+    loglevel = None
+    hostname = None
+    id = None
+    args = None
+    kwargs = None
+    retries = 0
+    eta = None
+    expires = None
+    is_eager = False
+    headers = None
+    delivery_info = None
+    reply_to = None
+    root_id = None
+    parent_id = None
+    correlation_id = None
+    taskset = None   # compat alias to group
+    group = None
+    group_index = None
+    chord = None
+    chain = None
+    utc = None
+    called_directly = True
+    callbacks = None
+    errbacks = None
+    timelimit = None
+    origin = None
+    _children = None   # see property
+    _protected = 0
+
+    def __init__(self, *args, **kwargs):
+        self.update(*args, **kwargs)
+
+    def update(self, *args, **kwargs):
+        return self.__dict__.update(*args, **kwargs)
+
+    def clear(self):
+        return self.__dict__.clear()
+
+    def get(self, key, default=None):
+        return getattr(self, key, default)
+
+    def __repr__(self):
+        return '<Context: {!r}>'.format(vars(self))
+
+    def as_execution_options(self):
+        limit_hard, limit_soft = self.timelimit or (None, None)
+        return {
+            'task_id': self.id,
+            'root_id': self.root_id,
+            'parent_id': self.parent_id,
+            'group_id': self.group,
+            'group_index': self.group_index,
+            'chord': self.chord,
+            'chain': self.chain,
+            'link': self.callbacks,
+            'link_error': self.errbacks,
+            'expires': self.expires,
+            'soft_time_limit': limit_soft,
+            'time_limit': limit_hard,
+            'headers': self.headers,
+            'retries': self.retries,
+            'reply_to': self.reply_to,
+            'origin': self.origin,
+        }
+
+    @property
+    def children(self):
+        # children must be an empty list for every thread
+        if self._children is None:
+            self._children = []
+        return self._children
+
+
+@abstract.CallableTask.register
+class Task:
+    """Task base class.
+
+    Note:
+        When called tasks apply the :meth:`run` method.  This method must
+        be defined by all tasks (that is unless the :meth:`__call__` method
+        is overridden).
+    """
+
+    __trace__ = None
+    __v2_compat__ = False  # set by old base in celery.task.base
+
+    MaxRetriesExceededError = MaxRetriesExceededError
+    OperationalError = OperationalError
+
+    #: Execution strategy used, or the qualified name of one.
+    Strategy = 'celery.worker.strategy:default'
+
+    #: Request class used, or the qualified name of one.
+    Request = 'celery.worker.request:Request'
+
+    #: The application instance associated with this task class.
+    _app = None
+
+    #: Name of the task.
+    name = None
+
+    #: Enable argument checking.
+    #: You can set this to false if you don't want the signature to be
+    #: checked when calling the task.
+    #: Defaults to :attr:`app.strict_typing <@Celery.strict_typing>`.
+    typing = None
+
+    #: Maximum number of retries before giving up.  If set to :const:`None`,
+    #: it will **never** stop retrying.
+    max_retries = 3
+
+    #: Default time in seconds before a retry of the task should be
+    #: executed.  3 minutes by default.
+    default_retry_delay = 3 * 60
+
+    #: Rate limit for this task type.  Examples: :const:`None` (no rate
+    #: limit), `'100/s'` (hundred tasks a second), `'100/m'` (hundred tasks
+    #: a minute),`'100/h'` (hundred tasks an hour)
+    rate_limit = None
+
+    #: If enabled the worker won't store task state and return values
+    #: for this task.  Defaults to the :setting:`task_ignore_result`
+    #: setting.
+    ignore_result = None
+
+    #: If enabled the request will keep track of subtasks started by
+    #: this task, and this information will be sent with the result
+    #: (``result.children``).
+    trail = True
+
+    #: If enabled the worker will send monitoring events related to
+    #: this task (but only if the worker is configured to send
+    #: task related events).
+    #: Note that this has no effect on the task-failure event case
+    #: where a task is not registered (as it will have no task class
+    #: to check this flag).
+    send_events = True
+
+    #: When enabled errors will be stored even if the task is otherwise
+    #: configured to ignore results.
+    store_errors_even_if_ignored = None
+
+    #: The name of a serializer that are registered with
+    #: :mod:`kombu.serialization.registry`.  Default is `'json'`.
+    serializer = None
+
+    #: Hard time limit.
+    #: Defaults to the :setting:`task_time_limit` setting.
+    time_limit = None
+
+    #: Soft time limit.
+    #: Defaults to the :setting:`task_soft_time_limit` setting.
+    soft_time_limit = None
+
+    #: The result store backend used for this task.
+    backend = None
+
+    #: If disabled this task won't be registered automatically.
+    autoregister = True
+
+    #: If enabled the task will report its status as 'started' when the task
+    #: is executed by a worker.  Disabled by default as the normal behavior
+    #: is to not report that level of granularity.  Tasks are either pending,
+    #: finished, or waiting to be retried.
+    #:
+    #: Having a 'started' status can be useful for when there are long
+    #: running tasks and there's a need to report what task is currently
+    #: running.
+    #:
+    #: The application default can be overridden using the
+    #: :setting:`task_track_started` setting.
+    track_started = None
+
+    #: When enabled messages for this task will be acknowledged **after**
+    #: the task has been executed, and not *just before* (the
+    #: default behavior).
+    #:
+    #: Please note that this means the task may be executed twice if the
+    #: worker crashes mid execution.
+    #:
+    #: The application default can be overridden with the
+    #: :setting:`task_acks_late` setting.
+    acks_late = None
+
+    #: When enabled messages for this task will be acknowledged even if it
+    #: fails or times out.
+    #:
+    #: Configuring this setting only applies to tasks that are
+    #: acknowledged **after** they have been executed and only if
+    #: :setting:`task_acks_late` is enabled.
+    #:
+    #: The application default can be overridden with the
+    #: :setting:`task_acks_on_failure_or_timeout` setting.
+    acks_on_failure_or_timeout = None
+
+    #: Even if :attr:`acks_late` is enabled, the worker will
+    #: acknowledge tasks when the worker process executing them abruptly
+    #: exits or is signaled (e.g., :sig:`KILL`/:sig:`INT`, etc).
+    #:
+    #: Setting this to true allows the message to be re-queued instead,
+    #: so that the task will execute again by the same worker, or another
+    #: worker.
+    #:
+    #: Warning: Enabling this can cause message loops; make sure you know
+    #: what you're doing.
+    reject_on_worker_lost = None
+
+    #: Tuple of expected exceptions.
+    #:
+    #: These are errors that are expected in normal operation
+    #: and that shouldn't be regarded as a real error by the worker.
+    #: Currently this means that the state will be updated to an error
+    #: state, but the worker won't log the event as an error.
+    throws = ()
+
+    #: Default task expiry time.
+    expires = None
+
+    #: Default task priority.
+    priority = None
+
+    #: Max length of result representation used in logs and events.
+    resultrepr_maxsize = 1024
+
+    #: Task request stack, the current request will be the topmost.
+    request_stack = None
+
+    #: Some may expect a request to exist even if the task hasn't been
+    #: called.  This should probably be deprecated.
+    _default_request = None
+
+    #: Deprecated attribute ``abstract`` here for compatibility.
+    abstract = True
+
+    _exec_options = None
+
+    __bound__ = False
+
+    from_config = (
+        ('serializer', 'task_serializer'),
+        ('rate_limit', 'task_default_rate_limit'),
+        ('priority', 'task_default_priority'),
+        ('track_started', 'task_track_started'),
+        ('acks_late', 'task_acks_late'),
+        ('acks_on_failure_or_timeout', 'task_acks_on_failure_or_timeout'),
+        ('reject_on_worker_lost', 'task_reject_on_worker_lost'),
+        ('ignore_result', 'task_ignore_result'),
+        ('store_errors_even_if_ignored', 'task_store_errors_even_if_ignored'),
+    )
+
+    _backend = None  # set by backend property.
+
+    # - Tasks are lazily bound, so that configuration is not set
+    # - until the task is actually used
+
+    @classmethod
+    def bind(cls, app):
+        was_bound, cls.__bound__ = cls.__bound__, True
+        cls._app = app
+        conf = app.conf
+        cls._exec_options = None  # clear option cache
+
+        if cls.typing is None:
+            cls.typing = app.strict_typing
+
+        for attr_name, config_name in cls.from_config:
+            if getattr(cls, attr_name, None) is None:
+                setattr(cls, attr_name, conf[config_name])
+
+        # decorate with annotations from config.
+        if not was_bound:
+            cls.annotate()
+
+            from celery.utils.threads import LocalStack
+            cls.request_stack = LocalStack()
+
+        # PeriodicTask uses this to add itself to the PeriodicTask schedule.
+        cls.on_bound(app)
+
+        return app
+
+    @classmethod
+    def on_bound(cls, app):
+        """Called when the task is bound to an app.
+
+        Note:
+            This class method can be defined to do additional actions when
+            the task class is bound to an app.
+        """
+
+    @classmethod
+    def _get_app(cls):
+        if cls._app is None:
+            cls._app = current_app
+        if not cls.__bound__:
+            # The app property's __set__  method is not called
+            # if Task.app is set (on the class), so must bind on use.
+            cls.bind(cls._app)
+        return cls._app
+    app = class_property(_get_app, bind)
+
+    @classmethod
+    def annotate(cls):
+        for d in resolve_all_annotations(cls.app.annotations, cls):
+            for key, value in d.items():
+                if key.startswith('@'):
+                    cls.add_around(key[1:], value)
+                else:
+                    setattr(cls, key, value)
+
+    @classmethod
+    def add_around(cls, attr, around):
+        orig = getattr(cls, attr)
+        if getattr(orig, '__wrapped__', None):
+            orig = orig.__wrapped__
+        meth = around(orig)
+        meth.__wrapped__ = orig
+        setattr(cls, attr, meth)
+
+    def __call__(self, *args, **kwargs):
+        _task_stack.push(self)
+        self.push_request(args=args, kwargs=kwargs)
+        try:
+            return self.run(*args, **kwargs)
+        finally:
+            self.pop_request()
+            _task_stack.pop()
+
+    def __reduce__(self):
+        # - tasks are pickled into the name of the task only, and the receiver
+        # - simply grabs it from the local registry.
+        # - in later versions the module of the task is also included,
+        # - and the receiving side tries to import that module so that
+        # - it will work even if the task hasn't been registered.
+        mod = type(self).__module__
+        mod = mod if mod and mod in sys.modules else None
+        return (_unpickle_task_v2, (self.name, mod), None)
+
+    def run(self, *args, **kwargs):
+        """The body of the task executed by workers."""
+        raise NotImplementedError('Tasks must define the run method.')
+
+    def start_strategy(self, app, consumer, **kwargs):
+        return instantiate(self.Strategy, self, app, consumer, **kwargs)
+
+    def delay(self, *args, **kwargs):
+        """Star argument version of :meth:`apply_async`.
+
+        Does not support the extra options enabled by :meth:`apply_async`.
+
+        Arguments:
+            *args (Any): Positional arguments passed on to the task.
+            **kwargs (Any): Keyword arguments passed on to the task.
+        Returns:
+            celery.result.AsyncResult: Future promise.
+        """
+        return self.apply_async(args, kwargs)
+
+    def apply_async(self, args=None, kwargs=None, task_id=None, producer=None,
+                    link=None, link_error=None, shadow=None, **options):
+        """Apply tasks asynchronously by sending a message.
+
+        Arguments:
+            args (Tuple): The positional arguments to pass on to the task.
+
+            kwargs (Dict): The keyword arguments to pass on to the task.
+
+            countdown (float): Number of seconds into the future that the
+                task should execute.  Defaults to immediate execution.
+
+            eta (~datetime.datetime): Absolute time and date of when the task
+                should be executed.  May not be specified if `countdown`
+                is also supplied.
+
+            expires (float, ~datetime.datetime): Datetime or
+                seconds in the future for the task should expire.
+                The task won't be executed after the expiration time.
+
+            shadow (str): Override task name used in logs/monitoring.
+                Default is retrieved from :meth:`shadow_name`.
+
+            connection (kombu.Connection): Re-use existing broker connection
+                instead of acquiring one from the connection pool.
+
+            retry (bool): If enabled sending of the task message will be
+                retried in the event of connection loss or failure.
+                Default is taken from the :setting:`task_publish_retry`
+                setting.  Note that you need to handle the
+                producer/connection manually for this to work.
+
+            retry_policy (Mapping): Override the retry policy used.
+                See the :setting:`task_publish_retry_policy` setting.
+
+            queue (str, kombu.Queue): The queue to route the task to.
+                This must be a key present in :setting:`task_queues`, or
+                :setting:`task_create_missing_queues` must be
+                enabled.  See :ref:`guide-routing` for more
+                information.
+
+            exchange (str, kombu.Exchange): Named custom exchange to send the
+                task to.  Usually not used in combination with the ``queue``
+                argument.
+
+            routing_key (str): Custom routing key used to route the task to a
+                worker server.  If in combination with a ``queue`` argument
+                only used to specify custom routing keys to topic exchanges.
+
+            priority (int): The task priority, a number between 0 and 9.
+                Defaults to the :attr:`priority` attribute.
+
+            serializer (str): Serialization method to use.
+                Can be `pickle`, `json`, `yaml`, `msgpack` or any custom
+                serialization method that's been registered
+                with :mod:`kombu.serialization.registry`.
+                Defaults to the :attr:`serializer` attribute.
+
+            compression (str): Optional compression method
+                to use.  Can be one of ``zlib``, ``bzip2``,
+                or any custom compression methods registered with
+                :func:`kombu.compression.register`.
+                Defaults to the :setting:`task_compression` setting.
+
+            link (Signature): A single, or a list of tasks signatures
+                to apply if the task returns successfully.
+
+            link_error (Signature): A single, or a list of task signatures
+                to apply if an error occurs while executing the task.
+
+            producer (kombu.Producer): custom producer to use when publishing
+                the task.
+
+            add_to_parent (bool): If set to True (default) and the task
+                is applied while executing another task, then the result
+                will be appended to the parent tasks ``request.children``
+                attribute.  Trailing can also be disabled by default using the
+                :attr:`trail` attribute
+
+            publisher (kombu.Producer): Deprecated alias to ``producer``.
+
+            headers (Dict): Message headers to be included in the message.
+
+        Returns:
+            celery.result.AsyncResult: Promise of future evaluation.
+
+        Raises:
+            TypeError: If not enough arguments are passed, or too many
+                arguments are passed.  Note that signature checks may
+                be disabled by specifying ``@task(typing=False)``.
+            kombu.exceptions.OperationalError: If a connection to the
+               transport cannot be made, or if the connection is lost.
+
+        Note:
+            Also supports all keyword arguments supported by
+            :meth:`kombu.Producer.publish`.
+        """
+        if self.typing:
+            try:
+                check_arguments = self.__header__
+            except AttributeError:  # pragma: no cover
+                pass
+            else:
+                check_arguments(*(args or ()), **(kwargs or {}))
+
+        if self.__v2_compat__:
+            shadow = shadow or self.shadow_name(self(), args, kwargs, options)
+        else:
+            shadow = shadow or self.shadow_name(args, kwargs, options)
+
+        preopts = self._get_exec_options()
+        options = dict(preopts, **options) if options else preopts
+
+        options.setdefault('ignore_result', self.ignore_result)
+        if self.priority:
+            options.setdefault('priority', self.priority)
+
+        app = self._get_app()
+        if app.conf.task_always_eager:
+            with app.producer_or_acquire(producer) as eager_producer:
+                serializer = options.get('serializer')
+                if serializer is None:
+                    if eager_producer.serializer:
+                        serializer = eager_producer.serializer
+                    else:
+                        serializer = app.conf.task_serializer
+                body = args, kwargs
+                content_type, content_encoding, data = serialization.dumps(
+                    body, serializer,
+                )
+                args, kwargs = serialization.loads(
+                    data, content_type, content_encoding,
+                    accept=[content_type]
+                )
+            with denied_join_result():
+                return self.apply(args, kwargs, task_id=task_id or uuid(),
+                                  link=link, link_error=link_error, **options)
+        else:
+            return app.send_task(
+                self.name, args, kwargs, task_id=task_id, producer=producer,
+                link=link, link_error=link_error, result_cls=self.AsyncResult,
+                shadow=shadow, task_type=self,
+                **options
+            )
+
+    def shadow_name(self, args, kwargs, options):
+        """Override for custom task name in worker logs/monitoring.
+
+        Example:
+            .. code-block:: python
+
+                from celery.utils.imports import qualname
+
+                def shadow_name(task, args, kwargs, options):
+                    return qualname(args[0])
+
+                @app.task(shadow_name=shadow_name, serializer='pickle')
+                def apply_function_async(fun, *args, **kwargs):
+                    return fun(*args, **kwargs)
+
+        Arguments:
+            args (Tuple): Task positional arguments.
+            kwargs (Dict): Task keyword arguments.
+            options (Dict): Task execution options.
+        """
+
+    def signature_from_request(self, request=None, args=None, kwargs=None,
+                               queue=None, **extra_options):
+        request = self.request if request is None else request
+        args = request.args if args is None else args
+        kwargs = request.kwargs if kwargs is None else kwargs
+        options = request.as_execution_options()
+        delivery_info = request.delivery_info or {}
+        priority = delivery_info.get('priority')
+        if priority is not None:
+            options['priority'] = priority
+        if queue:
+            options['queue'] = queue
+        else:
+            exchange = delivery_info.get('exchange')
+            routing_key = delivery_info.get('routing_key')
+            if exchange == '' and routing_key:
+                # sent to anon-exchange
+                options['queue'] = routing_key
+            else:
+                options.update(delivery_info)
+        return self.signature(
+            args, kwargs, options, type=self, **extra_options
+        )
+    subtask_from_request = signature_from_request  # XXX compat
+
+    def retry(self, args=None, kwargs=None, exc=None, throw=True,
+              eta=None, countdown=None, max_retries=None, **options):
+        """Retry the task, adding it to the back of the queue.
+
+        Example:
+            >>> from imaginary_twitter_lib import Twitter
+            >>> from proj.celery import app
+
+            >>> @app.task(bind=True)
+            ... def tweet(self, auth, message):
+            ...     twitter = Twitter(oauth=auth)
+            ...     try:
+            ...         twitter.post_status_update(message)
+            ...     except twitter.FailWhale as exc:
+            ...         # Retry in 5 minutes.
+            ...         self.retry(countdown=60 * 5, exc=exc)
+
+        Note:
+            Although the task will never return above as `retry` raises an
+            exception to notify the worker, we use `raise` in front of the
+            retry to convey that the rest of the block won't be executed.
+
+        Arguments:
+            args (Tuple): Positional arguments to retry with.
+            kwargs (Dict): Keyword arguments to retry with.
+            exc (Exception): Custom exception to report when the max retry
+                limit has been exceeded (default:
+                :exc:`~@MaxRetriesExceededError`).
+
+                If this argument is set and retry is called while
+                an exception was raised (``sys.exc_info()`` is set)
+                it will attempt to re-raise the current exception.
+
+                If no exception was raised it will raise the ``exc``
+                argument provided.
+            countdown (float): Time in seconds to delay the retry for.
+            eta (~datetime.datetime): Explicit time and date to run the
+                retry at.
+            max_retries (int): If set, overrides the default retry limit for
+                this execution.  Changes to this parameter don't propagate to
+                subsequent task retry attempts.  A value of :const:`None`,
+                means "use the default", so if you want infinite retries you'd
+                have to set the :attr:`max_retries` attribute of the task to
+                :const:`None` first.
+            time_limit (int): If set, overrides the default time limit.
+            soft_time_limit (int): If set, overrides the default soft
+                time limit.
+            throw (bool): If this is :const:`False`, don't raise the
+                :exc:`~@Retry` exception, that tells the worker to mark
+                the task as being retried.  Note that this means the task
+                will be marked as failed if the task raises an exception,
+                or successful if it returns after the retry call.
+            **options (Any): Extra options to pass on to :meth:`apply_async`.
+
+        Raises:
+
+            celery.exceptions.Retry:
+                To tell the worker that the task has been re-sent for retry.
+                This always happens, unless the `throw` keyword argument
+                has been explicitly set to :const:`False`, and is considered
+                normal operation.
+        """
+        request = self.request
+        retries = request.retries + 1
+        if max_retries is not None:
+            self.override_max_retries = max_retries
+        max_retries = self.max_retries if max_retries is None else max_retries
+
+        # Not in worker or emulated by (apply/always_eager),
+        # so just raise the original exception.
+        if request.called_directly:
+            # raises orig stack if PyErr_Occurred,
+            # and augments with exc' if that argument is defined.
+            raise_with_context(exc or Retry('Task can be retried', None))
+
+        if not eta and countdown is None:
+            countdown = self.default_retry_delay
+
+        is_eager = request.is_eager
+        S = self.signature_from_request(
+            request, args, kwargs,
+            countdown=countdown, eta=eta, retries=retries,
+            **options
+        )
+
+        if max_retries is not None and retries > max_retries:
+            if exc:
+                # On Py3: will augment any current exception with
+                # the exc' argument provided (raise exc from orig)
+                raise_with_context(exc)
+            raise self.MaxRetriesExceededError(
+                "Can't retry {}[{}] args:{} kwargs:{}".format(
+                    self.name, request.id, S.args, S.kwargs
+                ), task_args=S.args, task_kwargs=S.kwargs
+            )
+
+        ret = Retry(exc=exc, when=eta or countdown, is_eager=is_eager, sig=S)
+
+        if is_eager:
+            # if task was executed eagerly using apply(),
+            # then the retry must also be executed eagerly in apply method
+            if throw:
+                raise ret
+            return ret
+
+        try:
+            S.apply_async()
+        except Exception as exc:
+            raise Reject(exc, requeue=False)
+        if throw:
+            raise ret
+        return ret
+
+    def apply(self, args=None, kwargs=None,
+              link=None, link_error=None,
+              task_id=None, retries=None, throw=None,
+              logfile=None, loglevel=None, headers=None, **options):
+        """Execute this task locally, by blocking until the task returns.
+
+        Arguments:
+            args (Tuple): positional arguments passed on to the task.
+            kwargs (Dict): keyword arguments passed on to the task.
+            throw (bool): Re-raise task exceptions.
+                Defaults to the :setting:`task_eager_propagates` setting.
+
+        Returns:
+            celery.result.EagerResult: pre-evaluated result.
+        """
+        # trace imports Task, so need to import inline.
+        from celery.app.trace import build_tracer
+
+        app = self._get_app()
+        args = args or ()
+        kwargs = kwargs or {}
+        task_id = task_id or uuid()
+        retries = retries or 0
+        if throw is None:
+            throw = app.conf.task_eager_propagates
+
+        # Make sure we get the task instance, not class.
+        task = app._tasks[self.name]
+
+        request = {
+            'id': task_id,
+            'retries': retries,
+            'is_eager': True,
+            'logfile': logfile,
+            'loglevel': loglevel or 0,
+            'hostname': gethostname(),
+            'callbacks': maybe_list(link),
+            'errbacks': maybe_list(link_error),
+            'headers': headers,
+            'delivery_info': {'is_eager': True},
+        }
+        tb = None
+        tracer = build_tracer(
+            task.name, task, eager=True,
+            propagate=throw, app=self._get_app(),
+        )
+        ret = tracer(task_id, args, kwargs, request)
+        retval = ret.retval
+        if isinstance(retval, ExceptionInfo):
+            retval, tb = retval.exception, retval.traceback
+        if isinstance(retval, Retry) and retval.sig is not None:
+            return retval.sig.apply(retries=retries + 1)
+        state = states.SUCCESS if ret.info is None else ret.info.state
+        return EagerResult(task_id, retval, state, traceback=tb)
+
+    def AsyncResult(self, task_id, **kwargs):
+        """Get AsyncResult instance for the specified task.
+
+        Arguments:
+            task_id (str): Task id to get result for.
+        """
+        return self._get_app().AsyncResult(task_id, backend=self.backend,
+                                           task_name=self.name, **kwargs)
+
+    def signature(self, args=None, *starargs, **starkwargs):
+        """Create signature.
+
+        Returns:
+            :class:`~celery.signature`:  object for
+                this task, wrapping arguments and execution options
+                for a single task invocation.
+        """
+        starkwargs.setdefault('app', self.app)
+        return signature(self, args, *starargs, **starkwargs)
+    subtask = signature
+
+    def s(self, *args, **kwargs):
+        """Create signature.
+
+        Shortcut for ``.s(*a, **k) -> .signature(a, k)``.
+        """
+        return self.signature(args, kwargs)
+
+    def si(self, *args, **kwargs):
+        """Create immutable signature.
+
+        Shortcut for ``.si(*a, **k) -> .signature(a, k, immutable=True)``.
+        """
+        return self.signature(args, kwargs, immutable=True)
+
+    def chunks(self, it, n):
+        """Create a :class:`~celery.canvas.chunks` task for this task."""
+        from celery import chunks
+        return chunks(self.s(), it, n, app=self.app)
+
+    def map(self, it):
+        """Create a :class:`~celery.canvas.xmap` task from ``it``."""
+        from celery import xmap
+        return xmap(self.s(), it, app=self.app)
+
+    def starmap(self, it):
+        """Create a :class:`~celery.canvas.xstarmap` task from ``it``."""
+        from celery import xstarmap
+        return xstarmap(self.s(), it, app=self.app)
+
+    def send_event(self, type_, retry=True, retry_policy=None, **fields):
+        """Send monitoring event message.
+
+        This can be used to add custom event types in :pypi:`Flower`
+        and other monitors.
+
+        Arguments:
+            type_ (str):  Type of event, e.g. ``"task-failed"``.
+
+        Keyword Arguments:
+            retry (bool):  Retry sending the message
+                if the connection is lost.  Default is taken from the
+                :setting:`task_publish_retry` setting.
+            retry_policy (Mapping): Retry settings.  Default is taken
+                from the :setting:`task_publish_retry_policy` setting.
+            **fields (Any): Map containing information about the event.
+                Must be JSON serializable.
+        """
+        req = self.request
+        if retry_policy is None:
+            retry_policy = self.app.conf.task_publish_retry_policy
+        with self.app.events.default_dispatcher(hostname=req.hostname) as d:
+            return d.send(
+                type_,
+                uuid=req.id, retry=retry, retry_policy=retry_policy, **fields)
+
+    def replace(self, sig):
+        """Replace this task, with a new task inheriting the task id.
+
+        Execution of the host task ends immediately and no subsequent statements
+        will be run.
+
+        .. versionadded:: 4.0
+
+        Arguments:
+            sig (~@Signature): signature to replace with.
+
+        Raises:
+            ~@Ignore: This is always raised when called in asynchronous context.
+            It is best to always use ``return self.replace(...)`` to convey
+            to the reader that the task won't continue after being replaced.
+        """
+        chord = self.request.chord
+        if 'chord' in sig.options:
+            raise ImproperlyConfigured(
+                "A signature replacing a task must not be part of a chord"
+            )
+
+        if isinstance(sig, group):
+            sig |= self.app.tasks['celery.accumulate'].s(index=0).set(
+                link=self.request.callbacks,
+                link_error=self.request.errbacks,
+            )
+        elif isinstance(sig, _chain):
+            if not sig.tasks:
+                raise ImproperlyConfigured(
+                    "Cannot replace with an empty chain"
+                )
+
+        if self.request.chain:
+            # We need to freeze the new signature with the current task's ID to
+            # ensure that we don't disassociate the new chain from the existing
+            # task IDs which would break previously constructed results
+            # objects.
+            sig.freeze(self.request.id)
+            if "link" in sig.options:
+                final_task_links = sig.tasks[-1].options.setdefault("link", [])
+                final_task_links.extend(maybe_list(sig.options["link"]))
+            # Construct the new remainder of the task by chaining the signature
+            # we're being replaced by with signatures constructed from the
+            # chain elements in the current request.
+            for t in reversed(self.request.chain):
+                sig |= signature(t, app=self.app)
+
+        sig.set(
+            chord=chord,
+            group_id=self.request.group,
+            group_index=self.request.group_index,
+            root_id=self.request.root_id,
+        )
+        sig.freeze(self.request.id)
+
+        if self.request.is_eager:
+            return sig.apply().get()
+        else:
+            sig.delay()
+            raise Ignore('Replaced by new task')
+
+    def add_to_chord(self, sig, lazy=False):
+        """Add signature to the chord the current task is a member of.
+
+        .. versionadded:: 4.0
+
+        Currently only supported by the Redis result backend.
+
+        Arguments:
+            sig (~@Signature): Signature to extend chord with.
+            lazy (bool): If enabled the new task won't actually be called,
+                and ``sig.delay()`` must be called manually.
+        """
+        if not self.request.chord:
+            raise ValueError('Current task is not member of any chord')
+        sig.set(
+            group_id=self.request.group,
+            group_index=self.request.group_index,
+            chord=self.request.chord,
+            root_id=self.request.root_id,
+        )
+        result = sig.freeze()
+        self.backend.add_to_chord(self.request.group, result)
+        return sig.delay() if not lazy else sig
+
+    def update_state(self, task_id=None, state=None, meta=None, **kwargs):
+        """Update task state.
+
+        Arguments:
+            task_id (str): Id of the task to update.
+                Defaults to the id of the current task.
+            state (str): New state.
+            meta (Dict): State meta-data.
+        """
+        if task_id is None:
+            task_id = self.request.id
+        self.backend.store_result(task_id, meta, state, request=self.request, **kwargs)
+
+    def on_success(self, retval, task_id, args, kwargs):
+        """Success handler.
+
+        Run by the worker if the task executes successfully.
+
+        Arguments:
+            retval (Any): The return value of the task.
+            task_id (str): Unique id of the executed task.
+            args (Tuple): Original arguments for the executed task.
+            kwargs (Dict): Original keyword arguments for the executed task.
+
+        Returns:
+            None: The return value of this handler is ignored.
+        """
+
+    def on_retry(self, exc, task_id, args, kwargs, einfo):
+        """Retry handler.
+
+        This is run by the worker when the task is to be retried.
+
+        Arguments:
+            exc (Exception): The exception sent to :meth:`retry`.
+            task_id (str): Unique id of the retried task.
+            args (Tuple): Original arguments for the retried task.
+            kwargs (Dict): Original keyword arguments for the retried task.
+            einfo (~billiard.einfo.ExceptionInfo): Exception information.
+
+        Returns:
+            None: The return value of this handler is ignored.
+        """
+
+    def on_failure(self, exc, task_id, args, kwargs, einfo):
+        """Error handler.
+
+        This is run by the worker when the task fails.
+
+        Arguments:
+            exc (Exception): The exception raised by the task.
+            task_id (str): Unique id of the failed task.
+            args (Tuple): Original arguments for the task that failed.
+            kwargs (Dict): Original keyword arguments for the task that failed.
+            einfo (~billiard.einfo.ExceptionInfo): Exception information.
+
+        Returns:
+            None: The return value of this handler is ignored.
+        """
+
+    def after_return(self, status, retval, task_id, args, kwargs, einfo):
+        """Handler called after the task returns.
+
+        Arguments:
+            status (str): Current task state.
+            retval (Any): Task return value/exception.
+            task_id (str): Unique id of the task.
+            args (Tuple): Original arguments for the task.
+            kwargs (Dict): Original keyword arguments for the task.
+            einfo (~billiard.einfo.ExceptionInfo): Exception information.
+
+        Returns:
+            None: The return value of this handler is ignored.
+        """
+
+    def add_trail(self, result):
+        if self.trail:
+            self.request.children.append(result)
+        return result
+
+    def push_request(self, *args, **kwargs):
+        self.request_stack.push(Context(*args, **kwargs))
+
+    def pop_request(self):
+        self.request_stack.pop()
+
+    def __repr__(self):
+        """``repr(task)``."""
+        return _reprtask(self, R_INSTANCE)
+
+    def _get_request(self):
+        """Get current request object."""
+        req = self.request_stack.top
+        if req is None:
+            # task was not called, but some may still expect a request
+            # to be there, perhaps that should be deprecated.
+            if self._default_request is None:
+                self._default_request = Context()
+            return self._default_request
+        return req
+    request = property(_get_request)
+
+    def _get_exec_options(self):
+        if self._exec_options is None:
+            self._exec_options = extract_exec_options(self)
+        return self._exec_options
+
+    @property
+    def backend(self):
+        backend = self._backend
+        if backend is None:
+            return self.app.backend
+        return backend
+
+    @backend.setter
+    def backend(self, value):  # noqa
+        self._backend = value
+
+    @property
+    def __name__(self):
+        return self.__class__.__name__
+
+    # -----------------------------------------------------------------------------
+    # asyncio support
+    _aio_variant = None
+
+    @property
+    def aio(self):
+        return self._aio_variant
+
+    @aio.setter
+    def aio(self, value):  # noqa
+        self._aio_variant = value
+
+
+BaseTask = Task  # noqa: E305 XXX compat alias
```

### Comparing `deepfos-celery-1.0.2/celery/app/trace.py` & `deepfos-celery-1.0.3/celery/app/trace.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/app/utils.py` & `deepfos-celery-1.0.3/celery/app/utils.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/apps/beat.py` & `deepfos-celery-1.0.3/celery/apps/beat.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/apps/multi.py` & `deepfos-celery-1.0.3/celery/apps/multi.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/apps/worker.py` & `deepfos-celery-1.0.3/celery/apps/worker.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/arangodb.py` & `deepfos-celery-1.0.3/celery/backends/arangodb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/asynchronous.py` & `deepfos-celery-1.0.3/celery/backends/asynchronous.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/azureblockblob.py` & `deepfos-celery-1.0.3/celery/backends/azureblockblob.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/base.py` & `deepfos-celery-1.0.3/celery/backends/base.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/cache.py` & `deepfos-celery-1.0.3/celery/backends/cache.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/cassandra.py` & `deepfos-celery-1.0.3/celery/backends/cassandra.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/consul.py` & `deepfos-celery-1.0.3/celery/backends/consul.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/cosmosdbsql.py` & `deepfos-celery-1.0.3/celery/backends/cosmosdbsql.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/couchbase.py` & `deepfos-celery-1.0.3/celery/backends/couchbase.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/couchdb.py` & `deepfos-celery-1.0.3/celery/backends/couchdb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/database/__init__.py` & `deepfos-celery-1.0.3/celery/backends/database/__init__.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/database/models.py` & `deepfos-celery-1.0.3/celery/backends/database/models.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/database/session.py` & `deepfos-celery-1.0.3/celery/backends/database/session.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/dynamodb.py` & `deepfos-celery-1.0.3/celery/backends/dynamodb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/elasticsearch.py` & `deepfos-celery-1.0.3/celery/backends/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/filesystem.py` & `deepfos-celery-1.0.3/celery/backends/filesystem.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/mongodb.py` & `deepfos-celery-1.0.3/celery/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/redis.py` & `deepfos-celery-1.0.3/celery/backends/redis.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,594 +1,594 @@
-"""Redis result store backend."""
-import time
-from contextlib import contextmanager
-from functools import partial
-from ssl import CERT_NONE, CERT_OPTIONAL, CERT_REQUIRED
-from urllib.parse import unquote
-
-from kombu.utils.functional import retry_over_time
-from kombu.utils.objects import cached_property
-from kombu.utils.url import _parse_url
-
-from celery import states
-from celery._state import task_join_will_block
-from celery.canvas import maybe_signature
-from celery.exceptions import ChordError, ImproperlyConfigured
-from celery.result import GroupResult, allow_join_result
-from celery.utils.functional import dictfilter
-from celery.utils.log import get_logger
-from celery.utils.time import humanize_seconds
-
-from .asynchronous import AsyncBackendMixin, BaseResultConsumer
-from .base import BaseKeyValueStoreBackend
-
-try:
-    import redis.connection
-    from kombu.transport.redis import get_redis_error_classes
-except ImportError:  # pragma: no cover
-    redis = None  # noqa
-    get_redis_error_classes = None  # noqa
-
-try:
-    import redis.sentinel
-except ImportError:
-    pass
-
-__all__ = ('RedisBackend', 'SentinelBackend')
-
-E_REDIS_MISSING = """
-You need to install the redis library in order to use \
-the Redis result store backend.
-"""
-
-E_REDIS_SENTINEL_MISSING = """
-You need to install the redis library with support of \
-sentinel in order to use the Redis result store backend.
-"""
-
-W_REDIS_SSL_CERT_OPTIONAL = """
-Setting ssl_cert_reqs=CERT_OPTIONAL when connecting to redis means that \
-celery might not valdate the identity of the redis broker when connecting. \
-This leaves you vulnerable to man in the middle attacks.
-"""
-
-W_REDIS_SSL_CERT_NONE = """
-Setting ssl_cert_reqs=CERT_NONE when connecting to redis means that celery \
-will not valdate the identity of the redis broker when connecting. This \
-leaves you vulnerable to man in the middle attacks.
-"""
-
-E_REDIS_SSL_PARAMS_AND_SCHEME_MISMATCH = """
-SSL connection parameters have been provided but the specified URL scheme \
-is redis://. A Redis SSL connection URL should use the scheme rediss://.
-"""
-
-E_REDIS_SSL_CERT_REQS_MISSING_INVALID = """
-A rediss:// URL must have parameter ssl_cert_reqs and this must be set to \
-CERT_REQUIRED, CERT_OPTIONAL, or CERT_NONE
-"""
-
-E_LOST = 'Connection to Redis lost: Retry (%s/%s) %s.'
-
-E_RETRY_LIMIT_EXCEEDED = """
-Retry limit exceeded while trying to reconnect to the Celery redis result \
-store backend. The Celery application must be restarted.
-"""
-
-logger = get_logger(__name__)
-
-
-class ResultConsumer(BaseResultConsumer):
-    _pubsub = None
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._get_key_for_task = self.backend.get_key_for_task
-        self._decode_result = self.backend.decode_result
-        self._ensure = self.backend.ensure
-        self._connection_errors = self.backend.connection_errors
-        self.subscribed_to = set()
-
-    def on_after_fork(self):
-        try:
-            self.backend.client.connection_pool.reset()
-            if self._pubsub is not None:
-                self._pubsub.close()
-        except KeyError as e:
-            logger.warning(str(e))
-        super().on_after_fork()
-
-    def _reconnect_pubsub(self):
-        self._pubsub = None
-        self.backend.client.connection_pool.reset()
-        # task state might have changed when the connection was down so we
-        # retrieve meta for all subscribed tasks before going into pubsub mode
-        metas = self.backend.client.mget(self.subscribed_to)
-        metas = [meta for meta in metas if meta]
-        for meta in metas:
-            self.on_state_change(self._decode_result(meta), None)
-        self._pubsub = self.backend.client.pubsub(
-            ignore_subscribe_messages=True,
-        )
-        if self.subscribed_to:
-            self._pubsub.subscribe(*self.subscribed_to)
-
-    @contextmanager
-    def reconnect_on_error(self):
-        try:
-            yield
-        except self._connection_errors:
-            try:
-                self._ensure(self._reconnect_pubsub, ())
-            except self._connection_errors:
-                logger.critical(E_RETRY_LIMIT_EXCEEDED)
-                raise
-
-    def _maybe_cancel_ready_task(self, meta):
-        if meta['status'] in states.READY_STATES:
-            self.cancel_for(meta['task_id'])
-
-    def on_state_change(self, meta, message):
-        super().on_state_change(meta, message)
-        self._maybe_cancel_ready_task(meta)
-
-    def start(self, initial_task_id, **kwargs):
-        self._pubsub = self.backend.client.pubsub(
-            ignore_subscribe_messages=True,
-        )
-        self._consume_from(initial_task_id)
-
-    def on_wait_for_pending(self, result, **kwargs):
-        for meta in result._iter_meta(**kwargs):
-            if meta is not None:
-                self.on_state_change(meta, None)
-
-    def stop(self):
-        if self._pubsub is not None:
-            self._pubsub.close()
-
-    def drain_events(self, timeout=None):
-        if self._pubsub:
-            with self.reconnect_on_error():
-                message = self._pubsub.get_message(timeout=timeout)
-                if message and message['type'] == 'message':
-                    self.on_state_change(self._decode_result(message['data']), message)
-        elif timeout:
-            time.sleep(timeout)
-
-    def consume_from(self, task_id):
-        if self._pubsub is None:
-            return self.start(task_id)
-        self._consume_from(task_id)
-
-    def _consume_from(self, task_id):
-        key = self._get_key_for_task(task_id)
-        if key not in self.subscribed_to:
-            self.subscribed_to.add(key)
-            with self.reconnect_on_error():
-                self._pubsub.subscribe(key)
-
-    def cancel_for(self, task_id):
-        key = self._get_key_for_task(task_id)
-        self.subscribed_to.discard(key)
-        if self._pubsub:
-            with self.reconnect_on_error():
-                self._pubsub.unsubscribe(key)
-
-
-class RedisBackend(BaseKeyValueStoreBackend, AsyncBackendMixin):
-    """Redis task result store.
-
-    It makes use of the following commands:
-    GET, MGET, DEL, INCRBY, EXPIRE, SET, SETEX
-    """
-
-    ResultConsumer = ResultConsumer
-
-    #: :pypi:`redis` client module.
-    redis = redis
-
-    #: Maximum number of connections in the pool.
-    max_connections = None
-
-    supports_autoexpire = True
-    supports_native_join = True
-
-    def __init__(self, host=None, port=None, db=None, password=None,
-                 max_connections=None, url=None,
-                 connection_pool=None, **kwargs):
-        super().__init__(expires_type=int, **kwargs)
-        _get = self.app.conf.get
-        if self.redis is None:
-            raise ImproperlyConfigured(E_REDIS_MISSING.strip())
-
-        if host and '://' in host:
-            url, host = host, None
-
-        self.max_connections = (
-            max_connections or
-            _get('redis_max_connections') or
-            self.max_connections)
-        self._ConnectionPool = connection_pool
-
-        socket_timeout = _get('redis_socket_timeout')
-        socket_connect_timeout = _get('redis_socket_connect_timeout')
-        retry_on_timeout = _get('redis_retry_on_timeout')
-        socket_keepalive = _get('redis_socket_keepalive')
-
-        self.connparams = {
-            'host': _get('redis_host') or 'localhost',
-            'port': _get('redis_port') or 6379,
-            'db': _get('redis_db') or 0,
-            'password': _get('redis_password'),
-            'max_connections': self.max_connections,
-            'socket_timeout': socket_timeout and float(socket_timeout),
-            'retry_on_timeout': retry_on_timeout or False,
-            'socket_connect_timeout':
-                socket_connect_timeout and float(socket_connect_timeout),
-        }
-
-        # absent in redis.connection.UnixDomainSocketConnection
-        if socket_keepalive:
-            self.connparams['socket_keepalive'] = socket_keepalive
-
-        # "redis_backend_use_ssl" must be a dict with the keys:
-        # 'ssl_cert_reqs', 'ssl_ca_certs', 'ssl_certfile', 'ssl_keyfile'
-        # (the same as "broker_use_ssl")
-        ssl = _get('redis_backend_use_ssl')
-        if ssl:
-            self.connparams.update(ssl)
-            self.connparams['connection_class'] = redis.SSLConnection
-
-        if url:
-            self.connparams = self._params_from_url(url, self.connparams)
-
-        # If we've received SSL parameters via query string or the
-        # redis_backend_use_ssl dict, check ssl_cert_reqs is valid. If set
-        # via query string ssl_cert_reqs will be a string so convert it here
-        if ('connection_class' in self.connparams and
-                self.connparams['connection_class'] is redis.SSLConnection):
-            ssl_cert_reqs_missing = 'MISSING'
-            ssl_string_to_constant = {'CERT_REQUIRED': CERT_REQUIRED,
-                                      'CERT_OPTIONAL': CERT_OPTIONAL,
-                                      'CERT_NONE': CERT_NONE,
-                                      'required': CERT_REQUIRED,
-                                      'optional': CERT_OPTIONAL,
-                                      'none': CERT_NONE}
-            ssl_cert_reqs = self.connparams.get('ssl_cert_reqs', ssl_cert_reqs_missing)
-            ssl_cert_reqs = ssl_string_to_constant.get(ssl_cert_reqs, ssl_cert_reqs)
-            if ssl_cert_reqs not in ssl_string_to_constant.values():
-                raise ValueError(E_REDIS_SSL_CERT_REQS_MISSING_INVALID)
-
-            if ssl_cert_reqs == CERT_OPTIONAL:
-                logger.warning(W_REDIS_SSL_CERT_OPTIONAL)
-            elif ssl_cert_reqs == CERT_NONE:
-                logger.warning(W_REDIS_SSL_CERT_NONE)
-            self.connparams['ssl_cert_reqs'] = ssl_cert_reqs
-
-        self.url = url
-
-        self.connection_errors, self.channel_errors = \
-            self.get_redis_error_classes()
-        self.result_consumer = self.ResultConsumer(
-            self, self.app, self.accept,
-            self._pending_results, self._pending_messages,
-        )
-
-    def get_redis_error_classes(self):
-        if get_redis_error_classes:
-            return get_redis_error_classes()
-        return ((), ())
-
-    def _params_from_url(self, url, defaults):
-        scheme, host, port, _, password, path, query = _parse_url(url)
-        connparams = dict(
-            defaults, **dictfilter({
-                'host': host, 'port': port, 'password': password,
-                'db': query.pop('virtual_host', None)})
-        )
-
-        if scheme == 'socket':
-            # use 'path' as path to the socket… in this case
-            # the database number should be given in 'query'
-            connparams.update({
-                'connection_class': self.redis.UnixDomainSocketConnection,
-                'path': '/' + path,
-            })
-            # host+port are invalid options when using this connection type.
-            connparams.pop('host', None)
-            connparams.pop('port', None)
-            connparams.pop('socket_connect_timeout')
-        else:
-            connparams['db'] = path
-
-        ssl_param_keys = ['ssl_ca_certs', 'ssl_certfile', 'ssl_keyfile',
-                          'ssl_cert_reqs']
-
-        if scheme == 'redis':
-            # If connparams or query string contain ssl params, raise error
-            if (any(key in connparams for key in ssl_param_keys) or
-                    any(key in query for key in ssl_param_keys)):
-                raise ValueError(E_REDIS_SSL_PARAMS_AND_SCHEME_MISMATCH)
-
-        if scheme == 'rediss':
-            connparams['connection_class'] = redis.SSLConnection
-            # The following parameters, if present in the URL, are encoded. We
-            # must add the decoded values to connparams.
-            for ssl_setting in ssl_param_keys:
-                ssl_val = query.pop(ssl_setting, None)
-                if ssl_val:
-                    connparams[ssl_setting] = unquote(ssl_val)
-
-        # db may be string and start with / like in kombu.
-        db = connparams.get('db') or 0
-        db = db.strip('/') if isinstance(db, str) else db
-        connparams['db'] = int(db)
-
-        for key, value in query.items():
-            if key in redis.connection.URL_QUERY_ARGUMENT_PARSERS:
-                query[key] = redis.connection.URL_QUERY_ARGUMENT_PARSERS[key](
-                    value
-                )
-
-        # Query parameters override other parameters
-        connparams.update(query)
-        return connparams
-
-    @cached_property
-    def retry_policy(self):
-        retry_policy = super().retry_policy
-        if "retry_policy" in self._transport_options:
-            retry_policy = retry_policy.copy()
-            retry_policy.update(self._transport_options['retry_policy'])
-
-        return retry_policy
-
-    def on_task_call(self, producer, task_id):
-        if not task_join_will_block():
-            self.result_consumer.consume_from(task_id)
-
-    def get(self, key):
-        return self.client.get(key)
-
-    def mget(self, keys):
-        return self.client.mget(keys)
-
-    def ensure(self, fun, args, **policy):
-        retry_policy = dict(self.retry_policy, **policy)
-        max_retries = retry_policy.get('max_retries')
-        return retry_over_time(
-            fun, self.connection_errors, args, {},
-            partial(self.on_connection_error, max_retries),
-            **retry_policy)
-
-    def on_connection_error(self, max_retries, exc, intervals, retries):
-        tts = next(intervals)
-        logger.error(
-            E_LOST.strip(),
-            retries, max_retries or 'Inf', humanize_seconds(tts, 'in '))
-        return tts
-
-    def set(self, key, value, **retry_policy):
-        return self.ensure(self._set, (key, value), **retry_policy)
-
-    def _set(self, key, value):
-        with self.client.pipeline() as pipe:
-            if self.expires:
-                pipe.setex(key, self.expires, value)
-            else:
-                pipe.set(key, value)
-            pipe.publish(key, value)
-            pipe.execute()
-
-    def forget(self, task_id):
-        super().forget(task_id)
-        self.result_consumer.cancel_for(task_id)
-
-    def delete(self, key):
-        self.client.delete(key)
-
-    def incr(self, key):
-        return self.client.incr(key)
-
-    def expire(self, key, value):
-        return self.client.expire(key, value)
-
-    def add_to_chord(self, group_id, result):
-        self.client.incr(self.get_key_for_group(group_id, '.t'), 1)
-
-    def _unpack_chord_result(self, tup, decode,
-                             EXCEPTION_STATES=states.EXCEPTION_STATES,
-                             PROPAGATE_STATES=states.PROPAGATE_STATES):
-        _, tid, state, retval = decode(tup)
-        if state in EXCEPTION_STATES:
-            retval = self.exception_to_python(retval)
-        if state in PROPAGATE_STATES:
-            raise ChordError(f'Dependency {tid} raised {retval!r}')
-        return retval
-
-    def apply_chord(self, header_result, body, **kwargs):
-        # If any of the child results of this chord are complex (ie. group
-        # results themselves), we need to save `header_result` to ensure that
-        # the expected structure is retained when we finish the chord and pass
-        # the results onward to the body in `on_chord_part_return()`. We don't
-        # do this is all cases to retain an optimisation in the common case
-        # where a chord header is comprised of simple result objects.
-        if any(isinstance(nr, GroupResult) for nr in header_result.results):
-            header_result.save(backend=self)
-
-    @cached_property
-    def _chord_zset(self):
-        return self._transport_options.get('result_chord_ordered', True)
-
-    @cached_property
-    def _transport_options(self):
-        return self.app.conf.get('result_backend_transport_options', {})
-
-    def on_chord_part_return(self, request, state, result,
-                             propagate=None, **kwargs):
-        app = self.app
-        tid, gid, group_index = request.id, request.group, request.group_index
-        if not gid or not tid:
-            return
-        if group_index is None:
-            group_index = '+inf'
-
-        client = self.client
-        jkey = self.get_key_for_group(gid, '.j')
-        tkey = self.get_key_for_group(gid, '.t')
-        result = self.encode_result(result, state)
-        encoded = self.encode([1, tid, state, result])
-        with client.pipeline() as pipe:
-            pipeline = (
-                pipe.zadd(jkey, {encoded: group_index}).zcount(jkey, "-inf", "+inf")
-                if self._chord_zset
-                else pipe.rpush(jkey, encoded).llen(jkey)
-            ).get(tkey)
-            if self.expires:
-                pipeline = pipeline \
-                    .expire(jkey, self.expires) \
-                    .expire(tkey, self.expires)
-
-            _, readycount, totaldiff = pipeline.execute()[:3]
-
-        totaldiff = int(totaldiff or 0)
-
-        try:
-            callback = maybe_signature(request.chord, app=app)
-            total = callback['chord_size'] + totaldiff
-            if readycount == total:
-                header_result = GroupResult.restore(gid)
-                if header_result is not None:
-                    # If we manage to restore a `GroupResult`, then it must
-                    # have been complex and saved by `apply_chord()` earlier.
-                    #
-                    # Before we can join the `GroupResult`, it needs to be
-                    # manually marked as ready to avoid blocking
-                    header_result.on_ready()
-                    # We'll `join()` it to get the results and ensure they are
-                    # structured as intended rather than the flattened version
-                    # we'd construct without any other information.
-                    join_func = (
-                        header_result.join_native
-                        if header_result.supports_native_join
-                        else header_result.join
-                    )
-                    with allow_join_result():
-                        resl = join_func(timeout=3.0, propagate=True)
-                else:
-                    # Otherwise simply extract and decode the results we
-                    # stashed along the way, which should be faster for large
-                    # numbers of simple results in the chord header.
-                    decode, unpack = self.decode, self._unpack_chord_result
-                    with client.pipeline() as pipe:
-                        if self._chord_zset:
-                            pipeline = pipe.zrange(jkey, 0, -1)
-                        else:
-                            pipeline = pipe.lrange(jkey, 0, total)
-                        resl, = pipeline.execute()
-                    resl = [unpack(tup, decode) for tup in resl]
-                try:
-                    callback.delay(resl)
-                except Exception as exc:  # pylint: disable=broad-except
-                    logger.exception(
-                        'Chord callback for %r raised: %r', request.group, exc)
-                    return self.chord_error_from_stack(
-                        callback,
-                        ChordError(f'Callback error: {exc!r}'),
-                    )
-                finally:
-                    with client.pipeline() as pipe:
-                        _, _ = pipe \
-                            .delete(jkey) \
-                            .delete(tkey) \
-                            .execute()
-        except ChordError as exc:
-            logger.exception('Chord %r raised: %r', request.group, exc)
-            return self.chord_error_from_stack(callback, exc)
-        except Exception as exc:  # pylint: disable=broad-except
-            logger.exception('Chord %r raised: %r', request.group, exc)
-            return self.chord_error_from_stack(
-                callback,
-                ChordError(f'Join error: {exc!r}'),
-            )
-
-    def _create_client(self, **params):
-        return self._get_client()(
-            connection_pool=self._get_pool(**params),
-        )
-
-    def _get_client(self):
-        return self.redis.StrictRedis
-
-    def _get_pool(self, **params):
-        return self.ConnectionPool(**params)
-
-    @property
-    def ConnectionPool(self):
-        if self._ConnectionPool is None:
-            self._ConnectionPool = self.redis.ConnectionPool
-        return self._ConnectionPool
-
-    @cached_property
-    def client(self):
-        return self._create_client(**self.connparams)
-
-    def __reduce__(self, args=(), kwargs=None):
-        kwargs = {} if not kwargs else kwargs
-        return super().__reduce__(
-            (self.url,), {'expires': self.expires},
-        )
-
-
-class SentinelBackend(RedisBackend):
-    """Redis sentinel task result store."""
-
-    sentinel = getattr(redis, "sentinel", None)
-
-    def __init__(self, *args, **kwargs):
-        if self.sentinel is None:
-            raise ImproperlyConfigured(E_REDIS_SENTINEL_MISSING.strip())
-
-        super().__init__(*args, **kwargs)
-
-    def _params_from_url(self, url, defaults):
-        # URL looks like sentinel://0.0.0.0:26347/3;sentinel://0.0.0.0:26348/3.
-        chunks = url.split(";")
-        connparams = dict(defaults, hosts=[])
-        for chunk in chunks:
-            data = super()._params_from_url(
-                url=chunk, defaults=defaults)
-            connparams['hosts'].append(data)
-        for param in ("host", "port", "db", "password"):
-            connparams.pop(param)
-
-        # Adding db/password in connparams to connect to the correct instance
-        for param in ("db", "password"):
-            if connparams['hosts'] and param in connparams['hosts'][0]:
-                connparams[param] = connparams['hosts'][0].get(param)
-        return connparams
-
-    def _get_sentinel_instance(self, **params):
-        connparams = params.copy()
-
-        hosts = connparams.pop("hosts")
-        min_other_sentinels = self._transport_options.get("min_other_sentinels", 0)
-        sentinel_kwargs = self._transport_options.get("sentinel_kwargs", {})
-
-        sentinel_instance = self.sentinel.Sentinel(
-            [(cp['host'], cp['port']) for cp in hosts],
-            min_other_sentinels=min_other_sentinels,
-            sentinel_kwargs=sentinel_kwargs,
-            **connparams)
-
-        return sentinel_instance
-
-    def _get_pool(self, **params):
-        sentinel_instance = self._get_sentinel_instance(**params)
-
-        master_name = self._transport_options.get("master_name", None)
-
-        return sentinel_instance.master_for(
-            service_name=master_name,
-            redis_class=self._get_client(),
-        ).connection_pool
+"""Redis result store backend."""
+import time
+from contextlib import contextmanager
+from functools import partial
+from ssl import CERT_NONE, CERT_OPTIONAL, CERT_REQUIRED
+from urllib.parse import unquote
+
+from kombu.utils.functional import retry_over_time
+from kombu.utils.objects import cached_property
+from kombu.utils.url import _parse_url
+
+from celery import states
+from celery._state import task_join_will_block
+from celery.canvas import maybe_signature
+from celery.exceptions import ChordError, ImproperlyConfigured
+from celery.result import GroupResult, allow_join_result
+from celery.utils.functional import dictfilter
+from celery.utils.log import get_logger
+from celery.utils.time import humanize_seconds
+
+from .asynchronous import AsyncBackendMixin, BaseResultConsumer
+from .base import BaseKeyValueStoreBackend
+
+try:
+    import redis.connection
+    from kombu.transport.redis import get_redis_error_classes
+except ImportError:  # pragma: no cover
+    redis = None  # noqa
+    get_redis_error_classes = None  # noqa
+
+try:
+    import redis.sentinel
+except ImportError:
+    pass
+
+__all__ = ('RedisBackend', 'SentinelBackend')
+
+E_REDIS_MISSING = """
+You need to install the redis library in order to use \
+the Redis result store backend.
+"""
+
+E_REDIS_SENTINEL_MISSING = """
+You need to install the redis library with support of \
+sentinel in order to use the Redis result store backend.
+"""
+
+W_REDIS_SSL_CERT_OPTIONAL = """
+Setting ssl_cert_reqs=CERT_OPTIONAL when connecting to redis means that \
+celery might not valdate the identity of the redis broker when connecting. \
+This leaves you vulnerable to man in the middle attacks.
+"""
+
+W_REDIS_SSL_CERT_NONE = """
+Setting ssl_cert_reqs=CERT_NONE when connecting to redis means that celery \
+will not valdate the identity of the redis broker when connecting. This \
+leaves you vulnerable to man in the middle attacks.
+"""
+
+E_REDIS_SSL_PARAMS_AND_SCHEME_MISMATCH = """
+SSL connection parameters have been provided but the specified URL scheme \
+is redis://. A Redis SSL connection URL should use the scheme rediss://.
+"""
+
+E_REDIS_SSL_CERT_REQS_MISSING_INVALID = """
+A rediss:// URL must have parameter ssl_cert_reqs and this must be set to \
+CERT_REQUIRED, CERT_OPTIONAL, or CERT_NONE
+"""
+
+E_LOST = 'Connection to Redis lost: Retry (%s/%s) %s.'
+
+E_RETRY_LIMIT_EXCEEDED = """
+Retry limit exceeded while trying to reconnect to the Celery redis result \
+store backend. The Celery application must be restarted.
+"""
+
+logger = get_logger(__name__)
+
+
+class ResultConsumer(BaseResultConsumer):
+    _pubsub = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._get_key_for_task = self.backend.get_key_for_task
+        self._decode_result = self.backend.decode_result
+        self._ensure = self.backend.ensure
+        self._connection_errors = self.backend.connection_errors
+        self.subscribed_to = set()
+
+    def on_after_fork(self):
+        try:
+            self.backend.client.connection_pool.reset()
+            if self._pubsub is not None:
+                self._pubsub.close()
+        except KeyError as e:
+            logger.warning(str(e))
+        super().on_after_fork()
+
+    def _reconnect_pubsub(self):
+        self._pubsub = None
+        self.backend.client.connection_pool.reset()
+        # task state might have changed when the connection was down so we
+        # retrieve meta for all subscribed tasks before going into pubsub mode
+        metas = self.backend.client.mget(self.subscribed_to)
+        metas = [meta for meta in metas if meta]
+        for meta in metas:
+            self.on_state_change(self._decode_result(meta), None)
+        self._pubsub = self.backend.client.pubsub(
+            ignore_subscribe_messages=True,
+        )
+        if self.subscribed_to:
+            self._pubsub.subscribe(*self.subscribed_to)
+
+    @contextmanager
+    def reconnect_on_error(self):
+        try:
+            yield
+        except self._connection_errors:
+            try:
+                self._ensure(self._reconnect_pubsub, ())
+            except self._connection_errors:
+                logger.critical(E_RETRY_LIMIT_EXCEEDED)
+                raise
+
+    def _maybe_cancel_ready_task(self, meta):
+        if meta['status'] in states.READY_STATES:
+            self.cancel_for(meta['task_id'])
+
+    def on_state_change(self, meta, message):
+        super().on_state_change(meta, message)
+        self._maybe_cancel_ready_task(meta)
+
+    def start(self, initial_task_id, **kwargs):
+        self._pubsub = self.backend.client.pubsub(
+            ignore_subscribe_messages=True,
+        )
+        self._consume_from(initial_task_id)
+
+    def on_wait_for_pending(self, result, **kwargs):
+        for meta in result._iter_meta(**kwargs):
+            if meta is not None:
+                self.on_state_change(meta, None)
+
+    def stop(self):
+        if self._pubsub is not None:
+            self._pubsub.close()
+
+    def drain_events(self, timeout=None):
+        if self._pubsub:
+            with self.reconnect_on_error():
+                message = self._pubsub.get_message(timeout=timeout)
+                if message and message['type'] == 'message':
+                    self.on_state_change(self._decode_result(message['data']), message)
+        elif timeout:
+            time.sleep(timeout)
+
+    def consume_from(self, task_id):
+        if self._pubsub is None:
+            return self.start(task_id)
+        self._consume_from(task_id)
+
+    def _consume_from(self, task_id):
+        key = self._get_key_for_task(task_id)
+        if key not in self.subscribed_to:
+            self.subscribed_to.add(key)
+            with self.reconnect_on_error():
+                self._pubsub.subscribe(key)
+
+    def cancel_for(self, task_id):
+        key = self._get_key_for_task(task_id)
+        self.subscribed_to.discard(key)
+        if self._pubsub:
+            with self.reconnect_on_error():
+                self._pubsub.unsubscribe(key)
+
+
+class RedisBackend(BaseKeyValueStoreBackend, AsyncBackendMixin):
+    """Redis task result store.
+
+    It makes use of the following commands:
+    GET, MGET, DEL, INCRBY, EXPIRE, SET, SETEX
+    """
+
+    ResultConsumer = ResultConsumer
+
+    #: :pypi:`redis` client module.
+    redis = redis
+
+    #: Maximum number of connections in the pool.
+    max_connections = None
+
+    supports_autoexpire = True
+    supports_native_join = True
+
+    def __init__(self, host=None, port=None, db=None, password=None,
+                 max_connections=None, url=None,
+                 connection_pool=None, **kwargs):
+        super().__init__(expires_type=int, **kwargs)
+        _get = self.app.conf.get
+        if self.redis is None:
+            raise ImproperlyConfigured(E_REDIS_MISSING.strip())
+
+        if host and '://' in host:
+            url, host = host, None
+
+        self.max_connections = (
+            max_connections or
+            _get('redis_max_connections') or
+            self.max_connections)
+        self._ConnectionPool = connection_pool
+
+        socket_timeout = _get('redis_socket_timeout')
+        socket_connect_timeout = _get('redis_socket_connect_timeout')
+        retry_on_timeout = _get('redis_retry_on_timeout')
+        socket_keepalive = _get('redis_socket_keepalive')
+
+        self.connparams = {
+            'host': _get('redis_host') or 'localhost',
+            'port': _get('redis_port') or 6379,
+            'db': _get('redis_db') or 0,
+            'password': _get('redis_password'),
+            'max_connections': self.max_connections,
+            'socket_timeout': socket_timeout and float(socket_timeout),
+            'retry_on_timeout': retry_on_timeout or False,
+            'socket_connect_timeout':
+                socket_connect_timeout and float(socket_connect_timeout),
+        }
+
+        # absent in redis.connection.UnixDomainSocketConnection
+        if socket_keepalive:
+            self.connparams['socket_keepalive'] = socket_keepalive
+
+        # "redis_backend_use_ssl" must be a dict with the keys:
+        # 'ssl_cert_reqs', 'ssl_ca_certs', 'ssl_certfile', 'ssl_keyfile'
+        # (the same as "broker_use_ssl")
+        ssl = _get('redis_backend_use_ssl')
+        if ssl:
+            self.connparams.update(ssl)
+            self.connparams['connection_class'] = redis.SSLConnection
+
+        if url:
+            self.connparams = self._params_from_url(url, self.connparams)
+
+        # If we've received SSL parameters via query string or the
+        # redis_backend_use_ssl dict, check ssl_cert_reqs is valid. If set
+        # via query string ssl_cert_reqs will be a string so convert it here
+        if ('connection_class' in self.connparams and
+                self.connparams['connection_class'] is redis.SSLConnection):
+            ssl_cert_reqs_missing = 'MISSING'
+            ssl_string_to_constant = {'CERT_REQUIRED': CERT_REQUIRED,
+                                      'CERT_OPTIONAL': CERT_OPTIONAL,
+                                      'CERT_NONE': CERT_NONE,
+                                      'required': CERT_REQUIRED,
+                                      'optional': CERT_OPTIONAL,
+                                      'none': CERT_NONE}
+            ssl_cert_reqs = self.connparams.get('ssl_cert_reqs', ssl_cert_reqs_missing)
+            ssl_cert_reqs = ssl_string_to_constant.get(ssl_cert_reqs, ssl_cert_reqs)
+            if ssl_cert_reqs not in ssl_string_to_constant.values():
+                raise ValueError(E_REDIS_SSL_CERT_REQS_MISSING_INVALID)
+
+            if ssl_cert_reqs == CERT_OPTIONAL:
+                logger.warning(W_REDIS_SSL_CERT_OPTIONAL)
+            elif ssl_cert_reqs == CERT_NONE:
+                logger.warning(W_REDIS_SSL_CERT_NONE)
+            self.connparams['ssl_cert_reqs'] = ssl_cert_reqs
+
+        self.url = url
+
+        self.connection_errors, self.channel_errors = \
+            self.get_redis_error_classes()
+        self.result_consumer = self.ResultConsumer(
+            self, self.app, self.accept,
+            self._pending_results, self._pending_messages,
+        )
+
+    def get_redis_error_classes(self):
+        if get_redis_error_classes:
+            return get_redis_error_classes()
+        return ((), ())
+
+    def _params_from_url(self, url, defaults):
+        scheme, host, port, _, password, path, query = _parse_url(url)
+        connparams = dict(
+            defaults, **dictfilter({
+                'host': host, 'port': port, 'password': password,
+                'db': query.pop('virtual_host', None)})
+        )
+
+        if scheme == 'socket':
+            # use 'path' as path to the socket… in this case
+            # the database number should be given in 'query'
+            connparams.update({
+                'connection_class': self.redis.UnixDomainSocketConnection,
+                'path': '/' + path,
+            })
+            # host+port are invalid options when using this connection type.
+            connparams.pop('host', None)
+            connparams.pop('port', None)
+            connparams.pop('socket_connect_timeout')
+        else:
+            connparams['db'] = path
+
+        ssl_param_keys = ['ssl_ca_certs', 'ssl_certfile', 'ssl_keyfile',
+                          'ssl_cert_reqs']
+
+        if scheme == 'redis':
+            # If connparams or query string contain ssl params, raise error
+            if (any(key in connparams for key in ssl_param_keys) or
+                    any(key in query for key in ssl_param_keys)):
+                raise ValueError(E_REDIS_SSL_PARAMS_AND_SCHEME_MISMATCH)
+
+        if scheme == 'rediss':
+            connparams['connection_class'] = redis.SSLConnection
+            # The following parameters, if present in the URL, are encoded. We
+            # must add the decoded values to connparams.
+            for ssl_setting in ssl_param_keys:
+                ssl_val = query.pop(ssl_setting, None)
+                if ssl_val:
+                    connparams[ssl_setting] = unquote(ssl_val)
+
+        # db may be string and start with / like in kombu.
+        db = connparams.get('db') or 0
+        db = db.strip('/') if isinstance(db, str) else db
+        connparams['db'] = int(db)
+
+        for key, value in query.items():
+            if key in redis.connection.URL_QUERY_ARGUMENT_PARSERS:
+                query[key] = redis.connection.URL_QUERY_ARGUMENT_PARSERS[key](
+                    value
+                )
+
+        # Query parameters override other parameters
+        connparams.update(query)
+        return connparams
+
+    @cached_property
+    def retry_policy(self):
+        retry_policy = super().retry_policy
+        if "retry_policy" in self._transport_options:
+            retry_policy = retry_policy.copy()
+            retry_policy.update(self._transport_options['retry_policy'])
+
+        return retry_policy
+
+    def on_task_call(self, producer, task_id):
+        if not task_join_will_block():
+            self.result_consumer.consume_from(task_id)
+
+    def get(self, key):
+        return self.client.get(key)
+
+    def mget(self, keys):
+        return self.client.mget(keys)
+
+    def ensure(self, fun, args, **policy):
+        retry_policy = dict(self.retry_policy, **policy)
+        max_retries = retry_policy.get('max_retries')
+        return retry_over_time(
+            fun, self.connection_errors, args, {},
+            partial(self.on_connection_error, max_retries),
+            **retry_policy)
+
+    def on_connection_error(self, max_retries, exc, intervals, retries):
+        tts = next(intervals)
+        logger.error(
+            E_LOST.strip(),
+            retries, max_retries or 'Inf', humanize_seconds(tts, 'in '))
+        return tts
+
+    def set(self, key, value, **retry_policy):
+        return self.ensure(self._set, (key, value), **retry_policy)
+
+    def _set(self, key, value):
+        with self.client.pipeline() as pipe:
+            if self.expires:
+                pipe.setex(key, self.expires, value)
+            else:
+                pipe.set(key, value)
+            pipe.publish(key, value)
+            pipe.execute()
+
+    def forget(self, task_id):
+        super().forget(task_id)
+        self.result_consumer.cancel_for(task_id)
+
+    def delete(self, key):
+        self.client.delete(key)
+
+    def incr(self, key):
+        return self.client.incr(key)
+
+    def expire(self, key, value):
+        return self.client.expire(key, value)
+
+    def add_to_chord(self, group_id, result):
+        self.client.incr(self.get_key_for_group(group_id, '.t'), 1)
+
+    def _unpack_chord_result(self, tup, decode,
+                             EXCEPTION_STATES=states.EXCEPTION_STATES,
+                             PROPAGATE_STATES=states.PROPAGATE_STATES):
+        _, tid, state, retval = decode(tup)
+        if state in EXCEPTION_STATES:
+            retval = self.exception_to_python(retval)
+        if state in PROPAGATE_STATES:
+            raise ChordError(f'Dependency {tid} raised {retval!r}')
+        return retval
+
+    def apply_chord(self, header_result, body, **kwargs):
+        # If any of the child results of this chord are complex (ie. group
+        # results themselves), we need to save `header_result` to ensure that
+        # the expected structure is retained when we finish the chord and pass
+        # the results onward to the body in `on_chord_part_return()`. We don't
+        # do this is all cases to retain an optimisation in the common case
+        # where a chord header is comprised of simple result objects.
+        if any(isinstance(nr, GroupResult) for nr in header_result.results):
+            header_result.save(backend=self)
+
+    @cached_property
+    def _chord_zset(self):
+        return self._transport_options.get('result_chord_ordered', True)
+
+    @cached_property
+    def _transport_options(self):
+        return self.app.conf.get('result_backend_transport_options', {})
+
+    def on_chord_part_return(self, request, state, result,
+                             propagate=None, **kwargs):
+        app = self.app
+        tid, gid, group_index = request.id, request.group, request.group_index
+        if not gid or not tid:
+            return
+        if group_index is None:
+            group_index = '+inf'
+
+        client = self.client
+        jkey = self.get_key_for_group(gid, '.j')
+        tkey = self.get_key_for_group(gid, '.t')
+        result = self.encode_result(result, state)
+        encoded = self.encode([1, tid, state, result])
+        with client.pipeline() as pipe:
+            pipeline = (
+                pipe.zadd(jkey, {encoded: group_index}).zcount(jkey, "-inf", "+inf")
+                if self._chord_zset
+                else pipe.rpush(jkey, encoded).llen(jkey)
+            ).get(tkey)
+            if self.expires:
+                pipeline = pipeline \
+                    .expire(jkey, self.expires) \
+                    .expire(tkey, self.expires)
+
+            _, readycount, totaldiff = pipeline.execute()[:3]
+
+        totaldiff = int(totaldiff or 0)
+
+        try:
+            callback = maybe_signature(request.chord, app=app)
+            total = callback['chord_size'] + totaldiff
+            if readycount == total:
+                header_result = GroupResult.restore(gid)
+                if header_result is not None:
+                    # If we manage to restore a `GroupResult`, then it must
+                    # have been complex and saved by `apply_chord()` earlier.
+                    #
+                    # Before we can join the `GroupResult`, it needs to be
+                    # manually marked as ready to avoid blocking
+                    header_result.on_ready()
+                    # We'll `join()` it to get the results and ensure they are
+                    # structured as intended rather than the flattened version
+                    # we'd construct without any other information.
+                    join_func = (
+                        header_result.join_native
+                        if header_result.supports_native_join
+                        else header_result.join
+                    )
+                    with allow_join_result():
+                        resl = join_func(timeout=3.0, propagate=True)
+                else:
+                    # Otherwise simply extract and decode the results we
+                    # stashed along the way, which should be faster for large
+                    # numbers of simple results in the chord header.
+                    decode, unpack = self.decode, self._unpack_chord_result
+                    with client.pipeline() as pipe:
+                        if self._chord_zset:
+                            pipeline = pipe.zrange(jkey, 0, -1)
+                        else:
+                            pipeline = pipe.lrange(jkey, 0, total)
+                        resl, = pipeline.execute()
+                    resl = [unpack(tup, decode) for tup in resl]
+                try:
+                    callback.delay(resl)
+                except Exception as exc:  # pylint: disable=broad-except
+                    logger.exception(
+                        'Chord callback for %r raised: %r', request.group, exc)
+                    return self.chord_error_from_stack(
+                        callback,
+                        ChordError(f'Callback error: {exc!r}'),
+                    )
+                finally:
+                    with client.pipeline() as pipe:
+                        _, _ = pipe \
+                            .delete(jkey) \
+                            .delete(tkey) \
+                            .execute()
+        except ChordError as exc:
+            logger.exception('Chord %r raised: %r', request.group, exc)
+            return self.chord_error_from_stack(callback, exc)
+        except Exception as exc:  # pylint: disable=broad-except
+            logger.exception('Chord %r raised: %r', request.group, exc)
+            return self.chord_error_from_stack(
+                callback,
+                ChordError(f'Join error: {exc!r}'),
+            )
+
+    def _create_client(self, **params):
+        return self._get_client()(
+            connection_pool=self._get_pool(**params),
+        )
+
+    def _get_client(self):
+        return self.redis.StrictRedis
+
+    def _get_pool(self, **params):
+        return self.ConnectionPool(**params)
+
+    @property
+    def ConnectionPool(self):
+        if self._ConnectionPool is None:
+            self._ConnectionPool = self.redis.ConnectionPool
+        return self._ConnectionPool
+
+    @cached_property
+    def client(self):
+        return self._create_client(**self.connparams)
+
+    def __reduce__(self, args=(), kwargs=None):
+        kwargs = {} if not kwargs else kwargs
+        return super().__reduce__(
+            (self.url,), {'expires': self.expires},
+        )
+
+
+class SentinelBackend(RedisBackend):
+    """Redis sentinel task result store."""
+
+    sentinel = getattr(redis, "sentinel", None)
+
+    def __init__(self, *args, **kwargs):
+        if self.sentinel is None:
+            raise ImproperlyConfigured(E_REDIS_SENTINEL_MISSING.strip())
+
+        super().__init__(*args, **kwargs)
+
+    def _params_from_url(self, url, defaults):
+        # URL looks like sentinel://0.0.0.0:26347/3;sentinel://0.0.0.0:26348/3.
+        chunks = url.split(";")
+        connparams = dict(defaults, hosts=[])
+        for chunk in chunks:
+            data = super()._params_from_url(
+                url=chunk, defaults=defaults)
+            connparams['hosts'].append(data)
+        for param in ("host", "port", "db", "password"):
+            connparams.pop(param)
+
+        # Adding db/password in connparams to connect to the correct instance
+        for param in ("db", "password"):
+            if connparams['hosts'] and param in connparams['hosts'][0]:
+                connparams[param] = connparams['hosts'][0].get(param)
+        return connparams
+
+    def _get_sentinel_instance(self, **params):
+        connparams = params.copy()
+
+        hosts = connparams.pop("hosts")
+        min_other_sentinels = self._transport_options.get("min_other_sentinels", 0)
+        sentinel_kwargs = self._transport_options.get("sentinel_kwargs", {})
+
+        sentinel_instance = self.sentinel.Sentinel(
+            [(cp['host'], cp['port']) for cp in hosts],
+            min_other_sentinels=min_other_sentinels,
+            sentinel_kwargs=sentinel_kwargs,
+            **connparams)
+
+        return sentinel_instance
+
+    def _get_pool(self, **params):
+        sentinel_instance = self._get_sentinel_instance(**params)
+
+        master_name = self._transport_options.get("master_name", None)
+
+        return sentinel_instance.master_for(
+            service_name=master_name,
+            redis_class=self._get_client(),
+        ).connection_pool
```

### Comparing `deepfos-celery-1.0.2/celery/backends/rpc.py` & `deepfos-celery-1.0.3/celery/backends/rpc.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/backends/s3.py` & `deepfos-celery-1.0.3/celery/backends/s3.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/beat.py` & `deepfos-celery-1.0.3/celery/beat.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/amqp.py` & `deepfos-celery-1.0.3/celery/bin/amqp.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/base.py` & `deepfos-celery-1.0.3/celery/bin/base.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/beat.py` & `deepfos-celery-1.0.3/celery/bin/beat.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/call.py` & `deepfos-celery-1.0.3/celery/bin/call.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/celery.py` & `deepfos-celery-1.0.3/celery/bin/celery.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/control.py` & `deepfos-celery-1.0.3/celery/bin/control.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/events.py` & `deepfos-celery-1.0.3/celery/bin/events.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/graph.py` & `deepfos-celery-1.0.3/celery/bin/graph.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/list.py` & `deepfos-celery-1.0.3/celery/bin/list.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/logtool.py` & `deepfos-celery-1.0.3/celery/bin/logtool.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/migrate.py` & `deepfos-celery-1.0.3/celery/bin/migrate.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/multi.py` & `deepfos-celery-1.0.3/celery/bin/multi.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/purge.py` & `deepfos-celery-1.0.3/celery/bin/purge.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/result.py` & `deepfos-celery-1.0.3/celery/bin/result.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/shell.py` & `deepfos-celery-1.0.3/celery/bin/shell.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/upgrade.py` & `deepfos-celery-1.0.3/celery/bin/upgrade.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bin/worker.py` & `deepfos-celery-1.0.3/celery/bin/worker.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/bootsteps.py` & `deepfos-celery-1.0.3/celery/bootsteps.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/canvas.py` & `deepfos-celery-1.0.3/celery/canvas.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/concurrency/__init__.py` & `deepfos-celery-1.0.3/celery/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/concurrency/base.py` & `deepfos-celery-1.0.3/celery/concurrency/base.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/concurrency/eventlet.py` & `deepfos-celery-1.0.3/celery/concurrency/eventlet.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/concurrency/gevent.py` & `deepfos-celery-1.0.3/celery/concurrency/gevent.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/concurrency/prefork.py` & `deepfos-celery-1.0.3/celery/concurrency/prefork.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Prefork execution pool.
 
 Pool implementation using :mod:`multiprocessing`.
 """
+import functools
 import os
 
 from billiard import forking_enable
 from billiard.common import REMAP_SIGTERM, TERM_SIGNAME
 from billiard.pool import CLOSE, RUN
 from billiard.pool import Pool as BlockingPool
 
@@ -111,19 +112,23 @@
                               synack=False,
                               proc_alive_timeout=proc_alive_timeout,
                               **self.options)
 
         # Create proxy methods
         self.on_apply = P.apply_async
         self.maintain_pool = P.maintain_pool
-        self.terminate_job = P.terminate_job
+        self.terminate_job = functools.partial(self._terminate_job, P)
         self.grow = P.grow
         self.shrink = P.shrink
         self.flush = getattr(P, 'flush', None)  # FIXME add to billiard
 
+    def _terminate_job(self, P, pid, signal=None):
+        logger.info(f'will kill worker <{pid}>')
+        return P.terminate_job(pid, signal)
+
     def restart(self):
         self._pool.restart()
         self._pool.apply_async(noop)
 
     def did_start_ok(self):
         return self._pool.did_start_ok()
 
@@ -162,7 +167,11 @@
                          self._pool.timeout or 0),
             'writes': write_stats() if write_stats is not None else 'N/A',
         }
 
     @property
     def num_processes(self):
         return self._pool._processes
+
+    @property
+    def worker_processes(self):
+        return self._pool._pool
```

### Comparing `deepfos-celery-1.0.2/celery/concurrency/solo.py` & `deepfos-celery-1.0.3/celery/concurrency/solo.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/concurrency/thread.py` & `deepfos-celery-1.0.3/celery/concurrency/thread.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/abortable.py` & `deepfos-celery-1.0.3/celery/contrib/abortable.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/migrate.py` & `deepfos-celery-1.0.3/celery/contrib/migrate.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/pytest.py` & `deepfos-celery-1.0.3/celery/contrib/pytest.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/rdb.py` & `deepfos-celery-1.0.3/celery/contrib/rdb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/sphinx.py` & `deepfos-celery-1.0.3/celery/contrib/sphinx.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/testing/app.py` & `deepfos-celery-1.0.3/celery/contrib/testing/app.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/testing/manager.py` & `deepfos-celery-1.0.3/celery/contrib/testing/manager.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/testing/mocks.py` & `deepfos-celery-1.0.3/celery/contrib/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/contrib/testing/worker.py` & `deepfos-celery-1.0.3/celery/contrib/testing/worker.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/events/cursesmon.py` & `deepfos-celery-1.0.3/celery/events/cursesmon.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/events/dispatcher.py` & `deepfos-celery-1.0.3/celery/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/events/dumper.py` & `deepfos-celery-1.0.3/celery/events/dumper.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/events/event.py` & `deepfos-celery-1.0.3/celery/events/event.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/events/receiver.py` & `deepfos-celery-1.0.3/celery/events/receiver.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/events/snapshot.py` & `deepfos-celery-1.0.3/celery/events/snapshot.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/events/state.py` & `deepfos-celery-1.0.3/celery/events/state.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/exceptions.py` & `deepfos-celery-1.0.3/celery/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/fixups/django.py` & `deepfos-celery-1.0.3/celery/fixups/django.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/loaders/base.py` & `deepfos-celery-1.0.3/celery/loaders/base.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/loaders/default.py` & `deepfos-celery-1.0.3/celery/loaders/default.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/local.py` & `deepfos-celery-1.0.3/celery/local.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/platforms.py` & `deepfos-celery-1.0.3/celery/platforms.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/result.py` & `deepfos-celery-1.0.3/celery/result.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/schedules.py` & `deepfos-celery-1.0.3/celery/schedules.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/security/__init__.py` & `deepfos-celery-1.0.3/celery/security/__init__.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/security/certificate.py` & `deepfos-celery-1.0.3/celery/security/certificate.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/security/key.py` & `deepfos-celery-1.0.3/celery/security/key.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/security/serialization.py` & `deepfos-celery-1.0.3/celery/security/serialization.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/security/utils.py` & `deepfos-celery-1.0.3/celery/security/utils.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/signals.py` & `deepfos-celery-1.0.3/celery/signals.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/states.py` & `deepfos-celery-1.0.3/celery/states.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/__init__.py` & `deepfos-celery-1.0.3/celery/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/abstract.py` & `deepfos-celery-1.0.3/celery/utils/abstract.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/collections.py` & `deepfos-celery-1.0.3/celery/utils/collections.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/debug.py` & `deepfos-celery-1.0.3/celery/utils/debug.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/deprecated.py` & `deepfos-celery-1.0.3/celery/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/functional.py` & `deepfos-celery-1.0.3/celery/utils/functional.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/graph.py` & `deepfos-celery-1.0.3/celery/utils/graph.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/imports.py` & `deepfos-celery-1.0.3/celery/utils/imports.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/iso8601.py` & `deepfos-celery-1.0.3/celery/utils/iso8601.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/log.py` & `deepfos-celery-1.0.3/celery/utils/log.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/nodenames.py` & `deepfos-celery-1.0.3/celery/utils/nodenames.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/objects.py` & `deepfos-celery-1.0.3/celery/utils/objects.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-"""Object related utilities, including introspection, etc."""
-from functools import reduce
-import typing
-
-__all__ = ('Bunch', 'FallbackContext', 'getitem_property', 'mro_lookup')
-
-
-class Bunch:
-    """Object that enables you to modify attributes."""
-
-    def __init__(self, **kwargs):
-        self.__dict__.update(kwargs)
-
-
-def mro_lookup(cls, attr, stop=None, monkey_patched=None):
-    """Return the first node by MRO order that defines an attribute.
-
-    Arguments:
-        cls (Any): Child class to traverse.
-        attr (str): Name of attribute to find.
-        stop (Set[Any]): A set of types that if reached will stop
-            the search.
-        monkey_patched (Sequence): Use one of the stop classes
-            if the attributes module origin isn't in this list.
-            Used to detect monkey patched attributes.
-
-    Returns:
-        Any: The attribute value, or :const:`None` if not found.
-    """
-    stop = set() if not stop else stop
-    monkey_patched = [] if not monkey_patched else monkey_patched
-    for node in cls.mro():
-        if node in stop:
-            try:
-                value = node.__dict__[attr]
-                module_origin = value.__module__
-            except (AttributeError, KeyError):
-                pass
-            else:
-                if module_origin not in monkey_patched:
-                    return node
-            return
-        if attr in node.__dict__:
-            return node
-
-
-class FallbackContext:
-    """Context workaround.
-
-    The built-in ``@contextmanager`` utility does not work well
-    when wrapping other contexts, as the traceback is wrong when
-    the wrapped context raises.
-
-    This solves this problem and can be used instead of ``@contextmanager``
-    in this example::
-
-        @contextmanager
-        def connection_or_default_connection(connection=None):
-            if connection:
-                # user already has a connection, shouldn't close
-                # after use
-                yield connection
-            else:
-                # must've new connection, and also close the connection
-                # after the block returns
-                with create_new_connection() as connection:
-                    yield connection
-
-    This wrapper can be used instead for the above like this::
-
-        def connection_or_default_connection(connection=None):
-            return FallbackContext(connection, create_new_connection)
-    """
-
-    def __init__(self, provided, fallback, *fb_args, **fb_kwargs):
-        self.provided = provided
-        self.fallback = fallback
-        self.fb_args = fb_args
-        self.fb_kwargs = fb_kwargs
-        self._context = None
-
-    def __enter__(self):
-        if self.provided is not None:
-            return self.provided
-        context = self._context = self.fallback(
-            *self.fb_args, **self.fb_kwargs
-        ).__enter__()
-        return context
-
-    def __exit__(self, *exc_info):
-        if self._context is not None:
-            return self._context.__exit__(*exc_info)
-
-
-class AsyncFallbackContext:
-    """Context workaround.
-
-    The built-in ``@contextmanager`` utility does not work well
-    when wrapping other contexts, as the traceback is wrong when
-    the wrapped context raises.
-
-    This solves this problem and can be used instead of ``@contextmanager``
-    in this example::
-
-        @asynccontextmanager
-        async def connection_or_default_connection(connection=None):
-            if connection:
-                # user already has a connection, shouldn't close
-                # after use
-                yield connection
-            else:
-                # must've new connection, and also close the connection
-                # after the block returns
-                async with create_new_connection() as connection:
-                    yield connection
-
-    This wrapper can be used instead for the above like this::
-
-        def connection_or_default_connection(connection=None):
-            return AsyncFallbackContext(connection, create_new_connection)
-    """
-
-    def __init__(
-        self,
-        provided: typing.Any,
-        fallback: typing.AsyncContextManager,
-        *fb_args, **fb_kwargs
-    ):
-        self.provided = provided
-        self.fallback = fallback
-        self.fb_args = fb_args
-        self.fb_kwargs = fb_kwargs
-        self._context = None
-
-    async def __aenter__(self):
-        if self.provided is not None:
-            return self.provided
-        context = self._context = self.fallback(
-            *self.fb_args, **self.fb_kwargs
-        )
-        return await context.__aenter__()
-
-    async def __aexit__(self, *exc_info):
-        if self._context is not None:
-            return await self._context.__aexit__(*exc_info)
-
-
-class getitem_property:
-    """Attribute -> dict key descriptor.
-
-    The target object must support ``__getitem__``,
-    and optionally ``__setitem__``.
-
-    Example:
-        >>> from collections import defaultdict
-
-        >>> class Me(dict):
-        ...     deep = defaultdict(dict)
-        ...
-        ...     foo = getitem_property('foo')
-        ...     deep_thing = getitem_property('deep.thing')
-
-
-        >>> me = Me()
-        >>> me.foo
-        None
-
-        >>> me.foo = 10
-        >>> me.foo
-        10
-        >>> me['foo']
-        10
-
-        >>> me.deep_thing = 42
-        >>> me.deep_thing
-        42
-        >>> me.deep
-        defaultdict(<type 'dict'>, {'thing': 42})
-    """
-
-    def __init__(self, keypath, doc=None):
-        path, _, self.key = keypath.rpartition('.')
-        self.path = path.split('.') if path else None
-        self.__doc__ = doc
-
-    def _path(self, obj):
-        return (reduce(lambda d, k: d[k], [obj] + self.path) if self.path
-                else obj)
-
-    def __get__(self, obj, type=None):
-        if obj is None:
-            return type
-        return self._path(obj).get(self.key)
-
-    def __set__(self, obj, value):
-        self._path(obj)[self.key] = value
+"""Object related utilities, including introspection, etc."""
+from functools import reduce
+import typing
+
+__all__ = ('Bunch', 'FallbackContext', 'getitem_property', 'mro_lookup')
+
+
+class Bunch:
+    """Object that enables you to modify attributes."""
+
+    def __init__(self, **kwargs):
+        self.__dict__.update(kwargs)
+
+
+def mro_lookup(cls, attr, stop=None, monkey_patched=None):
+    """Return the first node by MRO order that defines an attribute.
+
+    Arguments:
+        cls (Any): Child class to traverse.
+        attr (str): Name of attribute to find.
+        stop (Set[Any]): A set of types that if reached will stop
+            the search.
+        monkey_patched (Sequence): Use one of the stop classes
+            if the attributes module origin isn't in this list.
+            Used to detect monkey patched attributes.
+
+    Returns:
+        Any: The attribute value, or :const:`None` if not found.
+    """
+    stop = set() if not stop else stop
+    monkey_patched = [] if not monkey_patched else monkey_patched
+    for node in cls.mro():
+        if node in stop:
+            try:
+                value = node.__dict__[attr]
+                module_origin = value.__module__
+            except (AttributeError, KeyError):
+                pass
+            else:
+                if module_origin not in monkey_patched:
+                    return node
+            return
+        if attr in node.__dict__:
+            return node
+
+
+class FallbackContext:
+    """Context workaround.
+
+    The built-in ``@contextmanager`` utility does not work well
+    when wrapping other contexts, as the traceback is wrong when
+    the wrapped context raises.
+
+    This solves this problem and can be used instead of ``@contextmanager``
+    in this example::
+
+        @contextmanager
+        def connection_or_default_connection(connection=None):
+            if connection:
+                # user already has a connection, shouldn't close
+                # after use
+                yield connection
+            else:
+                # must've new connection, and also close the connection
+                # after the block returns
+                with create_new_connection() as connection:
+                    yield connection
+
+    This wrapper can be used instead for the above like this::
+
+        def connection_or_default_connection(connection=None):
+            return FallbackContext(connection, create_new_connection)
+    """
+
+    def __init__(self, provided, fallback, *fb_args, **fb_kwargs):
+        self.provided = provided
+        self.fallback = fallback
+        self.fb_args = fb_args
+        self.fb_kwargs = fb_kwargs
+        self._context = None
+
+    def __enter__(self):
+        if self.provided is not None:
+            return self.provided
+        context = self._context = self.fallback(
+            *self.fb_args, **self.fb_kwargs
+        ).__enter__()
+        return context
+
+    def __exit__(self, *exc_info):
+        if self._context is not None:
+            return self._context.__exit__(*exc_info)
+
+
+class AsyncFallbackContext:
+    """Context workaround.
+
+    The built-in ``@contextmanager`` utility does not work well
+    when wrapping other contexts, as the traceback is wrong when
+    the wrapped context raises.
+
+    This solves this problem and can be used instead of ``@contextmanager``
+    in this example::
+
+        @asynccontextmanager
+        async def connection_or_default_connection(connection=None):
+            if connection:
+                # user already has a connection, shouldn't close
+                # after use
+                yield connection
+            else:
+                # must've new connection, and also close the connection
+                # after the block returns
+                async with create_new_connection() as connection:
+                    yield connection
+
+    This wrapper can be used instead for the above like this::
+
+        def connection_or_default_connection(connection=None):
+            return AsyncFallbackContext(connection, create_new_connection)
+    """
+
+    def __init__(
+        self,
+        provided: typing.Any,
+        fallback: typing.AsyncContextManager,
+        *fb_args, **fb_kwargs
+    ):
+        self.provided = provided
+        self.fallback = fallback
+        self.fb_args = fb_args
+        self.fb_kwargs = fb_kwargs
+        self._context = None
+
+    async def __aenter__(self):
+        if self.provided is not None:
+            return self.provided
+        context = self._context = self.fallback(
+            *self.fb_args, **self.fb_kwargs
+        )
+        return await context.__aenter__()
+
+    async def __aexit__(self, *exc_info):
+        if self._context is not None:
+            return await self._context.__aexit__(*exc_info)
+
+
+class getitem_property:
+    """Attribute -> dict key descriptor.
+
+    The target object must support ``__getitem__``,
+    and optionally ``__setitem__``.
+
+    Example:
+        >>> from collections import defaultdict
+
+        >>> class Me(dict):
+        ...     deep = defaultdict(dict)
+        ...
+        ...     foo = getitem_property('foo')
+        ...     deep_thing = getitem_property('deep.thing')
+
+
+        >>> me = Me()
+        >>> me.foo
+        None
+
+        >>> me.foo = 10
+        >>> me.foo
+        10
+        >>> me['foo']
+        10
+
+        >>> me.deep_thing = 42
+        >>> me.deep_thing
+        42
+        >>> me.deep
+        defaultdict(<type 'dict'>, {'thing': 42})
+    """
+
+    def __init__(self, keypath, doc=None):
+        path, _, self.key = keypath.rpartition('.')
+        self.path = path.split('.') if path else None
+        self.__doc__ = doc
+
+    def _path(self, obj):
+        return (reduce(lambda d, k: d[k], [obj] + self.path) if self.path
+                else obj)
+
+    def __get__(self, obj, type=None):
+        if obj is None:
+            return type
+        return self._path(obj).get(self.key)
+
+    def __set__(self, obj, value):
+        self._path(obj)[self.key] = value
```

### Comparing `deepfos-celery-1.0.2/celery/utils/saferepr.py` & `deepfos-celery-1.0.3/celery/utils/saferepr.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/serialization.py` & `deepfos-celery-1.0.3/celery/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/static/celery_128.png` & `deepfos-celery-1.0.3/celery/utils/static/celery_128.png`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/sysinfo.py` & `deepfos-celery-1.0.3/celery/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/term.py` & `deepfos-celery-1.0.3/celery/utils/term.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/text.py` & `deepfos-celery-1.0.3/celery/utils/text.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/threads.py` & `deepfos-celery-1.0.3/celery/utils/threads.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/time.py` & `deepfos-celery-1.0.3/celery/utils/time.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/utils/timer2.py` & `deepfos-celery-1.0.3/celery/utils/timer2.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/autoscale.py` & `deepfos-celery-1.0.3/celery/worker/autoscale.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/components.py` & `deepfos-celery-1.0.3/celery/worker/components.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/agent.py` & `deepfos-celery-1.0.3/celery/worker/consumer/agent.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/connection.py` & `deepfos-celery-1.0.3/celery/worker/consumer/connection.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/consumer.py` & `deepfos-celery-1.0.3/celery/worker/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/control.py` & `deepfos-celery-1.0.3/celery/worker/consumer/control.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/events.py` & `deepfos-celery-1.0.3/celery/worker/consumer/events.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/gossip.py` & `deepfos-celery-1.0.3/celery/worker/consumer/gossip.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/heart.py` & `deepfos-celery-1.0.3/celery/worker/consumer/heart.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/mingle.py` & `deepfos-celery-1.0.3/celery/worker/consumer/mingle.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/consumer/tasks.py` & `deepfos-celery-1.0.3/celery/worker/consumer/tasks.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/control.py` & `deepfos-celery-1.0.3/celery/worker/control.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/heartbeat.py` & `deepfos-celery-1.0.3/celery/worker/heartbeat.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/loops.py` & `deepfos-celery-1.0.3/celery/worker/loops.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/pidbox.py` & `deepfos-celery-1.0.3/celery/worker/pidbox.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/request.py` & `deepfos-celery-1.0.3/celery/worker/request.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/state.py` & `deepfos-celery-1.0.3/celery/worker/state.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/strategy.py` & `deepfos-celery-1.0.3/celery/worker/strategy.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/celery/worker/worker.py` & `deepfos-celery-1.0.3/celery/worker/worker.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/deepfos_celery.egg-info/PKG-INFO` & `deepfos-celery-1.0.3/deepfos_celery.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfos-celery
-Version: 1.0.2
+Version: 1.0.3
 Summary: Distributed Task Queue.
 Home-page: http://celeryproject.org
 Author: DeepFOS
 Author-email: python@deepfinance.com
 License: BSD
 Project-URL: Documentation, http://docs.celeryproject.org/en/latest/index.html
 Project-URL: Code, https://gitee.com/python-development-team/deepfos-celery/
@@ -22,121 +22,121 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6,
-Provides-Extra: pymemcache
-Provides-Extra: pyro
-Provides-Extra: sqs
-Provides-Extra: s3
+Provides-Extra: auth
 Provides-Extra: cassandra
+Provides-Extra: pyro
+Provides-Extra: gevent
 Provides-Extra: mongodb
-Provides-Extra: zookeeper
-Provides-Extra: azureblockblob
-Provides-Extra: eventlet
-Provides-Extra: solar
-Provides-Extra: tblib
-Provides-Extra: slmq
-Provides-Extra: sqlalchemy
-Provides-Extra: auth
-Provides-Extra: zstd
-Provides-Extra: brotli
 Provides-Extra: couchbase
-Provides-Extra: dynamodb
-Provides-Extra: elasticsearch
-Provides-Extra: gevent
-Provides-Extra: arangodb
+Provides-Extra: cosmosdbsql
 Provides-Extra: pytest
-Provides-Extra: lzma
+Provides-Extra: sqlalchemy
 Provides-Extra: yaml
+Provides-Extra: pymemcache
+Provides-Extra: consul
 Provides-Extra: msgpack
-Provides-Extra: cosmosdbsql
+Provides-Extra: brotli
 Provides-Extra: django
+Provides-Extra: zookeeper
+Provides-Extra: lzma
+Provides-Extra: sqs
 Provides-Extra: redis
-Provides-Extra: consul
+Provides-Extra: s3
+Provides-Extra: couchdb
+Provides-Extra: azureblockblob
+Provides-Extra: dynamodb
+Provides-Extra: arangodb
+Provides-Extra: slmq
+Provides-Extra: tblib
 Provides-Extra: librabbitmq
+Provides-Extra: solar
 Provides-Extra: memcache
-Provides-Extra: couchdb
+Provides-Extra: zstd
+Provides-Extra: eventlet
+Provides-Extra: elasticsearch
 License-File: LICENSE
 
-.. image:: http://docs.celeryproject.org/en/latest/_images/celery-banner-small.png
-
-|license| |wheel| |pyversion|
-
-:Version: 1.0.0
-:Web: http://celeryproject.org/
-:Download: https://pypi.org/project/celery/
-:Source: https://gitee.com/python-development-team/deepfos-celery/
-:Keywords: task, queue, job, async, rabbitmq, amqp, redis,
-  python, distributed, actors
-
-What is this?
-=============
-
-本项目基于 ``celery-5.0.5`` 开发，主要功能是添加 ``asyncio`` 支持，
-以更好地和 ``FastAPI`` 等异步web框架配合使用。
-
-项目是 ``celery`` 的超集，但并非所有功能都支持 ``asyncio`` ，
-并且目前仅完成了 ``redis`` 作为 ``broker`` 和 ``backend`` 的支持。
-
-
-Get Started
-===========
-
-创建任务和官方 ``celery`` 一样:
-
-.. code-block:: python
-
-    from celery import Celery
-
-    app = Celery('hello', broker='redis://:@localhost/')
-
-    @app.task(aio_variant=True)
-    def hello():
-        return 'hello world'
-
-
-但增加了 ``aio_variant`` 这一参数，相较于普通的任务发送和获取结果的方式：
-
-.. code-block:: python
-
-    task = hello.apply_async()
-    result = task.get()
-
-
-可以使用:
-
-.. code-block:: python
-
-    task = await hello.aio.apply_async()
-    result = await task.get()
-
-
-**注意**
-
-    这不只是一个简单的语法糖，而是确实使用 ``aioredis`` 替换了原有 ``redis-py`` 的同步网络请求。
-
-
-.. _license:
-
-License
-=======
-
-This software is licensed under the `New BSD License`. See the ``LICENSE``
-file in the top distribution directory for the full license text.
-
-.. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
-
-.. |license| image:: https://img.shields.io/pypi/l/celery.svg
-    :alt: BSD License
-    :target: https://opensource.org/licenses/BSD-3-Clause
-
-.. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
-    :alt: Celery can be installed via wheel
-    :target: https://pypi.org/project/celery/
-
-.. |pyversion| image:: https://img.shields.io/pypi/pyversions/celery.svg
-    :alt: Supported Python versions.
-    :target: https://pypi.org/project/celery/
-
+.. image:: http://docs.celeryproject.org/en/latest/_images/celery-banner-small.png
+
+|license| |wheel| |pyversion|
+
+:Version: 1.0.0
+:Web: http://celeryproject.org/
+:Download: https://pypi.org/project/celery/
+:Source: https://gitee.com/python-development-team/deepfos-celery/
+:Keywords: task, queue, job, async, rabbitmq, amqp, redis,
+  python, distributed, actors
+
+What is this?
+=============
+
+本项目基于 ``celery-5.0.5`` 开发，主要功能是添加 ``asyncio`` 支持，
+以更好地和 ``FastAPI`` 等异步web框架配合使用。
+
+项目是 ``celery`` 的超集，但并非所有功能都支持 ``asyncio`` ，
+并且目前仅完成了 ``redis`` 作为 ``broker`` 和 ``backend`` 的支持。
+
+
+Get Started
+===========
+
+创建任务和官方 ``celery`` 一样:
+
+.. code-block:: python
+
+    from celery import Celery
+
+    app = Celery('hello', broker='redis://:@localhost/')
+
+    @app.task(aio_variant=True)
+    def hello():
+        return 'hello world'
+
+
+但增加了 ``aio_variant`` 这一参数，相较于普通的任务发送和获取结果的方式：
+
+.. code-block:: python
+
+    task = hello.apply_async()
+    result = task.get()
+
+
+可以使用:
+
+.. code-block:: python
+
+    task = await hello.aio.apply_async()
+    result = await task.get()
+
+
+**注意**
+
+    这不只是一个简单的语法糖，而是确实使用 ``aioredis`` 替换了原有 ``redis-py`` 的同步网络请求。
+
+
+.. _license:
+
+License
+=======
+
+This software is licensed under the `New BSD License`. See the ``LICENSE``
+file in the top distribution directory for the full license text.
+
+.. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
+
+.. |license| image:: https://img.shields.io/pypi/l/celery.svg
+    :alt: BSD License
+    :target: https://opensource.org/licenses/BSD-3-Clause
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
+    :alt: Celery can be installed via wheel
+    :target: https://pypi.org/project/celery/
+
+.. |pyversion| image:: https://img.shields.io/pypi/pyversions/celery.svg
+    :alt: Supported Python versions.
+    :target: https://pypi.org/project/celery/
+
```

### Comparing `deepfos-celery-1.0.2/deepfos_celery.egg-info/SOURCES.txt` & `deepfos-celery-1.0.3/deepfos_celery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 celery/utils/functional.py
 celery/utils/graph.py
 celery/utils/imports.py
 celery/utils/iso8601.py
 celery/utils/log.py
 celery/utils/nodenames.py
 celery/utils/objects.py
+celery/utils/psutil.py
 celery/utils/saferepr.py
 celery/utils/serialization.py
 celery/utils/sysinfo.py
 celery/utils/term.py
 celery/utils/text.py
 celery/utils/threads.py
 celery/utils/time.py
```

### Comparing `deepfos-celery-1.0.2/deepfos_celery.egg-info/requires.txt` & `deepfos-celery-1.0.3/deepfos_celery.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/requirements/README.rst` & `deepfos-celery-1.0.3/requirements/README.rst`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/requirements/test-ci-default.txt` & `deepfos-celery-1.0.3/requirements/test-ci-default.txt`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/setup.cfg` & `deepfos-celery-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/benchmarks/bench_worker.py` & `deepfos-celery-1.0.3/t/benchmarks/bench_worker.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/distro/test_CI_reqs.py` & `deepfos-celery-1.0.3/t/distro/test_CI_reqs.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/integration/redissrv.py` & `deepfos-celery-1.0.3/t/integration/redissrv.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-import subprocess
-import socket
-import os
-from tempfile import NamedTemporaryFile
-
-
-def get_redis_connection(port=None):
-    from redis import StrictRedis
-    return StrictRedis(
-        port=port
-    )
-
-
-class RedisServer:
-    def __init__(self, redis_executable=None):
-        self._serving = False
-        self._proc: subprocess.Popen = None
-        self._redis = redis_executable or self.find_executable('redis-server')
-        self._port = self.find_available_port()
-
-    def as_url(self):
-        return f"redis://:{self.port}"
-
-    @property
-    def client(self):
-        from redis import StrictRedis
-        return StrictRedis(port=self.port)
-
-    @property
-    def port(self):
-        return self._port
-
-    @staticmethod
-    def find_executable(exe):
-        try:
-            executable = subprocess.check_output(
-                f"which {exe}".split(), text=True)
-            return executable.strip()
-        except subprocess.CalledProcessError:
-            raise RuntimeError(f'exe not avaliable.')
-
-    @staticmethod
-    def find_available_port() -> int:
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
-            sock.bind(("localhost", 0))
-            return sock.getsockname()[1]
-
-    def get_start_cmd(self):
-        return f"nohup {self._redis} --port {self._port}".split()
-
-    def start(self):
-        if self._serving:
-            return
-        cmd = self.get_start_cmd()
-        self._proc = subprocess.Popen(
-            cmd, stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-        )
-        self._serving = True
-
-    def stop(self):
-        if not self._serving:
-            return
-        self._proc.terminate()
-        self._proc.wait()
-        self._proc = None
-        self._serving = False
-
-    def restart(self):
-        self.stop()
-        self.start()
-
-    def kill_clients(self, type='all'):
-        if type == 'all':
-            types = ['normal', 'pubsub']
-        else:
-            types = [type.lower()]
-
-        with self.client.pipeline() as pipe:
-            for t in types:
-                pipe.client_kill_filter(_type=t)
-            pipe.execute()
-
-    def kill_by_port(self, port):
-        self.client.client_kill(f"127.0.0.1:{port}")
-
-    def pause(self, seconds):
-        self.client.client_pause(timeout=int(seconds * 1000))
-
-    def __repr__(self):
-        if self._serving:
-            return f"Redis | Port: {self._port} | PID: {self._proc.pid}"
-        else:
-            return f"Redis | Stopped"
-
-    def __del__(self):
-        self.stop()
-
-
-class RedisSentinelServer(RedisServer):
-    def __init__(self, master_name: str = 'mymaster', redis_executable=None):
-        super().__init__(redis_executable)
-        self.master_name = master_name
-        self.master = RedisServer()
-        self._redis = redis_executable or self.find_executable(
-            'redis-sentinel')
-        self._conf = None
-
-    def as_url(self):
-        return f"sentinel://:{self.port}"
-
-    @property
-    def client(self):
-        from redis.sentinel import Sentinel
-        s = Sentinel([('localhost', self.port)])
-        return s.master_for(self.master_name)
-
-    def get_start_cmd(self):
-        conf = self.create_configure()
-        return f"nohup {self._redis} {conf.name}".split()
-
-    def create_configure(self):
-        configure = "\n".join((
-            f"port {self.port}",
-            f"sentinel monitor {self.master_name} localhost {self.master.port} 2",
-            f"sentinel config-epoch {self.master_name} 0",
-            "sentinel deny-scripts-reconfig yes"
-        ))
-        self._conf = f = NamedTemporaryFile(
-            mode='wt', delete=False, encoding='utf8')
-        f.writelines(configure)
-        f.flush()
-        return f
-
-    def start(self):
-        if self._serving:
-            return
-        self.master.start()
-        super().start()
-
-    def stop(self):
-        if not self._serving:
-            return
-
-        super().stop()
-        self._conf.close()
-        os.unlink(self._conf.name)
-        self.master.stop()
+import subprocess
+import socket
+import os
+from tempfile import NamedTemporaryFile
+
+
+def get_redis_connection(port=None):
+    from redis import StrictRedis
+    return StrictRedis(
+        port=port
+    )
+
+
+class RedisServer:
+    def __init__(self, redis_executable=None):
+        self._serving = False
+        self._proc: subprocess.Popen = None
+        self._redis = redis_executable or self.find_executable('redis-server')
+        self._port = self.find_available_port()
+
+    def as_url(self):
+        return f"redis://:{self.port}"
+
+    @property
+    def client(self):
+        from redis import StrictRedis
+        return StrictRedis(port=self.port)
+
+    @property
+    def port(self):
+        return self._port
+
+    @staticmethod
+    def find_executable(exe):
+        try:
+            executable = subprocess.check_output(
+                f"which {exe}".split(), text=True)
+            return executable.strip()
+        except subprocess.CalledProcessError:
+            raise RuntimeError(f'exe not avaliable.')
+
+    @staticmethod
+    def find_available_port() -> int:
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
+            sock.bind(("localhost", 0))
+            return sock.getsockname()[1]
+
+    def get_start_cmd(self):
+        return f"nohup {self._redis} --port {self._port}".split()
+
+    def start(self):
+        if self._serving:
+            return
+        cmd = self.get_start_cmd()
+        self._proc = subprocess.Popen(
+            cmd, stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL,
+        )
+        self._serving = True
+
+    def stop(self):
+        if not self._serving:
+            return
+        self._proc.terminate()
+        self._proc.wait()
+        self._proc = None
+        self._serving = False
+
+    def restart(self):
+        self.stop()
+        self.start()
+
+    def kill_clients(self, type='all'):
+        if type == 'all':
+            types = ['normal', 'pubsub']
+        else:
+            types = [type.lower()]
+
+        with self.client.pipeline() as pipe:
+            for t in types:
+                pipe.client_kill_filter(_type=t)
+            pipe.execute()
+
+    def kill_by_port(self, port):
+        self.client.client_kill(f"127.0.0.1:{port}")
+
+    def pause(self, seconds):
+        self.client.client_pause(timeout=int(seconds * 1000))
+
+    def __repr__(self):
+        if self._serving:
+            return f"Redis | Port: {self._port} | PID: {self._proc.pid}"
+        else:
+            return f"Redis | Stopped"
+
+    def __del__(self):
+        self.stop()
+
+
+class RedisSentinelServer(RedisServer):
+    def __init__(self, master_name: str = 'mymaster', redis_executable=None):
+        super().__init__(redis_executable)
+        self.master_name = master_name
+        self.master = RedisServer()
+        self._redis = redis_executable or self.find_executable(
+            'redis-sentinel')
+        self._conf = None
+
+    def as_url(self):
+        return f"sentinel://:{self.port}"
+
+    @property
+    def client(self):
+        from redis.sentinel import Sentinel
+        s = Sentinel([('localhost', self.port)])
+        return s.master_for(self.master_name)
+
+    def get_start_cmd(self):
+        conf = self.create_configure()
+        return f"nohup {self._redis} {conf.name}".split()
+
+    def create_configure(self):
+        configure = "\n".join((
+            f"port {self.port}",
+            f"sentinel monitor {self.master_name} localhost {self.master.port} 2",
+            f"sentinel config-epoch {self.master_name} 0",
+            "sentinel deny-scripts-reconfig yes"
+        ))
+        self._conf = f = NamedTemporaryFile(
+            mode='wt', delete=False, encoding='utf8')
+        f.writelines(configure)
+        f.flush()
+        return f
+
+    def start(self):
+        if self._serving:
+            return
+        self.master.start()
+        super().start()
+
+    def stop(self):
+        if not self._serving:
+            return
+
+        super().stop()
+        self._conf.close()
+        os.unlink(self._conf.name)
+        self.master.stop()
```

### Comparing `deepfos-celery-1.0.2/t/integration/test_aiocanvas.py` & `deepfos-celery-1.0.3/t/integration/test_aiocanvas.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import pytest
-
-from celery.aio.result import GroupResult
-from celery.aio.canvas import group
-from t.base import AsyncFlakyTest, FlakyMixin
-
-from .tasks import (ExpectedException, add, add_chord_to_chord, add_replaced,
-                    add_to_all, add_to_all_to_chord, build_chain_inside_task,
-                    chord_error, collect_ids, delayed_sum,
-                    delayed_sum_with_soft_guard, fail, identity, ids,
-                    print_unicode, raise_error, redis_echo,
-                    replace_with_chain, replace_with_chain_which_raises,
-                    replace_with_empty_chain, retry_once, return_exception,
-                    return_priority, second_order_replace1, tsum)
-
-from .test_canvas import assert_ping, TIMEOUT
-
-
-class test_group(AsyncFlakyTest):
-    async def test_ready_with_exception(self, manager):
-        if not manager.app.conf.result_backend.startswith('redis'):
-            raise pytest.skip('Requires redis result backend.')
-
-        g = group([add.aio.s(1, 2), raise_error.aio.s()])
-        result = await g.apply_async()
-        while not await result.ready():
-            pass
-
-    async def test_empty_group_result(self, manager):
-        if not manager.app.conf.result_backend.startswith('redis'):
-            raise pytest.skip('Requires redis result backend.')
-
-        task = group([])
-        result = await task.apply_async()
-
-        await GroupResult.save(result)
-        task = await GroupResult.restore(result.id)
-        assert task.results == []
-
-    async def test_nested_group(self, manager):
-        assert_ping(manager)
-
-        c = group(
-            add.aio.si(1, 10),
-            group(
-                add.aio.si(1, 100),
-                group(
-                    add.aio.si(1, 1000),
-                    add.aio.si(1, 2000),
-                ),
-            ),
-        )
-        res = await c()
-
-        assert await res.get(timeout=TIMEOUT) == [11, 101, 1001, 2001]
-
-    async def test_large_group(self, manager):
-        assert_ping(manager)
-
-        c = group(identity.aio.s(i) for i in range(1000))
-        res = await c.delay()
-
-        assert await res.get(timeout=TIMEOUT) == list(range(1000))
-
-    async def test_group_lone(self, manager):
-        """
-        Test that a simple group completes.
-        """
-        sig = group(identity.aio.s(42), identity.aio.s(42))     # [42, 42]
-        res = await sig.delay()
-        assert await res.get(timeout=TIMEOUT) == [42, 42]
-
-    async def test_nested_group_group(self, manager):
-        """
-        Confirm that groups nested inside groups get unrolled.
-        """
-        sig = group(
-            group(identity.aio.s(42), identity.aio.s(42)),  # [42, 42]
-        )                                       # [42, 42] due to unrolling
-        res = await sig.delay()
-        assert await res.get(timeout=TIMEOUT) == [42, 42]
-
-    async def test_group_restore_fast(self):
-        sig = group(
-            group(identity.aio.s(42), identity.aio.s(42)),  # [42, 42]
-        )
-        g = await sig.delay()
-        await g.save()
-        g_clone = await GroupResult.restore(g.id)
-        assert await g_clone.get(timeout=5) == [42, 42]
-
-    async def test_group_restore_slow(self):
-        sig = group(
-            group(delayed_sum.aio.s([40, 2]), delayed_sum.aio.s([2, 40], 2)),  # [42, 42]
-        )
-        g = await sig.delay()
-        await g.save()
-        g_clone = await GroupResult.restore(g.id)
-        assert await g_clone.get(timeout=6) == [42, 42]
+import pytest
+
+from celery.aio.result import GroupResult
+from celery.aio.canvas import group
+from t.base import AsyncFlakyTest, FlakyMixin
+
+from .tasks import (ExpectedException, add, add_chord_to_chord, add_replaced,
+                    add_to_all, add_to_all_to_chord, build_chain_inside_task,
+                    chord_error, collect_ids, delayed_sum,
+                    delayed_sum_with_soft_guard, fail, identity, ids,
+                    print_unicode, raise_error, redis_echo,
+                    replace_with_chain, replace_with_chain_which_raises,
+                    replace_with_empty_chain, retry_once, return_exception,
+                    return_priority, second_order_replace1, tsum)
+
+from .test_canvas import assert_ping, TIMEOUT
+
+
+class test_group(AsyncFlakyTest):
+    async def test_ready_with_exception(self, manager):
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+
+        g = group([add.aio.s(1, 2), raise_error.aio.s()])
+        result = await g.apply_async()
+        while not await result.ready():
+            pass
+
+    async def test_empty_group_result(self, manager):
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+
+        task = group([])
+        result = await task.apply_async()
+
+        await GroupResult.save(result)
+        task = await GroupResult.restore(result.id)
+        assert task.results == []
+
+    async def test_nested_group(self, manager):
+        assert_ping(manager)
+
+        c = group(
+            add.aio.si(1, 10),
+            group(
+                add.aio.si(1, 100),
+                group(
+                    add.aio.si(1, 1000),
+                    add.aio.si(1, 2000),
+                ),
+            ),
+        )
+        res = await c()
+
+        assert await res.get(timeout=TIMEOUT) == [11, 101, 1001, 2001]
+
+    async def test_large_group(self, manager):
+        assert_ping(manager)
+
+        c = group(identity.aio.s(i) for i in range(1000))
+        res = await c.delay()
+
+        assert await res.get(timeout=TIMEOUT) == list(range(1000))
+
+    async def test_group_lone(self, manager):
+        """
+        Test that a simple group completes.
+        """
+        sig = group(identity.aio.s(42), identity.aio.s(42))     # [42, 42]
+        res = await sig.delay()
+        assert await res.get(timeout=TIMEOUT) == [42, 42]
+
+    async def test_nested_group_group(self, manager):
+        """
+        Confirm that groups nested inside groups get unrolled.
+        """
+        sig = group(
+            group(identity.aio.s(42), identity.aio.s(42)),  # [42, 42]
+        )                                       # [42, 42] due to unrolling
+        res = await sig.delay()
+        assert await res.get(timeout=TIMEOUT) == [42, 42]
+
+    async def test_group_restore_fast(self):
+        sig = group(
+            group(identity.aio.s(42), identity.aio.s(42)),  # [42, 42]
+        )
+        g = await sig.delay()
+        await g.save()
+        g_clone = await GroupResult.restore(g.id)
+        assert await g_clone.get(timeout=5) == [42, 42]
+
+    async def test_group_restore_slow(self):
+        sig = group(
+            group(delayed_sum.aio.s([40, 2]), delayed_sum.aio.s([2, 40], 2)),  # [42, 42]
+        )
+        g = await sig.delay()
+        await g.save()
+        g_clone = await GroupResult.restore(g.id)
+        assert await g_clone.get(timeout=6) == [42, 42]
```

### Comparing `deepfos-celery-1.0.2/t/integration/test_aiotasks.py` & `deepfos-celery-1.0.3/t/integration/test_aiotasks.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,296 +1,296 @@
-import asyncio
-import time
-from asyncio import sleep
-from datetime import datetime, timedelta
-from time import perf_counter
-
-import pytest
-
-import celery
-from celery import group
-
-from .conftest import get_active_redis_channels
-from .tasks import (ClassBasedAutoRetryTask, ExpectedException, add,
-                    add_ignore_result, add_not_typed, fail, print_unicode,
-                    retry, retry_once, retry_once_priority, sleeping)
-from t.base import AsyncTest, AsyncFlakyTest, FlakyTest
-
-
-TIMEOUT = 10
-
-
-class test_class_based_tasks(FlakyTest):
-    def test_class_based_task_retried(self, celery_session_app,
-                                      celery_session_worker):
-        task = ClassBasedAutoRetryTask()
-        celery_session_app.tasks.register(task)
-        res = task.delay()
-        assert res.get(timeout=TIMEOUT) == 1
-
-
-async def _concurrent_runner(j, repeat=10):
-    expects = [i + j for i in range(repeat)]
-    # Tests calling task only with args
-    async_results = await asyncio.gather(
-        *(
-            add.aio.delay(i, j)
-            for i in range(repeat)
-        )
-    )
-
-    results = await asyncio.gather(
-        *(
-            r.get(timeout=10)
-            for r in async_results
-        )
-    )
-
-    for expected, result, ar in zip(expects, results, async_results):
-        assert result == expected
-        assert (await ar.status) == 'SUCCESS'
-        assert (await ar.ready()) is True
-        assert (await ar.successful()) is True
-
-
-_loop = None
-
-def _producer(j):
-    """Single producer helper function"""
-    global _loop
-
-    if _loop is None:
-        _loop = asyncio.new_event_loop()
-    _loop.run_until_complete(_concurrent_runner(j, repeat=20))
-    return j
-
-
-async def assert_task_succeed(result):
-    assert (await result.status) == 'SUCCESS'
-    assert (await result.ready()) is True
-    assert (await result.successful()) is True
-
-
-class test_tasks(AsyncFlakyTest):
-    async def test_basic_task(self, manager):
-        """Tests basic task call"""
-        results = []
-        # Tests calling task only with args
-        for i in range(10):
-            results.append([i + i, await add.aio.delay(i, i)])
-        for expected, result in results:
-            value = await result.get(timeout=10)
-            assert value == expected
-            await assert_task_succeed(result)
-
-        results = []
-        # Tests calling task with args and kwargs
-        for i in range(10):
-            results.append([3*i, await add.aio.delay(i, i, z=i)])
-        for expected, result in results:
-            value = await result.get(timeout=10)
-            assert value == expected
-            await assert_task_succeed(result)
-
-    async def test_concurrent_task_only_args(self, manager):
-        """Tests basic task call"""
-        await _concurrent_runner(10, repeat=20)
-
-    async def test_concurrent_task_with_kwargs(self, manager):
-        """Tests basic task call"""
-        expects = [3*i for i in range(20)]
-        # Tests calling task only with args
-        async_results = await asyncio.gather(*(
-            add.aio.delay(i, i, z=i)
-            for i in range(10)
-        ))
-
-        results = await asyncio.gather(*(
-            r.get(timeout=10)
-            for r in async_results
-        ))
-
-        for expected, result, ar in zip(expects, results, async_results):
-            assert result == expected
-            await assert_task_succeed(ar)
-
-    def test_multiprocess_producer(self, manager):
-        """Testing multiple processes calling tasks."""
-        from multiprocessing import Pool
-        pool = Pool(20)
-        ret = pool.map(_producer, range(120))
-        assert list(ret) == list(range(120))
-
-    async def test_ignore_result(self, manager):
-        """Testing calling task with ignoring results."""
-        result = await add.aio.apply_async((1, 2), ignore_result=True)
-        assert (await result.get()) is None
-
-    async def test_timeout(self, manager):
-        """Testing timeout of getting results from tasks."""
-        result = await sleeping.aio.delay(10)
-        with pytest.raises(celery.exceptions.TimeoutError):
-            await result.get(timeout=5)
-
-    async def test_expired(self, manager):
-        """Testing expiration of task."""
-        # Fill the queue with tasks which took > 1 sec to process
-        for _ in range(4):
-            await sleeping.aio.delay(2)
-        # Execute task with expiration = 1 sec
-        result = await add.aio.apply_async((1, 1), expires=1)
-        with pytest.raises(celery.exceptions.TaskRevokedError):
-            await result.get()
-        assert (await result.status) == 'REVOKED'
-        assert (await result.ready()) is True
-        assert (await result.failed()) is False
-        assert (await result.successful()) is False
-
-        # Fill the queue with tasks which took > 1 sec to process
-        for _ in range(4):
-            await sleeping.aio.delay(2)
-        # Execute task with expiration at now + 1 sec
-        result = await add.aio.apply_async((1, 1), expires=datetime.utcnow() + timedelta(seconds=1))
-        with pytest.raises(celery.exceptions.TaskRevokedError):
-            await result.get()
-        assert (await result.status) == 'REVOKED'
-        assert (await result.ready()) is True
-        assert (await result.failed()) is False
-        assert (await result.successful()) is False
-
-    async def test_eta(self, manager):
-        """Tests tasks scheduled at some point in future."""
-        start = perf_counter()
-        # Schedule task to be executed in 3 seconds
-        result = await add.aio.apply_async((1, 1), countdown=3)
-        await sleep(1)
-        assert (await result.status) == 'PENDING'
-        assert (await result.ready()) is False
-        assert (await result.get()) == 2
-        end = perf_counter()
-        assert (await result.status) == 'SUCCESS'
-        assert (await result.ready()) is True
-        # Difference between calling the task and result must be bigger than 3 secs
-        assert (end - start) > 3
-
-        start = perf_counter()
-        # Schedule task to be executed at time now + 3 seconds
-        result = await add.aio.apply_async((2, 2), eta=datetime.utcnow() + timedelta(seconds=3))
-        await sleep(1)
-        assert (await result.status) == 'PENDING'
-        assert (await result.ready()) is False
-        assert (await result.get()) == 4
-        end = perf_counter()
-        assert (await result.status) == 'SUCCESS'
-        assert (await result.ready()) is True
-        # Difference between calling the task and result must be bigger than 3 secs
-        assert (end - start) > 3
-
-    async def test_fail(self, manager):
-        """Tests that the failing task propagates back correct exception."""
-        result = await fail.aio.delay()
-        with pytest.raises(ExpectedException):
-            await result.get(timeout=5)
-        assert (await result.status) == 'FAILURE'
-        assert (await result.ready()) is True
-        assert (await result.failed()) is True
-        assert (await result.successful()) is False
-
-    async def test_wrong_arguments(self, manager):
-        """Tests that proper exceptions are raised when task is called with wrong arguments."""
-        with pytest.raises(TypeError):
-            add(5)
-
-        with pytest.raises(TypeError):
-            add(5, 5, wrong_arg=5)
-
-        with pytest.raises(TypeError):
-            await add.aio.delay(5)
-
-        with pytest.raises(TypeError):
-            await add.aio.delay(5, wrong_arg=5)
-
-        # Tasks with typing=False are not checked but execution should fail
-        result = await add_not_typed.aio.delay(5)
-        with pytest.raises(TypeError):
-            await result.get(timeout=5)
-        assert (await result.status) == 'FAILURE'
-
-        result = await add_not_typed.aio.delay(5, wrong_arg=5)
-        with pytest.raises(TypeError):
-            await result.get(timeout=5)
-        assert (await result.status) == 'FAILURE'
-
-    async def test_retry(self, manager):
-        """Tests retrying of task."""
-        # Tests when max. retries is reached
-        result = await retry.aio.delay()
-        for _ in range(5):
-            status = await (result.status)
-            if status != 'PENDING':
-                break
-            await sleep(1)
-        assert status == 'RETRY'
-        with pytest.raises(ExpectedException):
-            await result.get()
-        assert (await result.status) == 'FAILURE'
-
-        # Tests when task is retried but after returns correct result
-        result = await retry.aio.delay(return_value='bar')
-        for _ in range(5):
-            status = await (result.status)
-            if status != 'PENDING':
-                break
-            await sleep(1)
-        assert status == 'RETRY'
-        assert (await result.get()) == 'bar'
-        assert (await result.status) == 'SUCCESS'
-
-    async def test_task_accepted(self, manager, sleep=1):
-        r1 = await sleeping.aio.delay(sleep)
-        await sleeping.aio.delay(sleep)
-        manager.assert_accepted([r1.id])
-
-    async def test_task_retried(self):
-        res = await retry_once.aio.delay()
-        assert (await res.get(timeout=TIMEOUT)) == 1  # retried once
-
-    async def test_task_retried_priority(self):
-        res = await retry_once_priority.aio.apply_async(priority=7)
-        assert (await res.get(timeout=TIMEOUT)) == 7  # retried once with priority 7
-
-    async def not_yet_test_unicode_task(self, manager):
-        manager.join(
-            group(print_unicode.s() for _ in range(5))(),
-            timeout=TIMEOUT, propagate=True,
-        )
-
-
-class test_task_redis_result_backend(AsyncTest):
-    @pytest.fixture(autouse=True)
-    def setup(self, redis_server, manager):
-        if not manager.app.conf.result_backend.startswith('redis'):
-            raise pytest.skip('Requires redis result backend.')
-        redis_server.restart()
-        time.sleep(1)
-
-    async def test_ignoring_result_no_subscriptions(self):
-        assert get_active_redis_channels() == []
-        result = await add_ignore_result.aio.delay(1, 2)
-        assert result.ignored is True
-        assert get_active_redis_channels() == []
-
-    async def test_asyncresult_forget_cancels_subscription(self):
-        result = await add.aio.delay(1, 2)
-        assert get_active_redis_channels(as_string=True) == [
-            f"celery-task-meta-{result.id}"
-        ]
-        await result.forget()
-        assert get_active_redis_channels() == []
-
-    async def test_asyncresult_get_cancels_subscription(self):
-        result = await add.aio.delay(1, 2)
-        assert get_active_redis_channels(as_string=True) == [
-            f"celery-task-meta-{result.id}"
-        ]
-        assert (await result.get(timeout=3)) == 3
-        assert get_active_redis_channels() == []
+import asyncio
+import time
+from asyncio import sleep
+from datetime import datetime, timedelta
+from time import perf_counter
+
+import pytest
+
+import celery
+from celery import group
+
+from .conftest import get_active_redis_channels
+from .tasks import (ClassBasedAutoRetryTask, ExpectedException, add,
+                    add_ignore_result, add_not_typed, fail, print_unicode,
+                    retry, retry_once, retry_once_priority, sleeping)
+from t.base import AsyncTest, AsyncFlakyTest, FlakyTest
+
+
+TIMEOUT = 10
+
+
+class test_class_based_tasks(FlakyTest):
+    def test_class_based_task_retried(self, celery_session_app,
+                                      celery_session_worker):
+        task = ClassBasedAutoRetryTask()
+        celery_session_app.tasks.register(task)
+        res = task.delay()
+        assert res.get(timeout=TIMEOUT) == 1
+
+
+async def _concurrent_runner(j, repeat=10):
+    expects = [i + j for i in range(repeat)]
+    # Tests calling task only with args
+    async_results = await asyncio.gather(
+        *(
+            add.aio.delay(i, j)
+            for i in range(repeat)
+        )
+    )
+
+    results = await asyncio.gather(
+        *(
+            r.get(timeout=10)
+            for r in async_results
+        )
+    )
+
+    for expected, result, ar in zip(expects, results, async_results):
+        assert result == expected
+        assert (await ar.status) == 'SUCCESS'
+        assert (await ar.ready()) is True
+        assert (await ar.successful()) is True
+
+
+_loop = None
+
+def _producer(j):
+    """Single producer helper function"""
+    global _loop
+
+    if _loop is None:
+        _loop = asyncio.new_event_loop()
+    _loop.run_until_complete(_concurrent_runner(j, repeat=20))
+    return j
+
+
+async def assert_task_succeed(result):
+    assert (await result.status) == 'SUCCESS'
+    assert (await result.ready()) is True
+    assert (await result.successful()) is True
+
+
+class test_tasks(AsyncFlakyTest):
+    async def test_basic_task(self, manager):
+        """Tests basic task call"""
+        results = []
+        # Tests calling task only with args
+        for i in range(10):
+            results.append([i + i, await add.aio.delay(i, i)])
+        for expected, result in results:
+            value = await result.get(timeout=10)
+            assert value == expected
+            await assert_task_succeed(result)
+
+        results = []
+        # Tests calling task with args and kwargs
+        for i in range(10):
+            results.append([3*i, await add.aio.delay(i, i, z=i)])
+        for expected, result in results:
+            value = await result.get(timeout=10)
+            assert value == expected
+            await assert_task_succeed(result)
+
+    async def test_concurrent_task_only_args(self, manager):
+        """Tests basic task call"""
+        await _concurrent_runner(10, repeat=20)
+
+    async def test_concurrent_task_with_kwargs(self, manager):
+        """Tests basic task call"""
+        expects = [3*i for i in range(20)]
+        # Tests calling task only with args
+        async_results = await asyncio.gather(*(
+            add.aio.delay(i, i, z=i)
+            for i in range(10)
+        ))
+
+        results = await asyncio.gather(*(
+            r.get(timeout=10)
+            for r in async_results
+        ))
+
+        for expected, result, ar in zip(expects, results, async_results):
+            assert result == expected
+            await assert_task_succeed(ar)
+
+    def test_multiprocess_producer(self, manager):
+        """Testing multiple processes calling tasks."""
+        from multiprocessing import Pool
+        pool = Pool(20)
+        ret = pool.map(_producer, range(120))
+        assert list(ret) == list(range(120))
+
+    async def test_ignore_result(self, manager):
+        """Testing calling task with ignoring results."""
+        result = await add.aio.apply_async((1, 2), ignore_result=True)
+        assert (await result.get()) is None
+
+    async def test_timeout(self, manager):
+        """Testing timeout of getting results from tasks."""
+        result = await sleeping.aio.delay(10)
+        with pytest.raises(celery.exceptions.TimeoutError):
+            await result.get(timeout=5)
+
+    async def test_expired(self, manager):
+        """Testing expiration of task."""
+        # Fill the queue with tasks which took > 1 sec to process
+        for _ in range(4):
+            await sleeping.aio.delay(2)
+        # Execute task with expiration = 1 sec
+        result = await add.aio.apply_async((1, 1), expires=1)
+        with pytest.raises(celery.exceptions.TaskRevokedError):
+            await result.get()
+        assert (await result.status) == 'REVOKED'
+        assert (await result.ready()) is True
+        assert (await result.failed()) is False
+        assert (await result.successful()) is False
+
+        # Fill the queue with tasks which took > 1 sec to process
+        for _ in range(4):
+            await sleeping.aio.delay(2)
+        # Execute task with expiration at now + 1 sec
+        result = await add.aio.apply_async((1, 1), expires=datetime.utcnow() + timedelta(seconds=1))
+        with pytest.raises(celery.exceptions.TaskRevokedError):
+            await result.get()
+        assert (await result.status) == 'REVOKED'
+        assert (await result.ready()) is True
+        assert (await result.failed()) is False
+        assert (await result.successful()) is False
+
+    async def test_eta(self, manager):
+        """Tests tasks scheduled at some point in future."""
+        start = perf_counter()
+        # Schedule task to be executed in 3 seconds
+        result = await add.aio.apply_async((1, 1), countdown=3)
+        await sleep(1)
+        assert (await result.status) == 'PENDING'
+        assert (await result.ready()) is False
+        assert (await result.get()) == 2
+        end = perf_counter()
+        assert (await result.status) == 'SUCCESS'
+        assert (await result.ready()) is True
+        # Difference between calling the task and result must be bigger than 3 secs
+        assert (end - start) > 3
+
+        start = perf_counter()
+        # Schedule task to be executed at time now + 3 seconds
+        result = await add.aio.apply_async((2, 2), eta=datetime.utcnow() + timedelta(seconds=3))
+        await sleep(1)
+        assert (await result.status) == 'PENDING'
+        assert (await result.ready()) is False
+        assert (await result.get()) == 4
+        end = perf_counter()
+        assert (await result.status) == 'SUCCESS'
+        assert (await result.ready()) is True
+        # Difference between calling the task and result must be bigger than 3 secs
+        assert (end - start) > 3
+
+    async def test_fail(self, manager):
+        """Tests that the failing task propagates back correct exception."""
+        result = await fail.aio.delay()
+        with pytest.raises(ExpectedException):
+            await result.get(timeout=5)
+        assert (await result.status) == 'FAILURE'
+        assert (await result.ready()) is True
+        assert (await result.failed()) is True
+        assert (await result.successful()) is False
+
+    async def test_wrong_arguments(self, manager):
+        """Tests that proper exceptions are raised when task is called with wrong arguments."""
+        with pytest.raises(TypeError):
+            add(5)
+
+        with pytest.raises(TypeError):
+            add(5, 5, wrong_arg=5)
+
+        with pytest.raises(TypeError):
+            await add.aio.delay(5)
+
+        with pytest.raises(TypeError):
+            await add.aio.delay(5, wrong_arg=5)
+
+        # Tasks with typing=False are not checked but execution should fail
+        result = await add_not_typed.aio.delay(5)
+        with pytest.raises(TypeError):
+            await result.get(timeout=5)
+        assert (await result.status) == 'FAILURE'
+
+        result = await add_not_typed.aio.delay(5, wrong_arg=5)
+        with pytest.raises(TypeError):
+            await result.get(timeout=5)
+        assert (await result.status) == 'FAILURE'
+
+    async def test_retry(self, manager):
+        """Tests retrying of task."""
+        # Tests when max. retries is reached
+        result = await retry.aio.delay()
+        for _ in range(5):
+            status = await (result.status)
+            if status != 'PENDING':
+                break
+            await sleep(1)
+        assert status == 'RETRY'
+        with pytest.raises(ExpectedException):
+            await result.get()
+        assert (await result.status) == 'FAILURE'
+
+        # Tests when task is retried but after returns correct result
+        result = await retry.aio.delay(return_value='bar')
+        for _ in range(5):
+            status = await (result.status)
+            if status != 'PENDING':
+                break
+            await sleep(1)
+        assert status == 'RETRY'
+        assert (await result.get()) == 'bar'
+        assert (await result.status) == 'SUCCESS'
+
+    async def test_task_accepted(self, manager, sleep=1):
+        r1 = await sleeping.aio.delay(sleep)
+        await sleeping.aio.delay(sleep)
+        manager.assert_accepted([r1.id])
+
+    async def test_task_retried(self):
+        res = await retry_once.aio.delay()
+        assert (await res.get(timeout=TIMEOUT)) == 1  # retried once
+
+    async def test_task_retried_priority(self):
+        res = await retry_once_priority.aio.apply_async(priority=7)
+        assert (await res.get(timeout=TIMEOUT)) == 7  # retried once with priority 7
+
+    async def not_yet_test_unicode_task(self, manager):
+        manager.join(
+            group(print_unicode.s() for _ in range(5))(),
+            timeout=TIMEOUT, propagate=True,
+        )
+
+
+class test_task_redis_result_backend(AsyncTest):
+    @pytest.fixture(autouse=True)
+    def setup(self, redis_server, manager):
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+        redis_server.restart()
+        time.sleep(1)
+
+    async def test_ignoring_result_no_subscriptions(self):
+        assert get_active_redis_channels() == []
+        result = await add_ignore_result.aio.delay(1, 2)
+        assert result.ignored is True
+        assert get_active_redis_channels() == []
+
+    async def test_asyncresult_forget_cancels_subscription(self):
+        result = await add.aio.delay(1, 2)
+        assert get_active_redis_channels(as_string=True) == [
+            f"celery-task-meta-{result.id}"
+        ]
+        await result.forget()
+        assert get_active_redis_channels() == []
+
+    async def test_asyncresult_get_cancels_subscription(self):
+        result = await add.aio.delay(1, 2)
+        assert get_active_redis_channels(as_string=True) == [
+            f"celery-task-meta-{result.id}"
+        ]
+        assert (await result.get(timeout=3)) == 3
+        assert get_active_redis_channels() == []
```

### Comparing `deepfos-celery-1.0.2/t/integration/test_auto_recovery.py` & `deepfos-celery-1.0.3/t/integration/test_auto_recovery.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import asyncio
-
-import pytest
-
-from celery.aio.result import AsyncResult
-
-from t.base import AsyncFlakyTest
-from .tasks import sleeping
-from .test_aiotasks import assert_task_succeed
-
-
-class test_redis(AsyncFlakyTest):
-    @pytest.fixture(autouse=True)
-    def setup(self, manager):
-        pass
-
-    async def test_restart_between_two_tasks(self, redis_server):
-        result = await sleeping.aio.delay(1)
-        await result.get()
-        await assert_task_succeed(result)
-        redis_server.restart()
-        await asyncio.sleep(2)
-        result = await sleeping.aio.delay(1)
-        await result.get()
-        await assert_task_succeed(result)
-
-    async def test_restart_during_drain_events(self, redis_server):
-        result = await sleeping.aio.delay(4)
-        task = asyncio.create_task(result.get())
-        redis_server.restart()
-        await asyncio.sleep(2)
-        await task
-        await assert_task_succeed(result)
-
-    async def test_conn_closed_between_two_tasks(self, redis_server):
-        result = await sleeping.aio.delay(1)
-        await result.get()
-        await assert_task_succeed(result)
-        redis_server.kill_clients()
-        await asyncio.sleep(0.5)
-        result = await sleeping.aio.delay(1)
-        await result.get()
-        await assert_task_succeed(result)
-
-    async def test_conn_closed_during_drain_events(self, redis_server):
-        result = await sleeping.aio.delay(3)
-        task = asyncio.create_task(result.get())
-        redis_server.kill_clients()
-        await asyncio.sleep(0.5)
-        await task
-        await assert_task_succeed(result)
-
-    async def test_get_result_ok(self, redis_server):
-        r = await sleeping.aio.delay(1)
-        result = AsyncResult(r.id)
-        await r.get()
-        redis_server.kill_clients()
-        await asyncio.sleep(0.5)
-        await result.get()
-        await assert_task_succeed(r)
-        await assert_task_succeed(result)
-
-    async def test_concurrent_get_result_ok(self, redis_server):
-        result1 = await sleeping.aio.delay(2)
-        result2 = AsyncResult(result1.id)
-        task1 = asyncio.create_task(result1.get())
-        task2 = asyncio.create_task(result2.get())
-        await asyncio.sleep(0.5)
-        redis_server.kill_clients()
-        await asyncio.sleep(0.5)
-        await task1
-        await task2
-        await assert_task_succeed(result1)
-        await assert_task_succeed(result2)
-
-    async def test_empty_pubsub_after_reconnect(self, redis_server):
-        result = await sleeping.aio.delay(1)
-        task = asyncio.create_task(result.get())
-        await asyncio.sleep(0)
-        pubsub_port = (
-            result.backend.result_consumer
-                ._pubsub.connection
-                ._writer.transport
-                ._extra['sockname'][1]
-        )
-        redis_server.pause(1.5)
-        redis_server.kill_by_port(pubsub_port)
-        await asyncio.sleep(0.5)
-        await task
-        await assert_task_succeed(result)
-
-    async def test_get_result_on_finished(self, redis_server):
-        result = await sleeping.aio.delay(1)
-        await asyncio.sleep(1.5)
-        redis_server.kill_clients()
-        await asyncio.sleep(0.5)
-        await result.get()
-        await assert_task_succeed(result)
-
-    async def test_get_result_on_finished_with_new_result(self, redis_server):
-        r = await sleeping.aio.delay(1)
-        await r.get()
-        task_id = r.id
-        del r
-        await asyncio.sleep(1.5)
-        result = AsyncResult(task_id)
-        await result.backend.client.ping()
-        redis_server.kill_clients()
-        await asyncio.sleep(0.5)
-        await result.get()
-        await assert_task_succeed(result)
+import asyncio
+
+import pytest
+
+from celery.aio.result import AsyncResult
+
+from t.base import AsyncFlakyTest
+from .tasks import sleeping
+from .test_aiotasks import assert_task_succeed
+
+
+class test_redis(AsyncFlakyTest):
+    @pytest.fixture(autouse=True)
+    def setup(self, manager):
+        pass
+
+    async def test_restart_between_two_tasks(self, redis_server):
+        result = await sleeping.aio.delay(1)
+        await result.get()
+        await assert_task_succeed(result)
+        redis_server.restart()
+        await asyncio.sleep(2)
+        result = await sleeping.aio.delay(1)
+        await result.get()
+        await assert_task_succeed(result)
+
+    async def test_restart_during_drain_events(self, redis_server):
+        result = await sleeping.aio.delay(4)
+        task = asyncio.create_task(result.get())
+        redis_server.restart()
+        await asyncio.sleep(2)
+        await task
+        await assert_task_succeed(result)
+
+    async def test_conn_closed_between_two_tasks(self, redis_server):
+        result = await sleeping.aio.delay(1)
+        await result.get()
+        await assert_task_succeed(result)
+        redis_server.kill_clients()
+        await asyncio.sleep(0.5)
+        result = await sleeping.aio.delay(1)
+        await result.get()
+        await assert_task_succeed(result)
+
+    async def test_conn_closed_during_drain_events(self, redis_server):
+        result = await sleeping.aio.delay(3)
+        task = asyncio.create_task(result.get())
+        redis_server.kill_clients()
+        await asyncio.sleep(0.5)
+        await task
+        await assert_task_succeed(result)
+
+    async def test_get_result_ok(self, redis_server):
+        r = await sleeping.aio.delay(1)
+        result = AsyncResult(r.id)
+        await r.get()
+        redis_server.kill_clients()
+        await asyncio.sleep(0.5)
+        await result.get()
+        await assert_task_succeed(r)
+        await assert_task_succeed(result)
+
+    async def test_concurrent_get_result_ok(self, redis_server):
+        result1 = await sleeping.aio.delay(2)
+        result2 = AsyncResult(result1.id)
+        task1 = asyncio.create_task(result1.get())
+        task2 = asyncio.create_task(result2.get())
+        await asyncio.sleep(0.5)
+        redis_server.kill_clients()
+        await asyncio.sleep(0.5)
+        await task1
+        await task2
+        await assert_task_succeed(result1)
+        await assert_task_succeed(result2)
+
+    async def test_empty_pubsub_after_reconnect(self, redis_server):
+        result = await sleeping.aio.delay(1)
+        task = asyncio.create_task(result.get())
+        await asyncio.sleep(0)
+        pubsub_port = (
+            result.backend.result_consumer
+                ._pubsub.connection
+                ._writer.transport
+                ._extra['sockname'][1]
+        )
+        redis_server.pause(1.5)
+        redis_server.kill_by_port(pubsub_port)
+        await asyncio.sleep(0.5)
+        await task
+        await assert_task_succeed(result)
+
+    async def test_get_result_on_finished(self, redis_server):
+        result = await sleeping.aio.delay(1)
+        await asyncio.sleep(1.5)
+        redis_server.kill_clients()
+        await asyncio.sleep(0.5)
+        await result.get()
+        await assert_task_succeed(result)
+
+    async def test_get_result_on_finished_with_new_result(self, redis_server):
+        r = await sleeping.aio.delay(1)
+        await r.get()
+        task_id = r.id
+        del r
+        await asyncio.sleep(1.5)
+        result = AsyncResult(task_id)
+        await result.backend.client.ping()
+        redis_server.kill_clients()
+        await asyncio.sleep(0.5)
+        await result.get()
+        await assert_task_succeed(result)
```

### Comparing `deepfos-celery-1.0.2/t/integration/test_backend.py` & `deepfos-celery-1.0.3/t/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/integration/test_canvas.py` & `deepfos-celery-1.0.3/t/integration/test_canvas.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/integration/test_security.py` & `deepfos-celery-1.0.3/t/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/integration/test_tasks.py` & `deepfos-celery-1.0.3/t/integration/test_tasks.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,282 +1,282 @@
-from datetime import datetime, timedelta
-from time import perf_counter, sleep
-
-import pytest
-
-import celery
-from celery import group
-
-from .conftest import get_active_redis_channels
-from .tasks import (ClassBasedAutoRetryTask, ExpectedException, add,
-                    add_ignore_result, add_not_typed, fail, print_unicode,
-                    retry, retry_once, retry_once_priority, sleeping)
-
-TIMEOUT = 10
-
-
-_flaky = pytest.mark.flaky(reruns=5, reruns_delay=2)
-_timeout = pytest.mark.timeout(timeout=300)
-
-
-def flaky(fn):
-    return _timeout(_flaky(fn))
-
-
-class test_class_based_tasks:
-
-    @flaky
-    def test_class_based_task_retried(self, celery_session_app,
-                                      celery_session_worker):
-        task = ClassBasedAutoRetryTask()
-        celery_session_app.tasks.register(task)
-        res = task.delay()
-        assert res.get(timeout=TIMEOUT) == 1
-
-
-def _producer(j):
-    """Single producer helper function"""
-    results = []
-    for i in range(20):
-        results.append([i + j, add.delay(i, j)])
-    for expected, result in results:
-        value = result.get(timeout=10)
-        assert value == expected
-        assert result.status == 'SUCCESS'
-        assert result.ready() is True
-        assert result.successful() is True
-    return j
-
-
-class test_tasks:
-
-    def test_simple_call(self):
-        """Tests direct simple call of task"""
-        assert add(1, 1) == 2
-        assert add(1, 1, z=1) == 3
-
-    @flaky
-    def test_basic_task(self, manager):
-        """Tests basic task call"""
-        results = []
-        # Tests calling task only with args
-        for i in range(10):
-            results.append([i + i, add.delay(i, i)])
-        for expected, result in results:
-            value = result.get(timeout=10)
-            assert value == expected
-            assert result.status == 'SUCCESS'
-            assert result.ready() is True
-            assert result.successful() is True
-
-        results = []
-        # Tests calling task with args and kwargs
-        for i in range(10):
-            results.append([3*i, add.delay(i, i, z=i)])
-        for expected, result in results:
-            value = result.get(timeout=10)
-            assert value == expected
-            assert result.status == 'SUCCESS'
-            assert result.ready() is True
-            assert result.successful() is True
-
-    @flaky
-    def test_multiprocess_producer(self, manager):
-        """Testing multiple processes calling tasks."""
-        from multiprocessing import Pool
-        pool = Pool(20)
-        ret = pool.map(_producer, range(120))
-        assert list(ret) == list(range(120))
-
-    @flaky
-    def test_multithread_producer(self, manager):
-        """Testing multiple threads calling tasks."""
-        from multiprocessing.pool import ThreadPool
-        pool = ThreadPool(20)
-        ret = pool.map(_producer, range(120))
-        assert list(ret) == list(range(120))
-
-    @flaky
-    def test_ignore_result(self, manager):
-        """Testing calling task with ignoring results."""
-        result = add.apply_async((1, 2), ignore_result=True)
-        assert result.get() is None
-
-    @flaky
-    def test_timeout(self, manager):
-        """Testing timeout of getting results from tasks."""
-        result = sleeping.delay(10)
-        with pytest.raises(celery.exceptions.TimeoutError):
-            result.get(timeout=5)
-
-    @flaky
-    def test_expired(self, manager):
-        """Testing expiration of task."""
-        # Fill the queue with tasks which took > 1 sec to process
-        for _ in range(4):
-            sleeping.delay(2)
-        # Execute task with expiration = 1 sec
-        result = add.apply_async((1, 1), expires=1)
-        with pytest.raises(celery.exceptions.TaskRevokedError):
-            result.get()
-        assert result.status == 'REVOKED'
-        assert result.ready() is True
-        assert result.failed() is False
-        assert result.successful() is False
-
-        # Fill the queue with tasks which took > 1 sec to process
-        for _ in range(4):
-            sleeping.delay(2)
-        # Execute task with expiration at now + 1 sec
-        result = add.apply_async((1, 1), expires=datetime.utcnow() + timedelta(seconds=1))
-        with pytest.raises(celery.exceptions.TaskRevokedError):
-            result.get()
-        assert result.status == 'REVOKED'
-        assert result.ready() is True
-        assert result.failed() is False
-        assert result.successful() is False
-
-    @flaky
-    def test_eta(self, manager):
-        """Tests tasks scheduled at some point in future."""
-        start = perf_counter()
-        # Schedule task to be executed in 3 seconds
-        result = add.apply_async((1, 1), countdown=3)
-        sleep(1)
-        assert result.status == 'PENDING'
-        assert result.ready() is False
-        assert result.get() == 2
-        end = perf_counter()
-        assert result.status == 'SUCCESS'
-        assert result.ready() is True
-        # Difference between calling the task and result must be bigger than 3 secs
-        assert (end - start) > 3
-
-        start = perf_counter()
-        # Schedule task to be executed at time now + 3 seconds
-        result = add.apply_async((2, 2), eta=datetime.utcnow() + timedelta(seconds=3))
-        sleep(1)
-        assert result.status == 'PENDING'
-        assert result.ready() is False
-        assert result.get() == 4
-        end = perf_counter()
-        assert result.status == 'SUCCESS'
-        assert result.ready() is True
-        # Difference between calling the task and result must be bigger than 3 secs
-        assert (end - start) > 3
-
-    @flaky
-    def test_fail(self, manager):
-        """Tests that the failing task propagates back correct exception."""
-        result = fail.delay()
-        with pytest.raises(ExpectedException):
-            result.get(timeout=5)
-        assert result.status == 'FAILURE'
-        assert result.ready() is True
-        assert result.failed() is True
-        assert result.successful() is False
-
-    @flaky
-    def test_wrong_arguments(self, manager):
-        """Tests that proper exceptions are raised when task is called with wrong arguments."""
-        with pytest.raises(TypeError):
-            add(5)
-
-        with pytest.raises(TypeError):
-            add(5, 5, wrong_arg=5)
-
-        with pytest.raises(TypeError):
-            add.delay(5)
-
-        with pytest.raises(TypeError):
-            add.delay(5, wrong_arg=5)
-
-        # Tasks with typing=False are not checked but execution should fail
-        result = add_not_typed.delay(5)
-        with pytest.raises(TypeError):
-            result.get(timeout=5)
-        assert result.status == 'FAILURE'
-
-        result = add_not_typed.delay(5, wrong_arg=5)
-        with pytest.raises(TypeError):
-            result.get(timeout=5)
-        assert result.status == 'FAILURE'
-
-    @flaky
-    def test_retry(self, manager):
-        """Tests retrying of task."""
-        # Tests when max. retries is reached
-        result = retry.delay()
-        for _ in range(5):
-            status = result.status
-            if status != 'PENDING':
-                break
-            sleep(1)
-        assert status == 'RETRY'
-        with pytest.raises(ExpectedException):
-            result.get()
-        assert result.status == 'FAILURE'
-
-        # Tests when task is retried but after returns correct result
-        result = retry.delay(return_value='bar')
-        for _ in range(5):
-            status = result.status
-            if status != 'PENDING':
-                break
-            sleep(1)
-        assert status == 'RETRY'
-        assert result.get() == 'bar'
-        assert result.status == 'SUCCESS'
-
-    @flaky
-    def test_task_accepted(self, manager, sleep=1):
-        r1 = sleeping.delay(sleep)
-        sleeping.delay(sleep)
-        manager.assert_accepted([r1.id])
-
-    @flaky
-    def test_task_retried(self):
-        res = retry_once.delay()
-        assert res.get(timeout=TIMEOUT) == 1  # retried once
-
-    @flaky
-    def test_task_retried_priority(self):
-        res = retry_once_priority.apply_async(priority=7)
-        assert res.get(timeout=TIMEOUT) == 7  # retried once with priority 7
-
-    @flaky
-    def test_unicode_task(self, manager):
-        manager.join(
-            group(print_unicode.s() for _ in range(5))(),
-            timeout=TIMEOUT, propagate=True,
-        )
-
-
-class test_task_redis_result_backend:
-    @pytest.fixture(autouse=True)
-    def setup(self, redis_server, manager):
-        if not manager.app.conf.result_backend.startswith('redis'):
-            raise pytest.skip('Requires redis result backend.')
-        redis_server.restart()
-        sleep(1)
-
-    def test_ignoring_result_no_subscriptions(self):
-        assert get_active_redis_channels() == []
-        result = add_ignore_result.delay(1, 2)
-        assert result.ignored is True
-        assert get_active_redis_channels() == []
-
-    def test_asyncresult_forget_cancels_subscription(self):
-        result = add.delay(1, 2)
-        assert get_active_redis_channels(as_string=True) == [
-            f"celery-task-meta-{result.id}"
-        ]
-        result.forget()
-        assert get_active_redis_channels() == []
-
-    def test_asyncresult_get_cancels_subscription(self):
-        result = add.delay(1, 2)
-        assert get_active_redis_channels(as_string=True) == [
-            f"celery-task-meta-{result.id}"
-        ]
-        assert result.get(timeout=3) == 3
-        assert get_active_redis_channels() == []
+from datetime import datetime, timedelta
+from time import perf_counter, sleep
+
+import pytest
+
+import celery
+from celery import group
+
+from .conftest import get_active_redis_channels
+from .tasks import (ClassBasedAutoRetryTask, ExpectedException, add,
+                    add_ignore_result, add_not_typed, fail, print_unicode,
+                    retry, retry_once, retry_once_priority, sleeping)
+
+TIMEOUT = 10
+
+
+_flaky = pytest.mark.flaky(reruns=5, reruns_delay=2)
+_timeout = pytest.mark.timeout(timeout=300)
+
+
+def flaky(fn):
+    return _timeout(_flaky(fn))
+
+
+class test_class_based_tasks:
+
+    @flaky
+    def test_class_based_task_retried(self, celery_session_app,
+                                      celery_session_worker):
+        task = ClassBasedAutoRetryTask()
+        celery_session_app.tasks.register(task)
+        res = task.delay()
+        assert res.get(timeout=TIMEOUT) == 1
+
+
+def _producer(j):
+    """Single producer helper function"""
+    results = []
+    for i in range(20):
+        results.append([i + j, add.delay(i, j)])
+    for expected, result in results:
+        value = result.get(timeout=10)
+        assert value == expected
+        assert result.status == 'SUCCESS'
+        assert result.ready() is True
+        assert result.successful() is True
+    return j
+
+
+class test_tasks:
+
+    def test_simple_call(self):
+        """Tests direct simple call of task"""
+        assert add(1, 1) == 2
+        assert add(1, 1, z=1) == 3
+
+    @flaky
+    def test_basic_task(self, manager):
+        """Tests basic task call"""
+        results = []
+        # Tests calling task only with args
+        for i in range(10):
+            results.append([i + i, add.delay(i, i)])
+        for expected, result in results:
+            value = result.get(timeout=10)
+            assert value == expected
+            assert result.status == 'SUCCESS'
+            assert result.ready() is True
+            assert result.successful() is True
+
+        results = []
+        # Tests calling task with args and kwargs
+        for i in range(10):
+            results.append([3*i, add.delay(i, i, z=i)])
+        for expected, result in results:
+            value = result.get(timeout=10)
+            assert value == expected
+            assert result.status == 'SUCCESS'
+            assert result.ready() is True
+            assert result.successful() is True
+
+    @flaky
+    def test_multiprocess_producer(self, manager):
+        """Testing multiple processes calling tasks."""
+        from multiprocessing import Pool
+        pool = Pool(20)
+        ret = pool.map(_producer, range(120))
+        assert list(ret) == list(range(120))
+
+    @flaky
+    def test_multithread_producer(self, manager):
+        """Testing multiple threads calling tasks."""
+        from multiprocessing.pool import ThreadPool
+        pool = ThreadPool(20)
+        ret = pool.map(_producer, range(120))
+        assert list(ret) == list(range(120))
+
+    @flaky
+    def test_ignore_result(self, manager):
+        """Testing calling task with ignoring results."""
+        result = add.apply_async((1, 2), ignore_result=True)
+        assert result.get() is None
+
+    @flaky
+    def test_timeout(self, manager):
+        """Testing timeout of getting results from tasks."""
+        result = sleeping.delay(10)
+        with pytest.raises(celery.exceptions.TimeoutError):
+            result.get(timeout=5)
+
+    @flaky
+    def test_expired(self, manager):
+        """Testing expiration of task."""
+        # Fill the queue with tasks which took > 1 sec to process
+        for _ in range(4):
+            sleeping.delay(2)
+        # Execute task with expiration = 1 sec
+        result = add.apply_async((1, 1), expires=1)
+        with pytest.raises(celery.exceptions.TaskRevokedError):
+            result.get()
+        assert result.status == 'REVOKED'
+        assert result.ready() is True
+        assert result.failed() is False
+        assert result.successful() is False
+
+        # Fill the queue with tasks which took > 1 sec to process
+        for _ in range(4):
+            sleeping.delay(2)
+        # Execute task with expiration at now + 1 sec
+        result = add.apply_async((1, 1), expires=datetime.utcnow() + timedelta(seconds=1))
+        with pytest.raises(celery.exceptions.TaskRevokedError):
+            result.get()
+        assert result.status == 'REVOKED'
+        assert result.ready() is True
+        assert result.failed() is False
+        assert result.successful() is False
+
+    @flaky
+    def test_eta(self, manager):
+        """Tests tasks scheduled at some point in future."""
+        start = perf_counter()
+        # Schedule task to be executed in 3 seconds
+        result = add.apply_async((1, 1), countdown=3)
+        sleep(1)
+        assert result.status == 'PENDING'
+        assert result.ready() is False
+        assert result.get() == 2
+        end = perf_counter()
+        assert result.status == 'SUCCESS'
+        assert result.ready() is True
+        # Difference between calling the task and result must be bigger than 3 secs
+        assert (end - start) > 3
+
+        start = perf_counter()
+        # Schedule task to be executed at time now + 3 seconds
+        result = add.apply_async((2, 2), eta=datetime.utcnow() + timedelta(seconds=3))
+        sleep(1)
+        assert result.status == 'PENDING'
+        assert result.ready() is False
+        assert result.get() == 4
+        end = perf_counter()
+        assert result.status == 'SUCCESS'
+        assert result.ready() is True
+        # Difference between calling the task and result must be bigger than 3 secs
+        assert (end - start) > 3
+
+    @flaky
+    def test_fail(self, manager):
+        """Tests that the failing task propagates back correct exception."""
+        result = fail.delay()
+        with pytest.raises(ExpectedException):
+            result.get(timeout=5)
+        assert result.status == 'FAILURE'
+        assert result.ready() is True
+        assert result.failed() is True
+        assert result.successful() is False
+
+    @flaky
+    def test_wrong_arguments(self, manager):
+        """Tests that proper exceptions are raised when task is called with wrong arguments."""
+        with pytest.raises(TypeError):
+            add(5)
+
+        with pytest.raises(TypeError):
+            add(5, 5, wrong_arg=5)
+
+        with pytest.raises(TypeError):
+            add.delay(5)
+
+        with pytest.raises(TypeError):
+            add.delay(5, wrong_arg=5)
+
+        # Tasks with typing=False are not checked but execution should fail
+        result = add_not_typed.delay(5)
+        with pytest.raises(TypeError):
+            result.get(timeout=5)
+        assert result.status == 'FAILURE'
+
+        result = add_not_typed.delay(5, wrong_arg=5)
+        with pytest.raises(TypeError):
+            result.get(timeout=5)
+        assert result.status == 'FAILURE'
+
+    @flaky
+    def test_retry(self, manager):
+        """Tests retrying of task."""
+        # Tests when max. retries is reached
+        result = retry.delay()
+        for _ in range(5):
+            status = result.status
+            if status != 'PENDING':
+                break
+            sleep(1)
+        assert status == 'RETRY'
+        with pytest.raises(ExpectedException):
+            result.get()
+        assert result.status == 'FAILURE'
+
+        # Tests when task is retried but after returns correct result
+        result = retry.delay(return_value='bar')
+        for _ in range(5):
+            status = result.status
+            if status != 'PENDING':
+                break
+            sleep(1)
+        assert status == 'RETRY'
+        assert result.get() == 'bar'
+        assert result.status == 'SUCCESS'
+
+    @flaky
+    def test_task_accepted(self, manager, sleep=1):
+        r1 = sleeping.delay(sleep)
+        sleeping.delay(sleep)
+        manager.assert_accepted([r1.id])
+
+    @flaky
+    def test_task_retried(self):
+        res = retry_once.delay()
+        assert res.get(timeout=TIMEOUT) == 1  # retried once
+
+    @flaky
+    def test_task_retried_priority(self):
+        res = retry_once_priority.apply_async(priority=7)
+        assert res.get(timeout=TIMEOUT) == 7  # retried once with priority 7
+
+    @flaky
+    def test_unicode_task(self, manager):
+        manager.join(
+            group(print_unicode.s() for _ in range(5))(),
+            timeout=TIMEOUT, propagate=True,
+        )
+
+
+class test_task_redis_result_backend:
+    @pytest.fixture(autouse=True)
+    def setup(self, redis_server, manager):
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+        redis_server.restart()
+        sleep(1)
+
+    def test_ignoring_result_no_subscriptions(self):
+        assert get_active_redis_channels() == []
+        result = add_ignore_result.delay(1, 2)
+        assert result.ignored is True
+        assert get_active_redis_channels() == []
+
+    def test_asyncresult_forget_cancels_subscription(self):
+        result = add.delay(1, 2)
+        assert get_active_redis_channels(as_string=True) == [
+            f"celery-task-meta-{result.id}"
+        ]
+        result.forget()
+        assert get_active_redis_channels() == []
+
+    def test_asyncresult_get_cancels_subscription(self):
+        result = add.delay(1, 2)
+        assert get_active_redis_channels(as_string=True) == [
+            f"celery-task-meta-{result.id}"
+        ]
+        assert result.get(timeout=3) == 3
+        assert get_active_redis_channels() == []
```

### Comparing `deepfos-celery-1.0.2/t/integration/test_tmp2.py` & `deepfos-celery-1.0.3/t/integration/test_tmp2.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/aio/test_aio_control.py` & `deepfos-celery-1.0.3/t/unit/app/test_control.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-from unittest.mock import Mock, AsyncMock
+from unittest.mock import Mock
 
 import pytest
 
 from celery import uuid
-from celery.aio import control as aio_control
 from celery.app import control
 from celery.exceptions import DuplicateNodenameWarning
 from celery.utils.collections import LimitedSet
 
-from t.base import AsyncTest
-
 
 def _info_for_commandclass(type_):
     from celery.worker.control import Panel
     return [
         (name, info)
         for name, info in Panel.meta.items()
         if info.type == type_
     ]
 
 
 def test_client_implements_all_commands(app):
     commands = _info_for_commandclass('control')
     assert commands
     for name, info in commands:
-        assert getattr(app.aio_control, name)
+        assert getattr(app.control, name)
 
 
 def test_inspect_implements_all_commands(app):
-    inspect = app.aio_control.inspect()
+    inspect = app.control.inspect()
     commands = _info_for_commandclass('inspect')
     assert commands
     for name, info in commands:
         if info.type == 'inspect':
             assert getattr(inspect, name)
 
 
@@ -49,381 +46,380 @@
 
         assert 'Received multiple replies from node name: {}.'.format(
             next(iter(reply[0]))) in str(w[0].message.args[0])
         assert 'foo@example.com' in nodes
         assert 'bar@example.com' in nodes
 
 
-class test_inspect(AsyncTest):
+class test_inspect:
 
     def setup(self):
-        self.app.aio_control.broadcast = AsyncMock(name='broadcast')
-        self.app.aio_control.broadcast.return_value = {}
-        self.inspect = self.app.aio_control.inspect()
+        self.app.control.broadcast = Mock(name='broadcast')
+        self.app.control.broadcast.return_value = {}
+        self.inspect = self.app.control.inspect()
 
     def test_prepare_reply(self):
         reply = self.inspect._prepare([
             {'w1': {'ok': 1}},
             {'w2': {'ok': 1}},
         ])
         assert reply == {
             'w1': {'ok': 1},
             'w2': {'ok': 1},
         }
 
-        i = self.app.aio_control.inspect(destination='w1')
+        i = self.app.control.inspect(destination='w1')
         assert i._prepare([{'w1': {'ok': 1}}]) == {'ok': 1}
 
     def assert_broadcast_called(self, command,
                                 destination=None,
                                 callback=None,
                                 connection=None,
                                 limit=None,
                                 timeout=None,
                                 reply=True,
                                 pattern=None,
                                 matcher=None,
                                 **arguments):
-        self.app.aio_control.broadcast.assert_called_with(
+        self.app.control.broadcast.assert_called_with(
             command,
             arguments=arguments,
             destination=destination or self.inspect.destination,
             pattern=pattern or self.inspect.pattern,
             matcher=matcher or self.inspect.destination,
             callback=callback or self.inspect.callback,
             connection=connection or self.inspect.connection,
             limit=limit if limit is not None else self.inspect.limit,
             timeout=timeout if timeout is not None else self.inspect.timeout,
             reply=reply,
         )
 
-    async def test_active(self):
-        await self.inspect.active()
+    def test_active(self):
+        self.inspect.active()
         self.assert_broadcast_called('active')
 
-    async def test_clock(self):
-        await self.inspect.clock()
+    def test_clock(self):
+        self.inspect.clock()
         self.assert_broadcast_called('clock')
 
-    async def test_conf(self):
-        await self.inspect.conf()
+    def test_conf(self):
+        self.inspect.conf()
         self.assert_broadcast_called('conf', with_defaults=False)
 
-    async def test_conf__with_defaults(self):
-        await self.inspect.conf(with_defaults=True)
+    def test_conf__with_defaults(self):
+        self.inspect.conf(with_defaults=True)
         self.assert_broadcast_called('conf', with_defaults=True)
 
-    async def test_hello(self):
-        await self.inspect.hello('george@vandelay.com')
+    def test_hello(self):
+        self.inspect.hello('george@vandelay.com')
         self.assert_broadcast_called(
             'hello', from_node='george@vandelay.com', revoked=None)
 
-    async def test_hello__with_revoked(self):
+    def test_hello__with_revoked(self):
         revoked = LimitedSet(100)
         for i in range(100):
             revoked.add(f'id{i}')
-        await self.inspect.hello('george@vandelay.com', revoked=revoked._data)
+        self.inspect.hello('george@vandelay.com', revoked=revoked._data)
         self.assert_broadcast_called(
             'hello', from_node='george@vandelay.com', revoked=revoked._data)
 
-    async def test_memsample(self):
-        await self.inspect.memsample()
+    def test_memsample(self):
+        self.inspect.memsample()
         self.assert_broadcast_called('memsample')
 
-    async def test_memdump(self):
-        await self.inspect.memdump()
+    def test_memdump(self):
+        self.inspect.memdump()
         self.assert_broadcast_called('memdump', samples=10)
 
-    async def test_memdump__samples_specified(self):
-        await self.inspect.memdump(samples=303)
+    def test_memdump__samples_specified(self):
+        self.inspect.memdump(samples=303)
         self.assert_broadcast_called('memdump', samples=303)
 
-    async def test_objgraph(self):
-        await self.inspect.objgraph()
+    def test_objgraph(self):
+        self.inspect.objgraph()
         self.assert_broadcast_called(
             'objgraph', num=200, type='Request', max_depth=10)
 
-    async def test_scheduled(self):
-        await self.inspect.scheduled()
+    def test_scheduled(self):
+        self.inspect.scheduled()
         self.assert_broadcast_called('scheduled')
 
-    async def test_reserved(self):
-        await self.inspect.reserved()
+    def test_reserved(self):
+        self.inspect.reserved()
         self.assert_broadcast_called('reserved')
 
-    async def test_stats(self):
-        await self.inspect.stats()
+    def test_stats(self):
+        self.inspect.stats()
         self.assert_broadcast_called('stats')
 
-    async def test_revoked(self):
-        await self.inspect.revoked()
+    def test_revoked(self):
+        self.inspect.revoked()
         self.assert_broadcast_called('revoked')
 
-    async def test_registered(self):
-        await self.inspect.registered()
+    def test_registered(self):
+        self.inspect.registered()
         self.assert_broadcast_called('registered', taskinfoitems=())
 
-    async def test_registered__taskinfoitems(self):
-        await self.inspect.registered('rate_limit', 'time_limit')
+    def test_registered__taskinfoitems(self):
+        self.inspect.registered('rate_limit', 'time_limit')
         self.assert_broadcast_called(
             'registered',
             taskinfoitems=('rate_limit', 'time_limit'),
         )
 
-    async def test_ping(self):
-        await self.inspect.ping()
+    def test_ping(self):
+        self.inspect.ping()
         self.assert_broadcast_called('ping')
 
-    async def test_ping_matcher_pattern(self):
+    def test_ping_matcher_pattern(self):
         orig_inspect = self.inspect
-        self.inspect = self.app.aio_control.inspect(pattern=".*", matcher="pcre")
-        await self.inspect.ping()
+        self.inspect = self.app.control.inspect(pattern=".*", matcher="pcre")
+        self.inspect.ping()
         try:
             self.assert_broadcast_called('ping', pattern=".*", matcher="pcre")
         except AssertionError as e:
             self.inspect = orig_inspect
             raise e
 
-    async def test_active_queues(self):
-        await self.inspect.active_queues()
+    def test_active_queues(self):
+        self.inspect.active_queues()
         self.assert_broadcast_called('active_queues')
 
-    async def test_query_task(self):
-        await self.inspect.query_task('foo', 'bar')
+    def test_query_task(self):
+        self.inspect.query_task('foo', 'bar')
         self.assert_broadcast_called('query_task', ids=('foo', 'bar'))
 
-    async def test_query_task__compat_single_list_argument(self):
-        await self.inspect.query_task(['foo', 'bar'])
+    def test_query_task__compat_single_list_argument(self):
+        self.inspect.query_task(['foo', 'bar'])
         self.assert_broadcast_called('query_task', ids=['foo', 'bar'])
 
-    async def test_query_task__scalar(self):
-        await self.inspect.query_task('foo')
+    def test_query_task__scalar(self):
+        self.inspect.query_task('foo')
         self.assert_broadcast_called('query_task', ids=('foo',))
 
-    async def test_report(self):
-        await self.inspect.report()
+    def test_report(self):
+        self.inspect.report()
         self.assert_broadcast_called('report')
 
 
-class test_Control_broadcast(AsyncTest):
+class test_Control_broadcast:
 
     def setup(self):
-        self.app.aio_control.mailbox = Mock(
-            name='mailbox', return_value=AsyncMock())
+        self.app.control.mailbox = Mock(name='mailbox')
 
-    async def test_broadcast(self):
-        await self.app.aio_control.broadcast('foobarbaz', arguments={'foo': 2})
-        self.app.aio_control.mailbox.assert_called()
-        self.app.aio_control.mailbox()._broadcast.assert_called_with(
+    def test_broadcast(self):
+        self.app.control.broadcast('foobarbaz', arguments={'foo': 2})
+        self.app.control.mailbox.assert_called()
+        self.app.control.mailbox()._broadcast.assert_called_with(
             'foobarbaz', {'foo': 2}, None, False, 1.0, None, None,
             channel=None,
         )
 
-    async def test_broadcast_limit(self):
-        await self.app.aio_control.broadcast(
+    def test_broadcast_limit(self):
+        self.app.control.broadcast(
             'foobarbaz1', arguments=None, limit=None, destination=[1, 2, 3],
         )
-        self.app.aio_control.mailbox.assert_called()
-        self.app.aio_control.mailbox()._broadcast.assert_called_with(
+        self.app.control.mailbox.assert_called()
+        self.app.control.mailbox()._broadcast.assert_called_with(
             'foobarbaz1', {}, [1, 2, 3], False, 1.0, None, None,
             channel=None,
         )
 
 
-class test_Control(AsyncTest):
+class test_Control:
 
     def setup(self):
-        self.app.aio_control.broadcast = AsyncMock(name='broadcast')
-        self.app.aio_control.broadcast.return_value = {}
+        self.app.control.broadcast = Mock(name='broadcast')
+        self.app.control.broadcast.return_value = {}
 
-        @self.app.task(shared=False, aio_variant=True)
+        @self.app.task(shared=False)
         def mytask():
             pass
         self.mytask = mytask
 
     def assert_control_called_with_args(self, name, destination=None,
                                         _options=None, **args):
-        self.app.aio_control.broadcast.assert_called_with(
+        self.app.control.broadcast.assert_called_with(
             name, destination=destination, arguments=args, **_options or {})
 
-    async def zzz_test_purge(self):
+    def test_purge(self):
         self.app.amqp.TaskConsumer = Mock(name='TaskConsumer')
-        await self.app.aio_control.purge()
+        self.app.control.purge()
         self.app.amqp.TaskConsumer().purge.assert_called_with()
 
-    async def test_rate_limit(self):
-        await self.app.aio_control.rate_limit(self.mytask.name, '100/m')
+    def test_rate_limit(self):
+        self.app.control.rate_limit(self.mytask.name, '100/m')
         self.assert_control_called_with_args(
             'rate_limit',
             destination=None,
             task_name=self.mytask.name,
             rate_limit='100/m',
         )
 
-    async def test_rate_limit__with_destination(self):
-        await self.app.aio_control.rate_limit(
+    def test_rate_limit__with_destination(self):
+        self.app.control.rate_limit(
             self.mytask.name, '100/m', 'a@w.com', limit=100)
         self.assert_control_called_with_args(
             'rate_limit',
             destination='a@w.com',
             task_name=self.mytask.name,
             rate_limit='100/m',
             _options={'limit': 100},
         )
 
-    async def test_time_limit(self):
-        await self.app.aio_control.time_limit(self.mytask.name, soft=10, hard=20)
+    def test_time_limit(self):
+        self.app.control.time_limit(self.mytask.name, soft=10, hard=20)
         self.assert_control_called_with_args(
             'time_limit',
             destination=None,
             task_name=self.mytask.name,
             soft=10,
             hard=20,
         )
 
-    async def test_time_limit__with_destination(self):
-        await self.app.aio_control.time_limit(
+    def test_time_limit__with_destination(self):
+        self.app.control.time_limit(
             self.mytask.name, soft=10, hard=20,
             destination='a@q.com', limit=99,
         )
         self.assert_control_called_with_args(
             'time_limit',
             destination='a@q.com',
             task_name=self.mytask.name,
             soft=10,
             hard=20,
             _options={'limit': 99},
         )
 
-    async def test_add_consumer(self):
-        await self.app.aio_control.add_consumer('foo')
+    def test_add_consumer(self):
+        self.app.control.add_consumer('foo')
         self.assert_control_called_with_args(
             'add_consumer',
             destination=None,
             queue='foo',
             exchange=None,
             exchange_type='direct',
             routing_key=None,
         )
 
-    async def test_add_consumer__with_options_and_dest(self):
-        await self.app.aio_control.add_consumer(
+    def test_add_consumer__with_options_and_dest(self):
+        self.app.control.add_consumer(
             'foo', 'ex', 'topic', 'rkey', destination='a@q.com', limit=78)
         self.assert_control_called_with_args(
             'add_consumer',
             destination='a@q.com',
             queue='foo',
             exchange='ex',
             exchange_type='topic',
             routing_key='rkey',
             _options={'limit': 78},
         )
 
-    async def test_cancel_consumer(self):
-        await self.app.aio_control.cancel_consumer('foo')
+    def test_cancel_consumer(self):
+        self.app.control.cancel_consumer('foo')
         self.assert_control_called_with_args(
             'cancel_consumer',
             destination=None,
             queue='foo',
         )
 
-    async def test_cancel_consumer__with_destination(self):
-        self.app.aio_control.cancel_consumer(
+    def test_cancel_consumer__with_destination(self):
+        self.app.control.cancel_consumer(
             'foo', destination='w1@q.com', limit=3)
         self.assert_control_called_with_args(
             'cancel_consumer',
             destination='w1@q.com',
             queue='foo',
             _options={'limit': 3},
         )
 
-    async def test_shutdown(self):
-        await self.app.aio_control.shutdown()
+    def test_shutdown(self):
+        self.app.control.shutdown()
         self.assert_control_called_with_args('shutdown', destination=None)
 
-    async def test_shutdown__with_destination(self):
-        await self.app.aio_control.shutdown(destination='a@q.com', limit=3)
+    def test_shutdown__with_destination(self):
+        self.app.control.shutdown(destination='a@q.com', limit=3)
         self.assert_control_called_with_args(
             'shutdown', destination='a@q.com', _options={'limit': 3})
 
-    async def test_heartbeat(self):
-        await self.app.aio_control.heartbeat()
+    def test_heartbeat(self):
+        self.app.control.heartbeat()
         self.assert_control_called_with_args('heartbeat', destination=None)
 
-    async def test_heartbeat__with_destination(self):
-        await self.app.aio_control.heartbeat(destination='a@q.com', limit=3)
+    def test_heartbeat__with_destination(self):
+        self.app.control.heartbeat(destination='a@q.com', limit=3)
         self.assert_control_called_with_args(
             'heartbeat', destination='a@q.com', _options={'limit': 3})
 
-    async def test_pool_restart(self):
-        await self.app.aio_control.pool_restart()
+    def test_pool_restart(self):
+        self.app.control.pool_restart()
         self.assert_control_called_with_args(
             'pool_restart',
             destination=None,
             modules=None,
             reload=False,
             reloader=None)
 
-    async def test_terminate(self):
-        self.app.aio_control.revoke = AsyncMock(name='revoke')
-        await self.app.aio_control.terminate('124')
-        self.app.aio_control.revoke.assert_called_with(
+    def test_terminate(self):
+        self.app.control.revoke = Mock(name='revoke')
+        self.app.control.terminate('124')
+        self.app.control.revoke.assert_called_with(
             '124', destination=None,
             terminate=True,
             signal=control.TERM_SIGNAME,
         )
 
-    async def test_enable_events(self):
-        await self.app.aio_control.enable_events()
+    def test_enable_events(self):
+        self.app.control.enable_events()
         self.assert_control_called_with_args('enable_events', destination=None)
 
-    async def test_enable_events_with_destination(self):
-        await self.app.aio_control.enable_events(destination='a@q.com', limit=3)
+    def test_enable_events_with_destination(self):
+        self.app.control.enable_events(destination='a@q.com', limit=3)
         self.assert_control_called_with_args(
             'enable_events', destination='a@q.com', _options={'limit': 3})
 
-    async def test_disable_events(self):
-        await self.app.aio_control.disable_events()
+    def test_disable_events(self):
+        self.app.control.disable_events()
         self.assert_control_called_with_args(
             'disable_events', destination=None)
 
-    async def test_disable_events_with_destination(self):
-        await self.app.aio_control.disable_events(destination='a@q.com', limit=3)
+    def test_disable_events_with_destination(self):
+        self.app.control.disable_events(destination='a@q.com', limit=3)
         self.assert_control_called_with_args(
             'disable_events', destination='a@q.com', _options={'limit': 3})
 
-    async def test_ping(self):
-        await self.app.aio_control.ping()
+    def test_ping(self):
+        self.app.control.ping()
         self.assert_control_called_with_args(
             'ping', destination=None,
             _options={'timeout': 1.0, 'reply': True})
 
-    async def test_ping_with_destination(self):
-        await self.app.aio_control.ping(destination='a@q.com', limit=3)
+    def test_ping_with_destination(self):
+        self.app.control.ping(destination='a@q.com', limit=3)
         self.assert_control_called_with_args(
             'ping',
             destination='a@q.com',
             _options={
                 'limit': 3,
                 'timeout': 1.0,
                 'reply': True,
             })
 
-    async def test_revoke(self):
-        await self.app.aio_control.revoke('foozbaaz')
+    def test_revoke(self):
+        self.app.control.revoke('foozbaaz')
         self.assert_control_called_with_args(
             'revoke',
             destination=None,
             task_id='foozbaaz',
             signal=control.TERM_SIGNAME,
             terminate=False,
         )
 
-    async def test_revoke__with_options(self):
-        await self.app.aio_control.revoke(
+    def test_revoke__with_options(self):
+        self.app.control.revoke(
             'foozbaaz',
             destination='a@q.com',
             terminate=True,
             signal='KILL',
             limit=404,
         )
         self.assert_control_called_with_args(
@@ -431,95 +427,95 @@
             destination='a@q.com',
             task_id='foozbaaz',
             signal='KILL',
             terminate=True,
             _options={'limit': 404},
         )
 
-    async def test_election(self):
-        await self.app.aio_control.election('some_id', 'topic', 'action')
+    def test_election(self):
+        self.app.control.election('some_id', 'topic', 'action')
         self.assert_control_called_with_args(
             'election',
             destination=None,
             topic='topic',
             action='action',
             id='some_id',
             _options={'connection': None},
         )
 
-    async def test_autoscale(self):
-        await self.app.aio_control.autoscale(300, 10)
+    def test_autoscale(self):
+        self.app.control.autoscale(300, 10)
         self.assert_control_called_with_args(
             'autoscale', max=300, min=10, destination=None)
 
-    async def test_autoscale__with_options(self):
-        await self.app.aio_control.autoscale(300, 10, destination='a@q.com', limit=39)
+    def test_autoscale__with_options(self):
+        self.app.control.autoscale(300, 10, destination='a@q.com', limit=39)
         self.assert_control_called_with_args(
             'autoscale', max=300, min=10,
             destination='a@q.com',
             _options={'limit': 39}
         )
 
-    async def test_pool_grow(self):
-        await self.app.aio_control.pool_grow(2)
+    def test_pool_grow(self):
+        self.app.control.pool_grow(2)
         self.assert_control_called_with_args(
             'pool_grow', n=2, destination=None)
 
-    async def test_pool_grow__with_options(self):
-        await self.app.aio_control.pool_grow(2, destination='a@q.com', limit=39)
+    def test_pool_grow__with_options(self):
+        self.app.control.pool_grow(2, destination='a@q.com', limit=39)
         self.assert_control_called_with_args(
             'pool_grow', n=2,
             destination='a@q.com',
             _options={'limit': 39}
         )
 
-    async def test_pool_shrink(self):
-        await self.app.aio_control.pool_shrink(2)
+    def test_pool_shrink(self):
+        self.app.control.pool_shrink(2)
         self.assert_control_called_with_args(
             'pool_shrink', n=2, destination=None)
 
-    async def test_pool_shrink__with_options(self):
-        await self.app.aio_control.pool_shrink(2, destination='a@q.com', limit=39)
+    def test_pool_shrink__with_options(self):
+        self.app.control.pool_shrink(2, destination='a@q.com', limit=39)
         self.assert_control_called_with_args(
             'pool_shrink', n=2,
             destination='a@q.com',
             _options={'limit': 39}
         )
 
-    async def test_revoke_from_result(self):
-        self.app.aio_control.revoke = AsyncMock(name='revoke')
-        await self.app.AioAsyncResult('foozbazzbar').revoke()
-        self.app.aio_control.revoke.assert_called_with(
+    def test_revoke_from_result(self):
+        self.app.control.revoke = Mock(name='revoke')
+        self.app.AsyncResult('foozbazzbar').revoke()
+        self.app.control.revoke.assert_called_with(
             'foozbazzbar',
             connection=None, reply=False, signal=None,
             terminate=False, timeout=None)
 
-    async def test_revoke_from_resultset(self):
-        self.app.aio_control.revoke = AsyncMock(name='revoke')
+    def test_revoke_from_resultset(self):
+        self.app.control.revoke = Mock(name='revoke')
         uuids = [uuid() for _ in range(10)]
-        r = self.app.AioGroupResult(
-            uuid(), [self.app.AioAsyncResult(x) for x in uuids])
-        await r.revoke()
-        self.app.aio_control.revoke.assert_called_with(
+        r = self.app.GroupResult(
+            uuid(), [self.app.AsyncResult(x) for x in uuids])
+        r.revoke()
+        self.app.control.revoke.assert_called_with(
             uuids,
             connection=None, reply=False, signal=None,
             terminate=False, timeout=None)
 
     def test_after_fork_clears_mailbox_pool(self):
         amqp = Mock(name='amqp')
-        self.app.aio_amqp = amqp
+        self.app.amqp = amqp
         closed_pool = Mock(name='closed pool')
         amqp.producer_pool = closed_pool
-        assert closed_pool is self.app.aio_control.mailbox.producer_pool
-        self.app.aio_control._after_fork()
+        assert closed_pool is self.app.control.mailbox.producer_pool
+        self.app.control._after_fork()
         new_pool = Mock(name='new pool')
         amqp.producer_pool = new_pool
-        assert new_pool is self.app.aio_control.mailbox.producer_pool
+        assert new_pool is self.app.control.mailbox.producer_pool
 
     def test_control_exchange__default(self):
-        c = aio_control.Control(self.app)
+        c = control.Control(self.app)
         assert c.mailbox.namespace == 'celery'
 
     def test_control_exchange__setting(self):
         self.app.conf.control_exchange = 'test_exchange'
-        c = aio_control.Control(self.app)
+        c = control.Control(self.app)
         assert c.mailbox.namespace == 'test_exchange'
```

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_amqp.py` & `deepfos-celery-1.0.3/t/unit/app/test_amqp.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_annotations.py` & `deepfos-celery-1.0.3/t/unit/app/test_annotations.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_app.py` & `deepfos-celery-1.0.3/t/unit/app/test_app.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_backends.py` & `deepfos-celery-1.0.3/t/unit/app/test_backends.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_beat.py` & `deepfos-celery-1.0.3/t/unit/app/test_beat.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_builtins.py` & `deepfos-celery-1.0.3/t/unit/app/test_builtins.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_control.py` & `deepfos-celery-1.0.3/t/unit/aio/test_aio_control.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,521 +1,525 @@
-from unittest.mock import Mock
-
-import pytest
-
-from celery import uuid
-from celery.app import control
-from celery.exceptions import DuplicateNodenameWarning
-from celery.utils.collections import LimitedSet
-
-
-def _info_for_commandclass(type_):
-    from celery.worker.control import Panel
-    return [
-        (name, info)
-        for name, info in Panel.meta.items()
-        if info.type == type_
-    ]
-
-
-def test_client_implements_all_commands(app):
-    commands = _info_for_commandclass('control')
-    assert commands
-    for name, info in commands:
-        assert getattr(app.control, name)
-
-
-def test_inspect_implements_all_commands(app):
-    inspect = app.control.inspect()
-    commands = _info_for_commandclass('inspect')
-    assert commands
-    for name, info in commands:
-        if info.type == 'inspect':
-            assert getattr(inspect, name)
-
-
-class test_flatten_reply:
-
-    def test_flatten_reply(self):
-        reply = [
-            {'foo@example.com': {'hello': 10}},
-            {'foo@example.com': {'hello': 20}},
-            {'bar@example.com': {'hello': 30}}
-        ]
-        with pytest.warns(DuplicateNodenameWarning) as w:
-            nodes = control.flatten_reply(reply)
-
-        assert 'Received multiple replies from node name: {}.'.format(
-            next(iter(reply[0]))) in str(w[0].message.args[0])
-        assert 'foo@example.com' in nodes
-        assert 'bar@example.com' in nodes
-
-
-class test_inspect:
-
-    def setup(self):
-        self.app.control.broadcast = Mock(name='broadcast')
-        self.app.control.broadcast.return_value = {}
-        self.inspect = self.app.control.inspect()
-
-    def test_prepare_reply(self):
-        reply = self.inspect._prepare([
-            {'w1': {'ok': 1}},
-            {'w2': {'ok': 1}},
-        ])
-        assert reply == {
-            'w1': {'ok': 1},
-            'w2': {'ok': 1},
-        }
-
-        i = self.app.control.inspect(destination='w1')
-        assert i._prepare([{'w1': {'ok': 1}}]) == {'ok': 1}
-
-    def assert_broadcast_called(self, command,
-                                destination=None,
-                                callback=None,
-                                connection=None,
-                                limit=None,
-                                timeout=None,
-                                reply=True,
-                                pattern=None,
-                                matcher=None,
-                                **arguments):
-        self.app.control.broadcast.assert_called_with(
-            command,
-            arguments=arguments,
-            destination=destination or self.inspect.destination,
-            pattern=pattern or self.inspect.pattern,
-            matcher=matcher or self.inspect.destination,
-            callback=callback or self.inspect.callback,
-            connection=connection or self.inspect.connection,
-            limit=limit if limit is not None else self.inspect.limit,
-            timeout=timeout if timeout is not None else self.inspect.timeout,
-            reply=reply,
-        )
-
-    def test_active(self):
-        self.inspect.active()
-        self.assert_broadcast_called('active')
-
-    def test_clock(self):
-        self.inspect.clock()
-        self.assert_broadcast_called('clock')
-
-    def test_conf(self):
-        self.inspect.conf()
-        self.assert_broadcast_called('conf', with_defaults=False)
-
-    def test_conf__with_defaults(self):
-        self.inspect.conf(with_defaults=True)
-        self.assert_broadcast_called('conf', with_defaults=True)
-
-    def test_hello(self):
-        self.inspect.hello('george@vandelay.com')
-        self.assert_broadcast_called(
-            'hello', from_node='george@vandelay.com', revoked=None)
-
-    def test_hello__with_revoked(self):
-        revoked = LimitedSet(100)
-        for i in range(100):
-            revoked.add(f'id{i}')
-        self.inspect.hello('george@vandelay.com', revoked=revoked._data)
-        self.assert_broadcast_called(
-            'hello', from_node='george@vandelay.com', revoked=revoked._data)
-
-    def test_memsample(self):
-        self.inspect.memsample()
-        self.assert_broadcast_called('memsample')
-
-    def test_memdump(self):
-        self.inspect.memdump()
-        self.assert_broadcast_called('memdump', samples=10)
-
-    def test_memdump__samples_specified(self):
-        self.inspect.memdump(samples=303)
-        self.assert_broadcast_called('memdump', samples=303)
-
-    def test_objgraph(self):
-        self.inspect.objgraph()
-        self.assert_broadcast_called(
-            'objgraph', num=200, type='Request', max_depth=10)
-
-    def test_scheduled(self):
-        self.inspect.scheduled()
-        self.assert_broadcast_called('scheduled')
-
-    def test_reserved(self):
-        self.inspect.reserved()
-        self.assert_broadcast_called('reserved')
-
-    def test_stats(self):
-        self.inspect.stats()
-        self.assert_broadcast_called('stats')
-
-    def test_revoked(self):
-        self.inspect.revoked()
-        self.assert_broadcast_called('revoked')
-
-    def test_registered(self):
-        self.inspect.registered()
-        self.assert_broadcast_called('registered', taskinfoitems=())
-
-    def test_registered__taskinfoitems(self):
-        self.inspect.registered('rate_limit', 'time_limit')
-        self.assert_broadcast_called(
-            'registered',
-            taskinfoitems=('rate_limit', 'time_limit'),
-        )
-
-    def test_ping(self):
-        self.inspect.ping()
-        self.assert_broadcast_called('ping')
-
-    def test_ping_matcher_pattern(self):
-        orig_inspect = self.inspect
-        self.inspect = self.app.control.inspect(pattern=".*", matcher="pcre")
-        self.inspect.ping()
-        try:
-            self.assert_broadcast_called('ping', pattern=".*", matcher="pcre")
-        except AssertionError as e:
-            self.inspect = orig_inspect
-            raise e
-
-    def test_active_queues(self):
-        self.inspect.active_queues()
-        self.assert_broadcast_called('active_queues')
-
-    def test_query_task(self):
-        self.inspect.query_task('foo', 'bar')
-        self.assert_broadcast_called('query_task', ids=('foo', 'bar'))
-
-    def test_query_task__compat_single_list_argument(self):
-        self.inspect.query_task(['foo', 'bar'])
-        self.assert_broadcast_called('query_task', ids=['foo', 'bar'])
-
-    def test_query_task__scalar(self):
-        self.inspect.query_task('foo')
-        self.assert_broadcast_called('query_task', ids=('foo',))
-
-    def test_report(self):
-        self.inspect.report()
-        self.assert_broadcast_called('report')
-
-
-class test_Control_broadcast:
-
-    def setup(self):
-        self.app.control.mailbox = Mock(name='mailbox')
-
-    def test_broadcast(self):
-        self.app.control.broadcast('foobarbaz', arguments={'foo': 2})
-        self.app.control.mailbox.assert_called()
-        self.app.control.mailbox()._broadcast.assert_called_with(
-            'foobarbaz', {'foo': 2}, None, False, 1.0, None, None,
-            channel=None,
-        )
-
-    def test_broadcast_limit(self):
-        self.app.control.broadcast(
-            'foobarbaz1', arguments=None, limit=None, destination=[1, 2, 3],
-        )
-        self.app.control.mailbox.assert_called()
-        self.app.control.mailbox()._broadcast.assert_called_with(
-            'foobarbaz1', {}, [1, 2, 3], False, 1.0, None, None,
-            channel=None,
-        )
-
-
-class test_Control:
-
-    def setup(self):
-        self.app.control.broadcast = Mock(name='broadcast')
-        self.app.control.broadcast.return_value = {}
-
-        @self.app.task(shared=False)
-        def mytask():
-            pass
-        self.mytask = mytask
-
-    def assert_control_called_with_args(self, name, destination=None,
-                                        _options=None, **args):
-        self.app.control.broadcast.assert_called_with(
-            name, destination=destination, arguments=args, **_options or {})
-
-    def test_purge(self):
-        self.app.amqp.TaskConsumer = Mock(name='TaskConsumer')
-        self.app.control.purge()
-        self.app.amqp.TaskConsumer().purge.assert_called_with()
-
-    def test_rate_limit(self):
-        self.app.control.rate_limit(self.mytask.name, '100/m')
-        self.assert_control_called_with_args(
-            'rate_limit',
-            destination=None,
-            task_name=self.mytask.name,
-            rate_limit='100/m',
-        )
-
-    def test_rate_limit__with_destination(self):
-        self.app.control.rate_limit(
-            self.mytask.name, '100/m', 'a@w.com', limit=100)
-        self.assert_control_called_with_args(
-            'rate_limit',
-            destination='a@w.com',
-            task_name=self.mytask.name,
-            rate_limit='100/m',
-            _options={'limit': 100},
-        )
-
-    def test_time_limit(self):
-        self.app.control.time_limit(self.mytask.name, soft=10, hard=20)
-        self.assert_control_called_with_args(
-            'time_limit',
-            destination=None,
-            task_name=self.mytask.name,
-            soft=10,
-            hard=20,
-        )
-
-    def test_time_limit__with_destination(self):
-        self.app.control.time_limit(
-            self.mytask.name, soft=10, hard=20,
-            destination='a@q.com', limit=99,
-        )
-        self.assert_control_called_with_args(
-            'time_limit',
-            destination='a@q.com',
-            task_name=self.mytask.name,
-            soft=10,
-            hard=20,
-            _options={'limit': 99},
-        )
-
-    def test_add_consumer(self):
-        self.app.control.add_consumer('foo')
-        self.assert_control_called_with_args(
-            'add_consumer',
-            destination=None,
-            queue='foo',
-            exchange=None,
-            exchange_type='direct',
-            routing_key=None,
-        )
-
-    def test_add_consumer__with_options_and_dest(self):
-        self.app.control.add_consumer(
-            'foo', 'ex', 'topic', 'rkey', destination='a@q.com', limit=78)
-        self.assert_control_called_with_args(
-            'add_consumer',
-            destination='a@q.com',
-            queue='foo',
-            exchange='ex',
-            exchange_type='topic',
-            routing_key='rkey',
-            _options={'limit': 78},
-        )
-
-    def test_cancel_consumer(self):
-        self.app.control.cancel_consumer('foo')
-        self.assert_control_called_with_args(
-            'cancel_consumer',
-            destination=None,
-            queue='foo',
-        )
-
-    def test_cancel_consumer__with_destination(self):
-        self.app.control.cancel_consumer(
-            'foo', destination='w1@q.com', limit=3)
-        self.assert_control_called_with_args(
-            'cancel_consumer',
-            destination='w1@q.com',
-            queue='foo',
-            _options={'limit': 3},
-        )
-
-    def test_shutdown(self):
-        self.app.control.shutdown()
-        self.assert_control_called_with_args('shutdown', destination=None)
-
-    def test_shutdown__with_destination(self):
-        self.app.control.shutdown(destination='a@q.com', limit=3)
-        self.assert_control_called_with_args(
-            'shutdown', destination='a@q.com', _options={'limit': 3})
-
-    def test_heartbeat(self):
-        self.app.control.heartbeat()
-        self.assert_control_called_with_args('heartbeat', destination=None)
-
-    def test_heartbeat__with_destination(self):
-        self.app.control.heartbeat(destination='a@q.com', limit=3)
-        self.assert_control_called_with_args(
-            'heartbeat', destination='a@q.com', _options={'limit': 3})
-
-    def test_pool_restart(self):
-        self.app.control.pool_restart()
-        self.assert_control_called_with_args(
-            'pool_restart',
-            destination=None,
-            modules=None,
-            reload=False,
-            reloader=None)
-
-    def test_terminate(self):
-        self.app.control.revoke = Mock(name='revoke')
-        self.app.control.terminate('124')
-        self.app.control.revoke.assert_called_with(
-            '124', destination=None,
-            terminate=True,
-            signal=control.TERM_SIGNAME,
-        )
-
-    def test_enable_events(self):
-        self.app.control.enable_events()
-        self.assert_control_called_with_args('enable_events', destination=None)
-
-    def test_enable_events_with_destination(self):
-        self.app.control.enable_events(destination='a@q.com', limit=3)
-        self.assert_control_called_with_args(
-            'enable_events', destination='a@q.com', _options={'limit': 3})
-
-    def test_disable_events(self):
-        self.app.control.disable_events()
-        self.assert_control_called_with_args(
-            'disable_events', destination=None)
-
-    def test_disable_events_with_destination(self):
-        self.app.control.disable_events(destination='a@q.com', limit=3)
-        self.assert_control_called_with_args(
-            'disable_events', destination='a@q.com', _options={'limit': 3})
-
-    def test_ping(self):
-        self.app.control.ping()
-        self.assert_control_called_with_args(
-            'ping', destination=None,
-            _options={'timeout': 1.0, 'reply': True})
-
-    def test_ping_with_destination(self):
-        self.app.control.ping(destination='a@q.com', limit=3)
-        self.assert_control_called_with_args(
-            'ping',
-            destination='a@q.com',
-            _options={
-                'limit': 3,
-                'timeout': 1.0,
-                'reply': True,
-            })
-
-    def test_revoke(self):
-        self.app.control.revoke('foozbaaz')
-        self.assert_control_called_with_args(
-            'revoke',
-            destination=None,
-            task_id='foozbaaz',
-            signal=control.TERM_SIGNAME,
-            terminate=False,
-        )
-
-    def test_revoke__with_options(self):
-        self.app.control.revoke(
-            'foozbaaz',
-            destination='a@q.com',
-            terminate=True,
-            signal='KILL',
-            limit=404,
-        )
-        self.assert_control_called_with_args(
-            'revoke',
-            destination='a@q.com',
-            task_id='foozbaaz',
-            signal='KILL',
-            terminate=True,
-            _options={'limit': 404},
-        )
-
-    def test_election(self):
-        self.app.control.election('some_id', 'topic', 'action')
-        self.assert_control_called_with_args(
-            'election',
-            destination=None,
-            topic='topic',
-            action='action',
-            id='some_id',
-            _options={'connection': None},
-        )
-
-    def test_autoscale(self):
-        self.app.control.autoscale(300, 10)
-        self.assert_control_called_with_args(
-            'autoscale', max=300, min=10, destination=None)
-
-    def test_autoscale__with_options(self):
-        self.app.control.autoscale(300, 10, destination='a@q.com', limit=39)
-        self.assert_control_called_with_args(
-            'autoscale', max=300, min=10,
-            destination='a@q.com',
-            _options={'limit': 39}
-        )
-
-    def test_pool_grow(self):
-        self.app.control.pool_grow(2)
-        self.assert_control_called_with_args(
-            'pool_grow', n=2, destination=None)
-
-    def test_pool_grow__with_options(self):
-        self.app.control.pool_grow(2, destination='a@q.com', limit=39)
-        self.assert_control_called_with_args(
-            'pool_grow', n=2,
-            destination='a@q.com',
-            _options={'limit': 39}
-        )
-
-    def test_pool_shrink(self):
-        self.app.control.pool_shrink(2)
-        self.assert_control_called_with_args(
-            'pool_shrink', n=2, destination=None)
-
-    def test_pool_shrink__with_options(self):
-        self.app.control.pool_shrink(2, destination='a@q.com', limit=39)
-        self.assert_control_called_with_args(
-            'pool_shrink', n=2,
-            destination='a@q.com',
-            _options={'limit': 39}
-        )
-
-    def test_revoke_from_result(self):
-        self.app.control.revoke = Mock(name='revoke')
-        self.app.AsyncResult('foozbazzbar').revoke()
-        self.app.control.revoke.assert_called_with(
-            'foozbazzbar',
-            connection=None, reply=False, signal=None,
-            terminate=False, timeout=None)
-
-    def test_revoke_from_resultset(self):
-        self.app.control.revoke = Mock(name='revoke')
-        uuids = [uuid() for _ in range(10)]
-        r = self.app.GroupResult(
-            uuid(), [self.app.AsyncResult(x) for x in uuids])
-        r.revoke()
-        self.app.control.revoke.assert_called_with(
-            uuids,
-            connection=None, reply=False, signal=None,
-            terminate=False, timeout=None)
-
-    def test_after_fork_clears_mailbox_pool(self):
-        amqp = Mock(name='amqp')
-        self.app.amqp = amqp
-        closed_pool = Mock(name='closed pool')
-        amqp.producer_pool = closed_pool
-        assert closed_pool is self.app.control.mailbox.producer_pool
-        self.app.control._after_fork()
-        new_pool = Mock(name='new pool')
-        amqp.producer_pool = new_pool
-        assert new_pool is self.app.control.mailbox.producer_pool
-
-    def test_control_exchange__default(self):
-        c = control.Control(self.app)
-        assert c.mailbox.namespace == 'celery'
-
-    def test_control_exchange__setting(self):
-        self.app.conf.control_exchange = 'test_exchange'
-        c = control.Control(self.app)
-        assert c.mailbox.namespace == 'test_exchange'
+from unittest.mock import Mock, AsyncMock
+
+import pytest
+
+from celery import uuid
+from celery.aio import control as aio_control
+from celery.app import control
+from celery.exceptions import DuplicateNodenameWarning
+from celery.utils.collections import LimitedSet
+
+from t.base import AsyncTest
+
+
+def _info_for_commandclass(type_):
+    from celery.worker.control import Panel
+    return [
+        (name, info)
+        for name, info in Panel.meta.items()
+        if info.type == type_
+    ]
+
+
+def test_client_implements_all_commands(app):
+    commands = _info_for_commandclass('control')
+    assert commands
+    for name, info in commands:
+        assert getattr(app.aio_control, name)
+
+
+def test_inspect_implements_all_commands(app):
+    inspect = app.aio_control.inspect()
+    commands = _info_for_commandclass('inspect')
+    assert commands
+    for name, info in commands:
+        if info.type == 'inspect':
+            assert getattr(inspect, name)
+
+
+class test_flatten_reply:
+
+    def test_flatten_reply(self):
+        reply = [
+            {'foo@example.com': {'hello': 10}},
+            {'foo@example.com': {'hello': 20}},
+            {'bar@example.com': {'hello': 30}}
+        ]
+        with pytest.warns(DuplicateNodenameWarning) as w:
+            nodes = control.flatten_reply(reply)
+
+        assert 'Received multiple replies from node name: {}.'.format(
+            next(iter(reply[0]))) in str(w[0].message.args[0])
+        assert 'foo@example.com' in nodes
+        assert 'bar@example.com' in nodes
+
+
+class test_inspect(AsyncTest):
+
+    def setup(self):
+        self.app.aio_control.broadcast = AsyncMock(name='broadcast')
+        self.app.aio_control.broadcast.return_value = {}
+        self.inspect = self.app.aio_control.inspect()
+
+    def test_prepare_reply(self):
+        reply = self.inspect._prepare([
+            {'w1': {'ok': 1}},
+            {'w2': {'ok': 1}},
+        ])
+        assert reply == {
+            'w1': {'ok': 1},
+            'w2': {'ok': 1},
+        }
+
+        i = self.app.aio_control.inspect(destination='w1')
+        assert i._prepare([{'w1': {'ok': 1}}]) == {'ok': 1}
+
+    def assert_broadcast_called(self, command,
+                                destination=None,
+                                callback=None,
+                                connection=None,
+                                limit=None,
+                                timeout=None,
+                                reply=True,
+                                pattern=None,
+                                matcher=None,
+                                **arguments):
+        self.app.aio_control.broadcast.assert_called_with(
+            command,
+            arguments=arguments,
+            destination=destination or self.inspect.destination,
+            pattern=pattern or self.inspect.pattern,
+            matcher=matcher or self.inspect.destination,
+            callback=callback or self.inspect.callback,
+            connection=connection or self.inspect.connection,
+            limit=limit if limit is not None else self.inspect.limit,
+            timeout=timeout if timeout is not None else self.inspect.timeout,
+            reply=reply,
+        )
+
+    async def test_active(self):
+        await self.inspect.active()
+        self.assert_broadcast_called('active')
+
+    async def test_clock(self):
+        await self.inspect.clock()
+        self.assert_broadcast_called('clock')
+
+    async def test_conf(self):
+        await self.inspect.conf()
+        self.assert_broadcast_called('conf', with_defaults=False)
+
+    async def test_conf__with_defaults(self):
+        await self.inspect.conf(with_defaults=True)
+        self.assert_broadcast_called('conf', with_defaults=True)
+
+    async def test_hello(self):
+        await self.inspect.hello('george@vandelay.com')
+        self.assert_broadcast_called(
+            'hello', from_node='george@vandelay.com', revoked=None)
+
+    async def test_hello__with_revoked(self):
+        revoked = LimitedSet(100)
+        for i in range(100):
+            revoked.add(f'id{i}')
+        await self.inspect.hello('george@vandelay.com', revoked=revoked._data)
+        self.assert_broadcast_called(
+            'hello', from_node='george@vandelay.com', revoked=revoked._data)
+
+    async def test_memsample(self):
+        await self.inspect.memsample()
+        self.assert_broadcast_called('memsample')
+
+    async def test_memdump(self):
+        await self.inspect.memdump()
+        self.assert_broadcast_called('memdump', samples=10)
+
+    async def test_memdump__samples_specified(self):
+        await self.inspect.memdump(samples=303)
+        self.assert_broadcast_called('memdump', samples=303)
+
+    async def test_objgraph(self):
+        await self.inspect.objgraph()
+        self.assert_broadcast_called(
+            'objgraph', num=200, type='Request', max_depth=10)
+
+    async def test_scheduled(self):
+        await self.inspect.scheduled()
+        self.assert_broadcast_called('scheduled')
+
+    async def test_reserved(self):
+        await self.inspect.reserved()
+        self.assert_broadcast_called('reserved')
+
+    async def test_stats(self):
+        await self.inspect.stats()
+        self.assert_broadcast_called('stats')
+
+    async def test_revoked(self):
+        await self.inspect.revoked()
+        self.assert_broadcast_called('revoked')
+
+    async def test_registered(self):
+        await self.inspect.registered()
+        self.assert_broadcast_called('registered', taskinfoitems=())
+
+    async def test_registered__taskinfoitems(self):
+        await self.inspect.registered('rate_limit', 'time_limit')
+        self.assert_broadcast_called(
+            'registered',
+            taskinfoitems=('rate_limit', 'time_limit'),
+        )
+
+    async def test_ping(self):
+        await self.inspect.ping()
+        self.assert_broadcast_called('ping')
+
+    async def test_ping_matcher_pattern(self):
+        orig_inspect = self.inspect
+        self.inspect = self.app.aio_control.inspect(pattern=".*", matcher="pcre")
+        await self.inspect.ping()
+        try:
+            self.assert_broadcast_called('ping', pattern=".*", matcher="pcre")
+        except AssertionError as e:
+            self.inspect = orig_inspect
+            raise e
+
+    async def test_active_queues(self):
+        await self.inspect.active_queues()
+        self.assert_broadcast_called('active_queues')
+
+    async def test_query_task(self):
+        await self.inspect.query_task('foo', 'bar')
+        self.assert_broadcast_called('query_task', ids=('foo', 'bar'))
+
+    async def test_query_task__compat_single_list_argument(self):
+        await self.inspect.query_task(['foo', 'bar'])
+        self.assert_broadcast_called('query_task', ids=['foo', 'bar'])
+
+    async def test_query_task__scalar(self):
+        await self.inspect.query_task('foo')
+        self.assert_broadcast_called('query_task', ids=('foo',))
+
+    async def test_report(self):
+        await self.inspect.report()
+        self.assert_broadcast_called('report')
+
+
+class test_Control_broadcast(AsyncTest):
+
+    def setup(self):
+        self.app.aio_control.mailbox = Mock(
+            name='mailbox', return_value=AsyncMock())
+
+    async def test_broadcast(self):
+        await self.app.aio_control.broadcast('foobarbaz', arguments={'foo': 2})
+        self.app.aio_control.mailbox.assert_called()
+        self.app.aio_control.mailbox()._broadcast.assert_called_with(
+            'foobarbaz', {'foo': 2}, None, False, 1.0, None, None,
+            channel=None,
+        )
+
+    async def test_broadcast_limit(self):
+        await self.app.aio_control.broadcast(
+            'foobarbaz1', arguments=None, limit=None, destination=[1, 2, 3],
+        )
+        self.app.aio_control.mailbox.assert_called()
+        self.app.aio_control.mailbox()._broadcast.assert_called_with(
+            'foobarbaz1', {}, [1, 2, 3], False, 1.0, None, None,
+            channel=None,
+        )
+
+
+class test_Control(AsyncTest):
+
+    def setup(self):
+        self.app.aio_control.broadcast = AsyncMock(name='broadcast')
+        self.app.aio_control.broadcast.return_value = {}
+
+        @self.app.task(shared=False, aio_variant=True)
+        def mytask():
+            pass
+        self.mytask = mytask
+
+    def assert_control_called_with_args(self, name, destination=None,
+                                        _options=None, **args):
+        self.app.aio_control.broadcast.assert_called_with(
+            name, destination=destination, arguments=args, **_options or {})
+
+    async def zzz_test_purge(self):
+        self.app.amqp.TaskConsumer = Mock(name='TaskConsumer')
+        await self.app.aio_control.purge()
+        self.app.amqp.TaskConsumer().purge.assert_called_with()
+
+    async def test_rate_limit(self):
+        await self.app.aio_control.rate_limit(self.mytask.name, '100/m')
+        self.assert_control_called_with_args(
+            'rate_limit',
+            destination=None,
+            task_name=self.mytask.name,
+            rate_limit='100/m',
+        )
+
+    async def test_rate_limit__with_destination(self):
+        await self.app.aio_control.rate_limit(
+            self.mytask.name, '100/m', 'a@w.com', limit=100)
+        self.assert_control_called_with_args(
+            'rate_limit',
+            destination='a@w.com',
+            task_name=self.mytask.name,
+            rate_limit='100/m',
+            _options={'limit': 100},
+        )
+
+    async def test_time_limit(self):
+        await self.app.aio_control.time_limit(self.mytask.name, soft=10, hard=20)
+        self.assert_control_called_with_args(
+            'time_limit',
+            destination=None,
+            task_name=self.mytask.name,
+            soft=10,
+            hard=20,
+        )
+
+    async def test_time_limit__with_destination(self):
+        await self.app.aio_control.time_limit(
+            self.mytask.name, soft=10, hard=20,
+            destination='a@q.com', limit=99,
+        )
+        self.assert_control_called_with_args(
+            'time_limit',
+            destination='a@q.com',
+            task_name=self.mytask.name,
+            soft=10,
+            hard=20,
+            _options={'limit': 99},
+        )
+
+    async def test_add_consumer(self):
+        await self.app.aio_control.add_consumer('foo')
+        self.assert_control_called_with_args(
+            'add_consumer',
+            destination=None,
+            queue='foo',
+            exchange=None,
+            exchange_type='direct',
+            routing_key=None,
+        )
+
+    async def test_add_consumer__with_options_and_dest(self):
+        await self.app.aio_control.add_consumer(
+            'foo', 'ex', 'topic', 'rkey', destination='a@q.com', limit=78)
+        self.assert_control_called_with_args(
+            'add_consumer',
+            destination='a@q.com',
+            queue='foo',
+            exchange='ex',
+            exchange_type='topic',
+            routing_key='rkey',
+            _options={'limit': 78},
+        )
+
+    async def test_cancel_consumer(self):
+        await self.app.aio_control.cancel_consumer('foo')
+        self.assert_control_called_with_args(
+            'cancel_consumer',
+            destination=None,
+            queue='foo',
+        )
+
+    async def test_cancel_consumer__with_destination(self):
+        self.app.aio_control.cancel_consumer(
+            'foo', destination='w1@q.com', limit=3)
+        self.assert_control_called_with_args(
+            'cancel_consumer',
+            destination='w1@q.com',
+            queue='foo',
+            _options={'limit': 3},
+        )
+
+    async def test_shutdown(self):
+        await self.app.aio_control.shutdown()
+        self.assert_control_called_with_args('shutdown', destination=None)
+
+    async def test_shutdown__with_destination(self):
+        await self.app.aio_control.shutdown(destination='a@q.com', limit=3)
+        self.assert_control_called_with_args(
+            'shutdown', destination='a@q.com', _options={'limit': 3})
+
+    async def test_heartbeat(self):
+        await self.app.aio_control.heartbeat()
+        self.assert_control_called_with_args('heartbeat', destination=None)
+
+    async def test_heartbeat__with_destination(self):
+        await self.app.aio_control.heartbeat(destination='a@q.com', limit=3)
+        self.assert_control_called_with_args(
+            'heartbeat', destination='a@q.com', _options={'limit': 3})
+
+    async def test_pool_restart(self):
+        await self.app.aio_control.pool_restart()
+        self.assert_control_called_with_args(
+            'pool_restart',
+            destination=None,
+            modules=None,
+            reload=False,
+            reloader=None)
+
+    async def test_terminate(self):
+        self.app.aio_control.revoke = AsyncMock(name='revoke')
+        await self.app.aio_control.terminate('124')
+        self.app.aio_control.revoke.assert_called_with(
+            '124', destination=None,
+            terminate=True,
+            signal=control.TERM_SIGNAME,
+        )
+
+    async def test_enable_events(self):
+        await self.app.aio_control.enable_events()
+        self.assert_control_called_with_args('enable_events', destination=None)
+
+    async def test_enable_events_with_destination(self):
+        await self.app.aio_control.enable_events(destination='a@q.com', limit=3)
+        self.assert_control_called_with_args(
+            'enable_events', destination='a@q.com', _options={'limit': 3})
+
+    async def test_disable_events(self):
+        await self.app.aio_control.disable_events()
+        self.assert_control_called_with_args(
+            'disable_events', destination=None)
+
+    async def test_disable_events_with_destination(self):
+        await self.app.aio_control.disable_events(destination='a@q.com', limit=3)
+        self.assert_control_called_with_args(
+            'disable_events', destination='a@q.com', _options={'limit': 3})
+
+    async def test_ping(self):
+        await self.app.aio_control.ping()
+        self.assert_control_called_with_args(
+            'ping', destination=None,
+            _options={'timeout': 1.0, 'reply': True})
+
+    async def test_ping_with_destination(self):
+        await self.app.aio_control.ping(destination='a@q.com', limit=3)
+        self.assert_control_called_with_args(
+            'ping',
+            destination='a@q.com',
+            _options={
+                'limit': 3,
+                'timeout': 1.0,
+                'reply': True,
+            })
+
+    async def test_revoke(self):
+        await self.app.aio_control.revoke('foozbaaz')
+        self.assert_control_called_with_args(
+            'revoke',
+            destination=None,
+            task_id='foozbaaz',
+            signal=control.TERM_SIGNAME,
+            terminate=False,
+        )
+
+    async def test_revoke__with_options(self):
+        await self.app.aio_control.revoke(
+            'foozbaaz',
+            destination='a@q.com',
+            terminate=True,
+            signal='KILL',
+            limit=404,
+        )
+        self.assert_control_called_with_args(
+            'revoke',
+            destination='a@q.com',
+            task_id='foozbaaz',
+            signal='KILL',
+            terminate=True,
+            _options={'limit': 404},
+        )
+
+    async def test_election(self):
+        await self.app.aio_control.election('some_id', 'topic', 'action')
+        self.assert_control_called_with_args(
+            'election',
+            destination=None,
+            topic='topic',
+            action='action',
+            id='some_id',
+            _options={'connection': None},
+        )
+
+    async def test_autoscale(self):
+        await self.app.aio_control.autoscale(300, 10)
+        self.assert_control_called_with_args(
+            'autoscale', max=300, min=10, destination=None)
+
+    async def test_autoscale__with_options(self):
+        await self.app.aio_control.autoscale(300, 10, destination='a@q.com', limit=39)
+        self.assert_control_called_with_args(
+            'autoscale', max=300, min=10,
+            destination='a@q.com',
+            _options={'limit': 39}
+        )
+
+    async def test_pool_grow(self):
+        await self.app.aio_control.pool_grow(2)
+        self.assert_control_called_with_args(
+            'pool_grow', n=2, destination=None)
+
+    async def test_pool_grow__with_options(self):
+        await self.app.aio_control.pool_grow(2, destination='a@q.com', limit=39)
+        self.assert_control_called_with_args(
+            'pool_grow', n=2,
+            destination='a@q.com',
+            _options={'limit': 39}
+        )
+
+    async def test_pool_shrink(self):
+        await self.app.aio_control.pool_shrink(2)
+        self.assert_control_called_with_args(
+            'pool_shrink', n=2, destination=None)
+
+    async def test_pool_shrink__with_options(self):
+        await self.app.aio_control.pool_shrink(2, destination='a@q.com', limit=39)
+        self.assert_control_called_with_args(
+            'pool_shrink', n=2,
+            destination='a@q.com',
+            _options={'limit': 39}
+        )
+
+    async def test_revoke_from_result(self):
+        self.app.aio_control.revoke = AsyncMock(name='revoke')
+        await self.app.AioAsyncResult('foozbazzbar').revoke()
+        self.app.aio_control.revoke.assert_called_with(
+            'foozbazzbar',
+            connection=None, reply=False, signal=None,
+            terminate=False, timeout=None)
+
+    async def test_revoke_from_resultset(self):
+        self.app.aio_control.revoke = AsyncMock(name='revoke')
+        uuids = [uuid() for _ in range(10)]
+        r = self.app.AioGroupResult(
+            uuid(), [self.app.AioAsyncResult(x) for x in uuids])
+        await r.revoke()
+        self.app.aio_control.revoke.assert_called_with(
+            uuids,
+            connection=None, reply=False, signal=None,
+            terminate=False, timeout=None)
+
+    def test_after_fork_clears_mailbox_pool(self):
+        amqp = Mock(name='amqp')
+        self.app.aio_amqp = amqp
+        closed_pool = Mock(name='closed pool')
+        amqp.producer_pool = closed_pool
+        assert closed_pool is self.app.aio_control.mailbox.producer_pool
+        self.app.aio_control._after_fork()
+        new_pool = Mock(name='new pool')
+        amqp.producer_pool = new_pool
+        assert new_pool is self.app.aio_control.mailbox.producer_pool
+
+    def test_control_exchange__default(self):
+        c = aio_control.Control(self.app)
+        assert c.mailbox.namespace == 'celery'
+
+    def test_control_exchange__setting(self):
+        self.app.conf.control_exchange = 'test_exchange'
+        c = aio_control.Control(self.app)
+        assert c.mailbox.namespace == 'test_exchange'
```

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_defaults.py` & `deepfos-celery-1.0.3/t/unit/app/test_defaults.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_exceptions.py` & `deepfos-celery-1.0.3/t/unit/app/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_loaders.py` & `deepfos-celery-1.0.3/t/unit/app/test_loaders.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_log.py` & `deepfos-celery-1.0.3/t/unit/app/test_log.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_registry.py` & `deepfos-celery-1.0.3/t/unit/app/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_routes.py` & `deepfos-celery-1.0.3/t/unit/app/test_routes.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_schedules.py` & `deepfos-celery-1.0.3/t/unit/app/test_schedules.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/app/test_utils.py` & `deepfos-celery-1.0.3/t/unit/app/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/apps/test_multi.py` & `deepfos-celery-1.0.3/t/unit/apps/test_multi.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_arangodb.py` & `deepfos-celery-1.0.3/t/unit/backends/test_arangodb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_asynchronous.py` & `deepfos-celery-1.0.3/t/unit/backends/test_asynchronous.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_azureblockblob.py` & `deepfos-celery-1.0.3/t/unit/backends/test_azureblockblob.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_base.py` & `deepfos-celery-1.0.3/t/unit/backends/test_base.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_cache.py` & `deepfos-celery-1.0.3/t/unit/backends/test_cache.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_cassandra.py` & `deepfos-celery-1.0.3/t/unit/backends/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_consul.py` & `deepfos-celery-1.0.3/t/unit/backends/test_consul.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_cosmosdbsql.py` & `deepfos-celery-1.0.3/t/unit/backends/test_cosmosdbsql.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_couchbase.py` & `deepfos-celery-1.0.3/t/unit/backends/test_couchbase.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_couchdb.py` & `deepfos-celery-1.0.3/t/unit/backends/test_couchdb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_database.py` & `deepfos-celery-1.0.3/t/unit/backends/test_database.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_dynamodb.py` & `deepfos-celery-1.0.3/t/unit/backends/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_elasticsearch.py` & `deepfos-celery-1.0.3/t/unit/backends/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_filesystem.py` & `deepfos-celery-1.0.3/t/unit/backends/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_mongodb.py` & `deepfos-celery-1.0.3/t/unit/backends/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_redis.py` & `deepfos-celery-1.0.3/t/unit/backends/test_redis.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_rpc.py` & `deepfos-celery-1.0.3/t/unit/backends/test_rpc.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/backends/test_s3.py` & `deepfos-celery-1.0.3/t/unit/backends/test_s3.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/concurrency/test_concurrency.py` & `deepfos-celery-1.0.3/t/unit/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/concurrency/test_eventlet.py` & `deepfos-celery-1.0.3/t/unit/concurrency/test_eventlet.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/concurrency/test_gevent.py` & `deepfos-celery-1.0.3/t/unit/concurrency/test_gevent.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/concurrency/test_pool.py` & `deepfos-celery-1.0.3/t/unit/concurrency/test_pool.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/concurrency/test_prefork.py` & `deepfos-celery-1.0.3/t/unit/concurrency/test_prefork.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/concurrency/test_solo.py` & `deepfos-celery-1.0.3/t/unit/concurrency/test_solo.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/concurrency/test_thread.py` & `deepfos-celery-1.0.3/t/unit/concurrency/test_thread.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/conftest.py` & `deepfos-celery-1.0.3/t/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/contrib/test_abortable.py` & `deepfos-celery-1.0.3/t/unit/contrib/test_abortable.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/contrib/test_migrate.py` & `deepfos-celery-1.0.3/t/unit/contrib/test_migrate.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/contrib/test_pytest.py` & `deepfos-celery-1.0.3/t/unit/contrib/test_pytest.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/contrib/test_rdb.py` & `deepfos-celery-1.0.3/t/unit/contrib/test_rdb.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/contrib/test_sphinx.py` & `deepfos-celery-1.0.3/t/unit/contrib/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/events/test_cursesmon.py` & `deepfos-celery-1.0.3/t/unit/events/test_cursesmon.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/events/test_events.py` & `deepfos-celery-1.0.3/t/unit/events/test_events.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/events/test_snapshot.py` & `deepfos-celery-1.0.3/t/unit/events/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/events/test_state.py` & `deepfos-celery-1.0.3/t/unit/events/test_state.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/fixups/test_django.py` & `deepfos-celery-1.0.3/t/unit/fixups/test_django.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/security/__init__.py` & `deepfos-celery-1.0.3/t/unit/security/__init__.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/security/test_certificate.py` & `deepfos-celery-1.0.3/t/unit/security/test_certificate.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/security/test_key.py` & `deepfos-celery-1.0.3/t/unit/security/test_key.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/security/test_security.py` & `deepfos-celery-1.0.3/t/unit/security/test_security.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/security/test_serialization.py` & `deepfos-celery-1.0.3/t/unit/security/test_serialization.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/tasks/test_canvas.py` & `deepfos-celery-1.0.3/t/unit/tasks/test_canvas.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/tasks/test_chord.py` & `deepfos-celery-1.0.3/t/unit/tasks/test_chord.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/tasks/test_context.py` & `deepfos-celery-1.0.3/t/unit/tasks/test_context.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/tasks/test_result.py` & `deepfos-celery-1.0.3/t/unit/tasks/test_result.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/tasks/test_states.py` & `deepfos-celery-1.0.3/t/unit/tasks/test_states.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/tasks/test_tasks.py` & `deepfos-celery-1.0.3/t/unit/tasks/test_tasks.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/tasks/test_trace.py` & `deepfos-celery-1.0.3/t/unit/tasks/test_trace.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/test_canvas.py` & `deepfos-celery-1.0.3/t/unit/test_canvas.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_collections.py` & `deepfos-celery-1.0.3/t/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_debug.py` & `deepfos-celery-1.0.3/t/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_deprecated.py` & `deepfos-celery-1.0.3/t/unit/utils/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_dispatcher.py` & `deepfos-celery-1.0.3/t/unit/utils/test_dispatcher.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,396 +1,396 @@
-import gc
-import sys
-import time
-
-from celery.utils.dispatch import Signal
-from t.base import AsyncTest
-
-if sys.platform.startswith('java'):
-
-    def garbage_collect():
-        # Some JVM GCs will execute finalizers in a different thread, meaning
-        # we need to wait for that to complete before we go on looking for the
-        # effects of that.
-        gc.collect()
-        time.sleep(0.1)
-
-elif hasattr(sys, 'pypy_version_info'):
-
-    def garbage_collect():  # noqa
-        # Collecting weakreferences can take two collections on PyPy.
-        gc.collect()
-        gc.collect()
-else:
-
-    def garbage_collect():  # noqa
-        gc.collect()
-
-
-def receiver_1_arg(val, **kwargs):
-    return val
-
-
-async def async_receiver_1_arg(val, **kwargs):
-    return val
-
-
-class Callable:
-
-    def __call__(self, val, **kwargs):
-        return val
-
-    def a(self, val, **kwargs):
-        return val
-
-
-class AsyncCallable:
-
-    async def __call__(self, val, **kwargs):
-        return val
-
-    async def a(self, val, **kwargs):
-        return val
-
-
-a_signal = Signal(providing_args=['val'], use_caching=False)
-
-
-class test_Signal:
-    """Test suite for dispatcher (barely started)"""
-
-    def _testIsClean(self, signal):
-        """Assert that everything has been cleaned up automatically"""
-        assert not signal.has_listeners()
-        assert signal.receivers == []
-
-    def test_exact(self):
-        a_signal.connect(receiver_1_arg, sender=self)
-        try:
-            expected = [(receiver_1_arg, 'test')]
-            result = a_signal.send(sender=self, val='test')
-            assert result == expected
-        finally:
-            a_signal.disconnect(receiver_1_arg, sender=self)
-        self._testIsClean(a_signal)
-
-    def test_ignored_sender(self):
-        a_signal.connect(receiver_1_arg)
-        try:
-            expected = [(receiver_1_arg, 'test')]
-            result = a_signal.send(sender=self, val='test')
-            assert result == expected
-        finally:
-            a_signal.disconnect(receiver_1_arg)
-        self._testIsClean(a_signal)
-
-    def test_garbage_collected(self):
-        a = Callable()
-        a_signal.connect(a.a, sender=self)
-        expected = []
-        del a
-        garbage_collect()
-        result = a_signal.send(sender=self, val='test')
-        assert result == expected
-        self._testIsClean(a_signal)
-
-    def test_multiple_registration(self):
-        a = Callable()
-        result = None
-        try:
-            a_signal.connect(a)
-            a_signal.connect(a)
-            a_signal.connect(a)
-            a_signal.connect(a)
-            a_signal.connect(a)
-            a_signal.connect(a)
-            result = a_signal.send(sender=self, val='test')
-            assert len(result) == 1
-            assert len(a_signal.receivers) == 1
-        finally:
-            del a
-            del result
-            garbage_collect()
-            self._testIsClean(a_signal)
-
-    def test_uid_registration(self):
-
-        def uid_based_receiver_1(**kwargs):
-            pass
-
-        def uid_based_receiver_2(**kwargs):
-            pass
-
-        a_signal.connect(uid_based_receiver_1, dispatch_uid='uid')
-        try:
-            a_signal.connect(uid_based_receiver_2, dispatch_uid='uid')
-            assert len(a_signal.receivers) == 1
-        finally:
-            a_signal.disconnect(dispatch_uid='uid')
-        self._testIsClean(a_signal)
-
-    def test_robust(self):
-
-        def fails(val, **kwargs):
-            raise ValueError('this')
-
-        a_signal.connect(fails)
-        try:
-            a_signal.send(sender=self, val='test')
-        finally:
-            a_signal.disconnect(fails)
-        self._testIsClean(a_signal)
-
-    def test_disconnection(self):
-        receiver_1 = Callable()
-        receiver_2 = Callable()
-        receiver_3 = Callable()
-        try:
-            try:
-                a_signal.connect(receiver_1)
-                a_signal.connect(receiver_2)
-                a_signal.connect(receiver_3)
-            finally:
-                a_signal.disconnect(receiver_1)
-            del receiver_2
-            garbage_collect()
-        finally:
-            a_signal.disconnect(receiver_3)
-        self._testIsClean(a_signal)
-
-    def test_retry(self):
-
-        class non_local:
-            counter = 1
-
-        def succeeds_eventually(val, **kwargs):
-            non_local.counter += 1
-            if non_local.counter < 3:
-                raise ValueError('this')
-
-            return val
-
-        a_signal.connect(succeeds_eventually, sender=self, retry=True)
-        try:
-            result = a_signal.send(sender=self, val='test')
-            assert non_local.counter == 3
-            assert result[0][1] == 'test'
-        finally:
-            a_signal.disconnect(succeeds_eventually, sender=self)
-        self._testIsClean(a_signal)
-
-    def test_retry_with_dispatch_uid(self):
-        uid = 'abc123'
-        a_signal.connect(receiver_1_arg, sender=self, retry=True,
-                         dispatch_uid=uid)
-        assert a_signal.receivers[0][0][0] == uid
-        a_signal.disconnect(receiver_1_arg, sender=self, dispatch_uid=uid)
-        self._testIsClean(a_signal)
-
-    def test_boundmethod(self):
-        a = Callable()
-        a_signal.connect(a.a, sender=self)
-        expected = [(a.a, 'test')]
-        garbage_collect()
-        result = a_signal.send(sender=self, val='test')
-        assert result == expected
-        del a, result, expected
-        garbage_collect()
-        self._testIsClean(a_signal)
-
-    def test_deco_no_arg(self):
-        class non_local:
-            counter = 1
-
-        @a_signal.connect
-        def f(val, **kwargs):
-            non_local.counter += 1
-            return val
-
-        try:
-            result = a_signal.send(sender=None, val='test')
-            assert non_local.counter == 2
-            assert result[0][1] == 'test'
-        finally:
-            a_signal.disconnect(f, sender=None)
-        self._testIsClean(a_signal)
-
-
-class test_AsyncSignal(AsyncTest):
-    def _testIsClean(self, signal):
-        """Assert that everything has been cleaned up automatically"""
-        assert not signal.has_listeners()
-        assert signal.areceivers == []
-
-    async def test_exact(self):
-        a_signal.connect(async_receiver_1_arg, sender=self)
-        try:
-            expected = [(async_receiver_1_arg, 'test')]
-            result = await a_signal.asend(sender=self, val='test')
-            assert result == expected
-        finally:
-            a_signal.disconnect(async_receiver_1_arg, sender=self)
-        self._testIsClean(a_signal)
-
-    async def test_ignored_sender(self):
-        a_signal.connect(async_receiver_1_arg)
-        try:
-            expected = [(async_receiver_1_arg, 'test')]
-            result = await a_signal.asend(sender=self, val='test')
-            assert result == expected
-        finally:
-            a_signal.disconnect(async_receiver_1_arg)
-        self._testIsClean(a_signal)
-
-    async def test_garbage_collected(self):
-        a = AsyncCallable()
-        a_signal.connect(a.a, sender=self)
-        expected = []
-        del a
-        garbage_collect()
-        result = await a_signal.asend(sender=self, val='test')
-        assert result == expected
-        self._testIsClean(a_signal)
-
-    async def test_multiple_registration(self):
-        a = AsyncCallable()
-        result = None
-        try:
-            a_signal.connect(a)
-            a_signal.connect(a)
-            a_signal.connect(a)
-            a_signal.connect(a)
-            a_signal.connect(a)
-            a_signal.connect(a)
-            result = await a_signal.asend(sender=self, val='test')
-            assert len(result) == 1
-            assert len(a_signal.areceivers) == 1
-        finally:
-            del a
-            del result
-            garbage_collect()
-            self._testIsClean(a_signal)
-
-    async def test_uid_registration(self):
-
-        async def uid_based_receiver_1(**kwargs):
-            pass
-
-        async def uid_based_receiver_2(**kwargs):
-            pass
-
-        a_signal.connect(uid_based_receiver_1, dispatch_uid='uid')
-        try:
-            a_signal.connect(uid_based_receiver_2, dispatch_uid='uid')
-            assert len(a_signal.areceivers) == 1
-        finally:
-            a_signal.disconnect(dispatch_uid='uid')
-        self._testIsClean(a_signal)
-
-    async def test_robust(self):
-
-        async def fails(val, **kwargs):
-            raise ValueError('this')
-
-        a_signal.connect(fails)
-        try:
-            await a_signal.asend(sender=self, val='test')
-        finally:
-            a_signal.disconnect(fails)
-        self._testIsClean(a_signal)
-
-    async def test_disconnection(self):
-        receiver_1 = AsyncCallable()
-        receiver_2 = AsyncCallable()
-        receiver_3 = AsyncCallable()
-        try:
-            try:
-                a_signal.connect(receiver_1)
-                a_signal.connect(receiver_2)
-                a_signal.connect(receiver_3)
-            finally:
-                a_signal.disconnect(receiver_1)
-            del receiver_2
-            garbage_collect()
-        finally:
-            a_signal.disconnect(receiver_3)
-        self._testIsClean(a_signal)
-
-    async def test_retry(self):
-
-        class non_local:
-            counter = 1
-
-        async def succeeds_eventually(val, **kwargs):
-            non_local.counter += 1
-            if non_local.counter < 3:
-                raise ValueError('this')
-
-            return val
-
-        a_signal.connect(succeeds_eventually, sender=self, retry=True)
-        try:
-            result = await a_signal.asend(sender=self, val='test')
-            assert non_local.counter == 3
-            assert result[0][1] == 'test'
-        finally:
-            a_signal.disconnect(succeeds_eventually, sender=self)
-        self._testIsClean(a_signal)
-
-    async def test_retry_with_dispatch_uid(self):
-        uid = 'abc123'
-        a_signal.connect(async_receiver_1_arg, sender=self, retry=True,
-                         dispatch_uid=uid)
-        assert a_signal.areceivers[0][0][0] == uid
-        a_signal.disconnect(async_receiver_1_arg, sender=self, dispatch_uid=uid)
-        self._testIsClean(a_signal)
-
-    async def test_boundmethod(self):
-        a = AsyncCallable()
-        a_signal.connect(a.a, sender=self)
-        expected = [(a.a, 'test')]
-        garbage_collect()
-        result = await a_signal.asend(sender=self, val='test')
-        assert result == expected
-        del a, result, expected
-        garbage_collect()
-        self._testIsClean(a_signal)
-
-    async def test_deco_no_arg(self):
-        class non_local:
-            counter = 1
-
-        @a_signal.connect
-        async def f(val, **kwargs):
-            non_local.counter += 1
-            return val
-
-        try:
-            result = await a_signal.asend(sender=None, val='test')
-            assert non_local.counter == 2
-            assert result[0][1] == 'test'
-        finally:
-            a_signal.disconnect(f, sender=None)
-        self._testIsClean(a_signal)
-
-    async def test_retry_on_async_callable(self):
-        class non_local:
-            counter = 1
-
-        class ARetry:
-            async def __call__(self, val, **kwargs):
-                non_local.counter += 1
-                if non_local.counter < 3:
-                    raise ValueError('this')
-
-                return val
-
-        succeeds_eventually = ARetry()
-
-        a_signal.connect(succeeds_eventually, sender=self, retry=True)
-        try:
-            result = await a_signal.asend(sender=self, val='test')
-            assert non_local.counter == 3
-            assert result[0][1] == 'test'
-        finally:
-            a_signal.disconnect(succeeds_eventually, sender=self)
-        self._testIsClean(a_signal)
+import gc
+import sys
+import time
+
+from celery.utils.dispatch import Signal
+from t.base import AsyncTest
+
+if sys.platform.startswith('java'):
+
+    def garbage_collect():
+        # Some JVM GCs will execute finalizers in a different thread, meaning
+        # we need to wait for that to complete before we go on looking for the
+        # effects of that.
+        gc.collect()
+        time.sleep(0.1)
+
+elif hasattr(sys, 'pypy_version_info'):
+
+    def garbage_collect():  # noqa
+        # Collecting weakreferences can take two collections on PyPy.
+        gc.collect()
+        gc.collect()
+else:
+
+    def garbage_collect():  # noqa
+        gc.collect()
+
+
+def receiver_1_arg(val, **kwargs):
+    return val
+
+
+async def async_receiver_1_arg(val, **kwargs):
+    return val
+
+
+class Callable:
+
+    def __call__(self, val, **kwargs):
+        return val
+
+    def a(self, val, **kwargs):
+        return val
+
+
+class AsyncCallable:
+
+    async def __call__(self, val, **kwargs):
+        return val
+
+    async def a(self, val, **kwargs):
+        return val
+
+
+a_signal = Signal(providing_args=['val'], use_caching=False)
+
+
+class test_Signal:
+    """Test suite for dispatcher (barely started)"""
+
+    def _testIsClean(self, signal):
+        """Assert that everything has been cleaned up automatically"""
+        assert not signal.has_listeners()
+        assert signal.receivers == []
+
+    def test_exact(self):
+        a_signal.connect(receiver_1_arg, sender=self)
+        try:
+            expected = [(receiver_1_arg, 'test')]
+            result = a_signal.send(sender=self, val='test')
+            assert result == expected
+        finally:
+            a_signal.disconnect(receiver_1_arg, sender=self)
+        self._testIsClean(a_signal)
+
+    def test_ignored_sender(self):
+        a_signal.connect(receiver_1_arg)
+        try:
+            expected = [(receiver_1_arg, 'test')]
+            result = a_signal.send(sender=self, val='test')
+            assert result == expected
+        finally:
+            a_signal.disconnect(receiver_1_arg)
+        self._testIsClean(a_signal)
+
+    def test_garbage_collected(self):
+        a = Callable()
+        a_signal.connect(a.a, sender=self)
+        expected = []
+        del a
+        garbage_collect()
+        result = a_signal.send(sender=self, val='test')
+        assert result == expected
+        self._testIsClean(a_signal)
+
+    def test_multiple_registration(self):
+        a = Callable()
+        result = None
+        try:
+            a_signal.connect(a)
+            a_signal.connect(a)
+            a_signal.connect(a)
+            a_signal.connect(a)
+            a_signal.connect(a)
+            a_signal.connect(a)
+            result = a_signal.send(sender=self, val='test')
+            assert len(result) == 1
+            assert len(a_signal.receivers) == 1
+        finally:
+            del a
+            del result
+            garbage_collect()
+            self._testIsClean(a_signal)
+
+    def test_uid_registration(self):
+
+        def uid_based_receiver_1(**kwargs):
+            pass
+
+        def uid_based_receiver_2(**kwargs):
+            pass
+
+        a_signal.connect(uid_based_receiver_1, dispatch_uid='uid')
+        try:
+            a_signal.connect(uid_based_receiver_2, dispatch_uid='uid')
+            assert len(a_signal.receivers) == 1
+        finally:
+            a_signal.disconnect(dispatch_uid='uid')
+        self._testIsClean(a_signal)
+
+    def test_robust(self):
+
+        def fails(val, **kwargs):
+            raise ValueError('this')
+
+        a_signal.connect(fails)
+        try:
+            a_signal.send(sender=self, val='test')
+        finally:
+            a_signal.disconnect(fails)
+        self._testIsClean(a_signal)
+
+    def test_disconnection(self):
+        receiver_1 = Callable()
+        receiver_2 = Callable()
+        receiver_3 = Callable()
+        try:
+            try:
+                a_signal.connect(receiver_1)
+                a_signal.connect(receiver_2)
+                a_signal.connect(receiver_3)
+            finally:
+                a_signal.disconnect(receiver_1)
+            del receiver_2
+            garbage_collect()
+        finally:
+            a_signal.disconnect(receiver_3)
+        self._testIsClean(a_signal)
+
+    def test_retry(self):
+
+        class non_local:
+            counter = 1
+
+        def succeeds_eventually(val, **kwargs):
+            non_local.counter += 1
+            if non_local.counter < 3:
+                raise ValueError('this')
+
+            return val
+
+        a_signal.connect(succeeds_eventually, sender=self, retry=True)
+        try:
+            result = a_signal.send(sender=self, val='test')
+            assert non_local.counter == 3
+            assert result[0][1] == 'test'
+        finally:
+            a_signal.disconnect(succeeds_eventually, sender=self)
+        self._testIsClean(a_signal)
+
+    def test_retry_with_dispatch_uid(self):
+        uid = 'abc123'
+        a_signal.connect(receiver_1_arg, sender=self, retry=True,
+                         dispatch_uid=uid)
+        assert a_signal.receivers[0][0][0] == uid
+        a_signal.disconnect(receiver_1_arg, sender=self, dispatch_uid=uid)
+        self._testIsClean(a_signal)
+
+    def test_boundmethod(self):
+        a = Callable()
+        a_signal.connect(a.a, sender=self)
+        expected = [(a.a, 'test')]
+        garbage_collect()
+        result = a_signal.send(sender=self, val='test')
+        assert result == expected
+        del a, result, expected
+        garbage_collect()
+        self._testIsClean(a_signal)
+
+    def test_deco_no_arg(self):
+        class non_local:
+            counter = 1
+
+        @a_signal.connect
+        def f(val, **kwargs):
+            non_local.counter += 1
+            return val
+
+        try:
+            result = a_signal.send(sender=None, val='test')
+            assert non_local.counter == 2
+            assert result[0][1] == 'test'
+        finally:
+            a_signal.disconnect(f, sender=None)
+        self._testIsClean(a_signal)
+
+
+class test_AsyncSignal(AsyncTest):
+    def _testIsClean(self, signal):
+        """Assert that everything has been cleaned up automatically"""
+        assert not signal.has_listeners()
+        assert signal.areceivers == []
+
+    async def test_exact(self):
+        a_signal.connect(async_receiver_1_arg, sender=self)
+        try:
+            expected = [(async_receiver_1_arg, 'test')]
+            result = await a_signal.asend(sender=self, val='test')
+            assert result == expected
+        finally:
+            a_signal.disconnect(async_receiver_1_arg, sender=self)
+        self._testIsClean(a_signal)
+
+    async def test_ignored_sender(self):
+        a_signal.connect(async_receiver_1_arg)
+        try:
+            expected = [(async_receiver_1_arg, 'test')]
+            result = await a_signal.asend(sender=self, val='test')
+            assert result == expected
+        finally:
+            a_signal.disconnect(async_receiver_1_arg)
+        self._testIsClean(a_signal)
+
+    async def test_garbage_collected(self):
+        a = AsyncCallable()
+        a_signal.connect(a.a, sender=self)
+        expected = []
+        del a
+        garbage_collect()
+        result = await a_signal.asend(sender=self, val='test')
+        assert result == expected
+        self._testIsClean(a_signal)
+
+    async def test_multiple_registration(self):
+        a = AsyncCallable()
+        result = None
+        try:
+            a_signal.connect(a)
+            a_signal.connect(a)
+            a_signal.connect(a)
+            a_signal.connect(a)
+            a_signal.connect(a)
+            a_signal.connect(a)
+            result = await a_signal.asend(sender=self, val='test')
+            assert len(result) == 1
+            assert len(a_signal.areceivers) == 1
+        finally:
+            del a
+            del result
+            garbage_collect()
+            self._testIsClean(a_signal)
+
+    async def test_uid_registration(self):
+
+        async def uid_based_receiver_1(**kwargs):
+            pass
+
+        async def uid_based_receiver_2(**kwargs):
+            pass
+
+        a_signal.connect(uid_based_receiver_1, dispatch_uid='uid')
+        try:
+            a_signal.connect(uid_based_receiver_2, dispatch_uid='uid')
+            assert len(a_signal.areceivers) == 1
+        finally:
+            a_signal.disconnect(dispatch_uid='uid')
+        self._testIsClean(a_signal)
+
+    async def test_robust(self):
+
+        async def fails(val, **kwargs):
+            raise ValueError('this')
+
+        a_signal.connect(fails)
+        try:
+            await a_signal.asend(sender=self, val='test')
+        finally:
+            a_signal.disconnect(fails)
+        self._testIsClean(a_signal)
+
+    async def test_disconnection(self):
+        receiver_1 = AsyncCallable()
+        receiver_2 = AsyncCallable()
+        receiver_3 = AsyncCallable()
+        try:
+            try:
+                a_signal.connect(receiver_1)
+                a_signal.connect(receiver_2)
+                a_signal.connect(receiver_3)
+            finally:
+                a_signal.disconnect(receiver_1)
+            del receiver_2
+            garbage_collect()
+        finally:
+            a_signal.disconnect(receiver_3)
+        self._testIsClean(a_signal)
+
+    async def test_retry(self):
+
+        class non_local:
+            counter = 1
+
+        async def succeeds_eventually(val, **kwargs):
+            non_local.counter += 1
+            if non_local.counter < 3:
+                raise ValueError('this')
+
+            return val
+
+        a_signal.connect(succeeds_eventually, sender=self, retry=True)
+        try:
+            result = await a_signal.asend(sender=self, val='test')
+            assert non_local.counter == 3
+            assert result[0][1] == 'test'
+        finally:
+            a_signal.disconnect(succeeds_eventually, sender=self)
+        self._testIsClean(a_signal)
+
+    async def test_retry_with_dispatch_uid(self):
+        uid = 'abc123'
+        a_signal.connect(async_receiver_1_arg, sender=self, retry=True,
+                         dispatch_uid=uid)
+        assert a_signal.areceivers[0][0][0] == uid
+        a_signal.disconnect(async_receiver_1_arg, sender=self, dispatch_uid=uid)
+        self._testIsClean(a_signal)
+
+    async def test_boundmethod(self):
+        a = AsyncCallable()
+        a_signal.connect(a.a, sender=self)
+        expected = [(a.a, 'test')]
+        garbage_collect()
+        result = await a_signal.asend(sender=self, val='test')
+        assert result == expected
+        del a, result, expected
+        garbage_collect()
+        self._testIsClean(a_signal)
+
+    async def test_deco_no_arg(self):
+        class non_local:
+            counter = 1
+
+        @a_signal.connect
+        async def f(val, **kwargs):
+            non_local.counter += 1
+            return val
+
+        try:
+            result = await a_signal.asend(sender=None, val='test')
+            assert non_local.counter == 2
+            assert result[0][1] == 'test'
+        finally:
+            a_signal.disconnect(f, sender=None)
+        self._testIsClean(a_signal)
+
+    async def test_retry_on_async_callable(self):
+        class non_local:
+            counter = 1
+
+        class ARetry:
+            async def __call__(self, val, **kwargs):
+                non_local.counter += 1
+                if non_local.counter < 3:
+                    raise ValueError('this')
+
+                return val
+
+        succeeds_eventually = ARetry()
+
+        a_signal.connect(succeeds_eventually, sender=self, retry=True)
+        try:
+            result = await a_signal.asend(sender=self, val='test')
+            assert non_local.counter == 3
+            assert result[0][1] == 'test'
+        finally:
+            a_signal.disconnect(succeeds_eventually, sender=self)
+        self._testIsClean(a_signal)
```

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_functional.py` & `deepfos-celery-1.0.3/t/unit/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_graph.py` & `deepfos-celery-1.0.3/t/unit/utils/test_graph.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_imports.py` & `deepfos-celery-1.0.3/t/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_local.py` & `deepfos-celery-1.0.3/t/unit/utils/test_local.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_pickle.py` & `deepfos-celery-1.0.3/t/unit/utils/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_platforms.py` & `deepfos-celery-1.0.3/t/unit/utils/test_platforms.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_saferepr.py` & `deepfos-celery-1.0.3/t/unit/utils/test_saferepr.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_serialization.py` & `deepfos-celery-1.0.3/t/unit/utils/test_serialization.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_sysinfo.py` & `deepfos-celery-1.0.3/t/unit/utils/test_sysinfo.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_term.py` & `deepfos-celery-1.0.3/t/unit/utils/test_term.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_text.py` & `deepfos-celery-1.0.3/t/unit/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_threads.py` & `deepfos-celery-1.0.3/t/unit/utils/test_threads.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_time.py` & `deepfos-celery-1.0.3/t/unit/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_timer2.py` & `deepfos-celery-1.0.3/t/unit/utils/test_timer2.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/utils/test_utils.py` & `deepfos-celery-1.0.3/t/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_autoscale.py` & `deepfos-celery-1.0.3/t/unit/worker/test_autoscale.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_bootsteps.py` & `deepfos-celery-1.0.3/t/unit/worker/test_bootsteps.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_components.py` & `deepfos-celery-1.0.3/t/unit/worker/test_components.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_consumer.py` & `deepfos-celery-1.0.3/t/unit/worker/test_consumer.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_control.py` & `deepfos-celery-1.0.3/t/unit/worker/test_control.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_heartbeat.py` & `deepfos-celery-1.0.3/t/unit/worker/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_loops.py` & `deepfos-celery-1.0.3/t/unit/worker/test_loops.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_request.py` & `deepfos-celery-1.0.3/t/unit/worker/test_request.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_state.py` & `deepfos-celery-1.0.3/t/unit/worker/test_state.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_strategy.py` & `deepfos-celery-1.0.3/t/unit/worker/test_strategy.py`

 * *Files identical despite different names*

### Comparing `deepfos-celery-1.0.2/t/unit/worker/test_worker.py` & `deepfos-celery-1.0.3/t/unit/worker/test_worker.py`

 * *Files identical despite different names*

