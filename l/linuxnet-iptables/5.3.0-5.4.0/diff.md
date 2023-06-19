# Comparing `tmp/linuxnet-iptables-5.3.0.tar.gz` & `tmp/linuxnet-iptables-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxnet-iptables-5.3.0.tar", last modified: Mon Jun  5 00:26:37 2023, max compression
+gzip compressed data, was "linuxnet-iptables-5.4.0.tar", last modified: Mon Jun 19 04:01:18 2023, max compression
```

## Comparing `linuxnet-iptables-5.3.0.tar` & `linuxnet-iptables-5.4.0.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/
--rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-5.3.0/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)     2807 2023-06-05 00:21:56.000000 linuxnet-iptables-5.3.0/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-5.3.0/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-5.3.0/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/README.md
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.274196 linuxnet-iptables-5.3.0/docs/
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-5.3.0/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/docs/chain.rst
--rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-5.3.0/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/exception.rst
--rw-r--r--   0 panos     (1001) users      (100)     8374 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/docs/iptables_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     3176 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/match-example.py
--rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-5.3.0/docs/match.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.278196 linuxnet-iptables-5.3.0/docs/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/commentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-5.3.0/docs/matches/connmarkmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/conntrackmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/icmpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-5.3.0/docs/matches/limitmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/markmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/ownermatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-5.3.0/docs/matches/packetmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/packettypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/statematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1492 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/tcpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/tcpmssmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/ttlmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/udpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/docs/rule.rst
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-5.3.0/docs/table.rst
--rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/target-example.py
--rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-5.3.0/docs/target.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.280196 linuxnet-iptables-5.3.0/docs/targets/
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/chaintarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/connmarktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/dnattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/logtarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/marktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/masqueradetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/docs/targets/notracktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/rejecttarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/snattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/docs/targets/tracetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/ttltarget.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.280196 linuxnet-iptables-5.3.0/linuxnet/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.3.0/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.281196 linuxnet-iptables-5.3.0/linuxnet/iptables/
--rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    25090 2023-06-05 00:20:02.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/chain.py
--rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/extension.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.284196 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1295 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     2889 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/commentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2271 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/connmarkmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5226 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/conntrackmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     9769 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/icmpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4667 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/limitmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3852 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/markmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    14678 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/match.py
--rw-r--r--   0 panos     (1001) users      (100)     7798 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/ownermatch.py
--rw-r--r--   0 panos     (1001) users      (100)     7343 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/packetmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2844 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/packettypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     3155 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/statematch.py
--rw-r--r--   0 panos     (1001) users      (100)    10665 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/tcpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3833 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/tcpmssmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4322 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/ttlmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2724 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/udpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5060 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/util.py
--rw-r--r--   0 panos     (1001) users      (100)      918 2023-06-05 00:20:02.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/parsing.py
--rw-r--r--   0 panos     (1001) users      (100)    16442 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/rule.py
--rw-r--r--   0 panos     (1001) users      (100)    29087 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/table.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.285196 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/
--rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/connmarktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/logtarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/marktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/masqueradetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/nattarget.py
--rw-r--r--   0 panos     (1001) users      (100)     1414 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/notracktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/rejecttarget.py
--rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/target.py
--rw-r--r--   0 panos     (1001) users      (100)     1396 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/tracetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/ttltarget.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-05 00:26:37.000000 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     2625 2023-06-05 00:26:37.000000 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2023-06-05 00:26:37.000000 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2023-06-05 00:26:37.000000 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/top_level.txt
--rw-r--r--   0 panos     (1001) users      (100)       38 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/setup.cfg
--rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:20:19.000000 linuxnet-iptables-5.3.0/setup.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.3.0/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    58452 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/tests/iptables_test.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/
+-rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-5.4.0/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)     2943 2023-06-19 03:07:11.000000 linuxnet-iptables-5.4.0/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-5.4.0/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-5.4.0/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/README.md
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.338386 linuxnet-iptables-5.4.0/docs/
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-5.4.0/docs/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/docs/chain.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-5.4.0/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/exception.rst
+-rw-r--r--   0 panos     (1001) users      (100)     8374 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/extensibility.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/docs/iptables_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3176 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/match-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-5.4.0/docs/match.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.341386 linuxnet-iptables-5.4.0/docs/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 03:00:51.000000 linuxnet-iptables-5.4.0/docs/matches/addrtypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/commentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-5.4.0/docs/matches/connmarkmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/conntrackmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/icmpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-5.4.0/docs/matches/limitmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/markmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/ownermatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-5.4.0/docs/matches/packetmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/packettypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/statematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1492 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/tcpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/tcpmssmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/ttlmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/udpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/docs/rule.rst
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-5.4.0/docs/table.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/target-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-5.4.0/docs/target.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.343387 linuxnet-iptables-5.4.0/docs/targets/
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/chaintarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/connmarktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/dnattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/logtarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/marktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/masqueradetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-5.4.0/docs/targets/notracktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/rejecttarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/snattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-5.4.0/docs/targets/tracetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/ttltarget.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.343387 linuxnet-iptables-5.4.0/linuxnet/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.4.0/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.344386 linuxnet-iptables-5.4.0/linuxnet/iptables/
+-rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    25234 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/chain.py
+-rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/extension.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.346387 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1339 2023-06-19 03:00:49.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     5239 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/addrtypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2889 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/commentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2271 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/connmarkmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5226 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/conntrackmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9769 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/icmpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4667 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/limitmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3852 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/markmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    14678 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/match.py
+-rw-r--r--   0 panos     (1001) users      (100)     7798 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/ownermatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     7343 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/packetmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2844 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/packettypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3155 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/statematch.py
+-rw-r--r--   0 panos     (1001) users      (100)    10665 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/tcpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3833 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/tcpmssmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4322 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/ttlmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2724 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/udpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5782 2023-06-19 03:00:49.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/util.py
+-rw-r--r--   0 panos     (1001) users      (100)      918 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/parsing.py
+-rw-r--r--   0 panos     (1001) users      (100)    16442 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/rule.py
+-rw-r--r--   0 panos     (1001) users      (100)    29087 2023-06-04 01:25:41.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/table.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.348387 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/
+-rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/connmarktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/logtarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/marktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/masqueradetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/nattarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 03:00:49.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/notracktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/rejecttarget.py
+-rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/target.py
+-rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/tracetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/ttltarget.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-19 04:01:18.000000 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     2699 2023-06-19 04:01:18.000000 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2023-06-19 04:01:18.000000 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2023-06-19 04:01:18.000000 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/top_level.txt
+-rw-r--r--   0 panos     (1001) users      (100)       38 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/setup.cfg
+-rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-5.4.0/setup.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.4.0/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    61555 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/tests/iptables_test.py
```

### Comparing `linuxnet-iptables-5.3.0/.pylintrc` & `linuxnet-iptables-5.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/CHANGELOG.md` & `linuxnet-iptables-5.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Change Log
 ==========
 
