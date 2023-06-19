# Comparing `tmp/mosaicml-streaming-0.5.0.tar.gz` & `tmp/mosaicml-streaming-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-streaming-0.5.0.tar", last modified: Tue Jun  6 13:22:20 2023, max compression
+gzip compressed data, was "mosaicml-streaming-0.5.1.tar", last modified: Mon Jun 19 05:49:43 2023, max compression
```

## Comparing `mosaicml-streaming-0.5.0.tar` & `mosaicml-streaming-0.5.1.tar`

### file list

```diff
@@ -1,149 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.304950 mosaicml-streaming-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-06 13:22:20.304950 mosaicml-streaming-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 13:22:20.000000 mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:22:20.304950 mosaicml-streaming-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    53423 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/format/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/format/base/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/base/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/base/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/format/json/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/json/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/json/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/json/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.292950 mosaicml-streaming-0.5.0/streaming/base/format/mds/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/mds/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/mds/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/mds/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/format/xsv/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/xsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/xsv/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/xsv/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/format/xsv/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/partition/orig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shared/scalar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/shuffle/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/py1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/py1s.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/shuffle/py2s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/spanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/base/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/storage/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    22606 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/storage/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/base/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/laion400m/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/laion400m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/crawl_webvid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/extract_webvid_videos.py
--rw-r--r--   0 runner    (1001) docker     (123)    20461 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/multimodal/webvid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/text/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/text/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.296950 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.300950 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/merge_shard_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.300950 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/count_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/enwiki_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/convert/pile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/enwiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/text/pile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.300950 mosaicml-streaming-0.5.0/streaming/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.300950 mosaicml-streaming-0.5.0/streaming/vision/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/fake_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/convert/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/streaming/vision/imagenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:22:20.304950 mosaicml-streaming-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_eviction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_laziness.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_spanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_streaming_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-06 13:22:02.000000 mosaicml-streaming-0.5.0/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.323979 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.323979 mosaicml-streaming-0.5.1/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.323979 mosaicml-streaming-0.5.1/streaming/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54779 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/base/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/json/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/json/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/json/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/mds/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/mds/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/mds/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/mds/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/xsv/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/xsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/xsv/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/xsv/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/xsv/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/partition/orig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/scalar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/shuffle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/py1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/py1s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/py2s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/spanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/storage/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22606 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/storage/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19451 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/multimodal/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/laion400m/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/laion400m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/crawl_webvid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/extract_webvid_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20461 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/webvid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/merge_shard_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/count_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/pile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/enwiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/pile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/streaming/vision/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/fake_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/imagenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_eviction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_laziness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_spanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_streaming_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.5.0/LICENSE` & `mosaicml-streaming-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/PKG-INFO` & `mosaicml-streaming-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.5.0
+Version: 0.5.1
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.1 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
```

### Comparing `mosaicml-streaming-0.5.0/README.md` & `mosaicml-streaming-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/PKG-INFO` & `mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.5.0
+Version: 0.5.1
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.1 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
```

### Comparing `mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/SOURCES.txt` & `mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 mosaicml_streaming.egg-info/top_level.txt
 streaming/__init__.py
 streaming/_version.py
 streaming/py.typed
 streaming/base/__init__.py
 streaming/base/array.py
 streaming/base/compression.py
+streaming/base/constant.py
 streaming/base/dataloader.py
 streaming/base/dataset.py
 streaming/base/distributed.py
 streaming/base/hashing.py
 streaming/base/local.py
 streaming/base/spanner.py
 streaming/base/stream.py
@@ -105,15 +106,17 @@
 tests/test_compression.py
 tests/test_distributed.py
 tests/test_download.py
 tests/test_encodings.py
 tests/test_eviction.py
 tests/test_hashing.py
 tests/test_laziness.py
+tests/test_local.py
 tests/test_mixing.py
+tests/test_partition.py
 tests/test_reader.py
 tests/test_shared.py
 tests/test_shuffle.py
 tests/test_spanner.py
 tests/test_streaming.py
 tests/test_streaming_remote.py
 tests/test_upload.py
```

### Comparing `mosaicml-streaming-0.5.0/mosaicml_streaming.egg-info/requires.txt` & `mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,48 +14,48 @@
 azure-storage-blob<13,>=12.0.0
 
 [all]
 GitPython==3.1.31
 datasets<3,>=2.4.0
 docformatter>=1.4
 docutils==0.18.1
-fastapi==0.96.0
+fastapi==0.97.0
 furo==2023.5.20
 jupyter==1.0.0
 moto<5,>=4.0
 myst-parser==1.0.0
 nbsphinx==0.9.2
 pandoc==2.3
 pre-commit<4,>=2.18.1
-pydantic==1.10.8
+pydantic==1.10.9
 pypandoc==1.11
 pytest-cov<5,>=4
-pytest==7.3.1
+pytest==7.3.2
 pytest_codeblocks==0.16.1
 sphinx-argparse==0.4.0
 sphinx-copybutton==0.5.2
 sphinx-tabs==3.4.1
 sphinx==6.2.1
 toml==0.10.2
 uvicorn==0.22.0
 yamllint==1.32.0
 
 [dev]
 datasets<3,>=2.4.0
 docformatter>=1.4
 jupyter==1.0.0
 pre-commit<4,>=2.18.1
-pytest==7.3.1
+pytest==7.3.2
 pytest_codeblocks==0.16.1
 pytest-cov<5,>=4
 toml==0.10.2
 yamllint==1.32.0
 moto<5,>=4.0
-fastapi==0.96.0
-pydantic==1.10.8
+fastapi==0.97.0
+pydantic==1.10.9
 uvicorn==0.22.0
 
 [docs]
 GitPython==3.1.31
 docutils==0.18.1
 furo==2023.5.20
 myst-parser==1.0.0
```

### Comparing `mosaicml-streaming-0.5.0/pyproject.toml` & `mosaicml-streaming-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/setup.py` & `mosaicml-streaming-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,22 @@
 extra_deps = {}
 
 extra_deps['dev'] = [
     'datasets>=2.4.0,<3',
     'docformatter>=1.4',
     'jupyter==1.0.0',
     'pre-commit>=2.18.1,<4',
-    'pytest==7.3.1',
+    'pytest==7.3.2',
     'pytest_codeblocks==0.16.1',
     'pytest-cov>=4,<5',
     'toml==0.10.2',
     'yamllint==1.32.0',
     'moto>=4.0,<5',
-    'fastapi==0.96.0',
-    'pydantic==1.10.8',
+    'fastapi==0.97.0',
+    'pydantic==1.10.9',
     'uvicorn==0.22.0',
 ]
 
 extra_deps['docs'] = [
     'GitPython==3.1.31',
     'docutils==0.18.1',
     'furo==2023.5.20',
```

### Comparing `mosaicml-streaming-0.5.0/streaming/__init__.py` & `mosaicml-streaming-0.5.1/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/__init__.py` & `mosaicml-streaming-0.5.1/streaming/base/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/array.py` & `mosaicml-streaming-0.5.1/streaming/base/array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/compression.py` & `mosaicml-streaming-0.5.1/streaming/base/compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/dataloader.py` & `mosaicml-streaming-0.5.1/streaming/base/dataloader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/dataset.py` & `mosaicml-streaming-0.5.1/streaming/base/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,32 @@
 from enum import IntEnum
 from math import ceil
 from threading import Event, Lock
 from time import sleep, time_ns
 from typing import Any, Dict, Iterator, Optional, Sequence, Tuple, Union
 
 import numpy as np
-import torch
 from filelock import FileLock
 from numpy.typing import NDArray
 from torch import distributed as dist
 from torch.utils.data import IterableDataset
 
 from streaming.base.array import Array
+from streaming.base.constant import (BARRIER, BARRIER_FILELOCK, CACHE_FILELOCK, CACHE_USAGE,
+                                     EPOCH_DATA, EPOCH_SHAPE, NEXT_EPOCH, RESUME,
+                                     SHARD_ACCESS_TIMES, SHARD_STATES, TICK)
+from streaming.base.distributed import maybe_init_dist
 from streaming.base.format import get_index_basename
 from streaming.base.partition import get_partitions
 from streaming.base.shared import (SharedArray, SharedBarrier, SharedMemory, SharedScalar,
-                                   get_shm_prefix)
+                                   _get_path, get_shm_prefix)
 from streaming.base.shuffle import get_shuffle
 from streaming.base.spanner import Spanner
 from streaming.base.stream import Stream
-from streaming.base.util import TICK, bytes_to_int
+from streaming.base.util import bytes_to_int
 from streaming.base.world import World
 
 # An arbitrary time in the future, used for cold shard eviction.
 NEVER = np.iinfo(np.uint64).max
 
 
 class _ShardState(IntEnum):
