# Comparing `tmp/pycti-5.7.post576.tar.gz` & `tmp/pycti-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.7.post576.tar", last modified: Sat May 20 08:21:39 2023, max compression
+gzip compressed data, was "pycti-5.8.0.tar", last modified: Mon Jun 19 01:40:10 2023, max compression
```

## Comparing `pycti-5.7.post576.tar` & `pycti-5.8.0.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-20 08:21:39.350945 pycti-5.7.post576/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-20 08:21:26.000000 pycti-5.7.post576/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4093 2023-05-20 08:21:39.350945 pycti-5.7.post576/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-05-20 08:21:26.000000 pycti-5.7.post576/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-20 08:21:39.342945 pycti-5.7.post576/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-20 08:21:39.342945 pycti-5.7.post576/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28212 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-20 08:21:39.342945 pycti-5.7.post576/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42775 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-20 08:21:39.350945 pycti-5.7.post576/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18873 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13395 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24396 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23837 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23845 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14531 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14618 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14175 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14023 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10890 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24602 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22933 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17579 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14043 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23075 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15937 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7853 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13002 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14543 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16314 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12155 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22349 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22661 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20977 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23801 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32054 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41821 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64475 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18392 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14229 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17702 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-20 08:21:39.350945 pycti-5.7.post576/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3308 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   101666 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-05-20 08:21:26.000000 pycti-5.7.post576/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-20 08:21:39.342945 pycti-5.7.post576/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4093 2023-05-20 08:21:39.000000 pycti-5.7.post576/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2250 2023-05-20 08:21:39.000000 pycti-5.7.post576/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-20 08:21:39.000000 pycti-5.7.post576/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-05-20 08:21:39.000000 pycti-5.7.post576/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-20 08:21:39.000000 pycti-5.7.post576/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-05-20 08:21:26.000000 pycti-5.7.post576/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-05-20 08:21:39.350945 pycti-5.7.post576/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 01:40:10.492329 pycti-5.8.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-19 01:40:00.000000 pycti-5.8.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-19 01:40:10.492329 pycti-5.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-06-19 01:40:00.000000 pycti-5.8.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 01:40:10.484329 pycti-5.8.0/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3856 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 01:40:10.484329 pycti-5.8.0/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28410 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 01:40:10.484329 pycti-5.8.0/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45416 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 01:40:10.492329 pycti-5.8.0/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13376 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25113 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24427 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24435 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14512 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14598 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14155 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10891 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22913 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17564 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14024 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23077 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15944 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22348 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22667 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20971 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23782 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32580 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64475 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23493 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18371 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 01:40:10.492329 pycti-5.8.0/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3397 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   103481 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-06-19 01:40:00.000000 pycti-5.8.0/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 01:40:10.484329 pycti-5.8.0/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-19 01:40:10.000000 pycti-5.8.0/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-06-19 01:40:10.000000 pycti-5.8.0/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-19 01:40:10.000000 pycti-5.8.0/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-06-19 01:40:10.000000 pycti-5.8.0/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-19 01:40:10.000000 pycti-5.8.0/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-06-19 01:40:00.000000 pycti-5.8.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-06-19 01:40:10.492329 pycti-5.8.0/setup.cfg
```

### Comparing `pycti-5.7.post576/LICENSE` & `pycti-5.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/PKG-INFO` & `pycti-5.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.7.post576
+Version: 5.8.0
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.7.post576 Summary: Python API
-client for OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-
-python Author: Filigran Author-email: contact@filigran.io Maintainer: Filigran
-License: Apache Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Information Technology Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Natural Language :: English Classifier: Natural Language :: French Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Topic :: Security Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: doc License-File: LICENSE #
-OpenCTI client for Python [![Website](https://img.shields.io/badge/website-
-opencti.io-blue.svg)](https://www.opencti.io) [![CircleCI](https://
-circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://
-circleci.com/gh/OpenCTI-Platform/client-python/tree/master) [![readthedocs]
-(https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)]
-(https://opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub
-release](https://img.shields.io/github/release/OpenCTI-Platform/client-
-python.svg)](https://github.com/OpenCTI-Platform/client-python/releases/latest)
-[![Number of PyPI downloads](https://img.shields.io/pypi/dm/pycti.svg)](https:/
-/pypi.python.org/pypi/pycti/) [![Slack Status](https://img.shields.io/badge/
-slack-3K%2B%20members-4A154B)](https://community.filigran.io) The official
-OpenCTI Python client helps developers to use the OpenCTI API by providing easy
-to use methods and utils. This client is also used by some OpenCTI components.
-## Install To install the latest Python client library, please use `pip`:
-```bash $ pip3 install pycti ``` ## Local development ```bash # Fork the
-current repository, then clone your fork $ git clone https://github.com/YOUR-
-USERNAME/client-python $ cd client-python $ git remote add upstream https://
-github.com/OpenCTI-Platform/client-python.git # Create a branch for your
-feature/fix $ git checkout -b [branch-name] # Create a virtualenv $ python3 -
-m venv .venv $ source .venv/bin/activate # Install the client-python and
-dependencies for the development and the documentation $ python3 -m pip install
--e .[dev,doc] # Set up the git hook scripts $ pre-commit install # Create your
-feature/fix # Create tests for your changes $ pytest # Push you feature/fix on
-Github $ git add [file(s)] $ git commit -m "[descriptive message]" $ git push
-origin [branch-name] # Open a pull request ``` ### Install the package locally
-```bash $ pip install -e . ``` ## Documentation ### Client usage To learn about
-how to use the OpenCTI Python client and read some examples and cases, refer to
-[the client documentation](https://opencti-client-for-python.readthedocs.io/en/
+Metadata-Version: 2.1 Name: pycti Version: 5.8.0 Summary: Python API client for
+OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
+Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Natural Language :: English
+Classifier: Natural Language :: French Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier: Topic
+:: Security Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: doc License-File: LICENSE # OpenCTI client
+for Python [![Website](https://img.shields.io/badge/website-opencti.io-
+blue.svg)](https://www.opencti.io) [![CircleCI](https://circleci.com/gh/
+OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/
+OpenCTI-Platform/client-python/tree/master) [![readthedocs](https://
+readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://
+opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub release](https:/
+/img.shields.io/github/release/OpenCTI-Platform/client-python.svg)](https://
+github.com/OpenCTI-Platform/client-python/releases/latest) [![Number of PyPI
+downloads](https://img.shields.io/pypi/dm/pycti.svg)](https://pypi.python.org/
+pypi/pycti/) [![Slack Status](https://img.shields.io/badge/slack-
+3K%2B%20members-4A154B)](https://community.filigran.io) The official OpenCTI
+Python client helps developers to use the OpenCTI API by providing easy to use
+methods and utils. This client is also used by some OpenCTI components. ##
+Install To install the latest Python client library, please use `pip`: ```bash
+$ pip3 install pycti ``` ## Local development ```bash # Fork the current
+repository, then clone your fork $ git clone https://github.com/YOUR-USERNAME/
+client-python $ cd client-python $ git remote add upstream https://github.com/
+OpenCTI-Platform/client-python.git # Create a branch for your feature/fix $ git
+checkout -b [branch-name] # Create a virtualenv $ python3 -m venv .venv $
+source .venv/bin/activate # Install the client-python and dependencies for the
+development and the documentation $ python3 -m pip install -e .[dev,doc] # Set
+up the git hook scripts $ pre-commit install # Create your feature/fix # Create
+tests for your changes $ pytest # Push you feature/fix on Github $ git add
+[file(s)] $ git commit -m "[descriptive message]" $ git push origin [branch-
+name] # Open a pull request ``` ### Install the package locally ```bash $ pip
+install -e . ``` ## Documentation ### Client usage To learn about how to use
+the OpenCTI Python client and read some examples and cases, refer to [the
+client documentation](https://opencti-client-for-python.readthedocs.io/en/
 latest/client_usage/getting_started.html). ### API reference To learn about the
 methods available for executing queries and retrieving their answers, refer to
 [the client API Reference](https://opencti-client-for-python.readthedocs.io/en/
 latest/pycti/pycti.html). ## Tests ### Install dependencies ```bash $ pip
 install -r ./test-requirements.txt ``` [pytest](https://docs.pytest.org/en/
 7.2.x/) is used to launch the tests. ### Launch tests #### Prerequisite Your
 OpenCTI API should be running. Your conftest.py should be configured with your
```

### Comparing `pycti-5.7.post576/README.md` & `pycti-5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/__init__.py` & `pycti-5.8.0/pycti/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.7.post576"
+__version__ = "5.8.0"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
@@ -25,27 +25,29 @@
 from .entities.opencti_indicator import Indicator
 from .entities.opencti_infrastructure import Infrastructure
 from .entities.opencti_intrusion_set import IntrusionSet
 from .entities.opencti_kill_chain_phase import KillChainPhase
 from .entities.opencti_label import Label
 from .entities.opencti_location import Location
 from .entities.opencti_malware import Malware
+from .entities.opencti_malware_analysis import MalwareAnalysis
 from .entities.opencti_marking_definition import MarkingDefinition
 from .entities.opencti_note import Note
 from .entities.opencti_observed_data import ObservedData
 from .entities.opencti_opinion import Opinion
 from .entities.opencti_report import Report
 from .entities.opencti_stix_core_relationship import StixCoreRelationship
 from .entities.opencti_stix_cyber_observable import StixCyberObservable
 from .entities.opencti_stix_domain_object import StixDomainObject
 from .entities.opencti_stix_nested_ref_relationship import StixNestedRefRelationship
 from .entities.opencti_stix_object_or_stix_relationship import (
     StixObjectOrStixRelationship,
 )
 from .entities.opencti_stix_sighting_relationship import StixSightingRelationship
+from .entities.opencti_task import Task
 from .entities.opencti_threat_actor import ThreatActor
 from .entities.opencti_tool import Tool
 from .entities.opencti_vulnerability import Vulnerability
 from .utils.constants import (
     MultipleRefRelationship,
     StixCyberObservableTypes,
     StixMetaTypes,
@@ -57,14 +59,15 @@
 
 __all__ = [
     "AttackPattern",
     "Campaign",
     "CaseIncident",
     "CaseRfi",
     "CaseRft",
+    "Task",
     "ConnectorType",
     "CourseOfAction",
     "DataComponent",
     "DataSource",
     "ExternalReference",
     "Feedback",
     "Grouping",
@@ -73,14 +76,15 @@
     "Indicator",
     "Infrastructure",
     "IntrusionSet",
     "KillChainPhase",
     "Label",
     "Location",
     "Malware",
+    "MalwareAnalysis",
     "MarkingDefinition",
     "Note",
     "ObservedData",
     "OpenCTIApiClient",
     "OpenCTIApiConnector",
     "OpenCTIApiWork",
     "OpenCTIConnector",
```

### Comparing `pycti-5.7.post576/pycti/api/opencti_api_client.py` & `pycti-5.8.0/pycti/api/opencti_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from pycti.entities.opencti_infrastructure import Infrastructure
 from pycti.entities.opencti_intrusion_set import IntrusionSet
 from pycti.entities.opencti_kill_chain_phase import KillChainPhase
 from pycti.entities.opencti_label import Label
 from pycti.entities.opencti_language import Language
 from pycti.entities.opencti_location import Location
 from pycti.entities.opencti_malware import Malware
+from pycti.entities.opencti_malware_analysis import MalwareAnalysis
 from pycti.entities.opencti_marking_definition import MarkingDefinition
 from pycti.entities.opencti_narrative import Narrative
 from pycti.entities.opencti_note import Note
 from pycti.entities.opencti_observed_data import ObservedData
 from pycti.entities.opencti_opinion import Opinion
 from pycti.entities.opencti_report import Report
 from pycti.entities.opencti_stix import Stix
@@ -52,14 +53,15 @@
 from pycti.entities.opencti_stix_nested_ref_relationship import (
     StixNestedRefRelationship,
 )
 from pycti.entities.opencti_stix_object_or_stix_relationship import (
     StixObjectOrStixRelationship,
 )
 from pycti.entities.opencti_stix_sighting_relationship import StixSightingRelationship
+from pycti.entities.opencti_task import Task
 from pycti.entities.opencti_threat_actor import ThreatActor
 from pycti.entities.opencti_tool import Tool
 from pycti.entities.opencti_vocabulary import Vocabulary
 from pycti.entities.opencti_vulnerability import Vulnerability
 from pycti.utils.opencti_stix2 import OpenCTIStix2
 from pycti.utils.opencti_stix2_utils import OpenCTIStix2Utils
 
@@ -182,16 +184,18 @@
         self.intrusion_set = IntrusionSet(self)
         self.infrastructure = Infrastructure(self)
         self.campaign = Campaign(self)
         self.case_incident = CaseIncident(self)
         self.feedback = Feedback(self)
         self.case_rfi = CaseRfi(self)
         self.case_rft = CaseRft(self)
+        self.task = Task(self)
         self.incident = Incident(self)
         self.malware = Malware(self)
+        self.malware_analysis = MalwareAnalysis(self)
         self.tool = Tool(self)
         self.channel = Channel(self)
         self.narrative = Narrative(self)
         self.language = Language(self)
         self.vulnerability = Vulnerability(self)
         self.attack_pattern = AttackPattern(self)
         self.course_of_action = CourseOfAction(self)
```

### Comparing `pycti-5.7.post576/pycti/api/opencti_api_connector.py` & `pycti-5.8.0/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/api/opencti_api_work.py` & `pycti-5.8.0/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/connector/opencti_connector.py` & `pycti-5.8.0/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/connector/opencti_connector_helper.py` & `pycti-5.8.0/pycti/connector/opencti_connector_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import logging
 import os
 import queue
 import signal
 import ssl
 import sys
+import tempfile
 import threading
 import time
 import traceback
 import uuid
 from queue import Queue
 from typing import Callable, Dict, List, Optional, Union
 
@@ -75,63 +76,122 @@
 
     if isinstance(result, str) and len(result) == 0:
         return default
 
     return result
 
 
-def create_ssl_context() -> ssl.SSLContext:
-    """Set strong SSL defaults: require TLSv1.2+
+def is_memory_certificate(certificate):
+    return certificate.startswith("-----BEGIN")
 
-    `ssl` uses bitwise operations to specify context `<enum 'Options'>`
-    """
 
-    ssl_context_options: List[int] = [
-        ssl.OP_NO_COMPRESSION,
-        ssl.OP_NO_TICKET,  # pylint: disable=no-member
-        ssl.OP_NO_RENEGOTIATION,  # pylint: disable=no-member
-        ssl.OP_SINGLE_DH_USE,
-        ssl.OP_SINGLE_ECDH_USE,
-    ]
-    ssl_context = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH)
-    ssl_context.options &= ~ssl.OP_ENABLE_MIDDLEBOX_COMPAT  # pylint: disable=no-member
-    ssl_context.verify_mode = ssl.CERT_REQUIRED
-    ssl_context.minimum_version = ssl.TLSVersion.TLSv1_2
+def ssl_verify_locations(ssl_context, certdata):
+    if certdata is None:
+        return
+
+    if is_memory_certificate(certdata):
+        ssl_context.load_verify_locations(cadata=certdata)
+    else:
+        ssl_context.load_verify_locations(cafile=certdata)
 
-    for option in ssl_context_options:
-        ssl_context.options |= option
 
+# As cert must be written in files to be loaded in ssl context
+# Creates a temporary file in the most secure manner possible
+def data_to_temp_file(data):
+    # The file is readable and writable only by the creating user ID.
+    # If the operating system uses permission bits to indicate whether a
+    # file is executable, the file is executable by no one. The file
+    # descriptor is not inherited by children of this process.
+    file_descriptor, file_path = tempfile.mkstemp()
+    with os.fdopen(file_descriptor, "w") as open_file:
+        open_file.write(data)
+        open_file.close()
+    return file_path
+
+
+def ssl_cert_chain(ssl_context, cert_data, key_data, passphrase):
+    if cert_data is None:
+        return
+
+    cert_file_path = None
+    key_file_path = None
+
+    # Cert loading
+    if cert_data is not None and is_memory_certificate(cert_data):
+        cert_file_path = data_to_temp_file(cert_data)
+    cert = cert_file_path if cert_file_path is not None else cert_data
+
+    # Key loading
+    if key_data is not None and is_memory_certificate(key_data):
+        key_file_path = data_to_temp_file(key_data)
+    key = key_file_path if key_file_path is not None else key_data
+
+    # Load cert
+    ssl_context.load_cert_chain(cert, key, passphrase)
+    # Remove temp files
+    if cert_file_path is not None:
+        os.unlink(cert_file_path)
+    if key_file_path is not None:
+        os.unlink(key_file_path)
+
+
+def create_mq_ssl_context(config) -> ssl.SSLContext:
+    use_ssl_ca = get_config_variable("MQ_USE_SSL_CA", ["mq", "use_ssl_ca"], config)
+    use_ssl_cert = get_config_variable(
+        "MQ_USE_SSL_CERT", ["mq", "use_ssl_cert"], config
+    )
+    use_ssl_key = get_config_variable("MQ_USE_SSL_KEY", ["mq", "use_ssl_key"], config)
+    use_ssl_reject_unauthorized = get_config_variable(
+        "MQ_USE_SSL_REJECT_UNAUTHORIZED",
+        ["mq", "use_ssl_reject_unauthorized"],
+        config,
+        False,
+        False,
+    )
+    use_ssl_passphrase = get_config_variable(
+        "MQ_USE_SSL_PASSPHRASE", ["mq", "use_ssl_passphrase"], config
+    )
+    ssl_context = ssl.create_default_context()
+    # If no rejection allowed, use private function to generate unverified context
+    if not use_ssl_reject_unauthorized:
+        # noinspection PyUnresolvedReferences,PyProtectedMember
+        ssl_context = ssl._create_unverified_context()
+    ssl_verify_locations(ssl_context, use_ssl_ca)
+    # Thanks to https://bugs.python.org/issue16487 is not possible today to easily use memory pem
+    # in SSL context. We need to write it to a temporary file before
+    ssl_cert_chain(ssl_context, use_ssl_cert, use_ssl_key, use_ssl_passphrase)
     return ssl_context
 
 
 class ListenQueue:
     """Main class for the ListenQueue used in OpenCTIConnectorHelper
 
     :param helper: instance of a `OpenCTIConnectorHelper` class
     :type helper: OpenCTIConnectorHelper
     :param config: dict containing client config
     :type config: Dict
     :param callback: callback function to process queue
     :type callback: callable
     """
 
-    def __init__(self, helper, config: Dict, callback) -> None:
+    def __init__(self, helper, config: Dict, connector_config: Dict, callback) -> None:
         self.pika_credentials = None
         self.pika_parameters = None
         self.pika_connection = None
         self.channel = None
         self.helper = helper
         self.callback = callback
-        self.host = config["connection"]["host"]
-        self.vhost = config["connection"]["vhost"]
-        self.use_ssl = config["connection"]["use_ssl"]
-        self.port = config["connection"]["port"]
-        self.user = config["connection"]["user"]
-        self.password = config["connection"]["pass"]
-        self.queue_name = config["listen"]
+        self.config = config
+        self.host = connector_config["connection"]["host"]
+        self.vhost = connector_config["connection"]["vhost"]
+        self.use_ssl = connector_config["connection"]["use_ssl"]
+        self.port = connector_config["connection"]["port"]
+        self.user = connector_config["connection"]["user"]
+        self.password = connector_config["connection"]["pass"]
+        self.queue_name = connector_config["listen"]
         self.connector_thread = None
         self.connector_event_loop = None
         self.queue_event_loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self.queue_event_loop)
         self.run()
 
     # noinspection PyUnusedLocal
@@ -211,15 +271,17 @@
                 # Connect the broker
                 self.pika_credentials = pika.PlainCredentials(self.user, self.password)
                 self.pika_parameters = pika.ConnectionParameters(
                     host=self.host,
                     port=self.port,
                     virtual_host=self.vhost,
                     credentials=self.pika_credentials,
-                    ssl_options=pika.SSLOptions(create_ssl_context(), self.host)
+                    ssl_options=pika.SSLOptions(
+                        create_mq_ssl_context(self.config), self.host
+                    )
                     if self.use_ssl
                     else None,
                 )
                 if asyncio.iscoroutinefunction(self.callback):
                     self.connector_event_loop = asyncio.new_event_loop()
                     self.connector_thread = threading.Thread(
                         target=lambda: start_loop(self.connector_event_loop)
@@ -480,14 +542,15 @@
     :type config: Dict
     """
 
     def __init__(self, config: Dict) -> None:
         sys.excepthook = killProgramHook
 
         # Load API config
+        self.config = config
         self.opencti_url = get_config_variable(
             "OPENCTI_URL", ["opencti", "url"], config
         )
         self.opencti_token = get_config_variable(
             "OPENCTI_TOKEN", ["opencti", "token"], config
         )
         self.opencti_ssl_verify = get_config_variable(
@@ -613,15 +676,15 @@
         )
         connector_configuration = self.api.connector.register(self.connector)
         LOGGER.info("Connector registered with ID: %s", self.connect_id)
         self.connector_id = connector_configuration["id"]
         self.work_id = None
         self.applicant_id = connector_configuration["connector_user_id"]
         self.connector_state = connector_configuration["connector_state"]
-        self.config = connector_configuration["config"]
+        self.connector_config = connector_configuration["config"]
 
         # Start ping thread
         if not self.connect_run_and_terminate:
             self.ping = PingAlive(
                 self.connector.id, self.api, self.get_state, self.set_state
             )
             self.ping.start()
@@ -721,15 +784,17 @@
     def listen(self, message_callback: Callable[[Dict], str]) -> None:
         """listen for messages and register callback function
 
         :param message_callback: callback function to process messages
         :type message_callback: Callable[[Dict], str]
         """
 
-        self.listen_queue = ListenQueue(self, self.config, message_callback)
+        self.listen_queue = ListenQueue(
+            self, self.config, self.connector_config, message_callback
+        )
 
     def listen_stream(
         self,
         message_callback,
         url=None,
         token=None,
         verify_ssl=None,
@@ -903,25 +968,27 @@
         if len(bundles) == 0:
             raise ValueError("Nothing to import")
 
         if work_id:
             self.api.work.add_expectations(work_id, len(bundles))
 
         pika_credentials = pika.PlainCredentials(
-            self.config["connection"]["user"], self.config["connection"]["pass"]
+            self.connector_config["connection"]["user"],
+            self.connector_config["connection"]["pass"],
         )
         pika_parameters = pika.ConnectionParameters(
-            host=self.config["connection"]["host"],
-            port=self.config["connection"]["port"],
-            virtual_host=self.config["connection"]["vhost"],
+            host=self.connector_config["connection"]["host"],
+            port=self.connector_config["connection"]["port"],
+            virtual_host=self.connector_config["connection"]["vhost"],
             credentials=pika_credentials,
             ssl_options=pika.SSLOptions(
-                create_ssl_context(), self.config["connection"]["host"]
+                create_mq_ssl_context(self.config),
+                self.connector_config["connection"]["host"],
             )
-            if self.config["connection"]["use_ssl"]
+            if self.connector_config["connection"]["use_ssl"]
             else None,
         )
 
         pika_connection = pika.BlockingConnection(pika_parameters)
         channel = pika_connection.channel()
         for sequence, bundle in enumerate(bundles, start=1):
             self._send_bundle(
@@ -974,16 +1041,16 @@
         }
         if work_id is not None:
             message["work_id"] = work_id
 
         # Send the message
         try:
             channel.basic_publish(
-                exchange=self.config["push_exchange"],
-                routing_key=self.config["push_routing"],
+                exchange=self.connector_config["push_exchange"],
+                routing_key=self.connector_config["push_routing"],
                 body=json.dumps(message),
                 properties=pika.BasicProperties(
                     delivery_mode=2,  # make message persistent
                 ),
             )
         except (UnroutableError, NackError) as e:
             LOGGER.error("Unable to send bundle, retry...%s", e)
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_attack_pattern.py` & `pycti-5.8.0/pycti/entities/opencti_attack_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,15 @@
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             LOGGER.info("Creating Attack-Pattern {%s}.", name)
             query = """
-                mutation AttackPatternAdd($input: AttackPatternAddInput) {
+                mutation AttackPatternAdd($input: AttackPatternAddInput!) {
                     attackPatternAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -438,31 +438,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 x_mitre_platforms=stix_object["x_mitre_platforms"]
                 if "x_mitre_platforms" in stix_object
                 else stix_object["x_amitt_platforms"]
                 if "x_amitt_platforms" in stix_object
                 else None,
                 x_mitre_permissions_required=stix_object["x_mitre_permissions_required"]
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_campaign.py` & `pycti-5.8.0/pycti/entities/opencti_campaign.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,27 +256,27 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         first_seen = kwargs.get("first_seen", None)
         last_seen = kwargs.get("last_seen", None)
         objective = kwargs.get("objective", None)
         granted_refs = kwargs.get("objectOrganization", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Campaign {%s}.", name)
             query = """
-                mutation CampaignAdd($input: CampaignAddInput) {
+                mutation CampaignAdd($input: CampaignAddInput!) {
                     campaignAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -339,31 +339,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 objective=stix_object["objective"]
                 if "objective" in stix_object
                 else None,
                 first_seen=stix_object["first_seen"]
                 if "first_seen" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_case_incident.py` & `pycti-5.8.0/pycti/entities/opencti_case_incident.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import uuid
 
 from dateutil.parser import parse
 from stix2.canonicalization.Canonicalize import canonicalize
 
+from pycti.entities import LOGGER
+
 
 class CaseIncident:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
@@ -455,15 +457,15 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         severity = kwargs.get("severity", None)
         priority = kwargs.get("priority", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
         response_types = kwargs.get("response_types", None)
 
@@ -534,16 +536,18 @@
                 + stix_object_or_stix_relationship_id
                 + "} to CaseIncident {"
                 + id
                 + "}",
             )
             query = """
                mutation CaseIncidentEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput!) {
-                    caseIncidentRelationAdd(id: $id, input: $input) {
-                        id
+                    stixDomainObjectEdit(id: $id) {
+                        relationAdd(input: $input) {
+                            id
+                        }
                     }
                }
             """
             self.opencti.query(
                 query,
                 {
                     "id": id,
@@ -581,16 +585,18 @@
                 + stix_object_or_stix_relationship_id
                 + "} to CaseIncident {"
                 + id
                 + "}",
             )
             query = """
                mutation CaseIncidentEditRelationDelete($id: ID!, $toId: StixRef!, $relationship_type: String!) {
-                    caseIncidentRelationDelete(id: $id, toId: $toId, relationship_type: $relationship_type) {
-                        id
+                    stixDomainObjectEdit(id: $id) {
+                        relationDelete(toId: $toId, relationship_type: $relationship_type) {
+                            id
+                        }
                     }
                }
             """
             self.opencti.query(
                 query,
                 {
                     "id": id,
@@ -634,32 +640,32 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 objects=extras["object_ids"] if "object_ids" in extras else [],
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 severity=stix_object["severity"] if "severity" in stix_object else None,
                 priority=stix_object["priority"] if "priority" in stix_object else None,
                 response_types=stix_object["response_types"]
                 if "response_types" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
@@ -669,7 +675,23 @@
                 else None,
                 update=update,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_caseIncident] Missing parameters: stixObject"
             )
+
+    def delete(self, **kwargs):
+        id = kwargs.get("id", None)
+        if id is not None:
+            LOGGER.info("Deleting Case Incident {%s}.", id)
+            query = """
+                 mutation CaseIncidentDelete($id: ID!) {
+                     stixDomainObjectEdit(id: $id) {
+                         delete
+                     }
+                 }
+             """
+            self.opencti.query(query, {"id": id})
+        else:
+            LOGGER.error("[opencti_case_incident] Missing parameters: id")
+            return None
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_case_rfi.py` & `pycti-5.8.0/pycti/entities/opencti_case_rfi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import uuid
 
 from dateutil.parser import parse
 from stix2.canonicalization.Canonicalize import canonicalize
 
+from pycti.entities import LOGGER
+
 
 class CaseRfi:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
@@ -452,15 +454,15 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
         information_types = kwargs.get("information_types", None)
 
         if name is not None:
             self.opencti.log("info", "Creating Case Rfi {" + name + "}.")
@@ -525,15 +527,15 @@
                 + stix_object_or_stix_relationship_id
                 + "} to CaseRfi {"
                 + id
                 + "}",
             )
             query = """
                mutation CaseRfiEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput) {
-                   caseRfiEdit(id: $id) {
+                   stixDomainObjectEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
             self.opencti.query(
@@ -574,15 +576,15 @@
                 + stix_object_or_stix_relationship_id
                 + "} to CaseRfi {"
                 + id
                 + "}",
             )
             query = """
                mutation CaseRfiEditRelationDelete($id: ID!, $toId: StixRef!, $relationship_type: String!) {
-                   caseRfiEdit(id: $id) {
+                   stixDomainObjectEdit(id: $id) {
                         relationDelete(toId: $toId, relationship_type: $relationship_type) {
                             id
                         }
                    }
                }
             """
             self.opencti.query(
@@ -629,32 +631,32 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 objects=extras["object_ids"] if "object_ids" in extras else [],
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
@@ -662,7 +664,23 @@
                 if "information_types" in stix_object
                 else None,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_caseRfi] Missing parameters: stixObject"
             )
+
+    def delete(self, **kwargs):
+        id = kwargs.get("id", None)
+        if id is not None:
+            LOGGER.info("Deleting Case RFI {%s}.", id)
+            query = """
+                 mutation CaseRFIDelete($id: ID!) {
+                     stixDomainObjectEdit(id: $id) {
+                         delete
+                     }
+                 }
+             """
+            self.opencti.query(query, {"id": id})
+        else:
+            LOGGER.error("[opencti_case_rfi] Missing parameters: id")
+            return None
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_case_rft.py` & `pycti-5.8.0/pycti/entities/opencti_case_rft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import uuid
 
 from dateutil.parser import parse
 from stix2.canonicalization.Canonicalize import canonicalize
 
+from pycti.entities import LOGGER
+
 
 class CaseRft:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
@@ -452,15 +454,15 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
         takedown_types = kwargs.get("takedown_types", None)
 
         if name is not None:
             self.opencti.log("info", "Creating Case Rft {" + name + "}.")
@@ -525,15 +527,15 @@
                 + stix_object_or_stix_relationship_id
                 + "} to CaseRft {"
                 + id
                 + "}",
             )
             query = """
                mutation CaseRftEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput) {
-                   caseRftEdit(id: $id) {
+                   stixDomainObjectEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
             self.opencti.query(
@@ -574,15 +576,15 @@
                 + stix_object_or_stix_relationship_id
                 + "} to CaseRft {"
                 + id
                 + "}",
             )
             query = """
                mutation CaseRftEditRelationDelete($id: ID!, $toId: StixRef!, $relationship_type: String!) {
-                   caseRftEdit(id: $id) {
+                   stixDomainObjectEdit(id: $id) {
                         relationDelete(toId: $toId, relationship_type: $relationship_type) {
                             id
                         }
                    }
                }
             """
             self.opencti.query(
@@ -629,32 +631,32 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 objects=extras["object_ids"] if "object_ids" in extras else [],
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 takedown_types=stix_object["takedown_types"]
                 if "takedown_types" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 objectOrganization=stix_object["granted_refs"]
@@ -662,7 +664,23 @@
                 else None,
                 update=update,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_caseRft] Missing parameters: stixObject"
             )
+
+    def delete(self, **kwargs):
+        id = kwargs.get("id", None)
+        if id is not None:
+            LOGGER.info("Deleting Case RFT {%s}.", id)
+            query = """
+                 mutation CaseRFTDelete($id: ID!) {
+                     stixDomainObjectEdit(id: $id) {
+                         delete
+                     }
+                 }
+             """
+            self.opencti.query(query, {"id": id})
+        else:
+            LOGGER.error("[opencti_case_rft] Missing parameters: id")
+            return None
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_channel.py` & `pycti-5.8.0/pycti/entities/opencti_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,22 +276,22 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         channel_types = kwargs.get("channel_types", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Channel {%s}.", name)
             query = """
                 mutation ChannelAdd($input: ChannelAddInput!) {
                     channelAdd(input: $input) {
                         id
                         standard_id
                         entity_type
@@ -355,31 +355,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 channel_types=stix_object["channel_types"]
                 if "channel_types" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_course_of_action.py` & `pycti-5.8.0/pycti/entities/opencti_course_of_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,25 +259,25 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         x_opencti_aliases = kwargs.get("x_opencti_aliases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         x_mitre_id = kwargs.get("x_mitre_id", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Course Of Action {%s}.", name)
             query = """
-                mutation CourseOfActionAdd($input: CourseOfActionAddInput) {
+                mutation CourseOfActionAdd($input: CourseOfActionAddInput!) {
                     courseOfActionAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -367,31 +367,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 x_opencti_aliases=self.opencti.stix2.pick_aliases(stix_object),
                 x_mitre_id=x_mitre_id,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_data_component.py` & `pycti-5.8.0/pycti/entities/opencti_data_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,22 +275,22 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         dataSource = kwargs.get("dataSource", None)
         aliases = kwargs.get("aliases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             self.opencti.log("info", "Creating Data Component {" + name + "}.")
             self.opencti.log("info", "Creating Data Component {" + str(kwargs) + "}.")
             query = """
                 mutation DataComponentAdd($input: DataComponentAddInput!) {
                     dataComponentAdd(input: $input) {
                         id
                         standard_id
@@ -373,31 +373,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 dataSource=stix_object["dataSource"]
                 if "dataSource" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_data_source.py` & `pycti-5.8.0/pycti/entities/opencti_data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,23 +259,23 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         platforms = kwargs.get("platforms", None)
         collection_layers = kwargs.get("collection_layers", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             self.opencti.log("info", "Creating Data Source {" + name + "}.")
             self.opencti.log("info", "Creating Data Source {" + str(kwargs) + "}.")
             query = """
                 mutation DataSourceAdd($input: DataSourceAddInput!) {
                     dataSourceAdd(input: $input) {
                         id
                         standard_id
@@ -359,31 +359,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 platforms=stix_object["platforms"]
                 if "platforms" in stix_object
                 else None,
                 collection_layers=stix_object["collection_layers"]
                 if "collection_layers" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_event.py` & `pycti-5.8.0/pycti/entities/opencti_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,23 +278,23 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         start_time = kwargs.get("start_time", None)
         stop_time = kwargs.get("stop_time", None)
         event_types = kwargs.get("event_types", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Event {%s}.", name)
             query = """
                 mutation EventAdd($input: EventAddInput!) {
                     eventAdd(input: $input) {
                         id
                         standard_id
                         entity_type
@@ -359,31 +359,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 event_types=stix_object["event_types"]
                 if "event_types" in stix_object
                 else None,
                 start_time=stix_object["start_time"]
                 if "start_time" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_external_reference.py` & `pycti-5.8.0/pycti/entities/opencti_external_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
         if source_name is not None or url is not None:
             LOGGER.info("Creating External Reference {%s}.", source_name)
             query = (
                 """
-                mutation ExternalReferenceAdd($input: ExternalReferenceAddInput) {
+                mutation ExternalReferenceAdd($input: ExternalReferenceAddInput!) {
                     externalReferenceAdd(input: $input) {
                         """
                 + self.properties
                 + """
                     }
                 }
             """
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_feedback.py` & `pycti-5.8.0/pycti/entities/opencti_feedback.py`

 * *Files 3% similar despite different names*

```diff
@@ -456,15 +456,15 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         rating = kwargs.get("rating", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             self.opencti.log("info", "Creating Feedback {" + name + "}.")
@@ -512,24 +512,28 @@
     def update_field(self, **kwargs):
         LOGGER.info("Updating Feedback {%s}.", json.dumps(kwargs))
         id = kwargs.get("id", None)
         input = kwargs.get("input", None)
         if id is not None and input is not None:
             query = """
                         mutation FeedbackEdit($id: ID!, $input: [EditInput]!) {
-                           feedbackFieldPatch(id: $id, input: $input) {
-                                id
-                                standard_id
-                                entity_type
+                           stixDomainObjectEdit(id: $id) {
+                                fieldPatch(input: $input) {
+                                    id
+                                    ... on Feedback {
+                                        name
+                                        description 
+                                    }
+                               }
                            }
                         }
                     """
             result = self.opencti.query(query, {"id": id, "input": input})
             return self.opencti.process_multiple_fields(
-                result["data"]["feedbackFieldPatch"]
+                result["data"]["stixDomainObjectEdit"]["fieldPatch"]
             )
         else:
             LOGGER.error("[opencti_feedback] Missing parameters: id and key and value")
             return None
 
         """
         Add a Stix-Entity object to Feedback object (object_refs)
@@ -551,16 +555,18 @@
                 + stix_object_or_stix_relationship_id
                 + "} to Feedback {"
                 + id
                 + "}",
             )
             query = """
                mutation FeedbackEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput!) {
-                    feedbackRelationAdd(id: $id, input: $input) {
-                        id
+                    stixDomainObjectEdit(id: $id) {
+                        relationAdd(input: $input) {
+                            id
+                        }
                     }
                }
             """
             self.opencti.query(
                 query,
                 {
                     "id": id,
@@ -598,16 +604,18 @@
                 + stix_object_or_stix_relationship_id
                 + "} to Feedback {"
                 + id
                 + "}",
             )
             query = """
                mutation FeedbackEditRelationDelete($id: ID!, $toId: StixRef!, $relationship_type: String!) {
-                    feedbackRelationDelete(id: $id, toId: $toId, relationship_type: $relationship_type) {
-                        id
+                    stixDomainObjectEdit(id: $id) {
+                        relationDelete(toId: $toId, relationship_type: $relationship_type) {
+                            id
+                        }
                     }
                }
             """
             self.opencti.query(
                 query,
                 {
                     "id": id,
@@ -651,38 +659,54 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 objects=extras["object_ids"] if "object_ids" in extras else [],
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 rating=stix_object["rating"] if "rating" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_feedback] Missing parameters: stixObject"
             )
+
+    def delete(self, **kwargs):
+        id = kwargs.get("id", None)
+        if id is not None:
+            LOGGER.info("Deleting Feedback {%s}.", id)
+            query = """
+                 mutation FeedbackDelete($id: ID!) {
+                     stixDomainObjectEdit(id: $id) {
+                         delete
+                     }
+                 }
+             """
+            self.opencti.query(query, {"id": id})
+        else:
+            LOGGER.error("[opencti_feedback] Missing parameters: id")
+            return None
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_grouping.py` & `pycti-5.8.0/pycti/entities/opencti_grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,21 +431,21 @@
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
         context = kwargs.get("context", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         x_opencti_aliases = kwargs.get("x_opencti_aliases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None and context is not None:
+        if name is not None and context is not None:
             LOGGER.info("Creating Grouping {%s}.", name)
             query = """
                 mutation GroupingAdd($input: GroupingAddInput!) {
                     groupingAdd(input: $input) {
                         id
                         standard_id
                         entity_type
@@ -598,33 +598,33 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 objects=extras["object_ids"] if "object_ids" in extras else [],
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 context=stix_object["context"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 x_opencti_aliases=self.opencti.stix2.pick_aliases(stix_object),
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_identity.py` & `pycti-5.8.0/pycti/entities/opencti_identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,26 +268,26 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         contact_information = kwargs.get("contact_information", None)
         roles = kwargs.get("roles", None)
         x_opencti_aliases = kwargs.get("x_opencti_aliases", None)
         x_opencti_organization_type = kwargs.get("x_opencti_organization_type", None)
         x_opencti_reliability = kwargs.get("x_opencti_reliability", None)
         x_opencti_firstname = kwargs.get("x_opencti_firstname", None)
         x_opencti_lastname = kwargs.get("x_opencti_lastname", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
-        if type is not None and name is not None and description is not None:
+        if type is not None and name is not None:
             LOGGER.info("Creating Identity {%s}.", name)
             input_variables = {
                 "stix_id": stix_id,
                 "createdBy": created_by,
                 "objectMarking": object_marking,
                 "objectLabel": object_label,
                 "externalReferences": external_references,
@@ -302,15 +302,15 @@
                 "roles": roles,
                 "x_opencti_aliases": x_opencti_aliases,
                 "x_opencti_stix_ids": x_opencti_stix_ids,
                 "update": update,
             }
             if type == IdentityTypes.ORGANIZATION.value:
                 query = """
-                    mutation OrganizationAdd($input: OrganizationAddInput) {
+                    mutation OrganizationAdd($input: OrganizationAddInput!) {
                         organizationAdd(input: $input) {
                             id
                             standard_id
                             entity_type
                             parent_types
                         }
                     }
@@ -318,29 +318,29 @@
                 input_variables[
                     "x_opencti_organization_type"
                 ] = x_opencti_organization_type
                 input_variables["x_opencti_reliability"] = x_opencti_reliability
                 result_data_field = "organizationAdd"
             elif type == IdentityTypes.INDIVIDUAL.value:
                 query = """
-                    mutation IndividualAdd($input: IndividualAddInput) {
+                    mutation IndividualAdd($input: IndividualAddInput!) {
                         individualAdd(input: $input) {
                             id
                             standard_id
                             entity_type
                             parent_types
                         }
                     }
                 """
                 input_variables["x_opencti_firstname"] = x_opencti_firstname
                 input_variables["x_opencti_lastname"] = x_opencti_lastname
                 result_data_field = "individualAdd"
             else:
                 query = """
-                    mutation IdentityAdd($input: IdentityAddInput) {
+                    mutation IdentityAdd($input: IdentityAddInput!) {
                         identityAdd(input: $input) {
                             id
                             standard_id
                             entity_type
                             parent_types
                         }
                     }
@@ -418,34 +418,34 @@
                 type=type,
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
-                else [],
+                else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 contact_information=self.opencti.stix2.convert_markdown(
                     stix_object["contact_information"]
                 )
                 if "contact_information" in stix_object
                 else None,
                 roles=stix_object["roles"] if "roles" in stix_object else None,
                 x_opencti_aliases=self.opencti.stix2.pick_aliases(stix_object),
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_incident.py` & `pycti-5.8.0/pycti/entities/opencti_incident.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,30 +259,30 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         first_seen = kwargs.get("first_seen", None)
         last_seen = kwargs.get("last_seen", None)
         objective = kwargs.get("objective", None)
         incident_type = kwargs.get("incident_type", None)
         severity = kwargs.get("severity", None)
         source = kwargs.get("source", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Incident {%s}.", name)
             query = """
-                mutation IncidentAdd($input: IncidentAddInput) {
+                mutation IncidentAdd($input: IncidentAddInput!) {
                     incidentAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                }
@@ -348,31 +348,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 objective=stix_object["objective"]
                 if "objective" in stix_object
                 else None,
                 first_seen=stix_object["first_seen"]
                 if "first_seen" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_indicator.py` & `pycti-5.8.0/pycti/entities/opencti_indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
             and pattern_type is not None
             and x_opencti_main_observable_type is not None
         ):
             if x_opencti_main_observable_type == "File":
                 x_opencti_main_observable_type = "StixFile"
             LOGGER.info("Creating Indicator {%s}.", name)
             query = """
-                mutation IndicatorAdd($input: IndicatorAddInput) {
+                mutation IndicatorAdd($input: IndicatorAddInput!) {
                     indicatorAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                         observables {
                             edges {
@@ -534,18 +534,18 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
@@ -559,15 +559,15 @@
                 name=stix_object["name"]
                 if "name" in stix_object
                 else stix_object["pattern"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 indicator_types=stix_object["indicator_types"]
                 if "indicator_types" in stix_object
                 else None,
                 valid_from=stix_object["valid_from"]
                 if "valid_from" in stix_object
                 else None,
                 valid_until=stix_object["valid_until"]
@@ -598,8 +598,8 @@
                 else False,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error("[opencti_indicator] Missing parameters: stixObject")
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_infrastructure.py` & `pycti-5.8.0/pycti/entities/opencti_infrastructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         kill_chain_phases = kwargs.get("killChainPhases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             LOGGER.info("Creating Infrastructure {%s}.", name)
             query = """
-                mutation InfrastructureAdd($input: InfrastructureAddInput) {
+                mutation InfrastructureAdd($input: InfrastructureAddInput!) {
                     infrastructureAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -395,31 +395,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 infrastructure_types=stix_object["infrastructure_types"]
                 if "infrastructure_types" in stix_object
                 else None,
                 first_seen=stix_object["first_seen"]
                 if "first_seen" in stix_object
                 else None,
@@ -431,8 +431,8 @@
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error("[opencti_infrastructure] Missing parameters: stixObject")
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_intrusion_set.py` & `pycti-5.8.0/pycti/entities/opencti_intrusion_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,30 +259,30 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         first_seen = kwargs.get("first_seen", None)
         last_seen = kwargs.get("last_seen", None)
         goals = kwargs.get("goals", None)
         resource_level = kwargs.get("resource_level", None)
         primary_motivation = kwargs.get("primary_motivation", None)
         secondary_motivations = kwargs.get("secondary_motivations", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Intrusion-Set {%s}.", name)
             query = """
-                mutation IntrusionSetAdd($input: IntrusionSetAddInput) {
+                mutation IntrusionSetAdd($input: IntrusionSetAddInput!) {
                     intrusionSetAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -352,31 +352,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 first_seen=stix_object["first_seen"]
                 if "first_seen" in stix_object
                 else None,
                 last_seen=stix_object["last_seen"]
                 if "last_seen" in stix_object
                 else None,
@@ -395,8 +395,8 @@
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error("[opencti_intrusion_set] Missing parameters: stixObject")
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.8.0/pycti/entities/opencti_kill_chain_phase.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         x_opencti_order = kwargs.get("x_opencti_order", 0)
         update = kwargs.get("update", False)
 
         if kill_chain_name is not None and phase_name is not None:
             LOGGER.info("Creating Kill-Chain-Phase {%s}.", phase_name)
             query = (
                 """
-                mutation KillChainPhaseAdd($input: KillChainPhaseAddInput) {
+                mutation KillChainPhaseAdd($input: KillChainPhaseAddInput!) {
                     killChainPhaseAdd(input: $input) {
                         """
                 + self.properties
                 + """
                     }
                 }
             """
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_label.py` & `pycti-5.8.0/pycti/entities/opencti_label.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
         if value is not None:
             LOGGER.info("Creating Label {%s}.", value)
             query = (
                 """
-                mutation LabelAdd($input: LabelAddInput) {
+                mutation LabelAdd($input: LabelAddInput!) {
                     labelAdd(input: $input) {
                         """
                 + self.properties
                 + """
                     }
                 }
             """
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_language.py` & `pycti-5.8.0/pycti/entities/opencti_language.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,18 +347,18 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_location.py` & `pycti-5.8.0/pycti/entities/opencti_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -263,26 +263,26 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         latitude = kwargs.get("latitude", None)
         longitude = kwargs.get("longitude", None)
         precision = kwargs.get("precision", None)
         x_opencti_aliases = kwargs.get("x_opencti_aliases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             LOGGER.info("Creating Location {%s}.", name)
             query = """
-                mutation LocationAdd($input: LocationAddInput) {
+                mutation LocationAdd($input: LocationAddInput!) {
                     locationAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -367,34 +367,34 @@
                 type=type,
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
-                else [],
+                else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=name,
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 latitude=stix_object["latitude"] if "latitude" in stix_object else None,
                 longitude=stix_object["longitude"]
                 if "longitude" in stix_object
                 else None,
                 precision=stix_object["precision"]
                 if "precision" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_malware.py` & `pycti-5.8.0/pycti/entities/opencti_malware.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,32 +297,32 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         malware_types = kwargs.get("malware_types", None)
         is_family = kwargs.get("is_family", None)
         first_seen = kwargs.get("first_seen", None)
         last_seen = kwargs.get("last_seen", None)
         architecture_execution_envs = kwargs.get("architecture_execution_envs", None)
         implementation_languages = kwargs.get("implementation_languages", None)
         capabilities = kwargs.get("capabilities", None)
         kill_chain_phases = kwargs.get("killChainPhases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Malware {%s}.", name)
             query = """
-                mutation MalwareAdd($input: MalwareAddInput) {
+                mutation MalwareAdd($input: MalwareAddInput!) {
                     malwareAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -390,31 +390,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 malware_types=stix_object["malware_types"]
                 if "malware_types" in stix_object
                 else None,
                 is_family=stix_object["is_family"]
                 if "is_family" in stix_object
                 else False,
@@ -441,8 +441,8 @@
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error("[opencti_malware] Missing parameters: stixObject")
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_marking_definition.py` & `pycti-5.8.0/pycti/entities/opencti_marking_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         x_opencti_color = kwargs.get("x_opencti_color", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
         if definition is not None and definition_type is not None:
             query = (
                 """
-                mutation MarkingDefinitionAdd($input: MarkingDefinitionAddInput) {
+                mutation MarkingDefinitionAdd($input: MarkingDefinitionAddInput!) {
                     markingDefinitionAdd(input: $input) {
                         """
                 + self.properties
                 + """
                     }
                 }
             """
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_narrative.py` & `pycti-5.8.0/pycti/entities/opencti_narrative.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,22 +276,22 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         narrative_types = kwargs.get("narrative_types", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Narrative {%s}.", name)
             query = """
                 mutation NarrativeAdd($input: NarrativeAddInput!) {
                     narrativeAdd(input: $input) {
                         id
                         standard_id
                         entity_type
@@ -355,31 +355,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 narrative_types=stix_object["narrative_types"]
                 if "narrative_types" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_note.py` & `pycti-5.8.0/pycti/entities/opencti_note.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,15 +428,15 @@
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if content is not None:
             LOGGER.info("Creating Note {%s}.", content)
             query = """
-                mutation NoteAdd($input: NoteAddInput) {
+                mutation NoteAdd($input: NoteAddInput!) {
                     noteAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -588,32 +588,32 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 objects=extras["object_ids"] if "object_ids" in extras else [],
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 abstract=self.opencti.stix2.convert_markdown(stix_object["abstract"])
                 if "abstract" in stix_object
-                else "",
+                else None,
                 content=self.opencti.stix2.convert_markdown(stix_object["content"])
                 if "content" in stix_object
-                else "",
+                else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 authors=stix_object["authors"] if "authors" in stix_object else None,
                 note_types=stix_object["note_types"]
                 if "note_types" in stix_object
                 else None,
@@ -622,8 +622,8 @@
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error("[opencti_note] Missing parameters: stixObject")
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_observed_data.py` & `pycti-5.8.0/pycti/entities/opencti_observed_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         if (
             first_observed is not None
             and last_observed is not None
             and objects is not None
         ):
             LOGGER.info("Creating ObservedData.")
             query = """
-                mutation ObservedDataAdd($input: ObservedDataAddInput) {
+                mutation ObservedDataAdd($input: ObservedDataAddInput!) {
                     observedDataAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -560,15 +560,15 @@
                         if "created_by_id" in extras
                         else None,
                         objectMarking=extras["object_marking_ids"]
                         if "object_marking_ids" in extras
                         else None,
                         objectLabel=extras["object_label_ids"]
                         if "object_label_ids" in extras
-                        else [],
+                        else None,
                         objectOrganization=extras["granted_refs_ids"]
                         if "granted_refs_ids" in extras
                         else None,
                     )
                 )
                 for item in stix_observable_results:
                     object_refs.append(item["standard_id"])
@@ -590,19 +590,19 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 objects=object_refs,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
@@ -622,8 +622,8 @@
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
 
             return observed_data_result
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error("[opencti_observed_data] Missing parameters: stixObject")
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_opinion.py` & `pycti-5.8.0/pycti/entities/opencti_opinion.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,15 +397,15 @@
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if opinion is not None:
             LOGGER.info("Creating Opinion {%s}.", opinion)
             query = """
-                mutation OpinionAdd($input: OpinionAddInput) {
+                mutation OpinionAdd($input: OpinionAddInput!) {
                     opinionAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -583,8 +583,8 @@
                 opinion=stix_object["opinion"] if "opinion" in stix_object else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error("[opencti_opinion] Missing parameters: stixObject")
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_report.py` & `pycti-5.8.0/pycti/entities/opencti_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,25 +455,25 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         report_types = kwargs.get("report_types", None)
         published = kwargs.get("published", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None and published is not None:
+        if name is not None and published is not None:
             LOGGER.info("Creating Report {%s}.", name)
             query = """
-                mutation ReportAdd($input: ReportAddInput) {
+                mutation ReportAdd($input: ReportAddInput!) {
                     reportAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -624,32 +624,32 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 objects=extras["object_ids"] if "object_ids" in extras else [],
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 report_types=stix_object["report_types"]
                 if "report_types" in stix_object
                 else None,
                 published=stix_object["published"]
                 if "published" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_stix.py` & `pycti-5.8.0/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/entities/opencti_stix_core_object.py` & `pycti-5.8.0/pycti/entities/opencti_stix_core_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,32 @@
                             x_opencti_order
                             created
                             modified
                         }
                     }
                 }
             }
+            ... on MalwareAnalysis {
+                product
+                version
+                hostVm
+                operatingSystem
+                installedSoftware
+                configuration_version
+                modules
+                analysis_engine_version
+                analysis_definition_version
+                submitted
+                analysis_started
+                analysis_ended
+                result_name
+                result
+                analysisSco
+                sample
+            }
             ... on ThreatActor {
                 name
                 description
                 aliases
                 threat_actor_types
                 first_seen
                 last_seen
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.8.0/pycti/entities/opencti_stix_core_relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -1122,15 +1122,15 @@
                 toId=target_ref,
                 stix_id=stix_relation["id"],
                 relationship_type=stix_relation["relationship_type"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_relation["description"]
                 )
                 if "description" in stix_relation
-                else "",
+                else None,
                 start_time=stix_relation["start_time"]
                 if "start_time" in stix_relation
                 else default_date,
                 stop_time=stix_relation["stop_time"]
                 if "stop_time" in stix_relation
                 else default_date,
                 revoked=stix_relation["revoked"]
@@ -1150,21 +1150,23 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 killChainPhases=extras["kill_chain_phases_ids"]
                 if "kill_chain_phases_ids" in extras
                 else None,
                 objectOrganization=stix_relation["granted_refs"]
                 if "granted_refs" in stix_relation
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error(
+                "[opencti_stix_core_relationship] Missing parameters: stixObject"
+            )
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.8.0/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.8.0/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.8.0/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.8.0/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.8.0/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/entities/opencti_threat_actor.py` & `pycti-5.8.0/pycti/entities/opencti_threat_actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,33 +310,33 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         threat_actor_types = kwargs.get("threat_actor_types", None)
         first_seen = kwargs.get("first_seen", None)
         last_seen = kwargs.get("last_seen", None)
         goals = kwargs.get("goals", None)
         sophistication = kwargs.get("sophistication", None)
         resource_level = kwargs.get("resource_level", None)
         primary_motivation = kwargs.get("primary_motivation", None)
         secondary_motivations = kwargs.get("secondary_motivations", None)
         personal_motivations = kwargs.get("personal_motivations", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Threat-Actor {%s}.", name)
             query = """
-                mutation ThreatActorAdd($input: ThreatActorAddInput) {
+                mutation ThreatActorAdd($input: ThreatActorAddInput!) {
                     threatActorAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -409,31 +409,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 threat_actor_types=stix_object["threat_actor_types"]
                 if "threat_actor_types" in stix_object
                 else None,
                 first_seen=stix_object["first_seen"]
                 if "first_seen" in stix_object
                 else None,
@@ -461,8 +461,8 @@
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
+            LOGGER.error("[opencti_threat_actor] Missing parameters: stixObject")
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_tool.py` & `pycti-5.8.0/pycti/entities/opencti_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,26 +291,26 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         tool_types = kwargs.get("tool_types", None)
         tool_version = kwargs.get("tool_version", None)
         kill_chain_phases = kwargs.get("killChainPhases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Tool {%s}.", name)
             query = """
-                mutation ToolAdd($input: ToolAddInput) {
+                mutation ToolAdd($input: ToolAddInput!) {
                     toolAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -368,31 +368,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 tool_types=stix_object["tool_types"]
                 if "tool_types" in stix_object
                 else None,
                 tool_version=stix_object["tool_version"]
                 if "tool_version" in stix_object
                 else None,
```

### Comparing `pycti-5.7.post576/pycti/entities/opencti_vocabulary.py` & `pycti-5.8.0/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/entities/opencti_vulnerability.py` & `pycti-5.8.0/pycti/entities/opencti_vulnerability.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,33 +282,33 @@
         external_references = kwargs.get("externalReferences", None)
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
-        description = kwargs.get("description", "")
+        description = kwargs.get("description", None)
         x_opencti_aliases = kwargs.get("x_opencti_aliases", None)
         x_opencti_base_score = kwargs.get("x_opencti_base_score", None)
         x_opencti_base_severity = kwargs.get("x_opencti_base_severity", None)
         x_opencti_attack_vector = kwargs.get("x_opencti_attack_vector", None)
         x_opencti_integrity_impact = kwargs.get("x_opencti_integrity_impact", None)
         x_opencti_availability_impact = kwargs.get(
             "x_opencti_availability_impact", None
         )
         x_opencti_confidentiality_impact = kwargs.get(
             "x_opencti_confidentiality_impact", None
         )
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
-        if name is not None and description is not None:
+        if name is not None:
             LOGGER.info("Creating Vulnerability {%s}.", name)
             query = """
-                mutation VulnerabilityAdd($input: VulnerabilityAddInput) {
+                mutation VulnerabilityAdd($input: VulnerabilityAddInput!) {
                     vulnerabilityAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
@@ -411,31 +411,31 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 revoked=stix_object["revoked"] if "revoked" in stix_object else None,
                 confidence=stix_object["confidence"]
                 if "confidence" in stix_object
                 else None,
                 lang=stix_object["lang"] if "lang" in stix_object else None,
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
-                else "",
+                else None,
                 x_opencti_aliases=stix_object["x_opencti_aliases"]
                 if "x_opencti_aliases" in stix_object
                 else None,
                 x_opencti_base_score=stix_object["x_opencti_base_score"]
                 if "x_opencti_base_score" in stix_object
                 else None,
                 x_opencti_base_severity=stix_object["x_opencti_base_severity"]
```

### Comparing `pycti-5.7.post576/pycti/utils/constants.py` & `pycti-5.8.0/pycti/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,12 +105,14 @@
     ENCAPSULATES = "encapsulates"
     OPENED_CONNECTION = "opened-connection"
     CHILD = "child"
     BODY_MULTIPART = "body-multipart"
     VALUES = "values"
     LINKED = "x_opencti_linked-to"
     SERVICE_DDL = "service-dll"
+    INSTALLED_SOFTWARE = "installed-software"
+    RELATION_ANALYSIS_SCO = "analysis-sco"
 
     @classmethod
     def has_value(cls, value):
         lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
         return value.lower() in lower_attr
```

### Comparing `pycti-5.7.post576/pycti/utils/opencti_stix2.py` & `pycti-5.8.0/pycti/utils/opencti_stix2.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     :param opencti: OpenCTI instance
     """
 
     def __init__(self, opencti):
         self.opencti = opencti
         self.stix2_update = OpenCTIStix2Update(opencti)
         self.mapping_cache = LRUCache(maxsize=50000)
+        self.mapping_cache_permanent = {}
 
     ######### UTILS
     # region utils
     def unknown_type(self, stix_object: Dict) -> None:
         API_LOGGER.error(
             'Unknown object type "%s", doing nothing...', stix_object["type"]
         )
@@ -295,52 +296,56 @@
             stix_object["object_marking_refs"]
             if "object_marking_refs" in stix_object
             else []
         )
 
         # Open vocabularies
         object_open_vocabularies = {}
-        if self.mapping_cache.get("vocabularies_definition_fields") is None:
-            self.mapping_cache["vocabularies_definition_fields"] = []
+        if self.mapping_cache_permanent.get("vocabularies_definition_fields") is None:
+            self.mapping_cache_permanent["vocabularies_definition_fields"] = []
             query = """
                     query getVocabCategories {
                       vocabularyCategories {
                         key
                         fields{
                           key
                           required
                         }
                       }
                     }
                 """
             result = self.opencti.query(query)
             for category in result["data"]["vocabularyCategories"]:
                 for field in category["fields"]:
-                    self.mapping_cache["vocabularies_definition_fields"].append(field)
-                    self.mapping_cache["category_" + field["key"]] = category["key"]
+                    self.mapping_cache_permanent[
+                        "vocabularies_definition_fields"
+                    ].append(field)
+                    self.mapping_cache_permanent["category_" + field["key"]] = category[
+                        "key"
+                    ]
         if any(
             field["key"] in stix_object
-            for field in self.mapping_cache["vocabularies_definition_fields"]
+            for field in self.mapping_cache_permanent["vocabularies_definition_fields"]
         ):
-            for f in self.mapping_cache["vocabularies_definition_fields"]:
+            for f in self.mapping_cache_permanent["vocabularies_definition_fields"]:
                 if stix_object.get(f["key"]) is None:
                     continue
                 if isinstance(stix_object.get(f["key"]), list):
                     object_open_vocabularies[f["key"]] = []
                     for vocab in stix_object[f["key"]]:
                         object_open_vocabularies[f["key"]].append(
                             self.opencti.vocabulary.handle_vocab(
-                                vocab, self.mapping_cache, field=f
+                                vocab, self.mapping_cache_permanent, field=f
                             )["name"]
                         )
                 else:
                     object_open_vocabularies[
                         f["key"]
                     ] = self.opencti.vocabulary.handle_vocab(
-                        stix_object[f["key"]], self.mapping_cache, field=f
+                        stix_object[f["key"]], self.mapping_cache_permanent, field=f
                     )[
                         "name"
                     ]
 
         # Object Labels
         object_label_ids = []
         if (
@@ -771,27 +776,29 @@
             "note": self.opencti.note.import_from_stix2,
             "observed-data": self.opencti.observed_data.import_from_stix2,
             "opinion": self.opencti.opinion.import_from_stix2,
             "report": self.opencti.report.import_from_stix2,
             "grouping": self.opencti.grouping.import_from_stix2,
             "case-rfi": self.opencti.case_rfi.import_from_stix2,
             "case-rft": self.opencti.case_rft.import_from_stix2,
+            "task": self.opencti.task.import_from_stix2,
             "case-incident": self.opencti.case_incident.import_from_stix2,
             "feedback": self.opencti.feedback.import_from_stix2,
             "course-of-action": self.opencti.course_of_action.import_from_stix2,
             "data-component": self.opencti.data_component.import_from_stix2,
             "x-mitre-data-component": self.opencti.data_component.import_from_stix2,
             "data-source": self.opencti.data_source.import_from_stix2,
             "x-mitre-data-source": self.opencti.data_source.import_from_stix2,
             "identity": self.opencti.identity.import_from_stix2,
             "indicator": self.opencti.indicator.import_from_stix2,
             "infrastructure": self.opencti.infrastructure.import_from_stix2,
             "intrusion-set": self.opencti.intrusion_set.import_from_stix2,
             "location": self.opencti.location.import_from_stix2,
             "malware": self.opencti.malware.import_from_stix2,
+            "malware-analysis": self.opencti.malware_analysis.import_from_stix2,
             "threat-actor": self.opencti.threat_actor.import_from_stix2,
             "tool": self.opencti.tool.import_from_stix2,
             "narrative": self.opencti.narrative.import_from_stix2,
             "vulnerability": self.opencti.vulnerability.import_from_stix2,
             "incident": self.opencti.incident.import_from_stix2,
         }
         do_import = importer.get(
@@ -898,18 +905,18 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else [],
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 createIndicator=stix_object["x_opencti_create_indicator"]
                 if "x_opencti_create_indicator" in stix_object
                 else None,
                 objectOrganization=extras["granted_refs_ids"]
                 if "granted_refs_ids" in extras
                 else [],
                 update=update,
@@ -921,18 +928,18 @@
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else [],
                 objectLabel=extras["object_label_ids"]
                 if "object_label_ids" in extras
-                else [],
+                else None,
                 externalReferences=extras["external_references_ids"]
                 if "external_references_ids" in extras
-                else [],
+                else None,
                 objectOrganization=extras["granted_refs_ids"]
                 if "granted_refs_ids" in extras
                 else [],
                 update=update,
             )
         if stix_observable_result is not None:
             # Add files
@@ -1195,18 +1202,18 @@
             else 15,
             createdBy=extras["created_by_id"] if "created_by_id" in extras else None,
             objectMarking=extras["object_marking_ids"]
             if "object_marking_ids" in extras
             else [],
             objectLabel=extras["object_label_ids"]
             if "object_label_ids" in extras
-            else [],
+            else None,
             externalReferences=extras["external_references_ids"]
             if "external_references_ids" in extras
-            else [],
+            else None,
             objectOrganization=extras["granted_refs_ids"]
             if "granted_refs_ids" in extras
             else [],
             update=update,
             ignore_dates=stix_sighting["x_opencti_ignore_dates"]
             if "x_opencti_ignore_dates" in stix_sighting
             else None,
@@ -1536,14 +1543,19 @@
                 ):
                     entity["object_refs"].append(entity_object["standard_id"])
                 elif (
                     entity["type"] == "case-rft"
                     and "stix-ref-relationship" not in entity_object["parent_types"]
                 ):
                     entity["object_refs"].append(entity_object["standard_id"])
+                elif (
+                    entity["type"] == "task"
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
+                    entity["object_refs"].append(entity_object["standard_id"])
         if "objects" in entity:
             del entity["objects"]
             del entity["objectsIds"]
         # Stix Sighting Relationship
         if entity["type"] == "stix-sighting-relationship":
             entity["type"] = "sighting"
             entity["count"] = entity["attribute_count"]
@@ -1608,39 +1620,46 @@
 
         # StixRefRelationship
         stix_nested_ref_relationships = self.opencti.stix_nested_ref_relationship.list(
             fromId=entity["x_opencti_id"]
         )
         for stix_nested_ref_relationship in stix_nested_ref_relationships:
             if "standard_id" in stix_nested_ref_relationship["to"]:
-                if MultipleRefRelationship.has_value(
+                # dirty fix because the sample and operating-system ref are not multiple for a Malware Analysis
+                # will be replaced by a proper toStix converter in the back
+                if not MultipleRefRelationship.has_value(
                     stix_nested_ref_relationship["relationship_type"]
+                ) or (
+                    entity["type"] == "malware-analysis"
+                    and stix_nested_ref_relationship["relationship_type"]
+                    in ["operating-system", "sample"]
                 ):
                     key = (
                         stix_nested_ref_relationship["relationship_type"]
                         .replace("obs_", "")
                         .replace("-", "_")
+                        + "_ref"
+                    )
+                    entity[key] = stix_nested_ref_relationship["to"]["standard_id"]
+
+                else:
+                    key = (
+                        stix_nested_ref_relationship["relationship_type"]
+                        .replace("obs_", "")
+                        .replace("-", "_")
                         + "_refs"
                     )
-                    if key in entity:
+                    if key in entity and isinstance(entity[key], list):
                         entity[key].append(
                             stix_nested_ref_relationship["to"]["standard_id"]
                         )
                     else:
                         entity[key] = [
                             stix_nested_ref_relationship["to"]["standard_id"]
                         ]
-                else:
-                    key = (
-                        stix_nested_ref_relationship["relationship_type"]
-                        .replace("obs_", "")
-                        .replace("-", "_")
-                        + "_ref"
-                    )
-                    entity[key] = stix_nested_ref_relationship["to"]["standard_id"]
         result.append(entity)
 
         if mode == "simple":
             return result
         elif mode == "full":
             uuids = [entity["id"]]
             for x in result:
@@ -1763,24 +1782,26 @@
                 "Observed-Data": self.opencti.observed_data.read,
                 "Opinion": self.opencti.opinion.read,
                 "Report": self.opencti.report.read,
                 "Case-Incident": self.opencti.case_incident.read,
                 "Feedback": self.opencti.feedback.read,
                 "Case-Rfi": self.opencti.case_rfi.read,
                 "Case-Rft": self.opencti.case_rft.read,
+                "Task": self.opencti.task.read,
                 "Course-Of-Action": self.opencti.course_of_action.read,
                 "Data-Component": self.opencti.data_component.read,
                 "Data-Source": self.opencti.data_source.read,
                 "Identity": self.opencti.identity.read,
                 "Indicator": self.opencti.indicator.read,
                 "Infrastructure": self.opencti.infrastructure.read,
                 "Intrusion-Set": self.opencti.intrusion_set.read,
                 "Location": self.opencti.location.read,
                 "Language": self.opencti.language.read,
                 "Malware": self.opencti.malware.read,
+                "Malware-Analysis": self.opencti.malware_analysis.read,
                 "Threat-Actor": self.opencti.threat_actor.read,
                 "Tool": self.opencti.tool.read,
                 "Vulnerability": self.opencti.vulnerability.read,
                 "Incident": self.opencti.incident.read,
                 "Stix-Core-Object": self.opencti.stix_core_object.read,
                 "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.read,
                 "Stix-Domain-Object": self.opencti.stix_domain_object.read,
@@ -1904,14 +1925,18 @@
             else None
         )
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
         }
+
+        if entity_type == "StixFile":
+            entity_type = "File"
+
         # Map types
         if IdentityTypes.has_value(entity_type):
             entity_type = "Identity"
         if LocationTypes.has_value(entity_type):
             entity_type = "Location"
 
         # Reader
@@ -1925,24 +1950,26 @@
             "Opinion": self.opencti.opinion.read,
             "Report": self.opencti.report.read,
             "Grouping": self.opencti.grouping.read,
             "Case-Incident": self.opencti.case_incident.read,
             "Feedback": self.opencti.feedback.read,
             "Case-Rfi": self.opencti.case_rfi.read,
             "Case-Rft": self.opencti.case_rft.read,
+            "Task": self.opencti.task.read,
             "Course-Of-Action": self.opencti.course_of_action.read,
             "Data-Component": self.opencti.data_component.read,
             "Data-Source": self.opencti.data_source.read,
             "Identity": self.opencti.identity.read,
             "Indicator": self.opencti.indicator.read,
             "Infrastructure": self.opencti.infrastructure.read,
             "Intrusion-Set": self.opencti.intrusion_set.read,
             "Location": self.opencti.location.read,
             "Language": self.opencti.language.read,
             "Malware": self.opencti.malware.read,
+            "Malware-Analysis": self.opencti.malware_analysis.read,
             "Threat-Actor": self.opencti.threat_actor.read,
             "Tool": self.opencti.tool.read,
             "Narrative": self.opencti.narrative.read,
             "Vulnerability": self.opencti.vulnerability.read,
             "Incident": self.opencti.incident.read,
             "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.read,
             "stix-core-relationship": self.opencti.stix_core_relationship.read,
@@ -2025,27 +2052,33 @@
                         "key": "entity_type",
                         "values": [
                             "Report",
                             "Grouping",
                             "Note",
                             "Observed-Data",
                             "Opinion",
+                            "Case-Incident",
+                            "Case-Rfi",
+                            "Case-Rft",
                         ],
                     }
                 )
             else:
                 filters = [
                     {
                         "key": "entity_type",
                         "values": [
                             "Report",
                             "Grouping",
                             "Note",
                             "Observed-Data",
                             "Opinion",
+                            "Case-Incident",
+                            "Case-Rfi",
+                            "Case-Rft",
                         ],
                     }
                 ]
             entity_type = "Stix-Domain-Object"
 
         # List
         lister = {
@@ -2060,24 +2093,26 @@
             "Opinion": self.opencti.opinion.list,
             "Report": self.opencti.report.list,
             "Grouping": self.opencti.grouping.list,
             "Case-Incident": self.opencti.case_incident.list,
             "Feedback": self.opencti.feedback.list,
             "Case-Rfi": self.opencti.case_rfi.list,
             "Case-Rft": self.opencti.case_rft.list,
+            "Task": self.opencti.task.list,
             "Course-Of-Action": self.opencti.course_of_action.list,
             "Data-Component": self.opencti.data_component.list,
             "Data-Source": self.opencti.data_source.list,
             "Identity": self.opencti.identity.list,
             "Indicator": self.opencti.indicator.list,
             "Infrastructure": self.opencti.infrastructure.list,
             "Intrusion-Set": self.opencti.intrusion_set.list,
             "Location": self.opencti.location.list,
             "Language": self.opencti.language.list,
             "Malware": self.opencti.malware.list,
+            "Malware-Analysis": self.opencti.malware_analysis.list,
             "Threat-Actor": self.opencti.threat_actor.list,
             "Tool": self.opencti.tool.list,
             "Narrative": self.opencti.narrative.list,
             "Vulnerability": self.opencti.vulnerability.list,
             "Incident": self.opencti.incident.list,
             "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.list,
             "stix-sighting-relationship": self.opencti.stix_sighting_relationship.list,
@@ -2114,28 +2149,32 @@
                     for x in entity_bundle_filtered:
                         uuids.append(x["id"])
                     bundle["objects"] = bundle["objects"] + entity_bundle_filtered
         return bundle
 
     def export_selected(
         self,
+        entity_type: str,
         entities_list: [str],
         element_id: str = None,
         max_marking_definition: Dict = None,
     ) -> Dict:
         max_marking_definition_entity = (
             self.opencti.marking_definition.read(id=max_marking_definition)
             if max_marking_definition is not None
             else None
         )
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
         }
+        if entity_type == "StixFile":
+            entity_type = "File"
+
         if entities_list is not None:
             uuids = []
             for entity in entities_list:
                 entity_bundle = self.prepare_export(
                     self.generate_export(entity),
                     "simple",
                     max_marking_definition_entity,
```

### Comparing `pycti-5.7.post576/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.8.0/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/utils/opencti_stix2_update.py` & `pycti-5.8.0/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti/utils/opencti_stix2_utils.py` & `pycti-5.8.0/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/pycti.egg-info/PKG-INFO` & `pycti-5.8.0/pycti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.7.post576
+Version: 5.8.0
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.7.post576 Summary: Python API
-client for OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-
-python Author: Filigran Author-email: contact@filigran.io Maintainer: Filigran
-License: Apache Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Information Technology Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Natural Language :: English Classifier: Natural Language :: French Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Topic :: Security Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: doc License-File: LICENSE #
-OpenCTI client for Python [![Website](https://img.shields.io/badge/website-
-opencti.io-blue.svg)](https://www.opencti.io) [![CircleCI](https://
-circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://
-circleci.com/gh/OpenCTI-Platform/client-python/tree/master) [![readthedocs]
-(https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)]
-(https://opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub
-release](https://img.shields.io/github/release/OpenCTI-Platform/client-
-python.svg)](https://github.com/OpenCTI-Platform/client-python/releases/latest)
-[![Number of PyPI downloads](https://img.shields.io/pypi/dm/pycti.svg)](https:/
-/pypi.python.org/pypi/pycti/) [![Slack Status](https://img.shields.io/badge/
-slack-3K%2B%20members-4A154B)](https://community.filigran.io) The official
-OpenCTI Python client helps developers to use the OpenCTI API by providing easy
-to use methods and utils. This client is also used by some OpenCTI components.
-## Install To install the latest Python client library, please use `pip`:
-```bash $ pip3 install pycti ``` ## Local development ```bash # Fork the
-current repository, then clone your fork $ git clone https://github.com/YOUR-
-USERNAME/client-python $ cd client-python $ git remote add upstream https://
-github.com/OpenCTI-Platform/client-python.git # Create a branch for your
-feature/fix $ git checkout -b [branch-name] # Create a virtualenv $ python3 -
-m venv .venv $ source .venv/bin/activate # Install the client-python and
-dependencies for the development and the documentation $ python3 -m pip install
--e .[dev,doc] # Set up the git hook scripts $ pre-commit install # Create your
-feature/fix # Create tests for your changes $ pytest # Push you feature/fix on
-Github $ git add [file(s)] $ git commit -m "[descriptive message]" $ git push
-origin [branch-name] # Open a pull request ``` ### Install the package locally
-```bash $ pip install -e . ``` ## Documentation ### Client usage To learn about
-how to use the OpenCTI Python client and read some examples and cases, refer to
-[the client documentation](https://opencti-client-for-python.readthedocs.io/en/
+Metadata-Version: 2.1 Name: pycti Version: 5.8.0 Summary: Python API client for
+OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
+Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Natural Language :: English
+Classifier: Natural Language :: French Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier: Topic
+:: Security Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: doc License-File: LICENSE # OpenCTI client
+for Python [![Website](https://img.shields.io/badge/website-opencti.io-
+blue.svg)](https://www.opencti.io) [![CircleCI](https://circleci.com/gh/
+OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/
+OpenCTI-Platform/client-python/tree/master) [![readthedocs](https://
+readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://
+opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub release](https:/
+/img.shields.io/github/release/OpenCTI-Platform/client-python.svg)](https://
+github.com/OpenCTI-Platform/client-python/releases/latest) [![Number of PyPI
+downloads](https://img.shields.io/pypi/dm/pycti.svg)](https://pypi.python.org/
+pypi/pycti/) [![Slack Status](https://img.shields.io/badge/slack-
+3K%2B%20members-4A154B)](https://community.filigran.io) The official OpenCTI
+Python client helps developers to use the OpenCTI API by providing easy to use
+methods and utils. This client is also used by some OpenCTI components. ##
+Install To install the latest Python client library, please use `pip`: ```bash
+$ pip3 install pycti ``` ## Local development ```bash # Fork the current
+repository, then clone your fork $ git clone https://github.com/YOUR-USERNAME/
+client-python $ cd client-python $ git remote add upstream https://github.com/
+OpenCTI-Platform/client-python.git # Create a branch for your feature/fix $ git
+checkout -b [branch-name] # Create a virtualenv $ python3 -m venv .venv $
+source .venv/bin/activate # Install the client-python and dependencies for the
+development and the documentation $ python3 -m pip install -e .[dev,doc] # Set
+up the git hook scripts $ pre-commit install # Create your feature/fix # Create
+tests for your changes $ pytest # Push you feature/fix on Github $ git add
+[file(s)] $ git commit -m "[descriptive message]" $ git push origin [branch-
+name] # Open a pull request ``` ### Install the package locally ```bash $ pip
+install -e . ``` ## Documentation ### Client usage To learn about how to use
+the OpenCTI Python client and read some examples and cases, refer to [the
+client documentation](https://opencti-client-for-python.readthedocs.io/en/
 latest/client_usage/getting_started.html). ### API reference To learn about the
 methods available for executing queries and retrieving their answers, refer to
 [the client API Reference](https://opencti-client-for-python.readthedocs.io/en/
 latest/pycti/pycti.html). ## Tests ### Install dependencies ```bash $ pip
 install -r ./test-requirements.txt ``` [pytest](https://docs.pytest.org/en/
 7.2.x/) is used to launch the tests. ### Launch tests #### Prerequisite Your
 OpenCTI API should be running. Your conftest.py should be configured with your
```

### Comparing `pycti-5.7.post576/pycti.egg-info/SOURCES.txt` & `pycti-5.8.0/pycti.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,28 +35,30 @@
 pycti/entities/opencti_infrastructure.py
 pycti/entities/opencti_intrusion_set.py
 pycti/entities/opencti_kill_chain_phase.py
 pycti/entities/opencti_label.py
 pycti/entities/opencti_language.py
 pycti/entities/opencti_location.py
 pycti/entities/opencti_malware.py
+pycti/entities/opencti_malware_analysis.py
 pycti/entities/opencti_marking_definition.py
 pycti/entities/opencti_narrative.py
 pycti/entities/opencti_note.py
 pycti/entities/opencti_observed_data.py
 pycti/entities/opencti_opinion.py
 pycti/entities/opencti_report.py
 pycti/entities/opencti_stix.py
 pycti/entities/opencti_stix_core_object.py
 pycti/entities/opencti_stix_core_relationship.py
 pycti/entities/opencti_stix_cyber_observable.py
 pycti/entities/opencti_stix_domain_object.py
 pycti/entities/opencti_stix_nested_ref_relationship.py
 pycti/entities/opencti_stix_object_or_stix_relationship.py
 pycti/entities/opencti_stix_sighting_relationship.py
+pycti/entities/opencti_task.py
 pycti/entities/opencti_threat_actor.py
 pycti/entities/opencti_tool.py
 pycti/entities/opencti_vocabulary.py
 pycti/entities/opencti_vulnerability.py
 pycti/utils/__init__.py
 pycti/utils/constants.py
 pycti/utils/opencti_stix2.py
```

### Comparing `pycti-5.7.post576/pycti.egg-info/requires.txt` & `pycti-5.8.0/pycti.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 datefinder~=0.7.3
 pika~=1.3.1
 python_json_logger~=2.0.4
 pyyaml~=6.0
-requests~=2.28.2
-setuptools~=66.1.1
-filigran_sseclient~=1.0.0
+requests~=2.31.0
+setuptools~=67.8.0
+filigran-sseclient~=1.0.0
 stix2~=3.0.1
 cachetools~=5.3.0
 
 [:sys_platform == "linux" or sys_platform == "darwin"]
 python-magic~=0.4.27
 
 [:sys_platform == "win32"]
 python-magic-bin~=0.4.14
 
 [dev]
-black~=23.1.0
-build~=0.8.0
-isort~=5.10.1
-types-pytz~=2022.2.1.0
-pre-commit~=2.20.0
+black~=23.3.0
+build~=0.10.0
+isort~=5.12.0
+types-pytz~=2023.3.0.0
+pre-commit~=3.3.2
 pytest-cases~=3.6.13
-pytest-cov~=3.0.0
+pytest-cov~=4.1.0
 pytest_randomly~=3.12.0
-pytest~=7.1.2
+pytest~=7.3.2
 types-python-dateutil~=2.8.19
-wheel~=0.37.1
+wheel~=0.40.0
 
 [doc]
 autoapi~=2.0.1
-sphinx-autodoc-typehints~=1.19.2
-sphinx-rtd-theme~=1.0.0
+sphinx-autodoc-typehints~=1.23.0
+sphinx-rtd-theme~=1.2.1
```

### Comparing `pycti-5.7.post576/pyproject.toml` & `pycti-5.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post576/setup.cfg` & `pycti-5.8.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -34,35 +34,35 @@
 install_requires = 
 	datefinder~=0.7.3
 	pika~=1.3.1
 	python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
 	python-magic-bin~=0.4.14; sys_platform == "win32"
 	python_json_logger~=2.0.4
 	pyyaml~=6.0
-	requests~=2.28.2
-	setuptools~=66.1.1
-	filigran_sseclient~=1.0.0
+	requests~=2.31.0
+	setuptools~=67.8.0
+	filigran-sseclient~=1.0.0
 	stix2~=3.0.1
 	cachetools~=5.3.0
 
 [options.extras_require]
 dev = 
-	black~=23.1.0
-	build~=0.8.0
-	isort~=5.10.1
-	types-pytz~=2022.2.1.0
-	pre-commit~=2.20.0
+	black~=23.3.0
+	build~=0.10.0
+	isort~=5.12.0
+	types-pytz~=2023.3.0.0
+	pre-commit~=3.3.2
 	pytest-cases~=3.6.13
-	pytest-cov~=3.0.0
+	pytest-cov~=4.1.0
 	pytest_randomly~=3.12.0
-	pytest~=7.1.2
+	pytest~=7.3.2
 	types-python-dateutil~=2.8.19
-	wheel~=0.37.1
+	wheel~=0.40.0
 doc = 
 	autoapi~=2.0.1
-	sphinx-autodoc-typehints~=1.19.2
-	sphinx-rtd-theme~=1.0.0
+	sphinx-autodoc-typehints~=1.23.0
+	sphinx-rtd-theme~=1.2.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

