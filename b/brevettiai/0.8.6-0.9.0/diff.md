# Comparing `tmp/brevettiai-0.8.6.tar.gz` & `tmp/brevettiai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brevettiai-0.8.6.tar", max compression
+gzip compressed data, was "brevettiai-0.9.0.tar", max compression
```

## Comparing `brevettiai-0.8.6.tar` & `brevettiai-0.9.0.tar`

### file list

```diff
@@ -1,138 +1,139 @@
--rw-r--r--   0        0        0    11358 2023-06-05 11:23:09.518812 brevettiai-0.8.6/LICENSE
--rw-r--r--   0        0        0      678 2023-06-05 11:23:09.518812 brevettiai-0.8.6/README.md
--rw-r--r--   0        0        0      306 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/__init__.py
--rw-r--r--   0        0        0      156 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/__init__.py
--rw-r--r--   0        0        0    21427 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/data_generator.py
--rw-r--r--   0        0        0      374 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/__init__.py
--rw-r--r--   0        0        0       86 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/annotation.py
--rw-r--r--   0        0        0     4805 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/annotation_loader.py
--rw-r--r--   0        0        0    10337 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/annotation_parser.py
--rw-r--r--   0        0        0     1683 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/annotation_pooling.py
--rw-r--r--   0        0        0      872 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/bayer_demosaic.py
--rw-r--r--   0        0        0    14429 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/bcimg_dataset.py
--rw-r--r--   0        0        0    26860 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_augmenter.py
--rw-r--r--   0        0        0    11743 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_loader.py
--rw-r--r--   0        0        0    10337 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_pipeline.py
--rw-r--r--   0        0        0      877 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_processor.py
--rw-r--r--   0        0        0     1271 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_region.py
--rw-r--r--   0        0        0      223 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/modules.py
--rw-r--r--   0        0        0     4612 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/multi_frame_imager.py
--rw-r--r--   0        0        0     4254 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/segmentation_loader.py
--rw-r--r--   0        0        0     3733 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/sequence_loader.py
--rw-r--r--   0        0        0    15180 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/utils.py
--rw-r--r--   0        0        0     1481 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/inspection_info.py
--rw-r--r--   0        0        0    10164 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/sample_integrity.py
--rw-r--r--   0        0        0     9711 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/sample_tools.py
--rw-r--r--   0        0        0     1075 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/serialization.py
--rw-r--r--   0        0        0     1292 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/tf_serialization.py
--rw-r--r--   0        0        0     4617 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/tf_types.py
--rw-r--r--   0        0        0     6422 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/data/tf_utils.py
--rw-r--r--   0        0        0      374 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/__init__.py
--rw-r--r--   0        0        0      348 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/camelmodel.py
--rw-r--r--   0        0        0      987 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/color.py
--rw-r--r--   0        0        0     3243 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/dataset.py
--rw-r--r--   0        0        0     4672 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/image.py
--rw-r--r--   0        0        0     5656 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/image_annotation.py
--rw-r--r--   0        0        0     1140 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/tag.py
--rw-r--r--   0        0        0     7570 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/web_api_types.py
--rw-r--r--   0        0        0     3819 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/examples/explore_application.py
--rw-r--r--   0        0        0      465 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/examples/plot_annotation.py
--rw-r--r--   0        0        0     1439 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/examples/run_experiment.py
--rw-r--r--   0        0        0       71 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/__init__.py
--rw-r--r--   0        0        0     3101 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/aws.py
--rw-r--r--   0        0        0     4862 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/facets_atlas.py
--rw-r--r--   0        0        0     2357 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/git_state.py
--rw-r--r--   0        0        0     2558 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/package_validation.py
--rw-r--r--   0        0        0     3559 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/pivot.py
--rw-r--r--   0        0        0     2268 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/raygun.py
--rw-r--r--   0        0        0     2311 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/remote_monitor.py
--rw-r--r--   0        0        0     1783 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/sagemaker.py
--rw-r--r--   0        0        0    21985 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/vue_schema_utils.py
--rw-r--r--   0        0        0      451 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/__init__.py
--rw-r--r--   0        0        0    15551 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/cloudpath.py
--rw-r--r--   0        0        0     1344 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/credentials.py
--rw-r--r--   0        0        0     4160 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/file_cache.py
--rw-r--r--   0        0        0     2071 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/files.py
--rw-r--r--   0        0        0      743 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/h5_metadata.py
--rw-r--r--   0        0        0     4677 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/local_io.py
--rw-r--r--   0        0        0     8813 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/minio_io.py
--rw-r--r--   0        0        0     4923 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/onnx.py
--rw-r--r--   0        0        0     2325 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/path.py
--rw-r--r--   0        0        0     1184 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/serialization.py
--rw-r--r--   0        0        0     2790 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/smart_open_patch.py
--rw-r--r--   0        0        0     3577 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/tf_recorder.py
--rw-r--r--   0        0        0     1365 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/url_io.py
--rw-r--r--   0        0        0     6825 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/utils.py
--rw-r--r--   0        0        0        0 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/ml/__init__.py
--rw-r--r--   0        0        0       47 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/ml/tensorflow/__init__.py
--rw-r--r--   0        0        0     5839 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/ml/tensorflow/annotation_loader.py
--rw-r--r--   0        0        0      111 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/model/__init__.py
--rw-r--r--   0        0        0     2692 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/model/catalogue.py
--rw-r--r--   0        0        0      534 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/model/factory/__init__.py
--rw-r--r--   0        0        0     2191 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/lenet_backbone.py
--rw-r--r--   0        0        0     8746 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/lraspp.py
--rw-r--r--   0        0        0     3690 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/mobilenetv2_backbone.py
--rw-r--r--   0        0        0     2652 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/segmentation.py
--rw-r--r--   0        0        0     2510 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/unet.py
--rw-r--r--   0        0        0     2972 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/losses.py
--rw-r--r--   0        0        0      137 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/__init__.py
--rw-r--r--   0        0        0     1465 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/history.py
--rw-r--r--   0        0        0     2805 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/image_segmentation.py
--rw-r--r--   0        0        0      538 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/inference.py
--rw-r--r--   0        0        0     2903 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/metadata.py
--rw-r--r--   0        0        0      346 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/__init__.py
--rw-r--r--   0        0        0     8568 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/aipackage.py
--rw-r--r--   0        0        0     2758 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/annotations.py
--rw-r--r--   0        0        0     1274 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/dataset.py
--rw-r--r--   0        0        0     8145 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/model_archive.py
--rw-r--r--   0        0        0      368 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/__init__.py
--rw-r--r--   0        0        0    21202 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/annotation.py
--rw-r--r--   0        0        0    12476 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/dataset.py
--rw-r--r--   0        0        0      370 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/iomodel.py
--rw-r--r--   0        0        0    21112 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/job.py
--rw-r--r--   0        0        0     5142 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/platform_backend.py
--rw-r--r--   0        0        0     3720 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/platform_credentials.py
--rw-r--r--   0        0        0    29359 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/web_api.py
--rw-r--r--   0        0        0   150582 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/bin/0_1543413266626.bmp
--rw-r--r--   0        0        0     6796 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/bin/1651574629796.json
--rw-r--r--   0        0        0      249 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/get_resources.py
--rw-r--r--   0        0        0     1767 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/test_aipackage.py
--rw-r--r--   0        0        0     5045 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/test_annotation_loader.py
--rw-r--r--   0        0        0     5858 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/test_annotation_tooling.py
--rw-r--r--   0        0        0    15003 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_data.py
--rw-r--r--   0        0        0     5048 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_data_image.py
--rw-r--r--   0        0        0      882 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_data_manipulation.py
--rw-r--r--   0        0        0     3923 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_image_loader.py
--rw-r--r--   0        0        0     1329 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_model_archive.py
--rw-r--r--   0        0        0      577 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_model_catalogue.py
--rw-r--r--   0        0        0     1139 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_model_loss.py
--rw-r--r--   0        0        0     3500 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_model_metadata.py
--rw-r--r--   0        0        0     1574 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_pivot.py
--rw-r--r--   0        0        0     1249 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_platform_annotation.py
--rw-r--r--   0        0        0     1263 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_platform_job.py
--rw-r--r--   0        0        0     3732 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_polygon_extraction.py
--rw-r--r--   0        0        0     1795 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_schema.py
--rw-r--r--   0        0        0     1200 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_tags.py
--rw-r--r--   0        0        0      667 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_web_api.py
--rw-r--r--   0        0        0        0 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tooling/__init__.py
--rw-r--r--   0        0        0     5288 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tooling/annotation_tools.py
--rw-r--r--   0        0        0     7247 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tooling/experiments.py
--rw-r--r--   0        0        0     1633 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tooling/plot.py
--rw-r--r--   0        0        0       67 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/__init__.py
--rw-r--r--   0        0        0     1117 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/argparse_utils.py
--rw-r--r--   0        0        0      614 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/dict_utils.py
--rw-r--r--   0        0        0      536 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/env_variables.py
--rw-r--r--   0        0        0     2651 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/model_version.py
--rw-r--r--   0        0        0     2589 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/module.py
--rw-r--r--   0        0        0      292 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/numpy_json_encoder.py
--rw-r--r--   0        0        0     5823 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/onnx_benchmark.py
--rw-r--r--   0        0        0     1491 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/pandas_utils.py
--rw-r--r--   0        0        0      850 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/polygon_utils.py
--rw-r--r--   0        0        0     1707 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/profiling.py
--rw-r--r--   0        0        0      433 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/singleton.py
--rw-r--r--   0        0        0     5961 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/tensorboard_collector.py
--rw-r--r--   0        0        0     3914 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/tf_serving_request.py
--rw-r--r--   0        0        0     4171 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/upload_data.py
--rw-r--r--   0        0        0      843 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/validate_args.py
--rw-r--r--   0        0        0     2372 2023-06-05 11:23:09.534812 brevettiai-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     2903 1970-01-01 00:00:00.000000 brevettiai-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-19 06:56:11.016377 brevettiai-0.9.0/LICENSE
+-rw-r--r--   0        0        0      678 2023-06-19 06:56:11.016377 brevettiai-0.9.0/README.md
+-rw-r--r--   0        0        0      306 2023-06-19 06:56:11.016377 brevettiai-0.9.0/brevettiai/__init__.py
+-rw-r--r--   0        0        0      156 2023-06-19 06:56:11.016377 brevettiai-0.9.0/brevettiai/data/__init__.py
+-rw-r--r--   0        0        0    21606 2023-06-19 06:56:11.016377 brevettiai-0.9.0/brevettiai/data/data_generator.py
+-rw-r--r--   0        0        0      374 2023-06-19 06:56:11.016377 brevettiai-0.9.0/brevettiai/data/image/__init__.py
+-rw-r--r--   0        0        0       86 2023-06-19 06:56:11.016377 brevettiai-0.9.0/brevettiai/data/image/annotation.py
+-rw-r--r--   0        0        0     4805 2023-06-19 06:56:11.016377 brevettiai-0.9.0/brevettiai/data/image/annotation_loader.py
+-rw-r--r--   0        0        0    10337 2023-06-19 06:56:11.016377 brevettiai-0.9.0/brevettiai/data/image/annotation_parser.py
+-rw-r--r--   0        0        0     1683 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/annotation_pooling.py
+-rw-r--r--   0        0        0      872 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/bayer_demosaic.py
+-rw-r--r--   0        0        0    14429 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/bcimg_dataset.py
+-rw-r--r--   0        0        0    26860 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/image_augmenter.py
+-rw-r--r--   0        0        0    11743 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/image_loader.py
+-rw-r--r--   0        0        0    10337 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/image_pipeline.py
+-rw-r--r--   0        0        0      877 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/image_processor.py
+-rw-r--r--   0        0        0     1271 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/image_region.py
+-rw-r--r--   0        0        0      223 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/modules.py
+-rw-r--r--   0        0        0     4612 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/multi_frame_imager.py
+-rw-r--r--   0        0        0     4254 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/segmentation_loader.py
+-rw-r--r--   0        0        0     5511 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/sequence_loader.py
+-rw-r--r--   0        0        0    15180 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/image/utils.py
+-rw-r--r--   0        0        0     1481 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/inspection_info.py
+-rw-r--r--   0        0        0    10164 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/sample_integrity.py
+-rw-r--r--   0        0        0     9711 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/sample_tools.py
+-rw-r--r--   0        0        0     1075 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/serialization.py
+-rw-r--r--   0        0        0     1292 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/tf_serialization.py
+-rw-r--r--   0        0        0     4617 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/tf_types.py
+-rw-r--r--   0        0        0     6422 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/data/tf_utils.py
+-rw-r--r--   0        0        0      423 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/datamodel/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/datamodel/camelmodel.py
+-rw-r--r--   0        0        0      987 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/datamodel/color.py
+-rw-r--r--   0        0        0     4069 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/datamodel/dataset.py
+-rw-r--r--   0        0        0     4672 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/datamodel/image.py
+-rw-r--r--   0        0        0     5656 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/datamodel/image_annotation.py
+-rw-r--r--   0        0        0     1140 2023-06-19 06:56:11.020377 brevettiai-0.9.0/brevettiai/datamodel/tag.py
+-rw-r--r--   0        0        0     7570 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/datamodel/web_api_types.py
+-rw-r--r--   0        0        0     3819 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/examples/explore_application.py
+-rw-r--r--   0        0        0      465 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/examples/plot_annotation.py
+-rw-r--r--   0        0        0     1439 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/examples/run_experiment.py
+-rw-r--r--   0        0        0       71 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/__init__.py
+-rw-r--r--   0        0        0     3101 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/aws.py
+-rw-r--r--   0        0        0     4862 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/facets_atlas.py
+-rw-r--r--   0        0        0     2357 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/git_state.py
+-rw-r--r--   0        0        0     2558 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/package_validation.py
+-rw-r--r--   0        0        0     3559 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/pivot.py
+-rw-r--r--   0        0        0     2268 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/raygun.py
+-rw-r--r--   0        0        0     2311 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/remote_monitor.py
+-rw-r--r--   0        0        0     1783 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/sagemaker.py
+-rw-r--r--   0        0        0    21985 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/interfaces/vue_schema_utils.py
+-rw-r--r--   0        0        0      451 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/__init__.py
+-rw-r--r--   0        0        0    15551 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/cloudpath.py
+-rw-r--r--   0        0        0     1344 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/credentials.py
+-rw-r--r--   0        0        0     4160 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/file_cache.py
+-rw-r--r--   0        0        0     2071 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/files.py
+-rw-r--r--   0        0        0      743 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/h5_metadata.py
+-rw-r--r--   0        0        0     4677 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/local_io.py
+-rw-r--r--   0        0        0     8813 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/minio_io.py
+-rw-r--r--   0        0        0     4923 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/onnx.py
+-rw-r--r--   0        0        0     2325 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/path.py
+-rw-r--r--   0        0        0     1184 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/serialization.py
+-rw-r--r--   0        0        0     2790 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/smart_open_patch.py
+-rw-r--r--   0        0        0     3577 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/tf_recorder.py
+-rw-r--r--   0        0        0     1365 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/url_io.py
+-rw-r--r--   0        0        0     6825 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/io/utils.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/ml/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/ml/tensorflow/__init__.py
+-rw-r--r--   0        0        0     5839 2023-06-19 06:56:11.024376 brevettiai-0.9.0/brevettiai/ml/tensorflow/annotation_loader.py
+-rw-r--r--   0        0        0      111 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/__init__.py
+-rw-r--r--   0        0        0     2692 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/catalogue.py
+-rw-r--r--   0        0        0      534 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/factory/__init__.py
+-rw-r--r--   0        0        0     2191 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/factory/lenet_backbone.py
+-rw-r--r--   0        0        0     8746 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/factory/lraspp.py
+-rw-r--r--   0        0        0     3690 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/factory/mobilenetv2_backbone.py
+-rw-r--r--   0        0        0     2652 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/factory/segmentation.py
+-rw-r--r--   0        0        0     2510 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/factory/unet.py
+-rw-r--r--   0        0        0     2972 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/losses.py
+-rw-r--r--   0        0        0      137 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/metadata/__init__.py
+-rw-r--r--   0        0        0     1465 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/metadata/history.py
+-rw-r--r--   0        0        0     2805 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/metadata/image_segmentation.py
+-rw-r--r--   0        0        0      538 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/metadata/inference.py
+-rw-r--r--   0        0        0     2903 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/model/metadata/metadata.py
+-rw-r--r--   0        0        0      346 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/__init__.py
+-rw-r--r--   0        0        0     8568 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/aipackage.py
+-rw-r--r--   0        0        0     2758 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/annotations.py
+-rw-r--r--   0        0        0     1274 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/dataset.py
+-rw-r--r--   0        0        0     3231 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/dataset_items.py
+-rw-r--r--   0        0        0     8145 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/model_archive.py
+-rw-r--r--   0        0        0      368 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/models/__init__.py
+-rw-r--r--   0        0        0    21202 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/models/annotation.py
+-rw-r--r--   0        0        0    12476 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/models/dataset.py
+-rw-r--r--   0        0        0      370 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/models/iomodel.py
+-rw-r--r--   0        0        0    21112 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/models/job.py
+-rw-r--r--   0        0        0     5142 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/models/platform_backend.py
+-rw-r--r--   0        0        0     3720 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/platform_credentials.py
+-rw-r--r--   0        0        0    30107 2023-06-19 06:56:11.028377 brevettiai-0.9.0/brevettiai/platform/web_api.py
+-rw-r--r--   0        0        0   150582 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/bin/0_1543413266626.bmp
+-rw-r--r--   0        0        0     6796 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/bin/1651574629796.json
+-rw-r--r--   0        0        0      249 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/get_resources.py
+-rw-r--r--   0        0        0     1767 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_aipackage.py
+-rw-r--r--   0        0        0     5045 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_annotation_loader.py
+-rw-r--r--   0        0        0     5858 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_annotation_tooling.py
+-rw-r--r--   0        0        0    15003 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_data.py
+-rw-r--r--   0        0        0     5048 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_data_image.py
+-rw-r--r--   0        0        0      882 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_data_manipulation.py
+-rw-r--r--   0        0        0     3923 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_image_loader.py
+-rw-r--r--   0        0        0     1329 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_model_archive.py
+-rw-r--r--   0        0        0      577 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_model_catalogue.py
+-rw-r--r--   0        0        0     1139 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_model_loss.py
+-rw-r--r--   0        0        0     3500 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_model_metadata.py
+-rw-r--r--   0        0        0     1574 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_pivot.py
+-rw-r--r--   0        0        0     1249 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_platform_annotation.py
+-rw-r--r--   0        0        0     1263 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_platform_job.py
+-rw-r--r--   0        0        0     3732 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_polygon_extraction.py
+-rw-r--r--   0        0        0     1795 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_schema.py
+-rw-r--r--   0        0        0     1200 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_tags.py
+-rw-r--r--   0        0        0      667 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tests/test_web_api.py
+-rw-r--r--   0        0        0        0 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tooling/__init__.py
+-rw-r--r--   0        0        0     5288 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tooling/annotation_tools.py
+-rw-r--r--   0        0        0     7247 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tooling/experiments.py
+-rw-r--r--   0        0        0     1633 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/tooling/plot.py
+-rw-r--r--   0        0        0       67 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/utils/__init__.py
+-rw-r--r--   0        0        0     1117 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/utils/argparse_utils.py
+-rw-r--r--   0        0        0      614 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/utils/dict_utils.py
+-rw-r--r--   0        0        0      536 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/utils/env_variables.py
+-rw-r--r--   0        0        0     2651 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/utils/model_version.py
+-rw-r--r--   0        0        0     2589 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/utils/module.py
+-rw-r--r--   0        0        0      292 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/utils/numpy_json_encoder.py
+-rw-r--r--   0        0        0     5823 2023-06-19 06:56:11.032377 brevettiai-0.9.0/brevettiai/utils/onnx_benchmark.py
+-rw-r--r--   0        0        0     1491 2023-06-19 06:56:11.036377 brevettiai-0.9.0/brevettiai/utils/pandas_utils.py
+-rw-r--r--   0        0        0      850 2023-06-19 06:56:11.036377 brevettiai-0.9.0/brevettiai/utils/polygon_utils.py
+-rw-r--r--   0        0        0     1707 2023-06-19 06:56:11.036377 brevettiai-0.9.0/brevettiai/utils/profiling.py
+-rw-r--r--   0        0        0      433 2023-06-19 06:56:11.036377 brevettiai-0.9.0/brevettiai/utils/singleton.py
+-rw-r--r--   0        0        0     5961 2023-06-19 06:56:11.036377 brevettiai-0.9.0/brevettiai/utils/tensorboard_collector.py
+-rw-r--r--   0        0        0     3914 2023-06-19 06:56:11.036377 brevettiai-0.9.0/brevettiai/utils/tf_serving_request.py
+-rw-r--r--   0        0        0     4171 2023-06-19 06:56:11.036377 brevettiai-0.9.0/brevettiai/utils/upload_data.py
+-rw-r--r--   0        0        0      843 2023-06-19 06:56:11.036377 brevettiai-0.9.0/brevettiai/utils/validate_args.py
+-rw-r--r--   0        0        0     2372 2023-06-19 06:56:11.036377 brevettiai-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2903 1970-01-01 00:00:00.000000 brevettiai-0.9.0/PKG-INFO
```

### Comparing `brevettiai-0.8.6/LICENSE` & `brevettiai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/README.md` & `brevettiai-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/data_generator.py` & `brevettiai-0.9.0/brevettiai/data/data_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,35 +73,38 @@
 
 
 def item_mapping(df):
     mapping = {}
     for name in df.columns:
         col = df[name]
         mapping_name = f"_{name}_mapping"