@@ -130,33 +133,14 @@
 
     def on_exit(self) -> None:
         """Note that a thread has exited."""
         with self._lock:
             self._num_exited += 1
 
 
-def _maybe_init_dist(world: World) -> bool:
-    """Initialize torch.distributed ourselves, if necessary.
-
-    Args:
-        world (World): Distributed environment.
-
-    Returns:
-        bool: Whether we initialized dist ourselves.
-    """
-    if world.num_ranks == 1 or not dist.is_available() or dist.is_initialized():
-        return False
-    if torch.cuda.is_available() and dist.is_nccl_available():
-        backend = 'nccl'
-    else:
-        backend = 'gloo'
-    dist.init_process_group(backend=backend, rank=world.rank, world_size=world.num_ranks)
-    return True
-
-
 class StreamingDataset(Array, IterableDataset):
     """A mid-epoch-resumable streaming/caching pytorch IterableDataset.
 
     Features elastically deterministic shuffling, which enables fast mid-epoch resumption.
 
     Checkpoints are represented in JSON as follows:
 
@@ -297,16 +281,15 @@
         self.shuffle_algo = shuffle_algo
         self.shuffle_seed = shuffle_seed
         self.shuffle_block_size = shuffle_block_size
 
         # Check streams vs remote/local.
         if bool(streams) == (bool(remote) or bool(local)):
             raise ValueError(
-                'You must provide either "streams" or "remote"/"local", but not both -- ' +
-                'that would be confusing')
+                'You must provide either `streams` or `remote`/`local`, but not both.')
 
         # Initialize the Stream defaults.
         default = Stream(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
@@ -332,15 +315,15 @@
         #
         # Beware: This information is for the per-rank process. DataLoader worker processes may see
         # different values for these fields. We are saving the rank World here because we cannot
         # instantiate a World inside the StreamingDataset destructor.
         self._rank_world = world = World()
 
         # Initialize torch dist ourselves, if necessary.
-        destroy_dist = _maybe_init_dist(world)
+        destroy_dist = maybe_init_dist()
 
         # Download each stream's index, load their shards, and map streams <-> shards.
         self.num_samples = 0
         self.shards = []
         stream_per_shard = []
         self.shard_offset_per_stream = np.zeros(self.num_streams, np.int64)
         self.shards_per_stream = np.zeros(self.num_streams, np.int64)
@@ -366,15 +349,15 @@
         if self.cache_limit:
             if isinstance(self.cache_limit, str):
                 self.cache_limit = bytes_to_int(self.cache_limit)
             min_cache_usage = sum(map(lambda stream: stream.get_index_size(), streams))
             if self.cache_limit <= min_cache_usage:
                 raise ValueError(f'Minimum cache usage ({min_cache_usage} bytes) is larger than ' +
                                  f'the cache limit ({self.cache_limit} bytes). Please raise ' +
-                                 f'cache_limit.')
+                                 f'`cache_limit`.')
 
         # Build the shard index (for partitioning and mapping samples to shards).
         self.samples_per_shard = np.array([shard.samples for shard in self.shards], np.int64)
         self.sample_offset_per_shard = self.samples_per_shard.cumsum() - self.samples_per_shard
         self.spanner = Spanner(self.samples_per_shard)
 
         # Now that we know the number of underlying samples of each stream, derive each stream's
@@ -383,47 +366,47 @@
                                                self.shuffle_seed)
 
         # Length (__len__) is the resampled epoch size divided over the number of devices.
         self.length = ceil(self.epoch_size / world.num_ranks)
 
         # Register/lookup our shared memory prefix and filelock root directory.
         my_locals = [os.path.abspath(os.path.join(x.local, x.split)) for x in streams]
-        self._shm_prefix, self._locals_shm = get_shm_prefix(my_locals, world)
+        self._shm_prefix_int, self._locals_shm = get_shm_prefix(my_locals, world)
         self._filelock_root = os.path.join(os.path.sep, 'tmp', 'streaming')
         os.makedirs(self._filelock_root, exist_ok=True)
 
         # Create the shared memory-backed barrier, without its lock, which is unpickleable.
         self._shared_barrier = SharedBarrier(
-            os.path.join(self._filelock_root, f'{self._shm_prefix}_barrier_filelock'),
-            f'{self._shm_prefix}_barrier')
+            os.path.join(self._filelock_root, _get_path(self._shm_prefix_int, BARRIER_FILELOCK)),
+            _get_path(self._shm_prefix_int, BARRIER))
 
         # Epoch counter.
         #
         # Note: we do not assume that the end of __iter__() will ever be reached, so we need to
         # increment the epoch counter at the start of __iter__() instead of at the end, so we need
         # to track what the next epoch is, not the current epoch.
-        self._next_epoch = SharedScalar(np.int64, f'{self._shm_prefix}_next_epoch')
+        self._next_epoch = SharedScalar(np.int64, _get_path(self._shm_prefix_int, NEXT_EPOCH))
 
         # Cache filelock. Protects downloading and evicting shards.
         self._cache_filelock_path = os.path.join(self._filelock_root,
-                                                 f'{self._shm_prefix}_cache_filelock')
+                                                 _get_path(self._shm_prefix_int, CACHE_FILELOCK))
         self._cache_filelock: FileLock
 
         # Cache usage in bytes.
-        self._cache_usage = SharedScalar(np.int64, f'{self._shm_prefix}_cache_usage')
+        self._cache_usage = SharedScalar(np.int64, _get_path(self._shm_prefix_int, CACHE_USAGE))
 
         # Shard states array. Tells if a shard is missing, downloading, or present (eviction
         # happens under the lock).
         self._shard_states = SharedArray(self.num_shards, np.uint8,
-                                         f'{self._shm_prefix}_shard_states')
+                                         _get_path(self._shm_prefix_int, SHARD_STATES))
 
         # Time of last access per shard. This is used to decide which shard(s) to evict when we run
         # out of space.
         self._shard_access_times = SharedArray(self.num_shards, np.uint64,
-                                               f'{self._shm_prefix}_shard_access_times')
+                                               _get_path(self._shm_prefix_int, SHARD_ACCESS_TIMES))
 
         # Initialize shared memory objects.
         if world.is_local_leader:
             # Set initial epoch (before any resumption).
             self.next_epoch = 0
 
             # Normalize each stream's local dir, discovering which shards are present.
@@ -526,15 +509,15 @@
 
         Args:
             cache_usage (int): Cache usage in bytes.
         """
         self._cache_usage.set(cache_usage)
 
     def __len__(self) -> int:
-        """Get the length as an IterableDataset.
+        """Get the length as a PyTorch IterableDataset.
 
         Returns:
             int: Dataset length.
         """
         return self.length
 
     def _set_predownload(self) -> None:
@@ -551,15 +534,15 @@
             world (World): World state.
             epoch (int): What epoch we think it is (pre-checkpoint).
 
         Returns:
             Tuple[int, int]: What epoch this is, and sample offset in that epoch.
         """
         # Get the resume state, if it exists.
-        name = f'{self._shm_prefix}_resume'
+        name = _get_path(self._shm_prefix_int, RESUME)
         try:
             shm = SharedMemory(name=name, create=False)
         except FileNotFoundError:
             # There is nothing to resume.
             if not self.num_canonical_nodes:
                 self.num_canonical_nodes = world.num_nodes * 64
             self._set_predownload()
@@ -652,15 +635,15 @@
         We just save the state to shared memory for workers to pick up when __iter__ is next
         called. We use shm because changes to this copy of the dataset wouldn't be picked up by
         persistent workers.
 
         Args:
             obj (Dict[str, Any]): The state.
         """
-        name = f'{self._shm_prefix}_resume'
+        name = _get_path(self._shm_prefix_int, RESUME)
         data = json.dumps(obj, sort_keys=True).encode('utf-8')
         # Some platforms choose to allocate chunks of memory based upon that platform's memory page
         # size, hence the exact size of the shared memory block that was returned may be larger
         # than what was requested.
         self._resume_shm = SharedMemory(name=name, size=len(data))
         self._resume_shm.buf[:len(data)] = data
 
@@ -739,15 +722,16 @@
 
         Returns:
             NDArray[np.int64]: The epoch (num physical nodes, ranks per node, workers per rank,
                 batches per worker, batch size).
         """
         # Ensure that num_canonical_nodes has been set.
         if self.num_canonical_nodes is None:
-            raise RuntimeError('Number of canonical nodes can never be None')
+            raise RuntimeError(f'`num_canonical_nodes` can never be None. ' +
+                               f'Provide a positive integer.')
 
         # Sample each shard of each stream according to their proportions/repeats/samples. This
         # gives us the resampled size of each underlying shard, and a mapping from each fake "big"
         # sample ID to its underlying "small" sample ID.
         shuffle_units, small_per_big = self._resample_streams(epoch)
 
         # Partition the global sample space (of resampled "big" sample IDs) into a tensor of shape
@@ -776,25 +760,26 @@
         Returns:
             Tuple[SharedMemory, SharedMemory]: Shared memory arrays containing shape and data.
         """
         ndim = 5
 
         # Validate shape.
         if sample_ids.ndim != ndim:
-            raise ValueError('Sample IDs must be of shape (num physical nodes, ranks per node, ' +
-                             'workers per rank, batches per worker, batch size)')
+            raise ValueError(f'Sample IDs must be of {ndim}D shape (num physical nodes, ' +
+                             f'ranks per node, workers per rank, batches per worker, ' +
+                             f'batch size). Instead, found as {sample_ids.ndim}D shape.')
 
         # Save the generated epoch shape to shared memory.
-        name = f'{self._shm_prefix}_epoch_shape'
+        name = _get_path(self._shm_prefix_int, EPOCH_SHAPE)
         size = ndim * np.int64().nbytes
         shape_shm = SharedMemory(name=name, create=True, size=size, auto_cleanup=False)
         shape_shm.buf[:size] = np.array(sample_ids.shape, np.int64).tobytes()
 
         # Save the generated epoch data to shared memory.
-        name = f'{self._shm_prefix}_epoch_data'
+        name = _get_path(self._shm_prefix_int, EPOCH_DATA)
         size = sample_ids.size * np.int64().nbytes
         data_shm = SharedMemory(name=name, create=True, size=size, auto_cleanup=False)
         data_shm.buf[:size] = sample_ids.tobytes()
 
         return shape_shm, data_shm
 
     def _attach_work(self) -> Tuple[NDArray[np.int64], SharedMemory, SharedMemory]:
@@ -802,21 +787,21 @@
 
         Returns:
             NDArray[np.int64]: Sample IDs.
         """
         ndim = 5
 
         # Load the generated epoch shape from shared memory.
-        name = f'{self._shm_prefix}_epoch_shape'
+        name = _get_path(self._shm_prefix_int, EPOCH_SHAPE)
         size = ndim * np.int64().nbytes
         shape_shm = SharedMemory(name=name, create=False, size=size, auto_cleanup=False)
         shape = tuple(np.ndarray(5, buffer=shape_shm.buf, dtype=np.int64))
 
         # Attach to the generated epoch data in shared memory.
-        name = f'{self._shm_prefix}_epoch_data'
+        name = _get_path(self._shm_prefix_int, EPOCH_DATA)
         size = int(np.prod(shape)) * np.int64().nbytes
         data_shm = SharedMemory(name=name, create=False, size=size, auto_cleanup=False)
         sample_ids = np.ndarray(shape, buffer=data_shm.buf, dtype=np.int64)
 
         return sample_ids, shape_shm, data_shm
 
     def _get_work(self, world: World, epoch: int, sample_in_epoch: int) -> NDArray[np.int64]:
@@ -925,28 +910,28 @@
         This method is multithread/multiprocess-safe.
 
         Args:
             shard_id (int): Shard to evict.
         """
         # Lock the cache. FileLocks contain threading Locks, which are not pickleable, which is
         # incompatible with spawn, so must be created lazily.
-        if not hasattr(self, '_cache_filelock'):
+        if not hasattr(self, CACHE_FILELOCK):
             self._cache_filelock = FileLock(self._cache_filelock_path)
 
         with self._cache_filelock:
             self._evict_shard(shard_id)
 
     def evict_coldest_shard(self) -> None:
         """Evict the coldest (i.e., least recently accessed) shard.
 
         This method is multithread/multiprocess-safe.
         """
         # Lock the cache. FileLocks contain threading Locks, which are not pickleable, which is
         # incompatible with spawn, so must be created lazily.
-        if not hasattr(self, '_cache_filelock'):
+        if not hasattr(self, CACHE_FILELOCK):
             self._cache_filelock = FileLock(self._cache_filelock_path)
 
         with self._cache_filelock:
             self._evict_coldest_shard()
 
     def download_shard(self, shard_id: int, blocking: bool = True) -> None:
         """Download a shard, either waiting or skipping if in progress by another worker.
@@ -959,15 +944,15 @@
         Args:
             shard_id (int): Shard to download.
             blocking (bool): Whether to wait or skip if the shard is currently being downloaded by
                 someone else.
         """
         # Lock the cache. FileLocks contain threading Locks, which are not pickleable, which is
         # incompatible with spawn, so must be created lazily.
-        if not hasattr(self, '_cache_filelock'):
+        if not hasattr(self, CACHE_FILELOCK):
             self._cache_filelock = FileLock(self._cache_filelock_path)
         lock = self._cache_filelock
         lock.acquire()
 
         # Get the state of the shard to download.
         state = self._shard_states[shard_id]
 
@@ -1028,24 +1013,28 @@
     def get_item(self, sample_id: int, retry: int = 7) -> Any:
         """Get sample by global index, blocking to download its shard if not present.
 
         Args:
             sample_id (int): Sample index.
             retry (int): Maximum number of times to download its shard before giving up. In the
                 edge case of a shard being evicted before sample access, you will have to
-                redownload it. Defaults to ``7``.
+                re-download it. Defaults to ``7``.
 
         Returns:
             Dict[str, Any]: Mapping of column name to column data.
         """
+        # Background thread crashed, terminate the main process
+        if hasattr(self, '_event') and self._event.is_set():
+            raise RuntimeError('Background thread failed. Check other traceback.')
         # Locate the shard and sample offset within that shard where the sample lives.
         shard_id, shard_sample_id = self.spanner[sample_id]
         shard = self.shards[shard_id]
 
         sample = None
+        errors = []
         for _ in range(1 + retry):
             try:
                 # Shortcut path: just assume the shard is present. Using exceptions as control flow
                 # is actually faster than checking that the shard is present because python.
                 sample = shard[shard_sample_id]
 
                 # Manually update the last access time afterward. This also happens at the end of
@@ -1054,20 +1043,31 @@
                 # Note: for performance reasons, we have not taken the lock here. This results in
                 # an edge case where a shard has a last access time but is actually not PRESENT.
                 # This impacts _evict_coldest_shard(), which we modify to handle this case.
                 self._shard_access_times[shard_id] = time_ns()
 
                 # On success, break out.
                 break
-            except:
-                # Fallback: ensure the shard is downloaded, then try to access the sample again.
+            except FileNotFoundError as e:
+                # Fallback: shard file is missing (generates `FileNotFoundError` exception),
+                # ensure the shard file is downloaded, then try to access the sample again.
                 # Loops because it may become evicted in the meantime.
+                errors.append(str(e))
                 self.download_shard(shard_id)
         else:
-            raise RuntimeError('StreamingDataset is thrashing. Raise cache_limit.')
+            # Main process failed. Let the threads know to terminate.
+            self._event.set()
+            if self.cache_limit:
+                raise RuntimeError(f'{errors[-1]}. StreamingDataset repeatedly failed to ' +
+                                   f'download a shard. This may be due to thrashing caused by ' +
+                                   f'`cache_limit` being set too low.')
+            else:
+                raise RuntimeError(f'{errors[-1]}. Check if the shard file exists in your ' +
+                                   f'remote location or have you deleted the shard file from ' +
+                                   f'the local directory?')
 
         return sample
 
     def on_exception(self, future: Future) -> None:
         """Raise an exception to the caller if an exception was generated by a thread.
 
         Also, set the thread event to let the other threads know about the exception.
@@ -1105,14 +1105,18 @@
             if it.should_exit():
                 break
 
             # If we're out of samples this epoch, exit this thread because we are done downloading.
             if it.download_index == it.total:
                 break
 
+            # Background thread or a main process crashed, terminate this thread.
+            if self._event.is_set():
+                break
+
             # If we are requested to only pre-download so many samples, if we have as many or more
             # downloaded already, we wait and check again later.
             if self.predownload is not None:
                 samples_ahead = it.download_index - it.yield_index
                 if self.predownload <= samples_ahead:
                     sleep(TICK)
                     continue
@@ -1153,14 +1157,18 @@
             if it.should_exit():
                 break
 
             # If we're out of samples this epoch, exit this thread because we are done downloading.
             if it.ready_index == it.total:
                 break
 
