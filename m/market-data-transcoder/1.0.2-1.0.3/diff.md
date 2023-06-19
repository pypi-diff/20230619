# Comparing `tmp/market-data-transcoder-1.0.2.tar.gz` & `tmp/market-data-transcoder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-data-transcoder-1.0.2.tar", last modified: Thu Apr 20 20:42:58 2023, max compression
+gzip compressed data, was "market-data-transcoder-1.0.3.tar", last modified: Mon Jun 19 13:45:51 2023, max compression
```

## Comparing `market-data-transcoder-1.0.2.tar` & `market-data-transcoder-1.0.3.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.637516 market-data-transcoder-1.0.2/
--rw-r--r--   0 mservidio   (501) staff       (20)    11357 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/LICENSE
--rw-r--r--   0 mservidio   (501) staff       (20)    13254 2023-04-20 20:42:58.637649 market-data-transcoder-1.0.2/PKG-INFO
--rw-r--r--   0 mservidio   (501) staff       (20)    12376 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/README.md
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.623352 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/
--rw-r--r--   0 mservidio   (501) staff       (20)    13254 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/PKG-INFO
--rw-r--r--   0 mservidio   (501) staff       (20)     4188 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/SOURCES.txt
--rw-r--r--   0 mservidio   (501) staff       (20)        1 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/dependency_links.txt
--rw-r--r--   0 mservidio   (501) staff       (20)       48 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/entry_points.txt
--rw-r--r--   0 mservidio   (501) staff       (20)        1 2023-04-20 20:22:51.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/not-zip-safe
--rw-r--r--   0 mservidio   (501) staff       (20)      149 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/requires.txt
--rw-r--r--   0 mservidio   (501) staff       (20)       23 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/top_level.txt
--rw-r--r--   0 mservidio   (501) staff       (20)      101 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/pyproject.toml
--rw-r--r--   0 mservidio   (501) staff       (20)     1263 2023-04-20 20:42:58.638472 market-data-transcoder-1.0.2/setup.cfg
--rw-r--r--   0 mservidio   (501) staff       (20)     1075 2023-04-20 20:41:12.000000 market-data-transcoder-1.0.2/setup.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.623486 market-data-transcoder-1.0.2/third_party/
--rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.624209 market-data-transcoder-1.0.2/third_party/pyfixmsg/
--rw-r--r--   0 mservidio   (501) staff       (20)     6276 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.624449 market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/
--rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/__init__.py
--rw-r--r--   0 mservidio   (501) staff       (20)    13965 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/stringfix.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.624718 market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/
--rw-r--r--   0 mservidio   (501) staff       (20)      945 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/__init__.py
--rw-r--r--   0 mservidio   (501) staff       (20)    18449 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/fixmessage.py
--rw-r--r--   0 mservidio   (501) staff       (20)     6960 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/parser.py
--rw-r--r--   0 mservidio   (501) staff       (20)    18582 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/reference.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1079 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/util.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.625469 market-data-transcoder-1.0.2/third_party/sbedecoder/
--rw-r--r--   0 mservidio   (501) staff       (20)      154 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/__init__.py
--rw-r--r--   0 mservidio   (501) staff       (20)    22959 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/message.py
--rw-r--r--   0 mservidio   (501) staff       (20)     5317 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/parser.py
--rw-r--r--   0 mservidio   (501) staff       (20)    27955 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/schema.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1326 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/typemap.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.626116 market-data-transcoder-1.0.2/transcoder/
--rw-r--r--   0 mservidio   (501) staff       (20)    11989 2023-04-20 19:43:43.000000 market-data-transcoder-1.0.2/transcoder/Transcoder.py
--rw-r--r--   0 mservidio   (501) staff       (20)      915 2023-04-20 20:38:35.000000 market-data-transcoder-1.0.2/transcoder/__init__.py
--rwxr-xr-x   0 mservidio   (501) staff       (20)    12218 2023-04-20 19:42:58.000000 market-data-transcoder-1.0.2/transcoder/main.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.627446 market-data-transcoder-1.0.2/transcoder/message/
--rw-r--r--   0 mservidio   (501) staff       (20)     1709 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/DatacastField.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2756 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/DatacastGroup.py
--rw-r--r--   0 mservidio   (501) staff       (20)     5117 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/DatacastParser.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1163 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/DatacastSchema.py
--rw-r--r--   0 mservidio   (501) staff       (20)     3775 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/ErrorWriter.py
--rw-r--r--   0 mservidio   (501) staff       (20)     3280 2023-04-20 19:45:10.000000 market-data-transcoder-1.0.2/transcoder/message/MessageUtil.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1335 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/NoParser.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1452 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/ParsedMessage.py
--rw-r--r--   0 mservidio   (501) staff       (20)      921 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.627881 market-data-transcoder-1.0.2/transcoder/message/exception/
--rw-r--r--   0 mservidio   (501) staff       (20)      974 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/exception/MessageParserNotDefinedError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      927 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/exception/ParserFunctionNotDefinedError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      959 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/exception/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.628731 market-data-transcoder-1.0.2/transcoder/message/factory/
--rw-r--r--   0 mservidio   (501) staff       (20)     1595 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/CmeMessageFactory.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1762 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/factory/ITCHMessageFactory.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2001 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/MDPMessageFactory.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1576 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/MemxMessageFactory.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1687 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/factory/MessageFactory.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1319 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/factory/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.629179 market-data-transcoder-1.0.2/transcoder/message/factory/exception/
--rw-r--r--   0 mservidio   (501) staff       (20)      915 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/exception/FactoryNotFoundError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      946 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      920 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/exception/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.630551 market-data-transcoder-1.0.2/transcoder/message/handler/
--rw-r--r--   0 mservidio   (501) staff       (20)     2269 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/CmeBinaryPacketHandler.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2287 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/FilterHandler.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1731 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandler.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1423 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerFloatField.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1417 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerIntField.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1424 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerStringField.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2137 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/SequencerHandler.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2151 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/TimestampPullForwardHandler.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1063 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.630995 market-data-transcoder-1.0.2/transcoder/output/
--rw-r--r--   0 mservidio   (501) staff       (20)     4536 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/output/OutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)     4975 2023-04-20 20:10:00.000000 market-data-transcoder-1.0.2/transcoder/output/OutputUtil.py
--rw-r--r--   0 mservidio   (501) staff       (20)      955 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/output/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.631615 market-data-transcoder-1.0.2/transcoder/output/avro/
--rw-r--r--   0 mservidio   (501) staff       (20)     1843 2023-04-20 20:30:03.000000 market-data-transcoder-1.0.2/transcoder/output/avro/AvroOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2736 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/avro/BaseAvroOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1756 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/avro/FastAvroOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)      953 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/avro/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.631933 market-data-transcoder-1.0.2/transcoder/output/diag/
--rw-r--r--   0 mservidio   (501) staff       (20)     1158 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/diag/DiagnosticOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)      908 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/diag/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.633464 market-data-transcoder-1.0.2/transcoder/output/exception/
--rw-r--r--   0 mservidio   (501) staff       (20)      983 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/BigQueryTableSchemaOutOfSyncError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      943 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/OutputFunctionNotDefinedError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      909 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/OutputManagerSchemaError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      953 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/OutputNotAvailableError.py
--rw-r--r--   0 mservidio   (501) staff       (20)      979 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/PubSubTopicSchemaOutOfSyncError.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1202 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.634238 market-data-transcoder-1.0.2/transcoder/output/google_cloud/
--rw-r--r--   0 mservidio   (501) staff       (20)     6504 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/BigQueryOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1016 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/Constants.py
--rw-r--r--   0 mservidio   (501) staff       (20)    12040 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/PubSubOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)      957 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.634859 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/
--rw-r--r--   0 mservidio   (501) staff       (20)     2792 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2118 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2892 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)      993 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.635140 market-data-transcoder-1.0.2/transcoder/output/json/
--rw-r--r--   0 mservidio   (501) staff       (20)     3559 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/json/JsonOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)      896 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/json/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.635435 market-data-transcoder-1.0.2/transcoder/output/length_delimited/
--rw-r--r--   0 mservidio   (501) staff       (20)     1909 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/output/length_delimited/LengthDelimitedOutputManager.py
--rw-r--r--   0 mservidio   (501) staff       (20)      918 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/output/length_delimited/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.636011 market-data-transcoder-1.0.2/transcoder/source/
--rw-r--r--   0 mservidio   (501) staff       (20)     1189 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/LineEncoding.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1826 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/source/Source.py
--rw-r--r--   0 mservidio   (501) staff       (20)     3776 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/SourceUtil.py
--rw-r--r--   0 mservidio   (501) staff       (20)      914 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/__init__.py
-drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.637389 market-data-transcoder-1.0.2/transcoder/source/file/
--rw-r--r--   0 mservidio   (501) staff       (20)     3867 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/CmeBinaryPacketFileMessageSource.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2623 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/FileMessageSource.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2630 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/LengthDelimitedFileMessageSource.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2719 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/LineDelimitedFileMessageSource.py
--rw-r--r--   0 mservidio   (501) staff       (20)     2295 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/PcapFileMessageSource.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1186 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/source/file/__init__.py
--rw-r--r--   0 mservidio   (501) staff       (20)     1624 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/test.py
--rw-r--r--   0 mservidio   (501) staff       (20)      837 2023-04-20 19:51:40.000000 market-data-transcoder-1.0.2/transcoder/version.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.081607 market-data-transcoder-1.0.3/
+-rw-r--r--   0 mservidio   (501) staff       (20)    11357 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/LICENSE
+-rw-r--r--   0 mservidio   (501) staff       (20)    18958 2023-06-19 13:45:51.081689 market-data-transcoder-1.0.3/PKG-INFO
+-rw-r--r--   0 mservidio   (501) staff       (20)    18081 2023-05-02 00:42:45.000000 market-data-transcoder-1.0.3/README.md
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.069236 market-data-transcoder-1.0.3/market_data_transcoder.egg-info/
+-rw-r--r--   0 mservidio   (501) staff       (20)    18958 2023-06-19 13:45:51.000000 market-data-transcoder-1.0.3/market_data_transcoder.egg-info/PKG-INFO
+-rw-r--r--   0 mservidio   (501) staff       (20)     4188 2023-06-19 13:45:51.000000 market-data-transcoder-1.0.3/market_data_transcoder.egg-info/SOURCES.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)        1 2023-06-19 13:45:51.000000 market-data-transcoder-1.0.3/market_data_transcoder.egg-info/dependency_links.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)       48 2023-06-19 13:45:51.000000 market-data-transcoder-1.0.3/market_data_transcoder.egg-info/entry_points.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)        1 2023-04-20 20:22:51.000000 market-data-transcoder-1.0.3/market_data_transcoder.egg-info/not-zip-safe
+-rw-r--r--   0 mservidio   (501) staff       (20)      149 2023-06-19 13:45:51.000000 market-data-transcoder-1.0.3/market_data_transcoder.egg-info/requires.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)       23 2023-06-19 13:45:51.000000 market-data-transcoder-1.0.3/market_data_transcoder.egg-info/top_level.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)      101 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/pyproject.toml
+-rw-r--r--   0 mservidio   (501) staff       (20)     1263 2023-06-19 13:45:51.082099 market-data-transcoder-1.0.3/setup.cfg
+-rw-r--r--   0 mservidio   (501) staff       (20)     1075 2023-04-20 20:41:12.000000 market-data-transcoder-1.0.3/setup.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.069355 market-data-transcoder-1.0.3/third_party/
+-rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.070083 market-data-transcoder-1.0.3/third_party/pyfixmsg/
+-rw-r--r--   0 mservidio   (501) staff       (20)     6276 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.070343 market-data-transcoder-1.0.3/third_party/pyfixmsg/codecs/
+-rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/codecs/__init__.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    13965 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/codecs/stringfix.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.070604 market-data-transcoder-1.0.3/third_party/pyfixmsg/exception/
+-rw-r--r--   0 mservidio   (501) staff       (20)      945 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/exception/__init__.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    18449 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/fixmessage.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     6960 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/parser.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    18582 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/reference.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1079 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/pyfixmsg/util.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.071212 market-data-transcoder-1.0.3/third_party/sbedecoder/
+-rw-r--r--   0 mservidio   (501) staff       (20)      154 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/sbedecoder/__init__.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    23241 2023-06-19 13:36:20.000000 market-data-transcoder-1.0.3/third_party/sbedecoder/message.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     5317 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/third_party/sbedecoder/parser.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    27955 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/sbedecoder/schema.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1326 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/third_party/sbedecoder/typemap.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.071799 market-data-transcoder-1.0.3/transcoder/
+-rw-r--r--   0 mservidio   (501) staff       (20)    12212 2023-06-19 13:36:20.000000 market-data-transcoder-1.0.3/transcoder/Transcoder.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      915 2023-04-20 20:38:35.000000 market-data-transcoder-1.0.3/transcoder/__init__.py
+-rwxr-xr-x   0 mservidio   (501) staff       (20)    12093 2023-05-02 00:42:45.000000 market-data-transcoder-1.0.3/transcoder/main.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.072880 market-data-transcoder-1.0.3/transcoder/message/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1709 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/DatacastField.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2756 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/DatacastGroup.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     5117 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/DatacastParser.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1163 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/DatacastSchema.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     3775 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/ErrorWriter.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     3280 2023-04-20 19:45:10.000000 market-data-transcoder-1.0.3/transcoder/message/MessageUtil.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1335 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/NoParser.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1452 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/ParsedMessage.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      921 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.073262 market-data-transcoder-1.0.3/transcoder/message/exception/
+-rw-r--r--   0 mservidio   (501) staff       (20)      974 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/exception/MessageParserNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      927 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/exception/ParserFunctionNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      959 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/exception/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.073946 market-data-transcoder-1.0.3/transcoder/message/factory/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1595 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/factory/CmeMessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1762 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.3/transcoder/message/factory/ITCHMessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2001 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/factory/MDPMessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1576 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/factory/MemxMessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1687 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.3/transcoder/message/factory/MessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1319 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.3/transcoder/message/factory/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.074336 market-data-transcoder-1.0.3/transcoder/message/factory/exception/
+-rw-r--r--   0 mservidio   (501) staff       (20)      915 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/factory/exception/FactoryNotFoundError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      946 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      920 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/message/factory/exception/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.075724 market-data-transcoder-1.0.3/transcoder/message/handler/
+-rw-r--r--   0 mservidio   (501) staff       (20)     2269 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/handler/CmeBinaryPacketHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2287 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/handler/FilterHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1731 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/handler/MessageHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1423 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.3/transcoder/message/handler/MessageHandlerFloatField.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1417 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.3/transcoder/message/handler/MessageHandlerIntField.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1424 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.3/transcoder/message/handler/MessageHandlerStringField.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2137 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/handler/SequencerHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2151 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/handler/TimestampPullForwardHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1063 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/message/handler/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.076162 market-data-transcoder-1.0.3/transcoder/output/
+-rw-r--r--   0 mservidio   (501) staff       (20)     4708 2023-06-19 13:36:20.000000 market-data-transcoder-1.0.3/transcoder/output/OutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     4975 2023-04-20 20:10:00.000000 market-data-transcoder-1.0.3/transcoder/output/OutputUtil.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      955 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/output/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.076709 market-data-transcoder-1.0.3/transcoder/output/avro/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1843 2023-04-20 20:30:03.000000 market-data-transcoder-1.0.3/transcoder/output/avro/AvroOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2907 2023-06-19 13:36:20.000000 market-data-transcoder-1.0.3/transcoder/output/avro/BaseAvroOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1756 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/avro/FastAvroOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      953 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/avro/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.076985 market-data-transcoder-1.0.3/transcoder/output/diag/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1158 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/diag/DiagnosticOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      908 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/diag/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.077847 market-data-transcoder-1.0.3/transcoder/output/exception/
+-rw-r--r--   0 mservidio   (501) staff       (20)      983 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/exception/BigQueryTableSchemaOutOfSyncError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      943 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/exception/OutputFunctionNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      909 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/exception/OutputManagerSchemaError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      953 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/exception/OutputNotAvailableError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      979 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/exception/PubSubTopicSchemaOutOfSyncError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1202 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/exception/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.078397 market-data-transcoder-1.0.3/transcoder/output/google_cloud/
+-rw-r--r--   0 mservidio   (501) staff       (20)     6504 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/google_cloud/BigQueryOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1016 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/google_cloud/Constants.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    12040 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/google_cloud/PubSubOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      957 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/google_cloud/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.079183 market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/
+-rw-r--r--   0 mservidio   (501) staff       (20)     2792 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2118 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2892 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      993 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.079509 market-data-transcoder-1.0.3/transcoder/output/json/
+-rw-r--r--   0 mservidio   (501) staff       (20)     3559 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/json/JsonOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      896 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/output/json/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.079826 market-data-transcoder-1.0.3/transcoder/output/length_delimited/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1909 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/output/length_delimited/LengthDelimitedOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      918 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/output/length_delimited/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.080410 market-data-transcoder-1.0.3/transcoder/source/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1189 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/source/LineEncoding.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1826 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/source/Source.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     3776 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/source/SourceUtil.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      914 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/source/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-06-19 13:45:51.081452 market-data-transcoder-1.0.3/transcoder/source/file/
+-rw-r--r--   0 mservidio   (501) staff       (20)     3867 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/source/file/CmeBinaryPacketFileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2623 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/source/file/FileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2630 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/source/file/LengthDelimitedFileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2719 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/source/file/LineDelimitedFileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2295 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.3/transcoder/source/file/PcapFileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1186 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/source/file/__init__.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1624 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.3/transcoder/test.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      837 2023-06-19 13:45:22.000000 market-data-transcoder-1.0.3/transcoder/version.py
```

### Comparing `market-data-transcoder-1.0.2/LICENSE` & `market-data-transcoder-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/PKG-INFO` & `market-data-transcoder-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-data-transcoder
-Version: 1.0.2
+Version: 1.0.3
 Summary: Market Data Transcoder
 Home-page: https://github.com/GoogleCloudPlatform/market-data-transcoder
 Author: Google Cloud FSI Solutions
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/GoogleCloudPlatform/market-data-transcoder/issues
 Keywords: bigquery,devops,json,automation,schema,trading,avro,binary,transcoding,pubsub,fix,fixprotocol,google-cloud-platform,itch,sbe,simple-binary-encoding,exchanges,marketdata,binaryencoding
 Classifier: Programming Language :: Python :: 3
