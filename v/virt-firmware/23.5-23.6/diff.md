# Comparing `tmp/virt-firmware-23.5.tar.gz` & `tmp/virt-firmware-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virt-firmware-23.5.tar", last modified: Thu May  4 08:06:41 2023, max compression
+gzip compressed data, was "virt-firmware-23.6.tar", last modified: Mon Jun 19 10:47:34 2023, max compression
```

## Comparing `virt-firmware-23.5.tar` & `virt-firmware-23.6.tar`

### file list

```diff
@@ -1,75 +1,81 @@
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.145242 virt-firmware-23.5/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    18012 2022-04-20 16:46:39.000000 virt-firmware-23.5/LICENSE
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      116 2023-01-26 11:26:15.000000 virt-firmware-23.5/MANIFEST.in
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-05-04 08:06:41.145242 virt-firmware-23.5/PKG-INFO
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2199 2022-07-18 11:50:43.000000 virt-firmware-23.5/README.md
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.135242 virt-firmware-23.5/experimental/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     5654 2023-05-04 07:26:42.000000 virt-firmware-23.5/experimental/bootcfg.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1820 2023-01-11 05:55:56.000000 virt-firmware-23.5/experimental/dbxupdate.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     8840 2023-05-03 10:09:28.000000 virt-firmware-23.5/experimental/measure.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.136242 virt-firmware-23.5/man/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      939 2023-05-04 07:54:14.000000 virt-firmware-23.5/man/virt-fw-dump.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      223 2022-10-05 11:46:37.000000 virt-firmware-23.5/man/virt-fw-dump.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      734 2023-05-04 07:54:14.000000 virt-firmware-23.5/man/virt-fw-sigdb.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2022-10-05 11:46:32.000000 virt-firmware-23.5/man/virt-fw-sigdb.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4317 2023-05-04 07:54:14.000000 virt-firmware-23.5/man/virt-fw-vars.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      515 2022-10-05 11:55:41.000000 virt-firmware-23.5/man/virt-fw-vars.inc
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       81 2022-03-30 09:41:51.000000 virt-firmware-23.5/pyproject.toml
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1027 2023-05-04 08:06:41.145242 virt-firmware-23.5/setup.cfg
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       69 2022-03-30 09:41:51.000000 virt-firmware-23.5/setup.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.138242 virt-firmware-23.5/tests/
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.138242 virt-firmware-23.5/tests/data/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3737 2022-11-24 12:28:42.000000 virt-firmware-23.5/tests/data/DBXUpdate-20100307.x64.bin
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1772 2022-05-11 20:36:49.000000 virt-firmware-23.5/tests/data/secboot.aws
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      345 2022-12-02 08:59:55.000000 virt-firmware-23.5/tests/test-dump.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      271 2023-04-14 07:25:30.000000 virt-firmware-23.5/tests/test-pe.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      185 2022-09-02 08:19:03.000000 virt-firmware-23.5/tests/test-sigdb.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      689 2022-09-02 08:10:06.000000 virt-firmware-23.5/tests/test-vars.sh
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     3687 2022-12-07 13:29:04.000000 virt-firmware-23.5/tests/tests.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.134242 virt-firmware-23.5/virt/
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.139242 virt-firmware-23.5/virt/firmware/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      130 2022-11-10 08:06:38.000000 virt-firmware-23.5/virt/firmware/__init__.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.139242 virt-firmware-23.5/virt/firmware/aws/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    11381 2022-05-11 20:36:49.000000 virt-firmware-23.5/virt/firmware/aws/dict.v0
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.142242 virt-firmware-23.5/virt/firmware/certs/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4323 2022-07-07 16:26:41.000000 virt-firmware-23.5/virt/firmware/certs/CentOSSecureBootCA2.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4339 2022-07-07 16:26:41.000000 virt-firmware-23.5/virt/firmware/certs/CentOSSecureBootCAkey1.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6739 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6869 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6698 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4615 2022-07-07 08:32:28.000000 virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA3.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4431 2022-07-07 08:32:38.000000 virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA5.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4324 2022-07-07 08:32:47.000000 virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA6.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4500 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5007 2022-07-16 16:13:52.000000 virt-firmware-23.5/virt/firmware/certs/fedoraca-20200709.pem
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    21517 2023-05-03 10:06:49.000000 virt-firmware-23.5/virt/firmware/dump.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.143242 virt-firmware-23.5/virt/firmware/efi/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      123 2023-04-28 10:54:50.000000 virt-firmware-23.5/virt/firmware/efi/__init__.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1892 2023-04-28 11:18:07.000000 virt-firmware-23.5/virt/firmware/efi/bootentry.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2774 2022-12-07 13:30:17.000000 virt-firmware-23.5/virt/firmware/efi/certs.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5109 2023-03-24 08:04:11.000000 virt-firmware-23.5/virt/firmware/efi/devpath.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1663 2022-12-14 07:11:30.000000 virt-firmware-23.5/virt/firmware/efi/efijson.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    17539 2023-04-28 11:17:30.000000 virt-firmware-23.5/virt/firmware/efi/efivar.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5173 2022-12-02 08:15:31.000000 virt-firmware-23.5/virt/firmware/efi/guids.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6167 2023-04-13 11:19:16.000000 virt-firmware-23.5/virt/firmware/efi/siglist.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1379 2022-03-30 10:39:05.000000 virt-firmware-23.5/virt/firmware/efi/ucs16.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1434 2023-01-11 05:55:56.000000 virt-firmware-23.5/virt/firmware/host.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1689 2023-01-11 05:55:56.000000 virt-firmware-23.5/virt/firmware/migrate.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      494 2022-05-11 20:36:49.000000 virt-firmware-23.5/virt/firmware/misc.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1588 2023-01-11 05:55:56.000000 virt-firmware-23.5/virt/firmware/sigdb.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)    13202 2023-04-13 10:13:39.000000 virt-firmware-23.5/virt/firmware/vars.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.144241 virt-firmware-23.5/virt/firmware/varstore/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       66 2023-03-03 10:32:41.000000 virt-firmware-23.5/virt/firmware/varstore/__init__.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5423 2022-11-24 13:01:24.000000 virt-firmware-23.5/virt/firmware/varstore/aws.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6271 2023-04-13 10:23:09.000000 virt-firmware-23.5/virt/firmware/varstore/edk2.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1707 2023-04-28 11:34:16.000000 virt-firmware-23.5/virt/firmware/varstore/linux.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.144241 virt-firmware-23.5/virt/peutils/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       60 2022-12-14 09:40:14.000000 virt-firmware-23.5/virt/peutils/__init__.py
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)     9437 2023-04-18 08:24:36.000000 virt-firmware-23.5/virt/peutils/peutils.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-05-04 08:06:41.145242 virt-firmware-23.5/virt_firmware.egg-info/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/PKG-INFO
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1738 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/SOURCES.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)        1 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/dependency_links.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      358 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/entry_points.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       31 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/requires.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       68 2023-05-04 08:06:41.000000 virt-firmware-23.5/virt_firmware.egg-info/top_level.txt
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.613739 virt-firmware-23.6/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    18012 2022-04-20 16:46:39.000000 virt-firmware-23.6/LICENSE
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      116 2023-01-26 11:26:15.000000 virt-firmware-23.6/MANIFEST.in
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-06-19 10:47:34.613739 virt-firmware-23.6/PKG-INFO
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2199 2022-07-18 11:50:43.000000 virt-firmware-23.6/README.md
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.601739 virt-firmware-23.6/experimental/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1820 2023-01-11 05:55:56.000000 virt-firmware-23.6/experimental/dbxupdate.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     8840 2023-05-03 10:09:28.000000 virt-firmware-23.6/experimental/measure.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.603739 virt-firmware-23.6/man/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      939 2023-05-04 07:54:14.000000 virt-firmware-23.6/man/virt-fw-dump.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      223 2022-10-05 11:46:37.000000 virt-firmware-23.6/man/virt-fw-dump.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      734 2023-05-04 07:54:14.000000 virt-firmware-23.6/man/virt-fw-sigdb.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2022-10-05 11:46:32.000000 virt-firmware-23.6/man/virt-fw-sigdb.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4317 2023-05-04 07:54:14.000000 virt-firmware-23.6/man/virt-fw-vars.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      515 2022-10-05 11:55:41.000000 virt-firmware-23.6/man/virt-fw-vars.inc
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       81 2022-03-30 09:41:51.000000 virt-firmware-23.6/pyproject.toml
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1150 2023-06-19 10:47:34.613739 virt-firmware-23.6/setup.cfg
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       69 2022-03-30 09:41:51.000000 virt-firmware-23.6/setup.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.604739 virt-firmware-23.6/tests/
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.604739 virt-firmware-23.6/tests/data/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3737 2022-11-24 12:28:42.000000 virt-firmware-23.6/tests/data/DBXUpdate-20100307.x64.bin
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1772 2022-05-11 20:36:49.000000 virt-firmware-23.6/tests/data/secboot.aws
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      106 2023-06-19 09:43:59.000000 virt-firmware-23.6/tests/test-bootcfg.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      345 2022-12-02 08:59:55.000000 virt-firmware-23.6/tests/test-dump.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      271 2023-04-14 07:25:30.000000 virt-firmware-23.6/tests/test-pe.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      185 2022-09-02 08:19:03.000000 virt-firmware-23.6/tests/test-sigdb.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      689 2022-09-02 08:10:06.000000 virt-firmware-23.6/tests/test-vars.sh
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     3711 2023-05-10 05:55:51.000000 virt-firmware-23.6/tests/tests.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.598739 virt-firmware-23.6/virt/
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.606739 virt-firmware-23.6/virt/firmware/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      141 2023-05-11 13:53:51.000000 virt-firmware-23.6/virt/firmware/__init__.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.606739 virt-firmware-23.6/virt/firmware/aws/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    11381 2022-05-11 20:36:49.000000 virt-firmware-23.6/virt/firmware/aws/dict.v0
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.607739 virt-firmware-23.6/virt/firmware/bootcfg/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       83 2023-06-19 09:21:32.000000 virt-firmware-23.6/virt/firmware/bootcfg/__init__.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6217 2023-05-31 09:45:46.000000 virt-firmware-23.6/virt/firmware/bootcfg/bootcfg.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6180 2023-05-31 09:45:46.000000 virt-firmware-23.6/virt/firmware/bootcfg/linuxcfg.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     9761 2023-05-31 09:45:46.000000 virt-firmware-23.6/virt/firmware/bootcfg/main.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1476 2023-05-31 09:45:46.000000 virt-firmware-23.6/virt/firmware/bootcfg/menu.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.609739 virt-firmware-23.6/virt/firmware/certs/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4323 2022-07-07 16:26:41.000000 virt-firmware-23.6/virt/firmware/certs/CentOSSecureBootCA2.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4339 2022-07-07 16:26:41.000000 virt-firmware-23.6/virt/firmware/certs/CentOSSecureBootCAkey1.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6739 2022-03-30 10:39:05.000000 virt-firmware-23.6/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6869 2022-03-30 10:39:05.000000 virt-firmware-23.6/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6698 2022-03-30 10:39:05.000000 virt-firmware-23.6/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4615 2022-07-07 08:32:28.000000 virt-firmware-23.6/virt/firmware/certs/RedHatSecureBootCA3.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4431 2022-07-07 08:32:38.000000 virt-firmware-23.6/virt/firmware/certs/RedHatSecureBootCA5.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4324 2022-07-07 08:32:47.000000 virt-firmware-23.6/virt/firmware/certs/RedHatSecureBootCA6.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4500 2022-03-30 10:39:05.000000 virt-firmware-23.6/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5007 2022-07-16 16:13:52.000000 virt-firmware-23.6/virt/firmware/certs/fedoraca-20200709.pem
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    21605 2023-06-01 11:55:57.000000 virt-firmware-23.6/virt/firmware/dump.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.610739 virt-firmware-23.6/virt/firmware/efi/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      123 2023-04-28 10:54:50.000000 virt-firmware-23.6/virt/firmware/efi/__init__.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1892 2023-04-28 11:18:07.000000 virt-firmware-23.6/virt/firmware/efi/bootentry.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2774 2022-12-07 13:30:17.000000 virt-firmware-23.6/virt/firmware/efi/certs.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6127 2023-05-17 10:47:35.000000 virt-firmware-23.6/virt/firmware/efi/devpath.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1663 2022-12-14 07:11:30.000000 virt-firmware-23.6/virt/firmware/efi/efijson.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    18276 2023-05-31 11:56:30.000000 virt-firmware-23.6/virt/firmware/efi/efivar.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5173 2022-12-02 08:15:31.000000 virt-firmware-23.6/virt/firmware/efi/guids.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6378 2023-05-23 05:54:53.000000 virt-firmware-23.6/virt/firmware/efi/siglist.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1383 2023-05-17 10:47:15.000000 virt-firmware-23.6/virt/firmware/efi/ucs16.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1460 2023-05-10 05:37:01.000000 virt-firmware-23.6/virt/firmware/host.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1689 2023-01-11 05:55:56.000000 virt-firmware-23.6/virt/firmware/migrate.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      494 2022-05-11 20:36:49.000000 virt-firmware-23.6/virt/firmware/misc.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1588 2023-01-11 05:55:56.000000 virt-firmware-23.6/virt/firmware/sigdb.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    13442 2023-05-31 11:49:40.000000 virt-firmware-23.6/virt/firmware/vars.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.611739 virt-firmware-23.6/virt/firmware/varstore/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       66 2023-03-03 10:32:41.000000 virt-firmware-23.6/virt/firmware/varstore/__init__.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5423 2022-11-24 13:01:24.000000 virt-firmware-23.6/virt/firmware/varstore/aws.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6902 2023-05-23 05:54:53.000000 virt-firmware-23.6/virt/firmware/varstore/edk2.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2821 2023-05-11 07:54:32.000000 virt-firmware-23.6/virt/firmware/varstore/linux.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.612739 virt-firmware-23.6/virt/peutils/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       60 2022-12-14 09:40:14.000000 virt-firmware-23.6/virt/peutils/__init__.py
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    10479 2023-05-31 09:45:46.000000 virt-firmware-23.6/virt/peutils/peutils.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-06-19 10:47:34.612739 virt-firmware-23.6/virt_firmware.egg-info/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-06-19 10:47:34.000000 virt-firmware-23.6/virt_firmware.egg-info/PKG-INFO
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1897 2023-06-19 10:47:34.000000 virt-firmware-23.6/virt_firmware.egg-info/SOURCES.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)        1 2023-06-19 10:47:34.000000 virt-firmware-23.6/virt_firmware.egg-info/dependency_links.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      456 2023-06-19 10:47:34.000000 virt-firmware-23.6/virt_firmware.egg-info/entry_points.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       31 2023-06-19 10:47:34.000000 virt-firmware-23.6/virt_firmware.egg-info/requires.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       90 2023-06-19 10:47:34.000000 virt-firmware-23.6/virt_firmware.egg-info/top_level.txt
```

### Comparing `virt-firmware-23.5/LICENSE` & `virt-firmware-23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/PKG-INFO` & `virt-firmware-23.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virt-firmware
-Version: 23.5
+Version: 23.6
 Summary: tools for virtual machine firmware volumes
 Author: Gerd Hoffmann
 Author-email: kraxel@redhat.com
 License: GPLv2
 Project-URL: GitLab, https://gitlab.com/kraxel/virt-firmware
 Keywords: ovmf,armvirt,edk2,aws
 Description-Content-Type: text/markdown
