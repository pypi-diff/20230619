# Comparing `tmp/keystoneauth1-5.2.0.tar.gz` & `tmp/keystoneauth1-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystoneauth1-5.2.0.tar", last modified: Wed May 17 11:03:14 2023, max compression
+gzip compressed data, was "keystoneauth1-5.2.1.tar", last modified: Mon Jun 19 14:09:39 2023, max compression
```

## Comparing `keystoneauth1-5.2.0.tar` & `keystoneauth1-5.2.1.tar`

### file list

```diff
@@ -1,323 +1,323 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8539 2023-05-17 11:03:13.000000 keystoneauth1-5.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43955 2023-05-17 11:03:13.000000 keystoneauth1-5.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11891 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.139093 keystoneauth1-5.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3174 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.139093 keystoneauth1-5.2.0/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/ext/list_plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.143093 keystoneauth1-5.2.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20657 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/authentication-plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7567 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2450 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/extras.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.143093 keystoneauth1-5.2.0/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/images/graphs_authComp.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/images/graphs_authCompDelegate.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/migrating.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/plugin-options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25823 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/using-sessions.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.143093 keystoneauth1-5.2.0/keystoneauth1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/_fair_semaphore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/access/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/access/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20111 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/access/access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24136 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/access/service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/access/service_providers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24392 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63222 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/discover.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/exceptions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2932 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/auth_plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1909 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12371 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/oidc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/response.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/service_providers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/_loading.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18677 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/adfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11111 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/saml2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3306 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2839 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/_loading.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/_loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2777 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/fixture/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11625 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2320 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5560 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/keystoneauth_betamax.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6281 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2969 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/serializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7705 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18080 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1585 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/http_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2991 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1852 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32471 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/identity/generic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/generic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9114 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/generic/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3447 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/generic/password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/generic/token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6285 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/identity/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/application_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12468 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4235 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6830 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/k2k.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/multi_factor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5133 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/oauth2_client_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5082 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/oauth2_mtls_client_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24908 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/oidc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3111 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/receipt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4706 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/tokenless_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3239 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/totp.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.155093 keystoneauth1-5.2.0/keystoneauth1/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2958 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.155093 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/admin_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1628 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/http_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.155093 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2728 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/generic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15077 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16394 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6349 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3759 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6452 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5612 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11147 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15084 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2959 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/service_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62863 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/session.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.155093 keystoneauth1-5.2.0/keystoneauth1/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8066 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v2_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11106 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v2_service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12168 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v3_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20956 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v3_service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/client_fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v2_sample_request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v2_sample_response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v3_sample_request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v3_sample_response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/ksa_betamax_test_cassette.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/ksa_serializer_data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/test_pre_record_hook.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/exceptions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/exceptions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1275 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/exceptions/test_exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_fedkerb_loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_kerberos_loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4754 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_mapped.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3078 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4601 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/test_oauth1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2149 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/test_oauth1_loading.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.135093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14138 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_RequestSecurityTokenResponse.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_fault.xml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3549 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/authn_request.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3698 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/saml_assertion.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/soap_response.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10747 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/test_auth_adfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12305 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/test_auth_saml2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2769 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    94579 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14472 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51660 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11461 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3_federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16077 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3_oidc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3974 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4615 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_tokenless_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6780 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5454 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/k2k_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/keystoneauth_fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11815 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8123 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8381 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_entry_points.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_generic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4279 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24004 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3223 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/matchers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3279 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/oidc_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6708 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_serializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51952 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_fair_sempahore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14190 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_hacking_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_http_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_matchers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_service_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    79474 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2633 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_token_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5556 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3230 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/token_endpoint.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.143093 keystoneauth1-5.2.0/keystoneauth1.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12051 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.139093 keystoneauth1-5.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.171093 keystoneauth1-5.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/1583780-700f99713e06324e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/add-oidc-client-credentials-2be065926ba4b849.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/add-oidc-discovery-document-support-b07fe54f83286d62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/add-prompt-to-opt-d083acc357a7f07b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/additional-headers-f2d16f85f5abe942.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/allow_version_hack-flag-9b53b72d9b084c04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/api-sig-error-guideline-handler.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/basic-http-auth-45bea4298209df75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bp-application-credentials-416a1f8bb2311e04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bp-support-oauth2-mtls-177cda05265ae65c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bp-system-scope-29e9c597039ddb1e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1582774-49af731b6dfc6f2f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1614688-c4a1bd54f4ba5644.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1616105-cc8b85eb056e99e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1654847-acdf9543158329ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1689424-set-adfspassword-endpointreference-f186d84a54007b09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1733052-1b4af3b3fe1b05bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1766235wq-0de60d0f996c6bfb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1839748-5d8dfc99c43aaefc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1876317-1db97d1b12a3e4b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1998366-27cd486b46fb56b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/cache-trailing-slash-3663c86cd9754379.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/cleanup-session-on-delete-1ed6177d4c5c1f83.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/client-side-rate-limiting-dec43fc9b54f5b70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/collect-timing-85f007f0d86c8b26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/drop-py-2-7-f90c67a5db0dfeb8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/drop-python-3-6-and-3-7-c407d5898c5eafec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/drop-python-3.5-362bb9d47f830353.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/expose-endpoint-status-6195a6b76d8a8de8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/filter-versions-service-type-763af68092344b7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/fix-get-all-version-data-a01ee58524755b9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/get-auth-ref-7418e13bd0942060.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/global_request_id-per-request-bd66c7e0f1a71d9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/improve-http-error-handling.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/ironic-discovery-fe41793ef97027bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/ironic-microversions-a69bf92ab21f0cf5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/ksa_2.2.0-81145229d4b43043.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/microversion-header-support-901acd820a21d788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/noauth-discovery-c26d82a32c36d41d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/none-auth-dab13ab9af6f5c86.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/oslo-config-split-loggers-6bda266d657fe921.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/retries-limit-dbaedcb3207934ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/retries-options-99e4dbc240941557.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/retry-delay-68d0c0a1dffcf2fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/serice-type-aliases-249454829c57f39a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/status-code-retries-75052a43efa4edb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/support-api-wg-discovery-2cb4b0186619e124.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/user-agent-generation-b069100508c06177.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/version-between-b4b0bcf4cecfb9e4.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9107 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3169 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.286376 keystoneauth1-5.2.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8605 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44141 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11891 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2530 2023-06-19 14:09:39.286376 keystoneauth1-5.2.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.262375 keystoneauth1-5.2.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3174 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.262375 keystoneauth1-5.2.1/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/ext/list_plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20657 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/authentication-plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7567 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2450 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/extras.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/images/graphs_authComp.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/images/graphs_authCompDelegate.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/migrating.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/plugin-options.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25823 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/doc/source/using-sessions.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/keystoneauth1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/_fair_semaphore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/keystoneauth1/access/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/access/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20111 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/access/access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24136 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/access/service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/access/service_providers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24392 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63222 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/discover.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/keystoneauth1/exceptions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2932 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/auth_plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1909 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12371 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/oidc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/response.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/exceptions/service_providers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/keystoneauth1/extras/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/_loading.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18677 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/adfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11111 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/saml2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/extras/kerberos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3306 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/kerberos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2839 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/kerberos/_loading.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/extras/oauth1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/oauth1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/oauth1/_loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2777 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/extras/oauth1/v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/fixture/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11625 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2320 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5560 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/keystoneauth_betamax.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6281 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2969 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/serializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7705 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18080 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/fixture/v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1585 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/http_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2991 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1852 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32471 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/identity/generic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/generic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9114 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/generic/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3447 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/generic/password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/generic/token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6285 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/application_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12468 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4235 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6830 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/k2k.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/multi_factor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5133 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/oauth2_client_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5061 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/oauth2_mtls_client_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24975 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/oidc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3111 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/receipt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4706 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/tokenless_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3239 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/identity/v3/totp.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2958 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.270375 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/admin_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1628 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/http_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.274375 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2728 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/identity/generic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/identity/v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15077 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/identity/v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16394 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6349 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3759 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6452 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5612 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11147 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/loading/session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15084 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2959 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/service_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62863 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/session.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.274375 keystoneauth1-5.2.1/keystoneauth1/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.274375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.274375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8066 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/test_v2_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11106 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/test_v2_service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12168 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/test_v3_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20956 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/test_v3_service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/client_fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.274375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/keystone_v2_sample_request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/keystone_v2_sample_response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/keystone_v3_sample_request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/keystone_v3_sample_response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/ksa_betamax_test_cassette.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/ksa_serializer_data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/test_pre_record_hook.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.274375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/exceptions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/exceptions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1275 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/exceptions/test_exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.274375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.278375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/test_fedkerb_loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/test_kerberos_loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4754 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/test_mapped.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/test_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3078 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.278375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/oauth1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/oauth1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4601 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/oauth1/test_oauth1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2149 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/oauth1/test_oauth1_loading.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.278375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.262375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/examples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.278375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/examples/xml/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14138 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_RequestSecurityTokenResponse.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_fault.xml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.278375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3549 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.278375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/authn_request.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3698 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/saml_assertion.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/soap_response.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10747 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/test_auth_adfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12305 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/test_auth_saml2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.278375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2769 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    94579 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14472 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51660 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11461 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_v3_federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16077 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_v3_oidc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3974 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4615 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_tokenless_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6780 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5454 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/k2k_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/keystoneauth_fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.278375 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11815 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8123 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8381 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_entry_points.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_generic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4279 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24004 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3223 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/matchers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3279 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/oidc_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_betamax_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6708 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_betamax_hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_betamax_serializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51952 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_fair_sempahore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14190 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_hacking_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_http_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_matchers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_service_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    79474 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2633 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_token_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5556 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/tests/unit/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3230 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/keystoneauth1/token_endpoint.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.266375 keystoneauth1-5.2.1/keystoneauth1.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2530 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/keystoneauth1.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12051 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/keystoneauth1.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/keystoneauth1.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/keystoneauth1.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/keystoneauth1.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/keystoneauth1.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/keystoneauth1.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-06-19 14:09:39.000000 keystoneauth1-5.2.1/keystoneauth1.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.262375 keystoneauth1-5.2.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.282375 keystoneauth1-5.2.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/1583780-700f99713e06324e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/add-oidc-client-credentials-2be065926ba4b849.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/add-oidc-discovery-document-support-b07fe54f83286d62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/add-prompt-to-opt-d083acc357a7f07b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/additional-headers-f2d16f85f5abe942.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/allow_version_hack-flag-9b53b72d9b084c04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/api-sig-error-guideline-handler.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/basic-http-auth-45bea4298209df75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bp-application-credentials-416a1f8bb2311e04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bp-support-oauth2-mtls-177cda05265ae65c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bp-system-scope-29e9c597039ddb1e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1582774-49af731b6dfc6f2f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1614688-c4a1bd54f4ba5644.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1616105-cc8b85eb056e99e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1654847-acdf9543158329ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1689424-set-adfspassword-endpointreference-f186d84a54007b09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1733052-1b4af3b3fe1b05bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1766235wq-0de60d0f996c6bfb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1839748-5d8dfc99c43aaefc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1876317-1db97d1b12a3e4b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/bug-1998366-27cd486b46fb56b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/cache-trailing-slash-3663c86cd9754379.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/cleanup-session-on-delete-1ed6177d4c5c1f83.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/client-side-rate-limiting-dec43fc9b54f5b70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/collect-timing-85f007f0d86c8b26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/drop-py-2-7-f90c67a5db0dfeb8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/drop-python-3-6-and-3-7-c407d5898c5eafec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/drop-python-3.5-362bb9d47f830353.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/expose-endpoint-status-6195a6b76d8a8de8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/filter-versions-service-type-763af68092344b7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/fix-get-all-version-data-a01ee58524755b9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/get-auth-ref-7418e13bd0942060.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/global_request_id-per-request-bd66c7e0f1a71d9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/improve-http-error-handling.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/ironic-discovery-fe41793ef97027bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/ironic-microversions-a69bf92ab21f0cf5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/ksa_2.2.0-81145229d4b43043.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/microversion-header-support-901acd820a21d788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/noauth-discovery-c26d82a32c36d41d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/none-auth-dab13ab9af6f5c86.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/oslo-config-split-loggers-6bda266d657fe921.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/retries-limit-dbaedcb3207934ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/retries-options-99e4dbc240941557.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/retry-delay-68d0c0a1dffcf2fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/serice-type-aliases-249454829c57f39a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/status-code-retries-75052a43efa4edb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/support-api-wg-discovery-2cb4b0186619e124.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/user-agent-generation-b069100508c06177.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/notes/version-between-b4b0bcf4cecfb9e4.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.286376 keystoneauth1-5.2.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.286376 keystoneauth1-5.2.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:39.286376 keystoneauth1-5.2.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9107 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2023-06-19 14:09:39.286376 keystoneauth1-5.2.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3169 2023-06-19 14:09:12.000000 keystoneauth1-5.2.1/tox.ini
```

### Comparing `keystoneauth1-5.2.0/AUTHORS` & `keystoneauth1-5.2.1/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 Colleen Murphy <colleen.murphy@suse.de>
 Colleen Murphy <colleen@gazlene.net>
 Corey Bryant <corey.bryant@canonical.com>
 Cyril Roelandt <cyril.roelandt@enovance.com>
 Cyril Roelandt <cyril@redhat.com>
 Dan Prince <dprince@redhat.com>
 Dave Chen <wei.d.chen@intel.com>