@@ -66,39 +66,47 @@
 #### Message factory
 
 A message factory takes a message payload read from the input source, determines the associated message type from the schema to apply, and performs any adjustments to the message data prior to transcoding. For example, a message producer may use non-standard SBE headers or metadata that you would like to remove or transform. For standard FIX tag/value input sources, the included `fix` message factory may be used.
 
 ### CLI usage
 
 ```
-# List available cli arguments
-usage: txcode [-h] --factory {cme,itch,memx,fix} --schema_file SCHEMA_FILE --source_file
-              SOURCE_FILE [--source_file_encoding SOURCE_FILE_ENCODING]
-              --source_file_format_type {pcap,length_delimited,line_delimited,cme_binary_packet}
-              [--base64 | --base64_urlsafe] [--fix_header_tags FIX_HEADER_TAGS]
-              [--fix_separator FIX_SEPARATOR] [--message_handlers MESSAGE_HANDLERS]
-              [--message_skip_bytes MESSAGE_SKIP_BYTES]
-              [--message_type_exclusions MESSAGE_TYPE_EXCLUSIONS | --message_type_inclusions MESSAGE_TYPE_INCLUSIONS]
-              [--sampling_count SAMPLING_COUNT] [--skip_bytes SKIP_BYTES]
-              [--skip_lines SKIP_LINES] [--source_file_endian {big,little}]
-              [--output_path OUTPUT_PATH]
-              [--output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl}]
-              [--error_output_path ERROR_OUTPUT_PATH] [--lazy_create_resources] [--stats_only]
-              [--create_schemas_only] [--destination_project_id DESTINATION_PROJECT_ID]
-              [--destination_dataset_id DESTINATION_DATASET_ID]
-              [--output_encoding {binary,json}]
-              [--create_schema_enforcing_topics | --no-create_schema_enforcing_topics]
-              [--continue_on_error] [--log {notset,debug,info,warning,error,critical}] [-q] [-v]
+usage: txcode  [-h] [--factory {cme,itch,memx,fix}]
+               [--schema_file SCHEMA_FILE] [--source_file SOURCE_FILE]
+               [--source_file_encoding SOURCE_FILE_ENCODING]
+               --source_file_format_type
+               {pcap,length_delimited,line_delimited,cme_binary_packet}
+               [--base64 | --base64_urlsafe]
+               [--fix_header_tags FIX_HEADER_TAGS]
+               [--fix_separator FIX_SEPARATOR]
+               [--message_handlers MESSAGE_HANDLERS]
+               [--message_skip_bytes MESSAGE_SKIP_BYTES]
+               [--prefix_length PREFIX_LENGTH]
+               [--message_type_exclusions MESSAGE_TYPE_EXCLUSIONS | --message_type_inclusions MESSAGE_TYPE_INCLUSIONS]
+               [--sampling_count SAMPLING_COUNT] [--skip_bytes SKIP_BYTES]
+               [--skip_lines SKIP_LINES] [--source_file_endian {big,little}]
+               [--output_path OUTPUT_PATH]
+               [--output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl,length_delimited}]
+               [--error_output_path ERROR_OUTPUT_PATH]
+               [--lazy_create_resources] [--frame_only] [--stats_only]
+               [--create_schemas_only]
+               [--destination_project_id DESTINATION_PROJECT_ID]
+               [--destination_dataset_id DESTINATION_DATASET_ID]
+               [--output_encoding {binary,json}]
+               [--create_schema_enforcing_topics | --no-create_schema_enforcing_topics]
+               [--continue_on_error]
+               [--log {notset,debug,info,warning,error,critical}] [-q] [-v]
 
 Datacast Transcoder process input arguments
 
 options:
   -h, --help            show this help message and exit
-  --continue_on_error   Indicates if an exception file should be created, and records continued
-                        to be processed upon message level exceptions
+  --continue_on_error   Indicates if an exception file should be created, and
+                        records continued to be processed upon message level
+                        exceptions
   --log {notset,debug,info,warning,error,critical}
                         The default logging level
   -q, --quiet           Suppress message output to console
   -v, --version         show program's version number and exit
 
 Input source arguments:
   --factory {cme,itch,memx,fix}
@@ -107,80 +115,225 @@
                         Path to the schema file
   --source_file SOURCE_FILE
                         Path to the source file
   --source_file_encoding SOURCE_FILE_ENCODING
                         The source file character encoding
   --source_file_format_type {pcap,length_delimited,line_delimited,cme_binary_packet}
                         The source file format
-  --base64              Indicates if each individual message extracted from the source is base
-                        64 encoded
-  --base64_urlsafe      Indicates if each individual message extracted from the source is base
-                        64 url safe encoded
+  --base64              Indicates if each individual message extracted from
+                        the source is base 64 encoded
+  --base64_urlsafe      Indicates if each individual message extracted from
+                        the source is base 64 url safe encoded
   --fix_header_tags FIX_HEADER_TAGS
                         Comma delimited list of fix header tags
   --fix_separator FIX_SEPARATOR
                         The unicode int representing the fix message separator
   --message_handlers MESSAGE_HANDLERS
-                        Comma delimited list of message handlers in priority order
+                        Comma delimited list of message handlers in priority
+                        order
   --message_skip_bytes MESSAGE_SKIP_BYTES
-                        Number of bytes to skip before processing individual messages within a
-                        repeated length delimited file message source
+                        Number of bytes to skip before processing individual
+                        messages within a repeated length delimited file
+                        message source
+  --prefix_length PREFIX_LENGTH
+                        How many bytes to use for the length prefix of length-
+                        delimited binary sources
   --message_type_exclusions MESSAGE_TYPE_EXCLUSIONS
-                        Comma-delimited list of message types to exclude when processing
+                        Comma-delimited list of message types to exclude when
+                        processing
   --message_type_inclusions MESSAGE_TYPE_INCLUSIONS
-                        Comma-delimited list of message types to include when processing
+                        Comma-delimited list of message types to include when
+                        processing
   --sampling_count SAMPLING_COUNT
-                        To be used for testing only - the sampling count indicates how many of
-                        each distinct message type to process, any additional will be skipped
+                        Halt processing after reaching this number of
+                        messages. Applied after all Handlers are executed per
+                        message
   --skip_bytes SKIP_BYTES
-                        Number of bytes to skip before processing the file. Useful for skipping
-                        file-level headers
+                        Number of bytes to skip before processing the file.
+                        Useful for skipping file-level headers
   --skip_lines SKIP_LINES
                         Number of lines to skip before processing the file
   --source_file_endian {big,little}
                         Source file endianness
 
 Output arguments:
   --output_path OUTPUT_PATH
                         Output file path. Defaults to avroOut
-  --output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl}
+  --output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl,length_delimited}
                         Output format type
   --error_output_path ERROR_OUTPUT_PATH
-                        Error output file path if --continue_on_error flag enabled. Defaults to
-                        errorOut
+                        Error output file path if --continue_on_error flag
+                        enabled. Defaults to errorOut
   --lazy_create_resources
-                        Flag indicating that output resources for message types should be only
-                        created as messages of each type are encountered in the source data.
-                        Default behavior is to create resources for each message type before
-                        messages are processed. Particularly useful when working with FIX but
-                        only processing a limited set of message types in the source data
-  --stats_only          Flag indicating that transcoder should only report on message type
-                        counts without parsing messages further
+                        Flag indicating that output resources for message
+                        types should be only created as messages of each type
+                        are encountered in the source data. Default behavior
+                        is to create resources for each message type before
+                        messages are processed. Particularly useful when
+                        working with FIX but only processing a limited set of
+                        message types in the source data
+  --frame_only          Flag indicating that transcoder should only frame
+                        messages to an output source
+  --stats_only          Flag indicating that transcoder should only report on
+                        message type counts without parsing messages further
   --create_schemas_only
-                        Flag indicating that transcoder should only create output resource
-                        schemas and not output message data
+                        Flag indicating that transcoder should only create
+                        output resource schemas and not output message data
 
 Google Cloud arguments:
   --destination_project_id DESTINATION_PROJECT_ID
-                        The Google Cloud project ID for the destination resource
+                        The Google Cloud project ID for the destination
+                        resource
 
 BigQuery arguments:
   --destination_dataset_id DESTINATION_DATASET_ID
-                        The BigQuery dataset for the destination. If it does not exist, it will
-                        be created
+                        The BigQuery dataset for the destination. If it does
+                        not exist, it will be created
 
 Pub/Sub arguments:
   --output_encoding {binary,json}
                         The encoding of the output
   --create_schema_enforcing_topics, --no-create_schema_enforcing_topics
-                        Indicates if Pub/Sub schemas should be created and used to validate
-                        messages sent to a topic (default: True)
+                        Indicates if Pub/Sub schemas should be created and
+                        used to validate messages sent to a topic
+```
+
+### Message handlers
+
+`txcode` supports the execution of _message handler_ classes that can
+be used to statefully mutate in-flight streams and messages. For example,
+`TimestampPullForwardHandler` will look for a `seconds`-styled ITCH
+message (that informs the stream of the prevailing epochs second to
+apply to subsequent messages), and append the latest value from
+that to all subsequent messages (between instances of the `seconds`
+message appearing. This helps individual messages be persisted with
+absolute timestamps that require less context to interpret
+(i.e. outbound messages contain more than just "nanoseconds past
+midnight" for a timestamp.
+
+Another handler is `SequencerHandler`, which appends a sequence number
+to all outbound messages. This is useful when processing bulk messages
+in length-delimited storage formats where the IP packet headers
+containing the original sequence numbers have been stripped.	
+
+`FilterHandler` lets you filter output based upon a specific property
+of a message. A common use for this is to filter messages pertaining
+only to a particular security identifier or symbol.
+
+Here is a combination of transcoding invocations that can
+be used to shard a message universe by trading symbol. First, the mnemonic
+trading symbol identifier (`stock`) must be used to find it's associated integer
+security identifier (`stock_locate`) from the `stock_directory`
+message. `stock_locate` is the identifier included in every
+relevant message (as opposed to `stock`, which is absent from
+certain message types):
+
+```
 
+txcode --source_file 12302019.NASDAQ_ITCH50 --schema_file totalview-itch-50.xml --message_type_inclusions stock_directory --source_file_format_type length_delimited --factory itch --message_handlers FilterHandler:stock=SPY --sampling_count 1
+
+authenticity: P
+etp_flag: Y
+etp_leverage_factor: null
+financial_status_indicator: ' '
+inverse_indicator: null
+ipo_flag: ' '
+issue_classification: Q
+issue_subtype: E
+luld_reference_price_tier: '1'
+market_category: P
+round_lot_size: 100
+round_lots_only: N
+short_sale_threshold_indicator: N
+stock: SPY
+stock_locate: 7451
+timestamp: 11354508113636
+tracking_number: 0
+
+INFO:root:Sampled messages: 1
+INFO:root:Message type inclusions: ['stock_directory']
+INFO:root:Source message count: 7466
+INFO:root:Processed message count: 7451
+INFO:root:Transcoded message count: 1
+INFO:root:Processed schema count: 1
+INFO:root:Summary of message counts: {'stock_directory': 7451}
+INFO:root:Summary of error message counts: {}
+INFO:root:Message rate: 53260.474108 per second
+INFO:root:Total runtime in seconds: 0.140179
+INFO:root:Total runtime in minutes: 0.002336
 ```
 
+Taking the value of the field `stock_locate` from the above message
+allows us to filter all messages for that field/value combination. In
+addition, we can append a sequence number to all transcoded messages
+that are output. The below combination returns the original `stock_directory`
+message we used to look up the `stock_locate` code, as well as the
+next two messages in the stream that have the same value for `stock_locate`:
+
+```
+
+txcode --source_file 12302019.NASDAQ_ITCH50 --schema_file totalview-itch-50.xml --source_file_format_type length_delimited --factory itch --message_handlers FilterHandler:stock_locate=7451,SequencerHandler --sampling_count 3 
+
+authenticity: P
+etp_flag: Y
+etp_leverage_factor: null
+financial_status_indicator: ' '
+inverse_indicator: null
+ipo_flag: ' '
+issue_classification: Q
+issue_subtype: E
+luld_reference_price_tier: '1'
+market_category: P
+round_lot_size: 100
+round_lots_only: N
+sequence_number: 1
+short_sale_threshold_indicator: N
+stock: SPY
+stock_locate: 7451
+timestamp: 11354508113636
+tracking_number: 0
+
+reason: ''
+reserved: ' '
+sequence_number: 2
+stock: SPY
+stock_locate: 7451
+timestamp: 11355134575401
+tracking_number: 0
+trading_state: T
+
+reg_sho_action: '0'
+sequence_number: 3
+stock: SPY
+stock_locate: 7451
+timestamp: 11355134599149
+tracking_number: 0
+
+INFO:root:Sampled messages: 3
+INFO:root:Source message count: 23781
+INFO:root:Processed message count: 23781
+INFO:root:Transcoded message count: 3
+INFO:root:Processed schema count: 21
+INFO:root:Summary of message counts: {'system_event': 1, 'stock_directory': 8906, 'stock_trading_action': 7437, 'reg_sho_restriction': 7437, 'market_participant_position': 0, 'mwcb_decline_level': 0, 'ipo_quoting_period_update': 0, 'luld_auction_collar': 0, 'operational_halt': 0, 'add_order_no_attribution': 0, 'add_order_attribution': 0, 'order_executed': 0, 'order_executed_price': 0, 'order_cancelled': 0, 'order_deleted': 0, 'order_replaced': 0, 'trade': 0, 'cross_trade': 0, 'broken_trade': 0, 'net_order_imbalance': 0, 'retail_price_improvement_indicator': 0}
+INFO:root:Summary of error message counts: {}
+INFO:root:Message rate: 80950.257512 per second
+INFO:root:Total runtime in seconds: 0.293773
+INFO:root:Total runtime in minutes: 0.004896
+
+
+```
+
+The syntax for handler specifications is:
+
+```
+<Handler1>:<Handler1Parameter>=<Handler1Parameter>,<Handler2>
+```
+
+Message handlers are deployed in `transcoder/message/handler/`.
+
 # Installation
 If you are a user looking to use the CLI or library without making changes, you can install the Market Data Transcoder from [PyPI](https://pypi.org/project/market-data-transcoder) using pip:
 ```
 pip install market-data-transcoder
 ```
 
 After the pip installation, you can validate that the transcoder is available by the following command:
```

### Comparing `market-data-transcoder-1.0.2/README.md` & `market-data-transcoder-1.0.3/market_data_transcoder.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: market-data-transcoder
+Version: 1.0.3
+Summary: Market Data Transcoder
+Home-page: https://github.com/GoogleCloudPlatform/market-data-transcoder
+Author: Google Cloud FSI Solutions
+License: Apache License 2.0
+Project-URL: Bug Tracker, https://github.com/GoogleCloudPlatform/market-data-transcoder/issues
+Keywords: bigquery,devops,json,automation,schema,trading,avro,binary,transcoding,pubsub,fix,fixprotocol,google-cloud-platform,itch,sbe,simple-binary-encoding,exchanges,marketdata,binaryencoding
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ```Google Cloud Datacast Solution```
  
 ##  _Ingest high-performance exchange feeds into Google Cloud_
 
 _This is not an official Google product or service_
 
 ### Introduction
@@ -48,39 +66,47 @@
 #### Message factory
 
 A message factory takes a message payload read from the input source, determines the associated message type from the schema to apply, and performs any adjustments to the message data prior to transcoding. For example, a message producer may use non-standard SBE headers or metadata that you would like to remove or transform. For standard FIX tag/value input sources, the included `fix` message factory may be used.
 
 ### CLI usage
 
 ```
-# List available cli arguments
-usage: txcode [-h] --factory {cme,itch,memx,fix} --schema_file SCHEMA_FILE --source_file
-              SOURCE_FILE [--source_file_encoding SOURCE_FILE_ENCODING]
-              --source_file_format_type {pcap,length_delimited,line_delimited,cme_binary_packet}
-              [--base64 | --base64_urlsafe] [--fix_header_tags FIX_HEADER_TAGS]
-              [--fix_separator FIX_SEPARATOR] [--message_handlers MESSAGE_HANDLERS]
-              [--message_skip_bytes MESSAGE_SKIP_BYTES]
-              [--message_type_exclusions MESSAGE_TYPE_EXCLUSIONS | --message_type_inclusions MESSAGE_TYPE_INCLUSIONS]
-              [--sampling_count SAMPLING_COUNT] [--skip_bytes SKIP_BYTES]
-              [--skip_lines SKIP_LINES] [--source_file_endian {big,little}]
-              [--output_path OUTPUT_PATH]
-              [--output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl}]
-              [--error_output_path ERROR_OUTPUT_PATH] [--lazy_create_resources] [--stats_only]
-              [--create_schemas_only] [--destination_project_id DESTINATION_PROJECT_ID]
-              [--destination_dataset_id DESTINATION_DATASET_ID]
-              [--output_encoding {binary,json}]
-              [--create_schema_enforcing_topics | --no-create_schema_enforcing_topics]
-              [--continue_on_error] [--log {notset,debug,info,warning,error,critical}] [-q] [-v]
+usage: txcode  [-h] [--factory {cme,itch,memx,fix}]
+               [--schema_file SCHEMA_FILE] [--source_file SOURCE_FILE]
+               [--source_file_encoding SOURCE_FILE_ENCODING]
+               --source_file_format_type
+               {pcap,length_delimited,line_delimited,cme_binary_packet}
+               [--base64 | --base64_urlsafe]
+               [--fix_header_tags FIX_HEADER_TAGS]
+               [--fix_separator FIX_SEPARATOR]
+               [--message_handlers MESSAGE_HANDLERS]
+               [--message_skip_bytes MESSAGE_SKIP_BYTES]
+               [--prefix_length PREFIX_LENGTH]
+               [--message_type_exclusions MESSAGE_TYPE_EXCLUSIONS | --message_type_inclusions MESSAGE_TYPE_INCLUSIONS]
+               [--sampling_count SAMPLING_COUNT] [--skip_bytes SKIP_BYTES]
+               [--skip_lines SKIP_LINES] [--source_file_endian {big,little}]
+               [--output_path OUTPUT_PATH]
+               [--output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl,length_delimited}]
+               [--error_output_path ERROR_OUTPUT_PATH]
+               [--lazy_create_resources] [--frame_only] [--stats_only]
+               [--create_schemas_only]
+               [--destination_project_id DESTINATION_PROJECT_ID]
+               [--destination_dataset_id DESTINATION_DATASET_ID]
+               [--output_encoding {binary,json}]
+               [--create_schema_enforcing_topics | --no-create_schema_enforcing_topics]
+               [--continue_on_error]
+               [--log {notset,debug,info,warning,error,critical}] [-q] [-v]
 
 Datacast Transcoder process input arguments
 
 options:
   -h, --help            show this help message and exit
-  --continue_on_error   Indicates if an exception file should be created, and records continued
-                        to be processed upon message level exceptions
+  --continue_on_error   Indicates if an exception file should be created, and
+                        records continued to be processed upon message level
+                        exceptions
   --log {notset,debug,info,warning,error,critical}
                         The default logging level
   -q, --quiet           Suppress message output to console
   -v, --version         show program's version number and exit
 
 Input source arguments:
   --factory {cme,itch,memx,fix}
@@ -89,80 +115,225 @@
                         Path to the schema file
   --source_file SOURCE_FILE
                         Path to the source file
   --source_file_encoding SOURCE_FILE_ENCODING
                         The source file character encoding
   --source_file_format_type {pcap,length_delimited,line_delimited,cme_binary_packet}
                         The source file format
-  --base64              Indicates if each individual message extracted from the source is base
-                        64 encoded
-  --base64_urlsafe      Indicates if each individual message extracted from the source is base
-                        64 url safe encoded
+  --base64              Indicates if each individual message extracted from
+                        the source is base 64 encoded
+  --base64_urlsafe      Indicates if each individual message extracted from
+                        the source is base 64 url safe encoded
   --fix_header_tags FIX_HEADER_TAGS
                         Comma delimited list of fix header tags
   --fix_separator FIX_SEPARATOR
                         The unicode int representing the fix message separator
   --message_handlers MESSAGE_HANDLERS
-                        Comma delimited list of message handlers in priority order
+                        Comma delimited list of message handlers in priority
+                        order
   --message_skip_bytes MESSAGE_SKIP_BYTES
-                        Number of bytes to skip before processing individual messages within a
-                        repeated length delimited file message source
+                        Number of bytes to skip before processing individual
+                        messages within a repeated length delimited file
+                        message source
+  --prefix_length PREFIX_LENGTH
+                        How many bytes to use for the length prefix of length-
+                        delimited binary sources
   --message_type_exclusions MESSAGE_TYPE_EXCLUSIONS
-                        Comma-delimited list of message types to exclude when processing
+                        Comma-delimited list of message types to exclude when
+                        processing
   --message_type_inclusions MESSAGE_TYPE_INCLUSIONS
-                        Comma-delimited list of message types to include when processing
+                        Comma-delimited list of message types to include when
+                        processing
   --sampling_count SAMPLING_COUNT
-                        To be used for testing only - the sampling count indicates how many of
-                        each distinct message type to process, any additional will be skipped
+                        Halt processing after reaching this number of
+                        messages. Applied after all Handlers are executed per
+                        message
   --skip_bytes SKIP_BYTES
-                        Number of bytes to skip before processing the file. Useful for skipping
-                        file-level headers
+                        Number of bytes to skip before processing the file.
+                        Useful for skipping file-level headers
   --skip_lines SKIP_LINES
                         Number of lines to skip before processing the file
   --source_file_endian {big,little}
                         Source file endianness
 
 Output arguments:
   --output_path OUTPUT_PATH
                         Output file path. Defaults to avroOut
-  --output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl}
+  --output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl,length_delimited}
                         Output format type
   --error_output_path ERROR_OUTPUT_PATH
-                        Error output file path if --continue_on_error flag enabled. Defaults to
-                        errorOut
+                        Error output file path if --continue_on_error flag
+                        enabled. Defaults to errorOut
   --lazy_create_resources
-                        Flag indicating that output resources for message types should be only
-                        created as messages of each type are encountered in the source data.
-                        Default behavior is to create resources for each message type before
-                        messages are processed. Particularly useful when working with FIX but
-                        only processing a limited set of message types in the source data
-  --stats_only          Flag indicating that transcoder should only report on message type
-                        counts without parsing messages further
+                        Flag indicating that output resources for message
+                        types should be only created as messages of each type
+                        are encountered in the source data. Default behavior
+                        is to create resources for each message type before
+                        messages are processed. Particularly useful when
+                        working with FIX but only processing a limited set of
+                        message types in the source data
+  --frame_only          Flag indicating that transcoder should only frame
+                        messages to an output source
+  --stats_only          Flag indicating that transcoder should only report on
+                        message type counts without parsing messages further
   --create_schemas_only
-                        Flag indicating that transcoder should only create output resource
-                        schemas and not output message data
+                        Flag indicating that transcoder should only create
+                        output resource schemas and not output message data
 
 Google Cloud arguments:
   --destination_project_id DESTINATION_PROJECT_ID
-                        The Google Cloud project ID for the destination resource
+                        The Google Cloud project ID for the destination
+                        resource
 
 BigQuery arguments:
   --destination_dataset_id DESTINATION_DATASET_ID
-                        The BigQuery dataset for the destination. If it does not exist, it will
-                        be created
+                        The BigQuery dataset for the destination. If it does
+                        not exist, it will be created
 
 Pub/Sub arguments:
   --output_encoding {binary,json}
                         The encoding of the output
   --create_schema_enforcing_topics, --no-create_schema_enforcing_topics
-                        Indicates if Pub/Sub schemas should be created and used to validate
-                        messages sent to a topic (default: True)
+                        Indicates if Pub/Sub schemas should be created and
+                        used to validate messages sent to a topic
+```
+
+### Message handlers
+
+`txcode` supports the execution of _message handler_ classes that can
+be used to statefully mutate in-flight streams and messages. For example,
+`TimestampPullForwardHandler` will look for a `seconds`-styled ITCH
+message (that informs the stream of the prevailing epochs second to
+apply to subsequent messages), and append the latest value from
+that to all subsequent messages (between instances of the `seconds`
+message appearing. This helps individual messages be persisted with
+absolute timestamps that require less context to interpret
+(i.e. outbound messages contain more than just "nanoseconds past
+midnight" for a timestamp.
+
+Another handler is `SequencerHandler`, which appends a sequence number
+to all outbound messages. This is useful when processing bulk messages
+in length-delimited storage formats where the IP packet headers
+containing the original sequence numbers have been stripped.	
+
+`FilterHandler` lets you filter output based upon a specific property
+of a message. A common use for this is to filter messages pertaining
+only to a particular security identifier or symbol.
+
+Here is a combination of transcoding invocations that can
+be used to shard a message universe by trading symbol. First, the mnemonic
+trading symbol identifier (`stock`) must be used to find it's associated integer
+security identifier (`stock_locate`) from the `stock_directory`
+message. `stock_locate` is the identifier included in every
+relevant message (as opposed to `stock`, which is absent from
+certain message types):
 
 ```
 
+txcode --source_file 12302019.NASDAQ_ITCH50 --schema_file totalview-itch-50.xml --message_type_inclusions stock_directory --source_file_format_type length_delimited --factory itch --message_handlers FilterHandler:stock=SPY --sampling_count 1
+
+authenticity: P
+etp_flag: Y
+etp_leverage_factor: null
+financial_status_indicator: ' '
+inverse_indicator: null
+ipo_flag: ' '
+issue_classification: Q
+issue_subtype: E
+luld_reference_price_tier: '1'
+market_category: P
+round_lot_size: 100
+round_lots_only: N
+short_sale_threshold_indicator: N
+stock: SPY
+stock_locate: 7451
+timestamp: 11354508113636
+tracking_number: 0
+
+INFO:root:Sampled messages: 1
+INFO:root:Message type inclusions: ['stock_directory']
+INFO:root:Source message count: 7466
+INFO:root:Processed message count: 7451
+INFO:root:Transcoded message count: 1
+INFO:root:Processed schema count: 1
+INFO:root:Summary of message counts: {'stock_directory': 7451}
+INFO:root:Summary of error message counts: {}
+INFO:root:Message rate: 53260.474108 per second
+INFO:root:Total runtime in seconds: 0.140179
+INFO:root:Total runtime in minutes: 0.002336
+```
+
+Taking the value of the field `stock_locate` from the above message
+allows us to filter all messages for that field/value combination. In
+addition, we can append a sequence number to all transcoded messages
+that are output. The below combination returns the original `stock_directory`
+message we used to look up the `stock_locate` code, as well as the
+next two messages in the stream that have the same value for `stock_locate`:
+
+```
+
+txcode --source_file 12302019.NASDAQ_ITCH50 --schema_file totalview-itch-50.xml --source_file_format_type length_delimited --factory itch --message_handlers FilterHandler:stock_locate=7451,SequencerHandler --sampling_count 3 
+
+authenticity: P
+etp_flag: Y
+etp_leverage_factor: null
+financial_status_indicator: ' '
+inverse_indicator: null
+ipo_flag: ' '
+issue_classification: Q
+issue_subtype: E
+luld_reference_price_tier: '1'
+market_category: P
+round_lot_size: 100
+round_lots_only: N
+sequence_number: 1
+short_sale_threshold_indicator: N
+stock: SPY
+stock_locate: 7451
+timestamp: 11354508113636
+tracking_number: 0
+
+reason: ''
+reserved: ' '
+sequence_number: 2
+stock: SPY
+stock_locate: 7451
+timestamp: 11355134575401
+tracking_number: 0
+trading_state: T
+
+reg_sho_action: '0'
+sequence_number: 3
+stock: SPY
+stock_locate: 7451
+timestamp: 11355134599149
+tracking_number: 0
+
+INFO:root:Sampled messages: 3
+INFO:root:Source message count: 23781
+INFO:root:Processed message count: 23781
+INFO:root:Transcoded message count: 3
+INFO:root:Processed schema count: 21
+INFO:root:Summary of message counts: {'system_event': 1, 'stock_directory': 8906, 'stock_trading_action': 7437, 'reg_sho_restriction': 7437, 'market_participant_position': 0, 'mwcb_decline_level': 0, 'ipo_quoting_period_update': 0, 'luld_auction_collar': 0, 'operational_halt': 0, 'add_order_no_attribution': 0, 'add_order_attribution': 0, 'order_executed': 0, 'order_executed_price': 0, 'order_cancelled': 0, 'order_deleted': 0, 'order_replaced': 0, 'trade': 0, 'cross_trade': 0, 'broken_trade': 0, 'net_order_imbalance': 0, 'retail_price_improvement_indicator': 0}
+INFO:root:Summary of error message counts: {}
+INFO:root:Message rate: 80950.257512 per second
+INFO:root:Total runtime in seconds: 0.293773
+INFO:root:Total runtime in minutes: 0.004896
+
+
+```
+
+The syntax for handler specifications is:
+
+```
+<Handler1>:<Handler1Parameter>=<Handler1Parameter>,<Handler2>
+```
+
+Message handlers are deployed in `transcoder/message/handler/`.
+
 # Installation
 If you are a user looking to use the CLI or library without making changes, you can install the Market Data Transcoder from [PyPI](https://pypi.org/project/market-data-transcoder) using pip:
 ```
 pip install market-data-transcoder
 ```
 
 After the pip installation, you can validate that the transcoder is available by the following command:
@@ -177,8 +348,8 @@
 pip install -r requirements.txt
 ```
 
 After installing the required dependencies, you can run the transcoder with the following:
 ```
 export PYTHONPATH=`pwd`
 python ./transcoder/main.py --help
-```
+```
```

### Comparing `market-data-transcoder-1.0.2/market_data_transcoder.egg-info/PKG-INFO` & `market-data-transcoder-1.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: market-data-transcoder
-Version: 1.0.2
-Summary: Market Data Transcoder
-Home-page: https://github.com/GoogleCloudPlatform/market-data-transcoder
-Author: Google Cloud FSI Solutions
-License: Apache License 2.0
-Project-URL: Bug Tracker, https://github.com/GoogleCloudPlatform/market-data-transcoder/issues
-Keywords: bigquery,devops,json,automation,schema,trading,avro,binary,transcoding,pubsub,fix,fixprotocol,google-cloud-platform,itch,sbe,simple-binary-encoding,exchanges,marketdata,binaryencoding
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ```Google Cloud Datacast Solution```
  
 ##  _Ingest high-performance exchange feeds into Google Cloud_
 
 _This is not an official Google product or service_
 
 ### Introduction
@@ -66,39 +48,47 @@
 #### Message factory
 
 A message factory takes a message payload read from the input source, determines the associated message type from the schema to apply, and performs any adjustments to the message data prior to transcoding. For example, a message producer may use non-standard SBE headers or metadata that you would like to remove or transform. For standard FIX tag/value input sources, the included `fix` message factory may be used.
 
 ### CLI usage
 
 ```
-# List available cli arguments
-usage: txcode [-h] --factory {cme,itch,memx,fix} --schema_file SCHEMA_FILE --source_file
-              SOURCE_FILE [--source_file_encoding SOURCE_FILE_ENCODING]
-              --source_file_format_type {pcap,length_delimited,line_delimited,cme_binary_packet}
-              [--base64 | --base64_urlsafe] [--fix_header_tags FIX_HEADER_TAGS]
-              [--fix_separator FIX_SEPARATOR] [--message_handlers MESSAGE_HANDLERS]
-              [--message_skip_bytes MESSAGE_SKIP_BYTES]
-              [--message_type_exclusions MESSAGE_TYPE_EXCLUSIONS | --message_type_inclusions MESSAGE_TYPE_INCLUSIONS]
-              [--sampling_count SAMPLING_COUNT] [--skip_bytes SKIP_BYTES]
-              [--skip_lines SKIP_LINES] [--source_file_endian {big,little}]
-              [--output_path OUTPUT_PATH]
-              [--output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl}]
-              [--error_output_path ERROR_OUTPUT_PATH] [--lazy_create_resources] [--stats_only]
-              [--create_schemas_only] [--destination_project_id DESTINATION_PROJECT_ID]
-              [--destination_dataset_id DESTINATION_DATASET_ID]
-              [--output_encoding {binary,json}]
-              [--create_schema_enforcing_topics | --no-create_schema_enforcing_topics]
-              [--continue_on_error] [--log {notset,debug,info,warning,error,critical}] [-q] [-v]
+usage: txcode  [-h] [--factory {cme,itch,memx,fix}]
+               [--schema_file SCHEMA_FILE] [--source_file SOURCE_FILE]
+               [--source_file_encoding SOURCE_FILE_ENCODING]
+               --source_file_format_type
+               {pcap,length_delimited,line_delimited,cme_binary_packet}
+               [--base64 | --base64_urlsafe]
+               [--fix_header_tags FIX_HEADER_TAGS]
+               [--fix_separator FIX_SEPARATOR]
+               [--message_handlers MESSAGE_HANDLERS]
+               [--message_skip_bytes MESSAGE_SKIP_BYTES]
+               [--prefix_length PREFIX_LENGTH]
+               [--message_type_exclusions MESSAGE_TYPE_EXCLUSIONS | --message_type_inclusions MESSAGE_TYPE_INCLUSIONS]
+               [--sampling_count SAMPLING_COUNT] [--skip_bytes SKIP_BYTES]
+               [--skip_lines SKIP_LINES] [--source_file_endian {big,little}]
+               [--output_path OUTPUT_PATH]
+               [--output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl,length_delimited}]
+               [--error_output_path ERROR_OUTPUT_PATH]
+               [--lazy_create_resources] [--frame_only] [--stats_only]
+               [--create_schemas_only]
+               [--destination_project_id DESTINATION_PROJECT_ID]
+               [--destination_dataset_id DESTINATION_DATASET_ID]
+               [--output_encoding {binary,json}]
+               [--create_schema_enforcing_topics | --no-create_schema_enforcing_topics]
+               [--continue_on_error]
+               [--log {notset,debug,info,warning,error,critical}] [-q] [-v]
 
 Datacast Transcoder process input arguments
 
 options:
   -h, --help            show this help message and exit
-  --continue_on_error   Indicates if an exception file should be created, and records continued
-                        to be processed upon message level exceptions
+  --continue_on_error   Indicates if an exception file should be created, and
+                        records continued to be processed upon message level
+                        exceptions
   --log {notset,debug,info,warning,error,critical}
                         The default logging level
   -q, --quiet           Suppress message output to console
   -v, --version         show program's version number and exit
 
 Input source arguments:
   --factory {cme,itch,memx,fix}
@@ -107,80 +97,225 @@
                         Path to the schema file
   --source_file SOURCE_FILE
                         Path to the source file
   --source_file_encoding SOURCE_FILE_ENCODING
                         The source file character encoding
   --source_file_format_type {pcap,length_delimited,line_delimited,cme_binary_packet}
                         The source file format
-  --base64              Indicates if each individual message extracted from the source is base
-                        64 encoded
-  --base64_urlsafe      Indicates if each individual message extracted from the source is base
-                        64 url safe encoded
+  --base64              Indicates if each individual message extracted from
+                        the source is base 64 encoded
+  --base64_urlsafe      Indicates if each individual message extracted from
+                        the source is base 64 url safe encoded
   --fix_header_tags FIX_HEADER_TAGS
                         Comma delimited list of fix header tags
   --fix_separator FIX_SEPARATOR
                         The unicode int representing the fix message separator
   --message_handlers MESSAGE_HANDLERS
-                        Comma delimited list of message handlers in priority order
+                        Comma delimited list of message handlers in priority
+                        order
   --message_skip_bytes MESSAGE_SKIP_BYTES
-                        Number of bytes to skip before processing individual messages within a
-                        repeated length delimited file message source
+                        Number of bytes to skip before processing individual
+                        messages within a repeated length delimited file
+                        message source
+  --prefix_length PREFIX_LENGTH
+                        How many bytes to use for the length prefix of length-
+                        delimited binary sources
   --message_type_exclusions MESSAGE_TYPE_EXCLUSIONS
-                        Comma-delimited list of message types to exclude when processing
+                        Comma-delimited list of message types to exclude when
+                        processing
   --message_type_inclusions MESSAGE_TYPE_INCLUSIONS
-                        Comma-delimited list of message types to include when processing
+                        Comma-delimited list of message types to include when
+                        processing
   --sampling_count SAMPLING_COUNT
-                        To be used for testing only - the sampling count indicates how many of
-                        each distinct message type to process, any additional will be skipped
+                        Halt processing after reaching this number of
+                        messages. Applied after all Handlers are executed per
+                        message
   --skip_bytes SKIP_BYTES
-                        Number of bytes to skip before processing the file. Useful for skipping
-                        file-level headers
+                        Number of bytes to skip before processing the file.
+                        Useful for skipping file-level headers
   --skip_lines SKIP_LINES
                         Number of lines to skip before processing the file
   --source_file_endian {big,little}
                         Source file endianness
 
 Output arguments:
   --output_path OUTPUT_PATH
                         Output file path. Defaults to avroOut
-  --output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl}
+  --output_type {diag,avro,fastavro,bigquery,pubsub,bigquery_terraform,pubsub_terraform,jsonl,length_delimited}
                         Output format type
   --error_output_path ERROR_OUTPUT_PATH
-                        Error output file path if --continue_on_error flag enabled. Defaults to
-                        errorOut
+                        Error output file path if --continue_on_error flag
+                        enabled. Defaults to errorOut
   --lazy_create_resources
-                        Flag indicating that output resources for message types should be only
-                        created as messages of each type are encountered in the source data.
-                        Default behavior is to create resources for each message type before
-                        messages are processed. Particularly useful when working with FIX but
-                        only processing a limited set of message types in the source data
-  --stats_only          Flag indicating that transcoder should only report on message type
-                        counts without parsing messages further
+                        Flag indicating that output resources for message
+                        types should be only created as messages of each type
+                        are encountered in the source data. Default behavior
+                        is to create resources for each message type before
+                        messages are processed. Particularly useful when
+                        working with FIX but only processing a limited set of
+                        message types in the source data
+  --frame_only          Flag indicating that transcoder should only frame
+                        messages to an output source
+  --stats_only          Flag indicating that transcoder should only report on
+                        message type counts without parsing messages further
   --create_schemas_only
-                        Flag indicating that transcoder should only create output resource
-                        schemas and not output message data
+                        Flag indicating that transcoder should only create
+                        output resource schemas and not output message data
 
 Google Cloud arguments:
   --destination_project_id DESTINATION_PROJECT_ID
-                        The Google Cloud project ID for the destination resource
+                        The Google Cloud project ID for the destination
+                        resource
 
 BigQuery arguments:
   --destination_dataset_id DESTINATION_DATASET_ID
-                        The BigQuery dataset for the destination. If it does not exist, it will
-                        be created
+                        The BigQuery dataset for the destination. If it does
+                        not exist, it will be created
 
 Pub/Sub arguments:
   --output_encoding {binary,json}
                         The encoding of the output
   --create_schema_enforcing_topics, --no-create_schema_enforcing_topics
-                        Indicates if Pub/Sub schemas should be created and used to validate
-                        messages sent to a topic (default: True)
+                        Indicates if Pub/Sub schemas should be created and
+                        used to validate messages sent to a topic
+```
+
+### Message handlers
+
+`txcode` supports the execution of _message handler_ classes that can
+be used to statefully mutate in-flight streams and messages. For example,
+`TimestampPullForwardHandler` will look for a `seconds`-styled ITCH
+message (that informs the stream of the prevailing epochs second to
+apply to subsequent messages), and append the latest value from
+that to all subsequent messages (between instances of the `seconds`
+message appearing. This helps individual messages be persisted with
+absolute timestamps that require less context to interpret
+(i.e. outbound messages contain more than just "nanoseconds past
+midnight" for a timestamp.
+
+Another handler is `SequencerHandler`, which appends a sequence number
+to all outbound messages. This is useful when processing bulk messages
+in length-delimited storage formats where the IP packet headers
+containing the original sequence numbers have been stripped.	
+
+`FilterHandler` lets you filter output based upon a specific property
+of a message. A common use for this is to filter messages pertaining
+only to a particular security identifier or symbol.
+
+Here is a combination of transcoding invocations that can
+be used to shard a message universe by trading symbol. First, the mnemonic
+trading symbol identifier (`stock`) must be used to find it's associated integer
+security identifier (`stock_locate`) from the `stock_directory`
+message. `stock_locate` is the identifier included in every
+relevant message (as opposed to `stock`, which is absent from
+certain message types):
+
+```
+
+txcode --source_file 12302019.NASDAQ_ITCH50 --schema_file totalview-itch-50.xml --message_type_inclusions stock_directory --source_file_format_type length_delimited --factory itch --message_handlers FilterHandler:stock=SPY --sampling_count 1
+
+authenticity: P
+etp_flag: Y
+etp_leverage_factor: null
+financial_status_indicator: ' '
+inverse_indicator: null
+ipo_flag: ' '
+issue_classification: Q
+issue_subtype: E
+luld_reference_price_tier: '1'
+market_category: P
+round_lot_size: 100
+round_lots_only: N
+short_sale_threshold_indicator: N
+stock: SPY
+stock_locate: 7451
+timestamp: 11354508113636
+tracking_number: 0
+
+INFO:root:Sampled messages: 1
+INFO:root:Message type inclusions: ['stock_directory']
+INFO:root:Source message count: 7466
+INFO:root:Processed message count: 7451
+INFO:root:Transcoded message count: 1
+INFO:root:Processed schema count: 1
+INFO:root:Summary of message counts: {'stock_directory': 7451}
+INFO:root:Summary of error message counts: {}
+INFO:root:Message rate: 53260.474108 per second
+INFO:root:Total runtime in seconds: 0.140179
+INFO:root:Total runtime in minutes: 0.002336
+```
+
+Taking the value of the field `stock_locate` from the above message
+allows us to filter all messages for that field/value combination. In
+addition, we can append a sequence number to all transcoded messages
+that are output. The below combination returns the original `stock_directory`
+message we used to look up the `stock_locate` code, as well as the
+next two messages in the stream that have the same value for `stock_locate`:
 
 ```
 
+txcode --source_file 12302019.NASDAQ_ITCH50 --schema_file totalview-itch-50.xml --source_file_format_type length_delimited --factory itch --message_handlers FilterHandler:stock_locate=7451,SequencerHandler --sampling_count 3 
+
+authenticity: P
+etp_flag: Y
+etp_leverage_factor: null
+financial_status_indicator: ' '
+inverse_indicator: null
+ipo_flag: ' '
+issue_classification: Q
+issue_subtype: E
+luld_reference_price_tier: '1'
+market_category: P
+round_lot_size: 100
+round_lots_only: N
+sequence_number: 1
+short_sale_threshold_indicator: N
+stock: SPY
+stock_locate: 7451
+timestamp: 11354508113636
+tracking_number: 0
+
+reason: ''
+reserved: ' '
+sequence_number: 2
+stock: SPY
+stock_locate: 7451
+timestamp: 11355134575401
+tracking_number: 0
+trading_state: T
+
+reg_sho_action: '0'
+sequence_number: 3
+stock: SPY
+stock_locate: 7451
+timestamp: 11355134599149
+tracking_number: 0
+
+INFO:root:Sampled messages: 3
+INFO:root:Source message count: 23781
+INFO:root:Processed message count: 23781
+INFO:root:Transcoded message count: 3
+INFO:root:Processed schema count: 21
+INFO:root:Summary of message counts: {'system_event': 1, 'stock_directory': 8906, 'stock_trading_action': 7437, 'reg_sho_restriction': 7437, 'market_participant_position': 0, 'mwcb_decline_level': 0, 'ipo_quoting_period_update': 0, 'luld_auction_collar': 0, 'operational_halt': 0, 'add_order_no_attribution': 0, 'add_order_attribution': 0, 'order_executed': 0, 'order_executed_price': 0, 'order_cancelled': 0, 'order_deleted': 0, 'order_replaced': 0, 'trade': 0, 'cross_trade': 0, 'broken_trade': 0, 'net_order_imbalance': 0, 'retail_price_improvement_indicator': 0}
+INFO:root:Summary of error message counts: {}
+INFO:root:Message rate: 80950.257512 per second
+INFO:root:Total runtime in seconds: 0.293773
+INFO:root:Total runtime in minutes: 0.004896
+
+
+```
+
+The syntax for handler specifications is:
+
+```
+<Handler1>:<Handler1Parameter>=<Handler1Parameter>,<Handler2>
+```
+
+Message handlers are deployed in `transcoder/message/handler/`.
+
 # Installation
 If you are a user looking to use the CLI or library without making changes, you can install the Market Data Transcoder from [PyPI](https://pypi.org/project/market-data-transcoder) using pip:
 ```
 pip install market-data-transcoder
 ```
 
 After the pip installation, you can validate that the transcoder is available by the following command:
```

### Comparing `market-data-transcoder-1.0.2/market_data_transcoder.egg-info/SOURCES.txt` & `market-data-transcoder-1.0.3/market_data_transcoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/setup.cfg` & `market-data-transcoder-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/setup.py` & `market-data-transcoder-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/__init__.py` & `market-data-transcoder-1.0.3/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/__init__.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/__init__.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/stringfix.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/codecs/stringfix.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/__init__.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/fixmessage.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/fixmessage.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/parser.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/parser.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/reference.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/reference.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/pyfixmsg/util.py` & `market-data-transcoder-1.0.3/third_party/pyfixmsg/util.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/sbedecoder/message.py` & `market-data-transcoder-1.0.3/third_party/sbedecoder/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,18 +311,23 @@
     def raw_value(self):
         if self.constant is not None:
             return self.constant
 
         start_index = self.msg_offset + self.relative_offset + self.field_offset
         end_index = start_index + self.field_length
 
-        _, primitive_type_size = TypeMap.primitive_type_map[self.primitive_type]
-        if self.is_int_type() and primitive_type_size != self.field_length:
-            _raw_value = int.from_bytes(self.msg_buffer[start_index: end_index], self.byte_order)
-        else:
+        # Handle variable length integers
+        variable_len_int_handled: bool = False;
+        if self.primitive_type is not None and self.primitive_type in TypeMap.primitive_type_map:
+            _, primitive_type_size = TypeMap.primitive_type_map[self.primitive_type]
+            if self.is_int_type() and primitive_type_size != self.field_length:
+                variable_len_int_handled = True;
+                _raw_value = int.from_bytes(self.msg_buffer[start_index: end_index], self.byte_order)
+
+        if variable_len_int_handled is False:
             _raw_value = unpack_from(self.unpack_fmt, self.msg_buffer, start_index)[0]
 
         return _raw_value
 
     def __repr__(self):
         return self.name
```

### Comparing `market-data-transcoder-1.0.2/third_party/sbedecoder/parser.py` & `market-data-transcoder-1.0.3/third_party/sbedecoder/parser.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/sbedecoder/schema.py` & `market-data-transcoder-1.0.3/third_party/sbedecoder/schema.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/third_party/sbedecoder/typemap.py` & `market-data-transcoder-1.0.3/third_party/sbedecoder/typemap.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/Transcoder.py` & `market-data-transcoder-1.0.3/transcoder/Transcoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,19 @@
 # pylint: disable=broad-except
 
 import importlib
 import logging
 import os
 import signal
 import sys
-
 from datetime import datetime
 
-from transcoder.message.MessageUtil import get_message_parser, parse_handler_config
 from transcoder.message import DatacastParser, NoParser
 from transcoder.message.ErrorWriter import ErrorWriter, TranscodeStep
+from transcoder.message.MessageUtil import get_message_parser, parse_handler_config
 from transcoder.output import get_output_manager
 from transcoder.source import get_message_source
 
 
 # pylint: disable=invalid-name
 class Transcoder:  # pylint: disable=too-many-instance-attributes
     """ Main entry point for transcodihg sessions, bounded by a schema, source and parser """
@@ -62,14 +61,15 @@
         self.create_schemas_only = create_schemas_only
         self.lazy_create_resources = lazy_create_resources
         self.prefix_length = prefix_length
         self.quiet = quiet
         self.start_time = None
         self.stats_only = stats_only
         self.sampling_count = sampling_count
+        self.transcoded_count = 0
 
         self.output_prefix = os.path.basename(
             os.path.splitext(source_file_path)[0]) if source_file_path else 'stdin'
 
         self.error_writer = ErrorWriter(prefix=self.output_prefix,
                                         output_path=self.error_output_path)
 
@@ -110,15 +110,15 @@
                 if self.frame_only:  # don't parse message
                     self.message_parser.process_message(raw_msg)
                     self.output_manager.write_record(None, raw_msg)
                 else:  # parse message
                     if self.stats_only is False:  # output message
                         self.transcode_message(raw_msg)
 
-                if self.message_parser.record_count == self.sampling_count:
+                if self.transcoded_count == self.sampling_count:
                     break
 
         self.print_summary()
 
     def transcode_message(self, raw):
         """ Transcoding steps executed on each source message """
         self.error_writer.set_step(TranscodeStep.PARSE_MESSAGE)
@@ -130,14 +130,16 @@
                 self.handle_exception(raw, msg, msg.exception)
 
             if msg.ignored is False:  # passed inclusions / exclusions
                 self.execute_handlers(msg)
                 if msg.ignored is False:  # passed filters
                     self.error_writer.set_step(TranscodeStep.WRITE_OUTPUT_RECORD)
                     self.output_manager.write_record(msg.name, msg.dictionary)
+                    self.transcoded_count += 1
+
         except Exception as ex:
             self.handle_exception(raw, msg, ex)
 
     def execute_handlers(self, message):
         """ Executes in sequence the message handlers specified for this transcoding instance """
         if self.handlers_enabled is True:  # execute handlers
             self.error_writer.set_step(TranscodeStep.EXECUTE_HANDLERS)
@@ -204,16 +206,17 @@
 
                 if self.message_parser.message_type_inclusions is not None:
                     logging.info('Message type inclusions: %s', self.message_parser.message_type_inclusions)
                 elif self.message_parser.message_type_exclusions is not None:
                     logging.info('Message type exclusions: %s', self.message_parser.message_type_exclusions)
 
                 if self.create_schemas_only is False:
-                    logging.info('Source record count: %s', self.source.record_count)
-                    logging.info('Processed record count: %s', self.message_parser.record_count)
+                    logging.info('Source message count: %s', self.source.record_count)
+                    logging.info('Processed message count: %s', self.message_parser.record_count)
+                    logging.info('Transcoded message count: %s', self.transcoded_count)
                     logging.info('Processed schema count: %s', self.message_parser.total_schema_count)
                     logging.info('Summary of message counts: %s', self.message_parser.record_type_count)
                     logging.info('Summary of error message counts: %s', self.message_parser.error_record_type_count)
                     logging.info('Message rate: %s per second', round(self.source.record_count / total_seconds, 6))
 
             else:
                 logging.info('Source record count: %s', self.source.record_count)
@@ -221,15 +224,15 @@
             logging.info('Total runtime in seconds: %s', round(total_seconds, 6))
             logging.info('Total runtime in minutes: %s', round(total_seconds / 60, 6))
 
     def process_schemas(self):
         """Process the schema specified at runtime"""
         spec_schemas = self.message_parser.process_schema()
         for schema in spec_schemas:
-            if len(schema.fields) == 0:
+            if self.output_manager.supports_zero_field_schemas() is False and len(schema.fields) == 0:
                 logging.info('Schema "%s" contains no field definitions, skipping schema creation', schema.name)
                 continue
 
             for handler in self.all_handlers:
                 if handler.supports_all_message_types is True \
                         or schema.message_id in handler.supported_message_types:
                     handler.append_manufactured_fields(schema)
```

### Comparing `market-data-transcoder-1.0.2/transcoder/__init__.py` & `market-data-transcoder-1.0.3/transcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/main.py` & `market-data-transcoder-1.0.3/transcoder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,15 @@
                                       help='Comma-delimited list of message types to exclude '
                                            'when processing')
     message_filter_group.add_argument('--message_type_inclusions', type=str,
                                       help='Comma-delimited list of message types to include '
                                            'when processing')
 
     source_options_group.add_argument('--sampling_count', type=int, default=None,
-                                      help='To be used for testing only - the sampling count indicates how many of '
-                                           'each distinct '
-                                           'message type to process, any additional will be skipped')
+                                      help='Halt processing after reaching this number of messages. Applied after all Handlers are executed per message')
     source_options_group.add_argument('--skip_bytes', type=int, default=0,
                                       help='Number of bytes to skip before processing the file. Useful for skipping '
                                            'file-level headers')
     source_options_group.add_argument('--skip_lines', type=int, default=0,
                                       help='Number of lines to skip before processing the file')
     source_options_group.add_argument('--source_file_endian', choices=['big', 'little'], default='big',
                                       help='Source file endianness')
```

### Comparing `market-data-transcoder-1.0.2/transcoder/message/DatacastField.py` & `market-data-transcoder-1.0.3/transcoder/message/DatacastField.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/DatacastGroup.py` & `market-data-transcoder-1.0.3/transcoder/message/DatacastGroup.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/DatacastParser.py` & `market-data-transcoder-1.0.3/transcoder/message/DatacastParser.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/DatacastSchema.py` & `market-data-transcoder-1.0.3/transcoder/message/DatacastSchema.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/ErrorWriter.py` & `market-data-transcoder-1.0.3/transcoder/message/ErrorWriter.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/MessageUtil.py` & `market-data-transcoder-1.0.3/transcoder/message/MessageUtil.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/NoParser.py` & `market-data-transcoder-1.0.3/transcoder/message/NoParser.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/ParsedMessage.py` & `market-data-transcoder-1.0.3/transcoder/message/ParsedMessage.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/__init__.py` & `market-data-transcoder-1.0.3/transcoder/message/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/exception/MessageParserNotDefinedError.py` & `market-data-transcoder-1.0.3/transcoder/message/exception/MessageParserNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/exception/ParserFunctionNotDefinedError.py` & `market-data-transcoder-1.0.3/transcoder/message/exception/ParserFunctionNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/exception/__init__.py` & `market-data-transcoder-1.0.3/transcoder/message/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/CmeMessageFactory.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/CmeMessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/ITCHMessageFactory.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/ITCHMessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/MDPMessageFactory.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/MDPMessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/MemxMessageFactory.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/MemxMessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/MessageFactory.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/MessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/__init__.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/exception/FactoryNotFoundError.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/exception/FactoryNotFoundError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/factory/exception/__init__.py` & `market-data-transcoder-1.0.3/transcoder/message/factory/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/CmeBinaryPacketHandler.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/CmeBinaryPacketHandler.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/FilterHandler.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/FilterHandler.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandler.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/MessageHandler.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerFloatField.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/MessageHandlerFloatField.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerIntField.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/MessageHandlerIntField.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerStringField.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/MessageHandlerStringField.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/SequencerHandler.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/SequencerHandler.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/TimestampPullForwardHandler.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/TimestampPullForwardHandler.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/message/handler/__init__.py` & `market-data-transcoder-1.0.3/transcoder/message/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/OutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/OutputManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,19 @@
         raise OutputFunctionNotDefinedError
 
     @staticmethod
     def supports_data_writing():
         """Returns flag indicating if data writes are supported"""
         return True
 
+    @staticmethod
+    def supports_zero_field_schemas():
+        """Returns flag indicating if the output manager support schemas with zero fields"""
+        return False
+
     def __init__(self, schema_max_workers=5, lazy_create_resources: bool = False):
         self.schema_thread_pool_executor: ThreadPoolExecutor = concurrent.futures.ThreadPoolExecutor(
             max_workers=schema_max_workers)
         self.lazy_create_resources = lazy_create_resources
         self.existing_schemas = {}
         self.schema_definitions = {}
         self.schema_futures = []
```

### Comparing `market-data-transcoder-1.0.2/transcoder/output/OutputUtil.py` & `market-data-transcoder-1.0.3/transcoder/output/OutputUtil.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/__init__.py` & `market-data-transcoder-1.0.3/transcoder/output/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/avro/AvroOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/avro/AvroOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/avro/BaseAvroOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/avro/BaseAvroOutputManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 from transcoder.output import OutputManager
 from transcoder.output.exception import OutputFunctionNotDefinedError
 
 
 class BaseAvroOutputManager(OutputManager):
     """Base avro output manager implementation. Used by both avro.io and fastavro implementations."""
 
+    @staticmethod
+    def supports_zero_field_schemas():
+        """Returns flag indicating if the output manager support schemas with zero fields"""
+        return True
+
     def __init__(self, prefix: str, output_path: str, lazy_create_resources: bool = False):
         super().__init__(lazy_create_resources=lazy_create_resources)
         self.prefix = prefix
         self.schemas = {}
         self.writers = {}
         self.output_path = self.create_output_path(output_path, 'avroOut')
```

### Comparing `market-data-transcoder-1.0.2/transcoder/output/avro/FastAvroOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/avro/FastAvroOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/avro/__init__.py` & `market-data-transcoder-1.0.3/transcoder/output/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/diag/DiagnosticOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/diag/DiagnosticOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/diag/__init__.py` & `market-data-transcoder-1.0.3/transcoder/output/diag/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/exception/BigQueryTableSchemaOutOfSyncError.py` & `market-data-transcoder-1.0.3/transcoder/output/exception/BigQueryTableSchemaOutOfSyncError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/exception/OutputFunctionNotDefinedError.py` & `market-data-transcoder-1.0.3/transcoder/output/exception/OutputFunctionNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/exception/OutputManagerSchemaError.py` & `market-data-transcoder-1.0.3/transcoder/output/exception/OutputManagerSchemaError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/exception/OutputNotAvailableError.py` & `market-data-transcoder-1.0.3/transcoder/output/exception/OutputNotAvailableError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/exception/PubSubTopicSchemaOutOfSyncError.py` & `market-data-transcoder-1.0.3/transcoder/output/exception/PubSubTopicSchemaOutOfSyncError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/exception/__init__.py` & `market-data-transcoder-1.0.3/transcoder/output/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/google_cloud/BigQueryOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/google_cloud/BigQueryOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/google_cloud/Constants.py` & `market-data-transcoder-1.0.3/transcoder/output/google_cloud/Constants.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/google_cloud/PubSubOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/google_cloud/PubSubOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/google_cloud/__init__.py` & `market-data-transcoder-1.0.3/transcoder/output/google_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/__init__.py` & `market-data-transcoder-1.0.3/transcoder/output/google_cloud/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/json/JsonOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/json/JsonOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/json/__init__.py` & `market-data-transcoder-1.0.3/transcoder/output/json/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/length_delimited/LengthDelimitedOutputManager.py` & `market-data-transcoder-1.0.3/transcoder/output/length_delimited/LengthDelimitedOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/output/length_delimited/__init__.py` & `market-data-transcoder-1.0.3/transcoder/output/length_delimited/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/LineEncoding.py` & `market-data-transcoder-1.0.3/transcoder/source/LineEncoding.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/Source.py` & `market-data-transcoder-1.0.3/transcoder/source/Source.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/SourceUtil.py` & `market-data-transcoder-1.0.3/transcoder/source/SourceUtil.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/__init__.py` & `market-data-transcoder-1.0.3/transcoder/source/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/file/CmeBinaryPacketFileMessageSource.py` & `market-data-transcoder-1.0.3/transcoder/source/file/CmeBinaryPacketFileMessageSource.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/file/FileMessageSource.py` & `market-data-transcoder-1.0.3/transcoder/source/file/FileMessageSource.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/file/LengthDelimitedFileMessageSource.py` & `market-data-transcoder-1.0.3/transcoder/source/file/LengthDelimitedFileMessageSource.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/file/LineDelimitedFileMessageSource.py` & `market-data-transcoder-1.0.3/transcoder/source/file/LineDelimitedFileMessageSource.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/file/PcapFileMessageSource.py` & `market-data-transcoder-1.0.3/transcoder/source/file/PcapFileMessageSource.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/source/file/__init__.py` & `market-data-transcoder-1.0.3/transcoder/source/file/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/test.py` & `market-data-transcoder-1.0.3/transcoder/test.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.2/transcoder/version.py` & `market-data-transcoder-1.0.3/transcoder/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
```

