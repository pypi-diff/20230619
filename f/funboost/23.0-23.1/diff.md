# Comparing `tmp/funboost-23.0-py3-none-any.whl.zip` & `tmp/funboost-23.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 1903446 bytes, number of entries: 235
--rw-rw-rw-  2.0 fat     2154 b- defN 23-Jun-05 10:48 funboost/__init__.py
--rw-rw-rw-  2.0 fat    20378 b- defN 23-Jun-05 04:48 funboost/__init__0000.py
--rw-rw-rw-  2.0 fat     6154 b- defN 23-May-24 10:24 funboost/constant.py
+Zip file size: 1910762 bytes, number of entries: 242
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-13 01:20 funboost/__init__.py
+-rw-rw-rw-  2.0 fat    20378 b- defN 23-Jun-13 01:20 funboost/__init__old.py
+-rw-rw-rw-  2.0 fat     6223 b- defN 23-Jun-09 01:42 funboost/constant.py
 -rw-rw-rw-  2.0 fat     7358 b- defN 23-Jun-05 04:48 funboost/funboost_config_deafult.py
 -rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-13 09:47 funboost/set_frame_config.py
--rw-rw-rw-  2.0 fat     3987 b- defN 23-May-17 08:56 funboost/assist/celery_helper.py
+-rw-rw-rw-  2.0 fat     4186 b- defN 23-Jun-19 02:19 funboost/assist/celery_helper.py
 -rw-rw-rw-  2.0 fat     2089 b- defN 23-May-22 01:31 funboost/assist/dramatiq_helper.py
 -rw-rw-rw-  2.0 fat     1760 b- defN 23-May-24 11:10 funboost/assist/huey_helper.py
+-rw-rw-rw-  2.0 fat     1509 b- defN 23-Jun-09 03:23 funboost/assist/rq_helper.py
+-rw-rw-rw-  2.0 fat     4831 b- defN 23-Jun-09 01:42 funboost/assist/rq_windows_worker.py
 -rw-rw-rw-  2.0 fat     3930 b- defN 22-Sep-17 06:12 funboost/beggar_version_implementation/beggar_redis_consumer.py
 -rw-rw-rw-  2.0 fat      759 b- defN 22-Dec-19 11:45 funboost/concurrent_pool/__init__.py
 -rw-rw-rw-  2.0 fat     3256 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/async_helper.py
 -rw-rw-rw-  2.0 fat     7227 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/async_pool_executor.py
 -rw-rw-rw-  2.0 fat     4723 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py
 -rw-rw-rw-  2.0 fat     3011 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_processpoolexcutor_py36.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_threadpoolexcutor.py
@@ -21,25 +23,25 @@
 -rw-rw-rw-  2.0 fat     9317 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/custom_threadpool_executor000.py
 -rw-rw-rw-  2.0 fat      373 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/single_thread_executor.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-24 11:39 funboost/concurrent_pool/backup/__init__.py
 -rw-rw-rw-  2.0 fat     9548 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor0223.py
 -rw-rw-rw-  2.0 fat     9568 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_back.py
 -rw-rw-rw-  2.0 fat     5728 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_janus.py
 -rw-rw-rw-  2.0 fat      126 b- defN 22-Sep-17 06:12 funboost/consumers/__init__.py
--rw-rw-rw-  2.0 fat    83054 b- defN 23-Jun-05 04:48 funboost/consumers/base_consumer.py
+-rw-rw-rw-  2.0 fat    82870 b- defN 23-Jun-19 02:19 funboost/consumers/base_consumer.py
 -rw-rw-rw-  2.0 fat     7574 b- defN 23-Jun-06 01:47 funboost/consumers/celery_consumer.py
 -rw-rw-rw-  2.0 fat     4574 b- defN 23-May-04 06:09 funboost/consumers/celery_consumer000.py
 -rw-rw-rw-  2.0 fat     5877 b- defN 23-Mar-29 02:19 funboost/consumers/confirm_mixin.py
 -rw-rw-rw-  2.0 fat     2144 b- defN 23-May-23 07:08 funboost/consumers/dramatiq_consumer.py
 -rw-rw-rw-  2.0 fat     2025 b- defN 23-May-15 01:33 funboost/consumers/http_consumer.py
 -rw-rw-rw-  2.0 fat     4463 b- defN 22-Sep-17 06:12 funboost/consumers/http_consumer000.py
 -rw-rw-rw-  2.0 fat     1080 b- defN 23-May-04 12:12 funboost/consumers/httpsqs_consumer.py
 -rw-rw-rw-  2.0 fat     1856 b- defN 23-May-24 11:08 funboost/consumers/huey_consumer.py
 -rw-rw-rw-  2.0 fat     4217 b- defN 23-May-04 12:12 funboost/consumers/kafka_consumer.py
--rw-rw-rw-  2.0 fat     6556 b- defN 23-May-04 12:12 funboost/consumers/kafka_consumer_manually_commit.py
+-rw-rw-rw-  2.0 fat     6947 b- defN 23-Jun-09 09:53 funboost/consumers/kafka_consumer_manually_commit.py
 -rw-rw-rw-  2.0 fat    10186 b- defN 23-May-12 08:42 funboost/consumers/kombu_consumer.py
 -rw-rw-rw-  2.0 fat     1291 b- defN 23-May-04 12:12 funboost/consumers/local_python_queue_consumer.py
 -rw-rw-rw-  2.0 fat     1090 b- defN 23-May-04 12:12 funboost/consumers/mongomq_consumer.py
 -rw-rw-rw-  2.0 fat     2228 b- defN 23-May-04 12:12 funboost/consumers/mqtt_consumer.py
 -rw-rw-rw-  2.0 fat     2183 b- defN 23-May-04 12:12 funboost/consumers/nameko_consumer.py
 -rw-rw-rw-  2.0 fat     1076 b- defN 23-May-04 12:12 funboost/consumers/nats_consumer.py
 -rw-rw-rw-  2.0 fat     1461 b- defN 23-May-18 03:26 funboost/consumers/nsq_consumer.py
@@ -54,36 +56,37 @@
 -rw-rw-rw-  2.0 fat     2829 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer.py
 -rw-rw-rw-  2.0 fat     7545 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer_ack_able.py
 -rw-rw-rw-  2.0 fat      922 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer_simple.py
 -rw-rw-rw-  2.0 fat     7135 b- defN 22-Sep-17 06:12 funboost/consumers/redis_filter.py
 -rw-rw-rw-  2.0 fat     1206 b- defN 23-May-04 12:12 funboost/consumers/redis_pubsub_consumer.py
 -rw-rw-rw-  2.0 fat     6497 b- defN 23-May-25 02:22 funboost/consumers/redis_stream_consumer.py
 -rw-rw-rw-  2.0 fat     1653 b- defN 23-May-04 12:12 funboost/consumers/rocketmq_consumer.py
+-rw-rw-rw-  2.0 fat      876 b- defN 23-Jun-08 11:07 funboost/consumers/rq_consumer.py
 -rw-rw-rw-  2.0 fat     1309 b- defN 23-May-04 12:12 funboost/consumers/sqlachemy_consumer.py
 -rw-rw-rw-  2.0 fat     2045 b- defN 23-May-04 12:12 funboost/consumers/tcp_consumer.py
 -rw-rw-rw-  2.0 fat     1340 b- defN 23-May-04 12:12 funboost/consumers/txt_file_consumer.py
 -rw-rw-rw-  2.0 fat     1643 b- defN 23-May-04 12:12 funboost/consumers/udp_consumer.py
 -rw-rw-rw-  2.0 fat     4157 b- defN 23-May-04 12:12 funboost/consumers/zeromq_consumer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-05 10:31 funboost/contrib/__init__.py
 -rw-rw-rw-  2.0 fat     4680 b- defN 23-May-15 08:24 funboost/contrib/queue2queue.py
 -rw-rw-rw-  2.0 fat     1817 b- defN 23-Mar-22 02:09 funboost/contrib/redis_consume_latest_msg_broker.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 04:48 funboost/core/__init__.py
 -rw-rw-rw-  2.0 fat     4984 b- defN 23-Jun-05 04:48 funboost/core/active_cousumer_info_getter.py
--rw-rw-rw-  2.0 fat    16419 b- defN 23-Jun-06 02:26 funboost/core/booster.py
--rw-rw-rw-  2.0 fat      421 b- defN 23-Jun-05 04:48 funboost/core/exit_signal.py
+-rw-rw-rw-  2.0 fat    16372 b- defN 23-Jun-08 02:26 funboost/core/booster.py
+-rw-rw-rw-  2.0 fat      576 b- defN 23-Jun-13 01:20 funboost/core/exit_signal.py
 -rw-rw-rw-  2.0 fat     8875 b- defN 23-Jun-05 04:48 funboost/core/fabric_deploy_helper.py
 -rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-05 04:48 funboost/core/function_result_status_config.py
 -rw-rw-rw-  2.0 fat     8819 b- defN 23-Jun-05 04:48 funboost/core/function_result_status_saver.py
--rw-rw-rw-  2.0 fat     1299 b- defN 23-Jun-06 02:26 funboost/core/get_booster.py
--rw-rw-rw-  2.0 fat      168 b- defN 23-Jun-05 04:48 funboost/core/global_boosters.py
--rw-rw-rw-  2.0 fat      604 b- defN 23-Jun-05 04:48 funboost/core/helper_funs.py
+-rw-rw-rw-  2.0 fat     1169 b- defN 23-Jun-08 03:26 funboost/core/get_booster.py
+-rw-rw-rw-  2.0 fat      340 b- defN 23-Jun-08 02:52 funboost/core/global_boosters.py
+-rw-rw-rw-  2.0 fat     1193 b- defN 23-Jun-12 01:35 funboost/core/helper_funs.py
 -rw-rw-rw-  2.0 fat     7782 b- defN 23-Jun-05 04:48 funboost/core/msg_result_getter.py
--rw-rw-rw-  2.0 fat     3766 b- defN 23-Jun-05 11:19 funboost/core/muliti_process_enhance.py
+-rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-08 03:05 funboost/core/muliti_process_enhance.py
 -rw-rw-rw-  2.0 fat      178 b- defN 22-Sep-17 06:12 funboost/factories/__init__.py
--rw-rw-rw-  2.0 fat     8420 b- defN 23-May-31 01:38 funboost/factories/broker_kind__publsiher_consumer_type_map.py
+-rw-rw-rw-  2.0 fat     8738 b- defN 23-Jun-09 03:28 funboost/factories/broker_kind__publsiher_consumer_type_map.py
 -rw-rw-rw-  2.0 fat      946 b- defN 23-May-29 03:09 funboost/factories/consumer_factory.py
 -rw-rw-rw-  2.0 fat     2281 b- defN 23-May-29 03:09 funboost/factories/publisher_factotry.py
 -rw-rw-rw-  2.0 fat     4841 b- defN 22-Sep-17 06:12 funboost/function_result_web/app.py
 -rw-rw-rw-  2.0 fat     7345 b- defN 23-Mar-08 10:19 funboost/function_result_web/functions.py
 -rw-rw-rw-  2.0 fat     4045 b- defN 22-Feb-21 07:34 funboost/function_result_web/__pycache__/app.cpython-37.pyc
 -rw-rw-rw-  2.0 fat     3921 b- defN 22-Mar-30 13:56 funboost/function_result_web/__pycache__/functions.cpython-37.pyc
 -rw-rw-rw-  2.0 fat     7674 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/css/custom.css