+            # Background thread or a main process crashed, terminate this thread.
+            if self._event.is_set():
+                break
+
             # If we are requested to only pre-download so many samples, if we have as many or more
             # downloaded already, we wait and check again later.
             if self.predownload is not None:
                 samples_ahead = it.ready_index - it.yield_index
                 if self.predownload <= samples_ahead:
                     sleep(TICK)
                     continue
@@ -1208,14 +1216,18 @@
             if it.should_exit():
                 break
 
             # Have we yielded all our samples?
             if it.yield_index == it.total:
                 break
 
+            # Background thread crashed, terminate the main process
+            if self._event.is_set():
+                break
+
             # Is there a sample ready to yield?
             if it.ready_index <= it.yield_index:
                 sleep(TICK)
                 continue
 
             # Yield sample ID if not -1.
             sample_id = it.sample_ids[it.yield_index]
@@ -1241,15 +1253,15 @@
 
         # For exception handling.
         if not hasattr(self, '_executor'):
             self._executor = ThreadPoolExecutor()
         if not hasattr(self, '_event'):
             self._event = Event()
         elif self._event.is_set():
-            raise RuntimeError('Thread failed. Check other traceback.')
+            raise RuntimeError('Background thread failed. Check other traceback.')
 
         # Discover where we left off, if there is a checkpoint, or start at the next epoch.
         # Also pre-increment the epoch counter.
         world = World()
         epoch, sample_in_epoch = self._resume_incr_epoch(world)
 
         # Get this worker's partition of samples to process.
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/distributed.py` & `mosaicml-streaming-0.5.1/streaming/base/distributed.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 from typing import List, TypeVar, cast
 
 import torch.distributed as dist
 
 TObj = TypeVar('TObj')
 
+import torch
 from torch import Tensor
 from torch import distributed as dist
 
 __all__ = [
     'all_gather', 'barrier', 'broadcast', 'get_rank', 'get_local_rank', 'get_local_world_size',
     'get_world_size'
 ]
@@ -106,7 +107,23 @@
     if world_size == 1:
         return [obj]
     raise RuntimeError(''.join([
         f'The world_size({world_size}) > 1, but the distributed package is not available ',
         'or has not been initialized. Please check you have initialized the distributed ',
         'runtime and that PyTorch has been built with distributed support.'
     ]))
+
+
+def maybe_init_dist() -> bool:
+    """Initialize torch.distributed ourselves, if necessary.
+
+    Returns:
+        bool: Whether we initialized dist ourselves.
+    """
+    if get_world_size() == 1 or not dist.is_available() or dist.is_initialized():
+        return False
+    if torch.cuda.is_available() and dist.is_nccl_available():
+        backend = 'nccl'
+    else:
+        backend = 'gloo'
+    dist.init_process_group(backend=backend, rank=get_rank(), world_size=get_world_size())
+    return True
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/__init__.py` & `mosaicml-streaming-0.5.1/streaming/base/format/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/base/reader.py` & `mosaicml-streaming-0.5.1/streaming/base/format/base/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/base/writer.py` & `mosaicml-streaming-0.5.1/streaming/base/format/base/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,26 +71,27 @@
                  extra_bytes_per_shard: int = 0,
                  extra_bytes_per_sample: int = 0,
                  **kwargs: Any) -> None:
 
         compression = compression or None
         if compression:
             if not is_compression(compression):
-                raise ValueError('Invalid compression: {compression}.')
+                raise ValueError(f'Invalid compression: {compression}.')
 
         hashes = hashes or []
         if list(hashes) != sorted(hashes):
             raise ValueError('Hashes must be unique and in sorted order.')
         for algo in hashes:
             if not is_hash(algo):
-                raise ValueError('Invalid hash: {algo}.')
+                raise ValueError(f'Invalid hash: {algo}.')
 
         if size_limit:
             if size_limit < 0:
-                raise ValueError('Size limit, if provided, must be greater than zero.')
+                raise ValueError(f'`size_limit` must be greater than zero, instead, ' +
+                                 f'found as {size_limit}.')
         else:
             size_limit = None
 
         self.keep_local = keep_local
         self.compression = compression
         self.hashes = hashes
         self.size_limit = size_limit
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/json/encodings.py` & `mosaicml-streaming-0.5.1/streaming/base/format/json/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/json/reader.py` & `mosaicml-streaming-0.5.1/streaming/base/format/json/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,17 +65,23 @@
             split (str, optional): Which dataset split to use, if any.
             obj (Dict[str, Any]): JSON object to load.
 
         Returns:
             Self: Loaded JSONReader.
         """
         args = deepcopy(obj)
-        assert args['version'] == 2
+        # Version check.
+        if args['version'] != 2:
+            raise ValueError(f'Unsupported streaming data version: {args["version"]}. ' +
+                             f'Expected version 2.')
         del args['version']
-        assert args['format'] == 'json'
+        # Check format.
+        if args['format'] != 'json':
+            raise ValueError(f'Unsupported data format: {args["format"]}. ' +
+                             f'Expected to be `json`.')
         del args['format']
         args['dirname'] = dirname
         args['split'] = split
         for key in ['raw_data', 'raw_meta', 'zip_data', 'zip_meta']:
             arg = args[key]
             args[key] = FileInfo(**arg) if arg else None
         return cls(**args)
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/json/writer.py` & `mosaicml-streaming-0.5.1/streaming/base/format/json/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/mds/reader.py` & `mosaicml-streaming-0.5.1/streaming/base/format/mds/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,17 +63,21 @@
             split (str, optional): Which dataset split to use, if any.
             obj (Dict[str, Any]): JSON object to load.
 
         Returns:
             Self: Loaded MDSReader.
         """
         args = deepcopy(obj)
-        assert args['version'] == 2
+        if args['version'] != 2:
+            raise ValueError(f'Unsupported streaming data version: {args["version"]}. ' +
+                             f'Expected version 2.')
         del args['version']
-        assert args['format'] == 'mds'
+        if args['format'] != 'mds':
+            raise ValueError(f'Unsupported data format: {args["format"]}. ' +
+                             f'Expected to be `mds`.')
         del args['format']
         args['dirname'] = dirname
         args['split'] = split
         for key in ['raw_data', 'zip_data']:
             arg = args[key]
             args[key] = FileInfo(**arg) if arg else None
         return cls(**args)
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/mds/writer.py` & `mosaicml-streaming-0.5.1/streaming/base/format/mds/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.columns = columns
         self.column_names = []
         self.column_encodings = []
         self.column_sizes = []
         for name in sorted(columns):
             encoding = columns[name]
             if not is_mds_encoding(encoding):
