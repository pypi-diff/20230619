# Comparing `tmp/tator-1.0.4.tar.gz` & `tmp/tator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tator-1.0.4.tar", last modified: Tue Jun  6 02:58:53 2023, max compression
+gzip compressed data, was "tator-1.0.5.tar", last modified: Mon Jun 19 16:04:04 2023, max compression
```

## Comparing `tator-1.0.4.tar` & `tator-1.0.5.tar`

### file list

```diff
@@ -1,292 +1,292 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.215602 tator-1.0.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-06-06 02:47:33.000000 tator-1.0.4/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-06-06 02:58:53.215602 tator-1.0.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2023-06-06 02:47:33.000000 tator-1.0.4/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-06-06 02:47:33.000000 tator-1.0.4/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-06 02:58:53.215602 tator-1.0.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-06-06 02:47:33.000000 tator-1.0.4/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-06-06 02:47:33.000000 tator-1.0.4/tator/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/extractor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:47:33.000000 tator-1.0.4/tator/extractor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2023-06-06 02:47:33.000000 tator-1.0.4/tator/extractor/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2023-06-06 02:47:33.000000 tator-1.0.4/tator/extractor/env_launcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12295 2023-06-06 02:47:33.000000 tator-1.0.4/tator/extractor/extractor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/openapi/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-06-06 02:47:33.000000 tator-1.0.4/tator/openapi/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/openapi/tator_openapi/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12710 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator/openapi/tator_openapi/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/api/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1854040 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/api/tator_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/api_client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.199602 tator-1.0.4/tator/openapi/tator_openapi/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12120 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8163 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/affiliation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/affiliation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/affiliation_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_manifest.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_parameter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4152 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/analysis.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/analysis_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/announcement.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/applet.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/applet_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/archive_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11001 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_filter_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12663 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_operation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14079 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2023-06-06 02:58:48.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/audio_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4042 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/autocomplete_service.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bad_request_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bookmark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bookmark_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bookmark_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_gcp_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_oci_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_s3_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/bucket_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/change_log.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/change_log_description_of_change.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5302 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/clone_media_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/color_map.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/concat_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/create_list_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/create_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/credentials.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/download_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/download_info_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/email_attachment_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/email_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9514 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/encode_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/favorite.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/favorite_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/favorite_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/feed_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/file_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/fill.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/float_array_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/generic_file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/generic_file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/get_cloned_media_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/image_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/invitation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/invitation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/invitation_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job_cluster.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job_cluster_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job_node.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4849 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/job_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_suggestion.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/leaf_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/live_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/live_update_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_bulk_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9386 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/localization_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18245 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_files.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_next.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_prev.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14774 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_stats.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/media_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/membership.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/membership_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/membership_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/message_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/multi_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/not_found_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/notify_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/organization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/organization_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/organization_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/password_reset_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/project.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/project_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/project_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/resolution_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/s3_storage_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7613 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/section.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6657 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/section_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/section_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_bulk_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10960 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_merge_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_trim_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/state_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/temporary_file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/temporary_file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/token.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/transcode.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10545 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/transcode_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/upload_completion_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/upload_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/upload_part.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/user.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/user_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7852 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/user_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/version_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/version_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/video_clip.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9722 2023-06-06 02:58:49.000000 tator-1.0.4/tator/openapi/tator_openapi/models/video_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13486 2023-06-06 02:58:51.000000 tator-1.0.4/tator/openapi/tator_openapi/rest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.203601 tator-1.0.4/tator/transcode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6547 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/black.mp4
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/create_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/delete_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9425 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/determine_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/make_fragment_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5938 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/make_thumbnails.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/prepare.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19001 2023-06-06 02:47:33.000000 tator-1.0.4/tator/transcode/transcode.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.207602 tator-1.0.4/tator/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/_download_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7168 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/_upload_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/chunked_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/chunked_file_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4470 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_leaf_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7441 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_localization_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11100 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_media_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_membership.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_section.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6560 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_state_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/clone_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4489 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/concat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/download_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/download_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/download_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/find_single_change.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/full_state_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/get_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/get_images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2219 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/get_paginator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      508 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/get_parser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/import_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1729 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/live_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/md5sum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/media_manipulation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17897 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/media_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7283 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/multi_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/register_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/register_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/tator-symbol.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/to_dataframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/update_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/upload_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3315 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/upload_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2023-06-06 02:47:33.000000 tator-1.0.4/tator/util/upload_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-06-06 02:47:33.000000 tator-1.0.4/tator/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.175601 tator-1.0.4/tator.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11773 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-06 02:58:53.000000 tator-1.0.4/tator.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 02:58:53.215602 tator-1.0.4/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4863 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_a_float_array.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_algorithm_launch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_archive_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8615 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attribute_type_addition.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attribute_type_deletion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attribute_type_mutation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_attributes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23749 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_change_log.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7204 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_membership.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_section.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_clone_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_collection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_download_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12346 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_file_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_get_clip.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_getframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_import_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_job_cancel.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_job_cluster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_leaf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2996 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_local_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9199 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_localization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_localization_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6973 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_poly.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_project_thumbnail.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9638 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_state_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_stategraphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_tracks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5487 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_util_media_manipulation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_util_media_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2023-06-06 02:47:33.000000 tator-1.0.4/test/test_version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.314694 tator-1.0.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-06-19 15:53:28.000000 tator-1.0.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-06-19 16:04:04.314694 tator-1.0.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2023-06-19 15:53:28.000000 tator-1.0.5/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-06-19 15:53:28.000000 tator-1.0.5/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-19 16:04:04.314694 tator-1.0.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-06-19 15:53:28.000000 tator-1.0.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.274693 tator-1.0.5/tator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-06-19 15:53:28.000000 tator-1.0.5/tator/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.274693 tator-1.0.5/tator/extractor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:53:28.000000 tator-1.0.5/tator/extractor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2023-06-19 15:53:28.000000 tator-1.0.5/tator/extractor/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2023-06-19 15:53:28.000000 tator-1.0.5/tator/extractor/env_launcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12295 2023-06-19 15:53:28.000000 tator-1.0.5/tator/extractor/extractor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.274693 tator-1.0.5/tator/openapi/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-06-19 15:53:28.000000 tator-1.0.5/tator/openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.278693 tator-1.0.5/tator/openapi/tator_openapi/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12710 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.278693 tator-1.0.5/tator/openapi/tator_openapi/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1854040 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/api/tator_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/api_client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.298693 tator-1.0.5/tator/openapi/tator_openapi/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12120 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8163 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/affiliation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/affiliation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/affiliation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_manifest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_parameter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4152 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/analysis.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/analysis_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/announcement.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/applet.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/applet_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/archive_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11001 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_filter_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12663 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_operation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14079 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/audio_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4042 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/autocomplete_service.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bad_request_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bookmark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bookmark_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bookmark_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_gcp_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_oci_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_s3_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/change_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/change_log_description_of_change.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5302 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/clone_media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/color_map.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/concat_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/create_list_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/create_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/credentials.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/download_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/download_info_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/email_attachment_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/email_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9514 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/encode_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/favorite.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/favorite_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/favorite_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/feed_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/fill.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/float_array_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/generic_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/generic_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/get_cloned_media_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/image_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/invitation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/invitation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/invitation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job_cluster.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job_cluster_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job_node.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4849 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_suggestion.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/live_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/live_update_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10180 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18245 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_files.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_next.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_prev.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14774 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_stats.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/membership.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/membership_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/membership_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/message_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/multi_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/not_found_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/notify_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/organization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/organization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/organization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/password_reset_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/project.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/project_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/project_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/resolution_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/s3_storage_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7613 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/section.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6657 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/section_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/section_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10960 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_merge_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_trim_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/temporary_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/temporary_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/token.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/transcode.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10545 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/transcode_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/upload_completion_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/upload_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/upload_part.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/user_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7852 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/user_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/version_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/version_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/video_clip.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9722 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/video_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13486 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/rest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.302693 tator-1.0.5/tator/transcode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6547 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/black.mp4
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/create_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/delete_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9425 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/determine_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/make_fragment_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5938 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/make_thumbnails.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/prepare.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19001 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/transcode.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.306693 tator-1.0.5/tator/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/_download_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7168 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/_upload_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/chunked_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/chunked_file_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4470 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_leaf_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7441 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_localization_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11100 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_media_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6560 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_state_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4489 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/concat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/download_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/download_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/find_single_change.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/full_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/get_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/get_images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2219 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/get_paginator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      508 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/get_parser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1729 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/live_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/md5sum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17897 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7283 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/multi_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/register_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/register_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/tator-symbol.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/to_dataframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/update_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/upload_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3315 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/upload_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/upload_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-06-19 15:53:28.000000 tator-1.0.5/tator/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.274693 tator-1.0.5/tator.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11773 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.314694 tator-1.0.5/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4863 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_a_float_array.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_algorithm_launch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_archive_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8615 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attribute_type_addition.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attribute_type_deletion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attribute_type_mutation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attributes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23749 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_change_log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7204 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_collection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12346 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_file_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_get_clip.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_getframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_job_cancel.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_job_cluster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_leaf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2996 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_local_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9199 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_localization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_localization_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6973 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_poly.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_project_thumbnail.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9638 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_stategraphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_tracks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5487 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_util_media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_util_media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_version.py
```

### Comparing `tator-1.0.4/README.md` & `tator-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/setup.py` & `tator-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/__init__.py` & `tator-1.0.5/tator/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/extractor/__main__.py` & `tator-1.0.5/tator/extractor/__main__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/extractor/env_launcher.py` & `tator-1.0.5/tator/extractor/env_launcher.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/extractor/extractor.py` & `tator-1.0.5/tator/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/__init__.py` & `tator-1.0.5/tator/openapi/tator_openapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 # import apis into sdk package
 from tator.openapi.tator_openapi.api.tator_api import TatorApi
 
 # import ApiClient
 from tator.openapi.tator_openapi.api_client import ApiClient
 from tator.openapi.tator_openapi.configuration import Configuration