+5.4.0 (2023-06-18)
+------------------
+
+- added AddressTypeMatch class to support the 'addrtype' match
+- added Chain.has_rules() method
+
 5.3.0 (2023-06-04)
 ------------------
 
 - added Chain.iter_rules() method
 - removed use of distutils from setup.py
 
 5.2.0 (2023-06-03)
```

### Comparing `linuxnet-iptables-5.3.0/LICENSE` & `linuxnet-iptables-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/Makefile` & `linuxnet-iptables-5.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/PKG-INFO` & `linuxnet-iptables-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 5.3.0
+Version: 5.4.0
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-iptables-5.3.0/README.md` & `linuxnet-iptables-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/Makefile` & `linuxnet-iptables-5.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/chain.rst` & `linuxnet-iptables-5.4.0/docs/chain.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/conf.py` & `linuxnet-iptables-5.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/exception.rst` & `linuxnet-iptables-5.4.0/docs/exception.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/extensibility.rst` & `linuxnet-iptables-5.4.0/docs/extensibility.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/index.rst` & `linuxnet-iptables-5.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/iptables_api.rst` & `linuxnet-iptables-5.4.0/docs/iptables_api.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/match-example.py` & `linuxnet-iptables-5.4.0/docs/match-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/match.rst` & `linuxnet-iptables-5.4.0/docs/match.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/commentmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/commentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/connmarkmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/connmarkmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/conntrackmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/conntrackmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/icmpmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/icmpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/limitmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/limitmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/markmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/markmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/ownermatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/ownermatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/packetmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/packetmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/packettypematch.rst` & `linuxnet-iptables-5.4.0/docs/matches/packettypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/statematch.rst` & `linuxnet-iptables-5.4.0/docs/matches/statematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/tcpmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/tcpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/tcpmssmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/tcpmssmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/ttlmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/ttlmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/matches/udpmatch.rst` & `linuxnet-iptables-5.4.0/docs/matches/udpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/rule.rst` & `linuxnet-iptables-5.4.0/docs/rule.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/table.rst` & `linuxnet-iptables-5.4.0/docs/table.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/target-example.py` & `linuxnet-iptables-5.4.0/docs/target-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/target.rst` & `linuxnet-iptables-5.4.0/docs/target.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/chaintarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/chaintarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/connmarktarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/connmarktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/dnattarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/dnattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/logtarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/logtarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/marktarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/marktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/masqueradetarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/masqueradetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/notracktarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/notracktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/rejecttarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/rejecttarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/snattarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/snattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/tracetarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/tracetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/docs/targets/ttltarget.rst` & `linuxnet-iptables-5.4.0/docs/targets/ttltarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/__init__.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/chain.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,19 @@
         return f'Chain({self.__real_chain_name})'
 
     def is_builtin(self) -> bool:       # pylint: disable=no-self-use
         """Returns ``True`` if this is a built-in chain (e.g. ``INPUT``)
         """
         return False
 