-                raise TypeError(f'MDSWriter passed column "{name}" with encoding "{encoding}" ' +
+                raise TypeError(f'MDSWriter passed column `{name}` with encoding `{encoding}` ' +
                                 f'is unsupported. Supported encodings are {get_mds_encodings()}')
             size = get_mds_encoded_size(encoding)
             self.column_names.append(name)
             self.column_encodings.append(encoding)
             self.column_sizes.append(size)
 
         obj = self.get_config()
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/xsv/encodings.py` & `mosaicml-streaming-0.5.1/streaming/base/format/xsv/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/xsv/reader.py` & `mosaicml-streaming-0.5.1/streaming/base/format/xsv/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,17 +70,21 @@
             split (str, optional): Which dataset split to use, if any.
             obj (Dict[str, Any]): JSON object to load.
 
         Returns:
             Self: Loaded XSVReader.
         """
         args = deepcopy(obj)
-        assert args['version'] == 2
+        if args['version'] != 2:
+            raise ValueError(f'Unsupported streaming data version: {args["version"]}. ' +
+                             f'Expected version 2.')
         del args['version']
-        assert args['format'] == 'xsv'
+        if args['format'] != 'xsv':
+            raise ValueError(f'Unsupported data format: {args["format"]}. ' +
+                             f'Expected to be `xsv`.')
         del args['format']
         args['dirname'] = dirname
         args['split'] = split
         for key in ['raw_data', 'raw_meta', 'zip_data', 'zip_meta']:
             arg = args[key]
             args[key] = FileInfo(**arg) if arg else None
         return cls(**args)
@@ -175,17 +179,21 @@
             split (str, optional): Which dataset split to use, if any.
             obj (Dict[str, Any]): JSON object to load.
 
         Returns:
             Self: Loaded CSVReader.
         """
         args = deepcopy(obj)
-        assert args['version'] == 2
+        if args['version'] != 2:
+            raise ValueError(f'Unsupported streaming data version: {args["version"]}. ' +
+                             f'Expected version 2.')
         del args['version']
-        assert args['format'] == 'csv'
+        if args['format'] != 'csv':
+            raise ValueError(f'Unsupported data format: {args["format"]}. ' +
+                             f'Expected to be `csv`.')
         del args['format']
         args['dirname'] = dirname
         args['split'] = split
         for key in ['raw_data', 'raw_meta', 'zip_data', 'zip_meta']:
             arg = args[key]
             args[key] = FileInfo(**arg) if arg else None
         return cls(**args)
@@ -242,17 +250,21 @@
             split (str, optional): Which dataset split to use, if any.
             obj (Dict[str, Any]): JSON object to load.
 
         Returns:
             Self: Loaded TSVReader.
         """
         args = deepcopy(obj)
-        assert args['version'] == 2
+        if args['version'] != 2:
+            raise ValueError(f'Unsupported streaming data version: {args["version"]}. ' +
+                             f'Expected version 2.')
         del args['version']
-        assert args['format'] == 'tsv'
+        if args['format'] != 'tsv':
+            raise ValueError(f'Unsupported data format: {args["format"]}. ' +
+                             f'Expected to be `tsv`.')
         del args['format']
         args['dirname'] = dirname
         args['split'] = split
         for key in ['raw_data', 'raw_meta', 'zip_data', 'zip_meta']:
             arg = args[key]
             args[key] = FileInfo(**arg) if arg else None
         return cls(**args)
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/format/xsv/writer.py` & `mosaicml-streaming-0.5.1/streaming/base/format/xsv/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/hashing.py` & `mosaicml-streaming-0.5.1/streaming/base/hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/local.py` & `mosaicml-streaming-0.5.1/streaming/base/local.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,33 +30,43 @@
 
         self.local = local
         self.split = split
 
         filename = os.path.join(local, split, get_index_basename())  # pyright: ignore
         obj = json.load(open(filename))
         if obj['version'] != 2:
-            raise ValueError('Unsupported version')
+            raise ValueError(f'Unsupported streaming data version: {obj["version"]}. ' +
+                             f'Expected version 2.')
 
         self.shards = []
         for info in obj['shards']:
             shard = reader_from_json(local, split, info)
             self.shards.append(shard)
         self.num_samples = sum([shard.samples for shard in self.shards])
 
         shard_sizes = np.array([x.samples for x in self.shards])
         self.spanner = Spanner(shard_sizes)
 
     def __len__(self) -> int:
-        """Get the length as an IterableDataset.
+        """Get the length as a PyTorch Dataset.
 
         Returns:
             int: Dataset length.
         """
         return self.num_samples
 
+    @property
+    def size(self) -> int:
+        """Get the size of the dataset in samples.
+
+        Returns:
+            int: Number of samples.
+        """
+        return self.num_samples
+
     def get_item(self, sample_id: int) -> Dict[str, Any]:
         """Get sample by global sample ID.
 
         Args:
             sample_id (int): Sample ID.
 
         Returns:
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/partition/__init__.py` & `mosaicml-streaming-0.5.1/streaming/base/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/partition/orig.py` & `mosaicml-streaming-0.5.1/streaming/base/partition/orig.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Apportion shards/samples to nodes/ranks/workers for elastically deterministic sample order."""
 
+import logging
 import math
 from typing import Optional
 
 import numpy as np
 from numpy.typing import NDArray
 
+logger = logging.getLogger(__name__)
+
 
 def get_partitions_orig(num_samples: int,
                         num_canonical_nodes: int,
                         num_physical_nodes: int,
                         ranks_per_node: int,
                         workers_per_rank: int,
                         batch_size: Optional[int] = None,
@@ -35,27 +38,37 @@
             partitioned over the workers. Defaults to ``None``.
         drop_first (int): Number of samples seen already, which are dropped. Defaults to ``0``.
 
     Returns:
         NDArray[np.int64]: Partitions of shape (physical nodes, ranks per node, workers per rank,
             batches per worker, batch size).
     """
+    if num_samples <= drop_first:
+        raise ValueError(f'Resuming further into the dataset ({drop_first}) than it has samples ' +
+                         f'({num_samples})')
+
     if num_canonical_nodes < num_physical_nodes:
         if num_physical_nodes % num_canonical_nodes:
             raise ValueError('Either canonical or physical nodes must be evenly divisible by ' +
                              'the other, otherwise striping slices of shards over nodes may ' +
                              'lead to each node downloading all shards')
     elif num_physical_nodes < num_canonical_nodes:
         if num_canonical_nodes % num_physical_nodes:
             raise ValueError('Either canonical or physical nodes must be evenly divisible by ' +
                              'the other, otherwise striping slices of shards over nodes may ' +
                              'lead to each node downloading all shards')
 
     batch_size = batch_size or 1
 
+    # If drop_first isn't a multiple of num_physical_nodes, round down to make it divisible.
+    if drop_first % num_physical_nodes:
+        logger.warn('`drop_first` was not divisible by `num_physical_nodes`. Rounding it down ' +
+                    'to make it divisible.')
+        drop_first -= drop_first % num_physical_nodes
+
     # Divide the full dataset sample range into a sample range per canonical node.
     samples_per_canonical_node = (num_samples + num_canonical_nodes - 1) // num_canonical_nodes
     node_ratio = 0
     padding = 0
     if num_canonical_nodes < num_physical_nodes:
         node_ratio = num_physical_nodes // num_canonical_nodes
         overflow = samples_per_canonical_node % node_ratio
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shared/__init__.py` & `mosaicml-streaming-0.5.1/streaming/base/shared/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 For when using `threading` or `multiprocessing` from the python standard library won't do, because
 we are coordinating separately instantiated pytorch worker processes.
 """
 
 from streaming.base.shared.array import SharedArray as SharedArray
 from streaming.base.shared.barrier import SharedBarrier as SharedBarrier
 from streaming.base.shared.memory import SharedMemory as SharedMemory
+from streaming.base.shared.prefix import _get_path as _get_path
 from streaming.base.shared.prefix import get_shm_prefix as get_shm_prefix
 from streaming.base.shared.scalar import SharedScalar as SharedScalar
 
 __all__ = ['SharedArray', 'SharedBarrier', 'SharedMemory', 'get_shm_prefix', 'SharedScalar']
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shared/array.py` & `mosaicml-streaming-0.5.1/streaming/base/shared/array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shared/barrier.py` & `mosaicml-streaming-0.5.1/streaming/base/shared/barrier.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 """
 
 from time import sleep
 
 import numpy as np
 from filelock import FileLock
 
+from streaming.base.constant import TICK
 from streaming.base.shared.array import SharedArray
 
-# Time to wait, in seconds.
-TICK = 0.07
-
 # Time out to wait before raising exception
 TIMEOUT = 60
 
 
 class SharedBarrier:
     """A barrier that works inter-process using a filelock and shared memory.
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shared/memory.py` & `mosaicml-streaming-0.5.1/streaming/base/shared/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 import atexit
 from multiprocessing import resource_tracker  # pyright: ignore
 from multiprocessing.shared_memory import SharedMemory as BuiltinSharedMemory
 from time import sleep
 from typing import Any, Optional
 
-# Time to wait, in seconds.
-TICK = 0.07
+from streaming.base.constant import TICK
 
 
 class SharedMemory:
     """Improved quiet implementation of shared memory.
 
     Args:
         name (str, optional): A unique shared memory block name. Defaults to ``None``.
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shared/prefix.py` & `mosaicml-streaming-0.5.1/streaming/base/shared/prefix.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from time import sleep
 from typing import Iterator, List, Set, Tuple
 
 import numpy as np
 from torch import distributed as dist
 
+from streaming.base.constant import LOCALS, TICK
 from streaming.base.shared import SharedMemory
-from streaming.base.util import TICK
 from streaming.base.world import World
 
 
 def _each_prefix_int() -> Iterator[int]:
     """Get each possible prefix int to check in order.
 
     Returns:
@@ -26,14 +26,27 @@
     """
     prefix_int = 0
     while True:
         yield prefix_int
         prefix_int += 1
 
 
+def _get_path(prefix_int: int, name: str) -> str:
+    """Get the name of the shared memory.
+
+    Args:
+        prefix (int): The prefix int.
+        name (str): The name of the shared memory.
+
+    Returns:
+        str: Unique shared memory name.
+    """
+    return f'{prefix_int:06}_{name}'
+
+
 def _pack_locals(dirnames: Set[str]) -> bytes:
     """Pack local dirnames.
 
     Args:
         dirnames (Set[str]): Unpacked local dirnames.
 
     Returns:
@@ -87,25 +100,28 @@
         my_locals_set (Set[str]): Our local working directories.
 
     Returns:
         int: Next available prefix int.
     """
     prefix_int = 0
     for prefix_int in _each_prefix_int():
-        prefix = f'{prefix_int:06}'
-        name = f'{prefix}_locals'
+        name = _get_path(prefix_int, LOCALS)
         try:
             shm = SharedMemory(name, False)
         except FileNotFoundError:
             break
         their_locals_set = _unpack_locals(bytes(shm.buf))
         both = my_locals_set & their_locals_set
         if both:
             raise ValueError(f'Reused local directory: {sorted(my_locals_set)} vs ' +
-                             f'{sorted(their_locals_set)}. Provide a different one.')
+                             f'{sorted(their_locals_set)}. Provide a different one. If using ' +
+                             f'a unique local directory, try deleting the local directory and ' +
+                             f'call `streaming.base.util.clean_stale_shared_memory()` only once ' +
+                             f'in your script to clean up the stale shared memory before ' +
+                             f'instantiation of `StreamingDataset`.')
     return prefix_int
 
 
 def _check_and_find_retrying(my_locals_set: Set[str], retry: int) -> int:
     """Find the next available prefix while checking existing dirs for overlap.
 
     If an overlap is found, sleeps for a tick and then tries again, up to "retry" times. We allow
@@ -129,49 +145,48 @@
             errs.append(err)
             sleep(TICK)
     raise errs[-1]
 
 
 def get_shm_prefix(my_locals: List[str],
                    world: World,
-                   retry: int = 100) -> Tuple[str, SharedMemory]:
+                   retry: int = 100) -> Tuple[int, SharedMemory]:
     """Register or lookup our shared memory prefix.
 
     Args:
         my_locals (List[str]): Local working dir of each stream, relative to /. We need to verify
             that there is no overlap with any other currently running StreamingDataset.
         world (World): Information about nodes, ranks, and workers.
-        retry (int): Number of retries upon failure before raising an exception. Defaults to ``7``.
+        retry (int): Number of retries upon failure before raising an exception. Defaults to ``100``.
 
     Returns:
-        Tuple[str, SharedMemory]: Shared memory prefix and object. The name is required to be very
+        Tuple[int, SharedMemory]: Shared memory integer prefix and object. The name is required to be very
             short due to limitations of Python on Mac OSX.
     """
     # Check my locals for overlap.
     my_locals_set = _check_self(my_locals)
 
     # First, the local leader registers the first available shm prefix, recording its locals.
     if world.is_local_leader:
         prefix_int = _check_and_find_retrying(my_locals_set, retry)
-        prefix = f'{prefix_int:06}'  # pyright: ignore
-        name = f'{prefix}_locals'
+        name = _get_path(prefix_int, LOCALS)
         data = _pack_locals(my_locals_set)
         shm = SharedMemory(name, True, len(data))
         shm.buf[:len(data)] = data
 
     if dist.is_available() and dist.is_initialized():
         dist.barrier()
 
     # Non-local leaders go next, searching for match.
     if not world.is_local_leader:
         for prefix_int in _each_prefix_int():
-            prefix = f'{prefix_int:06}'
-            name = f'{prefix}_locals'
+            name = _get_path(prefix_int, LOCALS)
             try:
                 shm = SharedMemory(name, False)
             except FileNotFoundError:
-                raise RuntimeError('Internal error: shm prefix was not registered by local leader')
+                raise RuntimeError(f'Internal error: shared memory prefix was not registered by ' +
+                                   f'local leader')
             their_locals_set = _unpack_locals(bytes(shm.buf))
             if my_locals_set == their_locals_set:
                 break
 
-    return prefix, shm  # pyright: ignore
+    return prefix_int, shm  # pyright: ignore
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shared/scalar.py` & `mosaicml-streaming-0.5.1/streaming/base/shared/scalar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shuffle/__init__.py` & `mosaicml-streaming-0.5.1/streaming/base/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shuffle/naive.py` & `mosaicml-streaming-0.5.1/streaming/base/shuffle/naive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shuffle/py1b.py` & `mosaicml-streaming-0.5.1/streaming/base/shuffle/py1b.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shuffle/py1s.py` & `mosaicml-streaming-0.5.1/streaming/base/shuffle/py1s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/shuffle/py2s.py` & `mosaicml-streaming-0.5.1/streaming/base/shuffle/py2s.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class _Shard(object):
     """Shard ID paired with its sample IDs.
 
     Args:
         index (int): Shard ID.
-        smaples (NDArray[np.int64]): Sample IDs
+        samples (NDArray[np.int64]): Sample IDs
     """
 
     def __init__(self, index: int, samples: NDArray[np.int64]) -> None:
         self.index = index
         self.samples = samples
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/spanner.py` & `mosaicml-streaming-0.5.1/streaming/base/spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/storage/__init__.py` & `mosaicml-streaming-0.5.1/streaming/base/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/storage/download.py` & `mosaicml-streaming-0.5.1/streaming/base/storage/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     from boto3.s3.transfer import TransferConfig
     from botocore import UNSIGNED
     from botocore.config import Config
     from botocore.exceptions import ClientError, NoCredentialsError
 
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 's3':
-        raise ValueError(f'Expected obj.scheme to be "s3", got {obj.scheme} for remote={remote}')
+        raise ValueError(
+            f'Expected obj.scheme to be `s3`, instead, got {obj.scheme} for remote={remote}')
 
     extra_args = {}
     # When enabled, the requester instead of the bucket owner pays the cost of the request
     # and the data download from the bucket.
     if os.environ.get('MOSAICML_STREAMING_AWS_REQUESTER_PAYS') is not None:
         requester_pays_buckets = os.environ.get(  # yapf: ignore
             'MOSAICML_STREAMING_AWS_REQUESTER_PAYS').split(',')  # pyright: ignore
@@ -159,15 +160,16 @@
     """
     import boto3
     from boto3.s3.transfer import TransferConfig
     from botocore.exceptions import ClientError
 
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 'gs':
-        raise ValueError(f'Expected obj.scheme to be "gs", got {obj.scheme} for remote={remote}')
+        raise ValueError(
+            f'Expected obj.scheme to be `gs`, instead, got {obj.scheme} for remote={remote}')
 
     # Create a new session per thread
     session = boto3.session.Session()
     # Create a resource client using a thread's session object
     gcs_client = session.client('s3',
                                 region_name='auto',
                                 endpoint_url='https://storage.googleapis.com',
@@ -198,15 +200,16 @@
     import oci
     config = oci.config.from_file()
     client = oci.object_storage.ObjectStorageClient(
         config=config, retry_strategy=oci.retry.DEFAULT_RETRY_STRATEGY)
     namespace = client.get_namespace().data
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 'oci':
-        raise ValueError(f'Expected obj.scheme to be "oci", got {obj.scheme} for remote={remote}')
+        raise ValueError(
+            f'Expected obj.scheme to be `oci`, instead, got {obj.scheme} for remote={remote}')
 
     bucket_name = obj.netloc.split('@' + namespace)[0]
     # Remove leading and trailing forward slash from string
     object_path = obj.path.strip('/')
     object_details = client.get_object(namespace, bucket_name, object_path)
     local_tmp = local + '.tmp'
     with open(local_tmp, 'wb') as f:
@@ -224,15 +227,15 @@
     """
     from azure.core.exceptions import ResourceNotFoundError
     from azure.storage.blob import BlobServiceClient
 
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 'azure':
         raise ValueError(
-            f'Expected obj.scheme to be "azure", got {obj.scheme} for remote={remote}')
+            f'Expected obj.scheme to be `azure`, instead, got {obj.scheme} for remote={remote}')
 
     # Create a new session per thread
     service = BlobServiceClient(
         account_url=f"https://{os.environ['AZURE_ACCOUNT_NAME']}.blob.core.windows.net",
         credential=os.environ['AZURE_ACCOUNT_ACCESS_KEY'])
     try:
         blob_client = service.get_blob_client(container=obj.netloc, blob=obj.path.lstrip('/'))
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/storage/upload.py` & `mosaicml-streaming-0.5.1/streaming/base/storage/upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/base/stream.py` & `mosaicml-streaming-0.5.1/streaming/base/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from typing import List, Optional, Sequence
 
 import numpy as np
 from numpy.typing import NDArray
 from typing_extensions import Self
 
 from streaming.base.compression import decompress