```

### Comparing `virt-firmware-23.5/README.md` & `virt-firmware-23.6/README.md`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/experimental/dbxupdate.py` & `virt-firmware-23.6/experimental/dbxupdate.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/experimental/measure.py` & `virt-firmware-23.6/experimental/measure.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/man/virt-fw-dump.1` & `virt-firmware-23.6/man/virt-fw-dump.1`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/man/virt-fw-sigdb.1` & `virt-firmware-23.6/man/virt-fw-sigdb.1`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/man/virt-fw-vars.1` & `virt-firmware-23.6/man/virt-fw-vars.1`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/man/virt-fw-vars.inc` & `virt-firmware-23.6/man/virt-fw-vars.inc`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/setup.cfg` & `virt-firmware-23.6/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = virt-firmware
-version = 23.5
+version = 23.6
 description = tools for virtual machine firmware volumes
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ovmf, armvirt, edk2, aws
 license = GPLv2
 license_files = LICENSE
 author = Gerd Hoffmann
@@ -13,27 +13,30 @@
 	GitLab = https://gitlab.com/kraxel/virt-firmware
 
 [options]
 packages = 
 	virt/firmware
 	virt/firmware/efi
 	virt/firmware/varstore
+	virt/firmware/bootcfg
 	virt/peutils
 install_requires = 
 	setuptools
 	cryptography
 	pefile
 
 [options.entry_points]
 console_scripts = 
 	host-efi-vars = virt.firmware.host:main
 	virt-fw-vars = virt.firmware.vars:main
 	virt-fw-dump = virt.firmware.dump:main
 	virt-fw-sigdb = virt.firmware.sigdb:main
 	migrate-vars = virt.firmware.migrate:main
+	kernel-bootcfg = virt.firmware.bootcfg.main:main
+	uefi-boot-menu = virt.firmware.bootcfg.menu:main
 	pe-dumpinfo = virt.peutils.peutils:pe_dumpinfo
 	pe-listsigs = virt.peutils.peutils:pe_listsigs
 	pe-addsigs = virt.peutils.peutils:pe_addsigs
 
 [options.package_data]
 virt/firmware = certs/*.pem, aws/dict.v0
```

