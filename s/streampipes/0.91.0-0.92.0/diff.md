# Comparing `tmp/streampipes-0.91.0.tar.gz` & `tmp/streampipes-0.92.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streampipes-0.91.0.tar", last modified: Fri Apr 14 06:09:38 2023, max compression
+gzip compressed data, was "streampipes-0.92.0.tar", last modified: Mon Jun 19 15:50:04 2023, max compression
```

## Comparing `streampipes-0.91.0.tar` & `streampipes-0.92.0.tar`

### file list

```diff
@@ -1,85 +1,80 @@
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.344386 streampipes-0.91.0/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     5323 2023-04-14 06:09:38.344162 streampipes-0.91.0/PKG-INFO
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     3994 2023-04-07 08:31:02.000000 streampipes-0.91.0/README.md
--rw-r--r--   0 tbossenmaier   (501) staff       (20)       38 2023-04-14 06:09:38.344467 streampipes-0.91.0/setup.cfg
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4253 2023-04-14 06:09:23.000000 streampipes-0.91.0/setup.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.321770 streampipes-0.91.0/streampipes/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      904 2023-04-14 05:54:46.000000 streampipes-0.91.0/streampipes/__version__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.323589 streampipes-0.91.0/streampipes/client/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      863 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/client/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     8765 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/client/client.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2078 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/client/config.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4889 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/client/credential_provider.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.324250 streampipes-0.91.0/streampipes/endpoint/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      898 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/endpoint/__init__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.324881 streampipes-0.91.0/streampipes/endpoint/api/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      956 2023-03-21 15:41:27.000000 streampipes-0.91.0/streampipes/endpoint/api/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)    14121 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/endpoint/api/data_lake_measure.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2775 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/endpoint/api/data_stream.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)    10562 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/endpoint/endpoint.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2042 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/endpoint/exceptions.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.325039 streampipes-0.91.0/streampipes/endpoint/messaging/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/endpoint/messaging/__init__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.325327 streampipes-0.91.0/streampipes/function_zoo/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/function_zoo/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     8227 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/function_zoo/river_function.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.326077 streampipes-0.91.0/streampipes/functions/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/functions/__init__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.334057 streampipes-0.91.0/streampipes/functions/broker/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1064 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     3428 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/broker.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2250 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/broker_handler.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2950 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/kafka_broker.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1468 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/kafka_message_fetcher.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2865 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/nats_broker.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2554 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/output_collector.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     7689 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/function_handler.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1996 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/registration.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4538 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/streampipes_function.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.338746 streampipes-0.91.0/streampipes/functions/utils/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/functions/utils/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2660 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/utils/async_iter_handler.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1910 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/utils/data_stream_context.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2698 2023-04-14 05:54:46.000000 streampipes-0.91.0/streampipes/functions/utils/data_stream_generator.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2054 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/utils/function_context.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.339206 streampipes-0.91.0/streampipes/model/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/model/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     6193 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/common.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.339978 streampipes-0.91.0/streampipes/model/container/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      930 2023-03-21 15:41:27.000000 streampipes-0.91.0/streampipes/model/container/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1853 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/container/data_lake_measures.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1796 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/container/data_streams.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     8463 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/container/resource_container.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.341183 streampipes-0.91.0/streampipes/model/resource/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1069 2023-04-07 08:29:39.000000 streampipes-0.91.0/streampipes/model/resource/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2624 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/resource/data_lake_measure.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4463 2023-04-14 05:54:46.000000 streampipes-0.91.0/streampipes/model/resource/data_lake_series.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     5869 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/resource/data_stream.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4108 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/resource/function_definition.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2545 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/resource/resource.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.322487 streampipes-0.91.0/streampipes.egg-info/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     5323 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/PKG-INFO
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2385 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/SOURCES.txt
--rw-r--r--   0 tbossenmaier   (501) staff       (20)        1 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/dependency_links.txt
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1574 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/requires.txt
--rw-r--r--   0 tbossenmaier   (501) staff       (20)       18 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/top_level.txt
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.320912 streampipes-0.91.0/tests/
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.342132 streampipes-0.91.0/tests/client/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/client/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4780 2023-03-21 15:41:27.000000 streampipes-0.91.0/tests/client/test_client.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1964 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/client/test_credential_provider.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     5475 2023-04-07 08:29:39.000000 streampipes-0.91.0/tests/client/test_data_lake_series.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)    18372 2023-03-21 15:41:27.000000 streampipes-0.91.0/tests/client/test_endpoint.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.342692 streampipes-0.91.0/tests/endpoint/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/endpoint/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     5128 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/endpoint/test_data_lake_measure.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.343237 streampipes-0.91.0/tests/functions/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/functions/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)    17234 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/functions/test_function_handler.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     8047 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/functions/test_river_function.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.343438 streampipes-0.91.0/tests/model/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/model/__init__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.343872 streampipes-0.91.0/tests/model/resource/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/model/resource/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2752 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/model/resource/test_data_stream.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.072867 streampipes-0.92.0/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     6517 2023-06-19 15:50:04.072633 streampipes-0.92.0/PKG-INFO
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     5188 2023-06-19 15:45:50.000000 streampipes-0.92.0/README.md
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)       38 2023-06-19 15:50:04.072934 streampipes-0.92.0/setup.cfg
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4315 2023-06-19 15:49:54.000000 streampipes-0.92.0/setup.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.029337 streampipes-0.92.0/streampipes/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      904 2023-04-14 10:57:19.000000 streampipes-0.92.0/streampipes/__version__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.043938 streampipes-0.92.0/streampipes/client/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      863 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/client/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)    10370 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/client/client.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2078 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/client/config.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4889 2023-06-19 15:45:50.000000 streampipes-0.92.0/streampipes/client/credential_provider.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.058955 streampipes-0.92.0/streampipes/endpoint/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      898 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/endpoint/__init__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.060345 streampipes-0.92.0/streampipes/endpoint/api/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1016 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/endpoint/api/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)    14105 2023-06-17 09:19:13.000000 streampipes-0.92.0/streampipes/endpoint/api/data_lake_measure.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2774 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/endpoint/api/data_stream.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4513 2023-06-19 15:45:58.000000 streampipes-0.92.0/streampipes/endpoint/api/version.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)    10562 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/endpoint/endpoint.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2042 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/endpoint/exceptions.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.061004 streampipes-0.92.0/streampipes/endpoint/messaging/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/endpoint/messaging/__init__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.061810 streampipes-0.92.0/streampipes/function_zoo/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/function_zoo/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     8458 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/function_zoo/river_function.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.063392 streampipes-0.92.0/streampipes/functions/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/functions/__init__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.065288 streampipes-0.92.0/streampipes/functions/broker/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1341 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2648 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/broker.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     3262 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/broker_handler.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2077 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/consumer.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.066430 streampipes-0.92.0/streampipes/functions/broker/kafka/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/kafka/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2658 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/kafka/kafka_consumer.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1514 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/kafka/kafka_message_fetcher.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2233 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/kafka/kafka_publisher.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.067237 streampipes-0.92.0/streampipes/functions/broker/nats/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/nats/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2380 2023-06-19 15:45:50.000000 streampipes-0.92.0/streampipes/functions/broker/nats/nats_consumer.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2199 2023-06-19 15:45:50.000000 streampipes-0.92.0/streampipes/functions/broker/nats/nats_publisher.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2632 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/output_collector.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1411 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/broker/publisher.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     7679 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/function_handler.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1996 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/functions/registration.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4538 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/functions/streampipes_function.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.068506 streampipes-0.92.0/streampipes/functions/utils/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/functions/utils/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2676 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/utils/async_iter_handler.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1911 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/utils/data_stream_context.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     3332 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/functions/utils/data_stream_generator.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2054 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/functions/utils/function_context.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.068995 streampipes-0.92.0/streampipes/model/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.92.0/streampipes/model/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     6193 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/common.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.070188 streampipes-0.92.0/streampipes/model/container/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      977 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/model/container/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1853 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/container/data_lake_measures.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1796 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/container/data_streams.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     8463 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/container/resource_container.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1914 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/model/container/versions.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.072271 streampipes-0.92.0/streampipes/model/resource/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1100 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/model/resource/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2624 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/resource/data_lake_measure.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4103 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/resource/data_series.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     5869 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/resource/data_stream.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1284 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/resource/exceptions.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4108 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/resource/function_definition.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     3412 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/resource/query_result.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2545 2023-05-06 05:45:00.000000 streampipes-0.92.0/streampipes/model/resource/resource.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1439 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/model/resource/version.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      785 2023-06-04 06:58:50.000000 streampipes-0.92.0/streampipes/py.typed
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-06-19 15:50:04.042134 streampipes-0.92.0/streampipes.egg-info/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     6517 2023-06-19 15:50:04.000000 streampipes-0.92.0/streampipes.egg-info/PKG-INFO
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2466 2023-06-19 15:50:04.000000 streampipes-0.92.0/streampipes.egg-info/SOURCES.txt
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)        1 2023-06-19 15:50:04.000000 streampipes-0.92.0/streampipes.egg-info/dependency_links.txt
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1584 2023-06-19 15:50:04.000000 streampipes-0.92.0/streampipes.egg-info/requires.txt
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)       12 2023-06-19 15:50:04.000000 streampipes-0.92.0/streampipes.egg-info/top_level.txt
```

### Comparing `streampipes-0.91.0/PKG-INFO` & `streampipes-0.92.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streampipes
-Version: 0.91.0
+Version: 0.92.0
 Summary: Python library for Apache StreamPipes
 Home-page: https://streampipes.apache.org/docs/docs/python/latest/
 Author: Apache Software Foundation
 Author-email: dev@streampipes.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://streampipes.apache.org/docs/docs/python/latest/
 Project-URL: Bug Tracker, https://github.com/apache/streampipes/issues