@@ -96,16 +99,16 @@
 -rw-rw-rw-  2.0 fat      546 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/password.png
 -rw-rw-rw-  2.0 fat     2912 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/tick.png
 -rw-rw-rw-  2.0 fat      622 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/user.png
 -rw-rw-rw-  2.0 fat    96383 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/js/jquery-1.11.0.min.js
 -rw-rw-rw-  2.0 fat    19501 b- defN 22-Feb-21 12:32 funboost/function_result_web/templates/index.html
 -rw-rw-rw-  2.0 fat     2007 b- defN 21-Dec-27 01:40 funboost/function_result_web/templates/login.html
 -rw-rw-rw-  2.0 fat      131 b- defN 22-Sep-17 06:12 funboost/publishers/__init__.py
--rw-rw-rw-  2.0 fat    15047 b- defN 23-Jun-05 04:48 funboost/publishers/base_publisher.py
--rw-rw-rw-  2.0 fat     3724 b- defN 23-May-15 01:33 funboost/publishers/celery_publisher.py
+-rw-rw-rw-  2.0 fat    15148 b- defN 23-Jun-08 03:14 funboost/publishers/base_publisher.py
+-rw-rw-rw-  2.0 fat     3755 b- defN 23-Jun-16 11:28 funboost/publishers/celery_publisher.py
 -rw-rw-rw-  2.0 fat     3897 b- defN 23-May-04 06:09 funboost/publishers/celery_publisher000.py
 -rw-rw-rw-  2.0 fat     3541 b- defN 23-Mar-23 05:32 funboost/publishers/confluent_kafka_publisher.py
 -rw-rw-rw-  2.0 fat     1410 b- defN 23-May-22 01:23 funboost/publishers/dramatiq_publisher.py
 -rw-rw-rw-  2.0 fat      753 b- defN 23-May-04 11:53 funboost/publishers/http_publisher.py
 -rw-rw-rw-  2.0 fat     2783 b- defN 22-Sep-17 06:12 funboost/publishers/httpsqs_publisher.py
 -rw-rw-rw-  2.0 fat     1101 b- defN 23-May-24 11:08 funboost/publishers/huey_publisher.py
 -rw-rw-rw-  2.0 fat     2160 b- defN 23-Apr-03 10:55 funboost/publishers/kafka_publisher.py
@@ -124,42 +127,44 @@
 -rw-rw-rw-  2.0 fat     1953 b- defN 22-Sep-17 06:12 funboost/publishers/rabbitmq_rabbitpy_publisher.py
 -rw-rw-rw-  2.0 fat     3982 b- defN 23-May-10 03:22 funboost/publishers/redis_publisher.py
 -rw-rw-rw-  2.0 fat      278 b- defN 22-Sep-17 06:12 funboost/publishers/redis_publisher_lpush.py
 -rw-rw-rw-  2.0 fat      872 b- defN 23-Apr-28 03:12 funboost/publishers/redis_publisher_simple.py
 -rw-rw-rw-  2.0 fat      721 b- defN 22-Sep-17 06:12 funboost/publishers/redis_pubsub_publisher.py
 -rw-rw-rw-  2.0 fat     2037 b- defN 21-Dec-27 01:40 funboost/publishers/redis_stream_publisher.py
 -rw-rw-rw-  2.0 fat     2343 b- defN 23-Mar-23 05:32 funboost/publishers/rocketmq_publisher.py
+-rw-rw-rw-  2.0 fat      893 b- defN 23-Jun-13 01:20 funboost/publishers/rq_publisher.py
 -rw-rw-rw-  2.0 fat     1215 b- defN 22-Sep-17 06:12 funboost/publishers/sqla_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1335 b- defN 23-May-10 08:53 funboost/publishers/tcp_publisher.py
 -rw-rw-rw-  2.0 fat     1380 b- defN 22-Sep-17 08:52 funboost/publishers/txt_file_publisher.py
 -rw-rw-rw-  2.0 fat     1194 b- defN 23-May-04 11:53 funboost/publishers/udp_publisher.py
 -rw-rw-rw-  2.0 fat     1002 b- defN 21-Dec-27 01:40 funboost/publishers/zeromq_publisher.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-22 02:44 funboost/queues/__init__.py
 -rw-rw-rw-  2.0 fat     4944 b- defN 23-May-22 04:27 funboost/queues/peewee_queue.py
 -rw-rw-rw-  2.0 fat    11024 b- defN 23-May-05 02:38 funboost/queues/sqla_queue.py
--rw-rw-rw-  2.0 fat     7919 b- defN 23-Jun-05 04:56 funboost/timing_job/__init__.py
+-rw-rw-rw-  2.0 fat     8267 b- defN 23-Jun-13 01:20 funboost/timing_job/__init__.py
 -rw-rw-rw-  2.0 fat      418 b- defN 23-Apr-06 06:09 funboost/timing_job/apscheduler_use_mysql_store.py
 -rw-rw-rw-  2.0 fat      876 b- defN 23-May-30 09:38 funboost/timing_job/apscheduler_use_redis_store.py
 -rw-rw-rw-  2.0 fat     1951 b- defN 23-Mar-09 07:27 funboost/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3124 b- defN 21-Dec-27 01:40 funboost/utils/apscheduler_monkey.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Jan-29 07:41 funboost/utils/block_exit.py
 -rw-rw-rw-  2.0 fat     9972 b- defN 22-Apr-01 02:17 funboost/utils/bulk_operation.py
 -rw-rw-rw-  2.0 fat     5923 b- defN 21-Dec-27 01:40 funboost/utils/custom_pysnooper.py
--rw-rw-rw-  2.0 fat    24284 b- defN 23-Mar-23 05:32 funboost/utils/decorators.py
+-rw-rw-rw-  2.0 fat    24296 b- defN 23-Jun-13 01:20 funboost/utils/decorators.py
 -rw-rw-rw-  2.0 fat      251 b- defN 21-Dec-27 01:40 funboost/utils/develop_log.py
+-rw-rw-rw-  2.0 fat     2837 b- defN 23-Jun-19 02:19 funboost/utils/kill_thread.py
 -rw-rw-rw-  2.0 fat     2984 b- defN 23-Apr-07 02:11 funboost/utils/mongo_util.py
 -rw-rw-rw-  2.0 fat     7367 b- defN 23-Mar-23 05:34 funboost/utils/monkey_color_log.py
 -rw-rw-rw-  2.0 fat     2882 b- defN 23-Feb-23 05:04 funboost/utils/monkey_patches.py
 -rw-rw-rw-  2.0 fat     3199 b- defN 21-Dec-27 01:40 funboost/utils/mqtt_util.py
 -rw-rw-rw-  2.0 fat     4901 b- defN 21-Dec-27 01:40 funboost/utils/paramiko_util.py
 -rw-rw-rw-  2.0 fat     2963 b- defN 22-Sep-17 06:12 funboost/utils/rabbitmq_factory.py
 -rw-rw-rw-  2.0 fat     4628 b- defN 23-May-12 03:14 funboost/utils/redis_manager.py
 -rw-rw-rw-  2.0 fat     5532 b- defN 22-Sep-17 06:12 funboost/utils/resource_monitoring.py
 -rw-rw-rw-  2.0 fat     1418 b- defN 23-Mar-15 02:41 funboost/utils/restart_python.py
--rw-rw-rw-  2.0 fat     2985 b- defN 23-Jan-29 07:39 funboost/utils/show_funboost_flag.py
+-rw-rw-rw-  2.0 fat     2985 b- defN 23-Jun-19 02:19 funboost/utils/show_funboost_flag.py
 -rw-rw-rw-  2.0 fat     1204 b- defN 22-Dec-12 08:11 funboost/utils/simple_data_class.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 21-Dec-27 01:40 funboost/utils/time_util.py
 -rw-rw-rw-  2.0 fat      408 b- defN 22-Jan-17 01:57 funboost/utils/un_strict_json_dumps.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Dec-27 01:40 funboost/utils/dependency_packages/__init__.py
 -rw-rw-rw-  2.0 fat      131 b- defN 21-Dec-27 01:40 funboost/utils/dependency_packages/mongomq/__init__.py
 -rw-rw-rw-  2.0 fat     2486 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/lock.py
 -rw-rw-rw-  2.0 fat     7902 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/mongomq.py
@@ -225,13 +230,15 @@
 -rw-rw-rw-  2.0 fat      303 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc
 -rw-rw-rw-  2.0 fat      311 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc
 -rw-rw-rw-  2.0 fat      909 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/__init__.py
 -rw-rw-rw-  2.0 fat     2243 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/pycompat.py
 -rw-rw-rw-  2.0 fat    19131 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/tracer.py
 -rw-rw-rw-  2.0 fat     2753 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/utils.py
 -rw-rw-rw-  2.0 fat     3693 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/variables.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    26423 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    25590 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/RECORD
-235 files, 3277831 bytes uncompressed, 1861004 bytes compressed:  43.2%
+-rw-rw-rw-  2.0 fat     2417 b- defN 23-Jun-09 01:42 funboost/utils/times/__init__.py
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-09 01:42 funboost/utils/times/version.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    26616 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    26209 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/RECORD
+242 files, 3294282 bytes uncompressed, 1867342 bytes compressed:  43.3%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: funboost/__init__.py
 Comment: 
 
-Filename: funboost/__init__0000.py
+Filename: funboost/__init__old.py
 Comment: 
 
 Filename: funboost/constant.py
 Comment: 
 
 Filename: funboost/funboost_config_deafult.py
 Comment: 
@@ -18,14 +18,20 @@
 
 Filename: funboost/assist/dramatiq_helper.py
 Comment: 
 
 Filename: funboost/assist/huey_helper.py
 Comment: 
 
+Filename: funboost/assist/rq_helper.py
+Comment: 
+
+Filename: funboost/assist/rq_windows_worker.py
+Comment: 
+
 Filename: funboost/beggar_version_implementation/beggar_redis_consumer.py
 Comment: 
 
 Filename: funboost/concurrent_pool/__init__.py
 Comment: 
 
 Filename: funboost/concurrent_pool/async_helper.py
@@ -171,14 +177,17 @@
 
 Filename: funboost/consumers/redis_stream_consumer.py
 Comment: 
 
 Filename: funboost/consumers/rocketmq_consumer.py
 Comment: 
 
+Filename: funboost/consumers/rq_consumer.py
+Comment: 
+
 Filename: funboost/consumers/sqlachemy_consumer.py
 Comment: 
 
 Filename: funboost/consumers/tcp_consumer.py
 Comment: 
 
 Filename: funboost/consumers/txt_file_consumer.py
@@ -381,14 +390,17 @@
 
 Filename: funboost/publishers/redis_stream_publisher.py
 Comment: 
 
 Filename: funboost/publishers/rocketmq_publisher.py
 Comment: 
 
+Filename: funboost/publishers/rq_publisher.py
+Comment: 
+
 Filename: funboost/publishers/sqla_queue_publisher.py
 Comment: 
 
 Filename: funboost/publishers/tcp_publisher.py
 Comment: 
 
 Filename: funboost/publishers/txt_file_publisher.py
@@ -435,14 +447,17 @@
 
 Filename: funboost/utils/decorators.py
 Comment: 
 
 Filename: funboost/utils/develop_log.py
 Comment: 
 
+Filename: funboost/utils/kill_thread.py
+Comment: 
+
 Filename: funboost/utils/mongo_util.py
 Comment: 
 
 Filename: funboost/utils/monkey_color_log.py
 Comment: 
 
 Filename: funboost/utils/monkey_patches.py