+Dave Wilde <dwilde@redhat.com>
 David Stanek <dstanek@dstanek.com>
 Dean Troyer <dtroyer@gmail.com>
 Dirk Mueller <dirk@dmllr.de>
 Dmitry Tantsur <divius.inside@gmail.com>
 Dmitry Tantsur <dtantsur@protonmail.com>
 Dolph Mathews <dolph.mathews@gmail.com>
 Doug Fish <drfish@us.ibm.com>
@@ -153,14 +154,15 @@
 Sergey Kraynev <skraynev@mirantis.com>
 Sergio Cazzolato <sergio.j.cazzolato@intel.com>
 Simon Li <libo04@inspur.com>
 Stephen Finucane <stephenfin@redhat.com>
 Steve Baker <sbaker@redhat.com>
 Steve Martinelli <s.martinelli@gmail.com>
 Steve Martinelli <stevemar@ca.ibm.com>
+Steve Relf <s.relf@eschercloud.ai>
 Steven Hardy <shardy@redhat.com>
 Stuart McLaren <stuart.mclaren@hp.com>
 Sushil Kumar <sushil.kumar2@globallogic.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Tang Chen <chen.tang@easystack.cn>
 TerryHowe <terrylhowe@gmail.com>
 Thierry Carrez <thierry@openstack.org>