### Comparing `virt-firmware-23.5/tests/data/DBXUpdate-20100307.x64.bin` & `virt-firmware-23.6/tests/data/DBXUpdate-20100307.x64.bin`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/tests/data/secboot.aws` & `virt-firmware-23.6/tests/data/secboot.aws`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/tests/test-vars.sh` & `virt-firmware-23.6/tests/test-vars.sh`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/tests/tests.py` & `virt-firmware-23.6/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
         path = devpath.DevicePath.filepath("\\EFI\\fedora\\shimx64.efi")
         varlist = efivar.EfiVarList()
         varlist.set_boot_entry(0x99, 'shim', path)
         varlist.set_boot_next(0x99)
 
     @unittest.skipUnless(os.path.exists('/sys/firmware/efi/efivars'), 'no efivars fs')
     def test_parse_linux(self):
-        varlist = linux.LinuxVarStore.get_varlist()
+        store = linux.LinuxVarStore()
+        varlist = store.get_varlist()
 
     def test_parse_aws(self):
         varlist = aws.AwsVarStore(TEST_AWS)
 
     def test_generate_aws(self):
         varlist = efivar.EfiVarList()
         varlist.enroll_platform_redhat()
```

### Comparing `virt-firmware-23.5/virt/firmware/aws/dict.v0` & `virt-firmware-23.6/virt/firmware/aws/dict.v0`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/CentOSSecureBootCA2.pem` & `virt-firmware-23.6/virt/firmware/certs/CentOSSecureBootCA2.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/CentOSSecureBootCAkey1.pem` & `virt-firmware-23.6/virt/firmware/certs/CentOSSecureBootCAkey1.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem` & `virt-firmware-23.6/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem` & `virt-firmware-23.6/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem` & `virt-firmware-23.6/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA3.pem` & `virt-firmware-23.6/virt/firmware/certs/RedHatSecureBootCA3.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA5.pem` & `virt-firmware-23.6/virt/firmware/certs/RedHatSecureBootCA5.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootCA6.pem` & `virt-firmware-23.6/virt/firmware/certs/RedHatSecureBootCA6.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem` & `virt-firmware-23.6/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/certs/fedoraca-20200709.pem` & `virt-firmware-23.6/virt/firmware/certs/fedoraca-20200709.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/dump.py` & `virt-firmware-23.6/virt/firmware/dump.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,23 +269,26 @@
         0x02 : 'freeform',
         0x03 : 'sec-core',
         0x04 : 'pei-core',
         0x05 : 'dxe-core',
         0x06 : 'peim',
         0x07 : 'driver',
         0x09 : 'application',
-        0x0a : 'smm',
+        0x0a : 'mm',
         0x0b : 'fw-volume',
-        0x0d : 'smm-core',
+        0x0d : 'mm-core',
+        0x0e : 'mm-standalone',
+        0x0f : 'mm-standalone-core',
         0xf0 : 'padding',
     }
     sectiontypes = (
         0x03, 0x04, 0x05,
         0x06, 0x07, 0x08, 0x09,
         0x0a, 0x0b, 0x0d,
+        0x0e, 0x0f,
     )
 
     def __init__(self, data = None):
         super().__init__()
         self.guid = None
         self.typeid = 0
         self.attr = 0
@@ -515,15 +518,15 @@
         if data:
             self.parse(data)
 
     def parse(self, data):
         pos = 0
         step = 1024
         skips = 0
-        maxskips = 32
+        maxskips = 256
         while pos + 32 < len(data):
             (tlen, sig) = struct.unpack_from('<QL', data, pos + 32)
             if sig == 0x4856465f:
                 skips = 0
                 vol = Edk2Volume(data = data [ pos : ],
                                  offset = pos)
                 pos += vol.size()
```