@@ -684,23 +699,29 @@
 
 Filename: funboost/utils/pysnooper_ydf/utils.py
 Comment: 
 
 Filename: funboost/utils/pysnooper_ydf/variables.py
 Comment: 
 
-Filename: funboost-23.0.dist-info/LICENSE
+Filename: funboost/utils/times/__init__.py
+Comment: 
+
+Filename: funboost/utils/times/version.py
+Comment: 
+
+Filename: funboost-23.1.dist-info/LICENSE
 Comment: 
 
-Filename: funboost-23.0.dist-info/METADATA
+Filename: funboost-23.1.dist-info/METADATA
 Comment: 
 
-Filename: funboost-23.0.dist-info/WHEEL
+Filename: funboost-23.1.dist-info/WHEEL
 Comment: 
 
-Filename: funboost-23.0.dist-info/top_level.txt
+Filename: funboost-23.1.dist-info/top_level.txt
 Comment: 
 
-Filename: funboost-23.0.dist-info/RECORD
+Filename: funboost-23.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funboost/__init__.py

```diff
@@ -1,9 +1,9 @@
 # noinspection PyUnresolvedReferences
-from funboost.utils.dependency_packages_in_pythonpath import add_to_pythonpath
+from funboost.utils.dependency_packages_in_pythonpath import add_to_pythonpath # 这是把 dependency_packages_in_pythonpath 添加到 PYTHONPATH了。
 
 from funboost.utils import monkey_patches
 from funboost.utils import show_funboost_flag
 
 # noinspection PyUnresolvedReferences
 import nb_log
 from funboost.set_frame_config import patch_frame_config, show_frame_config
@@ -28,11 +28,14 @@
 
 from funboost.timing_job import fsdf_background_scheduler, timing_publish_deco, funboost_aps_scheduler
 from funboost.constant import BrokerEnum, ConcurrentModeEnum
 
 from funboost.core.booster import boost, Booster
 from funboost.core.get_booster import get_booster
 
-from funboost.core import exit_signal
+from funboost.core.exit_signal import set_interrupt_signal_handler
+from funboost.core.helper_funs import run_forever
 
 # 有的包默认没加handlers，原始的日志不漂亮且不可跳转不知道哪里发生的。这里把warnning级别以上的日志默认加上handlers。
 # nb_log.get_logger(name='', log_level_int=30, log_filename='pywarning.log')
+
+set_interrupt_signal_handler()
```

## funboost/constant.py

```diff
@@ -68,14 +68,17 @@
     REDIS_PUBSUB = 27  # 基于redis 发布订阅的，发布一个消息多个消费者都能收到消息，但不支持持久化
 
     CELERY = 30  # funboost支持celery框架来发布和消费任务，由celery框架来调度执行任务，但是写法简单暴击celery，永无无需关心和操作Celery对象实例。
 
     DRAMATIQ = 31 # funboost使用 dramatiq 框架作为消息队列，dramatiq类似celery也是任务队列框架。用户使用funboost api来操作dramatiq核心调度。
 
     HUEY = 32 # huey任务队列框架作为funboost调度核心
+
+    RQ = 33  # huey任务队列框架作为funboost调度核心
+
     NAMEKO = 40  # funboost支持python微服务框架nameko，用户无需掌握nameko api语法，就玩转python nameko微服务
 
 
 class ConcurrentModeEnum:
     THREADING = 1
     GEVENT = 2
     EVENTLET = 3
```

## funboost/assist/celery_helper.py

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import os
 import sys
 import threading
 from functools import partial
 
 import celery
@@ -33,16 +34,19 @@
         :return:
         """
         celery_app.conf.update(celery_app_conf)
 
     @staticmethod
     def show_celery_app_conf():
         logger.debug('展示celery app的配置')
+        conf_dict_json_able = {}
         for k, v in celery_app.conf.items():
-            print(k, ' : ', v)
+            conf_dict_json_able[k] = str(v)
+            # print(k, ' : ', v)
+        print('celery app 的配置是：',json.dumps(conf_dict_json_able,ensure_ascii=False,indent=4))
 
     @staticmethod
     def celery_start_beat(beat_schedule: dict):
         celery_app.conf.beat_schedule = beat_schedule  # 配置celery定时任务
 
         def _f():
             beat = partial(celery_app.Beat, loglevel='INFO', )
```

## funboost/consumers/base_consumer.py

```diff
@@ -11,17 +11,15 @@
 from pathlib import Path
 # from multiprocessing import Process
 import datetime
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 import pytz
 import json
 import logging
-import sys
 import atexit
-import socket
 import os
 import uuid
 import time
 import traceback
 # from collections import Callable
 from typing import Callable
 from functools import wraps
@@ -29,27 +27,23 @@
 from threading import Lock, Thread
 import gevent
 import asyncio
 
 from apscheduler.jobstores.redis import RedisJobStore
 from apscheduler.executors.pool import ThreadPoolExecutor as ApschedulerThreadPoolExecutor
 
-import pymongo
-from pymongo import IndexModel, ReplaceOne
-from pymongo.errors import PyMongoError
-
 import nb_log
 from funboost.concurrent_pool.single_thread_executor import SoloExecutor
 from funboost.core.function_result_status_saver import FunctionResultStatusPersistanceConfig, ResultPersistenceHelper, FunctionResultStatus
 
 # noinspection PyUnresolvedReferences
 from funboost.core.helper_funs import _delete_keys_and_return_new_dict, get_publish_time
-from nb_log import get_logger, LoggerLevelSetterMixin, LogManager, nb_print, LoggerMixin, \
-    LoggerMixinDefaultWithFileHandler, stdout_write, stderr_write, is_main_process, \
-    only_print_on_main_process, nb_log_config_default
+from nb_log import get_logger, LoggerLevelSetterMixin, nb_print, LoggerMixin, \
+    LoggerMixinDefaultWithFileHandler, stdout_write, is_main_process, \
+    nb_log_config_default
 # noinspection PyUnresolvedReferences
 from funboost.concurrent_pool.async_helper import simple_run_in_executor
 from funboost.concurrent_pool.async_pool_executor import AsyncPoolExecutor
 # noinspection PyUnresolvedReferences
 from funboost.concurrent_pool.bounded_threadpoolexcutor import \
     BoundedThreadPoolExecutor
 from func_timeout import func_set_timeout  # noqa
```

## funboost/consumers/kafka_consumer_manually_commit.py

```diff
@@ -1,43 +1,48 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2021/4/18 0008 13:32
 
 
 import json
+import threading
 from collections import defaultdict, OrderedDict
 # noinspection PyPackageRequirements
 import time
 
 # noinspection PyPackageRequirements
 from kafka import KafkaProducer, KafkaAdminClient
 
 # noinspection PyPackageRequirements
 from kafka.admin import NewTopic
 # noinspection PyPackageRequirements
 from kafka.errors import TopicAlreadyExistsError
 from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
+from confluent_kafka.cimpl import TopicPartition
+from confluent_kafka import Consumer as ConfluentConsumer  # 这个包在win下不好安装，用户用这个中间件的时候自己再想办法安装。win用户需要安装c++ 14.0以上环境。
 
 
 class KafkaConsumerManuallyCommit(AbstractConsumer):
     """
     confluent_kafla作为中间件实现的。操作kafka中间件的速度比kafka-python快10倍。
     这个是自动间隔2秒的手动确认，由于是异步在并发池中并发消费，可以防止强制关闭程序造成正在运行的任务丢失，比自动commit好。
     如果使用kafka，推荐这个。
 
     可以让消费函数内部 sleep 60秒，突然停止消费代码，使用 kafka-consumer-groups.sh --bootstrap-server 127.0.0.1:9092 --describe --group frame_group 来证实自动确认消费和手动确认消费的区别。
     """
 
-    BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'group_id':'funboost_confluent_kafka','auto_offset_reset':'earliest'}
+    BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'group_id': 'funboost_confluent_kafka', 'auto_offset_reset': 'earliest'}
+
+    def custom_init(self):
+        self._lock_for_operate_offset_dict = threading.Lock()
 
     def _shedual_task(self):
 
-        from confluent_kafka import Consumer as ConfluentConsumer  # 这个包在win下不好安装，用户用这个中间件的时候自己再想办法安装。win用户需要安装c++ 14.0以上环境。
         try:
             admin_client = KafkaAdminClient(bootstrap_servers=funboost_config_deafult.KAFKA_BOOTSTRAP_SERVERS)
             admin_client.create_topics([NewTopic(self._queue_name, 10, 1)])
             # admin_client.create_partitions({self._queue_name: NewPartitions(total_count=16)})
         except TopicAlreadyExistsError:
             pass
 
@@ -73,45 +78,49 @@
 
             # kw = {'consumer': consumer, 'message': message, 'body': json.loads(message.value)}
             # self._submit_task(kw)
 
     def _manually_commit(self):
         """
         kafka要求消费线程数量和分区数量是一对一或一对多，不能多对一，消息并发处理收到分区数量的限制，这种是支持超高线程数量消费，所以commit非常复杂。