```

### Comparing `keystoneauth1-5.2.0/CONTRIBUTING.rst` & `keystoneauth1-5.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/ChangeLog` & `keystoneauth1-5.2.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 CHANGES
 =======
 
+5.2.1
+-----
+
+* Remove last reference to the python six package
+* Make v3oidcpassword send client\_id
+* Add RFC required headers and data to the request
+
 5.2.0
 -----
 
 * Update master for stable/2023.1
+* Fix up some packaging metadata
 * New auth plugin v3oidcdeviceauthz
 * OAuth 2.0 Mutual-TLS Support
 
 5.1.2
 -----
 
 * Fix docs build for tox4
```

### Comparing `keystoneauth1-5.2.0/HACKING.rst` & `keystoneauth1-5.2.1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/LICENSE` & `keystoneauth1-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/PKG-INFO` & `keystoneauth1-5.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystoneauth1
-Version: 5.2.0
+Version: 5.2.1
 Summary: Authentication Library for OpenStack Identity
 Home-page: https://docs.openstack.org/keystoneauth/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -53,12 +53,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: betamax
 Provides-Extra: kerberos
 Provides-Extra: oauth1
 Provides-Extra: saml2
 Provides-Extra: test
```

### Comparing `keystoneauth1-5.2.0/README.rst` & `keystoneauth1-5.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/Makefile` & `keystoneauth1-5.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/ext/list_plugins.py` & `keystoneauth1-5.2.1/doc/ext/list_plugins.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/requirements.txt` & `keystoneauth1-5.2.1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/authentication-plugins.rst` & `keystoneauth1-5.2.1/doc/source/authentication-plugins.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/conf.py` & `keystoneauth1-5.2.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/extras.rst` & `keystoneauth1-5.2.1/doc/source/extras.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/images/graphs_authComp.svg` & `keystoneauth1-5.2.1/doc/source/images/graphs_authComp.svg`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/images/graphs_authCompDelegate.svg` & `keystoneauth1-5.2.1/doc/source/images/graphs_authCompDelegate.svg`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/index.rst` & `keystoneauth1-5.2.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/migrating.rst` & `keystoneauth1-5.2.1/doc/source/migrating.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/plugin-options.rst` & `keystoneauth1-5.2.1/doc/source/plugin-options.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/doc/source/using-sessions.rst` & `keystoneauth1-5.2.1/doc/source/using-sessions.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/_fair_semaphore.py` & `keystoneauth1-5.2.1/keystoneauth1/_fair_semaphore.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/_utils.py` & `keystoneauth1-5.2.1/keystoneauth1/_utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/access/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/access/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/access/access.py` & `keystoneauth1-5.2.1/keystoneauth1/access/access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/access/service_catalog.py` & `keystoneauth1-5.2.1/keystoneauth1/access/service_catalog.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/access/service_providers.py` & `keystoneauth1-5.2.1/keystoneauth1/access/service_providers.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/adapter.py` & `keystoneauth1-5.2.1/keystoneauth1/adapter.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/discover.py` & `keystoneauth1-5.2.1/keystoneauth1/discover.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/auth.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/auth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/auth_plugins.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/auth_plugins.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/base.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/catalog.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/catalog.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/connection.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/connection.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/discovery.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/discovery.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/http.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/oidc.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/oidc.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/response.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/response.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/exceptions/service_providers.py` & `keystoneauth1-5.2.1/keystoneauth1/exceptions/service_providers.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/_loading.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/adfs.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/adfs.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/base.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/saml2.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/_saml2/v3/saml2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/kerberos/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/_loading.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/kerberos/_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/oauth1/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/_loading.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/oauth1/_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/v3.py` & `keystoneauth1-5.2.1/keystoneauth1/extras/oauth1/v3.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/discovery.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/discovery.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/exception.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/exception.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/hooks.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/hooks.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/keystoneauth_betamax.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/keystoneauth_betamax.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/plugin.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/plugin.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/serializer.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/serializer.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/v2.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/v2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/fixture/v3.py` & `keystoneauth1-5.2.1/keystoneauth1/fixture/v3.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/hacking/checks.py` & `keystoneauth1-5.2.1/keystoneauth1/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/http_basic.py` & `keystoneauth1-5.2.1/keystoneauth1/http_basic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/access.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/base.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/generic/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/generic/base.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/generic/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/generic/password.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/generic/password.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/generic/token.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/generic/token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v2.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/application_credential.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/application_credential.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/base.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/federation.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/federation.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/k2k.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/k2k.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/multi_factor.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/multi_factor.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/oauth2_client_credential.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/oauth2_client_credential.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/oauth2_mtls_client_credential.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/oauth2_mtls_client_credential.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
 