+from streaming.base.constant import TICK
 from streaming.base.format import FileInfo, Reader, get_index_basename, reader_from_json
 from streaming.base.hashing import get_hash
 from streaming.base.storage import download_file
-from streaming.base.util import TICK, wait_for_file_to_exist
+from streaming.base.util import wait_for_file_to_exist
 from streaming.base.world import World
 
 
 class Stream:
     """A dataset, or sub-dataset if mixing, from which we stream/cache samples.
 
     We initialize a StreamingDataset with one or more Streams. Streams may be resampled to achieve
@@ -100,45 +101,45 @@
         self.local = local or mkdtemp()
         self.split = split or ''
 
         has_proportion = proportion is not None
         has_repeat = repeat is not None
         has_choose = choose is not None
         if not (0 <= has_proportion + has_repeat + has_choose <= 1):
-            raise ValueError('At most one of "proportion", "repeat", and "choose" may be ' +
+            raise ValueError('At most one of `proportion`, `repeat`, and `choose` may be ' +
                              'specified; the others are derived')
 
         self._proportion = proportion
         if proportion is not None:
             if proportion < 0:
-                raise ValueError('Proportion must be non-negative')
+                raise ValueError('`proportion` must be non-negative')
             self.proportion = proportion
 
         self._repeat = repeat
         if repeat is not None:
             if repeat < 0:
-                raise ValueError('Repeat must be non-negative')
+                raise ValueError('`repeat` must be non-negative')
             self.repeat = repeat
 
         self._choose = choose
         if choose is not None:
             if choose < 0:
-                raise ValueError('Choose must be non-negative')
+                raise ValueError('`choose` must be non-negative')
             self.choose = choose
 
         self._download_retry = download_retry
         if download_retry is not None:
             if download_retry < 0:
-                raise ValueError('Download retry must be non-negative')
+                raise ValueError('`download_retry` must be non-negative')
             self.download_retry = download_retry
 
         self._download_timeout = download_timeout
         if download_timeout is not None:
             if download_timeout <= 0:
-                raise ValueError('Download timeout must be positive')
+                raise ValueError('`download_timeout` must be positive')
             self.download_timeout = download_timeout
 
         self.validate_hash = validate_hash
 
         self._keep_zip = keep_zip
         if keep_zip is not None:
             self.keep_zip = keep_zip
@@ -149,15 +150,15 @@
 
         We use pairs of (name, _name) in order to make type checking happy.
 
         Args:
             default (Self): Stream containing default values for all optional fields.
         """
         if not (self.remote or self._local):