### Comparing `virt-firmware-23.5/virt/firmware/efi/bootentry.py` & `virt-firmware-23.6/virt/firmware/efi/bootentry.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/efi/certs.py` & `virt-firmware-23.6/virt/firmware/efi/certs.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/efi/devpath.py` & `virt-firmware-23.6/virt/firmware/efi/devpath.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,22 @@
         self.data    = str(uri).encode()
 
     def set_filepath(self, filepath):
         self.devtype = 0x04	# media
         self.subtype = 0x04	# filepath
         self.data    = bytes(ucs16.from_string(str(filepath)))
 
+    def set_gpt(self, pnr, poff, plen, guid):
+        self.devtype = 0x04	# media
+        self.subtype = 0x01	# hard drive
+        self.data = b''
+        self.data += struct.pack('=LQQ', pnr, poff, plen)
+        self.data += guids.parse_str(guid).bytes_le
+        self.data += struct.pack('=BB', 0x02, 0x02)
+
     def fmt_hw(self):
         if self.subtype == 0x01:
             (func, dev) = struct.unpack_from('=BB', self.data)
             return f'PCI(dev={dev:02x}:{func:x})'
         if self.subtype == 0x04:
             guid = guids.parse_bin(self.data, 0)
             return f'VendorHW({guid})'
@@ -116,14 +124,29 @@
             return self.fmt_acpi()
         if self.devtype == 0x03:
             return self.fmt_msg()
         if self.devtype == 0x04:
             return self.fmt_media()
         return f'Unknown(type=0x{self.devtype:x},subtype=0x{self.subtype:x})'
 