-import six
-
 from keystoneauth1 import access
 from keystoneauth1 import exceptions
 from keystoneauth1.identity.v3 import base
 
 
-@six.add_metaclass(abc.ABCMeta)
-class OAuth2mTlsClientCredential(base.BaseAuth):
+class OAuth2mTlsClientCredential(base.BaseAuth, metaclass=abc.ABCMeta):
     """A plugin for authenticating via an OAuth2.0 mTLS client credential.
 
     :param string auth_url: keystone authorization endpoint.
     :param string oauth2_endpoint: OAuth2.0 endpoint.
     :param string oauth2_client_id: OAuth2.0 client credential id.
     """
```

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/oidc.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,16 @@
         :type session: keystoneauth1.session.Session
 
         :returns: a python dictionary containing the payload to be exchanged
         :rtype: dict
         """
         payload = {'username': self.username,
                    'password': self.password,
-                   'scope': self.scope}
+                   'scope': self.scope,
+                   'client_id': self.client_id}
         return payload
 
 
 class OidcClientCredentials(_OidcBase):
     """Implementation for OpenID Connect Client Credentials."""
 
     grant_type = 'client_credentials'
@@ -545,15 +546,15 @@
         :rtype: dict
         """
         client_auth = (self.client_id, self.client_secret)
         device_authz_endpoint = \
             self._get_device_authorization_endpoint(session)
         op_response = session.post(device_authz_endpoint,
                                    requests_auth=client_auth,
-                                   data={},
+                                   headers=self.HEADER_X_FORM,
                                    authenticated=False)
 
         self.expires_in = int(op_response.json()["expires_in"])
         self.timeout = time.time() + self.expires_in
         self.device_code = op_response.json()["device_code"]
         self.interval = int(op_response.json()["interval"])
         self.user_code = op_response.json()["user_code"]
```

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/password.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/password.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/receipt.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/receipt.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/token.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/tokenless_auth.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/tokenless_auth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/identity/v3/totp.py` & `keystoneauth1-5.2.1/keystoneauth1/identity/v3/totp.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/admin_token.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/admin_token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/http_basic.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/http_basic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/generic.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/identity/generic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/v2.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/identity/v2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/v3.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/identity/v3.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/noauth.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/_plugins/noauth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/_utils.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/_utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/adapter.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/adapter.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/base.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/cli.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/cli.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/conf.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/conf.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/identity.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/identity.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/opts.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/opts.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/loading/session.py` & `keystoneauth1-5.2.1/keystoneauth1/loading/session.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/noauth.py` & `keystoneauth1-5.2.1/keystoneauth1/noauth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/plugin.py` & `keystoneauth1-5.2.1/keystoneauth1/plugin.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/service_token.py` & `keystoneauth1-5.2.1/keystoneauth1/service_token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/session.py` & `keystoneauth1-5.2.1/keystoneauth1/session.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v2_access.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/test_v2_access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v2_service_catalog.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/test_v2_service_catalog.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v3_access.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/test_v3_access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v3_service_catalog.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/access/test_v3_service_catalog.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/client_fixtures.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v2_sample_response.json` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/keystone_v2_sample_response.json`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v3_sample_response.json` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/keystone_v3_sample_response.json`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/ksa_betamax_test_cassette.yaml` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/ksa_betamax_test_cassette.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/ksa_serializer_data.json` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/data/ksa_serializer_data.json`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/exceptions/test_exceptions.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/exceptions/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/base.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_fedkerb_loading.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/test_fedkerb_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_kerberos_loading.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/test_kerberos_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_mapped.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/test_mapped.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_v3.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/test_v3.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/utils.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/kerberos/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/test_oauth1.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/oauth1/test_oauth1.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/test_oauth1_loading.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/oauth1/test_oauth1_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_RequestSecurityTokenResponse.xml` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_RequestSecurityTokenResponse.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_fault.xml` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_fault.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/__init__.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/authn_request.xml` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/authn_request.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/saml_assertion.xml` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/saml_assertion.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/soap_response.xml` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/soap_response.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/test_auth_adfs.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/test_auth_adfs.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/test_auth_saml2.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/test_auth_saml2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/utils.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/extras/saml2/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_access.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_common.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_common.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v2.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_v2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_v3.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3_federation.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_v3_federation.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3_oidc.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_identity_v3_oidc.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_password.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_password.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_token.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_tokenless_auth.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/test_tokenless_auth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/utils.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/identity/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/k2k_fixtures.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/k2k_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/keystoneauth_fixtures.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/keystoneauth_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_adapter.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_adapter.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_cli.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_cli.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_conf.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_conf.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_entry_points.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_fixtures.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_generic.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_generic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_loading.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_session.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_session.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_v3.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/test_v3.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/utils.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/loading/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/matchers.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/matchers.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/oidc_fixtures.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/oidc_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_fixture.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_betamax_fixture.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_hooks.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_betamax_hooks.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_serializer.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_betamax_serializer.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_discovery.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_fair_sempahore.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_fair_sempahore.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_fixtures.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_hacking_checks.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_hacking_checks.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_http_basic.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_http_basic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_matchers.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_matchers.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_noauth.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_noauth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_service_token.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_service_token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_session.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_token_endpoint.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_token_endpoint.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_utils.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/tests/unit/utils.py` & `keystoneauth1-5.2.1/keystoneauth1/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1/token_endpoint.py` & `keystoneauth1-5.2.1/keystoneauth1/token_endpoint.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1.egg-info/PKG-INFO` & `keystoneauth1-5.2.1/keystoneauth1.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystoneauth1
-Version: 5.2.0
+Version: 5.2.1
 Summary: Authentication Library for OpenStack Identity
 Home-page: https://docs.openstack.org/keystoneauth/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -53,12 +53,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: betamax
 Provides-Extra: kerberos
 Provides-Extra: oauth1
 Provides-Extra: saml2
 Provides-Extra: test