+    def has_rules(self) -> bool:
+        """Returns ``True`` if the chain contains any rules
+        """
+        return bool(self.__rule_list)
+
     def get_reference_count(self) -> int:
         """Returns the reference count of a (non-builtin) chain; returns 0
         for builtin chains
         """
         return self.__reference_count
 
     def get_packet_count(self) -> int:
```

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/deps.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/deps.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/exceptions.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/exceptions.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/extension.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/extension.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/__init__.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # <https://www.gnu.org/licenses/>.
 
 """
 Available match classes
 """
 
 from .match import Match, MatchNone, Criterion
+from .addrtypematch import AddressTypeMatch
 from .commentmatch import CommentMatch
 from .connmarkmatch import ConnmarkMatch
 from .conntrackmatch import ConntrackMatch
 from .icmpmatch import IcmpMatch
 from .limitmatch import LimitMatch
 from .markmatch import MarkMatch
 from .ownermatch import OwnerMatch
```

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/commentmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/commentmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/connmarkmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/connmarkmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/conntrackmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/conntrackmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/icmpmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/icmpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/limitmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/limitmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/markmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/markmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/match.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/match.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/ownermatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/ownermatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/packetmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/packetmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/packettypematch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/packettypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/statematch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/statematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/tcpmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/tcpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/tcpmssmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/tcpmssmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/ttlmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/ttlmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/udpmatch.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/udpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/util.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 This module provides helper classes for implementing Match/Criteria
 subclasses.
 """
 
 from typing import Any, List, Optional
 
 from ..deps import get_logger
+from ..exceptions import IptablesError
 
 from .match import Criterion, Match
 
 _logger = get_logger('linuxnet.iptables.matches.util')
 
 
 
@@ -37,14 +38,19 @@
     """
 
     def __init__(self, match: Match, iptables_option: str):
         super().__init__(match)
         self.__value = None
         self.__option = iptables_option
 