+    def __eq__(self, other):
+        if self.devtype != other.devtype:
+            return False
+        if self.subtype != other.subtype:
+            return False
+
+        if self.devtype == 0x04 and self.subtype == 0x04:
+            # FilePath -> compare case-insensitive
+            p1 = str(ucs16.from_ucs16(self.data)).lower()
+            p2 = str(ucs16.from_ucs16(other.data)).lower()
+            return p1 == p2
+
+        return self.data == other.data
+
+
 class DevicePath(collections.UserList):
     """ class reprsenting an efi device path """
 
     def __init__(self, data = None):
         super().__init__()
         if data:
             pos = 0
@@ -155,7 +178,17 @@
         for elem in list(self):
             blob += bytes(elem)
         blob += bytes(DevicePathElem())
         return blob
 
     def __str__(self):
         return "/".join(map(str, list(self)))
+
+    def __eq__(self, other):
+        if len(self) != len(other):
+            return False
+        idx = 0
+        while idx < len(self):
+            if self[idx] != other[idx]:
+                return False
+            idx += 1
+        return True
```

### Comparing `virt-firmware-23.5/virt/firmware/efi/efijson.py` & `virt-firmware-23.6/virt/firmware/efi/efijson.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/efi/efivar.py` & `virt-firmware-23.6/virt/firmware/efi/efivar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# pylint: disable=too-many-public-methods
 """ efi variables """
 
 import re
 import struct
 import logging
 import datetime
 import collections
@@ -86,14 +87,19 @@
         'guid' : guids.Shim,
     },
     'MokListTrusted' : {
         'attr' : (EFI_VARIABLE_BOOTSERVICE_ACCESS |
                   EFI_VARIABLE_RUNTIME_ACCESS),
         'guid' : guids.Shim,
     },
+    'SbatLevel' : {
+        'attr' : (EFI_VARIABLE_NON_VOLATILE |
+                  EFI_VARIABLE_BOOTSERVICE_ACCESS),
+        'guid' : guids.Shim,
+    },
     'SHIM_DEBUG' : {
         'attr' : (EFI_VARIABLE_NON_VOLATILE |
                   EFI_VARIABLE_BOOTSERVICE_ACCESS),
         'guid' : guids.Shim,
     },
     'SHIM_VERBOSE' : {
         'attr' : (EFI_VARIABLE_NON_VOLATILE |
@@ -259,18 +265,29 @@
         self.data = bytes(entry)
         self.update_time()
 
     def set_boot_next(self, index):
         self.data = struct.pack('=H', index)
         self.update_time()
 
+    def set_boot_order(self, order):
+        self.data = b''
+        for item in order:
+            self.data += struct.pack('=H', item)
+        self.update_time()
+
     def append_boot_order(self, index):
         self.data += struct.pack('=H', index)
         self.update_time()
 
+    def set_from_file(self, filename):
+        with open(filename, 'rb') as f:
+            self.data = f.read()
+        self.update_time()
+
     def fmt_bool(self):
         if self.data[0]:
             return 'bool: ON'
         return 'bool: off'
 
     def fmt_ascii(self):
         string = self.data.decode().rstrip('\0')
@@ -384,14 +401,21 @@
         name = 'BootOrder'
         var = self.get(name)
         if not var:
             var = self.create(name)
         logging.info('append to variable %s: 0x%04X', name, index)
         var.append_boot_order(index)
 
+    def set_from_file(self, name, filename):
+        var = self.get(name)
+        if not var:
+            var = self.create(name)
+        logging.info('set variable %s from file %s', name, filename)
+        var.set_from_file(filename)
+
 
     def add_cert(self, name, owner, filename, replace = False):
         var = self.get(name)
         if not var:
             var = self.create(name)
         if replace:
             logging.info('clear %s sigdb', name)
```

### Comparing `virt-firmware-23.5/virt/firmware/efi/guids.py` & `virt-firmware-23.6/virt/firmware/efi/guids.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/efi/siglist.py` & `virt-firmware-23.6/virt/firmware/efi/siglist.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,20 +71,27 @@
             self.x509 = x509.load_der_x509_certificate(pem, default_backend())
         data = self.x509.public_bytes(serialization.Encoding.DER)
         self.add_sig(guid, data)
 
     def extract_cert(self, prefix = None):
         if self.x509 is None:
             return
-        cn = self.x509.subject.get_attributes_for_oid(x509.oid.NameOID.COMMON_NAME)[0]
+        names = self.x509.subject.get_attributes_for_oid(x509.oid.NameOID.COMMON_NAME)
+        if len(names) > 0:
+            name = names[0].value
+        else:
+            name = hashlib.sha256(
+                self.x509.public_bytes(
+                    serialization.Encoding.DER)).digest().hex()
+
         filename = ""
         if prefix:
             filename += prefix + '-'
         filename += str(self[0]['guid']) + '-'
-        filename += "".join(x for x in cn.value if x.isalnum())
+        filename += "".join(x for x in name if x.isalnum())
         filename += ".pem"
         if os.path.exists(filename):
             logging.info('exists: %s, skipping', filename)
             return
         logging.info('writing: %s', filename)
         with open(filename, "wb") as f:
             f.write(self.x509.public_bytes(serialization.Encoding.PEM))
```

### Comparing `virt-firmware-23.5/virt/firmware/efi/ucs16.py` & `virt-firmware-23.6/virt/firmware/efi/ucs16.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     def __str__(self):
         return self.data.decode('utf-16le')
 
     def __repr__(self):
         return f"{self.__class__.__name__}('{str(self)}')"
 
-def from_ucs16(data, offset):
+def from_ucs16(data, offset = 0):
     """ convert ucs-16 bytes to StringUCS16 """
     obj = StringUCS16()
     obj.parse_bin(data, offset)
     return obj
 
 def from_string(string):
     """ convert python string to StringUCS16 """
```

### Comparing `virt-firmware-23.5/virt/firmware/host.py` & `virt-firmware-23.6/virt/firmware/host.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,16 @@
                         action = 'store_true', default = False,
                         help = 'print volatile variables too')
     options = parser.parse_args()
 
     logging.basicConfig(format = '%(levelname)s: %(message)s',
                         level = getattr(logging, options.loglevel.upper()))
 
-    varlist = linux.LinuxVarStore.get_varlist(volatile = options.volatile)
+    varstore = linux.LinuxVarStore()
+    varlist = varstore.get_varlist(volatile = options.volatile)
     if options.verbose:
         varlist.print_normal(options.hexdump)
     else:
         varlist.print_compact()
 
     return 0
```

### Comparing `virt-firmware-23.5/virt/firmware/migrate.py` & `virt-firmware-23.6/virt/firmware/migrate.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/sigdb.py` & `virt-firmware-23.6/virt/firmware/sigdb.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/vars.py` & `virt-firmware-23.6/virt/firmware/vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
                         help = 'enable shim.efi verbose messages')
     pgroup.add_argument('--set-fallback-verbose', dest = 'set_fallback_verbose',
                         action = 'store_true', default = False,
                         help = 'enable fallback.efi verbose messages')
     pgroup.add_argument('--set-fallback-no-reboot', dest = 'set_fallback_no_reboot',
                         action = 'store_true', default = False,
                         help = 'disable rebooting for fallback.efi')