```

### Comparing `keystoneauth1-5.2.0/keystoneauth1.egg-info/SOURCES.txt` & `keystoneauth1-5.2.1/keystoneauth1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1.egg-info/entry_points.txt` & `keystoneauth1-5.2.1/keystoneauth1.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/keystoneauth1.egg-info/requires.txt` & `keystoneauth1-5.2.1/keystoneauth1.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml` & `keystoneauth1-5.2.1/releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml` & `keystoneauth1-5.2.1/releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/releasenotes/notes/bp-support-oauth2-mtls-177cda05265ae65c.yaml` & `keystoneauth1-5.2.1/releasenotes/notes/bp-support-oauth2-mtls-177cda05265ae65c.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml` & `keystoneauth1-5.2.1/releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml` & `keystoneauth1-5.2.1/releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/releasenotes/notes/user-agent-generation-b069100508c06177.yaml` & `keystoneauth1-5.2.1/releasenotes/notes/user-agent-generation-b069100508c06177.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/releasenotes/source/conf.py` & `keystoneauth1-5.2.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/requirements.txt` & `keystoneauth1-5.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/setup.cfg` & `keystoneauth1-5.2.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [metadata]
 name = keystoneauth1
 summary = Authentication Library for OpenStack Identity
 description_file = 
 	README.rst
+long_description_content_type = text/x-rst
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 home_page = https://docs.openstack.org/keystoneauth/latest/
 python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
```

### Comparing `keystoneauth1-5.2.0/setup.py` & `keystoneauth1-5.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/test-requirements.txt` & `keystoneauth1-5.2.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.2.0/tox.ini` & `keystoneauth1-5.2.1/tox.ini`

 * *Files identical despite different names*