-            raise ValueError('Remote and/or local path must be provided')
+            raise ValueError('`remote` and/or `local` path must be provided')
 
         if not self.split:
             self.split = default.split or ''
         if self._download_retry is None:
             self.download_retry = default.download_retry
         if self._download_timeout is None:
             self.download_timeout = default.download_timeout
@@ -180,18 +181,18 @@
         # Validate stream weights ("proportion", "repeat", "choose", or none).
         is_proportional = hasattr(streams[0], 'proportion')
         for stream_id, stream in enumerate(streams):
             has_proportion = hasattr(stream, 'proportion')
             has_repeat = hasattr(stream, 'repeat')
             has_choose = hasattr(stream, 'choose')
             if not (0 <= has_proportion + has_repeat + has_choose <= 1):
-                raise ValueError(f'Streams must provide at most one of "proportion", "repeat", ' +
-                                 f'or "choose" (error in stream {stream_id})')
+                raise ValueError(f'Streams must provide at most one of `proportion`, `repeat`, ' +
+                                 f'or `choose` (error in stream {stream_id})')
             if is_proportional != has_proportion:
-                raise ValueError(f'Relative ("proportion") and absolute ("repeat", "choose", ' +
+                raise ValueError(f'Relative (`proportion`) and absolute (`repeat`, `choose`, ' +
                                  f'none) stream weights are incompatible with each other (error ' +
                                  f'in stream {stream_id})')
         return is_proportional
 
     @classmethod
     def apply_weights(cls, streams: Sequence[Self], samples_per_stream: NDArray[np.int64],
                       choose_per_epoch: Optional[int], seed: int) -> int:
@@ -223,15 +224,15 @@
             rng = np.random.default_rng(seed)
             indices = rng.choice(len(streams), shortfall, False)
             choose_per_stream[indices] += 1
             repeat_per_stream = choose_per_stream / samples_per_stream
         else:
             # Absolute.
             if choose_per_epoch:
-                raise ValueError('Only provide "choose" when weighting streams relatively')
+                raise ValueError('Only provide `choose` when weighting streams relatively')
             choose_per_stream = np.zeros(len(streams), np.int64)
             for stream_id, stream in enumerate(streams):
                 if hasattr(stream, 'repeat'):
                     choose = int(stream.repeat * samples_per_stream[stream_id])
                 elif hasattr(stream, 'choose'):
                     choose = stream.choose
                 else:
@@ -277,15 +278,16 @@
             except Exception as e:  # Retry for all other causes of failure.
                 errors.append(e)
                 continue
             break
 
         if self.download_retry < len(errors):
             raise RuntimeError(
-                f'Failed to download {remote} -> {local}. Got errors:\n{errors}') from errors[-1]
+                f'Failed to download {remote} -> {local}. Tried {1 + self.download_retry} ' +
+                f'times, got errors:\n{errors}') from errors[-1]
 
         return local
 
     def _decompress_shard_part(self, zip_info: FileInfo, zip_filename: str, raw_filename: str,
                                compression: Optional[str]) -> None:
         """Validate and decompress shard data.
 
@@ -377,30 +379,33 @@
         filename = os.path.join(self.local, self.split, basename)  # pyright: ignore
         if world.is_local_leader:
             if self.remote:
                 tmp_filename = self._download_file(basename, basename + '.tmp')
                 os.rename(tmp_filename, filename)
             else:
                 if not os.path.exists(filename):
-                    raise RuntimeError(f'No remote provided, but local file {filename} does not ' +
-                                       'exist either')
+                    raise RuntimeError(f'No `remote` provided, but local file {filename} ' +
+                                       'does not exist either')
         else:
-            wait_for_file_to_exist(filename, TICK, 60,
-                                   f'Index file {filename} took too long to download')
+            wait_for_file_to_exist(
+                filename, TICK, self.download_timeout,
+                f'Index file {filename} took too long to download. Either ' +
+                f'increase the `download_timeout` value or check the other ' + f'traceback.')
 
         # Load the index.
         try:
             obj = json.load(open(filename))
         except json.decoder.JSONDecodeError as error:
             error.args = (f'Index file at {filename} is empty or corrupted. ' + error.args[0],)
             raise error
 
         # Version check.
         if obj['version'] != 2:
-            raise ValueError(f'Unsupported version: {obj["version"]}')
+            raise ValueError(f'Unsupported streaming data version: {obj["version"]}. ' +
+                             f'Expected version 2.')
 
         # Initialize shard readers according to the loaded info.
         shards = []
         for info in obj['shards']:
             shard = reader_from_json(self.local, self.split, info)
             shards.append(shard)
```

### Comparing `mosaicml-streaming-0.5.0/streaming/base/world.py` & `mosaicml-streaming-0.5.1/streaming/base/world.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py` & `mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/crawl_webvid.py` & `mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/crawl_webvid.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py` & `mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/multimodal/convert/webvid/extract_webvid_videos.py` & `mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/extract_webvid_videos.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/multimodal/webvid.py` & `mosaicml-streaming-0.5.1/streaming/multimodal/webvid.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/c4.py` & `mosaicml-streaming-0.5.1/streaming/text/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/c4.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/create_pretraining_data.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/make_train_parallel.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/merge_shard_groups.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/merge_shard_groups.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/pick_eval_samples.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/mds/tokenization.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/count_samples.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/count_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki/tfrecord/tokenization.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/enwiki_text.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki_text.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/convert/pile.py` & `mosaicml-streaming-0.5.1/streaming/text/convert/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/enwiki.py` & `mosaicml-streaming-0.5.1/streaming/text/enwiki.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/text/pile.py` & `mosaicml-streaming-0.5.1/streaming/text/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/ade20k.py` & `mosaicml-streaming-0.5.1/streaming/vision/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/base.py` & `mosaicml-streaming-0.5.1/streaming/vision/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/cifar10.py` & `mosaicml-streaming-0.5.1/streaming/vision/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/coco.py` & `mosaicml-streaming-0.5.1/streaming/vision/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/convert/ade20k.py` & `mosaicml-streaming-0.5.1/streaming/vision/convert/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/convert/base.py` & `mosaicml-streaming-0.5.1/streaming/vision/convert/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/convert/cifar10.py` & `mosaicml-streaming-0.5.1/streaming/vision/convert/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/convert/coco.py` & `mosaicml-streaming-0.5.1/streaming/vision/convert/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/convert/fake_cifar10.py` & `mosaicml-streaming-0.5.1/streaming/vision/convert/fake_cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/convert/imagenet.py` & `mosaicml-streaming-0.5.1/streaming/vision/convert/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/streaming/vision/imagenet.py` & `mosaicml-streaming-0.5.1/streaming/vision/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_array.py` & `mosaicml-streaming-0.5.1/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_barrier.py` & `mosaicml-streaming-0.5.1/tests/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_compression.py` & `mosaicml-streaming-0.5.1/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_distributed.py` & `mosaicml-streaming-0.5.1/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_download.py` & `mosaicml-streaming-0.5.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_encodings.py` & `mosaicml-streaming-0.5.1/tests/test_encodings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 import json
 import tempfile
-from typing import Any, Union
+from typing import Any, Tuple, Union
 
 import numpy as np
 import pytest
 from PIL import Image
 
 import streaming.base.format.json.encodings as jsonEnc
 import streaming.base.format.mds.encodings as mdsEnc
@@ -71,14 +71,70 @@
 
     @pytest.mark.parametrize('data', [b'9', 25.9])
     def test_int_encode_invalid_data(self, data: Any):
         with pytest.raises(AttributeError):
             int_enc = mdsEnc.Int()
             _ = int_enc.encode(data)
 
+    @pytest.mark.parametrize('dtype_str', [
+        'uint8',
+        'uint16',
+        'uint32',
+        'uint64',
+        'int8',
+        'int16',
+        'int32',
+        'int64',
+        'float16',
+        'float32',
+        'float64',
+    ])
+    @pytest.mark.parametrize('shape', [
+        (1,),
+        (1, 1),
+        (2, 3, 4, 5),
+        (1, 3, 1, 3, 1),
+        (300,),
+        (1, 256, 1),
+        (65536, 7, 1),
+    ])
+    def test_ndarray_encode_decode(self, dtype_str: str, shape: Tuple[int]):
+        dtype = getattr(np, dtype_str)
+        a = np.random.randint(0, 1000, shape).astype(dtype)
+
+        encoding = 'ndarray'
+        assert mdsEnc.is_mds_encoding(encoding)
+        assert mdsEnc.get_mds_encoded_size(encoding) is None
+        b = mdsEnc.mds_encode(encoding, a)
+        c = mdsEnc.mds_decode(encoding, b)
+        assert (a == c).all()
+        b1_len = len(b)
+
+        encoding = f'ndarray:{dtype.__name__}'
+        assert mdsEnc.is_mds_encoding(encoding)
+        assert mdsEnc.get_mds_encoded_size(encoding) is None
+        b = mdsEnc.mds_encode(encoding, a)
+        c = mdsEnc.mds_decode(encoding, b)
+        assert (a == c).all()
+        b2_len = len(b)
+
+        shape_str = ','.join(map(str, shape))
+        encoding = f'ndarray:{dtype.__name__}:{shape_str}'
+        assert mdsEnc.is_mds_encoding(encoding)
+        b_size = mdsEnc.get_mds_encoded_size(encoding)
+        assert b_size is not None
+        b = mdsEnc.mds_encode(encoding, a)
+        c = mdsEnc.mds_decode(encoding, b)
+        assert (a == c).all()
+        assert len(b) == b_size
+        b3_len = len(b)
+
+        assert b3_len < b2_len < b1_len
+        assert b3_len == np.prod(shape) * dtype().nbytes
+
     @pytest.mark.parametrize('mode', ['I', 'L', 'RGB'])
     def test_pil_encode_decode(self, mode: str):
         pil_enc = mdsEnc.PIL()
         assert pil_enc.size is None
 
         # Creating the (32 x 32) NumPy Array with random values
         np_data = np.random.randint(255, size=(32, 32), dtype=np.uint32)
@@ -365,15 +421,17 @@
         assert dec == decoded
 
     def test_get_mds_encodings(self):
         uints = {'uint8', 'uint16', 'uint32', 'uint64'}
         ints = {'int8', 'int16', 'int32', 'int64'}
         floats = {'float16', 'float32', 'float64'}
         scalars = uints | ints | floats
-        expected_encodings = {'int', 'bytes', 'json', 'png', 'jpeg', 'str', 'pil', 'pkl'} | scalars
+        expected_encodings = {
+            'int', 'bytes', 'json', 'ndarray', 'png', 'jpeg', 'str', 'pil', 'pkl'
+        } | scalars
         enc = mdsEnc.get_mds_encodings()
         assert len(enc) == len(expected_encodings)
         assert enc == expected_encodings
 
     @pytest.mark.parametrize(('enc_name', 'expected_output'), [('jpeg', True), ('', False),
                                                                ('pngg', False)])
     def test_is_mds_encoding(self, enc_name: str, expected_output: bool):
```

### Comparing `mosaicml-streaming-0.5.0/tests/test_eviction.py` & `mosaicml-streaming-0.5.1/tests/test_eviction.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 def shard_eviction_disabled(remote: str, local: str, keep_zip: bool):
     """
     With shard eviction disabled.
     """
     dataset = StreamingDataset(remote=remote, local=local, keep_zip=keep_zip)
-    for _ in range(3):
+    for _ in range(2):
         for sample in dataset:  # pyright: ignore
             pass
 
     validate(remote, local, dataset, keep_zip, False)
     rmtree(local, ignore_errors=False)
 
 
@@ -57,28 +57,32 @@
     With no shard evictions because cache_limit is bigger than the dataset.
     """
     dataset = StreamingDataset(remote=remote,
                                local=local,
                                keep_zip=keep_zip,
                                cache_limit=1_000_000)
     dataloader = DataLoader(dataset=dataset, num_workers=8)