@@ -60,36 +60,61 @@
 
 <br>
 <h3 align="center">Apache StreamPipes for Python</h3>
 
 <p align="center"> Apache StreamPipes meets Python! We are working highly motivated on a Python library to interact with StreamPipes.
 In this way, we would like to unite the power of StreamPipes to easily connect to and read different data sources, especially in the IoT domain,
 and the amazing universe of data analytics libraries in Python. </p>
+<br>
+
+<p align="center">
+<a href="https://github.com/apache/streampipes/tree/dev/streampipes-client-python" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/streampipes" alt="Supported Python versions">
+</a>
+<a href="https://pypi.org/project/streampipes/" target="_blank">
+    <img src="https://img.shields.io/pypi/v/streampipes" alt="Current PyPI version">
+</a>
+<a href="https://streampipes.apache.org/docs/docs/python/latest/" target="_blank">
+    <img src="https://github.com/apache/streampipes-website/actions/workflows/update-python-docs.yml/badge.svg" alt="Status Python Docs">
+</a>
+<a href="https://github.com/psf/black" target="_blank">
+    <img src="https://img.shields.io/badge/code%20style-black-black" alt="Code Style: Black">
+</a>
+<a href="https://github.com/python/mypy" target="_blank">
+    <img src="https://img.shields.io/badge/typed-mypy-blue" alt="Typed: MyPy">
+</a>
+<img src="./docs/img/interrogate_badge.svg" alt= “interrogate” height="20">
+<a href="https://pypi.org/project/streampipes/" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/streampipes" alt="Downloads: PyPI/Month">
+</a>
+</p>
 
 ---
 
 <br>
 
-**💡The current version of this Python client is still a beta version.**
-<br>
-**This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.**
+<h4 align="center">💡The current version of this Python client is still a beta version.</h4>
+<h4 align="center">This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.</h4>
+
 <br>
 
 
 ## 📚 Documentation