-        if col.dtype.name == "category":
-            df.loc[:, mapping_name] = col.cat.codes
-            lookup_tbl = tf.ragged.constant(col.cat.categories.values, name=f"{name}lookup")
-            mapping[mapping_name] = name, lambda x, tbl=lookup_tbl: tbl[tf.cast(x, tf.int32)]
-        if col.apply(pd.api.types.is_list_like).any():
-            if col.apply(pd.api.types.is_hashable).all():
-                grp = df.groupby(name)
-                df.loc[:, mapping_name] = grp.ngroup()
-                try:
-                    lookup_tbl = tf.ragged.constant([k for k, v in grp], name=f"{name}lookup")
-                except ValueError:
-                    lookup_tbl = tf.ragged.constant([tuple(k) for k, v in grp], name=f"{name}lookup")
+        try:
+            if col.dtype.name == "category":
+                df.loc[:, mapping_name] = col.cat.codes
+                lookup_tbl = tf.ragged.constant(col.cat.categories.values, name=f"{name}lookup")
+                mapping[mapping_name] = name, lambda x, tbl=lookup_tbl: tbl[tf.cast(x, tf.int32)]
+            if col.apply(pd.api.types.is_list_like).any():
+                if col.apply(pd.api.types.is_hashable).all():
+                    grp = df.groupby(name)
+                    df.loc[:, mapping_name] = grp.ngroup()
+                    try:
+                        lookup_tbl = tf.ragged.constant([k for k, v in grp], name=f"{name}lookup")
+                    except ValueError:
+                        lookup_tbl = tf.ragged.constant([tuple(k) for k, v in grp], name=f"{name}lookup")
+                else:
+                    df.loc[:, mapping_name] = np.arange(col.size)
+                    try:
+                        lookup_tbl = tf.constant(col.values.tolist())
+                    except ValueError:
+                        lookup_tbl = tf.ragged.constant(col.values.tolist())
+                mapping[mapping_name] = name, lambda x, tbl=lookup_tbl: tbl[tf.cast(x, tf.int32)]
             else:
-                df.loc[:, mapping_name] = np.arange(col.size)
-                try:
-                    lookup_tbl = tf.constant(col.values.tolist())
-                except ValueError:
-                    lookup_tbl = tf.ragged.constant(col.values.tolist())
-            mapping[mapping_name] = name, lambda x, tbl=lookup_tbl: tbl[tf.cast(x, tf.int32)]
-        else:
-            mapping[name] = name, lambda x: x
+                mapping[name] = name, lambda x: x
+        except ValueError:
+            log.warning(f"Cannot map column '{name}'")
 
     return df[mapping.keys()], mapping
 
 
 def _downcast(s):
     if is_signed_integer_dtype(s.dtype):
         return pd.to_numeric(s, downcast="integer")
```

### Comparing `brevettiai-0.8.6/brevettiai/data/image/annotation_loader.py` & `brevettiai-0.9.0/brevettiai/data/image/annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/annotation_parser.py` & `brevettiai-0.9.0/brevettiai/data/image/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/annotation_pooling.py` & `brevettiai-0.9.0/brevettiai/data/image/annotation_pooling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/bayer_demosaic.py` & `brevettiai-0.9.0/brevettiai/data/image/bayer_demosaic.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/bcimg_dataset.py` & `brevettiai-0.9.0/brevettiai/data/image/bcimg_dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/image_augmenter.py` & `brevettiai-0.9.0/brevettiai/data/image/image_augmenter.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/image_loader.py` & `brevettiai-0.9.0/brevettiai/data/image/image_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/image_pipeline.py` & `brevettiai-0.9.0/brevettiai/data/image/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/image_processor.py` & `brevettiai-0.9.0/brevettiai/data/image/image_processor.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/image_region.py` & `brevettiai-0.9.0/brevettiai/data/image/image_region.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/multi_frame_imager.py` & `brevettiai-0.9.0/brevettiai/data/image/multi_frame_imager.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/segmentation_loader.py` & `brevettiai-0.9.0/brevettiai/data/image/segmentation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/image/sequence_loader.py` & `brevettiai-0.9.0/brevettiai/data/image/sequence_loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,54 @@
 from brevettiai.io import AnyPath
 from brevettiai.data.image.image_loader import ImageLoader, ImageKeys
 from brevettiai.data.tf_types import TfRange, BBOX, SequenceShape
 
 log = logging.getLogger(__name__)
 
 