-        因为这种是支持单分区200线程消费，消费本身和拉取kafka任务不在同一个线程，而且可能offset较大的比offset较小的任务先完成，
+        因为这种是可以支持单分区200线程消费，消费本身和拉取kafka任务不在同一个线程，而且可能offset较大的比offset较小的任务先完成，
         每隔2秒对1组offset，对连续消费状态是1的最大offset进行commit
         :return:
         """
-        from confluent_kafka.cimpl import TopicPartition  # 这个包不好安装，用户用这个中间件的时候自己再想办法安装。win用户需要安装c++ 14.0以上环境。
-        if time.time() - self._recent_commit_time > 2:
-            partion_max_consumed_offset_map = dict()
-            to_be_remove_from_partion_max_consumed_offset_map = defaultdict(list)
-            for partion, offset_consume_status in self._partion__offset_consume_status_map.items():
-                max_consumed_offset = 0
-                for offset, consume_status in offset_consume_status.items():
-                    # print(offset,consume_status)
-                    if consume_status == 1:
-                        max_consumed_offset = offset
-                        to_be_remove_from_partion_max_consumed_offset_map[partion].append(offset)
-                    else:
-                        break
-                if max_consumed_offset:
-                    partion_max_consumed_offset_map[partion] = max_consumed_offset
-            # self.logger.info(partion_max_consumed_offset_map)
-            # TopicPartition
-            offsets = list()
-            for partion, max_consumed_offset in partion_max_consumed_offset_map.items():
-                # print(partion,max_consumed_offset)
-                offsets.append(TopicPartition(topic=self._queue_name, partition=partion, offset=max_consumed_offset + 1))
-            if len(offsets):
-                self._confluent_consumer.commit(offsets=offsets, asynchronous=False)
-            self._recent_commit_time = time.time()
-            for partion, offset_list in to_be_remove_from_partion_max_consumed_offset_map.items():
-                for offset in offset_list:
-                    del self._partion__offset_consume_status_map[partion][offset]
+        with self._lock_for_operate_offset_dict:
+            if time.time() - self._recent_commit_time > 2:
+                partion_max_consumed_offset_map = dict()
+                to_be_remove_from_partion_max_consumed_offset_map = defaultdict(list)
+                for partion, offset_consume_status in self._partion__offset_consume_status_map.items():
+                    sorted_keys = sorted(offset_consume_status.keys())
+                    offset_consume_status_ordered = {key: offset_consume_status[key] for key in sorted_keys}
+                    max_consumed_offset = None
+
+                    for offset, consume_status in offset_consume_status_ordered.items():
+                        # print(offset,consume_status)
+                        if consume_status == 1:
+                            max_consumed_offset = offset
+                            to_be_remove_from_partion_max_consumed_offset_map[partion].append(offset)
+                        else:
+                            break
+                    if max_consumed_offset is not None:
+                        partion_max_consumed_offset_map[partion] = max_consumed_offset
+                # self.logger.info(partion_max_consumed_offset_map)
+                # TopicPartition
+                offsets = list()
+                for partion, max_consumed_offset in partion_max_consumed_offset_map.items():
+                    # print(partion,max_consumed_offset)
+                    offsets.append(TopicPartition(topic=self._queue_name, partition=partion, offset=max_consumed_offset + 1))
+                if len(offsets):
+                    self._confluent_consumer.commit(offsets=offsets, asynchronous=False)
+                self._recent_commit_time = time.time()
+                for partion, offset_list in to_be_remove_from_partion_max_consumed_offset_map.items():
+                    for offset in offset_list:
+                        del self._partion__offset_consume_status_map[partion][offset]
 
     def _confirm_consume(self, kw):
-        self._partion__offset_consume_status_map[kw['partition']][kw['offset']] = 1
-        # print(self._partion__offset_consume_status_map)
+        with self._lock_for_operate_offset_dict:
+            self._partion__offset_consume_status_map[kw['partition']][kw['offset']] = 1
+            # print(self._partion__offset_consume_status_map)
 
     def _requeue(self, kw):
         self._producer.send(self._queue_name, json.dumps(kw['body']).encode())
```

## funboost/core/booster.py

```diff
@@ -1,13 +1,11 @@
 import copy
-import functools
 import types
 import typing
-from functools import wraps, partial
-import collections
+from functools import wraps
 
 from funboost.core.function_result_status_config import FunctionResultStatusPersistanceConfig
 
 from funboost.core.global_boosters import regist_booster
 
 from funboost.funboost_config_deafult import BoostDecoratorDefaultParams
```

## funboost/core/exit_signal.py

```diff
@@ -1,12 +1,15 @@
-import signal
 import os
+import signal
+
 
 # noinspection PyProtectedMember,PyUnusedLocal
 def _interrupt_signal_handler(signalx, framex):
     print('你按了 Ctrl+C  。 You pressed Ctrl+C!  结束程序！')
     # sys.exit(0)
     # noinspection PyUnresolvedReferences
     os._exit(0)  # os._exit才能更强力的迅速终止python，sys.exit只能退出主线程。
 
 
-signal.signal(signal.SIGINT, _interrupt_signal_handler)
+def set_interrupt_signal_handler():
+    ''' 有的包里面自己写了 signal.signal，导致这个_interrupt_signal_handler函数不能生效'''
+    signal.signal(signal.SIGINT, _interrupt_signal_handler)
```

## funboost/core/get_booster.py

```diff
@@ -1,33 +1,25 @@
 import os
-
 import typing
-
 from funboost.core.booster import Booster
-from funboost.core.global_boosters import pid_queue_name__booster_map
+from funboost.core.global_boosters import pid_queue_name__booster_map, queue_name__boost_params_consuming_function_map
 
 
 def get_booster(queue_name: str) -> Booster:
     pid = os.getpid()
     if (pid, queue_name) not in pid_queue_name__booster_map:
         err_msg = f'进程 {pid} ，没有 {queue_name} 对应的 booster'
         raise ValueError(err_msg)
     return pid_queue_name__booster_map[(pid, queue_name)]
 
 
-def get_booster_ignore_current_pid(queue_name: str) -> Booster:
+def get_boost_params_and_consuming_function(queue_name: str) -> (dict, typing.Callable):
     """
-    这个函数是为了在别的进程实例化 booster，consumer和publisher,是为了获取queue_name队列对应的booster的当时的入参。
+    这个函数是为了在别的进程实例化 booster，consumer和publisher,获取queue_name队列对应的booster的当时的入参。
     有些中间件python包的对中间件连接对象不是多进程安全的，不要在进程2中去操作进程1中生成的booster consumer publisher等对象。
     """
 
     """
-    _booster = get_booster_ignore_current_pid(queue_name)
-    booster_current_pid = boost(**_booster.boost_params)(_booster.consuming_function)
+    boost_params,consuming_function = get_boost_params_and_consuming_function(queue_name)
+    booster_current_pid = boost(**boost_params)(consuming_function)
     """
-
-    for k, v in pid_queue_name__booster_map.items():
-        if k[1] == queue_name:
-            booster = pid_queue_name__booster_map[k]  # type: Booster
-            return booster
-    err_msg = f'，没有 {queue_name} 对应的 booster'
-    raise ValueError(err_msg)
+    return queue_name__boost_params_consuming_function_map[queue_name]
```

## funboost/core/global_boosters.py

```diff
@@ -1,7 +1,9 @@
 import os
 
 pid_queue_name__booster_map = {}
+queue_name__boost_params_consuming_function_map = {}
 
 
 def regist_booster(queue_name: str, booster):
     pid_queue_name__booster_map[(os.getpid(), queue_name)] = booster
+    queue_name__boost_params_consuming_function_map[queue_name] = (booster.boost_params, booster.consuming_function)
```

## funboost/core/helper_funs.py

```diff
@@ -1,8 +1,9 @@
 import copy
+import time
 
 
 def get_publish_time(paramsx: dict):
     """
     :param paramsx:
     :return:
     """
@@ -13,8 +14,23 @@
     dict_new = copy.copy(dictx)  # 主要是去掉一级键 publish_time，浅拷贝即可。新的消息已经不是这样了。
     keys = ['publish_time', 'publish_time_format', 'extra'] if keys is None else keys
     for dict_key in keys:
         try:
             dict_new.pop(dict_key)
         except KeyError:
             pass
-    return dict_new
+    return dict_new
+
+
+def block_python_main_thread_exit():
+    """
+
+    https://funboost.readthedocs.io/zh/latest/articles/c10.html#runtimeerror-cannot-schedule-new-futures-after-interpreter-shutdown
+
+    主要是用于 python3.9以上 定时任务报错，  定时任务报错 RuntimeError: cannot schedule new futures after interpreter shutdown
+    如果主线程结束了，apscheduler就会报这个错，加上这个while 1 ： time.sleep(100) 目的就是阻止主线程退出。
+    """
+    while 1:
+        time.sleep(100)
+
+
+run_forever = block_python_main_thread_exit
```

## funboost/core/muliti_process_enhance.py

```diff
@@ -7,19 +7,19 @@
 import nb_log
 from funboost.core.booster import Booster
 
 logger = nb_log.get_logger('funboost')
 
 
 def _run_consumer_by_init_params(queue_name):
-    from funboost.core.get_booster import get_booster_ignore_current_pid
+    from funboost.core.get_booster import get_boost_params_and_consuming_function
     from funboost.core.booster import boost
     from funboost import ConsumersManager
-    _booster = get_booster_ignore_current_pid(queue_name)
-    booster_current_pid = boost(**_booster.boost_params)(_booster.consuming_function)
+    boost_params, consuming_function = get_boost_params_and_consuming_function(queue_name)
+    booster_current_pid = boost(**boost_params)(consuming_function)
     booster_current_pid.consume()
     ConsumersManager.join_all_consumer_shedual_task_thread()
 
 
 def run_consumer_with_multi_process(booster: Booster, process_num=1):
     """
     :param booster:被 boost 装饰器装饰的消费函数
@@ -47,18 +47,18 @@
         for i in range(process_num):
             # print(i)
             Process(target=_run_consumer_by_init_params,
                     args=(booster.queue_name,)).start()
 
 
 def _multi_process_pub_params_list_by_consumer_init_params(queue_name, msgs: List[dict]):
-    from funboost.core.get_booster import get_booster_ignore_current_pid
+    from funboost.core.get_booster import get_boost_params_and_consuming_function
     from funboost.core.booster import boost
-    _booster = get_booster_ignore_current_pid(queue_name)
-    booster_current_pid = boost(**_booster.boost_params)(_booster.consuming_function)
+    boost_params, consuming_function = get_boost_params_and_consuming_function(queue_name)
+    booster_current_pid = boost(**boost_params)(consuming_function)
     publisher = booster_current_pid.publisher
     publisher.set_log_level(20)  # 超高速发布，如果打印详细debug日志会卡死屏幕和严重降低代码速度。
     for msg in msgs:
         publisher.publish(msg)
 
 
 def multi_process_pub_params_list(booster: Booster, params_list, process_num=16):
```

## funboost/factories/broker_kind__publsiher_consumer_type_map.py

```diff
@@ -2,15 +2,14 @@
 
 from funboost.publishers.base_publisher import AbstractPublisher
 from funboost.consumers.base_consumer import AbstractConsumer
 
 from funboost.constant import BrokerEnum
 
 from funboost.publishers.http_publisher import HTTPPublisher
-from funboost.publishers.kombu_publisher import KombuPublisher
 from funboost.publishers.nats_publisher import NatsPublisher
 from funboost.publishers.peewee_publisher import PeeweePublisher
 from funboost.publishers.redis_publisher_lpush import RedisPublisherLpush
 from funboost.publishers.redis_pubsub_publisher import RedisPubSubPublisher
 from funboost.publishers.tcp_publisher import TCPPublisher
 from funboost.publishers.txt_file_publisher import TxtFilePublisher
 from funboost.publishers.udp_publisher import UDPPublisher
@@ -28,15 +27,14 @@
 from funboost.publishers.redis_stream_publisher import RedisStreamPublisher
 from funboost.publishers.mqtt_publisher import MqttPublisher
 from funboost.publishers.httpsqs_publisher import HttpsqsPublisher
 
 from funboost.consumers.redis_pubsub_consumer import RedisPbSubConsumer
 from funboost.consumers.http_consumer import HTTPConsumer
 from funboost.consumers.kafka_consumer import KafkaConsumer
-from funboost.consumers.kombu_consumer import KombuConsumer
 from funboost.consumers.local_python_queue_consumer import LocalPythonQueueConsumer
 from funboost.consumers.mongomq_consumer import MongoMqConsumer
 from funboost.consumers.nats_consumer import NatsConsumer
 from funboost.consumers.nsq_consumer import NsqConsumer
 from funboost.consumers.peewee_conusmer import PeeweeConsumer
 from funboost.consumers.persist_queue_consumer import PersistQueueConsumer
 from funboost.consumers.rabbitmq_amqpstorm_consumer import RabbitmqConsumerAmqpStorm
@@ -65,15 +63,14 @@
     BrokerEnum.NSQ: (NsqPublisher, NsqConsumer),
     BrokerEnum.KAFKA: (KafkaPublisher, KafkaConsumer),
     BrokerEnum.REDIS_ACK_ABLE: (RedisPublisher, RedisConsumerAckAble),
     BrokerEnum.ROCKETMQ: (RocketmqPublisher, RocketmqConsumer),
     BrokerEnum.REDIS_STREAM: (RedisStreamPublisher, RedisStreamConsumer),
     BrokerEnum.ZEROMQ: (ZeroMqPublisher, ZeroMqConsumer),
     BrokerEnum.RedisBrpopLpush: (RedisPublisherLpush, RedisBrpopLpushConsumer),