-Please visit our documentation: https://streampipes.apache.org/docs/docs/python/latest/
+Please visit our [documentation](https://streampipes.apache.org/docs/docs/python/latest/).
 There you can find information about how to [get started](https://streampipes.apache.org/docs/docs/python/latest/getting-started/first-steps/),
 follow some [tutorials](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/),
 or discover the library via our [references](https://streampipes.apache.org/docs/docs/python/latest/reference/client/client/).
 <br>
 
 In case you want to access the documentation of the current development state, you can go here:
 
 👉 [development docs 🤓](https://streampipes.apache.org/docs/docs/python/dev/)
 
+<br>
+
 ## ⚡️ Quickstart
 
 As a quick example, we demonstrate how to set up and configure a StreamPipes client.
 
 You can simply install the StreamPipes library by running the following command
 ```bash
 pip install streampipes
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streampipes Version: 0.91.0 Summary: Python library
+Metadata-Version: 2.1 Name: streampipes Version: 0.92.0 Summary: Python library
 for Apache StreamPipes Home-page: https://streampipes.apache.org/docs/docs/
 python/latest/ Author: Apache Software Foundation Author-email:
 dev@streampipes.apache.org License: Apache License 2.0 Project-URL:
 Documentation, https://streampipes.apache.org/docs/docs/python/latest/ Project-
 URL: Bug Tracker, https://github.com/apache/streampipes/issues Project-URL:
 Source Code, https://github.com/apache/streampipes Keywords:
 streampipes,iot,iiot,analytics,stream-processing,apache Classifier: Development
@@ -24,39 +24,44 @@
 
                     **** Apache StreamPipes for Python ****
  Apache StreamPipes meets Python! We are working highly motivated on a Python
  library to interact with StreamPipes. In this way, we would like to unite the
   power of StreamPipes to easily connect to and read different data sources,
    especially in the IoT domain, and the amazing universe of data analytics
                              libraries in Python.
+
+ [Supported_Python_versions] [Current_PyPI_version] [Status_Python_Docs] [Code
+    Style:_Black] [Typed:_MyPy] [âinterrogateâ] [Downloads:_PyPI/Month]
 ---
-**ð¡The current version of this Python client is still a beta version.**
-**This means that it is still under development, which may result in frequent
-and extensive API changes, unstable behavior, etc.**
-## ð Documentation Please visit our documentation: https://
-streampipes.apache.org/docs/docs/python/latest/ There you can find information
-about how to [get started](https://streampipes.apache.org/docs/docs/python/
-latest/getting-started/first-steps/), follow some [tutorials](https://
-streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
-streampipes-python-client/), or discover the library via our [references]
-(https://streampipes.apache.org/docs/docs/python/latest/reference/client/
-client/).
+*** ð¡The current version of this Python client is still a beta version. ***
+*** This means that it is still under development, which may result in frequent
+            and extensive API changes, unstable behavior, etc. ***
+
+## ð Documentation Please visit our [documentation](https://
+streampipes.apache.org/docs/docs/python/latest/). There you can find
+information about how to [get started](https://streampipes.apache.org/docs/
+docs/python/latest/getting-started/first-steps/), follow some [tutorials]
+(https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-
+introduction-to-streampipes-python-client/), or discover the library via our
+[references](https://streampipes.apache.org/docs/docs/python/latest/reference/
+client/client/).
 In case you want to access the documentation of the current development state,
 you can go here: ð [development docs ð¤](https://streampipes.apache.org/
-docs/docs/python/dev/) ## â¡ï¸ Quickstart As a quick example, we demonstrate
-how to set up and configure a StreamPipes client. You can simply install the
-StreamPipes library by running the following command ```bash pip install
-streampipes # if you want to have the current development state you can also
-execute pip install git+https://github.com/apache/
-streampipes.git#subdirectory=streampipes-client-python ``` ```python from
-streampipes.client import StreamPipesClient from streampipes.client.config
-import StreamPipesClientConfig from streampipes.client.credential_provider
-import StreamPipesApiKeyCredentials config = StreamPipesClientConfig
-( credential_provider = StreamPipesApiKeyCredentials( username =
-"test@streampipes.apache.org", api_key = "DEMO-KEY", ), host_address =
-"localhost", https_disabled = True, port = 80 ) client = StreamPipesClient
-(client_config=config) client.describe() ``` Output: ``` Hi there! You are
-connected to a StreamPipes instance running at http://localhost:80. The
-following StreamPipes resources are available with this client: 6x DataStreams
-1x DataLakeMeasures ``` For more information about how to use the StreamPipes
-client visit our [introduction tutorial](https://streampipes.apache.org/docs/
-docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
+docs/docs/python/dev/)
+## â¡ï¸ Quickstart As a quick example, we demonstrate how to set up and
+configure a StreamPipes client. You can simply install the StreamPipes library
+by running the following command ```bash pip install streampipes # if you want
+to have the current development state you can also execute pip install
+git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-
+python ``` ```python from streampipes.client import StreamPipesClient from
+streampipes.client.config import StreamPipesClientConfig from
+streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+config = StreamPipesClientConfig( credential_provider =
+StreamPipesApiKeyCredentials( username = "test@streampipes.apache.org", api_key
+= "DEMO-KEY", ), host_address = "localhost", https_disabled = True, port = 80 )
+client = StreamPipesClient(client_config=config) client.describe() ``` Output:
+``` Hi there! You are connected to a StreamPipes instance running at http://
+localhost:80. The following StreamPipes resources are available with this
+client: 6x DataStreams 1x DataLakeMeasures ``` For more information about how
+to use the StreamPipes client visit our [introduction tutorial](https://
+streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
+streampipes-python-client/).
```

### Comparing `streampipes-0.91.0/README.md` & `streampipes-0.92.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -27,36 +27,61 @@
 
 <br>
 <h3 align="center">Apache StreamPipes for Python</h3>
 
 <p align="center"> Apache StreamPipes meets Python! We are working highly motivated on a Python library to interact with StreamPipes.
 In this way, we would like to unite the power of StreamPipes to easily connect to and read different data sources, especially in the IoT domain,
 and the amazing universe of data analytics libraries in Python. </p>
+<br>
+
+<p align="center">
+<a href="https://github.com/apache/streampipes/tree/dev/streampipes-client-python" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/streampipes" alt="Supported Python versions">
+</a>
+<a href="https://pypi.org/project/streampipes/" target="_blank">
+    <img src="https://img.shields.io/pypi/v/streampipes" alt="Current PyPI version">
+</a>
+<a href="https://streampipes.apache.org/docs/docs/python/latest/" target="_blank">
+    <img src="https://github.com/apache/streampipes-website/actions/workflows/update-python-docs.yml/badge.svg" alt="Status Python Docs">
+</a>
+<a href="https://github.com/psf/black" target="_blank">
+    <img src="https://img.shields.io/badge/code%20style-black-black" alt="Code Style: Black">
+</a>
+<a href="https://github.com/python/mypy" target="_blank">
+    <img src="https://img.shields.io/badge/typed-mypy-blue" alt="Typed: MyPy">
+</a>
+<img src="./docs/img/interrogate_badge.svg" alt= “interrogate” height="20">
+<a href="https://pypi.org/project/streampipes/" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/streampipes" alt="Downloads: PyPI/Month">
+</a>
+</p>
 
 ---
 
 <br>
 
-**💡The current version of this Python client is still a beta version.**
-<br>
-**This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.**
+<h4 align="center">💡The current version of this Python client is still a beta version.</h4>
+<h4 align="center">This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.</h4>
+
 <br>
 
 
 ## 📚 Documentation
-Please visit our documentation: https://streampipes.apache.org/docs/docs/python/latest/
+Please visit our [documentation](https://streampipes.apache.org/docs/docs/python/latest/).
 There you can find information about how to [get started](https://streampipes.apache.org/docs/docs/python/latest/getting-started/first-steps/),
 follow some [tutorials](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/),
 or discover the library via our [references](https://streampipes.apache.org/docs/docs/python/latest/reference/client/client/).
 <br>
 
 In case you want to access the documentation of the current development state, you can go here:
 
 👉 [development docs 🤓](https://streampipes.apache.org/docs/docs/python/dev/)
 
+<br>
+
 ## ⚡️ Quickstart
 
 As a quick example, we demonstrate how to set up and configure a StreamPipes client.
 
 You can simply install the StreamPipes library by running the following command
 ```bash
 pip install streampipes
```

#### html2text {}

```diff
@@ -6,39 +6,44 @@
 
                     **** Apache StreamPipes for Python ****
  Apache StreamPipes meets Python! We are working highly motivated on a Python
  library to interact with StreamPipes. In this way, we would like to unite the
   power of StreamPipes to easily connect to and read different data sources,
    especially in the IoT domain, and the amazing universe of data analytics
                              libraries in Python.
+
+ [Supported_Python_versions] [Current_PyPI_version] [Status_Python_Docs] [Code
+    Style:_Black] [Typed:_MyPy] [âinterrogateâ] [Downloads:_PyPI/Month]
 ---
-**ð¡The current version of this Python client is still a beta version.**
-**This means that it is still under development, which may result in frequent
-and extensive API changes, unstable behavior, etc.**
-## ð Documentation Please visit our documentation: https://
-streampipes.apache.org/docs/docs/python/latest/ There you can find information
-about how to [get started](https://streampipes.apache.org/docs/docs/python/
-latest/getting-started/first-steps/), follow some [tutorials](https://
-streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
-streampipes-python-client/), or discover the library via our [references]
-(https://streampipes.apache.org/docs/docs/python/latest/reference/client/
-client/).
+*** ð¡The current version of this Python client is still a beta version. ***
+*** This means that it is still under development, which may result in frequent
+            and extensive API changes, unstable behavior, etc. ***
+
+## ð Documentation Please visit our [documentation](https://
+streampipes.apache.org/docs/docs/python/latest/). There you can find
+information about how to [get started](https://streampipes.apache.org/docs/
+docs/python/latest/getting-started/first-steps/), follow some [tutorials]
+(https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-
+introduction-to-streampipes-python-client/), or discover the library via our
+[references](https://streampipes.apache.org/docs/docs/python/latest/reference/
+client/client/).
 In case you want to access the documentation of the current development state,
 you can go here: ð [development docs ð¤](https://streampipes.apache.org/
-docs/docs/python/dev/) ## â¡ï¸ Quickstart As a quick example, we demonstrate
-how to set up and configure a StreamPipes client. You can simply install the
-StreamPipes library by running the following command ```bash pip install
-streampipes # if you want to have the current development state you can also
-execute pip install git+https://github.com/apache/
-streampipes.git#subdirectory=streampipes-client-python ``` ```python from
-streampipes.client import StreamPipesClient from streampipes.client.config
-import StreamPipesClientConfig from streampipes.client.credential_provider
-import StreamPipesApiKeyCredentials config = StreamPipesClientConfig
-( credential_provider = StreamPipesApiKeyCredentials( username =
-"test@streampipes.apache.org", api_key = "DEMO-KEY", ), host_address =
-"localhost", https_disabled = True, port = 80 ) client = StreamPipesClient
-(client_config=config) client.describe() ``` Output: ``` Hi there! You are
-connected to a StreamPipes instance running at http://localhost:80. The
-following StreamPipes resources are available with this client: 6x DataStreams
-1x DataLakeMeasures ``` For more information about how to use the StreamPipes
-client visit our [introduction tutorial](https://streampipes.apache.org/docs/
-docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
+docs/docs/python/dev/)
+## â¡ï¸ Quickstart As a quick example, we demonstrate how to set up and
+configure a StreamPipes client. You can simply install the StreamPipes library
+by running the following command ```bash pip install streampipes # if you want
+to have the current development state you can also execute pip install
+git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-
+python ``` ```python from streampipes.client import StreamPipesClient from
+streampipes.client.config import StreamPipesClientConfig from
+streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+config = StreamPipesClientConfig( credential_provider =
+StreamPipesApiKeyCredentials( username = "test@streampipes.apache.org", api_key
+= "DEMO-KEY", ), host_address = "localhost", https_disabled = True, port = 80 )
+client = StreamPipesClient(client_config=config) client.describe() ``` Output:
+``` Hi there! You are connected to a StreamPipes instance running at http://
+localhost:80. The following StreamPipes resources are available with this
+client: 6x DataStreams 1x DataLakeMeasures ``` For more information about how
+to use the StreamPipes client visit our [introduction tutorial](https://
+streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
+streampipes-python-client/).
```

### Comparing `streampipes-0.91.0/setup.py` & `streampipes-0.92.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,41 +41,41 @@
     "pydantic>=1.10.2",
     "requests>=2.28.1",
     "nats-py>=2.2.0",
     "confluent-kafka>=2.0.2"
 ]
 
 dev_packages = base_packages + [
-    "autoflake==2.0.0",
-    "black==23.1.0",
+    "autoflake==2.1.0",
+    "black==23.3.0",
     "blacken-docs==1.13.0",
     "flake8==6.0.0",
-    "interrogate==1.5.0",
+    "interrogate[png]==1.5.0",
     "isort==5.12.0",
-    "mypy==1.0.0",
-    "pandas-stubs==1.5.2.230105",
-    "pre-commit==3.0.0",
-    "pytest==7.2.1",
+    "mypy==1.3.0",
+    "pandas-stubs==2.0.0.230412",
+    "pre-commit==3.3.0",
+    "pytest==7.3.0",
     "pytest-cov==4.0.0",
-    "pyupgrade==3.3.1",
+    "pyupgrade==3.4.0",
     "types-Jinja2==2.11.9",
-    "types-requests==2.28.11.7",
+    "types-requests==2.30.0.0",
 ]
 
 docs_packages = [
     "mkdocs==1.4.2",
-    "mkdocs-awesome-pages-plugin==2.8.0",
-    "mkdocs-material==8.5.11",  # < 9.x.y is required by mkdocs-jupyter
-    "mkdocstrings[python]==0.20.0",
+    "mkdocs-awesome-pages-plugin==2.9.0",
+    "mkdocs-material==9.1.3",
+    "mkdocstrings[python]==0.21.1",
     "pytkdocs[numpy-style]>=0.16.1",
-    "mkdocs-gen-files==0.4.0",
+    "mkdocs-gen-files==0.5.0",
     "mkdocs-literate-nav==0.6.0",
     "numpydoc==1.5.0",
-    "mkdocs-jupyter==0.22.0",
-#    "mike @ git+https://github.com/jimporter/mike.git@872f72def32f588908f8251fe512189e0c41f4e2"
+    "mkdocs-jupyter==0.24.0",
+    #"mike @ git+https://github.com/jimporter/mike.git@872f72def32f588908f8251fe512189e0c41f4e2"
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
@@ -93,23 +93,29 @@
     long_description=long_description,
     long_description_content_type=LONG_DESCRIPTION_CONTENT_TYPE,
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     project_urls=PROJECT_URLS,
-    packages=setuptools.find_packages(exclude=("tests",)),
+    packages=setuptools.find_packages(exclude=("*tests*",)),
+    package_data={
+        "streampipes": [
+            "py.typed",
+            "*.pyi",
+            "**/*.pyi"
+        ]
+    },
     install_requires=base_packages,
     extras_require={
         "dev": dev_packages,
         "test": dev_packages,
         "docs": docs_packages,
         "all": dev_packages + docs_packages,
     },
-    include_package_data=True,
     license="Apache License 2.0",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `streampipes-0.91.0/streampipes/__init__.py` & `streampipes-0.92.0/streampipes/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/__version__.py` & `streampipes-0.92.0/streampipes/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
 
-VERSION = (0, 91, 0)  # pragma: no cover
+VERSION = (0, 92, 0)  # pragma: no cover
 
 __version__ = ".".join(map(str, VERSION))  # noqa: F401 # pragma: no cover
```

### Comparing `streampipes-0.91.0/streampipes/client/__init__.py` & `streampipes-0.92.0/streampipes/client/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/client/client.py` & `streampipes-0.92.0/streampipes/client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,16 +25,20 @@
 
 import logging
 import sys
 from typing import Dict, Optional
 
 from requests import Session
 from streampipes.client.config import StreamPipesClientConfig
-from streampipes.endpoint.api import DataLakeMeasureEndpoint, DataStreamEndpoint
-from streampipes.endpoint.endpoint import APIEndpoint
+from streampipes.endpoint import APIEndpoint
+from streampipes.endpoint.api import (
+    DataLakeMeasureEndpoint,
+    DataStreamEndpoint,
+    VersionEndpoint,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class StreamPipesClient:
     """The client to connect to StreamPipes.
 
@@ -122,14 +126,44 @@
         self.logging_level = logging_level
         self._set_up_logging(logging_level=self.logging_level)  # type: ignore
 
         # provide all available endpoints here
         # name of the endpoint needs to be consistent with the Java client
         self.dataLakeMeasureApi = DataLakeMeasureEndpoint(parent_client=self)
         self.dataStreamApi = DataStreamEndpoint(parent_client=self)
+        self.versionApi = VersionEndpoint(parent_client=self)
+
+        self.server_version = self._get_server_version()
+
+    def _get_server_version(self) -> str:
+        """Connects to the StreamPipes server and retrieves its version.
+
+        In addition to querying the server version, this method implicitly checks the specified credentials.
+
+        Returns
+        -------
+        sp_version: str
+            version of the connected StreamPipes instance
+
+        """
+
+        # retrieve metadata from the API via the Streampipes server
+        # as a side effect, the specified credentials are also tested to ensure that authentication is successful.
+        version_dict = self.versionApi.get(identifier="").to_dict(use_source_names=False)
+
+        # remove SNAPSHOT-suffix if present
+        sp_version = version_dict["backend_version"].replace("-SNAPSHOT", "")
+
+        logger.info(
+            "The StreamPipes version was successfully retrieved from the backend: %s. "
+            "By means of that, authentication via the provided credentials is also tested successfully.",
+            sp_version,
+        )
+
+        return sp_version
 
     @staticmethod
     def _set_up_logging(logging_level: int) -> None:
         """Configures the logging behavior of the `StreamPipesClient`.
 
         Parameters
         ----------
@@ -224,33 +258,44 @@
         The following StreamPipes resources are available with this client:
         6x DataStreams
         1x DataLakeMeasures
         ```
         """
 
         # get all endpoints of this client
-        available_endpoints = [
+        available_endpoints = {
             attr_name for attr_name in dir(self) if isinstance(self.__getattribute__(attr_name), APIEndpoint)
-        ]
+        }
+
+        # remove endpoints that are not suitable for the describe method
+        # this is mainly due to not providing the `all()` method
+        available_endpoints = available_endpoints.symmetric_difference(
+            {
+                "versionApi",
+            }
+        )
+
+        # ensure deterministic order
+        ordered_available_endpoints = sorted(available_endpoints)
 
         # collect the number of available resources per endpoint
         endpoint_stats = {
             (all_items := self.__getattribute__(endpoint_name).all()).__class__.__name__: len(all_items)
-            for endpoint_name in available_endpoints
+            for endpoint_name in ordered_available_endpoints
         }
 
         # sort the endpoints descending based on the number of resources
         sorted_endpoint_stats = {
             key: val for key, val in sorted(endpoint_stats.items(), key=lambda item: item[1], reverse=True)
         }
 
         base_message = (
             f"\nHi there!\n"
             f"You are connected to a StreamPipes instance running at "
             f"{'http://' if self.client_config.https_disabled else 'https://'}"
-            f"{self.client_config.host_address}:{self.client_config.port}.\n"
+            f"{self.client_config.host_address}:{self.client_config.port} with version {self.server_version}.\n"
             f"The following StreamPipes resources are available with this client:\n"
         )
 
         endpoint_stats_message = "\n".join(f"{count}x {name}" for name, count in sorted_endpoint_stats.items())
 
-        print(base_message + endpoint_stats_message)
+        logger.info(base_message + endpoint_stats_message)
```

### Comparing `streampipes-0.91.0/streampipes/client/config.py` & `streampipes-0.92.0/streampipes/client/config.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/client/credential_provider.py` & `streampipes-0.92.0/streampipes/client/credential_provider.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/endpoint/__init__.py` & `streampipes-0.92.0/streampipes/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/endpoint/api/__init__.py` & `streampipes-0.92.0/streampipes/endpoint/api/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from .data_lake_measure import DataLakeMeasureEndpoint
 from .data_stream import DataStreamEndpoint
+from .version import VersionEndpoint
 
 __all__ = [
     "DataLakeMeasureEndpoint",
     "DataStreamEndpoint",
+    "VersionEndpoint",
 ]
```

### Comparing `streampipes-0.91.0/streampipes/endpoint/api/data_lake_measure.py` & `streampipes-0.92.0/streampipes/endpoint/api/data_lake_measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from datetime import datetime
 from typing import Any, Dict, Literal, Optional, Tuple, Type
 
 from pydantic import BaseModel, Extra, Field, StrictInt, ValidationError, validator
 from streampipes.endpoint.endpoint import APIEndpoint
 from streampipes.model.container import DataLakeMeasures
 from streampipes.model.container.resource_container import ResourceContainer
-from streampipes.model.resource import DataLakeSeries
+from streampipes.model.resource.query_result import QueryResult
 
 __all__ = [
     "DataLakeMeasureEndpoint",
 ]
 
 
 class StreamPipesQueryValidationError(Exception):
@@ -154,17 +154,17 @@
 
         return query_param_string
 
 
 class DataLakeMeasureEndpoint(APIEndpoint):
     """Implementation of the DataLakeMeasure endpoint.
 
-    This endpoint provides an interfact to all data stored in the StreamPipes data lake.
+    This endpoint provides an interface to all data stored in the StreamPipes data lake.
 
-    Consequently, it allows uerying metadata about available data sets (see `all()` method).
+    Consequently, it allows querying metadata about available data sets (see `all()` method).
     The metadata is returned as an instance of [`DataLakeMeasures`][streampipes.model.container.DataLakeMeasures].
 
     In addition, the endpoint provides direct access to the data stored in the data laka by querying a
     specific data lake measure using the `get()` method.
 
     Examples
     --------
@@ -271,38 +271,38 @@
                 f"https://github.com/apache/streampipes.\n"
                 f"Please don't forget to include the following validation log from above."
             )
 
         return config
 
     @property
-    def _resource_cls(self) -> Type[DataLakeSeries]:
+    def _resource_cls(self) -> Type[QueryResult]:
         """
         Additional reference to resource class.
         This endpoint deviates from the desired relationship
         that the resource class of the resource container is
         the return type of the get endpoint.
         Therefore, this is only a temporary implementation and will be removed soon.
         """
-        return DataLakeSeries
+        return QueryResult
 
     @property
     def _container_cls(self) -> Type[ResourceContainer]:
         """Defines the model container class the endpoint refers to."""
         return DataLakeMeasures
 
     @property
     def _relative_api_path(self) -> Tuple[str, ...]:
         """Defines the relative api path to the DataLakeMeasurement endpoint.
         Each path within the URL is defined as an own string.
         """
 
         return "api", "v4", "datalake", "measurements"
 
-    def get(self, identifier: str, **kwargs: Optional[Dict[str, Any]]) -> DataLakeSeries:
+    def get(self, identifier: str, **kwargs: Optional[Dict[str, Any]]) -> QueryResult:
         """Queries the specified data lake measure from the API.
 
         By default, the maximum number of returned records is 1000.
         This behaviour can be influenced by passing the parameter `limit` with a different value
         (see [MeasurementGetQueryConfig][streampipes.endpoint.api.data_lake_measure.MeasurementGetQueryConfig]).
 
         Parameters
@@ -328,8 +328,8 @@
         url = f"{self.build_url()}/{identifier}"
 
         # extend base URL by query parameters
         measurement_get_config = self._validate_query_params(query_params=kwargs)
         url += measurement_get_config.build_query_string()
 
         response = self._make_request(request_method=self._parent_client.request_session.get, url=url)
-        return self._resource_cls.from_json(json_string=response.text)
+        return self._resource_cls(**response.json())
```

### Comparing `streampipes-0.91.0/streampipes/endpoint/api/data_stream.py` & `streampipes-0.92.0/streampipes/endpoint/api/data_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """
 Specific implementation of the StreamPipes API's data stream endpoints.
 """
-from typing import Tuple, Type
-
-from streampipes.endpoint.endpoint import APIEndpoint
-from streampipes.model.container import DataStreams
 
 __all__ = [
     "DataStreamEndpoint",
 ]
+from typing import Tuple, Type
 
+from streampipes.endpoint.endpoint import APIEndpoint
+from streampipes.model.container import DataStreams
 from streampipes.model.container.resource_container import ResourceContainer
 
 
 class DataStreamEndpoint(APIEndpoint):
     """Implementation of the DataStream endpoint.
 
     Consequently, it allows querying metadata about available data streams (see `all()` method).
```

### Comparing `streampipes-0.91.0/streampipes/endpoint/endpoint.py` & `streampipes-0.92.0/streampipes/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/endpoint/exceptions.py` & `streampipes-0.92.0/streampipes/endpoint/exceptions.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/endpoint/messaging/__init__.py` & `streampipes-0.92.0/streampipes/endpoint/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/function_zoo/__init__.py` & `streampipes-0.92.0/streampipes/function_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/function_zoo/river_function.py` & `streampipes-0.92.0/streampipes/function_zoo/river_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Any, Callable, Dict, List, Optional
 
 from streampipes.client.client import StreamPipesClient
+from streampipes.functions.broker.broker_handler import get_broker_description
 from streampipes.functions.function_handler import FunctionHandler
 from streampipes.functions.registration import Registration
 from streampipes.functions.streampipes_function import StreamPipesFunction
 from streampipes.functions.utils.data_stream_generator import (
     RuntimeType,
     create_data_stream,
 )
@@ -183,15 +184,20 @@
         self.client = client
 
         attributes = {"learning": RuntimeType.BOOLEAN.value, "prediction": prediction_type}
         if supervised:
             attributes["truth"] = prediction_type
             if target_label is None:
                 raise ValueError("You must define a target attribute for a supervised model.")
-        output_stream = create_data_stream("prediction", attributes)
+
+        output_stream = create_data_stream(
+            name="prediction",
+            attributes=attributes,
+            broker=get_broker_description(client.dataStreamApi.get(stream_ids[0])),  # type: ignore
+        )
         function_definition = FunctionDefinition().add_output_data_stream(output_stream)
         self.sp_function = RiverFunction(
             function_definition, stream_ids, model, supervised, target_label, on_start, on_event, on_stop
         )
 
     def start(self):
         """Registers the function and starts the training."""
```

### Comparing `streampipes-0.91.0/streampipes/functions/__init__.py` & `streampipes-0.92.0/streampipes/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/functions/broker/__init__.py` & `streampipes-0.92.0/streampipes/functions/broker/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from .broker import Broker
-from .kafka_broker import KafkaBroker
-from .nats_broker import NatsBroker
+from .consumer import Consumer
+from .publisher import Publisher
+
+# isort: split
+
+from .kafka.kafka_consumer import KafkaConsumer
+from .kafka.kafka_publisher import KafkaPublisher
+from .nats.nats_consumer import NatsConsumer
+from .nats.nats_publisher import NatsPublisher
 
 from .broker_handler import SupportedBroker, get_broker  # isort: skip
 
 __all__ = [
     "Broker",
-    "KafkaBroker",
-    "NatsBroker",
+    "Consumer",
+    "Publisher",
     "SupportedBroker",
     "get_broker",
+    "KafkaConsumer",
+    "KafkaPublisher",
+    "NatsConsumer",
+    "NatsPublisher",
 ]
```

### Comparing `streampipes-0.91.0/streampipes/functions/broker/broker.py` & `streampipes-0.92.0/streampipes/functions/broker/broker.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
 from abc import ABC, abstractmethod
-from typing import Any, AsyncIterator, Dict
 
 from streampipes.model.resource.data_stream import DataStream
 
 
 class Broker(ABC):
-    """Abstract implementation of a broker.
+    """Abstract implementation of a broker for consumer and publisher.
 
-    A broker allows both to subscribe to a data stream and to publish events to a data stream.
+    It contains the basic logic to connect to a data stream.
     """
 
     async def connect(self, data_stream: DataStream) -> None:
         """Connects to the broker running in StreamPipes.
 
         Parameters
         ----------
@@ -39,20 +38,23 @@
         -------
         None
         """
         self.stream_id = data_stream.element_id
         transport_protocol = data_stream.event_grounding.transport_protocols[0]
         self.topic_name = transport_protocol.topic_definition.actual_topic_name
         hostname = transport_protocol.broker_hostname
+        port = transport_protocol.port
         if "BROKER-HOST" in os.environ.keys():
             hostname = os.environ["BROKER-HOST"]
-        await self._makeConnection(hostname, transport_protocol.port)
+            if "Kafka" in transport_protocol.class_name and "KAFKA-PORT" in os.environ.keys():
+                port = int(os.environ["KAFKA-PORT"])
+        await self._make_connection(hostname, port)
 
     @abstractmethod
-    async def _makeConnection(self, hostname: str, port: int) -> None:
+    async def _make_connection(self, hostname: str, port: int) -> None:
         """Helper function to connect to a server.
 
         Parameters
         ----------
         hostname: str
             The hostname of the server, which the broker connects to.
         port: int
@@ -61,51 +63,15 @@
         Returns
         -------
         None
         """
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
-    async def createSubscription(self) -> None:
-        """Creates a subscription to a data stream.
-
-        Returns
-        -------
-        None
-        """
-        raise NotImplementedError  # pragma: no cover
-
-    @abstractmethod
-    async def publish_event(self, event: Dict[str, Any]) -> None:
-        """Publish an event to a connected data stream.
-
-        Parameters
-        ----------
-        event: Dict[str, Any]
-            The event to be published.
-
-        Returns
-        -------
-        None
-        """
-        raise NotImplementedError  # pragma: no cover
-
-    @abstractmethod
     async def disconnect(self) -> None:
         """Closes the connection to the server.
 
         Returns
         -------
         None
         """
         raise NotImplementedError  # pragma: no cover
-
-    @abstractmethod
-    def get_message(self) -> AsyncIterator:
-        """Get the published messages of the subscription.
-
-        Returns
-        -------
-        iterator: AsyncIterator
-            An async iterator for the messages.
-        """
-        raise NotImplementedError  # pragma: no cover
```

### Comparing `streampipes-0.91.0/streampipes/functions/broker/broker_handler.py` & `streampipes-0.92.0/streampipes/functions/broker/broker_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,34 +12,42 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from enum import Enum
 
-from streampipes.functions.broker import Broker, KafkaBroker, NatsBroker
+from streampipes.functions.broker import (
+    Broker,
+    KafkaConsumer,
+    KafkaPublisher,
+    NatsConsumer,
+    NatsPublisher,
+)
 from streampipes.model.resource.data_stream import DataStream
 
 
 class SupportedBroker(Enum):
     """Enum for the supported brokers."""
 
     NATS = "NatsTransportProtocol"
     KAFKA = "KafkaTransportProtocol"
 
 
 # TODO Exception should be removed once all brokers are implemented.
 class UnsupportedBrokerError(Exception):
     """Exception if a broker isn't implemented yet."""
 
-    def __init__(self, message):
-        super().__init__(message)
+    def __init__(self, broker_name: str):
+        super().__init__(f'The python client doesn\'t support the broker: "{broker_name}" yet')
 
 
-def get_broker(data_stream: DataStream) -> Broker:  # TODO implementation for more transport_protocols
+def get_broker(
+    data_stream: DataStream, is_publisher: bool = False
+) -> Broker:  # TODO implementation for more transport_protocols
     """Derive the broker for the given data stream.
 
     Parameters
     ----------
     data_stream: DataStream
         Data stream instance from which the broker is inferred
 
@@ -51,12 +59,41 @@
     Raises
     ------
     UnsupportedBrokerError
         Is raised when the given data stream belongs to a broker that is currently not supported by StreamPipes Python.
     """
     broker_name = data_stream.event_grounding.transport_protocols[0].class_name
     if SupportedBroker.NATS.value in broker_name:
-        return NatsBroker()
+        if is_publisher:
+            return NatsPublisher()
+        return NatsConsumer()
     elif SupportedBroker.KAFKA.value in broker_name:
-        return KafkaBroker()
+        if is_publisher:
+            return KafkaPublisher()
+        return KafkaConsumer()
     else:
-        raise UnsupportedBrokerError(f'The python client doesn\'t include the broker: "{broker_name}" yet')
+        raise UnsupportedBrokerError(broker_name)
+
+
+def get_broker_description(data_stream: DataStream) -> SupportedBroker:
+    """Derive the decription of the broker for the given data stream.
+
+    Parameters
+    ----------
+    data_stream: DataStream
+        Data stream instance from which the broker is inferred
+
+    Returns
+    -------
+    broker: SupportedBroker
+        The corresponding broker description derived from data stream.
+
+    Raises
+    ------
+    UnsupportedBrokerError
+        Is raised when the given data stream belongs to a broker that is currently not supported by StreamPipes Python.
+    """
+    broker_name = data_stream.event_grounding.transport_protocols[0].class_name
+    for b in SupportedBroker:
+        if b.value in broker_name:
+            return b
+    raise UnsupportedBrokerError(broker_name)
```

### Comparing `streampipes-0.91.0/streampipes/functions/broker/kafka_broker.py` & `streampipes-0.92.0/streampipes/functions/broker/kafka/kafka_consumer.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import logging
-from typing import Any, AsyncIterator, Dict
+from typing import AsyncIterator
 
-from confluent_kafka import Consumer  # type: ignore
-from streampipes.functions.broker.broker import Broker
-from streampipes.functions.broker.kafka_message_fetcher import KafkaMessageFetcher
+from confluent_kafka import Consumer as KafkaConnection  # type: ignore
+from streampipes.functions.broker import Consumer
+from streampipes.functions.broker.kafka.kafka_message_fetcher import KafkaMessageFetcher
 from streampipes.model.common import random_letters
 
 logger = logging.getLogger(__name__)
 
 
-class KafkaBroker(Broker):
-    """Implementation of the broker for Kafka"""
+class KafkaConsumer(Consumer):
+    """Implementation of a consumer for Kafka"""
 
-    async def _makeConnection(self, hostname: str, port: int) -> None:
+    async def _make_connection(self, hostname: str, port: int) -> None:
         """Helper function to connect to a server.
 
         Parameters
         ----------
 
         hostname: str
             The hostname of the server, which the broker connects to.
@@ -41,43 +41,28 @@
         port: int
             The port number of the connection.
 
         Returns
         -------
         None
         """
-        self.kafka_consumer = Consumer(
+        self.kafka_consumer = KafkaConnection(
             {"bootstrap.servers": f"{hostname}:{port}", "group.id": random_letters(6), "auto.offset.reset": "latest"}
         )
+        logger.info(f"Connecting to Kafka at {hostname}:{port}")
 
-    async def createSubscription(self) -> None:
+    async def _create_subscription(self) -> None:
         """Creates a subscription to a data stream.
 
         Returns
         -------
         None
         """
         self.kafka_consumer.subscribe([self.topic_name])
-
-        logger.info(f"Subscribed to stream: {self.stream_id}")
-
-    async def publish_event(self, event: Dict[str, Any]):
-        """Publish an event to a connected data stream.
-
-        Parameters
-        ----------
-        event: Dict[str, Any]
-            The event to be published.
-
-        Returns
-        -------
-        None
-        """
-
-        # await self.publish(subject=self.topic_name, payload=json.dumps(event).encode("utf-8"))
+        logger.info(f"Subscribing to stream: {self.stream_id}")
 
     async def disconnect(self) -> None:
         """Closes the connection to the server.
 
         Returns
         -------
         None
@@ -89,9 +74,8 @@
         """Get the published messages of the subscription.
 
         Returns
         -------
         iterator: AsyncIterator
             An async iterator for the messages.
         """
-
         return KafkaMessageFetcher(self.kafka_consumer)
```

### Comparing `streampipes-0.91.0/streampipes/functions/broker/kafka_message_fetcher.py` & `streampipes-0.92.0/streampipes/functions/broker/kafka/kafka_message_fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,9 +42,11 @@
     def __init__(self, consumer: Consumer):
         self.consumer = consumer
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
-        msg = self.consumer.poll(0.1)
+        msg = None
+        while not msg:
+            msg = self.consumer.poll(0.1)
         return KafkaMessage(msg.value())
```

### Comparing `streampipes-0.91.0/streampipes/functions/broker/nats_broker.py` & `streampipes-0.92.0/streampipes/functions/broker/nats/nats_consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import json
 import logging
-from typing import Any, AsyncIterator, Dict
+from typing import AsyncIterator
 
 from nats import connect
-from streampipes.functions.broker.broker import Broker
+from streampipes.functions.broker import Consumer
 
 logger = logging.getLogger(__name__)
 
 
-class NatsBroker(Broker):
-    """Implementation of the NatsBroker"""
+class NatsConsumer(Consumer):
+    """Implementation of a consumer for NATS"""
 
-    async def _makeConnection(self, hostname: str, port: int) -> None:
+    async def _make_connection(self, hostname: str, port: int) -> None:
         """Helper function to connect to a server.
 
         Parameters
         ----------
 
         hostname: str
             The hostname of the server, which the broker connects to.
@@ -41,43 +40,27 @@
 
         Returns
         -------
         None
 
         """
         self.nats_client = await connect(f"nats://{hostname}:{port}")
-        if self.nats_client.connected_url is not None:
-            logger.info(f"Connected to NATS at {self.nats_client.connected_url.netloc}")
+        logger.info(f"Connecting to NATS at {hostname}:{port}")
 
-    async def createSubscription(self) -> None:
+    async def _create_subscription(self) -> None:
         """Creates a subscription to a data stream.
 
         Returns
         -------
         None
 
         """
         self.subscription = await self.nats_client.subscribe(self.topic_name)
         logger.info(f"Subscribed to stream: {self.stream_id}")
 
-    async def publish_event(self, event: Dict[str, Any]):
-        """Publish an event to a connected data stream.
-
-        Parameters
-        ----------
-        event: Dict[str, Any]
-            The event to be published.
-
-        Returns
-        -------
-        None
-
-        """
-        await self.nats_client.publish(subject=self.topic_name, payload=json.dumps(event).encode("utf-8"))
-
     async def disconnect(self) -> None:
         """Closes the connection to the server.
 
         Returns
         -------
         None
         """
```

### Comparing `streampipes-0.91.0/streampipes/functions/broker/output_collector.py` & `streampipes-0.92.0/streampipes/functions/broker/output_collector.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,60 +13,60 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import asyncio
 from typing import Any, Coroutine, Dict
 
-from streampipes.functions.broker import get_broker
+from streampipes.functions.broker import Publisher, get_broker
 from streampipes.model.resource.data_stream import DataStream
 
 
 class OutputCollector:
     """Collector for output events. The events are published to an output data stream.
     Therefore, the output collector establishes a connection to the broker.
 
     Parameters
     ----------
     data_stream: DataStream
         The output data stream that will receive the events.
 
     Attributes
     ----------
-    broker: Broker
-        The broker instance that sends the data to StreamPipes
+    publisher: Publisher
+        The publisher instance that sends the data to StreamPipes
 
     """
 
     def __init__(self, data_stream: DataStream) -> None:
-        self.broker = get_broker(data_stream)
-        self._run_coroutine(self.broker.connect(data_stream))
+        self.publisher: Publisher = get_broker(data_stream, is_publisher=True)  # type: ignore
+        self._run_coroutine(self.publisher.connect(data_stream))
 
     def collect(self, event: Dict[str, Any]) -> None:
         """Publishes an event to the output stream.
 
         Parameters
         ----------
         event: Dict[str, Any]
             The event to be published.
 
         Returns
         -------
         None
         """
-        self._run_coroutine(self.broker.publish_event(event))
+        self._run_coroutine(self.publisher.publish_event(event))
 
     def disconnect(self) -> None:
         """Disconnects the broker of the output collector.
 
         Returns
         -------
         None
         """
-        self._run_coroutine(self.broker.disconnect())
+        self._run_coroutine(self.publisher.disconnect())
 
     @staticmethod
     def _run_coroutine(coroutine: Coroutine) -> None:
         """Run a coroutine in the event loop or create a new one if there is a running event loop.
 
         Parameters
         ----------
```

### Comparing `streampipes-0.91.0/streampipes/functions/function_handler.py` & `streampipes-0.92.0/streampipes/functions/function_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 import asyncio
 import json
 import logging
 from typing import AsyncIterator, Dict, List
 
 from streampipes.client.client import StreamPipesClient
-from streampipes.functions.broker import Broker, get_broker
+from streampipes.functions.broker import Broker, Consumer, get_broker
 from streampipes.functions.registration import Registration
 from streampipes.functions.utils.async_iter_handler import AsyncIterHandler
 from streampipes.functions.utils.data_stream_context import DataStreamContext
 from streampipes.functions.utils.function_context import FunctionContext
 from streampipes.model.resource.data_stream import DataStream
 
 logger = logging.getLogger(__name__)
@@ -73,15 +73,15 @@
                     f'for the function "{streampipes_function.getFunctionId().id}"'
                 )
             # Choose the broker and collect the schema for every data stream
             for stream_id in streampipes_function.requiredStreamIds():
                 # Get the data stream schema from the API
                 data_stream: DataStream = self.client.dataStreamApi.get(stream_id)  # type: ignore
                 # Get the broker
-                broker = get_broker(data_stream)
+                broker: Consumer = get_broker(data_stream)  # type: ignore
                 # Assign the functions, broker and schema to every stream
                 if stream_id in self.stream_contexts.keys():
                     self.stream_contexts[stream_id].add_function(streampipes_function)
                 else:
                     self.stream_contexts[stream_id] = DataStreamContext(
                         functions=[streampipes_function], schema=data_stream, broker=broker
                     )
@@ -106,15 +106,14 @@
         contexts: Dict[str, FunctionContext] = dict()
 
         for stream_id in self.stream_contexts.keys():
             data_stream = self.stream_contexts[stream_id].schema
             broker = self.stream_contexts[stream_id].broker
             # Connect the broker
             await broker.connect(data_stream)
-            await broker.createSubscription()
             self.brokers.append(broker)
             # Get the messages
             messages[stream_id] = broker.get_message()
             # Generate the function context
             for streampipes_function in self.stream_contexts[stream_id].functions:
                 function_id = streampipes_function.getFunctionId().id
                 if function_id in contexts.keys():
```

### Comparing `streampipes-0.91.0/streampipes/functions/registration.py` & `streampipes-0.92.0/streampipes/functions/registration.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/functions/streampipes_function.py` & `streampipes-0.92.0/streampipes/functions/streampipes_function.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/functions/utils/__init__.py` & `streampipes-0.92.0/streampipes/functions/broker/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/functions/utils/async_iter_handler.py` & `streampipes-0.92.0/streampipes/functions/utils/async_iter_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         Returns
         -------
         result: Tuple[str, Optional[Any]]
             Tuple of the stream id und next message or `("stop", None)` if no message is left.
         """
         try:
             return stream_id, await message.__anext__()
-        except StopAsyncIteration:
+        except (StopAsyncIteration, RuntimeError):
             return "stop", None
 
     @staticmethod
     async def combine_async_messages(messages: Dict[str, AsyncIterator]) -> AsyncGenerator:
         """Continuously gets the next published message from multiple AsyncIterators in parallel.
 
         Parameters
```

### Comparing `streampipes-0.91.0/streampipes/functions/utils/data_stream_context.py` & `streampipes-0.92.0/streampipes/functions/utils/data_stream_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import List
 
-from streampipes.functions.broker.broker import Broker
+from streampipes.functions.broker import Consumer
 from streampipes.functions.streampipes_function import StreamPipesFunction
 from streampipes.model.resource.data_stream import DataStream
 
 
 class DataStreamContext:
     """Container for the context of a data stream.
 
     Parameters
     ----------
     functions: List[StreamPipesFunction]
         StreamPipes Functions which require the data of this data stream.
     schema: DataStream
         The schema of this data stream.
-    broker: Broker
-        The broker to connect to this data stream.
+    broker: Consumer
+        The consumer to connect to this data stream.
     """
 
-    def __init__(self, functions: List[StreamPipesFunction], schema: DataStream, broker: Broker) -> None:
+    def __init__(self, functions: List[StreamPipesFunction], schema: DataStream, broker: Consumer) -> None:
         self.functions = functions
         self.schema = schema
         self.broker = broker
 
     def add_function(self, function: StreamPipesFunction):
         """Adds a new StreamPipes Function.
```

### Comparing `streampipes-0.91.0/streampipes/functions/utils/data_stream_generator.py` & `streampipes-0.92.0/streampipes/functions/utils/data_stream_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from enum import Enum
 from typing import Dict, Optional
 
-from streampipes.model.common import EventProperty, EventSchema
+from streampipes.functions.broker import SupportedBroker
+from streampipes.model.common import (
+    EventGrounding,
+    EventProperty,
+    EventSchema,
+    TransportProtocol,
+)
 from streampipes.model.resource.data_stream import DataStream
 
 
 class RuntimeType(Enum):
     """Runtime type names for the attributes of a data stream.
 
     Attributes
@@ -40,15 +46,20 @@
     DOUBLE = "double"
     FLOAT = "float"
     INTEGER = "integer"
     LONG = "long"
 
 
 # TODO Use an more general approach to create a data stream
-def create_data_stream(name: str, attributes: Dict[str, str], stream_id: Optional[str] = None):
+def create_data_stream(
+    name: str,
+    attributes: Dict[str, str],
+    stream_id: Optional[str] = None,
+    broker: SupportedBroker = SupportedBroker.NATS,
+):
     """Creates a data stream
 
     Parameters
     ----------
     name: str
         Name of the data stream to be shown at the UI.
     attributes: Dict[str, str]
@@ -60,29 +71,42 @@
     -------
     data_stream: DataStream
         The created data stream
     """
 
     event_schema = EventSchema(
         event_properties=[
-            EventProperty(
+            EventProperty(  # type: ignore
                 label="timestamp",
                 runtime_name="timestamp",
                 domain_properties=["http://schema.org/DateTime"],
                 property_scope="HEADER_PROPERTY",
                 runtime_type="http://www.w3.org/2001/XMLSchema#long",
             )
         ]
         + [
-            EventProperty(
+            EventProperty(  # type: ignore
                 label=attribute_name,
                 runtime_name=attribute_name,
                 index=i,
                 runtime_type=f"http://www.w3.org/2001/XMLSchema#{attribute_type}",
             )
             for i, (attribute_name, attribute_type) in enumerate(attributes.items(), start=1)
         ]
     )
 
-    if not stream_id:
-        return DataStream(name=name, event_schema=event_schema)
-    return DataStream(element_id=stream_id, name=name, event_schema=event_schema)
+    transport_protocols = [TransportProtocol()]
+    if broker == SupportedBroker.KAFKA:
+        transport_protocols = [
+            TransportProtocol(
+                class_name="org.apache.streampipes.model.grounding.KafkaTransportProtocol",  # type: ignore
+                broker_hostname="kafka",
+                port=9092,
+            )
+        ]
+
+    data_stream = DataStream(
+        name=name, event_schema=event_schema, event_grounding=EventGrounding(transport_protocols=transport_protocols)
+    )
+    if stream_id:
+        data_stream.element_id = stream_id
+    return data_stream
```

### Comparing `streampipes-0.91.0/streampipes/functions/utils/function_context.py` & `streampipes-0.92.0/streampipes/functions/utils/function_context.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/__init__.py` & `streampipes-0.92.0/streampipes/functions/broker/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/common.py` & `streampipes-0.92.0/streampipes/model/common.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/container/__init__.py` & `streampipes-0.92.0/streampipes/model/container/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from .data_lake_measures import DataLakeMeasures
 from .data_streams import DataStreams
+from .versions import Versions
 
 __all__ = [
     "DataLakeMeasures",
     "DataStreams",
+    "Versions",
 ]
```

### Comparing `streampipes-0.91.0/streampipes/model/container/data_lake_measures.py` & `streampipes-0.92.0/streampipes/model/container/data_lake_measures.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/container/data_streams.py` & `streampipes-0.92.0/streampipes/model/container/data_streams.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/container/resource_container.py` & `streampipes-0.92.0/streampipes/model/container/resource_container.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/resource/__init__.py` & `streampipes-0.92.0/streampipes/model/resource/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from .data_lake_measure import DataLakeMeasure
-from .data_lake_series import DataLakeSeries
+from .data_series import DataSeries
 from .data_stream import DataStream
 from .function_definition import FunctionDefinition
+from .version import Version
 
 __all__ = [
     "DataLakeMeasure",
-    "DataLakeSeries",
+    "DataSeries",
     "DataStream",
     "FunctionDefinition",
+    "Version",
 ]
```

### Comparing `streampipes-0.91.0/streampipes/model/resource/data_lake_measure.py` & `streampipes-0.92.0/streampipes/model/resource/data_lake_measure.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/resource/data_lake_series.py` & `streampipes-0.92.0/streampipes/model/resource/data_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,64 +18,53 @@
 from __future__ import annotations
 
 import json
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 from pydantic import StrictInt, StrictStr
+from streampipes.model.resource.exceptions import StreamPipesUnsupportedDataSeries
 from streampipes.model.resource.resource import Resource
 
 __all__ = [
-    "DataLakeSeries",
+    "DataSeries",
 ]
 
 
-class StreamPipesUnsupportedDataLakeSeries(Exception):
-    """Exception to be raised when the returned data lake series
-    cannot be parsed with the current implementation of the resource.
-    """
-
-    def __init__(self):
-        super().__init__(
-            "The Data Lake series returned by the API appears "
-            "to have a structure that is not currently supported by the Python client."
-        )
-
-
-class DataLakeSeries(Resource):
-    """Implementation of a resource for data lake series.
+class DataSeries(Resource):
+    """Implementation of a resource for data series.
     This resource defines the data model used by its resource container(`model.container.DataLakeMeasures`).
     It inherits from Pydantic's BaseModel to get all its superpowers,
     which are used to parse, validate the API response and to easily switch between
     the Python representation (both serialized and deserialized) and Java representation (serialized only).
 
     Notes
     ------
-        This class will only exist temporarily it its current appearance since
+        This class will only exist temporarily in it its current appearance since
         there are some inconsistencies in the StreamPipes API.
 
     """
 
     @classmethod
-    def from_json(cls, json_string: str) -> DataLakeSeries:
-        """Creates an instance of `DataLakeSeries` from a given JSON string.
+    def from_json(cls, json_string: str) -> DataSeries:
+        """Creates an instance of `DataSeries` from a given JSON string.
 
         This method is used by the resource container to parse the JSON response of
         the StreamPipes API.
         Currently, it only supports data lake series that consist of exactly one series of data.
 
         Parameters
         ----------
         json_string: str
             The JSON string the data lake series should be created on.
 
         Returns
         -------
-        DataLakeSeries
-            Instance of `DataLakeSeries` that is created based on the given JSON string.
+        DataSeries
+            Instance of `DataSeries` that is created based on the given JSON string.
 
         Raises
         ------
         StreamPipesUnsupportedDataLakeSeries
             If the data lake series returned by the StreamPipes API cannot be parsed
             with the current version of the Python client.
 
@@ -83,15 +72,15 @@
 
         # deserialize JSON string
         parsed_json = json.loads(json_string)
 
         # check if the provided JSON has only one data series entry
         # otherwise raise the proper exception
         if len(parsed_json["allDataSeries"]) != 1:
-            raise StreamPipesUnsupportedDataLakeSeries()
+            raise StreamPipesUnsupportedDataSeries()
 
         # get the data data series
         data_series = parsed_json["allDataSeries"][0]
 
         return cls.parse_obj(data_series)
 
     def convert_to_pandas_representation(self) -> Dict[str, Union[List[str], List[List[Any]]]]:
```

### Comparing `streampipes-0.91.0/streampipes/model/resource/data_stream.py` & `streampipes-0.92.0/streampipes/model/resource/data_stream.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/resource/function_definition.py` & `streampipes-0.92.0/streampipes/model/resource/function_definition.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes/model/resource/resource.py` & `streampipes-0.92.0/streampipes/model/resource/resource.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/streampipes.egg-info/PKG-INFO` & `streampipes-0.92.0/streampipes.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streampipes
-Version: 0.91.0
+Version: 0.92.0
 Summary: Python library for Apache StreamPipes
 Home-page: https://streampipes.apache.org/docs/docs/python/latest/
 Author: Apache Software Foundation
 Author-email: dev@streampipes.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://streampipes.apache.org/docs/docs/python/latest/
 Project-URL: Bug Tracker, https://github.com/apache/streampipes/issues
@@ -60,36 +60,61 @@
 
 <br>
 <h3 align="center">Apache StreamPipes for Python</h3>
 
 <p align="center"> Apache StreamPipes meets Python! We are working highly motivated on a Python library to interact with StreamPipes.
 In this way, we would like to unite the power of StreamPipes to easily connect to and read different data sources, especially in the IoT domain,
 and the amazing universe of data analytics libraries in Python. </p>
+<br>
+
+<p align="center">
+<a href="https://github.com/apache/streampipes/tree/dev/streampipes-client-python" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/streampipes" alt="Supported Python versions">
+</a>
+<a href="https://pypi.org/project/streampipes/" target="_blank">
+    <img src="https://img.shields.io/pypi/v/streampipes" alt="Current PyPI version">
+</a>
+<a href="https://streampipes.apache.org/docs/docs/python/latest/" target="_blank">
+    <img src="https://github.com/apache/streampipes-website/actions/workflows/update-python-docs.yml/badge.svg" alt="Status Python Docs">
+</a>
+<a href="https://github.com/psf/black" target="_blank">
+    <img src="https://img.shields.io/badge/code%20style-black-black" alt="Code Style: Black">
+</a>
+<a href="https://github.com/python/mypy" target="_blank">
+    <img src="https://img.shields.io/badge/typed-mypy-blue" alt="Typed: MyPy">
+</a>
+<img src="./docs/img/interrogate_badge.svg" alt= “interrogate” height="20">
+<a href="https://pypi.org/project/streampipes/" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/streampipes" alt="Downloads: PyPI/Month">
+</a>
+</p>
 
 ---
 
 <br>
 
-**💡The current version of this Python client is still a beta version.**
-<br>
-**This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.**
+<h4 align="center">💡The current version of this Python client is still a beta version.</h4>
+<h4 align="center">This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.</h4>
+
 <br>
 
 
 ## 📚 Documentation
-Please visit our documentation: https://streampipes.apache.org/docs/docs/python/latest/
+Please visit our [documentation](https://streampipes.apache.org/docs/docs/python/latest/).
 There you can find information about how to [get started](https://streampipes.apache.org/docs/docs/python/latest/getting-started/first-steps/),
 follow some [tutorials](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/),
 or discover the library via our [references](https://streampipes.apache.org/docs/docs/python/latest/reference/client/client/).
 <br>
 
 In case you want to access the documentation of the current development state, you can go here:
 
 👉 [development docs 🤓](https://streampipes.apache.org/docs/docs/python/dev/)
 
+<br>
+
 ## ⚡️ Quickstart
 
 As a quick example, we demonstrate how to set up and configure a StreamPipes client.
 
 You can simply install the StreamPipes library by running the following command
 ```bash
 pip install streampipes
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streampipes Version: 0.91.0 Summary: Python library
+Metadata-Version: 2.1 Name: streampipes Version: 0.92.0 Summary: Python library
 for Apache StreamPipes Home-page: https://streampipes.apache.org/docs/docs/
 python/latest/ Author: Apache Software Foundation Author-email:
 dev@streampipes.apache.org License: Apache License 2.0 Project-URL:
 Documentation, https://streampipes.apache.org/docs/docs/python/latest/ Project-
 URL: Bug Tracker, https://github.com/apache/streampipes/issues Project-URL:
 Source Code, https://github.com/apache/streampipes Keywords:
 streampipes,iot,iiot,analytics,stream-processing,apache Classifier: Development
@@ -24,39 +24,44 @@
 
                     **** Apache StreamPipes for Python ****
  Apache StreamPipes meets Python! We are working highly motivated on a Python
  library to interact with StreamPipes. In this way, we would like to unite the
   power of StreamPipes to easily connect to and read different data sources,
    especially in the IoT domain, and the amazing universe of data analytics
                              libraries in Python.
+
+ [Supported_Python_versions] [Current_PyPI_version] [Status_Python_Docs] [Code
+    Style:_Black] [Typed:_MyPy] [âinterrogateâ] [Downloads:_PyPI/Month]
 ---
-**ð¡The current version of this Python client is still a beta version.**
-**This means that it is still under development, which may result in frequent
-and extensive API changes, unstable behavior, etc.**
-## ð Documentation Please visit our documentation: https://
-streampipes.apache.org/docs/docs/python/latest/ There you can find information
-about how to [get started](https://streampipes.apache.org/docs/docs/python/
-latest/getting-started/first-steps/), follow some [tutorials](https://
-streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
-streampipes-python-client/), or discover the library via our [references]
-(https://streampipes.apache.org/docs/docs/python/latest/reference/client/
-client/).
+*** ð¡The current version of this Python client is still a beta version. ***
+*** This means that it is still under development, which may result in frequent
+            and extensive API changes, unstable behavior, etc. ***
+
+## ð Documentation Please visit our [documentation](https://
+streampipes.apache.org/docs/docs/python/latest/). There you can find
+information about how to [get started](https://streampipes.apache.org/docs/
+docs/python/latest/getting-started/first-steps/), follow some [tutorials]
+(https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-
+introduction-to-streampipes-python-client/), or discover the library via our
+[references](https://streampipes.apache.org/docs/docs/python/latest/reference/
+client/client/).
 In case you want to access the documentation of the current development state,
 you can go here: ð [development docs ð¤](https://streampipes.apache.org/
-docs/docs/python/dev/) ## â¡ï¸ Quickstart As a quick example, we demonstrate
-how to set up and configure a StreamPipes client. You can simply install the
-StreamPipes library by running the following command ```bash pip install
-streampipes # if you want to have the current development state you can also
-execute pip install git+https://github.com/apache/
-streampipes.git#subdirectory=streampipes-client-python ``` ```python from
-streampipes.client import StreamPipesClient from streampipes.client.config
-import StreamPipesClientConfig from streampipes.client.credential_provider
-import StreamPipesApiKeyCredentials config = StreamPipesClientConfig
-( credential_provider = StreamPipesApiKeyCredentials( username =
-"test@streampipes.apache.org", api_key = "DEMO-KEY", ), host_address =
-"localhost", https_disabled = True, port = 80 ) client = StreamPipesClient
-(client_config=config) client.describe() ``` Output: ``` Hi there! You are
-connected to a StreamPipes instance running at http://localhost:80. The
-following StreamPipes resources are available with this client: 6x DataStreams
-1x DataLakeMeasures ``` For more information about how to use the StreamPipes
-client visit our [introduction tutorial](https://streampipes.apache.org/docs/
-docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
+docs/docs/python/dev/)
+## â¡ï¸ Quickstart As a quick example, we demonstrate how to set up and
+configure a StreamPipes client. You can simply install the StreamPipes library
+by running the following command ```bash pip install streampipes # if you want
+to have the current development state you can also execute pip install
+git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-
+python ``` ```python from streampipes.client import StreamPipesClient from
+streampipes.client.config import StreamPipesClientConfig from
+streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+config = StreamPipesClientConfig( credential_provider =
+StreamPipesApiKeyCredentials( username = "test@streampipes.apache.org", api_key
+= "DEMO-KEY", ), host_address = "localhost", https_disabled = True, port = 80 )
+client = StreamPipesClient(client_config=config) client.describe() ``` Output:
+``` Hi there! You are connected to a StreamPipes instance running at http://
+localhost:80. The following StreamPipes resources are available with this
+client: 6x DataStreams 1x DataLakeMeasures ``` For more information about how
+to use the StreamPipes client visit our [introduction tutorial](https://
+streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
+streampipes-python-client/).
```

### Comparing `streampipes-0.91.0/streampipes.egg-info/requires.txt` & `streampipes-0.92.0/streampipes.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,83 +6,83 @@
 
 [all]
 pandas>=1.5.1
 pydantic>=1.10.2
 requests>=2.28.1
 nats-py>=2.2.0
 confluent-kafka>=2.0.2
-autoflake==2.0.0
-black==23.1.0
+autoflake==2.1.0
+black==23.3.0
 blacken-docs==1.13.0
 flake8==6.0.0
-interrogate==1.5.0
+interrogate[png]==1.5.0
 isort==5.12.0
-mypy==1.0.0
-pandas-stubs==1.5.2.230105
-pre-commit==3.0.0
-pytest==7.2.1
+mypy==1.3.0
+pandas-stubs==2.0.0.230412
+pre-commit==3.3.0
+pytest==7.3.0
 pytest-cov==4.0.0
-pyupgrade==3.3.1
+pyupgrade==3.4.0
 types-Jinja2==2.11.9
-types-requests==2.28.11.7
+types-requests==2.30.0.0
 mkdocs==1.4.2
-mkdocs-awesome-pages-plugin==2.8.0
-mkdocs-material==8.5.11
-mkdocstrings[python]==0.20.0
+mkdocs-awesome-pages-plugin==2.9.0
+mkdocs-material==9.1.3
+mkdocstrings[python]==0.21.1
 pytkdocs[numpy-style]>=0.16.1
-mkdocs-gen-files==0.4.0
+mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.0
 numpydoc==1.5.0
-mkdocs-jupyter==0.22.0
+mkdocs-jupyter==0.24.0
 
 [dev]
 pandas>=1.5.1
 pydantic>=1.10.2
 requests>=2.28.1
 nats-py>=2.2.0
 confluent-kafka>=2.0.2
-autoflake==2.0.0
-black==23.1.0
+autoflake==2.1.0
+black==23.3.0
 blacken-docs==1.13.0
 flake8==6.0.0
-interrogate==1.5.0
+interrogate[png]==1.5.0
 isort==5.12.0
-mypy==1.0.0
-pandas-stubs==1.5.2.230105
-pre-commit==3.0.0
-pytest==7.2.1
+mypy==1.3.0
+pandas-stubs==2.0.0.230412
+pre-commit==3.3.0
+pytest==7.3.0
 pytest-cov==4.0.0
-pyupgrade==3.3.1
+pyupgrade==3.4.0
 types-Jinja2==2.11.9
-types-requests==2.28.11.7
+types-requests==2.30.0.0
 
 [docs]
 mkdocs==1.4.2
-mkdocs-awesome-pages-plugin==2.8.0
-mkdocs-material==8.5.11
-mkdocstrings[python]==0.20.0
+mkdocs-awesome-pages-plugin==2.9.0
+mkdocs-material==9.1.3
+mkdocstrings[python]==0.21.1
 pytkdocs[numpy-style]>=0.16.1
-mkdocs-gen-files==0.4.0
+mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.0
 numpydoc==1.5.0
-mkdocs-jupyter==0.22.0
+mkdocs-jupyter==0.24.0
 
 [test]
 pandas>=1.5.1
 pydantic>=1.10.2
 requests>=2.28.1
 nats-py>=2.2.0
 confluent-kafka>=2.0.2
-autoflake==2.0.0
-black==23.1.0
+autoflake==2.1.0
+black==23.3.0
 blacken-docs==1.13.0
 flake8==6.0.0
-interrogate==1.5.0
+interrogate[png]==1.5.0
 isort==5.12.0
-mypy==1.0.0
-pandas-stubs==1.5.2.230105
-pre-commit==3.0.0
-pytest==7.2.1
+mypy==1.3.0
+pandas-stubs==2.0.0.230412
+pre-commit==3.3.0
+pytest==7.3.0
 pytest-cov==4.0.0
-pyupgrade==3.3.1
+pyupgrade==3.4.0
 types-Jinja2==2.11.9
-types-requests==2.28.11.7
+types-requests==2.30.0.0
```

### Comparing `streampipes-0.91.0/tests/client/__init__.py` & `streampipes-0.92.0/streampipes/functions/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/tests/endpoint/__init__.py` & `streampipes-0.92.0/streampipes/model/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.91.0/tests/functions/__init__.py` & `streampipes-0.92.0/streampipes/py.typed`

 * *Files 1% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+#
```