-    for _ in range(3):
+    for _ in range(2):
         for _ in dataloader:
             pass
     validate(remote, local, dataset, keep_zip, False)
     rmtree(local, ignore_errors=False)
 
 
 def shard_eviction(remote: str, local: str, keep_zip: bool):
     """
     With shard eviction because cache_limit is smaller than the whole dataset.
     """
-    dataset = StreamingDataset(remote=remote, local=local, keep_zip=keep_zip, cache_limit='50kb')
+    cache_limit = '120kb' if keep_zip else '100kb'
+    dataset = StreamingDataset(remote=remote,
+                               local=local,
+                               keep_zip=keep_zip,
+                               cache_limit=cache_limit)
     dataloader = DataLoader(dataset=dataset, num_workers=8)
-    for _ in range(3):
+    for _ in range(2):
         for _ in dataloader:
             pass
     validate(remote, local, dataset, keep_zip, True)
     rmtree(local, ignore_errors=False)
 
 
 def manual_shard_eviction(remote: str, local: str, keep_zip: bool):
```

### Comparing `mosaicml-streaming-0.5.0/tests/test_hashing.py` & `mosaicml-streaming-0.5.1/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_laziness.py` & `mosaicml-streaming-0.5.1/tests/test_laziness.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_mixing.py` & `mosaicml-streaming-0.5.1/tests/test_mixing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_reader.py` & `mosaicml-streaming-0.5.1/tests/test_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,7 +286,22 @@
 
     # Creates a `index.json` file and write the content to it
     with open(os.path.join(local_dir, filename), 'w') as outfile:
         json.dump(content, outfile)
 
     with pytest.raises(RuntimeError, match=f'Stream contains no samples: .*'):
         _ = StreamingDataset(local=local_dir)
+
+
+@pytest.mark.usefixtures('mds_dataset_dir')
+def test_accidental_shard_delete_exception(mds_dataset_dir: Any):
+    remote_dir, local_dir = mds_dataset_dir
+    filename = 'shard.00000.mds'
+    dataset = StreamingDataset(local=local_dir, remote=remote_dir)
+
+    with pytest.raises(RuntimeError,
+                       match=f'.*Check if the shard file exists in your remote location.*'):
+        for _ in dataset:
+            if os.path.exists(os.path.join(local_dir, filename)):
+                os.remove(os.path.join(local_dir, filename))
+            pass
+    shutil.rmtree(local_dir, ignore_errors=True)
```

### Comparing `mosaicml-streaming-0.5.0/tests/test_shared.py` & `mosaicml-streaming-0.5.1/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_shuffle.py` & `mosaicml-streaming-0.5.1/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_spanner.py` & `mosaicml-streaming-0.5.1/tests/test_spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_streaming.py` & `mosaicml-streaming-0.5.1/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_streaming_remote.py` & `mosaicml-streaming-0.5.1/tests/test_streaming_remote.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_upload.py` & `mosaicml-streaming-0.5.1/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.0/tests/test_writer.py` & `mosaicml-streaming-0.5.1/tests/test_writer.py`

 * *Files identical despite different names*