-    BrokerEnum.KOMBU: (KombuPublisher, KombuConsumer),
     BrokerEnum.MQTT: (MqttPublisher, MqttConsumer),
     BrokerEnum.HTTPSQS: (HttpsqsPublisher, HttpsqsConsumer),
     BrokerEnum.UDP: (UDPPublisher, UDPConsumer),
     BrokerEnum.TCP: (TCPPublisher, TCPConsumer),
     BrokerEnum.HTTP: (HTTPPublisher, HTTPConsumer),
     BrokerEnum.NATS: (NatsPublisher, NatsConsumer),
     BrokerEnum.TXT_FILE: (TxtFilePublisher, TxtFileConsumer),
@@ -138,7 +135,17 @@
         from funboost.publishers.huey_publisher import HueyPublisher
         register_custom_broker(BrokerEnum.HUEY, HueyPublisher, HueyConsumer)
 
     if broker_kind == BrokerEnum.KAFKA_CONFLUENT:
         from funboost.consumers.kafka_consumer_manually_commit import KafkaConsumerManuallyCommit
         from funboost.publishers.confluent_kafka_publisher import ConfluentKafkaPublisher
         register_custom_broker(BrokerEnum.KAFKA_CONFLUENT, ConfluentKafkaPublisher, KafkaConsumerManuallyCommit)
+
+    if broker_kind == BrokerEnum.RQ:
+        from funboost.consumers.rq_consumer import RqConsumer
+        from funboost.publishers.rq_publisher import RqPublisher
+        register_custom_broker(broker_kind, RqPublisher, RqConsumer)
+
+    if broker_kind == BrokerEnum.KOMBU:
+        from funboost.consumers.kombu_consumer import KombuConsumer
+        from funboost.publishers.kombu_publisher import KombuPublisher
+        register_custom_broker(broker_kind, KombuPublisher, KombuConsumer)
```

## funboost/publishers/base_publisher.py

```diff
@@ -2,14 +2,15 @@
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 11:57
 import abc
 import copy
 import inspect
 import atexit
 import json
+import multiprocessing
 import threading
 import uuid
 import time
 import typing
 from functools import wraps
 from threading import Lock
 import datetime
@@ -272,16 +273,17 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
         self.logger.warning(f'with中自动关闭publisher连接，累计推送了 {self.publish_msg_num_total} 条消息 ')
 
     def _at_exit(self):
-        self.logger.warning(
-            f'程序关闭前，{round(time.time() - self.__init_time)} 秒内，累计推送了 {self.publish_msg_num_total} 条消息 到 {self._queue_name} 中')
+        if multiprocessing.current_process().name == 'MainProcess':
+            self.logger.warning(
+                f'程序关闭前，{round(time.time() - self.__init_time)} 秒内，累计推送了 {self.publish_msg_num_total} 条消息 到 {self._queue_name} 中')
 
 
 has_init_broker_lock = threading.Lock()
 
 
 def deco_mq_conn_error(f):
     @wraps(f)
```

## funboost/publishers/celery_publisher.py

```diff
@@ -80,12 +80,12 @@
         self.logger.warning(f'刪除celery {self.queue_name} 隊列中的消息  {cmd}')
         os.system(cmd)
 
     def get_message_count(self):
         # return -1
         with celery_app.connection_or_acquire() as conn:
             msg_cnt = conn.default_channel.queue_declare(
-                queue=self.queue_name, passive=False).message_count
+                queue=self.queue_name, passive=False,durable=True,auto_delete=False).message_count
         return msg_cnt
 
     def close(self):
         pass
```

## funboost/timing_job/__init__.py

```diff
@@ -16,18 +16,18 @@
 from apscheduler.schedulers.base import STATE_STOPPED, STATE_RUNNING
 from apscheduler.util import undefined
 import deprecated
 
 from funboost import funboost_config_deafult
 
 from funboost.consumers.base_consumer import AbstractConsumer
-from funboost.core.get_booster import get_booster
+from funboost.core.get_booster import get_booster,Booster
 from funboost.publishers.base_publisher import AbstractPublisher
 
-
+@deprecated.deprecated(reason='以后不要再使用这种方式，对于job_store为数据库时候需要序列化不好。使用内存和数据库都兼容的添加任务方式: add_push_job')
 def timing_publish_deco(consuming_func_decorated_or_consumer: Union[callable, AbstractConsumer]):
     def _deco(*args, **kwargs):
         if getattr(consuming_func_decorated_or_consumer, 'is_decorated_as_consume_function', False) is True:
             consuming_func_decorated_or_consumer.push(*args, **kwargs)
         elif isinstance(consuming_func_decorated_or_consumer, AbstractConsumer):
             consuming_func_decorated_or_consumer.publisher_of_same_queue.push(*args, **kwargs)
         else:
@@ -55,15 +55,15 @@
                                next_run_time=undefined, jobstore='default', executor='default',
                                replace_existing=False, **trigger_args):
         return self.add_job(timing_publish_deco(func), trigger, args, kwargs, id, name,
                             misfire_grace_time, coalesce, max_instances,
                             next_run_time, jobstore, executor,
                             replace_existing, **trigger_args)
 
