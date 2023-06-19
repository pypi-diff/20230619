# Comparing `tmp/lusid-notification-sdk-preview-0.1.744.post2.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.748.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.744.post2.tar", last modified: Fri Jun 16 09:04:45 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.748.tar", last modified: Mon Jun 19 10:50:59 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.744.post2.tar` & `lusid-notification-sdk-preview-0.1.748.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8006 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4352 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7824 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52809 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47815 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27787 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16637 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5101 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3062 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7256 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9019 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    10959 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9236 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    38059 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/create_notification_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    12415 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    14937 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    11112 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8023 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9512 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6427 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9541 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10706 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6829 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    15841 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)    37019 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/notification_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7518 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8014 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    15858 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8549 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    11553 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15805 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13562 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 09:04:45.000000 lusid-notification-sdk-preview-0.1.744.post2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-06-16 09:04:04.000000 lusid-notification-sdk-preview-0.1.744.post2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8002 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52797 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47803 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27783 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    10957 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     9234 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10718 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    38057 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/create_notification_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    11110 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9510 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9539 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7863 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    15839 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)    37017 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/notification_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8547 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11551 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15803 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 10:50:59.000000 lusid-notification-sdk-preview-0.1.748/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-19 10:50:28.000000 lusid-notification-sdk-preview-0.1.748/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/README.md` & `lusid-notification-sdk-preview-0.1.748/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.744-2
-- Package version: 0.1.744-2
+- API version: 0.1.748
+- Package version: 0.1.748
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.744-2"
+__version__ = "0.1.748"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/api/application_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/api/event_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/api/manual_event_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/api/notifications_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.744-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.744-2/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.748/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.744-2\n"\
-               "SDK Package Version: 0.1.744-2".\
+               "Version of the API: 0.1.748\n"\
+               "SDK Package Version: 0.1.748".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/api_request_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/create_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/create_notification_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/create_notification_request_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/manual_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/manual_event_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/manual_event_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/matching_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/notification_notification_type.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/notification_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/sms_notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -44,44 +44,47 @@
         'description': 'str',
         'status': 'str',
         'matching_pattern': 'MatchingPattern',
         'created_at': 'datetime',
         'user_id_created': 'str',
         'modified_at': 'datetime',
         'user_id_modified': 'str',
-        'use_as_auth': 'str'
+        'use_as_auth': 'str',
+        'href': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
         'status': 'status',
         'matching_pattern': 'matchingPattern',
         'created_at': 'createdAt',
         'user_id_created': 'userIdCreated',
         'modified_at': 'modifiedAt',
         'user_id_modified': 'userIdModified',
-        'use_as_auth': 'useAsAuth'
+        'use_as_auth': 'useAsAuth',
+        'href': 'href'
     }
 
     required_map = {
         'id': 'required',
         'display_name': 'required',
         'description': 'optional',
         'status': 'required',
         'matching_pattern': 'required',
         'created_at': 'required',
         'user_id_created': 'required',
         'modified_at': 'required',
         'user_id_modified': 'required',
-        'use_as_auth': 'required'
+        'use_as_auth': 'required',
+        'href': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, status=None, matching_pattern=None, created_at=None, user_id_created=None, modified_at=None, user_id_modified=None, use_as_auth=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, display_name=None, description=None, status=None, matching_pattern=None, created_at=None, user_id_created=None, modified_at=None, user_id_modified=None, use_as_auth=None, href=None, local_vars_configuration=None):  # noqa: E501
         """Subscription - a model defined in OpenAPI"
         
         :param id:  (required)
         :type id: lusid_notification.ResourceId
         :param display_name:  The name of the subscription (required)
         :type display_name: str
         :param description:  The summary of the services provided by the subscription
@@ -96,14 +99,16 @@
         :type user_id_created: str
         :param modified_at:  The time at which the subscription was last modified (required)
         :type modified_at: datetime
         :param user_id_modified:  The user who last modified the subscription (required)
         :type user_id_modified: str
         :param use_as_auth:  The user to use as auth for the subscription (required)
         :type use_as_auth: str
+        :param href:  A URI for retrieving this subscription
+        :type href: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
@@ -112,26 +117,28 @@
         self._status = None
         self._matching_pattern = None
         self._created_at = None
         self._user_id_created = None
         self._modified_at = None
         self._user_id_modified = None
         self._use_as_auth = None
+        self._href = None
         self.discriminator = None
 
         self.id = id
         self.display_name = display_name
         self.description = description
         self.status = status
         self.matching_pattern = matching_pattern
         self.created_at = created_at
         self.user_id_created = user_id_created
         self.modified_at = modified_at
         self.user_id_modified = user_id_modified
         self.use_as_auth = use_as_auth
+        self.href = href
 
     @property
     def id(self):
         """Gets the id of this Subscription.  # noqa: E501
 
 
         :return: The id of this Subscription.  # noqa: E501
@@ -384,14 +391,37 @@
             raise ValueError("Invalid value for `use_as_auth`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 use_as_auth is not None and len(use_as_auth) < 1):
             raise ValueError("Invalid value for `use_as_auth`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._use_as_auth = use_as_auth
 
+    @property
+    def href(self):
+        """Gets the href of this Subscription.  # noqa: E501
+
+        A URI for retrieving this subscription  # noqa: E501
+
+        :return: The href of this Subscription.  # noqa: E501
+        :rtype: str
+        """
+        return self._href
+
+    @href.setter
+    def href(self, href):
+        """Sets the href of this Subscription.
+
+        A URI for retrieving this subscription  # noqa: E501
+
+        :param href: The href of this Subscription.  # noqa: E501
+        :type href: str
+        """
+
+        self._href = href
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/update_notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/models/webhook_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.744-2
+    The version of the OpenAPI document: 0.1.748
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.748/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.748/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.744.post2/setup.py` & `lusid-notification-sdk-preview-0.1.748/setup.py`

 * *Files identical despite different names*

