# Comparing `tmp/certipy-ad-4.5.0.tar.gz` & `tmp/certipy-ad-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certipy-ad-4.5.0.tar", last modified: Sun Jun 18 12:52:52 2023, max compression
+gzip compressed data, was "certipy-ad-4.5.1.tar", last modified: Mon Jun 19 12:08:47 2023, max compression
```

## Comparing `certipy-ad-4.5.0.tar` & `certipy-ad-4.5.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.937928 certipy-ad-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-06-18 12:52:52.937928 certipy-ad-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40570 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.929927 certipy-ad-4.5.0/certipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.929927 certipy-ad-4.5.0/certipy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8712 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22273 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34330 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/cert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    41865 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7949 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/forge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.933927 certipy-ad-4.5.0/certipy/commands/parsers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      224 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2115 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/cert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2590 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/forge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/ptt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2858 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/relay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3336 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/req.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1454 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/shadow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2903 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/target.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/template.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3094 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/ptt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15754 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/relay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25062 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/req.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/shadow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8468 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/template.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.933927 certipy-ad-4.5.0/certipy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27227 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/certificate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17569 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2382 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10035 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/kerberos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14144 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/ldap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2332 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10623 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/pkinit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5138 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/rpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.933927 certipy-ad-4.5.0/certipy/lib/sspi/
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/sspi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32016 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/sspi/encryption.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/sspi/kerberos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    52996 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/sspi/netsecapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37531 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/structs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10790 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/target.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      396 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.937928 certipy-ad-4.5.0/certipy_ad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 12:52:52.937928 certipy-ad-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:47.958757 certipy-ad-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-06-19 12:08:47.958757 certipy-ad-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40570 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:47.950758 certipy-ad-4.5.1/certipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:47.950758 certipy-ad-4.5.1/certipy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8712 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22273 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34330 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/cert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41865 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7949 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/forge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:47.954758 certipy-ad-4.5.1/certipy/commands/parsers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      224 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2115 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/cert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2590 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/forge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/ptt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2858 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/relay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3336 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/req.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1454 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/shadow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2903 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/target.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/parsers/template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3094 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/ptt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15754 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/relay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25062 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/req.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/shadow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8468 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/commands/template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:47.954758 certipy-ad-4.5.1/certipy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27227 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/certificate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17569 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2382 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10035 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/kerberos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14144 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/ldap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2332 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10623 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/pkinit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5138 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/rpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:47.954758 certipy-ad-4.5.1/certipy/lib/sspi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/sspi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32016 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/sspi/encryption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/sspi/kerberos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52996 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/sspi/netsecapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37531 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/structs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10790 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/lib/target.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      396 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/certipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:08:47.958757 certipy-ad-4.5.1/certipy_ad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-06-19 12:08:47.000000 certipy-ad-4.5.1/certipy_ad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-19 12:08:47.000000 certipy-ad-4.5.1/certipy_ad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:08:47.000000 certipy-ad-4.5.1/certipy_ad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 12:08:47.000000 certipy-ad-4.5.1/certipy_ad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 12:08:47.000000 certipy-ad-4.5.1/certipy_ad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 12:08:47.000000 certipy-ad-4.5.1/certipy_ad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:08:47.958757 certipy-ad-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-19 12:08:30.000000 certipy-ad-4.5.1/setup.py
```

### Comparing `certipy-ad-4.5.0/LICENSE` & `certipy-ad-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/PKG-INFO` & `certipy-ad-4.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certipy-ad
-Version: 4.5.0
+Version: 4.5.1
 Summary: Active Directory Certificate Services enumeration and abuse
 Home-page: https://github.com/ly4k/Certipy
 Author: ly4k
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `certipy-ad-4.5.0/README.md` & `certipy-ad-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/account.py` & `certipy-ad-4.5.1/certipy/commands/account.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/auth.py` & `certipy-ad-4.5.1/certipy/commands/auth.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/ca.py` & `certipy-ad-4.5.1/certipy/commands/ca.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/cert.py` & `certipy-ad-4.5.1/certipy/commands/cert.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/find.py` & `certipy-ad-4.5.1/certipy/commands/find.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/forge.py` & `certipy-ad-4.5.1/certipy/commands/forge.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/account.py` & `certipy-ad-4.5.1/certipy/commands/parsers/account.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/auth.py` & `certipy-ad-4.5.1/certipy/commands/parsers/auth.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/ca.py` & `certipy-ad-4.5.1/certipy/commands/parsers/ca.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/cert.py` & `certipy-ad-4.5.1/certipy/commands/parsers/cert.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/find.py` & `certipy-ad-4.5.1/certipy/commands/parsers/find.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/forge.py` & `certipy-ad-4.5.1/certipy/commands/parsers/forge.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/ptt.py` & `certipy-ad-4.5.1/certipy/commands/parsers/ptt.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/relay.py` & `certipy-ad-4.5.1/certipy/commands/parsers/relay.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/req.py` & `certipy-ad-4.5.1/certipy/commands/parsers/req.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/shadow.py` & `certipy-ad-4.5.1/certipy/commands/parsers/shadow.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/target.py` & `certipy-ad-4.5.1/certipy/commands/parsers/target.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/parsers/template.py` & `certipy-ad-4.5.1/certipy/commands/parsers/template.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/ptt.py` & `certipy-ad-4.5.1/certipy/commands/ptt.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/relay.py` & `certipy-ad-4.5.1/certipy/commands/relay.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/req.py` & `certipy-ad-4.5.1/certipy/commands/req.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/shadow.py` & `certipy-ad-4.5.1/certipy/commands/shadow.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/commands/template.py` & `certipy-ad-4.5.1/certipy/commands/template.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/entry.py` & `certipy-ad-4.5.1/certipy/entry.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/certificate.py` & `certipy-ad-4.5.1/certipy/lib/certificate.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/constants.py` & `certipy-ad-4.5.1/certipy/lib/constants.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/errors.py` & `certipy-ad-4.5.1/certipy/lib/errors.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/formatting.py` & `certipy-ad-4.5.1/certipy/lib/formatting.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/kerberos.py` & `certipy-ad-4.5.1/certipy/lib/kerberos.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/ldap.py` & `certipy-ad-4.5.1/certipy/lib/ldap.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/logger.py` & `certipy-ad-4.5.1/certipy/lib/logger.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/pkinit.py` & `certipy-ad-4.5.1/certipy/lib/pkinit.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/rpc.py` & `certipy-ad-4.5.1/certipy/lib/rpc.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/security.py` & `certipy-ad-4.5.1/certipy/lib/security.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/sspi/encryption.py` & `certipy-ad-4.5.1/certipy/lib/sspi/encryption.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/sspi/kerberos.py` & `certipy-ad-4.5.1/certipy/lib/sspi/kerberos.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/sspi/netsecapi.py` & `certipy-ad-4.5.1/certipy/lib/sspi/netsecapi.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/structs.py` & `certipy-ad-4.5.1/certipy/lib/structs.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy/lib/target.py` & `certipy-ad-4.5.1/certipy/lib/target.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/certipy_ad.egg-info/PKG-INFO` & `certipy-ad-4.5.1/certipy_ad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certipy-ad
-Version: 4.5.0
+Version: 4.5.1
 Summary: Active Directory Certificate Services enumeration and abuse
 Home-page: https://github.com/ly4k/Certipy
 Author: ly4k
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `certipy-ad-4.5.0/certipy_ad.egg-info/SOURCES.txt` & `certipy-ad-4.5.1/certipy_ad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.5.0/setup.py` & `certipy-ad-4.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="certipy-ad",
-    version="4.5.0",
+    version="4.5.1",
     license="MIT",
     author="ly4k",
     url="https://github.com/ly4k/Certipy",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=[
         "asn1crypto",
-        "cryptography>=37.0",
+        "cryptography>=39.0",
         "impacket",
         "ldap3",
         "pyasn1==0.4.8",
         "dnspython",
         "dsinternals",
-        "pyopenssl>=22.0.0",
+        "pyopenssl>=23.0.0",
         "requests",
         "requests_ntlm",
         'winacl; platform_system=="Windows"',
         'wmi; platform_system=="Windows"',
         "pycryptodome",
         "unicrypto"
     ],
```