+class SequenceLoaderV2(ImageLoader):
+    type: Literal["BcimgDatasetSequenceLoaderV2"] = "BcimgDatasetSequenceLoaderV2"
+    stack_channels: bool = True
+    path_key: str = Field(default="paths", exclude=True)
+    range_meta: ClassVar[Type] = TfRange
+    shape_meta: ClassVar[Type] = SequenceShape
+    metadata_spec = {
+        "sequence_shape": SequenceShape.build,
+        ImageKeys.BOUNDING_BOX: BBOX.build,
+    }
+
+    def load(self, paths, metadata=None, postprocess=True, **kwargs):
+        shape = metadata["sequence_shape"]
+
+        default_shape = (shape.height, shape.width, shape.channels if self.channels == 0 else self.channels)
+        if metadata is not None:
+            if ImageKeys.BOUNDING_BOX in metadata:
+                default_shape = (*metadata[ImageKeys.BOUNDING_BOX].shape, default_shape[-1])
+
+        if self.postprocessor and postprocess:
+            default_shape = (*self.postprocessor.output_size(default_shape[0], default_shape[1]),
+                             self.postprocessor.output_channels(default_shape[2]))
+
+        images, meta = tf.map_fn(
+            fn=lambda x: super(SequenceLoaderV2, self).load(x, metadata, postprocess=postprocess,
+                                                          default_shape=default_shape),
+            elems=paths if tf.is_tensor(paths) else np.array(paths),
+            fn_output_signature=(tf.float32, {'_image_file_shape': tf.int32}),
+            parallel_iterations=16
+        )
+        if self.stack_channels:
+            images = tf.transpose(images, [1, 2, 0, 3])
+            sh = tf.shape(images)
+            images = tf.reshape(images, [sh[0], sh[1], sh[2] * sh[3]])
+
+        _image_file_shape = meta["_image_file_shape"][0]
+
+        return images, {"_image_file_shape": _image_file_shape}
+
+
 class SequenceLoader(ImageLoader):
     type: Literal["BcimgDatasetSequenceLoader"] = "BcimgDatasetSequenceLoader"
     stack_channels: bool = True
     path_key: str = Field(default="path_format", exclude=True)
     range_meta: ClassVar[Type] = TfRange
     shape_meta: ClassVar[Type] = SequenceShape
     metadata_spec = {
```

### Comparing `brevettiai-0.8.6/brevettiai/data/image/utils.py` & `brevettiai-0.9.0/brevettiai/data/image/utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/inspection_info.py` & `brevettiai-0.9.0/brevettiai/data/inspection_info.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/sample_integrity.py` & `brevettiai-0.9.0/brevettiai/data/sample_integrity.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/sample_tools.py` & `brevettiai-0.9.0/brevettiai/data/sample_tools.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/serialization.py` & `brevettiai-0.9.0/brevettiai/data/serialization.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/tf_serialization.py` & `brevettiai-0.9.0/brevettiai/data/tf_serialization.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/tf_types.py` & `brevettiai-0.9.0/brevettiai/data/tf_types.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/data/tf_utils.py` & `brevettiai-0.9.0/brevettiai/data/tf_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/datamodel/color.py` & `brevettiai-0.9.0/brevettiai/datamodel/color.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/datamodel/dataset.py` & `brevettiai-0.9.0/brevettiai/datamodel/dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pydantic import BaseModel, Field, PrivateAttr
 from uuid import uuid4
-from typing import Optional, List, Union
+from typing import Optional, List, Union, Dict
 from datetime import datetime
 import urllib
 
+from brevettiai.datamodel import CamelModel
 from brevettiai.datamodel.tag import Tag
 from brevettiai.io import AnyPath, get_default_s3_client_manager, S3Path
 
 IMAGE_SUFFIXES = frozenset((".tif", ".bmp", ".jpeg", ".jpg", ".png"))
 
 
 def filter_suffix_in(paths, allowed_suffixes):
@@ -91,7 +92,38 @@
 
         return items
 
     def iter_images(self, path: Optional[str] = None, max_items=None):
         """Utility function for iterating over images in the dataset"""
         return self.iter(after_hidden=True, include_dirs=False,
                          recursive=True, max_items=max_items, file_types=IMAGE_SUFFIXES)
+
+
+class DatasetObject(CamelModel):
+    """
+    object located in a dataset
+    """
+    path: str
+    bici_reference: str = ""
+    dataset_id: Optional[str] = Field(default=None, exclude=True)
+    item: Optional['DatasetItem'] = Field(default=None, exclude=True)
+
+
+class DatasetItemMetadata(CamelModel, extra="allow"):
+    machine: Optional[str]
+    tv: Optional[str]
+    inspection_type: Optional[str]
+    camera_view: Optional[str]
+    category: Optional[str]
+    shape: Optional[Dict[str, int]]
+    run: Optional[int]
+    sample_id: Optional[str]
+
+
+class DatasetItem(CamelModel):
+    dataset_id: str = None
+    item_id: str
+    objects: List[DatasetObject]
+    metadata: DatasetItemMetadata = Field(default_factory=DatasetItemMetadata)
+
+
+DatasetObject.update_forward_refs()
```

### Comparing `brevettiai-0.8.6/brevettiai/datamodel/image.py` & `brevettiai-0.9.0/brevettiai/datamodel/image.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/datamodel/image_annotation.py` & `brevettiai-0.9.0/brevettiai/datamodel/image_annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/datamodel/tag.py` & `brevettiai-0.9.0/brevettiai/datamodel/tag.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/datamodel/web_api_types.py` & `brevettiai-0.9.0/brevettiai/datamodel/web_api_types.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/examples/explore_application.py` & `brevettiai-0.9.0/brevettiai/examples/explore_application.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/examples/run_experiment.py` & `brevettiai-0.9.0/brevettiai/examples/run_experiment.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/aws.py` & `brevettiai-0.9.0/brevettiai/interfaces/aws.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/facets_atlas.py` & `brevettiai-0.9.0/brevettiai/interfaces/facets_atlas.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/git_state.py` & `brevettiai-0.9.0/brevettiai/interfaces/git_state.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/package_validation.py` & `brevettiai-0.9.0/brevettiai/interfaces/package_validation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/pivot.py` & `brevettiai-0.9.0/brevettiai/interfaces/pivot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/raygun.py` & `brevettiai-0.9.0/brevettiai/interfaces/raygun.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/remote_monitor.py` & `brevettiai-0.9.0/brevettiai/interfaces/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/sagemaker.py` & `brevettiai-0.9.0/brevettiai/interfaces/sagemaker.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/interfaces/vue_schema_utils.py` & `brevettiai-0.9.0/brevettiai/interfaces/vue_schema_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/cloudpath.py` & `brevettiai-0.9.0/brevettiai/io/cloudpath.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/credentials.py` & `brevettiai-0.9.0/brevettiai/io/credentials.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/file_cache.py` & `brevettiai-0.9.0/brevettiai/io/file_cache.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/files.py` & `brevettiai-0.9.0/brevettiai/io/files.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/h5_metadata.py` & `brevettiai-0.9.0/brevettiai/io/h5_metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/local_io.py` & `brevettiai-0.9.0/brevettiai/io/local_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/minio_io.py` & `brevettiai-0.9.0/brevettiai/io/minio_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/onnx.py` & `brevettiai-0.9.0/brevettiai/io/onnx.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/path.py` & `brevettiai-0.9.0/brevettiai/io/path.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/serialization.py` & `brevettiai-0.9.0/brevettiai/io/serialization.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/smart_open_patch.py` & `brevettiai-0.9.0/brevettiai/io/smart_open_patch.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/tf_recorder.py` & `brevettiai-0.9.0/brevettiai/io/tf_recorder.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/url_io.py` & `brevettiai-0.9.0/brevettiai/io/url_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/io/utils.py` & `brevettiai-0.9.0/brevettiai/io/utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/ml/tensorflow/annotation_loader.py` & `brevettiai-0.9.0/brevettiai/ml/tensorflow/annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/catalogue.py` & `brevettiai-0.9.0/brevettiai/model/catalogue.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/factory/__init__.py` & `brevettiai-0.9.0/brevettiai/model/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/factory/lenet_backbone.py` & `brevettiai-0.9.0/brevettiai/model/factory/lenet_backbone.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/factory/lraspp.py` & `brevettiai-0.9.0/brevettiai/model/factory/lraspp.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/factory/mobilenetv2_backbone.py` & `brevettiai-0.9.0/brevettiai/model/factory/mobilenetv2_backbone.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/factory/segmentation.py` & `brevettiai-0.9.0/brevettiai/model/factory/segmentation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/factory/unet.py` & `brevettiai-0.9.0/brevettiai/model/factory/unet.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/losses.py` & `brevettiai-0.9.0/brevettiai/model/losses.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/metadata/history.py` & `brevettiai-0.9.0/brevettiai/model/metadata/history.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/metadata/image_segmentation.py` & `brevettiai-0.9.0/brevettiai/model/metadata/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/metadata/inference.py` & `brevettiai-0.9.0/brevettiai/model/metadata/inference.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/model/metadata/metadata.py` & `brevettiai-0.9.0/brevettiai/model/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/aipackage.py` & `brevettiai-0.9.0/brevettiai/platform/aipackage.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/annotations.py` & `brevettiai-0.9.0/brevettiai/platform/annotations.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/dataset.py` & `brevettiai-0.9.0/brevettiai/platform/dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/model_archive.py` & `brevettiai-0.9.0/brevettiai/platform/model_archive.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/models/annotation.py` & `brevettiai-0.9.0/brevettiai/platform/models/annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/models/dataset.py` & `brevettiai-0.9.0/brevettiai/platform/models/dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/models/job.py` & `brevettiai-0.9.0/brevettiai/platform/models/job.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/models/platform_backend.py` & `brevettiai-0.9.0/brevettiai/platform/models/platform_backend.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/platform_credentials.py` & `brevettiai-0.9.0/brevettiai/platform/platform_credentials.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/platform/web_api.py` & `brevettiai-0.9.0/brevettiai/platform/web_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from brevettiai.platform import backend as default_backend
 from brevettiai.platform.platform_credentials import PlatformDatasetCredentials
 from brevettiai.datamodel import Tag
 from brevettiai.datamodel import web_api_types as api
 from brevettiai.datamodel import Dataset
 from brevettiai.utils import env_variables
 from brevettiai.platform import annotations
+from brevettiai.platform.dataset_items import delete_item, get_items, put_item
 
 
 log = logging.getLogger(__name__)
 
 
 class WebApiConfig(BaseModel):
     """
@@ -429,19 +430,30 @@
     def rename_annotation(self, dataset, image_path, annotation_name, new_annotation_name):
         entry = self.get_dataset_annotations(dataset, image_path=image_path)
         annotation = entry.annotation_files[annotation_name]
         self.create_annotation(dataset, image_path, annotation_name=new_annotation_name)
         self.update_annotation(dataset, image_path, annotation_name=new_annotation_name, annotation=annotation)
         self.delete_annotation(dataset, image_path, annotation_name=annotation_name)
 
+    def get_items(self, dataset=None, item_id=None, filter: dict = None, **kwargs):
+        return get_items(host=self.host, get_fn=self._http_get,
+                         dataset=dataset, item_id=item_id, filter=filter, **kwargs)
+
+    def put_item(self, item, **kwargs):
+        return put_item(host=self.host, put_fn=self._http_put, item=item, **kwargs)
+
+    def delete_item(self, dataset_id, item_id, **kwargs):
+        return delete_item(host=self.host, delete_fn=self._http_delete,
+                           dataset_id=dataset_id, item_id=item_id, **kwargs)
+
     def create(self, obj: Union[Dataset, Tag, api.Model, api.Report], **kwargs):
         if isinstance(obj, Dataset):
             payload = obj.dict(include={"name", "reference", "notes", "locked"}, by_alias=True)
             payload["tagIds"] = [tag.id for tag in obj.tags]
-            r = self._http_post(f"{self.host}/api/data/", )
+            r = self._http_post(f"{self.host}/api/data/", json=payload)
             return self.get_dataset(r.json()["datasetId"], **kwargs)
         elif isinstance(obj, Tag):
             payload = obj.dict(include={"name", "parent_id"}, by_alias=True, exclude_none=True)
             self._http_post(f"{self.host}/api/resources/tags/", json=payload)
 
             # TODO: return tag id on api
             parent = self.get_tag(obj.parent_id)
@@ -728,16 +740,18 @@
         :param settings: Settings object or dict for the job
         :param datasets: list of datasets or string names
         :param application: string id or Application object
         :param kwargs: Other args; see tooling.experiments
         :return:
         """
         from brevettiai.tooling.experiments import experiment
-        return experiment(name=name, job_type=job_type, settings=settings or {}, datasets=datasets,
+        experiment = experiment(name=name, job_type=job_type, settings=settings or {}, datasets=datasets,
                               application=application, **kwargs, web=self)
+        print(f"{self.host}/models/{experiment.model.id}")
+        return experiment
 
     def run_test(self, name, job_type, settings, on,
                        datasets: Optional[List] = None, application=None, **kwargs):
         """
         :param name: Name of the experiment
         :param job_type: class of the Job
         :param settings: Settings object or dict for the job
```

### Comparing `brevettiai-0.8.6/brevettiai/tests/bin/0_1543413266626.bmp` & `brevettiai-0.9.0/brevettiai/tests/bin/0_1543413266626.bmp`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/bin/1651574629796.json` & `brevettiai-0.9.0/brevettiai/tests/bin/1651574629796.json`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_aipackage.py` & `brevettiai-0.9.0/brevettiai/tests/test_aipackage.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_annotation_loader.py` & `brevettiai-0.9.0/brevettiai/tests/test_annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_annotation_tooling.py` & `brevettiai-0.9.0/brevettiai/tests/test_annotation_tooling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_data.py` & `brevettiai-0.9.0/brevettiai/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_data_image.py` & `brevettiai-0.9.0/brevettiai/tests/test_data_image.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_data_manipulation.py` & `brevettiai-0.9.0/brevettiai/tests/test_data_manipulation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_image_loader.py` & `brevettiai-0.9.0/brevettiai/tests/test_image_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_model_archive.py` & `brevettiai-0.9.0/brevettiai/tests/test_model_archive.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_model_catalogue.py` & `brevettiai-0.9.0/brevettiai/tests/test_model_catalogue.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_model_loss.py` & `brevettiai-0.9.0/brevettiai/tests/test_model_loss.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_model_metadata.py` & `brevettiai-0.9.0/brevettiai/tests/test_model_metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_pivot.py` & `brevettiai-0.9.0/brevettiai/tests/test_pivot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_platform_annotation.py` & `brevettiai-0.9.0/brevettiai/tests/test_platform_annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_platform_job.py` & `brevettiai-0.9.0/brevettiai/tests/test_platform_job.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_polygon_extraction.py` & `brevettiai-0.9.0/brevettiai/tests/test_polygon_extraction.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_schema.py` & `brevettiai-0.9.0/brevettiai/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_tags.py` & `brevettiai-0.9.0/brevettiai/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tests/test_web_api.py` & `brevettiai-0.9.0/brevettiai/tests/test_web_api.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tooling/annotation_tools.py` & `brevettiai-0.9.0/brevettiai/tooling/annotation_tools.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tooling/experiments.py` & `brevettiai-0.9.0/brevettiai/tooling/experiments.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/tooling/plot.py` & `brevettiai-0.9.0/brevettiai/tooling/plot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/argparse_utils.py` & `brevettiai-0.9.0/brevettiai/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/dict_utils.py` & `brevettiai-0.9.0/brevettiai/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/env_variables.py` & `brevettiai-0.9.0/brevettiai/utils/env_variables.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/model_version.py` & `brevettiai-0.9.0/brevettiai/utils/model_version.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/module.py` & `brevettiai-0.9.0/brevettiai/utils/module.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/onnx_benchmark.py` & `brevettiai-0.9.0/brevettiai/utils/onnx_benchmark.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/pandas_utils.py` & `brevettiai-0.9.0/brevettiai/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/polygon_utils.py` & `brevettiai-0.9.0/brevettiai/utils/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/profiling.py` & `brevettiai-0.9.0/brevettiai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/tensorboard_collector.py` & `brevettiai-0.9.0/brevettiai/utils/tensorboard_collector.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/tf_serving_request.py` & `brevettiai-0.9.0/brevettiai/utils/tf_serving_request.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/upload_data.py` & `brevettiai-0.9.0/brevettiai/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/brevettiai/utils/validate_args.py` & `brevettiai-0.9.0/brevettiai/utils/validate_args.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.6/pyproject.toml` & `brevettiai-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brevettiai"
-version = "0.8.6"
+version = "0.9.0"
 readme = "README.md"
 homepage = "https://platform.brevetti.ai"
 documentation = "https://docs.brevetti.ai/"
 repository = "https://bitbucket.org/criterionai/core.git"
 description = "Brevetti AI library"
 license = "Apache-2.0"
 authors = ["Emil Tyge <emil@brevetti.ai>"]
```

### Comparing `brevettiai-0.8.6/PKG-INFO` & `brevettiai-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brevettiai
-Version: 0.8.6
+Version: 0.9.0
 Summary: Brevetti AI library
 Home-page: https://platform.brevetti.ai
 License: Apache-2.0
 Author: Emil Tyge
 Author-email: emil@brevetti.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