+    pgroup.add_argument('--set-sbat-level', dest = 'sbatlevel', type = str,
+                        help = 'set SbatLevel variable', metavar = 'FILE')
 
     pgroup = parser.add_argument_group('Secure boot setup options')
     pgroup.add_argument('--set-pk', dest = 'pk',  nargs = 2,
                         help = 'set PK to x509 cert, loaded in pem format ' +
                         'from FILE and with owner GUID',
                         metavar = ('GUID', 'FILE'))
     pgroup.add_argument('--add-kek', dest = 'kek',  action = 'append', nargs = 2,
@@ -202,14 +204,17 @@
 
     if options.set_fallback_verbose:
         varlist.set_uint32('FALLBACK_VERBOSE', 1)
 
     if options.set_fallback_no_reboot:
         varlist.set_uint32('FB_NO_REBOOT', 1)
 
+    if options.sbatlevel:
+        varlist.set_from_file('SbatLevel', options.sbatlevel)
+
     if options.set_json:
         with open(options.set_json, "r", encoding = 'utf-8') as f:
             l = json.loads(f.read(), object_hook = efijson.efi_decode)
         for (key, item) in l.items():
             logging.info('set variable %s from %s', key, options.set_json)
             varlist[key] = item
```

### Comparing `virt-firmware-23.5/virt/firmware/varstore/aws.py` & `virt-firmware-23.6/virt/firmware/varstore/aws.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-23.5/virt/firmware/varstore/edk2.py` & `virt-firmware-23.6/virt/firmware/varstore/edk2.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,41 +19,59 @@
         self.start    = None
         self.end      = None
 
         self.readfile()
         self.parse_volume()
 
     @staticmethod
+    def find_nvdata(data):
+        offset = 0
+        while offset + 64 < len(data):
+            guid = guids.parse_bin(data, offset + 16)
+            if str(guid) == guids.NvData:
+                return offset
+            if str(guid) == guids.Ffs:
+                (tlen, sig) = struct.unpack_from('<QL', data, offset + 32)
+                offset += tlen
+                continue
+            offset += 1024
+        return None
+
+    @staticmethod
     def probe(filename):
         with open(filename, "rb") as f:
-            header = f.read(64)
-        guid = guids.parse_bin(header, 16)
-        if str(guid) != guids.NvData:
+            data = f.read()
+        offset = Edk2VarStore.find_nvdata(data)
+        if offset is None:
             return False
         return True
 
     def readfile(self):
         logging.info('reading raw edk2 varstore from %s', self.filename)
         with open(self.filename, "rb") as f:
             self.filedata = f.read()
 
     def parse_volume(self):
-        guid = guids.parse_bin(self.filedata, 16)
+        offset = self.find_nvdata(self.filedata)
+        if offset is None:
+            logging.error('%s: varstore not found', self.filename)
+            sys.exit(1)
+        guid = guids.parse_bin(self.filedata, offset + 16)
         (vlen, sig, attr, hlen, csum, xoff, rev, blocks, blksize) = \
-            struct.unpack_from("=QLLHHHxBLL", self.filedata, 32)
+            struct.unpack_from("=QLLHHHxBLL", self.filedata, offset + 32)
         logging.debug('vol=%s vlen=0x%x rev=%d blocks=%d*%d (0x%x)',
                       guids.name(guid), vlen, rev,
                       blocks, blksize, blocks * blksize)
         if sig != 0x4856465f:
             logging.error('%s: not a firmware volume', self.filename)
             sys.exit(1)
         if str(guid) != guids.NvData:
             logging.error('%s: not a variable store', self.filename)
             sys.exit(1)
-        return self.parse_varstore(hlen)
+        return self.parse_varstore(offset + hlen)
 
     def parse_varstore(self, start):
         guid = guids.parse_bin(self.filedata, start)
         (size, storefmt, state) = struct.unpack_from("=LBB", self.filedata, start + 16)
         logging.debug('varstore=%s size=0x%x format=0x%x state=0x%x',
                       guids.name(guid), size, storefmt, state)
         if str(guid) != guids.AuthVars:
```

### Comparing `virt-firmware-23.5/virt/peutils/peutils.py` & `virt-firmware-23.6/virt/peutils/peutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,62 +26,62 @@
         bc = cert.extensions.get_extension_for_oid(x509.oid.ExtensionOID.BASIC_CONSTRAINTS)
     except x509.extensions.ExtensionNotFound:
         bc = False
     if bc:
         return bc.value.ca
     return False
 
-def print_cert(cert, verbose = False):
-    print('#          certificate')
+def print_cert(cert, ii, verbose = False):
+    print(f'# {ii}   certificate')
     if verbose:
-        print(f'#             subject: {cert.subject.rfc4514_string()}')
-        print(f'#             issuer : {cert.issuer.rfc4514_string()}')
-        print(f'#             valid  : {cert.not_valid_before} -> {cert.not_valid_after}')
-        print(f'#             CA     : {is_ca_cert(cert)}')
+        print(f'# {ii}      subject: {cert.subject.rfc4514_string()}')
+        print(f'# {ii}      issuer : {cert.issuer.rfc4514_string()}')
+        print(f'# {ii}      valid  : {cert.not_valid_before} -> {cert.not_valid_after}')
+        print(f'# {ii}      CA     : {is_ca_cert(cert)}')
     else:
         scn = common_name(cert.subject)
         icn = common_name(cert.issuer)
-        print(f'#             subject CN: {scn}')
-        print(f'#             issuer  CN: {icn}')
+        print(f'# {ii}      subject CN: {scn}')
+        print(f'# {ii}      issuer  CN: {icn}')
 
-def print_vendor_cert(db, verbose = False):
+def print_vendor_cert(db, ii, verbose = False):
     # VENDOR_CERT_FILE
     try:
         crt = x509.load_der_x509_certificate(db, default_backend())
-        print_cert(crt, verbose)
+        print_cert(crt, ii, verbose)
         return
     except ValueError:
         pass
 
     # VENDOR_DB_FILE
     sigdb = siglist.EfiSigDB(db)
     for sl in sigdb:
         if str(sl.guid) == guids.EfiCertX509:
-            print_cert(sl.x509, verbose)
+            print_cert(sl.x509, ii, verbose)
         elif str(sl.guid) == guids.EfiCertSha256:
-            print('#          sha256')
-            print(f'#             {len(sl)} entries')
+            print(f'# {ii}   sha256')
+            print(f'# {ii}      {len(sl)} entries')
         else:
-            print(f'#          {sl.guid}')
+            print(f'# {ii}   {sl.guid}')
 
-def print_sbat_entries(name, data):
-    print(f'#       {name}')
+def print_sbat_entries(ii, name, data):
+    print(f'# {ii}{name}')
     entries = data.decode().rstrip('\n').split('\n')
     for entry in entries:
-        print(f'#           {entry}')
+        print(f'# {ii}   {entry}')
 
-def sig_type2(data, extract = False, verbose = False):
+def sig_type2(data, ii, extract = False, verbose = False):
     certs = pkcs7.load_der_pkcs7_certificates(data)
     for cert in certs:
-        print_cert(cert, verbose)
+        print_cert(cert, ii, verbose)
 
         if extract:
             scn = common_name(cert.subject)
             fn = "".join(x for x in scn if x.isalnum()) + '.pem'
-            print(f'#             >>> {fn}')
+            print(f'# {ii}      >>> {fn}')
             with open(fn, 'wb') as f:
                 f.write(cert.public_bytes(serialization.Encoding.PEM))
 
 def getcstr(data):
     """ get C string (terminated by null byte) """
     idx = 0
     for b in data:
@@ -105,68 +105,96 @@
         r = 'r'
     if sec.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_WRITE']:
         w = 'w'
     if sec.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_EXECUTE']:
         x = 'x'
     return r + w + x
 
-def efi_binary(filename, extract = False, verbose = False):
-    print(f'# file: {filename}')
-    pe = pefile.PE(filename)
-    for sec in pe.sections:
-        if sec.Name.startswith(b'/'):
-            idx = getcstr(sec.Name[1:])
-            sec.Name = pe_string(pe, int(idx))
-        print(f'#    section: 0x{sec.PointerToRawData:06x} +0x{sec.SizeOfRawData:06x}'
-              f' {pe_section_flags(sec)}'
-              f' ({sec.Name.decode()})')
-        if sec.Name == b'.sbat\0\0\0':
-            sbat = sec.get_data()
-            entries = sbat.decode().rstrip('\n\0').split('\n')
-            for entry in entries:
-                print(f'#       {entry}')
-        if sec.Name == b'.vendor_cert':
-            vcert = sec.get_data()
-            (dbs, dbxs, dbo, dbxo) = struct.unpack_from('<IIII', vcert)
-            if dbs:
-                print(f'#       db: {dbo} +{dbs}')
-                db = vcert [ dbo : dbo + dbs ]
-                print_vendor_cert(db, verbose)
-            if dbxs:
-                print(f'#       dbx: {dbxo} +{dbxs}')
-                dbx = vcert [ dbxo : dbxo + dbxs ]
-                print_vendor_cert(dbx, verbose)
-        if sec.Name == b'.sbatlevel':
-            levels = sec.get_data()
-            (version, poff, loff) = struct.unpack_from('<III', levels)
-            print_sbat_entries('previous', getcstr(levels[poff + 4:]))
-            print_sbat_entries('latest', getcstr(levels[loff + 4:]))
-
+def pe_print_sigs(filename, pe, indent, extract, verbose):
+    i  = f'{"":{indent}s}'
+    ii = f'{"":{indent+3}s}'
     sighdr = pe.OPTIONAL_HEADER.DATA_DIRECTORY[4]
     if sighdr.VirtualAddress and sighdr.Size:
-        print(f'#    sigdata: 0x{sighdr.VirtualAddress:06x} +0x{sighdr.Size:06x}')
+        print(f'# {i}sigdata: 0x{sighdr.VirtualAddress:06x} +0x{sighdr.Size:06x}')
         sigs = pe.__data__[ sighdr.VirtualAddress :
                             sighdr.VirtualAddress + sighdr.Size ]
         pos = 0
         index = 0
         while pos + 8 < len(sigs):
             (slen, srev, stype) = struct.unpack_from('<LHH', sigs, pos)
-            print(f'#       signature: len 0x{slen:x}, type 0x{stype:x}')
+            print(f'# {ii}signature: len 0x{slen:x}, type 0x{stype:x}')
             if extract:
                 index += 1
                 fn = filename.split('/')[-1] + f'.sig{index}'
-                print(f'#       >>> {fn}')
+                print(f'# {ii}>>> {fn}')
                 with open(fn, 'wb') as f:
                     f.write(sigs [ pos : pos + slen ])
             if stype == 2:
                 sig_type2(sigs [ pos + 8 : pos + slen ],
-                          extract, verbose)
+                          ii, extract, verbose)
             pos += slen
             pos = (pos + 7) & ~7 # align
 