-    def add_push_job(self, func, trigger=None, args=None, kwargs=None, id=None, name=None,
+    def add_push_job(self, func:Booster, trigger=None, args=None, kwargs=None, id=None, name=None,
                      misfire_grace_time=undefined, coalesce=undefined, max_instances=undefined,
                      next_run_time=undefined, jobstore='default', executor='default',
                      replace_existing=False, **trigger_args):
         """
         :param func: 被@boost装饰器装饰的函数
         :param trigger:
         :param args:
@@ -84,19 +84,18 @@
         # kwargs['queue_name'] = func.queue_name
 
         """
         用户如果不使用funboost的 FunboostBackgroundScheduler 类型对象，而是使用原生的apscheduler类型对象，可以scheduler.add_jon(push_fun_params_to_broker,args=(,),kwargs={}) 
         push_fun_params_to_broker函数入参是消费函数队列的 queue_name 加上 原消费函数的入参
         """
         if args is None:
-            args = (func.queue_name,)
-        else:
-            args_list = list(args)
-            args_list.insert(0, func.queue_name)
-            args = tuple(args_list)
+            args = tuple()
+        args_list = list(args)
+        args_list.insert(0, func.queue_name)
+        args = tuple(args_list)
         return self.add_job(push_fun_params_to_broker, trigger, args, kwargs, id, name,
                             misfire_grace_time, coalesce, max_instances,
                             next_run_time, jobstore, executor,
                             replace_existing, **trigger_args)
 
     def start(self, paused=False, block_exit=True):
         # def _block_exit():
@@ -109,15 +108,15 @@
             while 1:
                 # print('阻止退出')
                 time.sleep(100)
 
         if block_exit:
             atexit.register(_when_exit)
         super().start(paused=paused, )
-        # _block_exit()   # python3.9 判断守护线程结束必须主线程在运行，否则结尾
+        # _block_exit()   # python3.9 判断守护线程结束必须主线程在运行。你自己在你的运行代碼的最末尾加上 while 1： time.sleep(100)  ,来阻止主线程退出。
 
     def _main_loop00000(self):
         """
         原来的代码是这，动态添加任务不友好。
         :return:
         """
         wait_seconds = threading.TIMEOUT_MAX
@@ -147,22 +146,22 @@
 
 funboost_aps_scheduler = FunboostBackgroundScheduler(timezone=funboost_config_deafult.TIMEZONE, daemon=False, )
 fsdf_background_scheduler = funboost_aps_scheduler  # 兼容一下老名字。
 
 if __name__ == '__main__':
     # 定时运行消费演示
     import datetime
-    from funboost import boost, BrokerEnum, fsdf_background_scheduler, timing_publish_deco
+    from funboost import boost, BrokerEnum, fsdf_background_scheduler, timing_publish_deco,run_forever,Booster
 
 
-    @boost('queue_test_666', broker_kind=BrokerEnum.LOCAL_PYTHON_QUEUE)
+    @Booster('queue_test_666', broker_kind=BrokerEnum.LOCAL_PYTHON_QUEUE)
     def consume_func(x, y):
         print(f'{x} + {y} = {x + y}')
 
-
+    print(consume_func,type(consume_func))
     # 定时每隔3秒执行一次。
     funboost_aps_scheduler.add_push_job(consume_func,
                                         'interval', id='3_second_job', seconds=3, kwargs={"x": 5, "y": 6})
 
     # 定时，只执行一次
     funboost_aps_scheduler.add_push_job(consume_func,
                                         'date', run_date=datetime.datetime(2020, 7, 24, 13, 53, 6), args=(5, 6,))
@@ -172,7 +171,8 @@
                                         'cron', day_of_week='*', hour=18, minute=22, second=20, args=(5, 6,))
 
     # 启动定时
     funboost_aps_scheduler.start()
 
     # 启动消费
     consume_func.consume()
+    run_forever()
```

## funboost/utils/decorators.py

```diff
@@ -519,18 +519,20 @@
 def timeout(seconds):
     """超时装饰器，指定超时时间
 
     若被装饰的方法在指定的时间内未返回，则抛出Timeout异常"""
 
     def timeout_decorator(func):
 
-        def _new_func(oldfunc, result, oldfunc_args, oldfunc_kwargs):
-            result.append(oldfunc(*oldfunc_args, **oldfunc_kwargs))
+
 
         def _(*args, **kwargs):
+            def _new_func(oldfunc, result, oldfunc_args, oldfunc_kwargs):
+                result.append(oldfunc(*oldfunc_args, **oldfunc_kwargs))
+
             result = []
             new_kwargs = {
                 'oldfunc': func,
                 'result': result,
                 'oldfunc_args': args,
                 'oldfunc_kwargs': kwargs
             }
```

## funboost/utils/show_funboost_flag.py

```diff
@@ -5,20 +5,20 @@
 funboost_flag_str = '''
 \033[0m
 FFFFFFFFFFFFFFFFFFFFFFUUUUUUUU     UUUUUUUUNNNNNNNN        NNNNNNNNBBBBBBBBBBBBBBBBB        OOOOOOOOO          OOOOOOOOO        SSSSSSSSSSSSSSS TTTTTTTTTTTTTTTTTTTTTTT
 F::::::::::::::::::::FU::::::U     U::::::UN:::::::N       N::::::NB::::::::::::::::B     OO:::::::::OO      OO:::::::::OO    SS:::::::::::::::ST:::::::::::::::::::::T
 F::::::::::::::::::::FU::::::U     U::::::UN::::::::N      N::::::NB::::::BBBBBB:::::B  OO:::::::::::::OO  OO:::::::::::::OO S:::::SSSSSS::::::ST:::::::::::::::::::::T
 FF::::::FFFFFFFFF::::FUU:::::U     U:::::UUN:::::::::N     N::::::NBB:::::B     B:::::BO:::::::OOO:::::::OO:::::::OOO:::::::OS:::::S     SSSSSSST:::::TT:::::::TT:::::T
   F:::::F       FFFFFF U:::::U     U:::::U N::::::::::N    N::::::N  B::::B     B:::::BO::::::O   O::::::OO::::::O   O::::::OS:::::S            TTTTTT  T:::::T  TTTTTT
-  F:::::F              U:::::D     D:::::U N:::::::::::N   N::::::N  B::::B     B:::::BO:::::O     O:::::OO:::::O     O:::::OS:::::S                    T:::::T        
-  F::::::FFFFFFFFFF    U:::::D     D:::::U N:::::::N::::N  N::::::N  B::::BBBBBB:::::B O:::::O     O:::::OO:::::O     O:::::O S::::SSSS                 T:::::T        
-  F:::::::::::::::F    U:::::D     D:::::U N::::::N N::::N N::::::N  B:::::::::::::BB  O:::::O     O:::::OO:::::O     O:::::O  SS::::::SSSSS            T:::::T        
-  F:::::::::::::::F    U:::::D     D:::::U N::::::N  N::::N:::::::N  B::::BBBBBB:::::B O:::::O     O:::::OO:::::O     O:::::O    SSS::::::::SS          T:::::T        
-  F::::::FFFFFFFFFF    U:::::D     D:::::U N::::::N   N:::::::::::N  B::::B     B:::::BO:::::O     O:::::OO:::::O     O:::::O       SSSSSS::::S         T:::::T        
-  F:::::F              U:::::D     D:::::U N::::::N    N::::::::::N  B::::B     B:::::BO:::::O     O:::::OO:::::O     O:::::O            S:::::S        T:::::T        
+  F:::::F              U:::::U     U:::::U N:::::::::::N   N::::::N  B::::B     B:::::BO:::::O     O:::::OO:::::O     O:::::OS:::::S                    T:::::T        
+  F::::::FFFFFFFFFF    U:::::U     U:::::U N:::::::N::::N  N::::::N  B::::BBBBBB:::::B O:::::O     O:::::OO:::::O     O:::::O S::::SSSS                 T:::::T        
+  F:::::::::::::::F    U:::::U     U:::::U N::::::N N::::N N::::::N  B:::::::::::::BB  O:::::O     O:::::OO:::::O     O:::::O  SS::::::SSSSS            T:::::T        
+  F:::::::::::::::F    U:::::U     U:::::U N::::::N  N::::N:::::::N  B::::BBBBBB:::::B O:::::O     O:::::OO:::::O     O:::::O    SSS::::::::SS          T:::::T        
+  F::::::FFFFFFFFFF    U:::::U     U:::::U N::::::N   N:::::::::::N  B::::B     B:::::BO:::::O     O:::::OO:::::O     O:::::O       SSSSSS::::S         T:::::T        
+  F:::::F              U:::::U     U:::::U N::::::N    N::::::::::N  B::::B     B:::::BO:::::O     O:::::OO:::::O     O:::::O            S:::::S        T:::::T        
   F:::::F              U::::::U   U::::::U N::::::N     N:::::::::N  B::::B     B:::::BO::::::O   O::::::OO::::::O   O::::::O            S:::::S        T:::::T        
 FF:::::::FF            U:::::::UUU:::::::U N::::::N      N::::::::NBB:::::BBBBBB::::::BO:::::::OOO:::::::OO:::::::OOO:::::::OSSSSSSS     S:::::S      TT:::::::TT      
 F::::::::FF             UU:::::::::::::UU  N::::::N       N:::::::NB:::::::::::::::::B  OO:::::::::::::OO  OO:::::::::::::OO S::::::SSSSSS:::::S      T:::::::::T      
 F::::::::FF               UU:::::::::UU    N::::::N        N::::::NB::::::::::::::::B     OO:::::::::OO      OO:::::::::OO   S:::::::::::::::SS       T:::::::::T      
 FFFFFFFFFFF                 UUUUUUUUU      NNNNNNNN         NNNNNNNBBBBBBBBBBBBBBBBB        OOOOOOOOO          OOOOOOOOO      SSSSSSSSSSSSSSS         TTTTTTTTTTT 
 \033[0m
 '''
```

## Comparing `funboost/__init__0000.py` & `funboost/__init__old.py`

 * *Files identical despite different names*

## Comparing `funboost-23.0.dist-info/LICENSE` & `funboost-23.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funboost-23.0.dist-info/METADATA` & `funboost-23.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funboost
-Version: 23.0
+Version: 23.1
 Summary: pip install funboost，python全功能分布式函数调度框架,。支持python所有类型的并发模式和一切知名消息队列中间件，python函数加速器，框架包罗万象，一统编程思维，兼容50% python业务场景，适用范围广。只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大，相见恨晚 
 Home-page: https://github.com/ydf0509/funboost
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -54,15 +54,14 @@
 Requires-Dist: rocketmq
 Requires-Dist: zmq
 Requires-Dist: pyzmq
 Requires-Dist: paho-mqtt
 Requires-Dist: setuptools-rust
 Requires-Dist: fabric2 (==2.6.0)
 Requires-Dist: nats-python
-Requires-Dist: kombu
 Requires-Dist: nb-filelock
 Requires-Dist: aiohttp (==3.8.3)
 Requires-Dist: pysnooper
 Requires-Dist: deprecated
 Requires-Dist: cryptography
 Requires-Dist: auto-run-on-remote
 Requires-Dist: frozenlist
@@ -71,25 +70,28 @@
 Requires-Dist: celery ; extra == 'extra_brokers'
 Requires-Dist: flower ; extra == 'extra_brokers'
 Requires-Dist: nameko (==2.14.1) ; extra == 'extra_brokers'
 Requires-Dist: sqlalchemy (==1.4.8) ; extra == 'extra_brokers'
 Requires-Dist: sqlalchemy-utils (==0.36.1) ; extra == 'extra_brokers'
 Requires-Dist: dramatiq (==1.14.2) ; extra == 'extra_brokers'
 Requires-Dist: huey (==2.4.5) ; extra == 'extra_brokers'
+Requires-Dist: rq (==1.15.0) ; extra == 'extra_brokers'
+Requires-Dist: kombu ; extra == 'extra_brokers'
 Requires-Dist: pulsar-client (==3.1.0) ; (python_version >= "3.7") and extra == 'extra_brokers'
 
 
 # 1.分布式函数调度框架简介
 
 <pre style="color: greenyellow;background-color: #0c1119; font-size: medium;">
 pip install funboost ,python全功能分布式函数调度框架,。 支持python所有类型的并发模式和全球一切知名消息队列中间件，
-同时funboost支持celery整个框架作为核心来发布和消费消息，使用funboost的极简api方式来自动化配置和操作celery,
+同时funboost支持celery整个框架作为核心来发布和消费消息，使用funboost的极简api方式来自动化配置和利用celery调度,
+也支持huey dramatiq rq等任务队列框架作为funboost的broker。 
 python函数加速器，框架包罗万象，一统编程思维，兼容50% python编程业务场景，适用范围广。
 只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大。
-python万能分布式函数调度框架，支持5种并发模式，30种消息中间件，20种任务控制功能。给任意python函数赋能。
+python万能分布式函数调度框架，支持5种并发模式，30+种消息队列中间件(或任务队列框架)，20种任务控制功能。给任意python函数赋能。
 用途概念就是常规经典的 生产者 + 消息队列中间件 + 消费者 编程思想。
 框架只需要学习@boost这一个装饰器的入参就可以，所有用法几乎和1.3例子一摸一样，非常简化简单。
 </pre>
 
 ### 框架评价
 
 ```
```

## Comparing `funboost-23.0.dist-info/RECORD` & `funboost-23.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-funboost/__init__.py,sha256=CZQbANWNTSr7o7WUTw60sR3Nzs8NS5pzXEb1yCnW0tQ,2154
-funboost/__init__0000.py,sha256=cSzw-ZQqtAAp5_-7eONXQT5fwz_JbZlRjDQPASDLUHk,20378
-funboost/constant.py,sha256=44kHqCwIiab7itJZeu1bk-QSUOy7V0T3etGtfeS3ViM,6154
+funboost/__init__.py,sha256=zw3heGt7VlM6lhZCHl5oSGEU0_maNM7HQHwr1vOatvY,2341
+funboost/__init__old.py,sha256=cSzw-ZQqtAAp5_-7eONXQT5fwz_JbZlRjDQPASDLUHk,20378
+funboost/constant.py,sha256=WXfZxM5uG5Cbjz6tSVRiImaBIGZz_V7b2iBiBbUmIlk,6223
 funboost/funboost_config_deafult.py,sha256=CSawbw5Yzkk73wMNOxhxkrkncS-OOSEYismtbK547xA,7358
 funboost/set_frame_config.py,sha256=hz_38C-IXEulYpHQdr1fhsMcdEDCHIsF2la8MkHiIjA,9149
-funboost/assist/celery_helper.py,sha256=iv6gY47nm1agS6E8q8FybhkzWUlYJ8Dej8R1LJCMSiI,3987
+funboost/assist/celery_helper.py,sha256=YvKP21xUzgazZHeFGq4FTgtd0A1g3BGNWzKLQ3gNygc,4186
 funboost/assist/dramatiq_helper.py,sha256=lRNouO8MyCB_Qj2ppYG4FbMpf-2Aok8QhtGZLH1zWkg,2089
 funboost/assist/huey_helper.py,sha256=VEzMdQDVJJ-ujcOXKw7chrTgvieLz4si3hrjt8gIK38,1760
+funboost/assist/rq_helper.py,sha256=-tUZ00FzkczwBAkbbISPHF-8J0K7HLSZsue39WiF-cM,1509
+funboost/assist/rq_windows_worker.py,sha256=jQlGmU0FWPVoKVP8cyuwTuAca9VfSd75F5Qw_hR04y0,4831
 funboost/beggar_version_implementation/beggar_redis_consumer.py,sha256=aiucCkj7-GWbLMIWHhevdQrAsxzyc55AL69fue8esYs,3930
 funboost/concurrent_pool/__init__.py,sha256=dGgxgzMSwcXWMexwAnojsML7EMjHAAsmAofNgrxtl2w,759
 funboost/concurrent_pool/async_helper.py,sha256=iyb0Jcjyx-vkUGC_saSUWqN657kcR5K7B-L_SB6cDCE,3256
 funboost/concurrent_pool/async_pool_executor.py,sha256=zCymNAFuPrV5CuW9hXCyzQ8nLCY73ixvvDsWFPNvt90,7227
 funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py,sha256=y6tL41X4sC_d5E2k2sNz0JZUJU2hyJDyMcOi2RzkI_w,4723
 funboost/concurrent_pool/bounded_processpoolexcutor_py36.py,sha256=fwhCvXCRILshQbGVv5Y9kFqCZsX0VMKTUdLhI9dLDbg,3011
 funboost/concurrent_pool/bounded_threadpoolexcutor.py,sha256=T1mJA1yxUYAkoDjrJMxCPPxSF3bUH4_5AFpYx3PWjfQ,1571
@@ -20,25 +22,25 @@
 funboost/concurrent_pool/custom_threadpool_executor000.py,sha256=jJLXy3h-bELap6nZA6yLtdozzTWcvCtZ7IY6MTqLEAM,9317
 funboost/concurrent_pool/single_thread_executor.py,sha256=NDWOegh8Nxpb-Bp-lUlj-DONWvepSmA9qepL1yNgdQI,373
 funboost/concurrent_pool/backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/concurrent_pool/backup/async_pool_executor0223.py,sha256=iTxxJFk2lu1P9ZAIkBip3euq3oEQ4_qTODy3xUaOecY,9548
 funboost/concurrent_pool/backup/async_pool_executor_back.py,sha256=vIgUUyF4Zb0jIRPWgNPqyO09YEkQP32kkpGBldqm4qA,9568
 funboost/concurrent_pool/backup/async_pool_executor_janus.py,sha256=OHMWJ9l3EYTpPpcrPrGGKd4K0tmQ2PN8HiX0Dta0EOo,5728
 funboost/consumers/__init__.py,sha256=ZXY_6Kut1VYNQiF5aWEgIWobsW1ht9YUP0TdRZRWFqI,126
-funboost/consumers/base_consumer.py,sha256=hn61aaexSs2j3kmUFd9ChRASZLozRzfyvuhyPZGUcT4,83054
+funboost/consumers/base_consumer.py,sha256=G-hmhk6H0F7tbKrwkXSUv1n37J1LXJ_yTffaPMfrJ50,82870
 funboost/consumers/celery_consumer.py,sha256=6CqorZH5pbxIjVwn5gNzcxSbos5YWT8eYqxYyYjgUcY,7574
 funboost/consumers/celery_consumer000.py,sha256=8SF8ppHIMH-BIAHO0NyJYnSQxe_PcT6hv05e7DySG54,4574
 funboost/consumers/confirm_mixin.py,sha256=H0w07PceU2gGf6X1EXvAB5oD7IavzGv96bQTxm-58sE,5877
 funboost/consumers/dramatiq_consumer.py,sha256=kiHM1wpSZykYDomtSGZ2PlMInCDn_8GOGEHqHUD9m0o,2144
 funboost/consumers/http_consumer.py,sha256=3HF8tsH90fUPX3iOmVid_nqW_7hZCFaL7feOkuAM36U,2025
 funboost/consumers/http_consumer000.py,sha256=NXOSiN1qpLAJfJkuF6SjFpWQ28YxMDULzWCBTNMwYe8,4463
 funboost/consumers/httpsqs_consumer.py,sha256=LICZzovaMVrZsJY4GgLrk3EaHz8f9ZZBLKZtWl3frMc,1080
 funboost/consumers/huey_consumer.py,sha256=_Z2lpfAzvs1HqkSouncN7eH1VfyQJPYNZNgv1FbZj-U,1856
 funboost/consumers/kafka_consumer.py,sha256=2BZT5UQIGqjS1emsX--V1J8gWFOhMjCMMiSnWy_Hto0,4217
-funboost/consumers/kafka_consumer_manually_commit.py,sha256=OJvua_kEZ8_MRuRxW9Jz5aiebM1tYSdjzQfVXd0sBd0,6556
+funboost/consumers/kafka_consumer_manually_commit.py,sha256=L-GYQrZ91TWCeI-GIDMXYg3LXFcq0mQ1ACu0gp4bkTI,6947
 funboost/consumers/kombu_consumer.py,sha256=VlU5LR69G0we6K5UCzWOiz-Ul_LJArWznMvTUCBwyR8,10186
 funboost/consumers/local_python_queue_consumer.py,sha256=29r44zUZPBIREvsHOfw59kRvwvfVBE2AJ8wWmXDh_3Y,1291
 funboost/consumers/mongomq_consumer.py,sha256=W5d4QnYun1OnnCn8K41ZmXuGdpAXmnzAa4EI7H7KQO4,1090
 funboost/consumers/mqtt_consumer.py,sha256=StlfPUeQ6o0HiZBpt7TlC_r2DjzPHBZBF2xLSxQW13A,2228
 funboost/consumers/nameko_consumer.py,sha256=IVwUxBixUx2m3F_q8Xn-UsnJWXayMpnOIZjICCd6mcU,2183
 funboost/consumers/nats_consumer.py,sha256=lIYLKvMHNReHnNqGtBA4wot4Ncaobtk60zVHFgm-9Zc,1076
 funboost/consumers/nsq_consumer.py,sha256=PaMRsP8oeRg0H_tq4FL7YhNUdOWAqJkjrwZWoYPNkqU,1461
@@ -53,36 +55,37 @@
 funboost/consumers/redis_consumer.py,sha256=f9nASEQUR3VHk5JH5Plf3RqKXmxogfrshu63RaFnfDM,2829
 funboost/consumers/redis_consumer_ack_able.py,sha256=DlZd76FTPo-AUiTreQd7cSiT5QAM5K9rFItAwLt2n5Y,7545
 funboost/consumers/redis_consumer_simple.py,sha256=9D3uvLw_9WOmLmwys1K39DK3gj1ex_q6NXadXwyGwrs,922
 funboost/consumers/redis_filter.py,sha256=TVyT2i9JhmhsJFyQZDx98phTiwBccNTl9fcErEDGXTM,7135
 funboost/consumers/redis_pubsub_consumer.py,sha256=eSy5QBMPaouiQbeGQ3ZaLVpU1BF8g3B_4CAJHFqhmmI,1206
 funboost/consumers/redis_stream_consumer.py,sha256=hPUMBoixd7F0Y9U4A8xC6QyOdM4EJAbXsgocHkRCarQ,6497
 funboost/consumers/rocketmq_consumer.py,sha256=sqJwxNFOz7c-4Dbk5Rgj_iJqDVwRVCGsw_tMTArGc2o,1653
+funboost/consumers/rq_consumer.py,sha256=JX84k6Jiv4pBiQMmnhdJ7s7Qz4ub5TWS4T7qTF-WdlM,876
 funboost/consumers/sqlachemy_consumer.py,sha256=-pY9pvAVUCw_T-1bRKRT37vNGjvv6BK9h-I5kfelpVk,1309
 funboost/consumers/tcp_consumer.py,sha256=hgjcXOtHyGBDS_h_p0gbOtF__Ba6DS1Chk5P9nc6Its,2045
 funboost/consumers/txt_file_consumer.py,sha256=rd8F7liwUfidk7SXY-qF4Iamx-U1NXJBYsOhOudFyyU,1340
 funboost/consumers/udp_consumer.py,sha256=J-G1ZYktXZ_er_1fg3FdSPVl4V_eEIHZXlBadCNpJmE,1643
 funboost/consumers/zeromq_consumer.py,sha256=7V1RwZKtPDDpjKTKj4GWGuz1AGZ83EBHCnWuYN4ooSM,4157
 funboost/contrib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/contrib/queue2queue.py,sha256=I6e1d2s_TQ_29rbwSs3KuA7Tuj9B905EcJruT287CnM,4680
 funboost/contrib/redis_consume_latest_msg_broker.py,sha256=V-8-pOyotOXNbs2olS7vig-yN1PxRdw_MeLOtpUufJc,1817
 funboost/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/core/active_cousumer_info_getter.py,sha256=VwVRxsApdKqnoBdg1PsHEkyWiOFJMm0_qWIdCFbPOWg,4984
-funboost/core/booster.py,sha256=xNQZt0UXzXdzk77pGiRs4hx_7BMOvLcgJz8bJXdC_6w,16419
-funboost/core/exit_signal.py,sha256=0nlDrtZnaHfYoumRXmXpeveUMvLT1iWoxfrBX2HR5OM,421
+funboost/core/booster.py,sha256=4uMrOpS_nsBVZDmPoJUJV_lcl1t-JGBotRXXrjK2kdY,16372
+funboost/core/exit_signal.py,sha256=GDP3si_hNm7-iNZeeRaON62He47j_jX5weOOsDYW68Y,576
 funboost/core/fabric_deploy_helper.py,sha256=yIdWhlJAR1rCpzvcSme-KrU7RwKH8B7tdwHG-q6QH0U,8875
 funboost/core/function_result_status_config.py,sha256=CE7xaGoL7vT2VsLTHvv-EnJE7K83XVWivBimHVmVfnQ,1570
 funboost/core/function_result_status_saver.py,sha256=6dMLpa74t3zsHF20lqfgAdCeRD1yc1oJcw--Usk-A3c,8819
-funboost/core/get_booster.py,sha256=nDD8LXanCb1h07bpgWAD113ct32XT1r6B9l6pTftnrk,1299
-funboost/core/global_boosters.py,sha256=q6-A3-H6RyKAhFofiunpn4XCtFfXumO7mcfLPXXFGX8,168
-funboost/core/helper_funs.py,sha256=hoT3IqsKCxlzF7KosvbWzE1VP4_oONIR8e86O4Phhb4,604
+funboost/core/get_booster.py,sha256=YlImXa5yjvuON_9JOa2yAlPw0tHj7RET5jBjmbj1gcM,1169
+funboost/core/global_boosters.py,sha256=CDrnKhxEEb-GxTL7JhrDTD1tyhLj7ciAtO1Cy2iyi1Q,340
+funboost/core/helper_funs.py,sha256=JDIawL6BWViC37rOJ9gFS8f4vCaispiA8Y7Zch-VM_o,1193
 funboost/core/msg_result_getter.py,sha256=a2ffSE8Rvz1t1KVEt4UxIPsWgcriaHE_Armkac-JrJY,7782
-funboost/core/muliti_process_enhance.py,sha256=ukqVJ2oPkqZvqAD8YgK1HiZRc0UoLqV96Ke0ctU1yEc,3766
+funboost/core/muliti_process_enhance.py,sha256=zNodv3Ww5yCmwO6xCh7k8HntFHjIYYJ9EPaGinvPV9Q,3814
 funboost/factories/__init__.py,sha256=s7kKKjR1HU5eMjPD6r5b-SXTVMo1zBp2JjOAtkyt5Yo,178
-funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=NFfHQHJuxBxg3icnpZD0y_vlKBf8mhQpZ43tf_O6c2s,8420
+funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=HlicHXVG_Pe3ZWoiZl84LSnhiU6fjJnB87gyo5MnKYM,8738
 funboost/factories/consumer_factory.py,sha256=KFvYkx1a7egtSiTLuVsoRMKLUAotx-QJX1jAI8Xzo3s,946
 funboost/factories/publisher_factotry.py,sha256=Vz66GrCxMt7GV5iqyIXSzZcC_eHF8fj-2kYduzbTTpg,2281
 funboost/function_result_web/app.py,sha256=xUSDBwwDA5wQVWFdFBXj9Y1s7BOh2itUw5pCZl0URMw,4841
 funboost/function_result_web/functions.py,sha256=OIPMxc4jv51qnhBxFGfTZnpMx5p4lQflPoTviDTbJUc,7345
 funboost/function_result_web/__pycache__/app.cpython-37.pyc,sha256=p-jwU7xf31KOJhmhNXqj6J79PTxjMbiTU16gAotpSEw,4045
 funboost/function_result_web/__pycache__/functions.cpython-37.pyc,sha256=KuU8DnYhFpYN0p9rdDXE9mqFuE7eKkcXHCNze3aAdOw,3921
 funboost/function_result_web/static/assets/css/custom.css,sha256=3brvjy2aBOTIXcTUK4NV6dX5wFRqx6K2aLu_jQn63jM,7674
@@ -95,16 +98,16 @@
 funboost/function_result_web/static/images/password.png,sha256=0jRivuQAhWKtkS73p8f_KiLy3D39_flqVTrpFKJPNqk,546
 funboost/function_result_web/static/images/tick.png,sha256=S9dZYN4HQzw7JsWPw3ut1dQp4OTJ_Uh2Qp2KUDF1Jv8,2912
 funboost/function_result_web/static/images/user.png,sha256=HxLjNc83WZzZEscZRdmVhGKlPXNdp_EKmmYxafuyb3g,622
 funboost/function_result_web/static/js/jquery-1.11.0.min.js,sha256=ryQZ3RXgnqkTz-lNEw-YcEhnMuV3ZODwLqOEbyBBRu4,96383
 funboost/function_result_web/templates/index.html,sha256=dWe-JFQhsDpoNjSsBF4P6SJWp_KvHX8EP_yECS5r7_o,19501
 funboost/function_result_web/templates/login.html,sha256=q37dj7O0LeyiV38Zd5P1Qn_qmhjdFomuYTRY1Yk48Bo,2007
 funboost/publishers/__init__.py,sha256=xqBHlvsJQVPfbdvP84G0LHmVB7-pFBS7vDnX1Uo9pVY,131
-funboost/publishers/base_publisher.py,sha256=Pq11w95VVPKQ5D9NEz9a3MuZa2YLplDmAI3F4TQI2OM,15047
-funboost/publishers/celery_publisher.py,sha256=OSNra9kx1_iSOc5WkqMTBkMvICBdRI2Eww1YVtf-eEE,3724
+funboost/publishers/base_publisher.py,sha256=QmK7g-U7vLl06-PbBxkblqDgEOeeRPMHIBMY5POZWqM,15148
+funboost/publishers/celery_publisher.py,sha256=exRiObJcRTpY_PgTc3rvGiu4kRMQ7OA8a4A4yKyzAyE,3755
 funboost/publishers/celery_publisher000.py,sha256=ag2s7MzPPrnNdza3u8vcbDJqtiqbQw4lJJzAVuJ6GF0,3897
 funboost/publishers/confluent_kafka_publisher.py,sha256=cpbyWvZ0T_kM62LWeBKRUuEuMkJAKOof97UUMSz6-Dk,3541
 funboost/publishers/dramatiq_publisher.py,sha256=RoZzfvkS5H-XXcmHGBomuvkQRQBlVyiaCdWpgy0LL9o,1410
 funboost/publishers/http_publisher.py,sha256=pS3z_AVqH6h4PAgqB7usihvzLJP5ZzfPKQRMQfHrJHQ,753
 funboost/publishers/httpsqs_publisher.py,sha256=7cf5ijwrbp4smq6ofndrKisruAqG0Wzfo_d_7bnLUk4,2783
 funboost/publishers/huey_publisher.py,sha256=z1CF18YZkQY6lqeoc6tiJkaYsRjRicbhYYeoHSvdD-w,1101
 funboost/publishers/kafka_publisher.py,sha256=cmlJ0mvwq0Ajlth4VQqwnoe6v_bZ4eIz49GgkiJr-ZU,2160
@@ -123,42 +126,44 @@
 funboost/publishers/rabbitmq_rabbitpy_publisher.py,sha256=GGXPKxE6-mAjqMIKqwvR9d7L-zuJQcQoU9uRsQLNGas,1953
 funboost/publishers/redis_publisher.py,sha256=mUHxfdHYrUn_Dw59NifN-mFsnj53hOhZDoEFlWs-W5M,3982
 funboost/publishers/redis_publisher_lpush.py,sha256=xEWuCTtbDcKFLTxGrECrbIVapFfUwqX2-GHenMClu-Q,278
 funboost/publishers/redis_publisher_simple.py,sha256=hLVWiDjy9ObGTmv7Vtrz21d18Fxkb52IfO5ZzaXjzMQ,872
 funboost/publishers/redis_pubsub_publisher.py,sha256=_6s7sbcGOSXxN2ZkBSDk9ILskmbj9cZTQyYHLQTYOuI,721
 funboost/publishers/redis_stream_publisher.py,sha256=DLxFcTlze0IdYFoaRmTcY8GCOaRwbj4aBNbylkt9gRA,2037
 funboost/publishers/rocketmq_publisher.py,sha256=vY82WgutDPsS9px6rukU1d3AexmsT_tqSS2dmX-Pw-c,2343
+funboost/publishers/rq_publisher.py,sha256=ANHrYnPTEj7KF_D_ov2L7PAT9swl82kjDazFqN1ULBY,893
 funboost/publishers/sqla_queue_publisher.py,sha256=yUbge08K311-jWlFyOUw6g7-Z-flbxEeWCeCTGnJcic,1215
 funboost/publishers/tcp_publisher.py,sha256=qMecOpgVqwTy-VYyevv4mCR6H5bQhCirRbJmcJIaFCE,1335
 funboost/publishers/txt_file_publisher.py,sha256=twTrqRAYnaNmFkXn0nr1xGBjeHCPJStt83voLX3vPao,1380
 funboost/publishers/udp_publisher.py,sha256=TOiKrhmCMjx4teqIgdUwRic0lxyK2cupinafsz--wzY,1194
 funboost/publishers/zeromq_publisher.py,sha256=QCsRDtmgxOdVe2F2z3PwvvkoXv1flmrHWo3Nzsx0X7g,1002
 funboost/queues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/queues/peewee_queue.py,sha256=AJlfXWSRK6GdwV8znBZasEum-VFsKHHh3YoUPK_3QVI,4944
 funboost/queues/sqla_queue.py,sha256=PxkMyXHCA_Je7H_p8c81QT7qN8x8Fq6NVmwli7PPhhg,11024
-funboost/timing_job/__init__.py,sha256=c9w4iakbF9LYqsZqeRKw01UbL80ftoD8HXCAtXOnwxU,7919
+funboost/timing_job/__init__.py,sha256=fANrkg_Dah5jdBiqIuFPQparFDo6EIhQxUftXs4OIME,8267
 funboost/timing_job/apscheduler_use_mysql_store.py,sha256=zIeK2LETm8m3VX7K6but8YAQOZomfO-P6AKLqeluxys,418
 funboost/timing_job/apscheduler_use_redis_store.py,sha256=zG2QSJYnDm6pgTwbyU3wvtr3GHKhlR9fonc5Fba1F5I,876
 funboost/utils/__init__.py,sha256=9YTXH5jt-_MulaWy5cbIpiJghy-fVQU9Gd1RHSajI94,1951
 funboost/utils/apscheduler_monkey.py,sha256=CcUISbqX6nMWSxr_QjZ26IvvhUk_ojYZWRaKenpsKfE,3124
 funboost/utils/block_exit.py,sha256=BnfxNYo3lnmhk686RAEoc4u3D4RU_iEMMMgu5L8gIuI,96
 funboost/utils/bulk_operation.py,sha256=jty8pvQWCPVUmfqeP6DnilveGc6YGjCMwVbnOAV4eRg,9972
 funboost/utils/custom_pysnooper.py,sha256=7yXLKEMY_JjPRRt0Y0N-wV2CFhILlYNh40Y6uRBUaj8,5923
-funboost/utils/decorators.py,sha256=7MesgoiZoPzhzXtGNQNSxCeFdzxg6iMg-2z7oDBsaJI,24284
+funboost/utils/decorators.py,sha256=vkshA4qHflg7G5xWuc6NcZyTKDMhS7ctGUZXlAeI_i4,24296
 funboost/utils/develop_log.py,sha256=f82JHBPBjdF_By5P_Ft4wMREeIHtF8MmqGFYa_pZbyA,251
+funboost/utils/kill_thread.py,sha256=qdqgFfWJjBimBLOKUQ0xDOn-H0AmmXIJM4_2NEUdaN8,2837
 funboost/utils/mongo_util.py,sha256=9oAWgYMBdP1rqY2KySW_VEuEBq8Xdsf5lgml4484OzM,2984
 funboost/utils/monkey_color_log.py,sha256=QChhQMTB6phZ2eBaPq-9tFZF1n7pWeJgmJPIB_ugkvs,7367
 funboost/utils/monkey_patches.py,sha256=Q0_jKxOfFrSgrIDSuSZFrgNh6w_LRGaKAITghrIpEwI,2882
 funboost/utils/mqtt_util.py,sha256=BfCmyYwI-B8VL9499_IuYlJDCbv6ZhwyWThMf8dANOU,3199
 funboost/utils/paramiko_util.py,sha256=pu67zkgptqNSV9m2Lznezb3zF1AFYvkWJp_6DVKFSPU,4901
 funboost/utils/rabbitmq_factory.py,sha256=NPzTwG-INZG9aJgkzp-QVk3TgV0rjiuTVT5lmRT77zg,2963
 funboost/utils/redis_manager.py,sha256=2Hg9UT-X6nS5TkZ-YrTRxRK-WPHZaLOsuvTxYuD1cCc,4628
 funboost/utils/resource_monitoring.py,sha256=vf1htYa3a4wlMfQqksvIINMw8laiXwG5N8NXU2Zm3qQ,5532
 funboost/utils/restart_python.py,sha256=bFbV0_24ajL8hBwVRLxWe9v9kTwiX1fGLhXRroNnmgQ,1418
-funboost/utils/show_funboost_flag.py,sha256=A4WB5P7SO9tFux1Y4yIurLmjLj09B973hq3LxEo4HOY,2985
+funboost/utils/show_funboost_flag.py,sha256=YPXtykSkRBJZ4ulOIAXiTAfpOmo9IsjePz9G9AEE6cg,2985
 funboost/utils/simple_data_class.py,sha256=HgFyyrw2mDuMX6l-re8W6q-6HXwhg2MalpIbP9JKW70,1204
 funboost/utils/time_util.py,sha256=Y-P6KowTNgGwXHzfQd4KnHdfLl8vAOqhg626MCKDvtA,5407
 funboost/utils/un_strict_json_dumps.py,sha256=uh2mXNRCq5dJcqMhb9CkfvehfEGYZAgI6RY1oLcYX_M,408
 funboost/utils/dependency_packages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/utils/dependency_packages/mongomq/__init__.py,sha256=yP7LHPsZ5ResiexksmtyJc9HGbMJWwZ0gOvHk2vNcz0,131
 funboost/utils/dependency_packages/mongomq/lock.py,sha256=anmWK7yoFnjW0ovPFuUiEKgIzw_1gymi2-mnyd3ViYY,2486
 funboost/utils/dependency_packages/mongomq/mongomq.py,sha256=A-_Y0OXmCqGHiCdOFWW4V0ciMyp6gIaPPVK95uaqd_k,7902
@@ -224,12 +229,14 @@
 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc,sha256=67Zqz4tjErzQSm9FM9mGaY3uMHYOUj3QYKtPqJQvQpE,303
 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc,sha256=a1ajayGg3JjQz--IC3-6YQHRFStG9etoieY8mXEdJ6Q,311
 funboost/utils/pysnooper_ydf/__init__.py,sha256=ctbQdJpLVZ5g_PPstj7Xaqcl0sMIgvUGwZXtcogYyHA,909
 funboost/utils/pysnooper_ydf/pycompat.py,sha256=ehsCfjsLdwoK0_o5fwYWDo3WeqCVfHW5lxekrEZxq4Y,2243
 funboost/utils/pysnooper_ydf/tracer.py,sha256=DYxYeRFSH1jXy4OTB5KIAgQm2EHRWEOwq3EXJig7Yrk,19131
 funboost/utils/pysnooper_ydf/utils.py,sha256=evSmGi_Oul7vSP47AJ0DLjFwoCYCfunJZ1mWxAkwPZw,2753
 funboost/utils/pysnooper_ydf/variables.py,sha256=QejRDESBA06KG9OH4sBT4J1M55eaU29EIHg8K_igaXo,3693
-funboost-23.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-funboost-23.0.dist-info/METADATA,sha256=OUxG861Z20n9X1M-h41oPeLXJarDNg65cnBnTK6XYrE,26423
-funboost-23.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-funboost-23.0.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
-funboost-23.0.dist-info/RECORD,,
+funboost/utils/times/__init__.py,sha256=Y4bQD3SIA_E7W2YvHq2Qdi0dGM4H2DxyFNdDOuFOq1w,2417
+funboost/utils/times/version.py,sha256=11XfnZVVzOgIhXXdeN_mYfdXThfrsbQHpA0wCjz-hpg,17
+funboost-23.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+funboost-23.1.dist-info/METADATA,sha256=NgbajoPP2oHHYl2V01BoEFyhGT2mzK0IVGGoZVv5OtY,26616
+funboost-23.1.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+funboost-23.1.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
+funboost-23.1.dist-info/RECORD,,
```