```

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/api/tator_api.py` & `tator-1.0.5/tator/openapi/tator_openapi/api/tator_api.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/api_client.py` & `tator-1.0.5/tator/openapi/tator_openapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.4/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.5/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/configuration.py` & `tator-1.0.5/tator/openapi/tator_openapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 1.0.4".\
+               "SDK Package Version: 1.0.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/exceptions.py` & `tator-1.0.5/tator/openapi/tator_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/__init__.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/affiliation.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/affiliation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/affiliation_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/affiliation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/affiliation_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/affiliation_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_manifest.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_manifest.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_parameter.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_parameter.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/algorithm_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/analysis.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/analysis.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/analysis_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/analysis_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/announcement.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/announcement.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/applet.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/applet_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/applet_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/archive_config.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/archive_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_combinator_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_combinator_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_filter_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_filter_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_operation_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_operation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_delete.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/audio_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/audio_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/autocomplete_service.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/autocomplete_service.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/auxiliary_file_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/auxiliary_file_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bad_request_response.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bad_request_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bookmark.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bookmark_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bookmark_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bookmark_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bookmark_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bucket.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bucket.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_gcp_config.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_gcp_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_oci_config.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_oci_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_oci_native_config.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_oci_native_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_s3_config.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_s3_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/bucket_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/change_log.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/change_log.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/change_log_description_of_change.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/change_log_description_of_change.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/clone_media_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/clone_media_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/color_map.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/color_map.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/concat_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/concat_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/create_list_response.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/create_list_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/create_response.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/create_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/credentials.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/credentials.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/download_info.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/download_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/download_info_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/download_info_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/email_attachment_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/email_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/email_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/email_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/encode_config.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/encode_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/favorite.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/favorite.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/favorite_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/favorite_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/favorite_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/favorite_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/feed_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/feed_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/file.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/file_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/file_type.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/file_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/file_type_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/file_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/file_type_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/file_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/file_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/file_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/fill.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/fill.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/float_array_query.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/float_array_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/generic_file.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/generic_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/generic_file_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/generic_file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/get_cloned_media_response.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/get_cloned_media_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/image_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/image_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/invitation.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/invitation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/invitation_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/invitation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/invitation_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/invitation_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/job.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/job.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/job_cluster.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/job_cluster.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/job_cluster_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/job_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/job_node.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/job_node.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/job_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/job_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_bulk_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_id_query.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_suggestion.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_suggestion.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_type_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/leaf_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/live_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/live_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/live_update_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/live_update_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_bulk_delete.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_bulk_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_bulk_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,43 +31,46 @@
     """
     openapi_types = {
         'attributes': 'dict(str, object)',
         'float_array': 'list[FloatArrayQuery]',
         'ids': 'list[int]',
         'media_ids': 'list[int]',
         'media_query': 'str',
+        'new_elemental_id': 'str',
         'new_version': 'int',
         'object_search': 'AttributeOperationSpec',
         'state_ids': 'list[int]',
         'user_elemental_id': 'str'
     }
 
     attribute_map = {
         'attributes': 'attributes',
         'float_array': 'float_array',
         'ids': 'ids',
         'media_ids': 'media_ids',
         'media_query': 'media_query',
+        'new_elemental_id': 'new_elemental_id',
         'new_version': 'new_version',
         'object_search': 'object_search',
         'state_ids': 'state_ids',
         'user_elemental_id': 'user_elemental_id'
     }
 
-    def __init__(self, attributes=None, float_array=None, ids=None, media_ids=None, media_query=None, new_version=None, object_search=None, state_ids=None, user_elemental_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, float_array=None, ids=None, media_ids=None, media_query=None, new_elemental_id=None, new_version=None, object_search=None, state_ids=None, user_elemental_id=None, local_vars_configuration=None):  # noqa: E501
         """LocalizationBulkUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
         self._float_array = None
         self._ids = None
         self._media_ids = None
         self._media_query = None
+        self._new_elemental_id = None
         self._new_version = None
         self._object_search = None
         self._state_ids = None
         self._user_elemental_id = None
         self.discriminator = None
 
         if attributes is not None:
@@ -76,14 +79,16 @@
             self.float_array = float_array
         if ids is not None:
             self.ids = ids
         if media_ids is not None:
             self.media_ids = media_ids
         if media_query is not None:
             self.media_query = media_query
+        if new_elemental_id is not None:
+            self.new_elemental_id = new_elemental_id
         if new_version is not None:
             self.new_version = new_version
         if object_search is not None:
             self.object_search = object_search
         if state_ids is not None:
             self.state_ids = state_ids
         if user_elemental_id is not None:
@@ -191,14 +196,35 @@
         :param media_query: The media_query of this LocalizationBulkUpdate.
         :type: str
         """
 
         self._media_query = media_query
 
     @property
+    def new_elemental_id(self):
+        """
+        The new elemental ID for these objects
+
+        :return: The new_elemental_id of this LocalizationBulkUpdate. 
+        :rtype: str
+        """
+        return self._new_elemental_id
+
+    @new_elemental_id.setter
+    def new_elemental_id(self, new_elemental_id):
+        """
+        The new elemental ID for these objects
+
+        :param new_elemental_id: The new_elemental_id of this LocalizationBulkUpdate.
+        :type: str
+        """
+
+        self._new_elemental_id = new_elemental_id
+
+    @property
     def new_version(self):
         """
         Unique integer identifying a new version for these objects
 
         :return: The new_version of this LocalizationBulkUpdate. 
         :rtype: int
         """
```

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_delete.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_id_query.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_type.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_type_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_type_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/localization_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/localization_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_bulk_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_files.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_files.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_id_query.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_next.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_next.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_prev.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_prev.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_stats.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_stats.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_type.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_type_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_type_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/media_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/media_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/membership.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/membership_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/membership_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/membership_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/membership_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/message_response.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/message_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/multi_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/multi_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/not_found_response.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/not_found_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/notify_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/notify_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/organization.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/organization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/organization_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/organization_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/organization_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/organization_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/password_reset_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/password_reset_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/project.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/project.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/project_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/project_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/project_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/project_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/resolution_config.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/resolution_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/s3_storage_config.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/s3_storage_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/section.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/section_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/section_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/section_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/section_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_bulk_delete.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_bulk_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_delete.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_id_query.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_merge_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_merge_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_trim_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_trim_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_type.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_type_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_type_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/state_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/state_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/temporary_file.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/temporary_file_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/temporary_file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/token.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/token.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/transcode.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/transcode_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/transcode_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/upload_completion_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/upload_completion_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/upload_info.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/upload_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/upload_part.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/upload_part.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/user.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/user.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/user_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/user_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/user_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/user_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/version.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/version_spec.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/version_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/version_update.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/version_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/video_clip.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/video_clip.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/models/video_definition.py` & `tator-1.0.5/tator/openapi/tator_openapi/models/video_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/openapi/tator_openapi/rest.py` & `tator-1.0.5/tator/openapi/tator_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/__main__.py` & `tator-1.0.5/tator/transcode/__main__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/black.mp4` & `tator-1.0.5/tator/transcode/black.mp4`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/create_media.py` & `tator-1.0.5/tator/transcode/create_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/delete_media.py` & `tator-1.0.5/tator/transcode/delete_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/determine_transcode.py` & `tator-1.0.5/tator/transcode/determine_transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/make_fragment_info.py` & `tator-1.0.5/tator/transcode/make_fragment_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/make_thumbnails.py` & `tator-1.0.5/tator/transcode/make_thumbnails.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/prepare.py` & `tator-1.0.5/tator/transcode/prepare.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/transcode/transcode.py` & `tator-1.0.5/tator/transcode/transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/__init__.py` & `tator-1.0.5/tator/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/_download_file.py` & `tator-1.0.5/tator/util/_download_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/_upload_file.py` & `tator-1.0.5/tator/util/_upload_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/chunked_create.py` & `tator-1.0.5/tator/util/chunked_create.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/chunked_file_list.py` & `tator-1.0.5/tator/util/chunked_file_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_leaf_list.py` & `tator-1.0.5/tator/util/clone_leaf_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_leaf_type.py` & `tator-1.0.5/tator/util/clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_localization_list.py` & `tator-1.0.5/tator/util/clone_localization_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_localization_type.py` & `tator-1.0.5/tator/util/clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_media_list.py` & `tator-1.0.5/tator/util/clone_media_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_media_type.py` & `tator-1.0.5/tator/util/clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_membership.py` & `tator-1.0.5/tator/util/clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_section.py` & `tator-1.0.5/tator/util/clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_state_list.py` & `tator-1.0.5/tator/util/clone_state_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_state_type.py` & `tator-1.0.5/tator/util/clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/clone_version.py` & `tator-1.0.5/tator/util/clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/concat.py` & `tator-1.0.5/tator/util/concat.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/download_attachment.py` & `tator-1.0.5/tator/util/download_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/download_media.py` & `tator-1.0.5/tator/util/download_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/download_temporary_file.py` & `tator-1.0.5/tator/util/download_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/find_single_change.py` & `tator-1.0.5/tator/util/find_single_change.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/full_state_graphic.py` & `tator-1.0.5/tator/util/full_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/get_api.py` & `tator-1.0.5/tator/util/get_api.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/get_images.py` & `tator-1.0.5/tator/util/get_images.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/get_paginator.py` & `tator-1.0.5/tator/util/get_paginator.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/import_media.py` & `tator-1.0.5/tator/util/import_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/live_stream.py` & `tator-1.0.5/tator/util/live_stream.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/md5sum.py` & `tator-1.0.5/tator/util/md5sum.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/media_manipulation.py` & `tator-1.0.5/tator/util/media_manipulation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/media_util.py` & `tator-1.0.5/tator/util/media_util.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/multi_stream.py` & `tator-1.0.5/tator/util/multi_stream.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/register_algorithm.py` & `tator-1.0.5/tator/util/register_algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/register_applet.py` & `tator-1.0.5/tator/util/register_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/tator-symbol.png` & `tator-1.0.5/tator/util/tator-symbol.png`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/to_dataframe.py` & `tator-1.0.5/tator/util/to_dataframe.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/update_applet.py` & `tator-1.0.5/tator/util/update_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/upload_attachment.py` & `tator-1.0.5/tator/util/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/upload_media.py` & `tator-1.0.5/tator/util/upload_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator/util/upload_temporary_file.py` & `tator-1.0.5/tator/util/upload_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/tator.egg-info/SOURCES.txt` & `tator-1.0.5/tator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_a_float_array.py` & `tator-1.0.5/test/test_a_float_array.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_algorithm.py` & `tator-1.0.5/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_algorithm_launch.py` & `tator-1.0.5/test/test_algorithm_launch.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_applet.py` & `tator-1.0.5/test/test_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_archive_date.py` & `tator-1.0.5/test/test_archive_date.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_attachment.py` & `tator-1.0.5/test/test_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_attribute_type_addition.py` & `tator-1.0.5/test/test_attribute_type_addition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_attribute_type_deletion.py` & `tator-1.0.5/test/test_attribute_type_deletion.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_attribute_type_mutation.py` & `tator-1.0.5/test/test_attribute_type_mutation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_attributes.py` & `tator-1.0.5/test/test_attributes.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_change_log.py` & `tator-1.0.5/test/test_change_log.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_clone_leaf_type.py` & `tator-1.0.5/test/test_clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_clone_localization_type.py` & `tator-1.0.5/test/test_clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_clone_media.py` & `tator-1.0.5/test/test_clone_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_clone_media_type.py` & `tator-1.0.5/test/test_clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_clone_membership.py` & `tator-1.0.5/test/test_clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_clone_section.py` & `tator-1.0.5/test/test_clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_clone_state_type.py` & `tator-1.0.5/test/test_clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_clone_version.py` & `tator-1.0.5/test/test_clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_collection.py` & `tator-1.0.5/test/test_collection.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_download_media.py` & `tator-1.0.5/test/test_download_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_extract.py` & `tator-1.0.5/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_file.py` & `tator-1.0.5/test/test_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_file_type.py` & `tator-1.0.5/test/test_file_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_get_clip.py` & `tator-1.0.5/test/test_get_clip.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_getframe.py` & `tator-1.0.5/test/test_getframe.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_import_media.py` & `tator-1.0.5/test/test_import_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_job_cancel.py` & `tator-1.0.5/test/test_job_cancel.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_job_cluster.py` & `tator-1.0.5/test/test_job_cluster.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_leaf.py` & `tator-1.0.5/test/test_leaf.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_leaf_type.py` & `tator-1.0.5/test/test_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_local_transcode.py` & `tator-1.0.5/test/test_local_transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_localization.py` & `tator-1.0.5/test/test_localization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_localization_graphic.py` & `tator-1.0.5/test/test_localization_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_localization_type.py` & `tator-1.0.5/test/test_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_media.py` & `tator-1.0.5/test/test_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_media_type.py` & `tator-1.0.5/test/test_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_pagination.py` & `tator-1.0.5/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_poly.py` & `tator-1.0.5/test/test_poly.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_search.py` & `tator-1.0.5/test/test_search.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_state.py` & `tator-1.0.5/test/test_state.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_state_graphic.py` & `tator-1.0.5/test/test_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_state_type.py` & `tator-1.0.5/test/test_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_stategraphic.py` & `tator-1.0.5/test/test_stategraphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_temporary_file.py` & `tator-1.0.5/test/test_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_tracks.py` & `tator-1.0.5/test/test_tracks.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_transcode.py` & `tator-1.0.5/test/test_transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_util_media_manipulation.py` & `tator-1.0.5/test/test_util_media_manipulation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_util_media_util.py` & `tator-1.0.5/test/test_util_media_util.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.4/test/test_version.py` & `tator-1.0.5/test/test_version.py`

 * *Files identical despite different names*