+# pylint: disable=too-many-branches
+def pe_print_section(pe, sec, indent, verbose):
+    i  = f'{"":{indent}s}'
+    ii = f'{"":{indent+3}s}'
+    if sec.Name.startswith(b'/'):
+        idx = getcstr(sec.Name[1:])
+        sec.Name = pe_string(pe, int(idx))
+    print(f'# {i}section: 0x{sec.PointerToRawData:08x} +0x{sec.SizeOfRawData:08x}'
+          f' {pe_section_flags(sec)}'
+          f' ({sec.Name.decode()})')
+    if sec.Name == b'.vendor_cert':
+        vcert = sec.get_data()
+        (dbs, dbxs, dbo, dbxo) = struct.unpack_from('<IIII', vcert)
+        if dbs:
+            print(f'# {ii}db: {dbo} +{dbs}')
+            db = vcert [ dbo : dbo + dbs ]
+            print_vendor_cert(db, ii, verbose)
+        if dbxs:
+            print(f'# {ii}dbx: {dbxo} +{dbxs}')
+            dbx = vcert [ dbxo : dbxo + dbxs ]
+            print_vendor_cert(dbx, ii, verbose)
+    if sec.Name == b'.sbatlevel':
+        levels = sec.get_data()
+        (version, poff, loff) = struct.unpack_from('<III', levels)
+        print_sbat_entries(ii, 'previous', getcstr(levels[poff + 4:]))
+        print_sbat_entries(ii, 'latest', getcstr(levels[loff + 4:]))
+    if sec.Name in (b'.sdmagic', b'.data.ident', b'.cmdline',
+                    b'.uname\0\0', b'.sbat\0\0\0'):
+        lines = sec.get_data().decode().rstrip('\n\0')
+        for line in lines.split('\n'):
+            print(f'# {ii}{line}')
+    if sec.Name == b'.osrel\0\0':
+        osrel = sec.get_data().decode().rstrip('\n\0')
+        entries = osrel.split('\n')
+        for entry in entries:
+            if entry.startswith('PRETTY_NAME'):
+                print(f'# {ii}{entry}')
+    if sec.Name == b'.linux\0\0':
+        print(f'# {ii}embedded binary')
+        try:
+            npe = pefile.PE(data = sec.get_data())
+            for nsec in npe.sections:
+                pe_print_section(npe, nsec, indent + 6, verbose)
+            pe_print_sigs(None, npe, indent + 6, False, verbose)
+        except pefile.PEFormatError:
+            print(f'# {ii}   not a PE binary')
+
+def efi_binary(filename, extract = False, verbose = False):
+    print(f'# file: {filename}')
+    try:
+        pe = pefile.PE(filename)
+        for sec in pe.sections:
+            pe_print_section(pe, sec, 3, verbose)
+        pe_print_sigs(filename, pe, 3, extract, verbose)
+    except pefile.PEFormatError:
+        print('#    not a PE binary')
+
 def read_sig(filename):
     print(f'# <<< {filename} (signature)')
     with open(filename, 'rb') as f:
         blob = f.read()
     while len(blob) & 7:
         blob += b'\0'
     return blob