+    def get_iptables_option(self) -> str:
+        """Returns the **iptables(8)** option
+        """
+        return self.__option
+
     def get_value(self) -> Any:
         """Returns the criterion value
         """
         return self.__value
 
     def equals(self, value) -> Match:    # pylint: disable=arguments-differ
         """Compare with the specified value
@@ -58,22 +64,26 @@
         return [self.__option, str(self.__value)]
 
 
 class BooleanCriterion(Criterion):
     """Helper class for criteria that test single bits.
     """
 
-    def __init__(self, match: Match, iptables_option: str):
+    def __init__(self, match: Match, iptables_option: str,
+                                        supports_negation=True):
         """
         :param match: the :class:`Match` object that owns this ``Criterion``
         :param iptables_option: the **iptables(8)** option to use for this
             criterion
+        :param supports_negation: if ``True``, the criteria supports
+            the meth:not_equals method
         """
         super().__init__(match)
         self.__option = iptables_option
+        self.__supports_negation = supports_negation
 
     def get_value(self) -> bool:
         """Returns the criterion value
         """
         return self.is_positive()
 
     def bit_set(self) -> Match:
@@ -87,14 +97,22 @@
         return self.not_equals()
 
     def equals(self) -> Match:    # pylint: disable=arguments-differ
         """Compare with the setting of the bit
         """
         return self._set_polarity(True)
 
+    def not_equals(self) -> Match:      # pylint: disable=arguments-differ
+        """Express a test against the criterion being ``False``
+        """
+        if not self.__supports_negation:
+            raise IptablesError(
+                    f'{self.__option} does not support negation')
+        return super().not_equals()
+
     def _crit_iptables_args(self) -> List[str]:
         """Convert to **iptables(8)** arguments
         """
         return [self.__option]
 
 
 class Rate:             # pylint: disable=too-few-public-methods
```

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/metadata.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """
 Metadata information intended to be used by setup.py and the
 Sphinx conf.py
 """
 
 # pylint: disable=invalid-name
 
-_version_ = "5.3.0"
+_version_ = "5.4.0"
 _author_ = "Panagiotis (Panos) Tsirigotis"
 _package_ = "linuxnet.iptables"
```

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/parsing.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/parsing.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/rule.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/rule.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/table.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/table.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/__init__.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/connmarktarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/connmarktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/logtarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/logtarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/marktarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/marktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/masqueradetarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/masqueradetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/nattarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/nattarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/notracktarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/notracktarget.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     def __init__(self):
         """The :meth:`__init__` method expects no arguments.
         """
         super().__init__('NOTRACK', terminates=False)
 
     @classmethod
-    def parse(cls, field_iter) -> Target:
+    def parse(cls, _) -> Target:
         """Parse the NOTRACK target
 
         :meta private:
         """
         return NoTrackTarget()
```

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/rejecttarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/rejecttarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/target.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/target.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/tracetarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/tracetarget.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     def __init__(self):
         """The :meth:`__init__` method expects no arguments.
         """
         super().__init__('TRACE', terminates=False)
 
     @classmethod
-    def parse(cls, field_iter) -> Target:
+    def parse(cls, _) -> Target:
         """Parse the TRACE target
 
         :meta private:
         """
         return TraceTarget()
```

### Comparing `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/ttltarget.py` & `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/ttltarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/PKG-INFO` & `linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 5.3.0
+Version: 5.4.0
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/SOURCES.txt` & `linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docs/iptables_api.rst
 docs/match-example.py
 docs/match.rst
 docs/rule.rst
 docs/table.rst
 docs/target-example.py
 docs/target.rst
+docs/matches/addrtypematch.rst
 docs/matches/commentmatch.rst
 docs/matches/connmarkmatch.rst
 docs/matches/conntrackmatch.rst
 docs/matches/icmpmatch.rst
 docs/matches/limitmatch.rst
 docs/matches/markmatch.rst
 docs/matches/ownermatch.rst
@@ -50,14 +51,15 @@
 linuxnet/iptables/exceptions.py
 linuxnet/iptables/extension.py
 linuxnet/iptables/metadata.py
 linuxnet/iptables/parsing.py
 linuxnet/iptables/rule.py
 linuxnet/iptables/table.py
 linuxnet/iptables/matches/__init__.py
+linuxnet/iptables/matches/addrtypematch.py
 linuxnet/iptables/matches/commentmatch.py
 linuxnet/iptables/matches/connmarkmatch.py
 linuxnet/iptables/matches/conntrackmatch.py
 linuxnet/iptables/matches/icmpmatch.py
 linuxnet/iptables/matches/limitmatch.py
 linuxnet/iptables/matches/markmatch.py
 linuxnet/iptables/matches/match.py
```

### Comparing `linuxnet-iptables-5.3.0/setup.py` & `linuxnet-iptables-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.3.0/tests/iptables_test.py` & `linuxnet-iptables-5.4.0/tests/iptables_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -536,14 +536,78 @@
             elif rulenum == 3:
                 cit = iter(['another comment', 'foo bar'])
                 for match in rule.get_match_list():
                     if isinstance(match, CommentMatch):
                         comment = match.comment().get_value()
                         self.assertEqual(comment, next(cit))
 
+    def test_parsing_addrtype_match(self):
+        """Parse output with ADDRTYPE match
+        """
+        output = """\
+Chain INPUT (policy DROP 0 packets, 0 bytes)
+    pkts      bytes target     prot opt in     out     source               destination
+       0        0 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           ADDRTYPE match src-type UNICAST dst-type !UNICAST
+       0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           ADDRTYPE match src-type !BLACKHOLE dst-type !UNICAST limit-in LOG flags 0 level 4 prefix `ADDR '
+       0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           ADDRTYPE match src-type MULTICAST limit-out LOG flags 0 level 4 prefix `MCAST '
+       0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           ADDRTYPE match src-type PROHIBIT /* PROHIBIT */ LOG flags 0 level 4 prefix `PROH '
+""" + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
+        pft = IptablesPacketFilterTable('filter')
+        self.assertTrue(pft.init_from_output(output))
+        input_chain = pft.get_builtin_chain('INPUT')
+        rule_list = input_chain.get_rules()
+        #
+        # Check 1st rule
+        #
+        rule = rule_list[0]
+        match_list = rule.get_match_list()
+        self.assertEqual(len(match_list), 1)
+        match = match_list[0]
+        src_addr_type = match.src_addr_type()
+        self.assertTrue(src_addr_type.is_positive() and
+                        src_addr_type.get_value() == 'UNICAST')
+        dst_addr_type = match.dst_addr_type()
+        self.assertTrue(not dst_addr_type.is_positive() and
+                        dst_addr_type.get_value() == 'UNICAST')
+        #
+        # Check 2nd rule
+        #
+        rule = rule_list[1]
+        match_list = rule.get_match_list()
+        self.assertEqual(len(match_list), 1)
+        match = match_list[0]
+        src_addr_type = match.src_addr_type()
+        self.assertTrue(not src_addr_type.is_positive() and
+                        src_addr_type.get_value() == 'BLACKHOLE')
+        dst_addr_type = match.dst_addr_type()
+        self.assertTrue(not dst_addr_type.is_positive() and
+                        dst_addr_type.get_value() == 'UNICAST')
+        self.assertTrue(match.limit_iface_in().is_positive())
+        #
+        # Check 3rd rule
+        #
+        rule = rule_list[2]
+        match_list = rule.get_match_list()
+        self.assertEqual(len(match_list), 1)
+        match = match_list[0]
+        src_addr_type = match.src_addr_type()
+        self.assertTrue(src_addr_type.is_positive() and
+                        src_addr_type.get_value() == 'MULTICAST')
+        self.assertTrue(match.limit_iface_out().is_positive())
+        #
+        # Check 4th rule
+        #
+        rule = rule_list[3]
+        match_list = rule.get_match_list()
+        self.assertEqual(len(match_list), 2)
+        match = match_list[0]
+        src_addr_type = match.src_addr_type()
+        self.assertTrue(src_addr_type.is_positive() and
+                        src_addr_type.get_value() == 'PROHIBIT')
+
     def test_parsing_unknown_match(self):
         """Parse output with unknown match
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
 196245663 314408786102 prod_INPUT  all  --  *      *       0.0.0.0/0            0.0.0.0/0
```

