# Comparing `tmp/pymobiledevice3-2.0.0.tar.gz` & `tmp/pymobiledevice3-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymobiledevice3-2.0.0.tar", last modified: Sun Jun 18 13:43:25 2023, max compression
+gzip compressed data, was "pymobiledevice3-2.0.1.tar", last modified: Sun Jun 18 14:46:55 2023, max compression
```

## Comparing `pymobiledevice3-2.0.0.tar` & `pymobiledevice3-2.0.1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.916023 pymobiledevice3-2.0.0/pymobiledevice3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/bonjour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/ca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.928023 pymobiledevice3-2.0.0/pymobiledevice3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/afc.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/bonjour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/companion_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/developer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/mounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/provision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/springboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/webinspector.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/irecv.py
--rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/irecv_devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27360 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/pair_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.932023 pymobiledevice3-2.0.0/pymobiledevice3/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/dsc_uuid_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/dsc_uuid_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/firmware_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/notifications.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.936023 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/element_attribute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/element_clear.js
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/enter_fullscreen.js
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/find_nodes.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/focus.js
--rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/get_attribute.js
--rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_displayed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_editable.js
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_enabled.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.936023 pymobiledevice3-2.0.0/pymobiledevice3/restore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/base_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/fdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/ftab.py
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/restore_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/restored_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/tss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6768 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/service_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.940023 pymobiledevice3-2.0.0/pymobiledevice3/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/accessibilityaudit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31043 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/afc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/crash_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/debugserver_applist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/device_arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/device_link.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6154 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/diagnostics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dtfetchsymbols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.940023 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.940023 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/application_listing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/condition_inducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/network_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/process_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/sysmontap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/file_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/heartbeat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/house_arrest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/installation_proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/misagent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3379 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_activation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3322 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_image_mounter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16752 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/mobilebackup2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/notification_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/os_trace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/pcapd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/preboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/remote_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/simulate_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/springboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/syslog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/automation_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_screencast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/inspector_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/selenium_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/session_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/switch_to.py
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/webinspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/tcp_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.920023 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.969881 pymobiledevice3-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-06-18 14:46:55.969881 pymobiledevice3-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.949880 pymobiledevice3-2.0.1/pymobiledevice3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/bonjour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/ca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.953881 pymobiledevice3-2.0.1/pymobiledevice3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/bonjour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/companion_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/developer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/mounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/cli/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/irecv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/irecv_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27360 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/pair_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.953881 pymobiledevice3-2.0.1/pymobiledevice3/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/dsc_uuid_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/dsc_uuid_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/firmware_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/notifications.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.953881 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/element_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/element_clear.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/enter_fullscreen.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/find_nodes.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/focus.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/get_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/is_displayed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/is_editable.js
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/is_enabled.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.957881 pymobiledevice3-2.0.1/pymobiledevice3/restore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/base_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/ftab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/restored_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/restore/tss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6768 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/service_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.961881 pymobiledevice3-2.0.1/pymobiledevice3/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/accessibilityaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31043 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/crash_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/debugserver_applist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/device_arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/device_link.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6154 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/diagnostics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dtfetchsymbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.961881 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.965881 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/application_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/condition_inducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/network_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/process_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/sysmontap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/file_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/heartbeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/house_arrest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/installation_proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/misagent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3379 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/mobile_activation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3322 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/mobile_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/mobile_image_mounter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16752 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/mobilebackup2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/notification_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/os_trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/pcapd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/preboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/remote_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/simulate_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/syslog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.965881 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/automation_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/cdp_screencast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/cdp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/cdp_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/inspector_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/selenium_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/session_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/switch_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/services/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/tcp_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pymobiledevice3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.949880 pymobiledevice3-2.0.1/pymobiledevice3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-06-18 14:46:55.000000 pymobiledevice3-2.0.1/pymobiledevice3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-06-18 14:46:55.000000 pymobiledevice3-2.0.1/pymobiledevice3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:46:55.000000 pymobiledevice3-2.0.1/pymobiledevice3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 14:46:55.000000 pymobiledevice3-2.0.1/pymobiledevice3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-18 14:46:55.000000 pymobiledevice3-2.0.1/pymobiledevice3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 14:46:55.000000 pymobiledevice3-2.0.1/pymobiledevice3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:46:55.969881 pymobiledevice3-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:46:55.965881 pymobiledevice3-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-18 14:46:40.000000 pymobiledevice3-2.0.1/tests/test_utils.py
```

### Comparing `pymobiledevice3-2.0.0/LICENSE` & `pymobiledevice3-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/PKG-INFO` & `pymobiledevice3-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 2.0.0
+Version: 2.0.1
 Summary: Pure python3 implementation for working with iDevices (iPhone, etc...)
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `pymobiledevice3-2.0.0/README.md` & `pymobiledevice3-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/__main__.py` & `pymobiledevice3-2.0.1/pymobiledevice3/__main__.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/bonjour.py` & `pymobiledevice3-2.0.1/pymobiledevice3/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/ca.py` & `pymobiledevice3-2.0.1/pymobiledevice3/ca.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/activation.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/activation.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/afc.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/afc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/amfi.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/amfi.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/apps.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/apps.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/backup.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/bonjour.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/cli_common.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/companion_proxy.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/companion_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/crash.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/crash.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/developer.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/developer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/diagnostics.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/lockdown.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/lockdown.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/mounter.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/mounter.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/notification.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/notification.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/pcap.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/pcap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/power_assertion.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/power_assertion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/processes.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/processes.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/profile.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/profile.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/provision.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/provision.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/restore.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/springboard.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/springboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/syslog.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/syslog.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/usbmux.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/usbmux.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/cli/webinspector.py` & `pymobiledevice3-2.0.1/pymobiledevice3/cli/webinspector.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/exceptions.py` & `pymobiledevice3-2.0.1/pymobiledevice3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/irecv.py` & `pymobiledevice3-2.0.1/pymobiledevice3/irecv.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/irecv_devices.py` & `pymobiledevice3-2.0.1/pymobiledevice3/irecv_devices.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/lockdown.py` & `pymobiledevice3-2.0.1/pymobiledevice3/lockdown.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/pair_records.py` & `pymobiledevice3-2.0.1/pymobiledevice3/pair_records.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     """
 
     # usbmuxd
     with suppress(NotPairedError, MuxException):
         with usbmux.create_mux() as mux:
             if isinstance(mux, PlistMuxConnection):
                 pair_record = mux.get_pair_record(identifier)
-    if pair_record is not None:
-        return pair_record
+                if pair_record is not None:
+                    return pair_record
 
     # iTunes
     pair_record = get_itunes_pairing_record(identifier)
     if pair_record is not None:
         return pair_record
 
     # local storage
```

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/dsc_uuid_map.json` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/dsc_uuid_map.json`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/dsc_uuid_map.py` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/dsc_uuid_map.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/firmware_notifications.py` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/firmware_notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/notifications.txt` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/notifications.txt`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/element_clear.js` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/element_clear.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/enter_fullscreen.js` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/enter_fullscreen.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/find_nodes.js` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/find_nodes.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/get_attribute.js` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/get_attribute.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_displayed.js` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/is_displayed.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_editable.js` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/is_editable.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_enabled.js` & `pymobiledevice3-2.0.1/pymobiledevice3/resources/webinspector/is_enabled.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/asr.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/asr.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/base_restore.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/base_restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/consts.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/consts.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/device.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/device.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/fdr.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/fdr.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/ftab.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/ftab.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/recovery.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/recovery.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/restore.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/restore_options.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/restore_options.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/restored_client.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/restored_client.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/restore/tss.py` & `pymobiledevice3-2.0.1/pymobiledevice3/restore/tss.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/service_connection.py` & `pymobiledevice3-2.0.1/pymobiledevice3/service_connection.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/accessibilityaudit.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/accessibilityaudit.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/afc.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/afc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/amfi.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/amfi.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/base_service.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/base_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/companion.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/companion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/crash_reports.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/crash_reports.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/debugserver_applist.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/debugserver_applist.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/device_arbitration.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/device_arbitration.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/device_link.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/device_link.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/diagnostics.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dtfetchsymbols.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dtfetchsymbols.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/application_listing.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/application_listing.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/condition_inducer.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/condition_inducer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/device_info.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/device_info.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/energy_monitor.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/graphics.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/graphics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/network_monitor.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/network_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/notifications.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/process_control.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/process_control.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/sysmontap.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/dvt/instruments/sysmontap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/file_relay.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/file_relay.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/heartbeat.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/house_arrest.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/house_arrest.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/installation_proxy.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/misagent.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/misagent.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_activation.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/mobile_activation.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_config.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/mobile_config.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_image_mounter.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/mobile_image_mounter.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/mobilebackup2.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/mobilebackup2.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/notification_proxy.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/os_trace.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/os_trace.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/pcapd.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/pcapd.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/power_assertion.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/power_assertion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/preboard.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/preboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/remote_server.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/remote_server.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/screenshot.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/screenshot.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/simulate_location.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/simulate_location.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/springboard.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/springboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/syslog.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/syslog.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/alert.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/alert.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/automation_session.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/automation_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_screencast.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/cdp_screencast.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_server.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/cdp_server.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_target.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/cdp_target.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/driver.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/driver.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/element.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/element.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/inspector_session.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/inspector_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/selenium_api.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/selenium_api.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/session_protocol.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/session_protocol.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/switch_to.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/web_protocol/switch_to.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/services/webinspector.py` & `pymobiledevice3-2.0.1/pymobiledevice3/services/webinspector.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/tcp_forwarder.py` & `pymobiledevice3-2.0.1/pymobiledevice3/tcp_forwarder.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/usbmux.py` & `pymobiledevice3-2.0.1/pymobiledevice3/usbmux.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3/utils.py` & `pymobiledevice3-2.0.1/pymobiledevice3/utils.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3.egg-info/PKG-INFO` & `pymobiledevice3-2.0.1/pymobiledevice3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 2.0.0
+Version: 2.0.1
 Summary: Pure python3 implementation for working with iDevices (iPhone, etc...)
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `pymobiledevice3-2.0.0/pymobiledevice3.egg-info/SOURCES.txt` & `pymobiledevice3-2.0.1/pymobiledevice3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.0/pyproject.toml` & `pymobiledevice3-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymobiledevice3"
-version = "2.0.0"
+version = "2.0.1"
 description = "Pure python3 implementation for working with iDevices (iPhone, etc...)"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["ios", "protocol", "lockdownd", "instruments", "automation", "cli", "afc"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
```