```

### Comparing `virt-firmware-23.5/virt_firmware.egg-info/PKG-INFO` & `virt-firmware-23.6/virt_firmware.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virt-firmware
-Version: 23.5
+Version: 23.6
 Summary: tools for virtual machine firmware volumes
 Author: Gerd Hoffmann
 Author-email: kraxel@redhat.com
 License: GPLv2
 Project-URL: GitLab, https://gitlab.com/kraxel/virt-firmware
 Keywords: ovmf,armvirt,edk2,aws
 Description-Content-Type: text/markdown
```

### Comparing `virt-firmware-23.5/virt_firmware.egg-info/SOURCES.txt` & `virt-firmware-23.6/virt_firmware.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-experimental/bootcfg.py
 experimental/dbxupdate.py
 experimental/measure.py
 man/virt-fw-dump.1
 man/virt-fw-dump.inc
 man/virt-fw-sigdb.1
 man/virt-fw-sigdb.inc
 man/virt-fw-vars.1
 man/virt-fw-vars.inc
+tests/test-bootcfg.sh
 tests/test-dump.sh
 tests/test-pe.sh
 tests/test-sigdb.sh
 tests/test-vars.sh
 tests/tests.py
 tests/data/DBXUpdate-20100307.x64.bin
 tests/data/secboot.aws
@@ -24,14 +24,19 @@
 virt/firmware/dump.py
 virt/firmware/host.py
 virt/firmware/migrate.py
 virt/firmware/misc.py
 virt/firmware/sigdb.py
 virt/firmware/vars.py
 virt/firmware/aws/dict.v0
+virt/firmware/bootcfg/__init__.py
+virt/firmware/bootcfg/bootcfg.py
+virt/firmware/bootcfg/linuxcfg.py
+virt/firmware/bootcfg/main.py
+virt/firmware/bootcfg/menu.py
 virt/firmware/certs/CentOSSecureBootCA2.pem
 virt/firmware/certs/CentOSSecureBootCAkey1.pem
 virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
 virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
 virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
 virt/firmware/certs/RedHatSecureBootCA3.pem
 virt/firmware/certs/RedHatSecureBootCA5.pem
```

