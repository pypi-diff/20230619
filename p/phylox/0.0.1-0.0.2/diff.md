# Comparing `tmp/phylox-0.0.1.tar.gz` & `tmp/phylox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylox-0.0.1.tar", last modified: Sun Jun 18 20:20:05 2023, max compression
+gzip compressed data, was "phylox-0.0.2.tar", last modified: Mon Jun 19 07:03:35 2023, max compression
```

## Comparing `phylox-0.0.1.tar` & `phylox-0.0.2.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.283912 phylox-0.0.1/
--rw-rw-r--   0 remie     (1000) remie     (1000)     1069 2023-06-06 08:24:00.000000 phylox-0.0.1/LICENSE
--rw-rw-r--   0 remie     (1000) remie     (1000)      835 2023-06-18 20:20:05.283912 phylox-0.0.1/PKG-INFO
--rw-rw-r--   0 remie     (1000) remie     (1000)      265 2023-06-06 08:27:33.000000 phylox-0.0.1/README.md
--rw-rw-r--   0 remie     (1000) remie     (1000)      778 2023-06-16 21:18:14.000000 phylox-0.0.1/pyproject.toml
--rw-rw-r--   0 remie     (1000) remie     (1000)       38 2023-06-18 20:20:05.283912 phylox-0.0.1/setup.cfg
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.267912 phylox-0.0.1/src/
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.267912 phylox-0.0.1/src/phylox/
--rw-rw-r--   0 remie     (1000) remie     (1000)       56 2023-06-16 20:17:29.000000 phylox-0.0.1/src/phylox/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      473 2023-06-18 16:22:17.000000 phylox-0.0.1/src/phylox/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.271912 phylox-0.0.1/src/phylox/cherrypicking/
--rw-r--r--   0 remie     (1000) remie     (1000)    63811 2021-02-16 08:57:15.000000 phylox-0.0.1/src/phylox/cherrypicking/CPH.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     9799 2021-02-04 13:17:13.000000 phylox-0.0.1/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     4934 2019-11-20 13:54:23.000000 phylox-0.0.1/src/phylox/cherrypicking/NetworkContainment.py
--rw-rw-r--   0 remie     (1000) remie     (1000)       19 2023-06-16 18:43:28.000000 phylox-0.0.1/src/phylox/cherrypicking/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     1889 2023-06-16 19:13:11.000000 phylox-0.0.1/src/phylox/cherrypicking/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.271912 phylox-0.0.1/src/phylox/classes/
--rw-rw-r--   0 remie     (1000) remie     (1000)      117 2023-06-16 18:23:58.000000 phylox-0.0.1/src/phylox/classes/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3334 2023-06-16 19:26:51.000000 phylox-0.0.1/src/phylox/classes/dinetwork.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      158 2023-06-16 18:20:46.000000 phylox-0.0.1/src/phylox/classes/networkclass.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3212 2023-06-18 17:29:23.000000 phylox-0.0.1/src/phylox/dinetwork.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.275912 phylox-0.0.1/src/phylox/exceptions/
--rw-rw-r--   0 remie     (1000) remie     (1000)      129 2023-06-16 17:26:34.000000 phylox-0.0.1/src/phylox/exceptions/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      185 2023-06-16 17:26:16.000000 phylox-0.0.1/src/phylox/exceptions/invalidmovedefinitionexception.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      178 2023-06-16 17:26:08.000000 phylox-0.0.1/src/phylox/exceptions/invalidmoveexception.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.275912 phylox-0.0.1/src/phylox/generators/
--rw-rw-r--   0 remie     (1000) remie     (1000)       49 2023-06-06 08:38:26.000000 phylox-0.0.1/src/phylox/generators/__init__.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.275912 phylox-0.0.1/src/phylox/generators/betasplitting/
--rw-rw-r--   0 remie     (1000) remie     (1000)     4577 2020-10-19 08:10:39.000000 phylox-0.0.1/src/phylox/generators/betasplitting/BetaSplittingModelTree.py
--rw-r--r--   0 remie     (1000) remie     (1000)     3159 2020-12-07 16:15:32.000000 phylox-0.0.1/src/phylox/generators/betasplitting/BetaSplittingNetwork_Main.py
--rw-r--r--   0 remie     (1000) remie     (1000)     6642 2021-02-25 14:03:40.000000 phylox-0.0.1/src/phylox/generators/betasplitting/BetaSplittingNetwork_Tools.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3281 2021-02-25 14:06:14.000000 phylox-0.0.1/src/phylox/generators/betasplitting/MakeCatAndBalancedWithEdges.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     3188 2021-05-14 07:21:48.000000 phylox-0.0.1/src/phylox/generators/betasplitting/MakeNetworksBeta.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.275912 phylox-0.0.1/src/phylox/generators/heath/
--rw-rw-r--   0 remie     (1000) remie     (1000)    31494 2023-06-06 09:34:55.000000 phylox-0.0.1/src/phylox/generators/heath/heath.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.275912 phylox-0.0.1/src/phylox/generators/lgt/
--rw-rw-r--   0 remie     (1000) remie     (1000)    13196 2023-06-06 09:39:31.000000 phylox-0.0.1/src/phylox/generators/lgt/Generator.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.275912 phylox-0.0.1/src/phylox/generators/mcmc/
--rw-rw-r--   0 remie     (1000) remie     (1000)       19 2023-06-18 20:18:48.000000 phylox-0.0.1/src/phylox/generators/mcmc/__init__.py
--rw-r--r--   0 remie     (1000) remie     (1000)     4395 2023-06-18 18:02:25.000000 phylox-0.0.1/src/phylox/generators/mcmc/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.275912 phylox-0.0.1/src/phylox/generators/randomTC/
--rw-rw-r--   0 remie     (1000) remie     (1000)    11032 2023-06-06 09:44:46.000000 phylox-0.0.1/src/phylox/generators/randomTC/RandomNetworks.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.275912 phylox-0.0.1/src/phylox/generators/zods/
--rw-rw-r--   0 remie     (1000) remie     (1000)     4482 2023-06-06 09:20:33.000000 phylox-0.0.1/src/phylox/generators/zods/zods.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.279912 phylox-0.0.1/src/phylox/isomorphism/
--rw-rw-r--   0 remie     (1000) remie     (1000)       52 2023-06-18 06:31:40.000000 phylox-0.0.1/src/phylox/isomorphism/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     4584 2023-06-18 06:40:52.000000 phylox-0.0.1/src/phylox/isomorphism/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.279912 phylox-0.0.1/src/phylox/networkproperties/
--rw-rw-r--   0 remie     (1000) remie     (1000)     3164 2023-06-06 09:30:01.000000 phylox-0.0.1/src/phylox/networkproperties/properties.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     7505 2023-06-17 08:24:27.000000 phylox-0.0.1/src/phylox/parser.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.279912 phylox-0.0.1/src/phylox/rearrangement/
--rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-06 08:38:49.000000 phylox-0.0.1/src/phylox/rearrangement/__init__.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.279912 phylox-0.0.1/src/phylox/rearrangement/exact_distance/
--rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-16 17:58:07.000000 phylox-0.0.1/src/phylox/rearrangement/exact_distance/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     5128 2023-06-16 17:59:17.000000 phylox-0.0.1/src/phylox/rearrangement/exact_distance/base.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.283912 phylox-0.0.1/src/phylox/rearrangement/heuristics/
--rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-16 17:57:13.000000 phylox-0.0.1/src/phylox/rearrangement/heuristics/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     7240 2020-11-06 11:55:16.000000 phylox-0.0.1/src/phylox/rearrangement/heuristics/cli_main.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    25763 2023-06-18 17:46:04.000000 phylox-0.0.1/src/phylox/rearrangement/heuristics/green_line_heuristic.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    11796 2023-06-16 17:59:14.000000 phylox-0.0.1/src/phylox/rearrangement/heuristics/heuristic_tools.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    26154 2023-06-18 17:46:04.000000 phylox-0.0.1/src/phylox/rearrangement/heuristics/red_line_heuristic.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     2365 2023-06-18 07:09:10.000000 phylox-0.0.1/src/phylox/rearrangement/invertsequence.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     5959 2023-06-18 17:51:07.000000 phylox-0.0.1/src/phylox/rearrangement/movability.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     8224 2023-06-18 17:42:36.000000 phylox-0.0.1/src/phylox/rearrangement/move.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      192 2023-06-18 07:04:48.000000 phylox-0.0.1/src/phylox/rearrangement/movetype.py
--rw-rw-r--   0 remie     (1000) remie     (1000)      669 2023-06-16 17:52:19.000000 phylox-0.0.1/src/phylox/rearrangement/rearrangementproblem.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.271912 phylox-0.0.1/src/phylox.egg-info/
--rw-rw-r--   0 remie     (1000) remie     (1000)      835 2023-06-18 20:20:05.000000 phylox-0.0.1/src/phylox.egg-info/PKG-INFO
--rw-rw-r--   0 remie     (1000) remie     (1000)     2018 2023-06-18 20:20:05.000000 phylox-0.0.1/src/phylox.egg-info/SOURCES.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)        1 2023-06-18 20:20:05.000000 phylox-0.0.1/src/phylox.egg-info/dependency_links.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)        7 2023-06-18 20:20:05.000000 phylox-0.0.1/src/phylox.egg-info/top_level.txt
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-18 20:20:05.283912 phylox-0.0.1/tests/
--rw-rw-r--   0 remie     (1000) remie     (1000)     3548 2023-06-16 17:01:13.000000 phylox-0.0.1/tests/test_dinetwork.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/
+-rw-rw-r--   0 remie     (1000) remie     (1000)     1069 2023-06-06 08:24:00.000000 phylox-0.0.2/LICENSE
+-rw-rw-r--   0 remie     (1000) remie     (1000)     1243 2023-06-19 07:03:35.717074 phylox-0.0.2/PKG-INFO
+-rw-rw-r--   0 remie     (1000) remie     (1000)      673 2023-06-19 07:03:23.000000 phylox-0.0.2/README.md
+-rw-rw-r--   0 remie     (1000) remie     (1000)      809 2023-06-19 06:53:37.000000 phylox-0.0.2/pyproject.toml
+-rw-rw-r--   0 remie     (1000) remie     (1000)       38 2023-06-19 07:03:35.717074 phylox-0.0.2/setup.cfg
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.709074 phylox-0.0.2/src/
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/
+-rw-rw-r--   0 remie     (1000) remie     (1000)       57 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)      469 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/base.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/cherrypicking/
+-rw-rw-r--   0 remie     (1000) remie     (1000)    65903 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/CPH.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)    10138 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     5145 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/NetworkContainment.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)       20 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     1903 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/cherrypicking/base.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/classes/
+-rw-rw-r--   0 remie     (1000) remie     (1000)      143 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/classes/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     3226 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/classes/dinetwork.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)      160 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/classes/networkclass.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     3245 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/dinetwork.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/exceptions/
+-rw-rw-r--   0 remie     (1000) remie     (1000)      130 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/exceptions/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)      187 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/exceptions/invalidmovedefinitionexception.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)      180 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/exceptions/invalidmoveexception.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/
+-rw-rw-r--   0 remie     (1000) remie     (1000)       49 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/generators/__init__.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/betasplitting/
+-rw-rw-r--   0 remie     (1000) remie     (1000)     4821 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingModelTree.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     3278 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingNetwork_Main.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     6926 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingNetwork_Tools.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     3416 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/MakeCatAndBalancedWithEdges.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     3300 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/betasplitting/MakeNetworksBeta.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/heath/
+-rw-rw-r--   0 remie     (1000) remie     (1000)    32262 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/heath/heath.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/lgt/
+-rw-rw-r--   0 remie     (1000) remie     (1000)    13796 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/lgt/Generator.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox/generators/mcmc/
+-rw-rw-r--   0 remie     (1000) remie     (1000)       20 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/mcmc/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     4562 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/mcmc/base.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/generators/randomTC/
+-rw-rw-r--   0 remie     (1000) remie     (1000)    11203 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/randomTC/RandomNetworks.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/generators/zods/
+-rw-rw-r--   0 remie     (1000) remie     (1000)     4739 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/generators/zods/zods.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/isomorphism/
+-rw-rw-r--   0 remie     (1000) remie     (1000)       53 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/isomorphism/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     4640 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/isomorphism/base.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/networkproperties/
+-rw-rw-r--   0 remie     (1000) remie     (1000)     3283 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/networkproperties/properties.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     7804 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/parser.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/rearrangement/
+-rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/rearrangement/__init__.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/rearrangement/exact_distance/
+-rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/rearrangement/exact_distance/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     5317 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/exact_distance/base.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/src/phylox/rearrangement/heuristics/
+-rw-rw-r--   0 remie     (1000) remie     (1000)        0 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     7496 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/cli_main.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)    26629 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/green_line_heuristic.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)    12283 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/heuristic_tools.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)    27078 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/heuristics/red_line_heuristic.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     2431 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/invertsequence.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     4777 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/movability.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     8793 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/move.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)      193 2023-06-19 06:53:37.000000 phylox-0.0.2/src/phylox/rearrangement/movetype.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)      669 2023-06-19 06:04:07.000000 phylox-0.0.2/src/phylox/rearrangement/rearrangementproblem.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.713074 phylox-0.0.2/src/phylox.egg-info/
+-rw-rw-r--   0 remie     (1000) remie     (1000)     1243 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/PKG-INFO
+-rw-rw-r--   0 remie     (1000) remie     (1000)     2051 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/SOURCES.txt
+-rw-rw-r--   0 remie     (1000) remie     (1000)        1 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/dependency_links.txt
+-rw-rw-r--   0 remie     (1000) remie     (1000)       28 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/requires.txt
+-rw-rw-r--   0 remie     (1000) remie     (1000)        7 2023-06-19 07:03:35.000000 phylox-0.0.2/src/phylox.egg-info/top_level.txt
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-19 07:03:35.717074 phylox-0.0.2/tests/
+-rw-rw-r--   0 remie     (1000) remie     (1000)     3530 2023-06-19 06:53:37.000000 phylox-0.0.2/tests/test_dinetwork.py
```

### Comparing `phylox-0.0.1/LICENSE` & `phylox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phylox-0.0.1/pyproject.toml` & `phylox-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
 requires = [
     "setuptools>=61.0",
-    "networkx>=3.1",    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phylox"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Remie Janssen", email="remiejanssen92@gmail.com" },
 ]
 description = "A package with tools for constructing, manipulating, and analyzing phylogenetic networks."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "networkx>=2.6",
+  "numpy>=1.21.6"
+]
 
 [tool.pytest.ini_options]
 pythonpath = [
   ".", "src",
 ]
 addopts = "--cov --cov-report term-missing"
```

### Comparing `phylox-0.0.1/src/phylox/cherrypicking/CPH.py` & `phylox-0.0.2/src/phylox/cherrypicking/CPH.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1381 +1,1349 @@
-import networkx as nx
-import random
-import matplotlib.pyplot as plt
-import os
-import ast
-import re
-import sys
-import time
-from copy import deepcopy
-memodict={}
-import numpy as np
-
-
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########                             Index                         #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-'''
-AAA I/O Functions
-	Functions for reading newick sequences
-AAB ANALYSIS OF SEQUENCE FOR TREES
-	Two functions:
-          - Checking whether a CPS reduces a set of trees
-          - Sequence_Add_Roots (i.e. CompletePartialSequence from the paper) to extend a partial CPS to a CPS
-AAC INPUT SET CLASS with CPS methods
-	Class containing a set of inputs
-        Methods for running the CP heuristic and improving the sequence
-AAD PHYLOGENETIC TREE CLASS
-	Class for a phylogenetic tree
-	Contains methods to cherry-pick a tree and to find reducible pairs
-	Gives the height of a pair in the tree
-AAE CutTree CLASS
-	Class meant for converting a network into a Newick string
-        It `cuts' the reticulation arcs to produce a tree that can be converted to Newick
-AAF PHYLOGENETIC NETWORK CLASS
-        Class for a phylogenetic network
-        Contains methods 
-		to add pairs to the network from a sequence
-		to compute scores of edges (inheritance and number of embedded trees)
-                to reduce pairs (not used if input consists of only trees)
-
-'''
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########                     AAA I/O Functions                     #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-########
-######## Convert Newick to a networkx Digraph with labels (and branch lengths)
-########
-#Write length newick: convert ":" to "," and then evaluate as list of lists using ast.literal_eval
-# Then, in each list, the node is followed by the length of the incoming arc.
-# This only works as long as each branch has length and all internal nodes are labeled.
-def Newick_To_Tree(newick, current_labels = dict()):
-    newick=newick[:-1]
-    distances = False
-    #presence of : indicates the use of lengths in the trees
-    if ":" in newick:
-        distances = True
-        #taxon names may already be enclosed by " or ', otherwise, we add these now
-        if not "'" in newick and not '"' in newick:
-            newick = re.sub(r"([,\(])([a-zA-Z\d]+)", r"\1'\2", newick)
-            newick = re.sub(r"([a-zA-Z\d]):", r"\1':", newick)
-        newick = newick.replace(":",",")
-    else:
-        #taxon names may already be enclosed by " or ', otherwise, we add these now
-        if not "'" in newick and not '"' in newick:
-            newick = re.sub(r"([,\(])([a-zA-Z\d]+)", r"\1'\2", newick)
-            newick = re.sub(r"([a-zA-Z\d])([,\(\)])", r"\1'\2", newick)
-    #turn the string into a pyhton nested list using [ instead of (
-    newick = newick.replace("(","[")
-    newick = newick.replace(")","]")
-    nestedtree = ast.literal_eval(newick)
-    #parse the nested list into a list of edges with some additional information about the leaves
-    #we start with the root 2, so that we can append a root edge (1,2)
-    edges, leaves, current_labels, current_node = NestedList_To_Tree(nestedtree,2,current_labels, distances = distances)
-    #put all this information into a networkx DiGraph with or without distances/lengths
-    tree = nx.DiGraph()
-    if distances:
-        edges.append((1,2,0))
-        tree.add_weighted_edges_from(edges,weight='length')        
-    else:
-        edges.append((1,2))
-        tree.add_edges_from(edges)
-    return tree, leaves, current_labels, distances
-    
-#Auxiliary function to convert list of lists to tree (graph)
-#Works recursively, where we keep track of the nodes we have already used
-#Leaves are nodes with negative integer as ID, and already existing taxa are coupled to node IDs by current_labels.
-def NestedList_To_Tree(nestedList, next_node, current_labels, distances = False):
-    edges = []
-    leaves = set()
-    top_node = next_node
-    current_node = next_node+1
-    if distances:
-        #each element in the sublist has 2 properties, the subtree, and the length, which are adjacent in nestedList
-        for i in range(0,len(nestedList),2):
-            t = nestedList[i]
-            length = nestedList[i+1]
-            if type(t)==list: #Not a leaf 
-                edges.append((top_node,current_node,length))
-                extra_edges, extra_leaves, current_labels, current_node = NestedList_To_Tree(t,current_node,current_labels,distances=distances)
-            else: #A leaf
-                if str(t) not in current_labels:
-                    current_labels[str(t)] = -len(current_labels) 
-                edges.append((top_node,current_labels[str(t)],length))
-                extra_edges = []
-                extra_leaves = set([current_labels[str(t)]])
-            edges = edges + extra_edges
-            leaves = leaves.union(extra_leaves)
-    else:
-        #no lengths/distances, so each subtree is simply an element of nestedList
-        for t in nestedList:
-            if type(t)==list: 
-                edges.append((top_node,current_node))
-                extra_edges, extra_leaves, current_labels, current_node = NestedList_To_Tree(t,current_node,current_labels)
-            else: 
-                if str(t) not in current_labels:
-                    current_labels[str(t)] = -len(current_labels) 
-                edges.append((top_node,current_labels[str(t)]))
-                extra_edges = []
-                extra_leaves = set([current_labels[str(t)]])
-            edges = edges + extra_edges
-            leaves = leaves.union(extra_leaves)
-    return edges, leaves, current_labels, current_node
-
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########          AAB ANALYSIS OF SEQUENCE FOR TREES               #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-
- 
-      
-
-#Checks whether a given cherry-picking sequence `seq' reduces a given tree `tree'
-#if not,    returns false
-#otherwise, returns the indices of the pairs that actually reduce a cherry in the tree 
-def Sequence_Reduces_Tree(seq,tree):
-    t_copy=deepcopy(tree)
-    indices = []
-    for i, pair in enumerate(seq):
-        if t_copy.reduce_pair(*pair):
-            indices +=[i] 
-            if len(t_copy.nw.edges)==1:
-                return indices
-    return False
-
-
-#Modifies a cherry-picking sequence so that it represents a network with exactly one root.
-#A sequence may be such that reconstructing a network from the sequence results in multiple roots
-#This function adds some pairs to the sequence so that the network has a single root.
-#returns the new sequence, and also modifies the sets of trees reduced by each pair in the sequence, so that the new pairs are also represented (they reduce no trees)
-def Sequence_add_roots(seq, red_trees):
-    leaves_encountered = set()
-    roots = set()
-    #The roots can be found by going back through the sequence and finding pairs where the second element has not been encountered in the sequence yet
-    for pair in reversed(seq):
-        if pair[1] not in leaves_encountered:
-            roots.add(pair[1])
-        leaves_encountered.add(pair[0])
-        leaves_encountered.add(pair[1])
-    i=0
-    roots = list(roots)
-    #Now add some pairs to make sure each second element is already part of some pair in the sequence read backwards, except for the last pair in the sequence
-    for i in range(len(roots)-1):
-       seq.append((roots[i],roots[i+1]))
-       #none of the trees are reduced by the new pairs.
-       red_trees.append(set())
-       i+=1
-    return seq, red_trees
-
-
-
-
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########         AAC INPUT SET CLASS with CPS methods              #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-
-#Methods for sets of phylogenetic trees
-class Input_Set:
-    def __init__(self, newick_strings = []):
-        #The dictionary of trees
-        self.trees = dict()
-        #the set of leaf labels of the trees
-        self.labels = dict()
-        self.labels_reversed = dict()
-        self.leaves = set()
-        
-        #the current best sequence we have found for this set of trees
-        self.best_seq = None
-        #the list of reduced trees for each of the pairs in the best sequence
-        self.best_red_trees = None
-        
-        #the best sequence for the algorithm using lengths as input as well
-        self.best_seq_with_lengths = None
-        #the sets of reduced trees for each pair in this sequence
-        self.best_seq_with_lengths_red_trees = None
-        #the height of each pair in this sequence
-        self.best_seq_with_lengths_heights = None
-        
-        #true if distances are used
-        self.distances = True
-        #computation times
-        self.CPS_Compute_Time = 0
-        self.CPS_Compute_Reps = 0
-        
-        #read the input trees in 'newick_strings'
-        for n in newick_strings:
-            tree = PhT()
-            self.trees[len(self.trees)] = tree
-            self.labels, distances_in_tree = tree.Tree_From_Newick(newick = n, current_labels = self.labels)
-            self.distances = self.distances and distances_in_tree
-        self.leaves = list(self.labels)
-        
-        #make a reverse dictionary for the leaf labels, to look up the label of a given node
-        for l,i in self.labels.items():
-            self.labels_reversed[i] = l
-
-    #Make a deepcopy of an instance
-    def __deepcopy__(self, memodict={}):
-        copy_inputs = Input_Set()
-        copy_inputs.trees = deepcopy(self.trees,memodict)
-        copy_inputs.labels = deepcopy(self.labels,memodict)
-        copy_inputs.labels_reversed = deepcopy(self.labels_reversed,memodict)
-        copy_inputs.leaves = deepcopy(self.leaves,memodict)
-#        copy_inputs.best_seq = deepcopy(self.best_seq)
-#        copy_inputs.best_red_trees = deepcopy(self.best_red_trees)
-        return copy_inputs
-
-    #Find new cherry-picking sequences for the trees and update the best found
-    def CPSBound(self, repeats = 1, progress = False, track = False, lengths = False, time_limit = None):
-        #Set the specific heuristic that we use, based on the user input and whether the trees have lengths
-        Heuristic = self.CPHeuristic
-        if track and not lengths:
-            print("Tracking reducible cherries")
-            Heuristic = self.CPHeuristicStorePairs
-        if lengths:
-            if not self.distances:
-                print("not all trees have branch lengths!")
-                sys.exit()
-                return []
-            print("Picking the lowest cherry")
-            Heuristic = self.CPHeuristicLengths
-            heights_best = []
-        #Initialize the recorded best sequences and corresponding data
-        best = None
-        red_trees_best = []
-        starting_time = time.time()
-        #Try as many times as required by the integer 'repeats'
-        for i in range(repeats):
-            print(i+1)
-            if lengths:
-                new, reduced_trees, seq_heights = Heuristic(progress=progress)  
-                print("found sequence of length: "+str(len(new)))
-            else:
-                new, reduced_trees = Heuristic(progress=progress)
-                print("found sequence of length: "+str(len(new)))
-                print("improving sequence")
-                new, reduced_trees = self.Improve_Sequence(new, reduced_trees, progress = progress)
-                print("new length = "+str(len(new)))
-            print("adding roots")
-            new,reduced_trees = Sequence_add_roots(new,reduced_trees)
-            if lengths:
-                for i in range(len(new)-len(seq_heights)):
-                    seq_heights+=[seq_heights[-1]]
-            print("final length = "+str(len(new)))
-            if best == None or len(new) < len(best):
-                best = new
-                red_trees_best = reduced_trees
-                if lengths:
-                    heights_best = seq_heights
-            print("best sequence has length "+str(len(best)))
-            self.CPS_Compute_Reps+=1
-            if time_limit and time.time()-starting_time > time_limit:
-                break
-        self.CPS_Compute_Time += time.time() - starting_time
-        new_seq = best
-        if lengths:
-            if not self.best_seq_with_lengths or len(new_seq)<len(self.best_seq_with_lengths):
-                converted_new_seq = []
-                for pair in new_seq:
-                    converted_new_seq += [(self.labels_reversed[pair[0]],self.labels_reversed[pair[1]])]
-                self.best_seq_with_lengths = converted_new_seq
-                self.best_seq_with_lengths_red_trees = red_trees_best
-                self.best_seq_with_lengths_heights = heights_best
-            return self.best_seq_with_lengths
-        else:
-            if not self.best_seq or len(new_seq)<len(self.best_seq):
-                converted_new_seq = []
-                for pair in new_seq:
-                    converted_new_seq += [(self.labels_reversed[pair[0]],self.labels_reversed[pair[1]])]
-                self.best_seq = converted_new_seq
-                self.best_red_trees = red_trees_best
-            return self.best_seq
-
-
-
-
-
-    #Version of the code that uses minimal memory: recompute reducible pairs when necessary.
-    def CPHeuristic(self, progress=False):
-        if progress:
-            print("Copying all inputs to reduce on")
-        #Works in a copy of the input trees, copy_of_inputs, because trees have to be reduced somewhere.         
-        copy_of_inputs = deepcopy(self)
-        if progress:
-            print("Done, starting reduction of trees")
-        CPS = []
-        reduced_trees = []
-        candidate_leaves = deepcopy(self.leaves)
-        while copy_of_inputs.trees:
-            if progress:
-                print("Sequence has length: "+str(len(CPS)))
-                print(str(len(copy_of_inputs.trees))+" trees left.\n")
-                print("Reducing trivial pairs")
-                 #First reduce trivial cherries
-            new_seq, new_red_trees = copy_of_inputs.Reduce_Trivial_Pairs(candidate_leaves)
-            if progress:
-                print("done")
-            CPS           += new_seq
-            reduced_trees += new_red_trees
-            if len(copy_of_inputs.trees)==0:
-                break
-             #Now reduce a random cherry from a random tree
-            random_index, random_tree = random.choice(list(copy_of_inputs.trees.items()))
-            list_of_cherries = random_tree.Find_All_Reducible_Pairs()
-            random_cherry = random.choice(list(list_of_cherries))
-            CPS         += [random_cherry]
-            reduced_by_random_cherry = copy_of_inputs.Reduce_Pair_In_All(random_cherry)
-            reduced_trees += [reduced_by_random_cherry]
-            candidate_leaves = set(random_cherry)
-        return CPS, reduced_trees
-
-    #Version of the code that uses more memory: stores all reducible pairs.
-    #Runs when user toggles -t or --track
-    def CPHeuristicStorePairs(self, progress=False):
-        if progress:
-            print("Copying all inputs to reduce on")
-        #Works in a copy of the input trees, copy_of_inputs, because trees have to be reduced somewhere. 
-        copy_of_inputs = deepcopy(self)
-        if progress:
-            print("Done")
-        CPS = []
-        reduced_trees = []
-        candidate_leaves = deepcopy(self.leaves)
-        # Make dict of reducible pairs
-        if progress:
-            print("finding all reducible pairs")
-        reducible_pairs = self.Find_All_Pairs()
-        if progress:
-            print("found all reducible pairs")
-        while copy_of_inputs.trees:
-            if progress:
-                print("Sequence has length: "+str(len(CPS)))
-                print(str(len(copy_of_inputs.trees))+" trees left.\n")
-                print("Reducing trivial pairs")
-              #First reduce trivial cherries
-            new_seq, new_red_trees, reducible_pairs = copy_of_inputs.Reduce_Trivial_Pairs_Store_Pairs(candidate_leaves, reducible_pairs)
-            if progress:
-                print("done")
-            CPS           += new_seq
-            reduced_trees += new_red_trees
-            if len(copy_of_inputs.trees)==0:
-                break
-
-               #Now reduce a random cherry from a random tree
-              #EITHER: (Get random tree, then random pair from the tree), just like in CPHeuristic
-            random_index, random_tree = random.choice(list(copy_of_inputs.trees.items()))
-            list_of_cherries = random_tree.Find_All_Reducible_Pairs()
-            random_cherry = random.choice(list(list_of_cherries))
-
-              #OR: (Get a random reducible pair from all pairs)  
-              #Note that this would result in a different algorithm than CPHeuristic, so we use the previous option
-#            random_cherry = random.choice(list(reducible_pairs.keys()))
-
-
-            CPS         += [random_cherry]
-            #reduce all trees with this pair, this is where the list of reducible_pairs is used
-            #using the list makes it faster to find all trees that need to be reduced.
-            reduced_by_random_cherry = copy_of_inputs.Reduce_Pair_In_All(random_cherry, reducible_pairs = reducible_pairs)
-            reducible_pairs = copy_of_inputs.Update_Reducible_Pairs(reducible_pairs, reduced_by_random_cherry)
-            reduced_trees += [reduced_by_random_cherry]
-            candidate_leaves = set(random_cherry)
-        return CPS, reduced_trees
-
-
-    #Version of the code that always picks the lowest available pair
-    #Runs when user toggles -l or --lengths and all edges in the input trees have lengths.
-    def CPHeuristicLengths(self, progress=False):
-        if progress:
-            print("Copying all inputs to reduce on")
-        #Works in a copy of the input trees, copy_of_inputs, because trees have to be reduced somewhere. 
-        copy_of_inputs = deepcopy(self)
-        if progress:
-            print("Done")
-        CPS = []
-        reduced_trees = []
-        heights_seq = []
-        
-        candidate_leaves = deepcopy(self.leaves)
-        # Make dict of reducible pairs
-        if progress:
-            print("finding all reducible pairs")
-        reducible_pairs = self.Find_All_Pairs()
-        current_heights = dict()    #for each reducible pair: [0] gives height, [1] the number of trees it was computed in.      
-
-        if progress:
-            print("found all reducible pairs")
-        while copy_of_inputs.trees:
-            if progress:
-                print("Sequence has length: "+str(len(CPS)))
-                print(str(len(copy_of_inputs.trees))+" trees left.\n")
-              #First reduce trivial cherries
-                print("Reducing trivial pairs")
-            new_seq, new_red_trees, reducible_pairs, new_heights_seq = copy_of_inputs.Reduce_Trivial_Pairs_Lengths(candidate_leaves, reducible_pairs)
-            if progress:
-                print("done")
-            CPS           += new_seq
-            reduced_trees += new_red_trees
-            heights_seq   += new_heights_seq
-            if len(copy_of_inputs.trees)==0:
-                break
-
-               #Now find the lowest cherry.
-            current_heights = copy_of_inputs.Update_Heights(current_heights, reducible_pairs)
-            lowest_cherry        = None
-            lowest_height        = None
-            lowest_height_tuple  = None
-            lowest_heights_found = 1
-            for pair in reducible_pairs:
-                height_pair_tuple = current_heights[pair][0]
-                height_pair       = float(height_pair_tuple[0]+height_pair_tuple[1])/2
-                new_found = False
-                if (not lowest_height) or lowest_height>height_pair:
-                    new_found = True
-                    lowest_heights_found=1
-                elif lowest_height==height_pair:
-                    lowest_heights_found+=1
-                    if random.random()<1/float(lowest_heights_found):
-                        new_found = True
-                if new_found:
-                    lowest_cherry       = pair
-                    lowest_height       = height_pair
-                    lowest_height_tuple = height_pair_tuple
-                        
-                    
-            CPS         += [lowest_cherry]
-            heights_seq += [lowest_height_tuple]
-            reduced_by_lowest_cherry = copy_of_inputs.Reduce_Pair_In_All(lowest_cherry, reducible_pairs = reducible_pairs)
-            reducible_pairs = copy_of_inputs.Update_Reducible_Pairs(reducible_pairs, reduced_by_lowest_cherry)
-            reduced_trees += [reduced_by_lowest_cherry]
-            candidate_leaves = set(lowest_cherry)
-        return CPS, reduced_trees, heights_seq
-
-
-    #Returns an updated distcionary of heights of the reducible pairs
-    def Update_Heights(self,current_heights,reducible_pairs):
-        for pair, trees in reducible_pairs.items():
-            #updating is only necessary when the set of trees for that pair is changed or the reducible pair was not reducible before.
-            if not pair in current_heights or not current_heights[pair][1]==len(trees):
-                height_pair = self.Height_Pair(pair,trees)
-                current_heights[pair] = (height_pair, len(trees))
-        return current_heights
-
-
-    #Returns the average height of a pair in a set of trees
-    # The pair must be reducible in each tree in 'trees'
-    def Height_Pair(self, pair, trees):
-        height_pair = [0,0]
-        for t in trees:
-            height_in_t = self.trees[t].Height_Of_Cherry(*pair)
-            height_pair[0]+=height_in_t[0]
-            height_pair[1]+=height_in_t[1]
-        return [height_pair[0]/float(len(trees)),height_pair[1]/float(len(trees))]
-
-
-    #Finds the set of reducible pairs in all trees
-    #Returns a dictionary with reducible pairs as keys, and the trees they reduce as values.
-    def Find_All_Pairs(self):
-        reducible_pairs = dict()
-        for i,t in self.trees.items():
-            red_pairs_t = t.Find_All_Reducible_Pairs()
-            for pair in red_pairs_t:
-                if pair in reducible_pairs:
-                    reducible_pairs[pair].add(i)
-                else:
-                    reducible_pairs[pair] = set([i])
-        return reducible_pairs
-
-
-
-    #UReturns the updated dictionary of reducible pairs in all trees after a reduction (with the trees they reduce as values)
-    #we only need to update for the trees that got reduced: 'new_red_treed'
-    def Update_Reducible_Pairs(self, reducible_pairs, new_red_trees):
-        #Remove trees to update from all pairs
-        for pair,trees in reducible_pairs.items():
-            trees.difference_update(new_red_trees)
-            if len(trees)==0:
-                del reducible_pairs[pair]
-        #Add the trees to the right pairs again
-        for index in new_red_trees:
-            if index in self.trees:
-                t = self.trees[index]
-                red_pairs_t = t.Find_All_Reducible_Pairs()
-                for pair in red_pairs_t:
-                    if pair in reducible_pairs:
-                        reducible_pairs[pair].add(index)
-                    else:
-                        reducible_pairs[pair] = set([index])
-        return reducible_pairs
-
-    #reduces the given pair in all trees
-    #Returns the set of trees thet were reduced
-    #CHANGES THE SET OF TREES, ONLY PERFORM IN A COPY OF THE CLASS INSTANCE
-    def Reduce_Pair_In_All(self, pair, reducible_pairs = dict()):
-        reduced_trees_for_pair=[]
-        if pair in reducible_pairs:
-            trees_to_reduce = reducible_pairs[pair]
-        else:
-            if reducible_pairs:
-                print("pair not found, trying all trees")
-            trees_to_reduce = deepcopy(self.trees)
-        for i in trees_to_reduce:
-            if i in self.trees:
-                t = self.trees[i]
-                if t.reduce_pair(*pair):
-                    reduced_trees_for_pair+=[i]
-                    if len(t.nw.edges())<=1:
-                        del self.trees[i]   
-        return set(reduced_trees_for_pair)
-
-
-    #reduces the trivial pairs in the current set of trees
-    #runs efficiently by giving a set of leaves 'candidate_leaves' that may be involved in trivial pairs
-    #this set must be given; after a reduction of the pair (a,b) only using the leaves a and b works
-    #Returns the reduced pairs and the sets of trees thet were reduced
-    #CHANGES THE SET OF TREES, ONLY PERFORM IN A COPY OF THE CLASS INSTANCE
-    def Reduce_Trivial_Pairs(self,candidate_leaves):
-        seq = []
-        reduced_tree_sets = []
-        while candidate_leaves:
-            l = candidate_leaves.pop()
-            new_pairs = list(self.Trivial_Pair_With(l))
-            if new_pairs:
-                seq += new_pairs
-                for p in new_pairs:
-                    red_trees_p = self.Reduce_Pair_In_All(p) 
-                    reduced_tree_sets += [red_trees_p]
-                    candidate_leaves   = candidate_leaves | set(p)
-        return seq, reduced_tree_sets
-
-    #reduces the trivial pairs in the current set of trees
-    #runs efficiently by giving a set of leaves 'candidate_leaves' that may be involved in trivial pairs
-    #this set must be given; after a reduction of the pair (a,b) only using the leaves a and b works
-    #Returns the reduced pairs and the sets of trees thet were reduced, also updates the reducible pairs.
-    #CHANGES THE SET OF TREES, ONLY PERFORM IN A COPY OF THE CLASS INSTANCE
-    def Reduce_Trivial_Pairs_Store_Pairs(self,candidate_leaves, reducible_pairs):
-        seq = []
-        reduced_tree_sets = []
-        while candidate_leaves:
-            l = candidate_leaves.pop()
-            new_pairs = list(self.Trivial_Pair_With(l))
-            if new_pairs:
-#                print("found a trivial pair")
-                seq += new_pairs
-                for p in new_pairs:
-                    red_trees_p = self.Reduce_Pair_In_All(p, reducible_pairs = reducible_pairs)
-                    reducible_pairs = self.Update_Reducible_Pairs(reducible_pairs, red_trees_p)
-                    reduced_tree_sets += [red_trees_p]
-                    candidate_leaves   = candidate_leaves | set(p)
-        return seq, reduced_tree_sets, reducible_pairs
-
-    #reduces the trivial pairs in the current set of trees with branch lengths
-    #runs efficiently by giving a set of leaves 'candidate_leaves' that may be involved in trivial pairs
-    #this set must be given; after a reduction of the pair (a,b) only using the leaves a and b works
-    #Returns the reduced pairs and the sets of trees thet were reduced, also updates the reducible pairs and their heights.
-    #CHANGES THE SET OF TREES, ONLY PERFORM IN A COPY OF THE CLASS INSTANCE
-    def Reduce_Trivial_Pairs_Lengths(self,candidate_leaves, reducible_pairs):
-        seq = []
-        reduced_tree_sets = []
-        heights_seq = []
-        while candidate_leaves:
-            l = candidate_leaves.pop()
-            new_pairs = list(self.Trivial_Pair_With(l))
-            if new_pairs:
-#                print("found a trivial pair")
-                seq += new_pairs
-                for p in new_pairs:
-                    height_p = self.Height_Pair(p,reducible_pairs[p])
-                    red_trees_p = self.Reduce_Pair_In_All(p, reducible_pairs = reducible_pairs)
-                    heights_seq += [height_p]
-                    reducible_pairs = self.Update_Reducible_Pairs(reducible_pairs, red_trees_p)
-                    reduced_tree_sets += [red_trees_p]
-                    candidate_leaves   = candidate_leaves | set(p)
-        return seq, reduced_tree_sets, reducible_pairs, heights_seq
-
-    #Returns all trivial pairs involving the leaf l
-    def Trivial_Pair_With(self,l):
-        pairs = set()
-        #Go through all trees t with index i.
-        for i,t in self.trees.items():
-            #If the leaf occurs in t
-            if l in t.leaves:
-                #Compute reducible pairs of t with the leaf as first coordinate
-                pairs_in_t = t.Find_Pairs_With_First(l)
-                #If we did not have a set of candidate pairs yet, use pairs_in_t
-                if not pairs:
-                    pairs = pairs_in_t
-                #Else, the candidate pairs must also be in t, so take intersection
-                else:
-                    pairs = pairs & pairs_in_t
-                #If we do not have any candidate pairs after checking a tree with l as leaf, we stop.
-                if not pairs:
-                    break
-        return pairs
-
-
-    #Improves a sequence 'CPS' for the input trees by removing elements and checking whether the new sequence still reduces all trees
-    #Returns this improved sequence and the corresponding sets of reduced trees for each pair.
-    def Improve_Sequence(self, CPS, reduced_trees, progress = False):
-        seq = deepcopy(CPS)
-        i=0
-        while i<len(seq):
-            redundant = True
-            relevant_tree_indices = reduced_trees[i]
-            new_relevant_pairs_for_trees = dict()
-            for j in relevant_tree_indices:
-                #Check if the shorter sequence reduces the trees, and if so, record which pairs reduced a cherry in which tree
-                new_relevant_pairs_for_trees[j] = Sequence_Reduces_Tree(seq[:i]+seq[i+1:],self.trees[j])
-                if not new_relevant_pairs_for_trees[j]:
-                    redundant = False
-                    break
-            if redundant:
-                #Remove the ith element from seq and reduced trees
-                seq.pop(i)
-                reduced_trees.pop(i)
-                #Update reduced_trees for the relevant trees
-                   #First remove all j in relevant_tree_indices 
-                for tree_index_set in reduced_trees:                
-                    for j in relevant_tree_indices:
-                        tree_index_set.discard(j)
-                   #Now add them back at the right places, according to "new_relevant_pairs_for_trees"
-                for j in relevant_tree_indices:
-                    for index in new_relevant_pairs_for_trees[j]:
-                        reduced_trees[index].add(j)                  
-                if progress:
-                    print("New length is "+str(len(seq)))
-                    print("Continue at position "+str(i))
-            else:
-                i+=1
-        return seq, reduced_trees 
-
-
-
-        
-
-
-
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########              AAD PHYLOGENETIC TREE CLASS                  #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-
-#A class representing a phylogenetic tree
-#Contains methods to reduce trees
-class PhT:
-    def __init__(self):
-        #the actual graph
-        self.nw = nx.DiGraph()
-        #the set of leaf labels of the network
-        self.leaves = set()
-    
-    #Builds a tree from a newick string
-    def Tree_From_Newick(self, newick = None, current_labels = dict()):
-        self.nw, self.leaves, current_labels, distances = Newick_To_Tree(newick, current_labels)
-        return current_labels, distances
-        
-    #Checks whether the pair (x,y) forms a cherry in the tree
-    def Is_Cherry(self,x,y):
-        if (not x in self.leaves) or (not y in self.leaves):
-            return False
-        px=-1
-        py=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        for p in self.nw.predecessors(y):
-            py=p
-        return px==py
-   
-    #Returns the height of (x,y) if it is a cherry:
-    #     i.e.: length(p,x)+length(p,y)/2
-    #Returns false otherwise
-    def Height_Of_Cherry(self,x,y):
-        if (not x in self.leaves) or (not y in self.leaves):
-            return False
-        px=-1
-        py=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        for p in self.nw.predecessors(y):
-            py=p
-        if px==py:
-            height = [float(self.nw[px][x]['length']),float(self.nw[py][y]['length'])]
-            return height
-        return False 
-        
-
-    #suppresses a degree-2 node v and returns true if successful
-    # the new arc has length length(p,v)+length(v,c)
-    #returns false if v is not a degree-2 node
-    def Clean_Node(self,v):
-        if self.nw.out_degree(v)==1 and self.nw.in_degree(v)==1:
-            pv=-1
-            for p in self.nw.predecessors(v):
-                pv=p
-            cv=-1
-            for c in self.nw.successors(v):
-                cv=c
-            self.nw.add_edges_from([(pv,cv,self.nw[pv][v])])
-            if 'length' in self.nw[pv][v] and 'length' in self.nw[v][cv]:
-                self.nw[pv][cv]['length']=self.nw[pv][v]['length']+self.nw[v][cv]['length']
-            self.nw.remove_node(v)
-            return True
-        return False
- 
-    #reduces the pair (x,y) in the tree if it is present as cherry
-    # i.e., removes the leaf x and its incoming arc, and then cleans up its parent node.
-    # note that if px, and py have different lengths, the length of px is lost in the new network.
-    #returns true if successful and false otherwise
-    def reduce_pair(self,x,y):
-        if not x in self.leaves or not y in self.leaves:
-            return False
-        px=-1
-        py=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        for p in self.nw.predecessors(y):
-            py=p 
-        if self.Is_Cherry(x,y):
-            self.nw.remove_node(x)
-            self.leaves.remove(x)
-            self.Clean_Node(py)
-            return True
-        return False
-
-
-    #Returns all reducible pairs in the tree involving x, where x is the first element
-    def Find_Pairs_With_First(self,x):
-        pairs = set()
-        px=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        if self.nw.out_degree(px)>1:
-            for cpx in self.nw.successors(px):
-                if cpx in self.leaves:
-                    pairs.add((x,cpx))
-        return pairs-set([(x,x)])
-
-    #Returns all reducible pairs in the tree
-    def Find_All_Reducible_Pairs(self):
-        red_pairs=set()
-        for l in self.leaves:
-            red_pairs=red_pairs.union(self.Find_Pairs_With_First(l))
-        return red_pairs
-        
-        
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########                     AAE CutTree CLASS                     #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-#A class that represents a network as a tree where hybrid edges have been cut at the hybrid nodes.
-#Used as an intermediate to find the Newick string of a network.
-class CutTree:
-    def __init__(self, network = None, current_node = None, leaf_labels= dict()):
-         self.hybrid_nodes = dict()
-         self.no_of_hybrids = 0
-         self.root = None
-         self.nw = deepcopy(network)
-         self.current_node = current_node
-         self.leaf_labels = leaf_labels
-         if not self.current_node:
-             self.current_node = 2*len(self.nw)
-         if network:
-             self.Find_Root()
-             network_nodes = list(self.nw.nodes)
-             for node in network_nodes:
-                 if self.nw.in_degree(node)>1:
-                     self.no_of_hybrids+=1
-                     enumerated_parents = list(enumerate(self.nw.predecessors(node))) 
-                     for i,parent in enumerated_parents:
-                         if i==0:
-                             self.hybrid_nodes[node]=self.no_of_hybrids
-                         else:
-                             self.nw.add_edges_from([(parent,self.current_node,self.nw[parent][node])])
-                             self.nw.remove_edge(parent,node)
-                             self.hybrid_nodes[self.current_node] = self.no_of_hybrids
-                             self.current_node+=1
-#             self.CheckLabelSet()
-
-    #Returns the root node of the tree
-    def Find_Root(self):
-        for node in self.nw.nodes:
-            if self.nw.in_degree(node)==0:
-                self.root = node  
-                return node           
-
-    #Returns a newick string for the tree
-    def Newick(self,probabilities = False):
-        return self.Newick_Recursive(self.root,probabilities = probabilities)+";"
-
-    #Returns the newick string for the subtree with given root
-    #does not append the; at the end, for the full newick string of the tree, use Newick()
-    # auxiliary function for finding the newick string for the tree
-    def Newick_Recursive(self,root,probabilities = False):
-        if self.nw.out_degree(root)==0:
-            if root in self.hybrid_nodes:
-                return "#H"+str(self.hybrid_nodes[root])
-            elif root in self.leaf_labels:
-                return self.leaf_labels[root]
-            return str(root)
-        Newick = ""
-        for v in self.nw.successors(root):
-            Newick+= self.Newick_Recursive(v,probabilities)+":"+str(self.nw[root][v]['length'])
-            if probabilities and v in self.hybrid_nodes:
-                Newick+="::"+str(self.nw[root][v]['prob'])
-            Newick+= ","
-        Newick = "("+Newick[:-1]+")"
-        if root in self.hybrid_nodes:
-            Newick += "#H"+str(self.hybrid_nodes[root])
-        return Newick
-
-    '''
-    def CheckLabelSet(self):
-        for v in self.nw.nodes:
-            if self.nw.out_degree(v)==0:
-                if v not in self.leaf_labels and v not in self.hybrid_nodes:
-                    print("non-labelled leaf!")
-                    return False
-        return True
-    '''
-
-
-
-
-
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########              AAF PHYLOGENETIC NETWORK CLASS               #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-
-
-#A class for phylogenetic networks
-class PhN:
-    def __init__(self, seq = None, newick = None, best_tree_from_network = None, reduced_trees = None, heights = None):
-        #the actual graph
-        self.nw = nx.DiGraph()
-        #the set of leaf labels of the network
-        self.leaves = set()
-        #a dictionary giving the node for a given leaf label
-        self.labels = dict()
-        #the number of nodes in the graph
-        self.no_nodes = 0
-        self.leaf_nodes = dict()
-        self.TCS=seq
-        self.CPS=seq
-        self.newick=newick
-        self.reducible_pairs=set()
-        self.reticulated_cherries=set()
-        self.cherries=set()
-        self.level = None
-        self.no_embedded_trees = 0
-        #if a cherry-picking sequence is given, build the network from this sequence
-        if seq:
-            total_len = len(seq)
-            current_trees_embedded = set()
-            #Creates a phylogenetic network from a cherry picking sequence:
-            if reduced_trees:
-                for i,pair in enumerate(reversed(seq)):
-                    if heights:
-                        self.add_pair(*pair,red_trees = reduced_trees[total_len-1-i], current_trees=current_trees_embedded, height = heights[total_len-1-i])
-                        current_trees_embedded = current_trees_embedded | reduced_trees[total_len-1-i]
-                    else:
-                        self.add_pair(*pair,red_trees = reduced_trees[total_len-1-i], current_trees=current_trees_embedded)
-                self.no_embedded_trees = len(current_trees_embedded)
-                self.ScoreEdges()
-            else:
-                for pair in reversed(seq):
-                    self.add_pair(*pair)
-        #if a newick string is given, build the network from the newick string
-        elif newick:
-            self.newick = newick
-            network, self.leaves, self.labels = Newick_To_Network(newick)
-            self.nw = network
-            self.no_nodes = len(list(self.nw))
-            self.Compute_Leaf_Nodes()
-        #if a network 'best_tree_from_network' is given, extract the best tree from this network and use this tree as the network            
-        elif best_tree_from_network:
-            self.nw.add_edges_from(best_tree_from_network.Best_Tree())
-            self.labels = best_tree_from_network.labels
-            self.leaf_nodes = best_tree_from_network.leaf_nodes
-            self.leaves = best_tree_from_network.leaves
-            self.no_nodes = best_tree_from_network.no_nodes
-            #self.Clean_Up()
-
-
-    #Checks if the graph in the instance is a network
-    # i.e., checks whether it has a single root, all levaes are labeled, there are no degree-2 nodes, and each non-leaf non-root node is either a reticulation or a tree node.
-    def IsANetwork(self):
-        rootFound = False
-        for v in self.nw.nodes:
-            if self.nw.in_degree(v) == 0:
-                if rootFound:
-                    print("Multiple Roots!")
-                    return False
-                rootFound = True
-            if self.nw.out_degree(v) == 0 and not v in self.leaf_nodes:
-                print("Unlabelled leaf!")
-                return False
-            if self.nw.out_degree(v) == 1 and self.nw.in_degree(v) == 1:
-                print("Suppressable node, do not forget to clean up your network!")
-                return False
-            if self.nw.out_degree(v) > 1 and self.nw.in_degree(v) > 1:
-                print("Combined split and reticulation!")
-                return False
-        return True
-
-
-    #Returns the leaf nodes of the network
-    def Compute_Leaf_Nodes(self):
-        self.leaf_nodes = dict()
-        for v in self.labels:
-            self.leaf_nodes[self.labels[v]]=v
-            
-    #Returns the level (retirculations in the largest biconnected component) of the network
-    def Level(self, recompute = False):
-        if recompute or not self.level:
-            blobs = nx.biconnected_component_edges(self.nw.to_undirected())
-            lvl = 0
-            for b_edges in blobs:
-                blob = nx.Graph(b_edges)
-                lvl = max(lvl, blob.number_of_edges() - blob.number_of_nodes() +1)
-            self.level = lvl
-        return self.level 
-                  
-    
-    
-    #Add the probabilities for each edge, returns true
-    # probabilties of hybrid edges are stored as edge property 'prob' (i.e. fraction of TREES THAT GO THROUGH THE RETICULATION NODE that use this edge)
-    # probabilities of all edges are stored in 'probability_all'
-    # the fraction of ALL INPUT TREES going through the edge is stored in 'frac_of_trees'
-    def ScoreEdges(self):
-        for node in self.nw.nodes:
-            #for the hybrid edges
-            if self.nw.in_degree(node)>1:
-                total_trees = 0.0
-                for parent in self.nw.predecessors(node):
-                   total_trees+= self.nw[parent][node]['no_of_trees']
-                for parent in self.nw.predecessors(node):
-                   self.nw[parent][node]['prob'] = self.nw[parent][node]['no_of_trees']/total_trees
-                   self.nw[parent][node]['probability_all'] = self.nw[parent][node]['prob']
-                   if self.no_embedded_trees > 0:
-                       self.nw[parent][node]['frac_of_trees'] = self.nw[parent][node]['no_of_trees']/float(self.no_embedded_trees)
-            #and also for the non-hybrid edges (their probability is one)
-            else:
-                for parent in self.nw.predecessors(node):
-                    self.nw[parent][node]['probability_all'] = 1
-                    if self.no_embedded_trees > 0:
-                        self.nw[parent][node]['frac_of_trees'] = self.nw[parent][node]['no_of_trees']/float(self.no_embedded_trees)
-        return True
-
-
-    #Adds a pair to the network, using the construction from a cherry-picking sequence
-    # returns false if y is not yet in the network and the network is not empty
-    def add_pair(self,x,y, red_trees = set(), current_trees = set(), height = [1,1]):
-        #if the network is empty, create a cherry (x,y)
-        if len(self.leaves)==0:
-            self.nw.add_edge(0,1,no_of_trees=len(red_trees), length=0)
-            self.nw.add_edge(1,2,no_of_trees=len(red_trees), length=height[0])
-            self.nw.add_edge(1,3,no_of_trees=len(red_trees), length=height[1])
-            self.leaves = set([x,y])
-            self.labels[x]=2
-            self.labels[y]=3
-            self.leaf_nodes[2]=x
-            self.leaf_nodes[3]=y
-            self.no_nodes=4
-            return True
-        #if y is not in the network return false, as there is no way to add the pair and get a phylogenetic network
-        if y not in self.leaves:
-            return False
-        #add the pair to the existing network
-        node_y=self.labels[y]
-        parent_node_y = -1
-        for p in self.nw.predecessors(node_y):
-            parent_node_y=p
-
-        #first add all edges around y
-        length_incoming_y = self.nw[parent_node_y][node_y]['length']
-        no_of_trees_incoming_y = self.nw[parent_node_y][node_y]['no_of_trees']
-        height_goal_x = height[0]
-        if height[1]<length_incoming_y:
-            height_pair_y_real = height[1]
-        else:
-            height_pair_y_real = length_incoming_y
-            height_goal_x+=height[1]-height_pair_y_real
-        
-        
-        self.nw.add_edge(node_y,self.no_nodes,no_of_trees=no_of_trees_incoming_y+len(red_trees-current_trees), length=height_pair_y_real)
-        self.nw[parent_node_y][node_y]['length'] = length_incoming_y - height_pair_y_real
-        self.leaf_nodes.pop(self.labels[y],False)
-        self.labels[y]=self.no_nodes
-        self.leaf_nodes[self.no_nodes]=y
-
-        #Now also add edges around x
-        #x is not yet in the network, so make a cherry (x,y)
-        if x not in self.leaves:
-            self.nw.add_edge(node_y,self.no_nodes+1,no_of_trees=len(red_trees), length=height_goal_x)
-            self.leaves.add(x)
-            self.labels[x]=self.no_nodes+1
-            self.leaf_nodes[self.no_nodes+1]=x
-            self.no_nodes+=2          
-        #x is already in the network, so create a reticulate cherry (x,y)
-        else:
-            node_x=self.labels[x]
-            for parent in self.nw.predecessors(node_x):
-                px = parent
-            length_incoming_x = self.nw[px][node_x]['length']
-            no_of_trees_incoming_x = self.nw[px][node_x]['no_of_trees']
-            #if x is below a reticulation, and the height of the new pair is above the height of this reticulation, add the new hybrid arc to the existing reticulation
-            if self.nw.in_degree(px)>1 and length_incoming_x<=height_goal_x:
-                self.nw.add_edge(node_y,px,no_of_trees=len(red_trees), length=height_goal_x-length_incoming_x)
-                self.nw[px][node_x]['no_of_trees']+=len(red_trees)
-                self.no_nodes+=1
-            #create a new reticulation vertex above x to attach the hybrid arc to
-            else: 
-                height_pair_x = min(height_goal_x,length_incoming_x)
-                self.nw.add_edge(node_y,node_x,no_of_trees=len(red_trees), length=height_goal_x-height_pair_x)
-                self.nw.add_edge(node_x,self.no_nodes+1,no_of_trees = no_of_trees_incoming_x+len(red_trees), length = height_pair_x)
-                self.nw[px][node_x]['length'] = length_incoming_x - height_pair_x
-                self.leaf_nodes.pop(self.labels[x],False)
-                self.labels[x]=self.no_nodes+1
-                self.leaf_nodes[self.no_nodes+1]=x
-                self.no_nodes+=2
-        return True
-
-
-    
-
-
-    #returns the 'best tree' in the network
-    # i.e., pick the best incoming arc for each reticulation, and use this to find a tree.
-    def Best_Tree(self):
-        edges = []
-        for v in self.nw.nodes:
-            best_p=None
-            best_value=-1
-            for p in self.nw.predecessors(v):
-                if self.nw[p][v]['no_of_trees']>best_value:
-                    best_value = self.nw[p][v]['no_of_trees']
-                    best_p=p
-            if best_p:
-                edges.append((best_p,v,self.nw[best_p][v]))
-        return edges
-
-    #Returns a subnetwork by selecting the highest scoring hybrid arcs (we pick 'reticulations' of these) and extending this to a network, so that the resulting network
-    # the threshold may be the fraction of trees that uses the edge, or the probability of the edge.
-    def SelectSubNetworkByReticulations(self,type_is_probability = True, reticulations = 0):
-        restrictedNetwork = PhN(best_tree_from_network = self)
-        score_type = 'frac_of_trees'
-        if type_is_probability:
-            score_type = 'probability_all'
-        for i in range(reticulations):
-            best_score = -1
-            best_edge = None
-            for e in self.nw.edges:
-                if (not restrictedNetwork.nw.has_edge(e[0],e[1])) and self.nw[e[0]][e[1]][score_type]>best_score:
-                    best_edge = e
-                    best_score = self.nw[e[0]][e[1]][score_type]
-            #If we have already selected the whole network
-            if not best_edge:
-                break
-            restrictedNetwork.nw.add_edges_from([(best_edge[0],best_edge[1],self.nw[best_edge[0]][best_edge[1]])])
-            up_node = best_edge[1]
-            while restrictedNetwork.nw.in_degree(up_node) == 0:
-                best_score = -1
-                best_parent = None
-                for parent in self.nw.predecesors(up_node):
-                    if self.nw[parent][up_node][score_type] > best_score:
-                        best_score = self.nw[parent][up_node][score_type]
-                        best_parent = parent
-                restrictedNetwork.nw.add_edges_from([(best_parent,up_node,self.nw[best_parent][up_node])])
-                up_node = best_parent
-        restrictedNetwork.Clean_Up()
-        #Debug: check if we find a valid network
-        restrictedNetwork.IsANetwork()
-        restrictedNetwork.ScoreEdges()
-        return restrictedNetwork
-
-    #Returns a subnetwork by selecting all hybrid arcs that have a score above a given threshold and extending this to a network
-    # the threshold may be the fraction of trees that uses the edge, or the probability of the edge.
-    def SelectSubNetworkByScore(self,type_is_probability = True, score = .5):
-        restrictedNetwork = PhN(best_tree_from_network = self)
-        score_type = 'frac_of_trees'
-        if type_is_probability:
-            score_type = 'probability_all'
-        done = False
-        while not done:
-            best_score = -1
-            best_edge = None
-            for e in self.nw.edges:
-                if (not restrictedNetwork.nw.has_edge(e[0],e[1])) and self.nw[e[0]][e[1]][score_type]>best_score:
-                    best_edge = e
-                    best_score = self.nw[e[0]][e[1]][score_type]
-            if best_score >= score:
-
-                restrictedNetwork.nw.add_edges_from([(best_edge[0],best_edge[1],self.nw[best_edge[0]][best_edge[1]])])
-                up_node = best_edge[1]
-                while restrictedNetwork.nw.in_degree(up_node) == 0:
-                    best_score = -1
-                    best_parent = None
-                    for parent in self.nw.predecesors(up_node):
-                        if self.nw[parent][up_node][score_type] > best_score:
-                            best_score = self.nw[parent][up_node][score_type]
-                            best_parent = parent
-                    restrictedNetwork.nw.add_edges_from([(best_parent,up_node,self.nw[best_parent][up_node])])
-                    up_node = best_parent
-            else:
-                done = True
-        restrictedNetwork.Clean_Up()
-        #Debug: check if we find a valid network
-        restrictedNetwork.IsANetwork()
-        restrictedNetwork.ScoreEdges()
-        return restrictedNetwork
-        
-
-    #Returns true if (x_label,y_label) forms a cherry in the network, false otherwise
-    def Is_Cherry(self,x_label,y_label):
-        if not x_label in self.leaves or not x_label in self.leaves:
-            return False
-        x = self.labels[x_label]
-        y = self.labels[y_label]
-        px=-1
-        py=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        for p in self.nw.predecessors(y):
-            py=p
-        return px==py
-
-    #Returns true if (x_label,y_label) forms a reticulate cherry in the network, false otherwise
-    def Is_Ret_Cherry(self,x_label,y_label):
-        if not x_label in self.leaves or not x_label in self.leaves:
-            return False
-        x = self.labels[x_label]
-        y = self.labels[y_label]
-        px=-1
-        py=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        for p in self.nw.predecessors(y):
-            py=p
-        return (self.nw.in_degree(px)>1) and self.nw.out_degree(px)==1 and (py in self.nw.predecessors(px))
-
-    #Returns true if (x_label,y_label) forms a reducible pair in the network, false otherwise
-    def Is_Reducible_Pair(self,x_label,y_label):
-        if not x_label in self.leaves or not x_label in self.leaves:
-            return False
-        x = self.labels[x_label]
-        y = self.labels[y_label]
-        px=-1
-        py=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        for p in self.nw.predecessors(y):
-            py=p
-        return (px==py) or (self.nw.in_degree(px)>1 and self.nw.out_degree(px)==1 and py in self.nw.predecessors(px))
-
-    #Iteratively removes unlabeled leaves until none are left, then supresses al degree-2 nodes
-    def Clean_Up(self):
-        nodes_to_check = set(deepcopy(self.nw.nodes))
-        while nodes_to_check:
-            v = nodes_to_check.pop()
-            if self.nw.out_degree(v)==0 and v not in self.leaf_nodes:
-                for p in self.nw.predecessors(v):
-                    nodes_to_check.add(p)
-                self.nw.remove_node(v)
-        list_nodes = deepcopy(self.nw.nodes)
-        for v in list_nodes:
-            self.Clean_Node(v)
-
-    #supresses v if it is a degree-2 node
-    def Clean_Node(self,v):
-        if self.nw.out_degree(v)==1 and self.nw.in_degree(v)==1:
-            pv=-1
-            for p in self.nw.predecessors(v):
-                pv=p
-            cv=-1
-            for c in self.nw.successors(v):
-                cv=c
-            self.nw.add_edges_from([(pv,cv,self.nw[v][cv])])
-            if self.nw[pv][v]['length'] and self.nw[v][cv]['length']:
-                self.nw[pv][cv]['length'] = self.nw[pv][v]['length'] + self.nw[v][cv]['length']
-            self.nw.remove_node(v)
-            return True
-        return False
- 
-    #reduces the pair (x_label,y_label) if it is reducible in the network
-    #returns a new set reducible pairs that involve the leaves x_label and y_label
-    def reduce_pair(self,x_label,y_label):
-        if not x_label in self.leaves or not y_label in self.leaves:
-            return set()
-        x = self.labels[x_label]
-        y = self.labels[y_label]
-        px=-1
-        py=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        for p in self.nw.predecessors(y):
-            py=p 
-        if self.Is_Cherry(x_label,y_label):
-            self.reducible_pairs.difference_update(set([(x_label,y_label),(y_label,x_label)])) 
-            self.nw.remove_node(x)
-            self.leaves.remove(x_label)
-            self.labels.pop(x_label,False)
-            self.Clean_Node(py)
-            #AddCherriesInvolving y
-            new_pairs = set([("no_leaf","no_leaf")])|self.Find_Pairs_With_First(y_label)| self.Find_Pairs_With_Second(y_label)
-            self.reducible_pairs=self.reducible_pairs.union(new_pairs-set([("no_leaf","no_leaf")]))
-            return new_pairs
-        if self.Is_Ret_Cherry(x_label,y_label):
-            self.reducible_pairs.difference_update(set([(x_label,y_label),(y_label,x_label)]))
-            self.nw.remove_edge(py,px)
-            self.Clean_Node(px)
-            self.Clean_Node(py)
-            #AddCherriesInvolving x and y
-            new_pairs = set([("no_leaf","no_leaf")])|self.Find_Pairs_With_First(x_label) |self.Find_Pairs_With_Second(x_label)|self.Find_Pairs_With_First(y_label)|self.Find_Pairs_With_Second(y_label)
-            self.reducible_pairs=self.reducible_pairs.union(new_pairs-set([("no_leaf","no_leaf")]))
-            return new_pairs
-        return set()
-    
-
-    #Returns all reducible pairs in the network where x_label is the first element of the pair
-    def Find_Pairs_With_First(self,x_label):
-        pairs = set()
-        x = self.labels[x_label]
-        px=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        if self.nw.in_degree(px)>1:
-            for ppx in self.nw.predecessors(px):
-                for cppx in self.nw.successors(ppx):
-                    if cppx in self.leaf_nodes:
-                        pairs.add((x_label,self.leaf_nodes[cppx]))
-        if self.nw.out_degree(px)>1:
-            for cpx in self.nw.successors(px):
-                if cpx in self.leaf_nodes:
-                    pairs.add((x_label,self.leaf_nodes[cpx]))
-        return pairs-set([(x_label,x_label)])
-
-    #Returns all reducible pairs in the network where x_label is the second element of the pair
-    def Find_Pairs_With_Second(self,x_label):
-        pairs = set()
-        x = self.labels[x_label]
-        px=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        if self.nw.out_degree(px)>1:
-            for cpx in self.nw.successors(px):
-                if cpx in self.leaf_nodes:
-                    pairs.add((self.leaf_nodes[cpx],x_label))
-                if self.nw.in_degree(cpx)>1:
-                    for ccpx in self.nw.successors(cpx):
-                        if ccpx in self.leaf_nodes:
-                            pairs.add((self.leaf_nodes[ccpx],x_label))
-        return pairs-set([(x_label,x_label)])
-
-    #Returns all cherries and reticulate cherries in the network where x_label is the second element of the pair
-    def Find_Pairs_With_Second_Separated(self,x_label):
-        cherries = set()
-        retic_cherries = set()
-        x = self.labels[x_label]
-        px=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        if self.nw.out_degree(px)>1:
-            for cpx in self.nw.successors(px):
-                if cpx in self.leaf_nodes:
-                    cherries.add((self.leaf_nodes[cpx],x_label))
-                if self.nw.in_degree(cpx)>1:
-                    for ccpx in self.nw.successors(cpx):
-                        if ccpx in self.leaf_nodes:
-                            retic_cherries.add((self.leaf_nodes[ccpx],x_label))
-        return cherries-set([(x_label,x_label)]), retic_cherries-set([(x_label,x_label)])
-
-    #Returns all reticulate cherries in the network where x_label is the second element of the pair    
-    def Find_Retic_Cherry_Second(self,x_label):
-        pairs = set()
-        x = self.labels[x_label]
-        px=-1
-        for p in self.nw.predecessors(x):
-            px=p
-        if self.nw.out_degree(px)>1:
-            for cpx in self.nw.successors(px):
-                if self.nw.in_degree(cpx)>1:
-                    for ccpx in self.nw.successors(cpx):
-                        if ccpx in self.leaf_nodes:
-                            pairs.add((self.leaf_nodes[ccpx],x_label))
-        return pairs-set([(x_label,x_label)]) 
-
-    #Returns all reducible pairs in the network
-    # also sets this as value of self.reducible_pairs
-    def Find_All_Reducible_Pairs(self):
-        self.reducible_pairs=set()
-        for l in self.leaves:
-            self.reducible_pairs=self.reducible_pairs.union(self.Find_Pairs_With_First(l))
-            self.reducible_pairs=self.reducible_pairs.union(self.Find_Pairs_With_Second(l))
-        return self.reducible_pairs
-
-    #Returns all cherries and reticulate cherries in the network
-    # also sets these as values of self.cherries and self.reticulate_cherries
-    def Find_All_Reducible_Pairs_Separated(self):
-        self.reticulated_cherries=set()
-        self.cherries=set()        
-        for l in self.leaves:
-            added_cherries, added_retic_cherries = self.Find_Pairs_With_Second_Separated(l)
-            self.cherries=self.reticulated_cherries.union(added_cherries)
-            self.reticulated_cherries=self.reticulated_cherries.union(added_retic_cherries)
-        return(self.cherries, self.reticulated_cherries)
-
-
-
-
-
-
+# import networkx as nx
+# import random
+# import matplotlib.pyplot as plt
+# import os
+# import ast
+# import re
+# import sys
+# import time
+# from copy import deepcopy
+# memodict={}
+# import numpy as np
+
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########                             Index                         #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+# '''
+# AAA I/O Functions
+# 	Functions for reading newick sequences
+# AAB ANALYSIS OF SEQUENCE FOR TREES
+# 	Two functions:
+#           - Checking whether a CPS reduces a set of trees
+#           - Sequence_Add_Roots (i.e. CompletePartialSequence from the paper) to extend a partial CPS to a CPS
+# AAC INPUT SET CLASS with CPS methods
+# 	Class containing a set of inputs
+#         Methods for running the CP heuristic and improving the sequence
+# AAD PHYLOGENETIC TREE CLASS
+# 	Class for a phylogenetic tree
+# 	Contains methods to cherry-pick a tree and to find reducible pairs
+# 	Gives the height of a pair in the tree
+# AAE CutTree CLASS
+# 	Class meant for converting a network into a Newick string
+#         It `cuts' the reticulation arcs to produce a tree that can be converted to Newick
+# AAF PHYLOGENETIC NETWORK CLASS
+#         Class for a phylogenetic network
+#         Contains methods
+# 		to add pairs to the network from a sequence
+# 		to compute scores of edges (inheritance and number of embedded trees)
+#                 to reduce pairs (not used if input consists of only trees)
+
+# '''
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########                     AAA I/O Functions                     #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# ########
+# ######## Convert Newick to a networkx Digraph with labels (and branch lengths)
+# ########
+# #Write length newick: convert ":" to "," and then evaluate as list of lists using ast.literal_eval
+# # Then, in each list, the node is followed by the length of the incoming arc.
+# # This only works as long as each branch has length and all internal nodes are labeled.
+# def Newick_To_Tree(newick, current_labels = dict()):
+#     newick=newick[:-1]
+#     distances = False
+#     #presence of : indicates the use of lengths in the trees
+#     if ":" in newick:
+#         distances = True
+#         #taxon names may already be enclosed by " or ', otherwise, we add these now
+#         if not "'" in newick and not '"' in newick:
+#             newick = re.sub(r"([,\(])([a-zA-Z\d]+)", r"\1'\2", newick)
+#             newick = re.sub(r"([a-zA-Z\d]):", r"\1':", newick)
+#         newick = newick.replace(":",",")
+#     else:
+#         #taxon names may already be enclosed by " or ', otherwise, we add these now
+#         if not "'" in newick and not '"' in newick:
+#             newick = re.sub(r"([,\(])([a-zA-Z\d]+)", r"\1'\2", newick)
+#             newick = re.sub(r"([a-zA-Z\d])([,\(\)])", r"\1'\2", newick)
+#     #turn the string into a pyhton nested list using [ instead of (
+#     newick = newick.replace("(","[")
+#     newick = newick.replace(")","]")
+#     nestedtree = ast.literal_eval(newick)
+#     #parse the nested list into a list of edges with some additional information about the leaves
+#     #we start with the root 2, so that we can append a root edge (1,2)
+#     edges, leaves, current_labels, current_node = NestedList_To_Tree(nestedtree,2,current_labels, distances = distances)
+#     #put all this information into a networkx DiGraph with or without distances/lengths
+#     tree = nx.DiGraph()
+#     if distances:
+#         edges.append((1,2,0))
+#         tree.add_weighted_edges_from(edges,weight='length')
+#     else:
+#         edges.append((1,2))
+#         tree.add_edges_from(edges)
+#     return tree, leaves, current_labels, distances
+
+# #Auxiliary function to convert list of lists to tree (graph)
+# #Works recursively, where we keep track of the nodes we have already used
+# #Leaves are nodes with negative integer as ID, and already existing taxa are coupled to node IDs by current_labels.
+# def NestedList_To_Tree(nestedList, next_node, current_labels, distances = False):
+#     edges = []
+#     leaves = set()
+#     top_node = next_node
+#     current_node = next_node+1
+#     if distances:
+#         #each element in the sublist has 2 properties, the subtree, and the length, which are adjacent in nestedList
+#         for i in range(0,len(nestedList),2):
+#             t = nestedList[i]
+#             length = nestedList[i+1]
+#             if type(t)==list: #Not a leaf
+#                 edges.append((top_node,current_node,length))
+#                 extra_edges, extra_leaves, current_labels, current_node = NestedList_To_Tree(t,current_node,current_labels,distances=distances)
+#             else: #A leaf
+#                 if str(t) not in current_labels:
+#                     current_labels[str(t)] = -len(current_labels)
+#                 edges.append((top_node,current_labels[str(t)],length))
+#                 extra_edges = []
+#                 extra_leaves = set([current_labels[str(t)]])
+#             edges = edges + extra_edges
+#             leaves = leaves.union(extra_leaves)
+#     else:
+#         #no lengths/distances, so each subtree is simply an element of nestedList
+#         for t in nestedList:
+#             if type(t)==list:
+#                 edges.append((top_node,current_node))
+#                 extra_edges, extra_leaves, current_labels, current_node = NestedList_To_Tree(t,current_node,current_labels)
+#             else:
+#                 if str(t) not in current_labels:
+#                     current_labels[str(t)] = -len(current_labels)
+#                 edges.append((top_node,current_labels[str(t)]))
+#                 extra_edges = []
+#                 extra_leaves = set([current_labels[str(t)]])
+#             edges = edges + extra_edges
+#             leaves = leaves.union(extra_leaves)
+#     return edges, leaves, current_labels, current_node
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########          AAB ANALYSIS OF SEQUENCE FOR TREES               #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# #Checks whether a given cherry-picking sequence `seq' reduces a given tree `tree'
+# #if not,    returns false
+# #otherwise, returns the indices of the pairs that actually reduce a cherry in the tree
+# def Sequence_Reduces_Tree(seq,tree):
+#     t_copy=deepcopy(tree)
+#     indices = []
+#     for i, pair in enumerate(seq):
+#         if t_copy.reduce_pair(*pair):
+#             indices +=[i]
+#             if len(t_copy.nw.edges)==1:
+#                 return indices
+#     return False
+
+
+# #Modifies a cherry-picking sequence so that it represents a network with exactly one root.
+# #A sequence may be such that reconstructing a network from the sequence results in multiple roots
+# #This function adds some pairs to the sequence so that the network has a single root.
+# #returns the new sequence, and also modifies the sets of trees reduced by each pair in the sequence, so that the new pairs are also represented (they reduce no trees)
+# def Sequence_add_roots(seq, red_trees):
+#     leaves_encountered = set()
+#     roots = set()
+#     #The roots can be found by going back through the sequence and finding pairs where the second element has not been encountered in the sequence yet
+#     for pair in reversed(seq):
+#         if pair[1] not in leaves_encountered:
+#             roots.add(pair[1])
+#         leaves_encountered.add(pair[0])
+#         leaves_encountered.add(pair[1])
+#     i=0
+#     roots = list(roots)
+#     #Now add some pairs to make sure each second element is already part of some pair in the sequence read backwards, except for the last pair in the sequence
+#     for i in range(len(roots)-1):
+#        seq.append((roots[i],roots[i+1]))
+#        #none of the trees are reduced by the new pairs.
+#        red_trees.append(set())
+#        i+=1
+#     return seq, red_trees
+
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########         AAC INPUT SET CLASS with CPS methods              #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# #Methods for sets of phylogenetic trees
+# class Input_Set:
+#     def __init__(self, newick_strings = []):
+#         #The dictionary of trees
+#         self.trees = dict()
+#         #the set of leaf labels of the trees
+#         self.labels = dict()
+#         self.labels_reversed = dict()
+#         self.leaves = set()
+
+#         #the current best sequence we have found for this set of trees
+#         self.best_seq = None
+#         #the list of reduced trees for each of the pairs in the best sequence
+#         self.best_red_trees = None
+
+#         #the best sequence for the algorithm using lengths as input as well
+#         self.best_seq_with_lengths = None
+#         #the sets of reduced trees for each pair in this sequence
+#         self.best_seq_with_lengths_red_trees = None
+#         #the height of each pair in this sequence
+#         self.best_seq_with_lengths_heights = None
+
+#         #true if distances are used
+#         self.distances = True
+#         #computation times
+#         self.CPS_Compute_Time = 0
+#         self.CPS_Compute_Reps = 0
+
+#         #read the input trees in 'newick_strings'
+#         for n in newick_strings:
+#             tree = PhT()
+#             self.trees[len(self.trees)] = tree
+#             self.labels, distances_in_tree = tree.Tree_From_Newick(newick = n, current_labels = self.labels)
+#             self.distances = self.distances and distances_in_tree
+#         self.leaves = list(self.labels)
+
+#         #make a reverse dictionary for the leaf labels, to look up the label of a given node
+#         for l,i in self.labels.items():
+#             self.labels_reversed[i] = l
+
+#     #Make a deepcopy of an instance
+#     def __deepcopy__(self, memodict={}):
+#         copy_inputs = Input_Set()
+#         copy_inputs.trees = deepcopy(self.trees,memodict)
+#         copy_inputs.labels = deepcopy(self.labels,memodict)
+#         copy_inputs.labels_reversed = deepcopy(self.labels_reversed,memodict)
+#         copy_inputs.leaves = deepcopy(self.leaves,memodict)
+# #        copy_inputs.best_seq = deepcopy(self.best_seq)
+# #        copy_inputs.best_red_trees = deepcopy(self.best_red_trees)
+#         return copy_inputs
+
+#     #Find new cherry-picking sequences for the trees and update the best found
+#     def CPSBound(self, repeats = 1, progress = False, track = False, lengths = False, time_limit = None):
+#         #Set the specific heuristic that we use, based on the user input and whether the trees have lengths
+#         Heuristic = self.CPHeuristic
+#         if track and not lengths:
+#             print("Tracking reducible cherries")
+#             Heuristic = self.CPHeuristicStorePairs
+#         if lengths:
+#             if not self.distances:
+#                 print("not all trees have branch lengths!")
+#                 sys.exit()
+#                 return []
+#             print("Picking the lowest cherry")
+#             Heuristic = self.CPHeuristicLengths
+#             heights_best = []
+#         #Initialize the recorded best sequences and corresponding data
+#         best = None
+#         red_trees_best = []
+#         starting_time = time.time()
+#         #Try as many times as required by the integer 'repeats'
+#         for i in range(repeats):
+#             print(i+1)
+#             if lengths:
+#                 new, reduced_trees, seq_heights = Heuristic(progress=progress)
+#                 print("found sequence of length: "+str(len(new)))
+#             else:
+#                 new, reduced_trees = Heuristic(progress=progress)
+#                 print("found sequence of length: "+str(len(new)))
+#                 print("improving sequence")
+#                 new, reduced_trees = self.Improve_Sequence(new, reduced_trees, progress = progress)
+#                 print("new length = "+str(len(new)))
+#             print("adding roots")
+#             new,reduced_trees = Sequence_add_roots(new,reduced_trees)
+#             if lengths:
+#                 for i in range(len(new)-len(seq_heights)):
+#                     seq_heights+=[seq_heights[-1]]
+#             print("final length = "+str(len(new)))
+#             if best == None or len(new) < len(best):
+#                 best = new
+#                 red_trees_best = reduced_trees
+#                 if lengths:
+#                     heights_best = seq_heights
+#             print("best sequence has length "+str(len(best)))
+#             self.CPS_Compute_Reps+=1
+#             if time_limit and time.time()-starting_time > time_limit:
+#                 break
+#         self.CPS_Compute_Time += time.time() - starting_time
+#         new_seq = best
+#         if lengths:
+#             if not self.best_seq_with_lengths or len(new_seq)<len(self.best_seq_with_lengths):
+#                 converted_new_seq = []
+#                 for pair in new_seq:
+#                     converted_new_seq += [(self.labels_reversed[pair[0]],self.labels_reversed[pair[1]])]
+#                 self.best_seq_with_lengths = converted_new_seq
+#                 self.best_seq_with_lengths_red_trees = red_trees_best
+#                 self.best_seq_with_lengths_heights = heights_best
+#             return self.best_seq_with_lengths
+#         else:
+#             if not self.best_seq or len(new_seq)<len(self.best_seq):
+#                 converted_new_seq = []
+#                 for pair in new_seq:
+#                     converted_new_seq += [(self.labels_reversed[pair[0]],self.labels_reversed[pair[1]])]
+#                 self.best_seq = converted_new_seq
+#                 self.best_red_trees = red_trees_best
+#             return self.best_seq
+
+
+#     #Version of the code that uses minimal memory: recompute reducible pairs when necessary.
+#     def CPHeuristic(self, progress=False):
+#         if progress:
+#             print("Copying all inputs to reduce on")
+#         #Works in a copy of the input trees, copy_of_inputs, because trees have to be reduced somewhere.
+#         copy_of_inputs = deepcopy(self)
+#         if progress:
+#             print("Done, starting reduction of trees")
+#         CPS = []
+#         reduced_trees = []
+#         candidate_leaves = deepcopy(self.leaves)
+#         while copy_of_inputs.trees:
+#             if progress:
+#                 print("Sequence has length: "+str(len(CPS)))
+#                 print(str(len(copy_of_inputs.trees))+" trees left.\n")
+#                 print("Reducing trivial pairs")
+#                  #First reduce trivial cherries
+#             new_seq, new_red_trees = copy_of_inputs.Reduce_Trivial_Pairs(candidate_leaves)
+#             if progress:
+#                 print("done")
+#             CPS           += new_seq
+#             reduced_trees += new_red_trees
+#             if len(copy_of_inputs.trees)==0:
+#                 break
+#              #Now reduce a random cherry from a random tree
+#             random_index, random_tree = random.choice(list(copy_of_inputs.trees.items()))
+#             list_of_cherries = random_tree.Find_All_Reducible_Pairs()
+#             random_cherry = random.choice(list(list_of_cherries))
+#             CPS         += [random_cherry]
+#             reduced_by_random_cherry = copy_of_inputs.Reduce_Pair_In_All(random_cherry)
+#             reduced_trees += [reduced_by_random_cherry]
+#             candidate_leaves = set(random_cherry)
+#         return CPS, reduced_trees
+
+#     #Version of the code that uses more memory: stores all reducible pairs.
+#     #Runs when user toggles -t or --track
+#     def CPHeuristicStorePairs(self, progress=False):
+#         if progress:
+#             print("Copying all inputs to reduce on")
+#         #Works in a copy of the input trees, copy_of_inputs, because trees have to be reduced somewhere.
+#         copy_of_inputs = deepcopy(self)
+#         if progress:
+#             print("Done")
+#         CPS = []
+#         reduced_trees = []
+#         candidate_leaves = deepcopy(self.leaves)
+#         # Make dict of reducible pairs
+#         if progress:
+#             print("finding all reducible pairs")
+#         reducible_pairs = self.Find_All_Pairs()
+#         if progress:
+#             print("found all reducible pairs")
+#         while copy_of_inputs.trees:
+#             if progress:
+#                 print("Sequence has length: "+str(len(CPS)))
+#                 print(str(len(copy_of_inputs.trees))+" trees left.\n")
+#                 print("Reducing trivial pairs")
+#               #First reduce trivial cherries
+#             new_seq, new_red_trees, reducible_pairs = copy_of_inputs.Reduce_Trivial_Pairs_Store_Pairs(candidate_leaves, reducible_pairs)
+#             if progress:
+#                 print("done")
+#             CPS           += new_seq
+#             reduced_trees += new_red_trees
+#             if len(copy_of_inputs.trees)==0:
+#                 break
+
+#                #Now reduce a random cherry from a random tree
+#               #EITHER: (Get random tree, then random pair from the tree), just like in CPHeuristic
+#             random_index, random_tree = random.choice(list(copy_of_inputs.trees.items()))
+#             list_of_cherries = random_tree.Find_All_Reducible_Pairs()
+#             random_cherry = random.choice(list(list_of_cherries))
+
+#               #OR: (Get a random reducible pair from all pairs)
+#               #Note that this would result in a different algorithm than CPHeuristic, so we use the previous option
+# #            random_cherry = random.choice(list(reducible_pairs.keys()))
+
+
+#             CPS         += [random_cherry]
+#             #reduce all trees with this pair, this is where the list of reducible_pairs is used
+#             #using the list makes it faster to find all trees that need to be reduced.
+#             reduced_by_random_cherry = copy_of_inputs.Reduce_Pair_In_All(random_cherry, reducible_pairs = reducible_pairs)
+#             reducible_pairs = copy_of_inputs.Update_Reducible_Pairs(reducible_pairs, reduced_by_random_cherry)
+#             reduced_trees += [reduced_by_random_cherry]
+#             candidate_leaves = set(random_cherry)
+#         return CPS, reduced_trees
+
+
+#     #Version of the code that always picks the lowest available pair
+#     #Runs when user toggles -l or --lengths and all edges in the input trees have lengths.
+#     def CPHeuristicLengths(self, progress=False):
+#         if progress:
+#             print("Copying all inputs to reduce on")
+#         #Works in a copy of the input trees, copy_of_inputs, because trees have to be reduced somewhere.
+#         copy_of_inputs = deepcopy(self)
+#         if progress:
+#             print("Done")
+#         CPS = []
+#         reduced_trees = []
+#         heights_seq = []
+
+#         candidate_leaves = deepcopy(self.leaves)
+#         # Make dict of reducible pairs
+#         if progress:
+#             print("finding all reducible pairs")
+#         reducible_pairs = self.Find_All_Pairs()
+#         current_heights = dict()    #for each reducible pair: [0] gives height, [1] the number of trees it was computed in.
+
+#         if progress:
+#             print("found all reducible pairs")
+#         while copy_of_inputs.trees:
+#             if progress:
+#                 print("Sequence has length: "+str(len(CPS)))
+#                 print(str(len(copy_of_inputs.trees))+" trees left.\n")
+#               #First reduce trivial cherries
+#                 print("Reducing trivial pairs")
+#             new_seq, new_red_trees, reducible_pairs, new_heights_seq = copy_of_inputs.Reduce_Trivial_Pairs_Lengths(candidate_leaves, reducible_pairs)
+#             if progress:
+#                 print("done")
+#             CPS           += new_seq
+#             reduced_trees += new_red_trees
+#             heights_seq   += new_heights_seq
+#             if len(copy_of_inputs.trees)==0:
+#                 break
+
+#                #Now find the lowest cherry.
+#             current_heights = copy_of_inputs.Update_Heights(current_heights, reducible_pairs)
+#             lowest_cherry        = None
+#             lowest_height        = None
+#             lowest_height_tuple  = None
+#             lowest_heights_found = 1
+#             for pair in reducible_pairs:
+#                 height_pair_tuple = current_heights[pair][0]
+#                 height_pair       = float(height_pair_tuple[0]+height_pair_tuple[1])/2
+#                 new_found = False
+#                 if (not lowest_height) or lowest_height>height_pair:
+#                     new_found = True
+#                     lowest_heights_found=1
+#                 elif lowest_height==height_pair:
+#                     lowest_heights_found+=1
+#                     if random.random()<1/float(lowest_heights_found):
+#                         new_found = True
+#                 if new_found:
+#                     lowest_cherry       = pair
+#                     lowest_height       = height_pair
+#                     lowest_height_tuple = height_pair_tuple
+
+
+#             CPS         += [lowest_cherry]
+#             heights_seq += [lowest_height_tuple]
+#             reduced_by_lowest_cherry = copy_of_inputs.Reduce_Pair_In_All(lowest_cherry, reducible_pairs = reducible_pairs)
+#             reducible_pairs = copy_of_inputs.Update_Reducible_Pairs(reducible_pairs, reduced_by_lowest_cherry)
+#             reduced_trees += [reduced_by_lowest_cherry]
+#             candidate_leaves = set(lowest_cherry)
+#         return CPS, reduced_trees, heights_seq
+
+
+#     #Returns an updated distcionary of heights of the reducible pairs
+#     def Update_Heights(self,current_heights,reducible_pairs):
+#         for pair, trees in reducible_pairs.items():
+#             #updating is only necessary when the set of trees for that pair is changed or the reducible pair was not reducible before.
+#             if not pair in current_heights or not current_heights[pair][1]==len(trees):
+#                 height_pair = self.Height_Pair(pair,trees)
+#                 current_heights[pair] = (height_pair, len(trees))
+#         return current_heights
+
+
+#     #Returns the average height of a pair in a set of trees
+#     # The pair must be reducible in each tree in 'trees'
+#     def Height_Pair(self, pair, trees):
+#         height_pair = [0,0]
+#         for t in trees:
+#             height_in_t = self.trees[t].Height_Of_Cherry(*pair)
+#             height_pair[0]+=height_in_t[0]
+#             height_pair[1]+=height_in_t[1]
+#         return [height_pair[0]/float(len(trees)),height_pair[1]/float(len(trees))]
+
+
+#     #Finds the set of reducible pairs in all trees
+#     #Returns a dictionary with reducible pairs as keys, and the trees they reduce as values.
+#     def Find_All_Pairs(self):
+#         reducible_pairs = dict()
+#         for i,t in self.trees.items():
+#             red_pairs_t = t.Find_All_Reducible_Pairs()
+#             for pair in red_pairs_t:
+#                 if pair in reducible_pairs:
+#                     reducible_pairs[pair].add(i)
+#                 else:
+#                     reducible_pairs[pair] = set([i])
+#         return reducible_pairs
+
+
+#     #UReturns the updated dictionary of reducible pairs in all trees after a reduction (with the trees they reduce as values)
+#     #we only need to update for the trees that got reduced: 'new_red_treed'
+#     def Update_Reducible_Pairs(self, reducible_pairs, new_red_trees):
+#         #Remove trees to update from all pairs
+#         for pair,trees in reducible_pairs.items():
+#             trees.difference_update(new_red_trees)
+#             if len(trees)==0:
+#                 del reducible_pairs[pair]
+#         #Add the trees to the right pairs again
+#         for index in new_red_trees:
+#             if index in self.trees:
+#                 t = self.trees[index]
+#                 red_pairs_t = t.Find_All_Reducible_Pairs()
+#                 for pair in red_pairs_t:
+#                     if pair in reducible_pairs:
+#                         reducible_pairs[pair].add(index)
+#                     else:
+#                         reducible_pairs[pair] = set([index])
+#         return reducible_pairs
+
+#     #reduces the given pair in all trees
+#     #Returns the set of trees thet were reduced
+#     #CHANGES THE SET OF TREES, ONLY PERFORM IN A COPY OF THE CLASS INSTANCE
+#     def Reduce_Pair_In_All(self, pair, reducible_pairs = dict()):
+#         reduced_trees_for_pair=[]
+#         if pair in reducible_pairs:
+#             trees_to_reduce = reducible_pairs[pair]
+#         else:
+#             if reducible_pairs:
+#                 print("pair not found, trying all trees")
+#             trees_to_reduce = deepcopy(self.trees)
+#         for i in trees_to_reduce:
+#             if i in self.trees:
+#                 t = self.trees[i]
+#                 if t.reduce_pair(*pair):
+#                     reduced_trees_for_pair+=[i]
+#                     if len(t.nw.edges())<=1:
+#                         del self.trees[i]
+#         return set(reduced_trees_for_pair)
+
+
+#     #reduces the trivial pairs in the current set of trees
+#     #runs efficiently by giving a set of leaves 'candidate_leaves' that may be involved in trivial pairs
+#     #this set must be given; after a reduction of the pair (a,b) only using the leaves a and b works
+#     #Returns the reduced pairs and the sets of trees thet were reduced
+#     #CHANGES THE SET OF TREES, ONLY PERFORM IN A COPY OF THE CLASS INSTANCE
+#     def Reduce_Trivial_Pairs(self,candidate_leaves):
+#         seq = []
+#         reduced_tree_sets = []
+#         while candidate_leaves:
+#             l = candidate_leaves.pop()
+#             new_pairs = list(self.Trivial_Pair_With(l))
+#             if new_pairs:
+#                 seq += new_pairs
+#                 for p in new_pairs:
+#                     red_trees_p = self.Reduce_Pair_In_All(p)
+#                     reduced_tree_sets += [red_trees_p]
+#                     candidate_leaves   = candidate_leaves | set(p)
+#         return seq, reduced_tree_sets
+
+#     #reduces the trivial pairs in the current set of trees
+#     #runs efficiently by giving a set of leaves 'candidate_leaves' that may be involved in trivial pairs
+#     #this set must be given; after a reduction of the pair (a,b) only using the leaves a and b works
+#     #Returns the reduced pairs and the sets of trees thet were reduced, also updates the reducible pairs.
+#     #CHANGES THE SET OF TREES, ONLY PERFORM IN A COPY OF THE CLASS INSTANCE
+#     def Reduce_Trivial_Pairs_Store_Pairs(self,candidate_leaves, reducible_pairs):
+#         seq = []
+#         reduced_tree_sets = []
+#         while candidate_leaves:
+#             l = candidate_leaves.pop()
+#             new_pairs = list(self.Trivial_Pair_With(l))
+#             if new_pairs:
+# #                print("found a trivial pair")
+#                 seq += new_pairs
+#                 for p in new_pairs:
+#                     red_trees_p = self.Reduce_Pair_In_All(p, reducible_pairs = reducible_pairs)
+#                     reducible_pairs = self.Update_Reducible_Pairs(reducible_pairs, red_trees_p)
+#                     reduced_tree_sets += [red_trees_p]
+#                     candidate_leaves   = candidate_leaves | set(p)
+#         return seq, reduced_tree_sets, reducible_pairs
+
+#     #reduces the trivial pairs in the current set of trees with branch lengths
+#     #runs efficiently by giving a set of leaves 'candidate_leaves' that may be involved in trivial pairs
+#     #this set must be given; after a reduction of the pair (a,b) only using the leaves a and b works
+#     #Returns the reduced pairs and the sets of trees thet were reduced, also updates the reducible pairs and their heights.
+#     #CHANGES THE SET OF TREES, ONLY PERFORM IN A COPY OF THE CLASS INSTANCE
+#     def Reduce_Trivial_Pairs_Lengths(self,candidate_leaves, reducible_pairs):
+#         seq = []
+#         reduced_tree_sets = []
+#         heights_seq = []
+#         while candidate_leaves:
+#             l = candidate_leaves.pop()
+#             new_pairs = list(self.Trivial_Pair_With(l))
+#             if new_pairs:
+# #                print("found a trivial pair")
+#                 seq += new_pairs
+#                 for p in new_pairs:
+#                     height_p = self.Height_Pair(p,reducible_pairs[p])
+#                     red_trees_p = self.Reduce_Pair_In_All(p, reducible_pairs = reducible_pairs)
+#                     heights_seq += [height_p]
+#                     reducible_pairs = self.Update_Reducible_Pairs(reducible_pairs, red_trees_p)
+#                     reduced_tree_sets += [red_trees_p]
+#                     candidate_leaves   = candidate_leaves | set(p)
+#         return seq, reduced_tree_sets, reducible_pairs, heights_seq
+
+#     #Returns all trivial pairs involving the leaf l
+#     def Trivial_Pair_With(self,l):
+#         pairs = set()
+#         #Go through all trees t with index i.
+#         for i,t in self.trees.items():
+#             #If the leaf occurs in t
+#             if l in t.leaves:
+#                 #Compute reducible pairs of t with the leaf as first coordinate
+#                 pairs_in_t = t.Find_Pairs_With_First(l)
+#                 #If we did not have a set of candidate pairs yet, use pairs_in_t
+#                 if not pairs:
+#                     pairs = pairs_in_t
+#                 #Else, the candidate pairs must also be in t, so take intersection
+#                 else:
+#                     pairs = pairs & pairs_in_t
+#                 #If we do not have any candidate pairs after checking a tree with l as leaf, we stop.
+#                 if not pairs:
+#                     break
+#         return pairs
+
+
+#     #Improves a sequence 'CPS' for the input trees by removing elements and checking whether the new sequence still reduces all trees
+#     #Returns this improved sequence and the corresponding sets of reduced trees for each pair.
+#     def Improve_Sequence(self, CPS, reduced_trees, progress = False):
+#         seq = deepcopy(CPS)
+#         i=0
+#         while i<len(seq):
+#             redundant = True
+#             relevant_tree_indices = reduced_trees[i]
+#             new_relevant_pairs_for_trees = dict()
+#             for j in relevant_tree_indices:
+#                 #Check if the shorter sequence reduces the trees, and if so, record which pairs reduced a cherry in which tree
+#                 new_relevant_pairs_for_trees[j] = Sequence_Reduces_Tree(seq[:i]+seq[i+1:],self.trees[j])
+#                 if not new_relevant_pairs_for_trees[j]:
+#                     redundant = False
+#                     break
+#             if redundant:
+#                 #Remove the ith element from seq and reduced trees
+#                 seq.pop(i)
+#                 reduced_trees.pop(i)
+#                 #Update reduced_trees for the relevant trees
+#                    #First remove all j in relevant_tree_indices
+#                 for tree_index_set in reduced_trees:
+#                     for j in relevant_tree_indices:
+#                         tree_index_set.discard(j)
+#                    #Now add them back at the right places, according to "new_relevant_pairs_for_trees"
+#                 for j in relevant_tree_indices:
+#                     for index in new_relevant_pairs_for_trees[j]:
+#                         reduced_trees[index].add(j)
+#                 if progress:
+#                     print("New length is "+str(len(seq)))
+#                     print("Continue at position "+str(i))
+#             else:
+#                 i+=1
+#         return seq, reduced_trees
+
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########              AAD PHYLOGENETIC TREE CLASS                  #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# #A class representing a phylogenetic tree
+# #Contains methods to reduce trees
+# class PhT:
+#     def __init__(self):
+#         #the actual graph
+#         self.nw = nx.DiGraph()
+#         #the set of leaf labels of the network
+#         self.leaves = set()
+
+#     #Builds a tree from a newick string
+#     def Tree_From_Newick(self, newick = None, current_labels = dict()):
+#         self.nw, self.leaves, current_labels, distances = Newick_To_Tree(newick, current_labels)
+#         return current_labels, distances
+
+#     #Checks whether the pair (x,y) forms a cherry in the tree
+#     def Is_Cherry(self,x,y):
+#         if (not x in self.leaves) or (not y in self.leaves):
+#             return False
+#         px=-1
+#         py=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         for p in self.nw.predecessors(y):
+#             py=p
+#         return px==py
+
+#     #Returns the height of (x,y) if it is a cherry:
+#     #     i.e.: length(p,x)+length(p,y)/2
+#     #Returns false otherwise
+#     def Height_Of_Cherry(self,x,y):
+#         if (not x in self.leaves) or (not y in self.leaves):
+#             return False
+#         px=-1
+#         py=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         for p in self.nw.predecessors(y):
+#             py=p
+#         if px==py:
+#             height = [float(self.nw[px][x]['length']),float(self.nw[py][y]['length'])]
+#             return height
+#         return False
+
+
+#     #suppresses a degree-2 node v and returns true if successful
+#     # the new arc has length length(p,v)+length(v,c)
+#     #returns false if v is not a degree-2 node
+#     def Clean_Node(self,v):
+#         if self.nw.out_degree(v)==1 and self.nw.in_degree(v)==1:
+#             pv=-1
+#             for p in self.nw.predecessors(v):
+#                 pv=p
+#             cv=-1
+#             for c in self.nw.successors(v):
+#                 cv=c
+#             self.nw.add_edges_from([(pv,cv,self.nw[pv][v])])
+#             if 'length' in self.nw[pv][v] and 'length' in self.nw[v][cv]:
+#                 self.nw[pv][cv]['length']=self.nw[pv][v]['length']+self.nw[v][cv]['length']
+#             self.nw.remove_node(v)
+#             return True
+#         return False
+
+#     #reduces the pair (x,y) in the tree if it is present as cherry
+#     # i.e., removes the leaf x and its incoming arc, and then cleans up its parent node.
+#     # note that if px, and py have different lengths, the length of px is lost in the new network.
+#     #returns true if successful and false otherwise
+#     def reduce_pair(self,x,y):
+#         if not x in self.leaves or not y in self.leaves:
+#             return False
+#         px=-1
+#         py=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         for p in self.nw.predecessors(y):
+#             py=p
+#         if self.Is_Cherry(x,y):
+#             self.nw.remove_node(x)
+#             self.leaves.remove(x)
+#             self.Clean_Node(py)
+#             return True
+#         return False
+
+
+#     #Returns all reducible pairs in the tree involving x, where x is the first element
+#     def Find_Pairs_With_First(self,x):
+#         pairs = set()
+#         px=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         if self.nw.out_degree(px)>1:
+#             for cpx in self.nw.successors(px):
+#                 if cpx in self.leaves:
+#                     pairs.add((x,cpx))
+#         return pairs-set([(x,x)])
+
+#     #Returns all reducible pairs in the tree
+#     def Find_All_Reducible_Pairs(self):
+#         red_pairs=set()
+#         for l in self.leaves:
+#             red_pairs=red_pairs.union(self.Find_Pairs_With_First(l))
+#         return red_pairs
+
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########                     AAE CutTree CLASS                     #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# #A class that represents a network as a tree where hybrid edges have been cut at the hybrid nodes.
+# #Used as an intermediate to find the Newick string of a network.
+# class CutTree:
+#     def __init__(self, network = None, current_node = None, leaf_labels= dict()):
+#          self.hybrid_nodes = dict()
+#          self.no_of_hybrids = 0
+#          self.root = None
+#          self.nw = deepcopy(network)
+#          self.current_node = current_node
+#          self.leaf_labels = leaf_labels
+#          if not self.current_node:
+#              self.current_node = 2*len(self.nw)
+#          if network:
+#              self.Find_Root()
+#              network_nodes = list(self.nw.nodes)
+#              for node in network_nodes:
+#                  if self.nw.in_degree(node)>1:
+#                      self.no_of_hybrids+=1
+#                      enumerated_parents = list(enumerate(self.nw.predecessors(node)))
+#                      for i,parent in enumerated_parents:
+#                          if i==0:
+#                              self.hybrid_nodes[node]=self.no_of_hybrids
+#                          else:
+#                              self.nw.add_edges_from([(parent,self.current_node,self.nw[parent][node])])
+#                              self.nw.remove_edge(parent,node)
+#                              self.hybrid_nodes[self.current_node] = self.no_of_hybrids
+#                              self.current_node+=1
+# #             self.CheckLabelSet()
+
+#     #Returns the root node of the tree
+#     def Find_Root(self):
+#         for node in self.nw.nodes:
+#             if self.nw.in_degree(node)==0:
+#                 self.root = node
+#                 return node
+
+#     #Returns a newick string for the tree
+#     def Newick(self,probabilities = False):
+#         return self.Newick_Recursive(self.root,probabilities = probabilities)+";"
+
+#     #Returns the newick string for the subtree with given root
+#     #does not append the; at the end, for the full newick string of the tree, use Newick()
+#     # auxiliary function for finding the newick string for the tree
+#     def Newick_Recursive(self,root,probabilities = False):
+#         if self.nw.out_degree(root)==0:
+#             if root in self.hybrid_nodes:
+#                 return "#H"+str(self.hybrid_nodes[root])
+#             elif root in self.leaf_labels:
+#                 return self.leaf_labels[root]
+#             return str(root)
+#         Newick = ""
+#         for v in self.nw.successors(root):
+#             Newick+= self.Newick_Recursive(v,probabilities)+":"+str(self.nw[root][v]['length'])
+#             if probabilities and v in self.hybrid_nodes:
+#                 Newick+="::"+str(self.nw[root][v]['prob'])
+#             Newick+= ","
+#         Newick = "("+Newick[:-1]+")"
+#         if root in self.hybrid_nodes:
+#             Newick += "#H"+str(self.hybrid_nodes[root])
+#         return Newick
+
+#     '''
+#     def CheckLabelSet(self):
+#         for v in self.nw.nodes:
+#             if self.nw.out_degree(v)==0:
+#                 if v not in self.leaf_labels and v not in self.hybrid_nodes:
+#                     print("non-labelled leaf!")
+#                     return False
+#         return True
+#     '''
+
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########              AAF PHYLOGENETIC NETWORK CLASS               #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# #A class for phylogenetic networks
+# class PhN:
+#     def __init__(self, seq = None, newick = None, best_tree_from_network = None, reduced_trees = None, heights = None):
+#         #the actual graph
+#         self.nw = nx.DiGraph()
+#         #the set of leaf labels of the network
+#         self.leaves = set()
+#         #a dictionary giving the node for a given leaf label
+#         self.labels = dict()
+#         #the number of nodes in the graph
+#         self.no_nodes = 0
+#         self.leaf_nodes = dict()
+#         self.TCS=seq
+#         self.CPS=seq
+#         self.newick=newick
+#         self.reducible_pairs=set()
+#         self.reticulated_cherries=set()
+#         self.cherries=set()
+#         self.level = None
+#         self.no_embedded_trees = 0
+#         #if a cherry-picking sequence is given, build the network from this sequence
+#         if seq:
+#             total_len = len(seq)
+#             current_trees_embedded = set()
+#             #Creates a phylogenetic network from a cherry picking sequence:
+#             if reduced_trees:
+#                 for i,pair in enumerate(reversed(seq)):
+#                     if heights:
+#                         self.add_pair(*pair,red_trees = reduced_trees[total_len-1-i], current_trees=current_trees_embedded, height = heights[total_len-1-i])
+#                         current_trees_embedded = current_trees_embedded | reduced_trees[total_len-1-i]
+#                     else:
+#                         self.add_pair(*pair,red_trees = reduced_trees[total_len-1-i], current_trees=current_trees_embedded)
+#                 self.no_embedded_trees = len(current_trees_embedded)
+#                 self.ScoreEdges()
+#             else:
+#                 for pair in reversed(seq):
+#                     self.add_pair(*pair)
+#         #if a newick string is given, build the network from the newick string
+#         elif newick:
+#             self.newick = newick
+#             network, self.leaves, self.labels = Newick_To_Network(newick)
+#             self.nw = network
+#             self.no_nodes = len(list(self.nw))
+#             self.Compute_Leaf_Nodes()
+#         #if a network 'best_tree_from_network' is given, extract the best tree from this network and use this tree as the network
+#         elif best_tree_from_network:
+#             self.nw.add_edges_from(best_tree_from_network.Best_Tree())
+#             self.labels = best_tree_from_network.labels
+#             self.leaf_nodes = best_tree_from_network.leaf_nodes
+#             self.leaves = best_tree_from_network.leaves
+#             self.no_nodes = best_tree_from_network.no_nodes
+#             #self.Clean_Up()
+
+
+#     #Checks if the graph in the instance is a network
+#     # i.e., checks whether it has a single root, all levaes are labeled, there are no degree-2 nodes, and each non-leaf non-root node is either a reticulation or a tree node.
+#     def IsANetwork(self):
+#         rootFound = False
+#         for v in self.nw.nodes:
+#             if self.nw.in_degree(v) == 0:
+#                 if rootFound:
+#                     print("Multiple Roots!")
+#                     return False
+#                 rootFound = True
+#             if self.nw.out_degree(v) == 0 and not v in self.leaf_nodes:
+#                 print("Unlabelled leaf!")
+#                 return False
+#             if self.nw.out_degree(v) == 1 and self.nw.in_degree(v) == 1:
+#                 print("Suppressable node, do not forget to clean up your network!")
+#                 return False
+#             if self.nw.out_degree(v) > 1 and self.nw.in_degree(v) > 1:
+#                 print("Combined split and reticulation!")
+#                 return False
+#         return True
+
+
+#     #Returns the leaf nodes of the network
+#     def Compute_Leaf_Nodes(self):
+#         self.leaf_nodes = dict()
+#         for v in self.labels:
+#             self.leaf_nodes[self.labels[v]]=v
+
+#     #Returns the level (retirculations in the largest biconnected component) of the network
+#     def Level(self, recompute = False):
+#         if recompute or not self.level:
+#             blobs = nx.biconnected_component_edges(self.nw.to_undirected())
+#             lvl = 0
+#             for b_edges in blobs:
+#                 blob = nx.Graph(b_edges)
+#                 lvl = max(lvl, blob.number_of_edges() - blob.number_of_nodes() +1)
+#             self.level = lvl
+#         return self.level
+
+
+#     #Add the probabilities for each edge, returns true
+#     # probabilties of hybrid edges are stored as edge property 'prob' (i.e. fraction of TREES THAT GO THROUGH THE RETICULATION NODE that use this edge)
+#     # probabilities of all edges are stored in 'probability_all'
+#     # the fraction of ALL INPUT TREES going through the edge is stored in 'frac_of_trees'
+#     def ScoreEdges(self):
+#         for node in self.nw.nodes:
+#             #for the hybrid edges
+#             if self.nw.in_degree(node)>1:
+#                 total_trees = 0.0
+#                 for parent in self.nw.predecessors(node):
+#                    total_trees+= self.nw[parent][node]['no_of_trees']
+#                 for parent in self.nw.predecessors(node):
+#                    self.nw[parent][node]['prob'] = self.nw[parent][node]['no_of_trees']/total_trees
+#                    self.nw[parent][node]['probability_all'] = self.nw[parent][node]['prob']
+#                    if self.no_embedded_trees > 0:
+#                        self.nw[parent][node]['frac_of_trees'] = self.nw[parent][node]['no_of_trees']/float(self.no_embedded_trees)
+#             #and also for the non-hybrid edges (their probability is one)
+#             else:
+#                 for parent in self.nw.predecessors(node):
+#                     self.nw[parent][node]['probability_all'] = 1
+#                     if self.no_embedded_trees > 0:
+#                         self.nw[parent][node]['frac_of_trees'] = self.nw[parent][node]['no_of_trees']/float(self.no_embedded_trees)
+#         return True
+
+
+#     #Adds a pair to the network, using the construction from a cherry-picking sequence
+#     # returns false if y is not yet in the network and the network is not empty
+#     def add_pair(self,x,y, red_trees = set(), current_trees = set(), height = [1,1]):
+#         #if the network is empty, create a cherry (x,y)
+#         if len(self.leaves)==0:
+#             self.nw.add_edge(0,1,no_of_trees=len(red_trees), length=0)
+#             self.nw.add_edge(1,2,no_of_trees=len(red_trees), length=height[0])
+#             self.nw.add_edge(1,3,no_of_trees=len(red_trees), length=height[1])
+#             self.leaves = set([x,y])
+#             self.labels[x]=2
+#             self.labels[y]=3
+#             self.leaf_nodes[2]=x
+#             self.leaf_nodes[3]=y
+#             self.no_nodes=4
+#             return True
+#         #if y is not in the network return false, as there is no way to add the pair and get a phylogenetic network
+#         if y not in self.leaves:
+#             return False
+#         #add the pair to the existing network
+#         node_y=self.labels[y]
+#         parent_node_y = -1
+#         for p in self.nw.predecessors(node_y):
+#             parent_node_y=p
+
+#         #first add all edges around y
+#         length_incoming_y = self.nw[parent_node_y][node_y]['length']
+#         no_of_trees_incoming_y = self.nw[parent_node_y][node_y]['no_of_trees']
+#         height_goal_x = height[0]
+#         if height[1]<length_incoming_y:
+#             height_pair_y_real = height[1]
+#         else:
+#             height_pair_y_real = length_incoming_y
+#             height_goal_x+=height[1]-height_pair_y_real
+
+
+#         self.nw.add_edge(node_y,self.no_nodes,no_of_trees=no_of_trees_incoming_y+len(red_trees-current_trees), length=height_pair_y_real)
+#         self.nw[parent_node_y][node_y]['length'] = length_incoming_y - height_pair_y_real
+#         self.leaf_nodes.pop(self.labels[y],False)
+#         self.labels[y]=self.no_nodes
+#         self.leaf_nodes[self.no_nodes]=y
+
+#         #Now also add edges around x
+#         #x is not yet in the network, so make a cherry (x,y)
+#         if x not in self.leaves:
+#             self.nw.add_edge(node_y,self.no_nodes+1,no_of_trees=len(red_trees), length=height_goal_x)
+#             self.leaves.add(x)
+#             self.labels[x]=self.no_nodes+1
+#             self.leaf_nodes[self.no_nodes+1]=x
+#             self.no_nodes+=2
+#         #x is already in the network, so create a reticulate cherry (x,y)
+#         else:
+#             node_x=self.labels[x]
+#             for parent in self.nw.predecessors(node_x):
+#                 px = parent
+#             length_incoming_x = self.nw[px][node_x]['length']
+#             no_of_trees_incoming_x = self.nw[px][node_x]['no_of_trees']
+#             #if x is below a reticulation, and the height of the new pair is above the height of this reticulation, add the new hybrid arc to the existing reticulation
+#             if self.nw.in_degree(px)>1 and length_incoming_x<=height_goal_x:
+#                 self.nw.add_edge(node_y,px,no_of_trees=len(red_trees), length=height_goal_x-length_incoming_x)
+#                 self.nw[px][node_x]['no_of_trees']+=len(red_trees)
+#                 self.no_nodes+=1
+#             #create a new reticulation vertex above x to attach the hybrid arc to
+#             else:
+#                 height_pair_x = min(height_goal_x,length_incoming_x)
+#                 self.nw.add_edge(node_y,node_x,no_of_trees=len(red_trees), length=height_goal_x-height_pair_x)
+#                 self.nw.add_edge(node_x,self.no_nodes+1,no_of_trees = no_of_trees_incoming_x+len(red_trees), length = height_pair_x)
+#                 self.nw[px][node_x]['length'] = length_incoming_x - height_pair_x
+#                 self.leaf_nodes.pop(self.labels[x],False)
+#                 self.labels[x]=self.no_nodes+1
+#                 self.leaf_nodes[self.no_nodes+1]=x
+#                 self.no_nodes+=2
+#         return True
+
+
+#     #returns the 'best tree' in the network
+#     # i.e., pick the best incoming arc for each reticulation, and use this to find a tree.
+#     def Best_Tree(self):
+#         edges = []
+#         for v in self.nw.nodes:
+#             best_p=None
+#             best_value=-1
+#             for p in self.nw.predecessors(v):
+#                 if self.nw[p][v]['no_of_trees']>best_value:
+#                     best_value = self.nw[p][v]['no_of_trees']
+#                     best_p=p
+#             if best_p:
+#                 edges.append((best_p,v,self.nw[best_p][v]))
+#         return edges
+
+#     #Returns a subnetwork by selecting the highest scoring hybrid arcs (we pick 'reticulations' of these) and extending this to a network, so that the resulting network
+#     # the threshold may be the fraction of trees that uses the edge, or the probability of the edge.
+#     def SelectSubNetworkByReticulations(self,type_is_probability = True, reticulations = 0):
+#         restrictedNetwork = PhN(best_tree_from_network = self)
+#         score_type = 'frac_of_trees'
+#         if type_is_probability:
+#             score_type = 'probability_all'
+#         for i in range(reticulations):
+#             best_score = -1
+#             best_edge = None
+#             for e in self.nw.edges:
+#                 if (not restrictedNetwork.nw.has_edge(e[0],e[1])) and self.nw[e[0]][e[1]][score_type]>best_score:
+#                     best_edge = e
+#                     best_score = self.nw[e[0]][e[1]][score_type]
+#             #If we have already selected the whole network
+#             if not best_edge:
+#                 break
+#             restrictedNetwork.nw.add_edges_from([(best_edge[0],best_edge[1],self.nw[best_edge[0]][best_edge[1]])])
+#             up_node = best_edge[1]
+#             while restrictedNetwork.nw.in_degree(up_node) == 0:
+#                 best_score = -1
+#                 best_parent = None
+#                 for parent in self.nw.predecesors(up_node):
+#                     if self.nw[parent][up_node][score_type] > best_score:
+#                         best_score = self.nw[parent][up_node][score_type]
+#                         best_parent = parent
+#                 restrictedNetwork.nw.add_edges_from([(best_parent,up_node,self.nw[best_parent][up_node])])
+#                 up_node = best_parent
+#         restrictedNetwork.Clean_Up()
+#         #Debug: check if we find a valid network
+#         restrictedNetwork.IsANetwork()
+#         restrictedNetwork.ScoreEdges()
+#         return restrictedNetwork
+
+#     #Returns a subnetwork by selecting all hybrid arcs that have a score above a given threshold and extending this to a network
+#     # the threshold may be the fraction of trees that uses the edge, or the probability of the edge.
+#     def SelectSubNetworkByScore(self,type_is_probability = True, score = .5):
+#         restrictedNetwork = PhN(best_tree_from_network = self)
+#         score_type = 'frac_of_trees'
+#         if type_is_probability:
+#             score_type = 'probability_all'
+#         done = False
+#         while not done:
+#             best_score = -1
+#             best_edge = None
+#             for e in self.nw.edges:
+#                 if (not restrictedNetwork.nw.has_edge(e[0],e[1])) and self.nw[e[0]][e[1]][score_type]>best_score:
+#                     best_edge = e
+#                     best_score = self.nw[e[0]][e[1]][score_type]
+#             if best_score >= score:
+
+#                 restrictedNetwork.nw.add_edges_from([(best_edge[0],best_edge[1],self.nw[best_edge[0]][best_edge[1]])])
+#                 up_node = best_edge[1]
+#                 while restrictedNetwork.nw.in_degree(up_node) == 0:
+#                     best_score = -1
+#                     best_parent = None
+#                     for parent in self.nw.predecesors(up_node):
+#                         if self.nw[parent][up_node][score_type] > best_score:
+#                             best_score = self.nw[parent][up_node][score_type]
+#                             best_parent = parent
+#                     restrictedNetwork.nw.add_edges_from([(best_parent,up_node,self.nw[best_parent][up_node])])
+#                     up_node = best_parent
+#             else:
+#                 done = True
+#         restrictedNetwork.Clean_Up()
+#         #Debug: check if we find a valid network
+#         restrictedNetwork.IsANetwork()
+#         restrictedNetwork.ScoreEdges()
+#         return restrictedNetwork
+
+
+#     #Returns true if (x_label,y_label) forms a cherry in the network, false otherwise
+#     def Is_Cherry(self,x_label,y_label):
+#         if not x_label in self.leaves or not x_label in self.leaves:
+#             return False
+#         x = self.labels[x_label]
+#         y = self.labels[y_label]
+#         px=-1
+#         py=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         for p in self.nw.predecessors(y):
+#             py=p
+#         return px==py
+
+#     #Returns true if (x_label,y_label) forms a reticulate cherry in the network, false otherwise
+#     def Is_Ret_Cherry(self,x_label,y_label):
+#         if not x_label in self.leaves or not x_label in self.leaves:
+#             return False
+#         x = self.labels[x_label]
+#         y = self.labels[y_label]
+#         px=-1
+#         py=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         for p in self.nw.predecessors(y):
+#             py=p
+#         return (self.nw.in_degree(px)>1) and self.nw.out_degree(px)==1 and (py in self.nw.predecessors(px))
+
+#     #Returns true if (x_label,y_label) forms a reducible pair in the network, false otherwise
+#     def Is_Reducible_Pair(self,x_label,y_label):
+#         if not x_label in self.leaves or not x_label in self.leaves:
+#             return False
+#         x = self.labels[x_label]
+#         y = self.labels[y_label]
+#         px=-1
+#         py=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         for p in self.nw.predecessors(y):
+#             py=p
+#         return (px==py) or (self.nw.in_degree(px)>1 and self.nw.out_degree(px)==1 and py in self.nw.predecessors(px))
+
+#     #Iteratively removes unlabeled leaves until none are left, then supresses al degree-2 nodes
+#     def Clean_Up(self):
+#         nodes_to_check = set(deepcopy(self.nw.nodes))
+#         while nodes_to_check:
+#             v = nodes_to_check.pop()
+#             if self.nw.out_degree(v)==0 and v not in self.leaf_nodes:
+#                 for p in self.nw.predecessors(v):
+#                     nodes_to_check.add(p)
+#                 self.nw.remove_node(v)
+#         list_nodes = deepcopy(self.nw.nodes)
+#         for v in list_nodes:
+#             self.Clean_Node(v)
+
+#     #supresses v if it is a degree-2 node
+#     def Clean_Node(self,v):
+#         if self.nw.out_degree(v)==1 and self.nw.in_degree(v)==1:
+#             pv=-1
+#             for p in self.nw.predecessors(v):
+#                 pv=p
+#             cv=-1
+#             for c in self.nw.successors(v):
+#                 cv=c
+#             self.nw.add_edges_from([(pv,cv,self.nw[v][cv])])
+#             if self.nw[pv][v]['length'] and self.nw[v][cv]['length']:
+#                 self.nw[pv][cv]['length'] = self.nw[pv][v]['length'] + self.nw[v][cv]['length']
+#             self.nw.remove_node(v)
+#             return True
+#         return False
+
+#     #reduces the pair (x_label,y_label) if it is reducible in the network
+#     #returns a new set reducible pairs that involve the leaves x_label and y_label
+#     def reduce_pair(self,x_label,y_label):
+#         if not x_label in self.leaves or not y_label in self.leaves:
+#             return set()
+#         x = self.labels[x_label]
+#         y = self.labels[y_label]
+#         px=-1
+#         py=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         for p in self.nw.predecessors(y):
+#             py=p
+#         if self.Is_Cherry(x_label,y_label):
+#             self.reducible_pairs.difference_update(set([(x_label,y_label),(y_label,x_label)]))
+#             self.nw.remove_node(x)
+#             self.leaves.remove(x_label)
+#             self.labels.pop(x_label,False)
+#             self.Clean_Node(py)
+#             #AddCherriesInvolving y
+#             new_pairs = set([("no_leaf","no_leaf")])|self.Find_Pairs_With_First(y_label)| self.Find_Pairs_With_Second(y_label)
+#             self.reducible_pairs=self.reducible_pairs.union(new_pairs-set([("no_leaf","no_leaf")]))
+#             return new_pairs
+#         if self.Is_Ret_Cherry(x_label,y_label):
+#             self.reducible_pairs.difference_update(set([(x_label,y_label),(y_label,x_label)]))
+#             self.nw.remove_edge(py,px)
+#             self.Clean_Node(px)
+#             self.Clean_Node(py)
+#             #AddCherriesInvolving x and y
+#             new_pairs = set([("no_leaf","no_leaf")])|self.Find_Pairs_With_First(x_label) |self.Find_Pairs_With_Second(x_label)|self.Find_Pairs_With_First(y_label)|self.Find_Pairs_With_Second(y_label)
+#             self.reducible_pairs=self.reducible_pairs.union(new_pairs-set([("no_leaf","no_leaf")]))
+#             return new_pairs
+#         return set()
+
+
+#     #Returns all reducible pairs in the network where x_label is the first element of the pair
+#     def Find_Pairs_With_First(self,x_label):
+#         pairs = set()
+#         x = self.labels[x_label]
+#         px=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         if self.nw.in_degree(px)>1:
+#             for ppx in self.nw.predecessors(px):
+#                 for cppx in self.nw.successors(ppx):
+#                     if cppx in self.leaf_nodes:
+#                         pairs.add((x_label,self.leaf_nodes[cppx]))
+#         if self.nw.out_degree(px)>1:
+#             for cpx in self.nw.successors(px):
+#                 if cpx in self.leaf_nodes:
+#                     pairs.add((x_label,self.leaf_nodes[cpx]))
+#         return pairs-set([(x_label,x_label)])
+
+#     #Returns all reducible pairs in the network where x_label is the second element of the pair
+#     def Find_Pairs_With_Second(self,x_label):
+#         pairs = set()
+#         x = self.labels[x_label]
+#         px=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         if self.nw.out_degree(px)>1:
+#             for cpx in self.nw.successors(px):
+#                 if cpx in self.leaf_nodes:
+#                     pairs.add((self.leaf_nodes[cpx],x_label))
+#                 if self.nw.in_degree(cpx)>1:
+#                     for ccpx in self.nw.successors(cpx):
+#                         if ccpx in self.leaf_nodes:
+#                             pairs.add((self.leaf_nodes[ccpx],x_label))
+#         return pairs-set([(x_label,x_label)])
+
+#     #Returns all cherries and reticulate cherries in the network where x_label is the second element of the pair
+#     def Find_Pairs_With_Second_Separated(self,x_label):
+#         cherries = set()
+#         retic_cherries = set()
+#         x = self.labels[x_label]
+#         px=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         if self.nw.out_degree(px)>1:
+#             for cpx in self.nw.successors(px):
+#                 if cpx in self.leaf_nodes:
+#                     cherries.add((self.leaf_nodes[cpx],x_label))
+#                 if self.nw.in_degree(cpx)>1:
+#                     for ccpx in self.nw.successors(cpx):
+#                         if ccpx in self.leaf_nodes:
+#                             retic_cherries.add((self.leaf_nodes[ccpx],x_label))
+#         return cherries-set([(x_label,x_label)]), retic_cherries-set([(x_label,x_label)])
+
+#     #Returns all reticulate cherries in the network where x_label is the second element of the pair
+#     def Find_Retic_Cherry_Second(self,x_label):
+#         pairs = set()
+#         x = self.labels[x_label]
+#         px=-1
+#         for p in self.nw.predecessors(x):
+#             px=p
+#         if self.nw.out_degree(px)>1:
+#             for cpx in self.nw.successors(px):
+#                 if self.nw.in_degree(cpx)>1:
+#                     for ccpx in self.nw.successors(cpx):
+#                         if ccpx in self.leaf_nodes:
+#                             pairs.add((self.leaf_nodes[ccpx],x_label))
+#         return pairs-set([(x_label,x_label)])
+
+#     #Returns all reducible pairs in the network
+#     # also sets this as value of self.reducible_pairs
+#     def Find_All_Reducible_Pairs(self):
+#         self.reducible_pairs=set()
+#         for l in self.leaves:
+#             self.reducible_pairs=self.reducible_pairs.union(self.Find_Pairs_With_First(l))
+#             self.reducible_pairs=self.reducible_pairs.union(self.Find_Pairs_With_Second(l))
+#         return self.reducible_pairs
+
+#     #Returns all cherries and reticulate cherries in the network
+#     # also sets these as values of self.cherries and self.reticulate_cherries
+#     def Find_All_Reducible_Pairs_Separated(self):
+#         self.reticulated_cherries=set()
+#         self.cherries=set()
+#         for l in self.leaves:
+#             added_cherries, added_retic_cherries = self.Find_Pairs_With_Second_Separated(l)
+#             self.cherries=self.reticulated_cherries.union(added_cherries)
+#             self.reticulated_cherries=self.reticulated_cherries.union(added_retic_cherries)
+#         return(self.cherries, self.reticulated_cherries)
```

### Comparing `phylox-0.0.1/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py` & `phylox-0.0.2/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,204 +1,200 @@
-import CPH
-import os
-import sys
-import csv
-
-errorInFile = False
-
-#####################################################################
-#####################################################################
-##############          Terminal arguments                ###########
-#####################################################################
-#####################################################################
-
-#Set default values
-option_out = False
-option_out_argument = ""
-option_file = False
-option_file_argument = ""
-option_progress = False
-option_bestTree = False
-option_repeats = False
-option_track = False
-option_repeats_argument = 1
-option_lengths = False
-option_timeLimit = False
-option_timeLimit_argument = None
-option_scoreSubnetwork = False
-option_scoreSubnetwork_argument = None
-option_reticsSubnetwork = False
-option_reticsSubnetwork_argument = None
-option_help = False
-
-#Read the arguments
-i = 1
-while i < len(sys.argv):
-    arg= sys.argv[i]
-    if arg == "-f" or arg == "--file":
-        option_file = True
-        i+=1
-        option_file_argument = sys.argv[i]
-        option_out_argument = option_file_argument+"OUT"
-    if arg == "-o" or arg == "--output":
-        option_out = True
-        i+=1
-        option_out_argument = sys.argv[i]
-    if arg == "-p" or arg == "--progress":
-        option_progress = True
-    if arg == "-t" or arg == "--track":
-        option_track = True
-    if arg == "-l" or arg == "--lengths":
-        option_lengths = True
-    if arg == "-r" or arg == "--repeats":
-        option_repeats = True
-        i+=1
-        option_repeats_argument = int(sys.argv[i])
-    if arg == "-rsn" or arg == "--reticssubnetwork":
-        option_reticsSubnetwork = True
-        i+=1
-        option_reticsSubnetwork_argument = int(sys.argv[i])
-    if arg == "-ssn" or arg == "--scoresubnetwork":
-        option_scoreSubnetwork = True
-        i+=1
-        option_scoreSubnetwork_argument = float(sys.argv[i])
-    if arg == "-tl" or arg == "--timelimit":
-        option_timeLimit = True
-        i+=1
-        option_timeLimit_argument = float(sys.argv[i])
-    if arg == "-bt" or arg == "--besttree":
-        option_bestTree = True
-    if arg == "-h" or arg == "--help":
-        option_help = True
-    i += 1
-
-#Output the help text to the terminal if no argument is given, or if the help option is chosen.
-if len(sys.argv)==1 or option_help:
-    print("Mandatory arguments:\n -f or --file followed by the input file in simple Newick format. \n\nOptional arguments:\n -o or --output followed by the output file containing the sequence, Default: [input_filename]+OUT\n -p or --progress for extra progress reports during the running of the algorithm\n -r or --repeats followed by an integer, the number of repeated attempts to find a good sequence.\n -tl or --timelimit followed by a float number of seconds, the timelimit given to the algorithm. The code will finish a repetition it is currently executing.\n -bt or --besttree for extracting the best tree out of the network, i.e. selecting the most used edges per reticulation node.\n -t or --track For tracking all reducible pairs during the algorithm.\n -l or --lengths For picking the lowest reducible cherry every time. If there are multiple, pick one at random.\n -rsn or --reticssubnetwork followed by an integer, the reticulation number of the subnetwork, to extract a subnetwork with this number of reticulations by iteratively adding reticulations with high probability (if probabilities are given) or by adding the reticulation edge that is used most by all input trees. \n -ssn or --scoresubnetwork followed by a threshold number (float) to extract a subnetwork by using all edges with a score above this threshold. If the network has probabilities, this score is the probability of an edge, otherwise it is the fraction of the input trees that uses this edge in their embedding.")
-    sys.exit()
-
-
-
-#####################################################################
-#####################################################################
-##############             Read the input                 ###########
-#####################################################################
-#####################################################################
-
-#Empty set of inputs
-inputs = []
-
-#Read each line of the input file with name set by "option_file_argument"
-f = open("./"+option_file_argument, "rt")
-reader = csv.reader(f, delimiter='~', quotechar='|')
-for row in reader:
-    inputs.append(str(row[0]))
-f.close()
-
-#Make the set of inputs usable for all algorithms: use the CPH class
-tree_set = CPH.Input_Set(newick_strings = inputs)
-
-
-
-
-#####################################################################
-#####################################################################
-##############            Find the sequence               ###########
-#####################################################################
-#####################################################################
-
-#Run the heuristic to find a cherry-pciking sequence `seq' for the set of input trees.
-#Arguments are set as given by the terminal arguments
-seq = tree_set.CPSBound(repeats = option_repeats_argument, 
-                    progress    = option_progress, 
-                    track       = option_track, 
-                    lengths     = option_lengths, 
-                    time_limit  = option_timeLimit_argument)
-
-
-
-#####################################################################
-#####################################################################
-##############                   Output                   ###########
-#####################################################################
-#####################################################################
-
-
-#Open the output file for writing
-f= open(option_out_argument,"w+")
-
-#Output the raw network.
-f.write("Best network in Newick format;\r\n")
-if option_lengths:
-    network = CPH.PhN(seq = tree_set.best_seq_with_lengths, 
-            reduced_trees = tree_set.best_seq_with_lengths_red_trees, 
-            heights       = tree_set.best_seq_with_lengths_heights)
-else:
-    network = CPH.PhN(seq = tree_set.best_seq, 
-            reduced_trees = tree_set.best_red_trees)
-#Cut the network into a tree to find the newick string
-cuttree = CPH.CutTree(network    = network.nw, 
-                    current_node = network.no_nodes, 
-                    leaf_labels  = network.leaf_nodes)
-f.write(cuttree.Newick(probabilities = True)+"\r\n")
-f.write(cuttree.Newick(probabilities = False)+"\r\n")
-
-#Output the desired subnetworks.
-f.write("Good subnetworks in Newick format;\r\n")
-#Find the best tree inside the network
-if option_bestTree:
-    resNW = network.SelectSubNetworkByReticulations(type_is_probability=True, reticulations = 0)
-    resNW.Clean_Up()
-    cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels  = resNW.leaf_nodes)
-    f.write(cuttree.Newick(probabilities = True)+"\r\n")
-    f.write(cuttree.Newick(probabilities = False)+"\r\n")
-#Find the best subnetwork with the given number of reticulations: option_reticsSubnetwork_argument from option -rsn
-if option_reticsSubnetwork:
-    #probabilities on edges
-    resNW = network.SelectSubNetworkByReticulations(type_is_probability=True, reticulations = option_reticsSubnetwork_argument)
-    cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels = resNW.leaf_nodes)
-    f.write(cuttree.Newick(probabilities = True)+"\r\n")
-    f.write(cuttree.Newick(probabilities = False)+"\r\n")
-    #no probabilities on edges
-    resNW = network.SelectSubNetworkByReticulations(type_is_probability=False, reticulations = option_reticsSubnetwork_argument)
-    cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels = resNW.leaf_nodes)
-    f.write(cuttree.Newick(probabilities = True)+"\r\n")
-    f.write(cuttree.Newick(probabilities = False)+"\r\n")
-#Find the best subnetwork with the given number of reticulations: option_reticsSubnetwork_argument from option -rsn
-if option_scoreSubnetwork:
-    #probabilities on edges
-    resNW = network.SelectSubNetworkByScore(type_is_probability=True, score = option_scoreSubnetwork_argument)
-    cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels = resNW.leaf_nodes)
-    f.write(cuttree.Newick(probabilities = True)+"\r\n")
-    f.write(cuttree.Newick(probabilities = False)+"\r\n")
-    #no probabilities on edges
-    resNW = network.SelectSubNetworkByScore(type_is_probability=False, score = option_scoreSubnetwork_argument)
-    cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels = resNW.leaf_nodes)
-    f.write(cuttree.Newick(probabilities = True)+"\r\n")
-    f.write(cuttree.Newick(probabilities = False)+"\r\n")
-
-
-#Output additional information about the given arguments
-f.write("END\r\n")
-f.write("Selected by score: \r\n")
-f.write(str(option_scoreSubnetwork_argument)+"\r\n")
-f.write("Selected by reticulation number: \r\n")
-f.write(str(option_reticsSubnetwork_argument)+"\r\n\r\n")
-
-#Output the computation time for the heuristic
-f.write("Computation time; CPS Heuristic reps\r\n")
-f.write(str(tree_set.CPS_Compute_Time) +";" + str(tree_set.CPS_Compute_Reps)+"\r\n\r\n")
-
-#Output the raw sequence found by the heuristic
-last = '0'
-f.write("Best sequence\r\n")
-f.write("Pair; reduced trees; (height of reduced pair)\r\n")
-for i, pair in enumerate(seq):
-    if option_lengths:
-        f.write("("+pair[0]+","+pair[1]+"); "+str(tree_set.best_seq_with_lengths_red_trees[i])+"); "+str(tree_set.best_seq_with_lengths_heights[i])+"\r\n")
-    else:
-        f.write("("+pair[0]+","+pair[1]+"); "+str(tree_set.best_red_trees[i])+"\r\n")
-    last = pair[1]
-f.write("("+last+",-)\r\n")
+# import CPH
+# import os
+# import sys
+# import csv
+
+# errorInFile = False
+
+# #####################################################################
+# #####################################################################
+# ##############          Terminal arguments                ###########
+# #####################################################################
+# #####################################################################
+
+# #Set default values
+# option_out = False
+# option_out_argument = ""
+# option_file = False
+# option_file_argument = ""
+# option_progress = False
+# option_bestTree = False
+# option_repeats = False
+# option_track = False
+# option_repeats_argument = 1
+# option_lengths = False
+# option_timeLimit = False
+# option_timeLimit_argument = None
+# option_scoreSubnetwork = False
+# option_scoreSubnetwork_argument = None
+# option_reticsSubnetwork = False
+# option_reticsSubnetwork_argument = None
+# option_help = False
+
+# #Read the arguments
+# i = 1
+# while i < len(sys.argv):
+#     arg= sys.argv[i]
+#     if arg == "-f" or arg == "--file":
+#         option_file = True
+#         i+=1
+#         option_file_argument = sys.argv[i]
+#         option_out_argument = option_file_argument+"OUT"
+#     if arg == "-o" or arg == "--output":
+#         option_out = True
+#         i+=1
+#         option_out_argument = sys.argv[i]
+#     if arg == "-p" or arg == "--progress":
+#         option_progress = True
+#     if arg == "-t" or arg == "--track":
+#         option_track = True
+#     if arg == "-l" or arg == "--lengths":
+#         option_lengths = True
+#     if arg == "-r" or arg == "--repeats":
+#         option_repeats = True
+#         i+=1
+#         option_repeats_argument = int(sys.argv[i])
+#     if arg == "-rsn" or arg == "--reticssubnetwork":
+#         option_reticsSubnetwork = True
+#         i+=1
+#         option_reticsSubnetwork_argument = int(sys.argv[i])
+#     if arg == "-ssn" or arg == "--scoresubnetwork":
+#         option_scoreSubnetwork = True
+#         i+=1
+#         option_scoreSubnetwork_argument = float(sys.argv[i])
+#     if arg == "-tl" or arg == "--timelimit":
+#         option_timeLimit = True
+#         i+=1
+#         option_timeLimit_argument = float(sys.argv[i])
+#     if arg == "-bt" or arg == "--besttree":
+#         option_bestTree = True
+#     if arg == "-h" or arg == "--help":
+#         option_help = True
+#     i += 1
+
+# #Output the help text to the terminal if no argument is given, or if the help option is chosen.
+# if len(sys.argv)==1 or option_help:
+#     print("Mandatory arguments:\n -f or --file followed by the input file in simple Newick format. \n\nOptional arguments:\n -o or --output followed by the output file containing the sequence, Default: [input_filename]+OUT\n -p or --progress for extra progress reports during the running of the algorithm\n -r or --repeats followed by an integer, the number of repeated attempts to find a good sequence.\n -tl or --timelimit followed by a float number of seconds, the timelimit given to the algorithm. The code will finish a repetition it is currently executing.\n -bt or --besttree for extracting the best tree out of the network, i.e. selecting the most used edges per reticulation node.\n -t or --track For tracking all reducible pairs during the algorithm.\n -l or --lengths For picking the lowest reducible cherry every time. If there are multiple, pick one at random.\n -rsn or --reticssubnetwork followed by an integer, the reticulation number of the subnetwork, to extract a subnetwork with this number of reticulations by iteratively adding reticulations with high probability (if probabilities are given) or by adding the reticulation edge that is used most by all input trees. \n -ssn or --scoresubnetwork followed by a threshold number (float) to extract a subnetwork by using all edges with a score above this threshold. If the network has probabilities, this score is the probability of an edge, otherwise it is the fraction of the input trees that uses this edge in their embedding.")
+#     sys.exit()
+
+
+# #####################################################################
+# #####################################################################
+# ##############             Read the input                 ###########
+# #####################################################################
+# #####################################################################
+
+# #Empty set of inputs
+# inputs = []
+
+# #Read each line of the input file with name set by "option_file_argument"
+# f = open("./"+option_file_argument, "rt")
+# reader = csv.reader(f, delimiter='~', quotechar='|')
+# for row in reader:
+#     inputs.append(str(row[0]))
+# f.close()
+
+# #Make the set of inputs usable for all algorithms: use the CPH class
+# tree_set = CPH.Input_Set(newick_strings = inputs)
+
+
+# #####################################################################
+# #####################################################################
+# ##############            Find the sequence               ###########
+# #####################################################################
+# #####################################################################
+
+# #Run the heuristic to find a cherry-pciking sequence `seq' for the set of input trees.
+# #Arguments are set as given by the terminal arguments
+# seq = tree_set.CPSBound(repeats = option_repeats_argument,
+#                     progress    = option_progress,
+#                     track       = option_track,
+#                     lengths     = option_lengths,
+#                     time_limit  = option_timeLimit_argument)
+
+
+# #####################################################################
+# #####################################################################
+# ##############                   Output                   ###########
+# #####################################################################
+# #####################################################################
+
+
+# #Open the output file for writing
+# f= open(option_out_argument,"w+")
+
+# #Output the raw network.
+# f.write("Best network in Newick format;\r\n")
+# if option_lengths:
+#     network = CPH.PhN(seq = tree_set.best_seq_with_lengths,
+#             reduced_trees = tree_set.best_seq_with_lengths_red_trees,
+#             heights       = tree_set.best_seq_with_lengths_heights)
+# else:
+#     network = CPH.PhN(seq = tree_set.best_seq,
+#             reduced_trees = tree_set.best_red_trees)
+# #Cut the network into a tree to find the newick string
+# cuttree = CPH.CutTree(network    = network.nw,
+#                     current_node = network.no_nodes,
+#                     leaf_labels  = network.leaf_nodes)
+# f.write(cuttree.Newick(probabilities = True)+"\r\n")
+# f.write(cuttree.Newick(probabilities = False)+"\r\n")
+
+# #Output the desired subnetworks.
+# f.write("Good subnetworks in Newick format;\r\n")
+# #Find the best tree inside the network
+# if option_bestTree:
+#     resNW = network.SelectSubNetworkByReticulations(type_is_probability=True, reticulations = 0)
+#     resNW.Clean_Up()
+#     cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels  = resNW.leaf_nodes)
+#     f.write(cuttree.Newick(probabilities = True)+"\r\n")
+#     f.write(cuttree.Newick(probabilities = False)+"\r\n")
+# #Find the best subnetwork with the given number of reticulations: option_reticsSubnetwork_argument from option -rsn
+# if option_reticsSubnetwork:
+#     #probabilities on edges
+#     resNW = network.SelectSubNetworkByReticulations(type_is_probability=True, reticulations = option_reticsSubnetwork_argument)
+#     cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels = resNW.leaf_nodes)
+#     f.write(cuttree.Newick(probabilities = True)+"\r\n")
+#     f.write(cuttree.Newick(probabilities = False)+"\r\n")
+#     #no probabilities on edges
+#     resNW = network.SelectSubNetworkByReticulations(type_is_probability=False, reticulations = option_reticsSubnetwork_argument)
+#     cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels = resNW.leaf_nodes)
+#     f.write(cuttree.Newick(probabilities = True)+"\r\n")
+#     f.write(cuttree.Newick(probabilities = False)+"\r\n")
+# #Find the best subnetwork with the given number of reticulations: option_reticsSubnetwork_argument from option -rsn
+# if option_scoreSubnetwork:
+#     #probabilities on edges
+#     resNW = network.SelectSubNetworkByScore(type_is_probability=True, score = option_scoreSubnetwork_argument)
+#     cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels = resNW.leaf_nodes)
+#     f.write(cuttree.Newick(probabilities = True)+"\r\n")
+#     f.write(cuttree.Newick(probabilities = False)+"\r\n")
+#     #no probabilities on edges
+#     resNW = network.SelectSubNetworkByScore(type_is_probability=False, score = option_scoreSubnetwork_argument)
+#     cuttree = CPH.CutTree(network = resNW.nw, current_node = resNW.no_nodes, leaf_labels = resNW.leaf_nodes)
+#     f.write(cuttree.Newick(probabilities = True)+"\r\n")
+#     f.write(cuttree.Newick(probabilities = False)+"\r\n")
+
+
+# #Output additional information about the given arguments
+# f.write("END\r\n")
+# f.write("Selected by score: \r\n")
+# f.write(str(option_scoreSubnetwork_argument)+"\r\n")
+# f.write("Selected by reticulation number: \r\n")
+# f.write(str(option_reticsSubnetwork_argument)+"\r\n\r\n")
+
+# #Output the computation time for the heuristic
+# f.write("Computation time; CPS Heuristic reps\r\n")
+# f.write(str(tree_set.CPS_Compute_Time) +";" + str(tree_set.CPS_Compute_Reps)+"\r\n\r\n")
+
+# #Output the raw sequence found by the heuristic
+# last = '0'
+# f.write("Best sequence\r\n")
+# f.write("Pair; reduced trees; (height of reduced pair)\r\n")
+# for i, pair in enumerate(seq):
+#     if option_lengths:
+#         f.write("("+pair[0]+","+pair[1]+"); "+str(tree_set.best_seq_with_lengths_red_trees[i])+"); "+str(tree_set.best_seq_with_lengths_heights[i])+"\r\n")
+#     else:
+#         f.write("("+pair[0]+","+pair[1]+"); "+str(tree_set.best_red_trees[i])+"\r\n")
+#     last = pair[1]
+# f.write("("+last+",-)\r\n")
 
-#close the output file
-f.close()
+# #close the output file
+# f.close()
```

### Comparing `phylox-0.0.1/src/phylox/cherrypicking/NetworkContainment.py` & `phylox-0.0.2/src/phylox/cherrypicking/NetworkContainment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,150 +1,178 @@
-import networkx as nx
-import ast
-import time
-import matplotlib.pyplot as plt
-import random
-import itertools
-
-random.seed(a=1234321)
-
-def find_cherry(N, x):
-    lst = list()
-    for p in N.predecessors(x):
-        if N.in_degree(p) == 1:
-            for pc in N.successors(p):
-                if pc != x:
-                    t = N.out_degree(pc)
-                    if t == 0:
-                        lst.append((pc, x))
-                    if t == 1:
-                        for pcc in N.successors(pc):
-                            if N.out_degree(pcc) == 0:
-                                lst.append((pcc,x))
-    return lst
-
-
-def find_ret_cherry(N, x):
-    lst = list()
-    for p in N.predecessors(x):
-        if N.out_degree(p) == 1:
-            for pp in N.predecessors(p):
-                for ppc in N.successors(pp):
-                    if ppc != p:
-                        if N.out_degree(ppc) == 0:
-                            lst.append((x, ppc))
-    return lst
-
-
-def check_cherry(N, x, y):
-    if N.has_node(x):
-        if N.has_node(y):
-            for px in N.predecessors(x):
-                for py in N.predecessors(y):
-                    if px == py:
-                        return 1
-                    if N.out_degree(px) == 1:
-                        if px in N.successors(py):
-                            return 2
-    return False
-
-
-def reduce_pair(N, x, y):
-    k = check_cherry(N, x, y)
-    if k == 1:
-        for px in N.predecessors(x):
-            N.remove_node(x)
-            for ppx in N.predecessors(px):
-                N.remove_node(px)
-                N.add_edge(ppx,y)
-            return True
-    if k == 2:
-        for px in N.predecessors(x):
-            for py in N.predecessors(y):
-                N.remove_edge(py,px)
-                if N.in_degree(px) == 1:
-                    for ppx in N.predecessors(px):
-                        N.add_edge(ppx, x)
-                        N.remove_node(px)
-                for ppy in N.predecessors(py):
-                    N.add_edge(ppy, y)
-                    N.remove_node(py)
-                return True
-    return False
-
-def find_tcs(N):
-    lst1 = list()
-    for x in N.nodes():
-        if N.out_degree(x) == 0:
-            cherry1 = find_cherry(N,x)
-            lst1.extend(cherry1)
-    lst2 = list()
-    while lst1:
-        cherry = lst1.pop()
-        k = check_cherry(N, *cherry)
-        if (k == 1) or (k == 2):
-            reduce_pair(N, *cherry)
-            lst2.append(cherry)
-            lst1.extend(find_cherry(N,cherry[1]))
-            lst1.extend(find_ret_cherry(N,cherry[1]))
-    return lst2
-
-
-def cps_reduces_network(N, lst):
-    for cherry in lst:
-        reduce_pair(N, *cherry)
-    if N.size() == 1:
-        return True
-    return False
-
-
-def tcn_contains(N, M):
-    return cps_reduces_network(M,find_tcs(N))
-
-
-def tester(foldername):
-    maxLeavesRetics = 1000
-    stepLeavesRetics = 25
-    reps = 4
-    folder_name = foldername
-    f = open("./" + folder_name + "/data.txt", "w+")
-    f.write("leaves;reticulations;reticulations_subnetwork;repetition;subnetwork;running_time\n")
-    f.close()
-    
-    allIndices = list(itertools.product(range(stepLeavesRetics, maxLeavesRetics+1,stepLeavesRetics),range(stepLeavesRetics, maxLeavesRetics+1,stepLeavesRetics),range(stepLeavesRetics, maxLeavesRetics+1,stepLeavesRetics),range(reps)))
-    print(list(allIndices)[0])
-    random.shuffle(allIndices)
-    print(list(allIndices)[0])
-    for i in allIndices:
-        if i[2]<=i[1]:
-            leaves,reticulations,reticulationsSubnetwork,rep = i
-            index1 = "0000000" + str(leaves)
-            index1 = index1[-4:]
-            index2 = "0000000" + str(reticulations)
-            index2 = index2[-4:]
-            index3 = "0000000" + str(reticulationsSubnetwork)
-            index3 = index3[-4:]
-            index = "n="+index1+"_k=" + index2+ "_kSub="+index3 + "_rep=" + str(rep)
-            name = index + ".txt"
- 
-            test = open("./" + folder_name+"/"+ name, "r")
-            line1 = test.read()
-            test.close()
-            line1 = line1.split("\n")
-            M = nx.DiGraph()
-            N = nx.DiGraph()
-            N.add_edges_from(ast.literal_eval(line1[0]))
-            M.add_edges_from(ast.literal_eval(line1[1]))
-
-            start = time.time()
-            contains = tcn_contains(N, M)
-            end = time.time()
-            runningTime = end-start;
-            f = open("./" + folder_name + "/data.txt", "a+")
-            f.write(index1 + " ; " + index2 + " ; " + index3 + " ; " + str(rep) + " ; " + str(contains) + " ; " + str(runningTime) + "\n")
-            f.close()
-
-
-#path of the folder with all input files
-foldername = "tests"
-#use network containment on all input files and store the data in data.txt in the same folder
-tester(foldername)
+import ast
+import itertools
+import random
+import time
+
+import networkx as nx
+
+import matplotlib.pyplot as plt
+
+random.seed(a=1234321)
+
+
+def find_cherry(N, x):
+    lst = list()
+    for p in N.predecessors(x):
+        if N.in_degree(p) == 1:
+            for pc in N.successors(p):
+                if pc != x:
+                    t = N.out_degree(pc)
+                    if t == 0:
+                        lst.append((pc, x))
+                    if t == 1:
+                        for pcc in N.successors(pc):
+                            if N.out_degree(pcc) == 0:
+                                lst.append((pcc, x))
+    return lst
+
+
+def find_ret_cherry(N, x):
+    lst = list()
+    for p in N.predecessors(x):
+        if N.out_degree(p) == 1:
+            for pp in N.predecessors(p):
+                for ppc in N.successors(pp):
+                    if ppc != p:
+                        if N.out_degree(ppc) == 0:
+                            lst.append((x, ppc))
+    return lst
+
+
+def check_cherry(N, x, y):
+    if N.has_node(x):
+        if N.has_node(y):
+            for px in N.predecessors(x):
+                for py in N.predecessors(y):
+                    if px == py:
+                        return 1
+                    if N.out_degree(px) == 1:
+                        if px in N.successors(py):
+                            return 2
+    return False
+
+
+def reduce_pair(N, x, y):
+    k = check_cherry(N, x, y)
+    if k == 1:
+        for px in N.predecessors(x):
+            N.remove_node(x)
+            for ppx in N.predecessors(px):
+                N.remove_node(px)
+                N.add_edge(ppx, y)
+            return True
+    if k == 2:
+        for px in N.predecessors(x):
+            for py in N.predecessors(y):
+                N.remove_edge(py, px)
+                if N.in_degree(px) == 1:
+                    for ppx in N.predecessors(px):
+                        N.add_edge(ppx, x)
+                        N.remove_node(px)
+                for ppy in N.predecessors(py):
+                    N.add_edge(ppy, y)
+                    N.remove_node(py)
+                return True
+    return False
+
+
+def find_tcs(N):
+    lst1 = list()
+    for x in N.nodes():
+        if N.out_degree(x) == 0:
+            cherry1 = find_cherry(N, x)
+            lst1.extend(cherry1)
+    lst2 = list()
+    while lst1:
+        cherry = lst1.pop()
+        k = check_cherry(N, *cherry)
+        if (k == 1) or (k == 2):
+            reduce_pair(N, *cherry)
+            lst2.append(cherry)
+            lst1.extend(find_cherry(N, cherry[1]))
+            lst1.extend(find_ret_cherry(N, cherry[1]))
+    return lst2
+
+
+def cps_reduces_network(N, lst):
+    for cherry in lst:
+        reduce_pair(N, *cherry)
+    if N.size() == 1:
+        return True
+    return False
+
+
+def tcn_contains(N, M):
+    return cps_reduces_network(M, find_tcs(N))
+
+
+def tester(foldername):
+    maxLeavesRetics = 1000
+    stepLeavesRetics = 25
+    reps = 4
+    folder_name = foldername
+    f = open("./" + folder_name + "/data.txt", "w+")
+    f.write(
+        "leaves;reticulations;reticulations_subnetwork;repetition;subnetwork;running_time\n"
+    )
+    f.close()
+
+    allIndices = list(
+        itertools.product(
+            range(stepLeavesRetics, maxLeavesRetics + 1, stepLeavesRetics),
+            range(stepLeavesRetics, maxLeavesRetics + 1, stepLeavesRetics),
+            range(stepLeavesRetics, maxLeavesRetics + 1, stepLeavesRetics),
+            range(reps),
+        )
+    )
+    print(list(allIndices)[0])
+    random.shuffle(allIndices)
+    print(list(allIndices)[0])
+    for i in allIndices:
+        if i[2] <= i[1]:
+            leaves, reticulations, reticulationsSubnetwork, rep = i
+            index1 = "0000000" + str(leaves)
+            index1 = index1[-4:]
+            index2 = "0000000" + str(reticulations)
+            index2 = index2[-4:]
+            index3 = "0000000" + str(reticulationsSubnetwork)
+            index3 = index3[-4:]
+            index = (
+                "n=" + index1 + "_k=" + index2 + "_kSub=" + index3 + "_rep=" + str(rep)
+            )
+            name = index + ".txt"
+
+            test = open("./" + folder_name + "/" + name, "r")
+            line1 = test.read()
+            test.close()
+            line1 = line1.split("\n")
+            M = nx.DiGraph()
+            N = nx.DiGraph()
+            N.add_edges_from(ast.literal_eval(line1[0]))
+            M.add_edges_from(ast.literal_eval(line1[1]))
+
+            start = time.time()
+            contains = tcn_contains(N, M)
+            end = time.time()
+            runningTime = end - start
+            f = open("./" + folder_name + "/data.txt", "a+")
+            f.write(
+                index1
+                + " ; "
+                + index2
+                + " ; "
+                + index3
+                + " ; "
+                + str(rep)
+                + " ; "
+                + str(contains)
+                + " ; "
+                + str(runningTime)
+                + "\n"
+            )
+            f.close()
+
+
+# path of the folder with all input files
+foldername = "tests"
+# use network containment on all input files and store the data in data.txt in the same folder
+tester(foldername)
```

### Comparing `phylox-0.0.1/src/phylox/cherrypicking/base.py` & `phylox-0.0.2/src/phylox/cherrypicking/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-from enum import Enum
 from copy import deepcopy
+from enum import Enum
+
 
 class CHERRYTYPE(Enum):
     CHERRY = 1
     RETICULATEDCHERRY = 2
     NONE = 0
 
+
 def is_second_in_reducible_pair(network, x):
     for node in network.predecessors(x):
         px = node
     for cpx in network.successors(px):
         if cpx != x:
-            if network.out_degree(cpx)==0:
-                return (cpx,x)
-            if network.out_degree(cpx)==1:
+            if network.out_degree(cpx) == 0:
+                return (cpx, x)
+            if network.out_degree(cpx) == 1:
                 for ccpx in network.successors(cpx):
-                    if network.out_degree(ccpx)==0:
-                        return (ccpx,x)
+                    if network.out_degree(ccpx) == 0:
+                        return (ccpx, x)
     return False
 
+
 def reduce_pair(network, x, y):
     network = deepcopy(network)
 
     cherry_type = check_cherry(network, x, y)
     if cherry_type == CHERRYTYPE.CHERRY:
         px = network.parent(x)
         network.remove_node(x)
         if network.out_degree(px) == 1:
             ppx = network.parent(px)
             network.remove_node(px)
-            network.add_edge(ppx,y)
+            network.add_edge(ppx, y)
     if cherry_type == CHERRYTYPE.RETICULATEDCHERRY:
         px = network.parent(x)
         py = network.parent(y)
-        network.remove_edge(py,px)
+        network.remove_edge(py, px)
         if network.in_degree(px) == 1:
             ppx = network.parent(px)
             network.add_edge(ppx, x)
             network.remove_node(px)
         if network.out_degree(py) == 1:
             ppy = network.parent(py)
             network.add_edge(ppy, y)
             network.remove_node(py)
     return network, cherry_type
 
+
 def check_cherry(network, x, y):
     if network.has_node(x):
         if network.has_node(y):
             for px in network.predecessors(x):
                 for py in network.predecessors(y):
                     if px == py:
                         return CHERRYTYPE.CHERRY
```

### Comparing `phylox-0.0.1/src/phylox/classes/dinetwork.py` & `phylox-0.0.2/src/phylox/classes/dinetwork.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from copy import deepcopy
-from phylox.cherrypicking import is_second_in_reducible_pair, reduce_pair, CHERRYTYPE
+
 import networkx as nx
 
+from phylox.cherrypicking import CHERRYTYPE, is_second_in_reducible_pair, reduce_pair
+
+
 def is_binary(network):
     binary_node_types = [
         [0, 1],  # root
         [0, 2],  # root
         [1, 2],  # tree node
         [2, 1],  # reticulation
         [1, 0],  # leaf
     ]
     for node in network.nodes:
         degrees = [network.in_degree(node), network.out_degree(node)]
         if degrees not in binary_node_types:
             return False
     return True
 
+
 def is_orchard(network):
     if len(network) == 0:
         return True
     leaves = network.leaves
     root = list(network.roots)[0]
 
     # make a copy and fix a root edge
@@ -34,30 +38,28 @@
     done = False
     while not done:
         checked_all_leaves = True
         for leaf in leaves:
             pair = is_second_in_reducible_pair(network_copy, leaf)
             if pair:
                 network_copy, cherry_type = reduce_pair(network_copy, *pair)
-                if cherry_type ==  CHERRYTYPE.CHERRY:
+                if cherry_type == CHERRYTYPE.CHERRY:
                     leaves.remove(pair[0])
                 checked_all_leaves = False
                 break
         if len(network_copy.edges) == 1:
             return True
         done = checked_all_leaves
     return False
 
+
 def is_stack_free(network):
     for node in network.nodes:
         if network.is_reticulation(node) and any(
-            [
-                network.is_reticulation(child)
-                for child in network.successors(node)
-            ]
+            [network.is_reticulation(child) for child in network.successors(node)]
         ):
             return False
     return True
 
 
 def is_endpoint_of_w_fence(network, node):
     if not network.is_reticulation(node):
@@ -78,34 +80,30 @@
             next_node = network.child(current_node, exclude=[previous_node])
         previous_node, current_node = current_node, next_node
         currently_at_fence_top = not currently_at_fence_top
 
 
 def is_tree_based(network):
     if not is_binary(network):
-        raise CannotComputeError(
+        raise NotImplementedError(
             "tree-basedness cannot be computed for non-binary networks yet."
         )
 
     if len(network) > 0 and not nx.is_weakly_connected(network):
         return False
 
     if len(network.roots) > 1:
         return False
 
     for node in network.nodes:
         if is_endpoint_of_w_fence(network, node):
             return False
     return True
 
+
 def is_tree_child(network):
     for node in network.nodes:
         if network.is_leaf(node):
             continue
-        if all(
-            [
-                network.is_reticulation(child)
-                for child in network.successors(node)
-            ]
-        ):
+        if all([network.is_reticulation(child) for child in network.successors(node)]):
             return False
     return True
```

### Comparing `phylox-0.0.1/src/phylox/dinetwork.py` & `phylox-0.0.2/src/phylox/dinetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import networkx as nx
 import random
 
+import networkx as nx
+
 LABEL_ATTR = "label"
 
+
 class DiNetwork(nx.DiGraph):
     def __init__(self, *args, **kwargs):
         edges = kwargs.get("edges", [])
         super().__init__(edges, *args, **kwargs)
         self.add_nodes_from(kwargs.get("nodes", []))
         for label in kwargs.get("labels", []):
             self.nodes[label[0]][LABEL_ATTR] = label[1]
@@ -30,15 +32,17 @@
         if not hasattr(self, "_roots"):
             self._set_roots()
         return self._roots
 
     @property
     def reticulation_number(self):
         if not hasattr(self, "_reticulation_number"):
-            self._reticulation_number = sum([max(self.in_degree(node) - 1, 0) for node in self.nodes])
+            self._reticulation_number = sum(
+                [max(self.in_degree(node) - 1, 0) for node in self.nodes]
+            )
         return self._reticulation_number
 
     def child(self, node, exclude=[], randomNodes=False):
         """
         Finds a child node of a node.
 
         :param node: a node of self.
@@ -81,8 +85,8 @@
     def is_leaf(self, node):
         return self.out_degree(node) == 0 and self.in_degree(node) > 0
 
     def is_root(self, node):
         return self.in_degree(node) == 0
 
     def is_tree_node(self, node):
-        return self.out_degree(node) > 1 and self.in_degree(node) <= 1
+        return self.out_degree(node) > 1 and self.in_degree(node) <= 1
```

### Comparing `phylox-0.0.1/src/phylox/generators/betasplitting/BetaSplittingModelTree.py` & `phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingModelTree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,146 @@
-############################################
-# Beta-splitting model (Aldous1996)
-#
-# To run this script, type in your terminal:
-# python3 BetaSplittingModel.py
-#
-# Parameters can be adjusted inside the code (line 74).
-#
-############################################
-
-import os
-import sys
-import math
-import random
-import numpy as np
-from scipy.special import gamma, loggamma
-import dendropy
-from pathlib import Path
-import multiprocessing
-from multiprocessing import Manager
-
-############################################
-# Simulation functions
-############################################
-
-# a_n is a normalizing constant defined in 
-# Equation (2) of Aldous1996 (so the sum of 
-# the values is equal to 1. It is not 
-# computed here to save time.
-def a_n(beta):
-	return 1
-
-# Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
-def computeProb(n,beta):
-	q_n = []
-	for i in range(1,n):
-		q_i_n = np.exp((loggamma(beta+i+1)+loggamma(beta+n-i+1))-((a_n(beta)+loggamma(i+1)+loggamma(n-i+1))))
-		q_n.append(q_i_n)
-	return q_n
-
-# n: number of tips
-def simulateBetaSplitting(n, beta):
-	# Initialize tree.
-	taxon_namespace = dendropy.TaxonNamespace(["N" + str(i) for i in range(1, 2*n)])
-	tree            = dendropy.Tree(taxon_namespace=taxon_namespace) # dendropy.Tree()
-	setattr(tree.seed_node, "n", n)
-	queue = [tree.seed_node]
-	# Insert one node at each iteration.
-	while queue:
-		node       = queue.pop(0)
-		node.taxon = taxon_namespace.get_taxon("N" + str(len(tree.nodes())))		
-		n          = node.n
-		# Internal node. Splits again.
-		if (n > 1): 
-			# Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
-			q_n   = computeProb(n,beta)
-			split = random.choices(population=list(range(1,n)), weights=q_n, k=1)[0]
-			# Create children.
-			ch1 = node.new_child(edge_length=1)
-			ch2 = node.new_child(edge_length=1)
-			setattr(ch1, "n", split)
-			setattr(ch2, "n", n-split)
-			# Add children to the queue.
-			queue.append(ch1)
-			queue.append(ch2)
-	# Return tree.
-	return tree
-
-############################################
-# MAIN
-############################################
-
-############################################
-# General parameters.
-
-# All desired tree sizes.
-tree_size_all   = [500,750,1000] # Trees with 500, 750, and 1000 tips respectively.
-# Number of simulated trees per tree size.
-nb_trees        = 10
-# Range of beta parameter.
-min_beta        = -2.0
-max_beta        = 10.0
-# Flag to indicate if files should overwrite possible existent files.
-saveifexists    = False
-# Number of cores in your computer (trees are simulated in parallel to save time).
-nb_threads      = 4
-
-############################################
-# Simulate trees
-
-# Each tree size
-for tree_size in tree_size_all:
-	sim_prefix =  "betaSplitting-tips" + str(tree_size)
-	if (not saveifexists) and any(sim_file.startswith(sim_prefix) for sim_file in os.listdir(".")):
-		print("WARNING! Skipping simulation (files already exists): tree_size=" + str(tree_size))
-	else:
-
-		# Method to simulate a single tree.
-		def runsubproc(pars):
-			# Simulate tree.
-			tree_size, beta = pars
-			tree            = simulateBetaSplitting(tree_size, beta)
-			infostr = str(tree_size) + "\t" + str(beta) + "\n"
-			treeStr = tree.as_string(schema="newick")
-			return (infostr, treeStr)
-
-		# Simulate trees.
-		current_points = 0
-		while (current_points < nb_trees):
-
-			# Uniform sample parameters (beta values).
-			print("Current number of points: " + str(current_points) + " / Desired: " + str(nb_trees))
-			points_i        = 0
-			beta_values_all = []
-			while points_i < (nb_trees-current_points):
-				beta = np.random.uniform(low=min_beta, high=max_beta)
-				beta_values_all.append(beta)
-				points_i += 1
-
-			# Simulate
-			all_sim   = [(tree_size, beta) for beta in beta_values_all]
-
-			print("  Run all simulations (" + str(len(all_sim)) +  ")...")
-			p = multiprocessing.Pool(nb_threads)
-			all_trees = p.map(runsubproc, all_sim)
-
-			filepath_trees = sim_prefix + ".nwk"
-			filepath_pars  = sim_prefix + ".tsv"
-
-			if os.path.exists(filepath_trees) and os.path.exists(filepath_pars):
-				append_write = 'a' # append if already exists
-			else:
-				append_write = 'w' # append if already exists
-			
-			with open(filepath_trees, append_write) as f:
-				for (infostr, treeStr) in all_trees:
-					if treeStr:
-						f.write(treeStr)
-						current_points += 1
-				print("\t Saved: '" + str(filepath_trees) + "'")
-
-			with open(filepath_pars, append_write) as f:
-				for (infostr, treeStr) in all_trees:
-					if treeStr:
-						f.write(infostr)
-				print("\t Saved: '" + str(filepath_pars) + "'")
-
+# ############################################
+# # Beta-splitting model (Aldous1996)
+# #
+# # To run this script, type in your terminal:
+# # python3 BetaSplittingModel.py
+# #
+# # Parameters can be adjusted inside the code (line 74).
+# #
+# ############################################
+
+# import os
+# import sys
+# import math
+# import random
+# import numpy as np
+# from scipy.special import gamma, loggamma
+# import dendropy
+# from pathlib import Path
+# import multiprocessing
+# from multiprocessing import Manager
+
+# ############################################
+# # Simulation functions
+# ############################################
+
+# # a_n is a normalizing constant defined in
+# # Equation (2) of Aldous1996 (so the sum of
+# # the values is equal to 1. It is not
+# # computed here to save time.
+# def a_n(beta):
+# 	return 1
+
+# # Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
+# def computeProb(n,beta):
+# 	q_n = []
+# 	for i in range(1,n):
+# 		q_i_n = np.exp((loggamma(beta+i+1)+loggamma(beta+n-i+1))-((a_n(beta)+loggamma(i+1)+loggamma(n-i+1))))
+# 		q_n.append(q_i_n)
+# 	return q_n
+
+# # n: number of tips
+# def simulateBetaSplitting(n, beta):
+# 	# Initialize tree.
+# 	taxon_namespace = dendropy.TaxonNamespace(["N" + str(i) for i in range(1, 2*n)])
+# 	tree            = dendropy.Tree(taxon_namespace=taxon_namespace) # dendropy.Tree()
+# 	setattr(tree.seed_node, "n", n)
+# 	queue = [tree.seed_node]
+# 	# Insert one node at each iteration.
+# 	while queue:
+# 		node       = queue.pop(0)
+# 		node.taxon = taxon_namespace.get_taxon("N" + str(len(tree.nodes())))
+# 		n          = node.n
+# 		# Internal node. Splits again.
+# 		if (n > 1):
+# 			# Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
+# 			q_n   = computeProb(n,beta)
+# 			split = random.choices(population=list(range(1,n)), weights=q_n, k=1)[0]
+# 			# Create children.
+# 			ch1 = node.new_child(edge_length=1)
+# 			ch2 = node.new_child(edge_length=1)
+# 			setattr(ch1, "n", split)
+# 			setattr(ch2, "n", n-split)
+# 			# Add children to the queue.
+# 			queue.append(ch1)
+# 			queue.append(ch2)
+# 	# Return tree.
+# 	return tree
+
+# ############################################
+# # MAIN
+# ############################################
+
+# ############################################
+# # General parameters.
+
+# # All desired tree sizes.
+# tree_size_all   = [500,750,1000] # Trees with 500, 750, and 1000 tips respectively.
+# # Number of simulated trees per tree size.
+# nb_trees        = 10
+# # Range of beta parameter.
+# min_beta        = -2.0
+# max_beta        = 10.0
+# # Flag to indicate if files should overwrite possible existent files.
+# saveifexists    = False
+# # Number of cores in your computer (trees are simulated in parallel to save time).
+# nb_threads      = 4
+
+# ############################################
+# # Simulate trees
+
+# # Each tree size
+# for tree_size in tree_size_all:
+# 	sim_prefix =  "betaSplitting-tips" + str(tree_size)
+# 	if (not saveifexists) and any(sim_file.startswith(sim_prefix) for sim_file in os.listdir(".")):
+# 		print("WARNING! Skipping simulation (files already exists): tree_size=" + str(tree_size))
+# 	else:
+
+# 		# Method to simulate a single tree.
+# 		def runsubproc(pars):
+# 			# Simulate tree.
+# 			tree_size, beta = pars
+# 			tree            = simulateBetaSplitting(tree_size, beta)
+# 			infostr = str(tree_size) + "\t" + str(beta) + "\n"
+# 			treeStr = tree.as_string(schema="newick")
+# 			return (infostr, treeStr)
+
+# 		# Simulate trees.
+# 		current_points = 0
+# 		while (current_points < nb_trees):
+
+# 			# Uniform sample parameters (beta values).
+# 			print("Current number of points: " + str(current_points) + " / Desired: " + str(nb_trees))
+# 			points_i        = 0
+# 			beta_values_all = []
+# 			while points_i < (nb_trees-current_points):
+# 				beta = np.random.uniform(low=min_beta, high=max_beta)
+# 				beta_values_all.append(beta)
+# 				points_i += 1
+
+# 			# Simulate
+# 			all_sim   = [(tree_size, beta) for beta in beta_values_all]
+
+# 			print("  Run all simulations (" + str(len(all_sim)) +  ")...")
+# 			p = multiprocessing.Pool(nb_threads)
+# 			all_trees = p.map(runsubproc, all_sim)
+
+# 			filepath_trees = sim_prefix + ".nwk"
+# 			filepath_pars  = sim_prefix + ".tsv"
+
+# 			if os.path.exists(filepath_trees) and os.path.exists(filepath_pars):
+# 				append_write = 'a' # append if already exists
+# 			else:
+# 				append_write = 'w' # append if already exists
+
+# 			with open(filepath_trees, append_write) as f:
+# 				for (infostr, treeStr) in all_trees:
+# 					if treeStr:
+# 						f.write(treeStr)
+# 						current_points += 1
+# 				print("\t Saved: '" + str(filepath_trees) + "'")
+
+# 			with open(filepath_pars, append_write) as f:
+# 				for (infostr, treeStr) in all_trees:
+# 					if treeStr:
+# 						f.write(infostr)
+# 				print("\t Saved: '" + str(filepath_pars) + "'")
```

### Comparing `phylox-0.0.1/src/phylox/generators/betasplitting/BetaSplittingNetwork_Main.py` & `phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingNetwork_Main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,74 @@
-############################################
-#
-# Adapted from BetasplittingModel.py
-# which contains the code for Beta-splitting model (Aldous1996)
-# Written for python3
-#
-############################################
-
-import os
-import sys
-import math
-import random
-import numpy as np
-import networkx as nx
-from scipy.special import gamma, loggamma
-from BetaSplittingNetwork_Tools import *
-
-
-
-############################################
-# I/O
-############################################
-    # General parameters and default values
-# All desired tree sizes.
-tree_size       = 100
-# Range of beta parameter.
-beta            = -0.0
-# Number of reticulations
-retics          = 10
-# Edge addition type; 
-#  default = None, in which case edges are added uniformly; 
-#  otherwise, float value gives the probability of stopping the random walk
-local           = None
-# output type: pl=parent list, el=edge list, nw=newick (not implemented)
-out_type        = "el"
-
-
-option_help = False
-i = 1
-while i < len(sys.argv):
-    arg= sys.argv[i]
-    if arg == "-n" or arg == "--number_of_tips":
-        i+=1
-        tree_size = int(sys.argv[i])
-    if arg == "-b" or arg == "--beta":
-        i+=1
-        beta = float(sys.argv[i])
-    if arg == "-r" or arg == "--reticulations":
-        i+=1
-        retics = int(sys.argv[i])
-    if arg == "-l" or arg == "--local":
-        i+=1
-        local = float(sys.argv[i])
-    if arg == "-pl" or arg == "--parent_list":
-        out_type = "pl"
-    if arg == "-el" or arg == "--edge_list":
-        out_type = "el"
-    if arg == "-h" or arg == "--help":
-        option_help = True
-    i += 1
-
-
-if option_help:
-    print("Generates a tree under the beta-splitting model (Aldous 1996) and then adds edges to generate a network. The edges are added one by one, by randomly choosing two edges in the network and attaching a new edge between them. The two edges can be randomly chosen in two ways: uniformly at random [Default]; or by chosing one edge uniformly at random and then performing a random walk to find a second edge. The second option has a parameter `stop_prob' that determines the length of the random walk: after each step of the walk, the walk stops with probability `stop_prob. Hence, the higher this parameter, the more local the extra reticulation edges become.\n\nOptional arguments:\n -n or --number_of_tips followed by an int [Default=100] to set the number of tips of the network.\n -b or --beta followed by a float [Default=0.0] to set the beta parameter of the tree generating beta-splitting model.\n -r or --reticulations followed by an int [Default=10] to set the number of reticulations (i.e., extra edges).\n -l or --local followed by a float to use the local edge adding method. The float is the stop probability for the random walk.\n -pl or --parent_list to get output as a parent list.\n -el or --edge_list to get output as an edge list.")
-    sys.exit()
-
-
-
-
-############################################
-# MAIN: Simulate network
-############################################
-
-
-
-tree = simulateBetaSplitting(tree_size, beta)
-network = GenerateNetwork(tree,retics,local)
-print(OutputNetwork(network,out_type))
-
+# ############################################
+# #
+# # Adapted from BetasplittingModel.py
+# # which contains the code for Beta-splitting model (Aldous1996)
+# # Written for python3
+# #
+# ############################################
+
+# import os
+# import sys
+# import math
+# import random
+# import numpy as np
+# import networkx as nx
+# from scipy.special import gamma, loggamma
+# from BetaSplittingNetwork_Tools import *
+
+
+# ############################################
+# # I/O
+# ############################################
+#     # General parameters and default values
+# # All desired tree sizes.
+# tree_size       = 100
+# # Range of beta parameter.
+# beta            = -0.0
+# # Number of reticulations
+# retics          = 10
+# # Edge addition type;
+# #  default = None, in which case edges are added uniformly;
+# #  otherwise, float value gives the probability of stopping the random walk
+# local           = None
+# # output type: pl=parent list, el=edge list, nw=newick (not implemented)
+# out_type        = "el"
+
+
+# option_help = False
+# i = 1
+# while i < len(sys.argv):
+#     arg= sys.argv[i]
+#     if arg == "-n" or arg == "--number_of_tips":
+#         i+=1
+#         tree_size = int(sys.argv[i])
+#     if arg == "-b" or arg == "--beta":
+#         i+=1
+#         beta = float(sys.argv[i])
+#     if arg == "-r" or arg == "--reticulations":
+#         i+=1
+#         retics = int(sys.argv[i])
+#     if arg == "-l" or arg == "--local":
+#         i+=1
+#         local = float(sys.argv[i])
+#     if arg == "-pl" or arg == "--parent_list":
+#         out_type = "pl"
+#     if arg == "-el" or arg == "--edge_list":
+#         out_type = "el"
+#     if arg == "-h" or arg == "--help":
+#         option_help = True
+#     i += 1
+
+
+# if option_help:
+#     print("Generates a tree under the beta-splitting model (Aldous 1996) and then adds edges to generate a network. The edges are added one by one, by randomly choosing two edges in the network and attaching a new edge between them. The two edges can be randomly chosen in two ways: uniformly at random [Default]; or by chosing one edge uniformly at random and then performing a random walk to find a second edge. The second option has a parameter `stop_prob' that determines the length of the random walk: after each step of the walk, the walk stops with probability `stop_prob. Hence, the higher this parameter, the more local the extra reticulation edges become.\n\nOptional arguments:\n -n or --number_of_tips followed by an int [Default=100] to set the number of tips of the network.\n -b or --beta followed by a float [Default=0.0] to set the beta parameter of the tree generating beta-splitting model.\n -r or --reticulations followed by an int [Default=10] to set the number of reticulations (i.e., extra edges).\n -l or --local followed by a float to use the local edge adding method. The float is the stop probability for the random walk.\n -pl or --parent_list to get output as a parent list.\n -el or --edge_list to get output as an edge list.")
+#     sys.exit()
+
+
+# ############################################
+# # MAIN: Simulate network
+# ############################################
+
+
+# tree = simulateBetaSplitting(tree_size, beta)
+# network = GenerateNetwork(tree,retics,local)
+# print(OutputNetwork(network,out_type))
```

### Comparing `phylox-0.0.1/src/phylox/generators/betasplitting/BetaSplittingNetwork_Tools.py` & `phylox-0.0.2/src/phylox/generators/betasplitting/BetaSplittingNetwork_Tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,188 +1,181 @@
-############################################
-#
-# Adapted from BetasplittingModel.py
-# which contains the code for Beta-splitting model (Aldous1996)
-# Written for python3
-#
-############################################
-
-import os
-import sys
-import math
-import random
-import numpy as np
-import networkx as nx
-from scipy.special import gamma, loggamma
-
-
-
-############################################
-# Simulation functions
-############################################
-
-# a_n is a normalizing constant defined in 
-# Equation (2) of Aldous1996 (so the sum of 
-# the values is equal to 1. It is not 
-# computed here to save time.
-def a_n(beta):
-    return 1
-
-# Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
-def computeProb(n,beta):
-    q_n = []
-    for i in range(1,n):
-        q_i_n = np.exp((loggamma(beta+i+1)+loggamma(beta+n-i+1))-((a_n(beta)+loggamma(i+1)+loggamma(n-i+1))))
-        q_n.append(q_i_n)
-    return q_n
-
-# n: number of tips
-def simulateBetaSplitting(n, beta):
-    # Initialize tree.
-    tree = nx.DiGraph()
-    tree.add_node(n+1)
-    tree.node[n+1]['label'] = n
-    last_internal_node       = n+1
-    last_leaf_node           = 0 
-    queue                    = [n+1]
-    # Insert one node at each iteration.
-    while queue:
-        node        = queue.pop()
-        n_node      = tree.node[node].get('label')
-        # Internal node. Splits again.
-        if (n_node > 1): 
-            # Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
-            q_n   = computeProb(n_node,beta)
-            split = random.choices(population=list(range(1,n_node)), weights=q_n, k=1)[0]
-            # Create children.
-            for new_n in [split,n_node-split]:
-                if new_n == 1:
-                    tree.add_edge(node,last_leaf_node+1)
-                    last_leaf_node+=1
-                else:
-                    tree.add_edge(node,last_internal_node+1)
-                    tree.node[last_internal_node+1]['label']=new_n
-                    queue.append(last_internal_node+1)
-                    last_internal_node+=1
-    # Return tree.
-    return tree
-
-
-def GenerateNetwork(tree,r,method):
-    network = tree.copy()
-    if method=="Horizontal":
-        leaves = [x for x in tree.nodes() if tree.out_degree(x)==0]
-    for i in range(r):
-        if method==None:
-            AddEdgeUniform(network)
-        elif method=="Horizontal":
-            AddEdgeHorizontal(network,leaves=leaves)
-        else:
-            AddEdgeLocal(network,stop_prob=method)
-    return network
-
-
-def AddEdgeBetween(network,edge1,edge2,new_nodes=None):
-    #if we dont have new nodes yet, determine new nodes
-    if new_nodes==None:
-        max_node = max(network.nodes())
-        new_nodes = (max_node+1,max_node+2)
-    #make sure edge2 is not above edge1
-    if nx.has_path(network,edge2[1],edge1[0]):
-        edge1,edge2=edge2,edge1
-    length1 = network[edge1[0]][edge1[1]].get('length')
-    prob1 = network[edge1[0]][edge1[1]].get('prob')    
-    length2 = network[edge2[0]][edge2[1]].get('length')
-    prob2 = network[edge2[0]][edge2[1]].get('prob')    
-    #add an edge from edge1 to edge2
-    network.remove_edges_from([edge1,edge2])
-    network.add_edges_from([(edge1[0],new_nodes[0]),(new_nodes[0],edge1[1]),(edge2[0],new_nodes[1]),(new_nodes[1],edge2[1]),(new_nodes[0],new_nodes[1])])
-    
-    #If the original network had lengths and probabilities, add these to the subdivided arcs as well.
-    if length1!=None:
-        l11 = random.random()*length1
-        l12 = length1-l11
-        network[edge1[0]][new_nodes[0]]['length']=l11
-        network[new_nodes[0]][edge1[1]]['length']=l12
-    if prob1!=None:
-        network[new_nodes[0]][edge1[1]]['prob']=prob1
-    if length2!=None:
-        l21 = random.random()*length2
-        l22 = length2-l21
-        network[edge2[0]][new_nodes[1]]['length']=l21
-        network[new_nodes[1]][edge2[1]]['length']=l22
-    if prob2!=None:
-        network[new_nodes[1]][edge2[1]]['prob']=prob2
-    #TODO: add probabilities and length to the other new arcs as well?
-
-    
-
-#Pick two edges uniformly at random and add an edge between these
-def AddEdgeHorizontal(network,leaves = None,new_nodes=None):
-    if leaves==None:
-        leaves = [x for x in network.nodes() if network.out_degree(x)==0]
-    leaf_indices = np.random.choice(range(len(leaves)),2,replace=False)
-    l0 = leaves[leaf_indices[0]]
-    l1 = leaves[leaf_indices[1]]
-    e0 = list(network.in_edges(l0))[0]
-    e1 = list(network.in_edges(l1))[0]
-    AddEdgeBetween(network,e0,e1,new_nodes=new_nodes)
-
-
-#Pick two edges uniformly at random and add an edge between these
-def AddEdgeUniform(network,new_nodes=None):
-    edges = list(network.edges())
-    edge_indices = np.random.choice(range(len(edges)),2,replace=False)
-    AddEdgeBetween(network,edges[edge_indices[0]],edges[edge_indices[1]],new_nodes=new_nodes)
-
-
-    
-    
-#Pick one edge, move a random number of edges through the network to find a second edge
-#Add and edge between the two edges.    
-def AddEdgeLocal(network,new_nodes=None,stop_prob=0.2,max_steps=None,max_tries=None):
-    try_number = 1
-    while max_tries==None or try_number<=max_tries:
-        #Pick a random edge
-        edge1 = random.choice(list(network.edges()))
-        edge2 = None
-        #Initiate the random walk, by choosing an orientation
-        previous_node = random.choice(edge1)
-        current_node  = edge1[0]
-        if current_node == previous_node:
-            current_node = edge1[1]
-        #Take a number of steps
-        step_number =1
-        while max_steps==None or step_number<=max_steps:
-            previous_node,current_node = current_node,random.choice(list(network.successors(current_node))+list(network.predecessors(current_node)))
-            if random.random()<stop_prob:
-                break
-            step_number+=1
-        #Set the new edge
-        edge2 = (previous_node,current_node)
-        if edge2 not in network.edges():
-            edge2 = (current_node,previous_node)
-        #Add an edge if possible, otherwise repeat the search
-        if edge1!=edge2:
-            break
-        try_number+=1
-    AddEdgeBetween(network,edge1,edge2,new_nodes=new_nodes)
-
-
-def OutputNetwork(network,out_type):
-    output = ""
-    if out_type=="el":
-        for i,e in enumerate(network.edges):
-            if i!=0:
-                output+="\r\n"
-            output += str(e[0])+" "+str(e[1])
-    elif out_type=="pl":
-        for i,v in enumerate(network.nodes):
-            if i!=0:
-                output+="\r\n"
-            output += str(v)
-            for p in network.predecessors(v):
-                output+=" "+str(p)
-    return output
-
-
-
+# ############################################
+# #
+# # Adapted from BetasplittingModel.py
+# # which contains the code for Beta-splitting model (Aldous1996)
+# # Written for python3
+# #
+# ############################################
+
+# import os
+# import sys
+# import math
+# import random
+# import numpy as np
+# import networkx as nx
+# from scipy.special import gamma, loggamma
+
+
+# ############################################
+# # Simulation functions
+# ############################################
+
+# # a_n is a normalizing constant defined in
+# # Equation (2) of Aldous1996 (so the sum of
+# # the values is equal to 1. It is not
+# # computed here to save time.
+# def a_n(beta):
+#     return 1
+
+# # Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
+# def computeProb(n,beta):
+#     q_n = []
+#     for i in range(1,n):
+#         q_i_n = np.exp((loggamma(beta+i+1)+loggamma(beta+n-i+1))-((a_n(beta)+loggamma(i+1)+loggamma(n-i+1))))
+#         q_n.append(q_i_n)
+#     return q_n
+
+# # n: number of tips
+# def simulateBetaSplitting(n, beta):
+#     # Initialize tree.
+#     tree = nx.DiGraph()
+#     tree.add_node(n+1)
+#     tree.node[n+1]['label'] = n
+#     last_internal_node       = n+1
+#     last_leaf_node           = 0
+#     queue                    = [n+1]
+#     # Insert one node at each iteration.
+#     while queue:
+#         node        = queue.pop()
+#         n_node      = tree.node[node].get('label')
+#         # Internal node. Splits again.
+#         if (n_node > 1):
+#             # Compute the "probability" to split n in (i|n-1), where i=1,..,n-1
+#             q_n   = computeProb(n_node,beta)
+#             split = random.choices(population=list(range(1,n_node)), weights=q_n, k=1)[0]
+#             # Create children.
+#             for new_n in [split,n_node-split]:
+#                 if new_n == 1:
+#                     tree.add_edge(node,last_leaf_node+1)
+#                     last_leaf_node+=1
+#                 else:
+#                     tree.add_edge(node,last_internal_node+1)
+#                     tree.node[last_internal_node+1]['label']=new_n
+#                     queue.append(last_internal_node+1)
+#                     last_internal_node+=1
+#     # Return tree.
+#     return tree
+
+
+# def GenerateNetwork(tree,r,method):
+#     network = tree.copy()
+#     if method=="Horizontal":
+#         leaves = [x for x in tree.nodes() if tree.out_degree(x)==0]
+#     for i in range(r):
+#         if method==None:
+#             AddEdgeUniform(network)
+#         elif method=="Horizontal":
+#             AddEdgeHorizontal(network,leaves=leaves)
+#         else:
+#             AddEdgeLocal(network,stop_prob=method)
+#     return network
+
+
+# def AddEdgeBetween(network,edge1,edge2,new_nodes=None):
+#     #if we dont have new nodes yet, determine new nodes
+#     if new_nodes==None:
+#         max_node = max(network.nodes())
+#         new_nodes = (max_node+1,max_node+2)
+#     #make sure edge2 is not above edge1
+#     if nx.has_path(network,edge2[1],edge1[0]):
+#         edge1,edge2=edge2,edge1
+#     length1 = network[edge1[0]][edge1[1]].get('length')
+#     prob1 = network[edge1[0]][edge1[1]].get('prob')
+#     length2 = network[edge2[0]][edge2[1]].get('length')
+#     prob2 = network[edge2[0]][edge2[1]].get('prob')
+#     #add an edge from edge1 to edge2
+#     network.remove_edges_from([edge1,edge2])
+#     network.add_edges_from([(edge1[0],new_nodes[0]),(new_nodes[0],edge1[1]),(edge2[0],new_nodes[1]),(new_nodes[1],edge2[1]),(new_nodes[0],new_nodes[1])])
+
+#     #If the original network had lengths and probabilities, add these to the subdivided arcs as well.
+#     if length1!=None:
+#         l11 = random.random()*length1
+#         l12 = length1-l11
+#         network[edge1[0]][new_nodes[0]]['length']=l11
+#         network[new_nodes[0]][edge1[1]]['length']=l12
+#     if prob1!=None:
+#         network[new_nodes[0]][edge1[1]]['prob']=prob1
+#     if length2!=None:
+#         l21 = random.random()*length2
+#         l22 = length2-l21
+#         network[edge2[0]][new_nodes[1]]['length']=l21
+#         network[new_nodes[1]][edge2[1]]['length']=l22
+#     if prob2!=None:
+#         network[new_nodes[1]][edge2[1]]['prob']=prob2
+#     #TODO: add probabilities and length to the other new arcs as well?
+
+
+# #Pick two edges uniformly at random and add an edge between these
+# def AddEdgeHorizontal(network,leaves = None,new_nodes=None):
+#     if leaves==None:
+#         leaves = [x for x in network.nodes() if network.out_degree(x)==0]
+#     leaf_indices = np.random.choice(range(len(leaves)),2,replace=False)
+#     l0 = leaves[leaf_indices[0]]
+#     l1 = leaves[leaf_indices[1]]
+#     e0 = list(network.in_edges(l0))[0]
+#     e1 = list(network.in_edges(l1))[0]
+#     AddEdgeBetween(network,e0,e1,new_nodes=new_nodes)
+
+
+# #Pick two edges uniformly at random and add an edge between these
+# def AddEdgeUniform(network,new_nodes=None):
+#     edges = list(network.edges())
+#     edge_indices = np.random.choice(range(len(edges)),2,replace=False)
+#     AddEdgeBetween(network,edges[edge_indices[0]],edges[edge_indices[1]],new_nodes=new_nodes)
+
+
+# #Pick one edge, move a random number of edges through the network to find a second edge
+# #Add and edge between the two edges.
+# def AddEdgeLocal(network,new_nodes=None,stop_prob=0.2,max_steps=None,max_tries=None):
+#     try_number = 1
+#     while max_tries==None or try_number<=max_tries:
+#         #Pick a random edge
+#         edge1 = random.choice(list(network.edges()))
+#         edge2 = None
+#         #Initiate the random walk, by choosing an orientation
+#         previous_node = random.choice(edge1)
+#         current_node  = edge1[0]
+#         if current_node == previous_node:
+#             current_node = edge1[1]
+#         #Take a number of steps
+#         step_number =1
+#         while max_steps==None or step_number<=max_steps:
+#             previous_node,current_node = current_node,random.choice(list(network.successors(current_node))+list(network.predecessors(current_node)))
+#             if random.random()<stop_prob:
+#                 break
+#             step_number+=1
+#         #Set the new edge
+#         edge2 = (previous_node,current_node)
+#         if edge2 not in network.edges():
+#             edge2 = (current_node,previous_node)
+#         #Add an edge if possible, otherwise repeat the search
+#         if edge1!=edge2:
+#             break
+#         try_number+=1
+#     AddEdgeBetween(network,edge1,edge2,new_nodes=new_nodes)
+
+
+# def OutputNetwork(network,out_type):
+#     output = ""
+#     if out_type=="el":
+#         for i,e in enumerate(network.edges):
+#             if i!=0:
+#                 output+="\r\n"
+#             output += str(e[0])+" "+str(e[1])
+#     elif out_type=="pl":
+#         for i,v in enumerate(network.nodes):
+#             if i!=0:
+#                 output+="\r\n"
+#             output += str(v)
+#             for p in network.predecessors(v):
+#                 output+=" "+str(p)
+#     return output
```

### Comparing `phylox-0.0.1/src/phylox/generators/betasplitting/MakeCatAndBalancedWithEdges.py` & `phylox-0.0.2/src/phylox/generators/betasplitting/MakeNetworksBeta.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,95 @@
-import os
-import sys
-import math
-import random
-import numpy as np
-import networkx as nx
-from pathlib import Path
-import multiprocessing
-from multiprocessing import Manager
-from BetaSplittingNetwork_Tools import *
-
-
-############################################
-# MAIN
-############################################
-
-############################################
-# General parameters.
-
-# Desired tree size.
-leaves          = [8,16,32]
-# Range of reticulations.
-reticulations   = [1,2,3,4,5,6,7,8,9,10,15,20,25,30,40,50,100,200,300,400,500,1000,2000,5000]
-# Edge adding methods.
-methods         = ["Horizontal"]#[None,0.01,0.02,0.10,0.20]
-# Number of networks per tree, reticulation number, and method.
-nb_networks     = 100
-
-# Folder 
-folder = "balanced_and_caterpillar/"
-
-############################################
-
-
-def Balanced_Tree(n):
-    tree = nx.DiGraph()
-    tree.add_nodes_from(range(1,n+1))
-    roots = list(range(1,n+1))
-    curr = n+1
-    while len(roots)>1:
-        while len(roots)>1:
-            r1 = roots.pop()
-            r2 = roots.pop()
-            tree.add_edges_from([(curr,r1),(curr,r2)])
-            curr+=1
-        roots = [x for x in tree.nodes() if tree.in_degree(x)==0]
-    return tree
-
-
-
-def Caterpillar_Tree(n):
-    tree = nx.DiGraph()
-    tree.add_node(n+1)
-    for i in range(1,n):
-        tree.add_edges_from([(n+i,i),(n+i,n+i+1)])
-    tree=nx.relabel_nodes(tree,{2*n:n})
-    return tree             
-
-# Set all parameters for network simulation.
-all_sim = []
-for retics in reticulations:
-    for method in methods:
-        for index in range(nb_networks):
-            all_sim+=[(retics,method,index)]
-
-for out_type in ["el","pl"]:
-    this_path = folder+out_type
-    if not os.path.exists(this_path):
-        os.makedirs(this_path) 
-    
-
-# Simulate networks
-for tree_type in ["balanced","caterpillar"]:
-    for n in leaves:
-        print(tree_type,n)
-        if tree_type =="balanced":
-            tree = Balanced_Tree(n)
-        else:
-            tree = Caterpillar_Tree(n)
-        tree_prefix = "/"+tree_type+"_"+str(n)
-        for out_type in ["el","pl"]:
-            this_path = folder+out_type+tree_prefix+"/0"
-            if not os.path.exists(this_path):
-                os.makedirs(this_path) 
-            f=open(this_path+"/1.txt", 'w')
-            f.write(OutputNetwork(tree,out_type))
-            f.close()    
-
-        
-        # Method to simulate a single network.
-        def runsubproc(pars):
-            # Simulate tree.
-            retics, method, index  = pars
-            network  = GenerateNetwork(tree,retics,method)
-            filepath_network  = "/"+str(retics)+"/"+str(method)
-            index_txt      = "/"+str(index+1)+".txt"
-            for out_type in ["el", "pl"]:
-                this_path = folder+out_type+tree_prefix+filepath_network
-                if not os.path.exists(this_path):
-                    os.makedirs(this_path) 
-                filename = this_path+index_txt
-                if not os.path.exists(filename):
-                    f=open(filename, 'w')
-                    f.write(OutputNetwork(network,out_type))
-                    f.close()    
-
-        #p = multiprocessing.Pool(nb_threads)
-        #p.map(runsubproc, all_sim)
-        for par in all_sim:
-            runsubproc(par)
-        
-
-
+# import os
+# import sys
+# import math
+# import random
+# import numpy as np
+# from pathlib import Path
+# import multiprocessing
+# from multiprocessing import Manager
+# from BetaSplittingNetwork_Tools import *
+
+
+# ############################################
+# # MAIN
+# ############################################
+
+# ############################################
+# # General parameters.
+
+# # Desired tree size.
+# leaves          = 10
+# # Number of simulated trees per tree size.
+# nb_trees        = 50
+# # Range of beta parameter.
+# betas           = [0.0,-0.5,-1.0,-1.5]
+# # Range of reticulations.
+# reticulations   = [6,7,8,9,10,11,12,13,14,15,16,17,18,19]#[1,2,3,4,5,10,20,50,100,200,500]
+# # Edge adding methods.
+# methods         = ["Horizontal",None,0.002,0.020,0.200]
+# # Number of networks per tree, reticulation number, and method.
+# nb_networks     = 10
+# # Number of cores in your computer (trees are simulated in parallel to save time).
+# nb_threads      = 4
+
+# # Folder
+# folder = "Beta_Splitting_Networks_"+str(leaves)+"/"
+
+# ############################################
+
+
+# # Set all parameters for network simulation.
+# all_sim = []
+# for retics in reticulations:
+#     for method in methods:
+#         for index in range(nb_networks):
+#             all_sim+=[(retics,method,index)]
+
+# for out_type in ["el","pl"]:
+#     this_path = folder+out_type
+#     if not os.path.exists(this_path):
+#         os.makedirs(this_path)
+
+
+# # Simulate networks
+# for b in betas:
+#     for t in range(nb_trees):
+#         print(b,t+1)
+#         #Check whether the tree exists:
+#         tree_prefix  = "/"+str(b)+"/"+str(t+1)
+#         tree_path = folder+"el"+tree_prefix+"/0/1.txt"
+#         if os.path.exists(tree_path):
+#             tree        = nx.read_edgelist(tree_path,create_using=nx.DiGraph())
+#             relabel_dict = {node: int(node) for node in tree.nodes}
+#             tree=nx.relabel_nodes(tree,relabel_dict)
+#         else:
+#             tree        = simulateBetaSplitting(leaves, b)
+#             for out_type in ["el","pl"]:
+#                 this_path = folder+out_type+tree_prefix+"/0"
+#                 if not os.path.exists(this_path):
+#                     os.makedirs(this_path)
+#                 f=open(this_path+"/1.txt", 'w')
+#                 f.write(OutputNetwork(tree,out_type))
+#                 f.close()
+
+
+#         # Method to simulate a single network.
+#         def runsubproc(pars):
+#             # Simulate tree.
+#             retics, method, index  = pars
+#             network                = GenerateNetwork(tree,retics,method)
+#             filepath_network  = "/"+str(retics)+"/"+str(method)
+#             index_txt      = "/"+str(index+1)+".txt"
+#             for out_type in ["el", "pl"]:
+#                 this_path = folder+out_type+tree_prefix+filepath_network
+#                 if not os.path.exists(this_path):
+#                     os.makedirs(this_path)
+#                 filename = this_path+index_txt
+#                 if not os.path.exists(filename):
+#                     f=open(filename, 'w')
+#                     f.write(OutputNetwork(network,out_type))
+#                     f.close()
+
+#         #p = multiprocessing.Pool(nb_threads)
+#         #p.map(runsubproc, all_sim)
+#         for par in all_sim:
+#             runsubproc(par)
```

### Comparing `phylox-0.0.1/src/phylox/generators/heath/heath.py` & `phylox-0.0.2/src/phylox/generators/heath/heath.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,668 +1,647 @@
-import numpy as np
-import math
-import scipy.stats
-import random
-import networkx as nx
-import sys
-import itertools
-
-
-
-
-#For each choice of reticulation arcs, calculate the distance between all pairs of taxa
-#Add up all these distances for each pair, weighed by the probability of this embedded tree
-#The hyb rates are e^(-hybridization_rate*sum_for_pair-offset) for each pair.
-#####
-#Updating distances between pairs can be done smartly: 
-#  for a speciation event, the distances simply increase by two times the time to speciation, and the new species copies the distances from its sister species
-#  for an extinction event, the distances simply increase by two times the time to speciation, and the distances to the extinct species are removed.
-#  for a HGT event, only the rates for the receiving taxon have to be updated. They can be computed from the distances to the receiving and the donating easily
-#  for a hyb event, all paths go via exactly one of the parent species, so we can use those distances again.
-def UpdateHybridizationRates():
-    return False
-    #This is done within the CalculateNetwork function
-    
-
-def GammaDistributionPDF(value,mean,shape):
-    scale = mean/shape
-    return scipy.stats.gamma.pdf(value,shape,0,scale)
-
-def CalculateNewRate(parent_rate,prior_mean,prior_shape,update_shape):
-    proposed_rate = parent_rate * random.gammavariate(update_shape, 1/update_shape)
-    if random.random()<GammaDistributionPDF(proposed_rate,prior_mean,prior_shape)/GammaDistributionPDF(parent_rate,prior_mean,prior_shape):
-        return proposed_rate
-    return parent_rate
-
-
-
-def CalculateAllNewRates(parent_rates, update_shape, 
-            speciation_rate_mean, speciation_rate_shape, 
-            ext_used, extinction_rate_mean, extinction_rate_shape,
-            hgt_used, hgt_rate_mean, hgt_rate_shape
-            ):
-    sp_rate = CalculateNewRate(parent_rates[0],speciation_rate_mean,speciation_rate_shape,update_shape)
-    ext_rate = 0
-    if ext_used:
-        ext_rate = CalculateNewRate(parent_rates[1],extinction_rate_mean,extinction_rate_shape,update_shape)
-    hgt_rate = 0
-    if hgt_used:
-        hgt_rate = CalculateNewRate(parent_rates[2],hgt_rate_mean,hgt_rate_shape,update_shape)
-    return (sp_rate,ext_rate,hgt_rate)
-
-def DistanceToRate(distance,        
-        hybridization_left_bound,
-        hybridization_right_bound,
-        hybridization_left_rate,
-        hybridization_right_rate    
-        ):
-    #TODO Update this rate function, make it more of a gradual switch?
-    if distance<=hybridization_left_bound:
-        return hybridization_left_rate
-    elif distance>=hybridization_right_bound:
-        return hybridization_right_rate
-    return hybridization_left_rate+(hybridization_right_rate-hybridization_left_rate)*(distance-hybridization_left_bound)/(hybridization_right_bound-hybridization_left_bound);
-
-
-def RestrictToLeafSet(network, leaves_to_keep, suppress_trivial_blobs = False):
-    #find leaves to remove
-    leaves_to_keep = set(leaves_to_keep)
-    remove_nodes = set()
-    for v in network.nodes():
-        if network.out_degree(v)==0 and v not in leaves_to_keep:
-            remove_nodes.add(v)
-    
-    #remove the sinks that we don't want to keep
-    while remove_nodes:
-        removed_node = remove_nodes.pop()
-        parents = list(network.predecessors(removed_node))
-        network.remove_node(removed_node)
-        for p in parents:
-            if network.out_degree(p)==0:
-                remove_nodes.add(p)
-        
-    #optionally: suppress biconnected components with indegree-1 and outdegree-1    
-    if suppress_trivial_blobs:
-        #TODO: write this function.
-        #What to do with the length of the resulting arc? the blob may have multiple paths, do we average?
-        print("suppressing trivial blobs is not implemented yet")
-    
-   
-    #suppress degree-2 nodes 
-    network = SuppressDegree2(network)
-    return network    
-
-
-def SuppressDegree2(network):
-    to_remove =[]    
-    to_check = set(list(network.nodes())[:])
-    while to_check:
-        v=to_check.pop()
-        if network.in_degree(v)==1 and network.out_degree(v)==1:
-            to_remove      +=[v]
-            parent          = list(network.predecessors(v))[0]
-            child           = list(network.successors(v))[0]
-            if network.has_edge(parent,child):
-                to_check.add(parent)
-                to_check.add(child)
-            in_edge_length  = network[parent][v]['length']
-            out_edge_length = network[v][child]['length']
-            out_edge_prob   = network[v][child].get('prob')
-            network.remove_edges_from([(parent,v),(v,child)])
-            network.add_weighted_edges_from([(parent,child,in_edge_length+out_edge_length)],weight = 'length')
-            if out_edge_prob!=None:
-                network[parent][child]['prob']=out_edge_prob
-    network.remove_nodes_from(to_remove)
-    return network
-    
-
-
-def CalculateNetwork(time_limit = 1.0,
-        taxa_limit = None,
-        update_shape = 2.0,
-        speciation_rate_mean  = 2.0,
-        speciation_rate_shape = 2.0,
-        ext_used = True,
-        count_extinct    = 0,
-        extinction_rate_mean  = 2.0,
-        extinction_rate_shape = 2.0,
-        hgt_used = False,
-        hgt_rate_mean   = None,
-        hgt_rate_shape  = None,
-        hgt_inheritance = 0.05,
-        hyb_used = False,
-        hybridization_left_bound  = None,
-        hybridization_right_bound = None,
-        hybridization_left_rate   = None,
-        hybridization_right_rate  = None,
-        simple_output = False             ):
-    #Initiate the network
-    nw = nx.DiGraph()
-    nw.add_node(0)
-    leaves = set([0])
-    current_node = 1
-    no_of_extinct = 0
-
-    #Set initial rates and distances
-    current_speciation_rate   = random.gammavariate(speciation_rate_shape, speciation_rate_mean/speciation_rate_shape)
-    current_extinction_rate   = 0.0
-    if ext_used:
-        current_extinction_rate   = random.gammavariate(extinction_rate_shape, extinction_rate_mean/extinction_rate_shape)
-    current_hgt_rate          = 0.0
-    if hgt_used:
-        current_hgt_rate      = random.gammavariate(hgt_rate_shape, hgt_rate_mean/hgt_rate_shape)
-    current_hybridization_rate = float(0)
-    #Force the first event to be a speciation
-    total_rate = current_speciation_rate
-    distances = dict()
-
-    #Set the initial leaf rates per leaf
-    leaf_rates = dict()
-    leaf_rates[0]=(current_speciation_rate,current_extinction_rate,current_hgt_rate)
-
-    #Pick a time for the first event
-    extra_time = np.random.exponential(1/float(total_rate))
-    current_time = extra_time
-
-    #####First create the network as a MUL-tree, to make it easier to convert to Newick (not currently implemented)
-    hybrid_nodes=dict()
-    no_of_hybrids = 0
-
-
-    while len(leaves)>0 and ((not taxa_limit and current_time<time_limit) or (taxa_limit and len(leaves)+count_extinct*no_of_extinct<taxa_limit)) :
-        random_number     = random.random()
-        splitting_leaf    = None
-        extinction_leaf   = None
-        hgt_donor_leaf    = None
-        parent_acceptor   = None
-        hgt_acceptor_leaf = None
-        hyb_pair          = None
-        if random_number < current_speciation_rate / total_rate:
-            ######################
-            #     Speciation     #
-            ######################
-            if not simple_output:
-                print("speciation")
-            random_number = random.random()*current_speciation_rate
-            for leaf,rates in leaf_rates.items():
-                if random_number < rates[0]:
-                    splitting_leaf = leaf
-                    break
-                random_number -= rates[0]
-            if splitting_leaf == None:
-                if not simple_output:
-                    print("ouch, speciation rate computed wrong")
-            nw.add_weighted_edges_from([(splitting_leaf,current_node,0),(splitting_leaf,current_node+1,0)], weight = 'length')
-            #Update the rates and distances
-            #rates
-            leaf_rates[current_node]=CalculateAllNewRates(leaf_rates[splitting_leaf],update_shape, 
-                speciation_rate_mean, speciation_rate_shape, 
-                ext_used, extinction_rate_mean, extinction_rate_shape,
-                hgt_used, hgt_rate_mean, hgt_rate_shape)
-            leaf_rates[current_node+1]=CalculateAllNewRates(leaf_rates[splitting_leaf],update_shape,
-                speciation_rate_mean, speciation_rate_shape, 
-                ext_used, extinction_rate_mean, extinction_rate_shape,
-                hgt_used, hgt_rate_mean, hgt_rate_shape)
-            current_speciation_rate += leaf_rates[current_node][0]+leaf_rates[current_node+1][0]-leaf_rates[splitting_leaf][0]
-            current_extinction_rate += leaf_rates[current_node][1]+leaf_rates[current_node+1][1]-leaf_rates[splitting_leaf][1]
-            current_hgt_rate        += leaf_rates[current_node][2]+leaf_rates[current_node+1][2]-leaf_rates[splitting_leaf][2]
-            #distances
-            if hyb_used:
-                for l in leaves:
-                    if l!=splitting_leaf:
-                        pair = (splitting_leaf,l)
-                        if pair in distances.keys():
-                            new_distance = distances[pair]
-                        else:
-                            pair = (l,splitting_leaf)
-                            new_distance = distances[pair]
-                        distances[(l,current_node)]=new_distance
-                        distances[(l,current_node+1)]=new_distance
-                        del distances[pair]
-                distances[(current_node,current_node+1)]=0
-
-            leaves.add(current_node)
-            leaves.add(current_node+1)
-            leaves.remove(splitting_leaf)            
-            del leaf_rates[splitting_leaf]
-            current_node+=2            
-
-
-        elif random_number < (current_extinction_rate + current_speciation_rate) / total_rate:
-            ######################
-            #     Extinction     #
-            ######################
-            if not simple_output:
-                print("extinction")
-
-            random_number = random.random()*current_extinction_rate
-            for leaf,rates in leaf_rates.items():
-                if random_number < rates[1]:
-                    extinction_leaf = leaf
-                    break
-                random_number -= rates[1]
-            if extinction_leaf == None:
-                if not simple_output:
-                    print("ouch, extinction rate computed wrong")
-            
-            #Update the rates and distances
-            #rates
-            current_speciation_rate -= leaf_rates[extinction_leaf][0]
-            current_extinction_rate -= leaf_rates[extinction_leaf][1]
-            current_hgt_rate        -= leaf_rates[extinction_leaf][2]
-            #distances
-            if hyb_used:
-                for l in leaves:
-                    if l!=extinction_leaf:
-                        if (extinction_leaf,l) in distances.keys():
-                            del distances[(extinction_leaf,l)] 
-                        else:
-                            del distances[(l,extinction_leaf)]
-                        
-            del leaf_rates[extinction_leaf]
-            leaves.remove(extinction_leaf)            
-            no_of_extinct+=1
-
-        elif random_number < (current_extinction_rate + current_speciation_rate + current_hgt_rate) / total_rate:
-            ######################
-            #      HGT event     #
-            ######################
-            if not simple_output:
-                print("HGT")
-            
-            random_number = random.random()*current_hgt_rate
-            for leaf,rates in leaf_rates.items():
-                if random_number < rates[2]:
-                    hgt_acceptor_leaf = leaf
-                    break
-                random_number -= rates[2]
-            if hgt_acceptor_leaf == None:
-                if not simple_output:
-                    print("ouch, hgt rate computed wrong")
-            if len(leaves)>1:
-                hgt_donor_leaf = random.sample(leaves-set([hgt_acceptor_leaf]),1)[0]
-                for p in nw.predecessors(hgt_acceptor_leaf):
-                    parent_acceptor=p
-                nw.add_weighted_edges_from([(hgt_donor_leaf,hgt_acceptor_leaf,0),(hgt_donor_leaf,current_node,0),(hgt_acceptor_leaf,current_node+1,0)], weight = 'length')
-                prob = hgt_inheritance*random.random()
-                nw[parent_acceptor][hgt_acceptor_leaf]['prob'] = 1-prob
-                nw[hgt_donor_leaf][hgt_acceptor_leaf]['prob'] = prob
-
-                hybrid_nodes[hgt_acceptor_leaf]=no_of_hybrids
-                no_of_hybrids+=1
-                #Update the rates and distances
-                #rates
-                leaf_rates[current_node+1]=CalculateAllNewRates(tuple(prob*x + (1-prob)*y for x, y in zip(leaf_rates[hgt_acceptor_leaf], leaf_rates[hgt_donor_leaf])),update_shape, 
-                    speciation_rate_mean, speciation_rate_shape, 
-                    ext_used, extinction_rate_mean, extinction_rate_shape,
-                    hgt_used, hgt_rate_mean, hgt_rate_shape)
-                leaf_rates[current_node]  =leaf_rates[hgt_donor_leaf]
-                current_speciation_rate += leaf_rates[current_node+1][0]-leaf_rates[hgt_acceptor_leaf][0]
-                current_extinction_rate += leaf_rates[current_node+1][1]-leaf_rates[hgt_acceptor_leaf][1]
-                current_hgt_rate        += leaf_rates[current_node+1][2]-leaf_rates[hgt_acceptor_leaf][2]        
-                del leaf_rates[hgt_donor_leaf]
-                del leaf_rates[hgt_acceptor_leaf]            
-                #distances
-                if hyb_used:
-                    for l in leaves:
-                        if l!=hgt_acceptor_leaf:
-                            acceptor_pair = (hgt_acceptor_leaf,l)
-                            if acceptor_pair in distances.keys():
-                                acceptor_distance = distances[acceptor_pair]
-                            else:
-                                acceptor_pair = (l,hgt_acceptor_leaf)
-                                acceptor_distance = distances[acceptor_pair]
-                            donor_pair = (l,hgt_donor_leaf)
-                            donor_distance = 0.0
-                            if l!=hgt_donor_leaf:
-                                if donor_pair in distances.keys():
-                                    donor_distance = distances[donor_pair]
-                                else:
-                                    donor_pair = (hgt_donor_leaf,l)
-                                    donor_distance = distances[donor_pair]
-                                distances[(l,current_node)]=donor_distance
-                                del distances[donor_pair]
-                            distances[(l,current_node+1)]=(1-prob)*acceptor_distance+prob*donor_distance
-                            del distances[acceptor_pair]
-                    distances[(current_node,current_node+1)]=distances[(hgt_donor_leaf,current_node+1)]
-                    del distances[(hgt_donor_leaf,current_node+1)]
-                leaves.remove(hgt_donor_leaf)
-                leaves.remove(hgt_acceptor_leaf)
-                leaves.add(current_node)
-                leaves.add(current_node+1)
-                current_node+=2
-
-    #        else:
-    #            print("trying HGT with only one leaf")
-    #             #Do nothing, there is only one leaf.    
-            
-                
-        else:
-            ######################
-            #    Hybridization   #
-            ######################
-            if not simple_output:
-                print("hybridization")
-        	#i.e.: pick two leaf nodes, create a hybrid between these two leaves
-            random_number = random.random()*current_hybridization_rate
-            for pair,distance in distances.items():
-        	    pair_rate = DistanceToRate(distance,        
-                    hybridization_left_bound,
-                    hybridization_right_bound,
-                    hybridization_left_rate,
-                    hybridization_right_rate)
-        	    if random_number<pair_rate:
-        	        hyb_pair = pair
-        	        break
-        	    random_number -=pair_rate
-            if hyb_pair == None and not simple_output:
-                if len(leaves)==1:
-                    print("ah, no leaves for hyb")
-                else:
-                    print("ouch, hybridization rate computed wrong")
-            nw.add_weighted_edges_from([(current_node,current_node+1,0),(hyb_pair[0],current_node,0),(hyb_pair[1],current_node,0),(hyb_pair[0],current_node+2,0),(hyb_pair[1],current_node+3,0)],weight = 'length')
-            prob = random.random()
-            nw[hyb_pair[0]][current_node]['prob'] = prob
-            nw[hyb_pair[1]][current_node]['prob'] = 1-prob
-            hybrid_nodes[current_node]=no_of_hybrids
-            no_of_hybrids+=1
-
-
-            #Update the rates and distances
-            #rates
-            leaf_rates[current_node+1]  =CalculateAllNewRates(tuple(prob*x + (1-prob)*y for x, y in zip(leaf_rates[hyb_pair[0]], leaf_rates[hyb_pair[1]])),update_shape, 
-                    speciation_rate_mean, speciation_rate_shape, 
-                    ext_used, extinction_rate_mean, extinction_rate_shape,
-                    hgt_used, hgt_rate_mean, hgt_rate_shape)
-            leaf_rates[current_node+2]  =leaf_rates[hyb_pair[0]]
-            leaf_rates[current_node+3]  =leaf_rates[hyb_pair[1]]
-            current_speciation_rate += leaf_rates[current_node+1][0]
-            current_extinction_rate += leaf_rates[current_node+1][1]
-            current_hgt_rate        += leaf_rates[current_node+1][2]
-            #distances
-            #TODO FIXED?!: The order may still be wrong. It seems I already delete some distances when I still need them later.
-            #These are probably the distances related to the hybrid parent species.
-            for l in leaves:
-                if l == hyb_pair[0]:
-                    pair_0_distance = 0
-                else:
-                    pair_0 = (hyb_pair[0],l)
-                    if pair_0 not in distances.keys():
-                        pair_0 = (l,hyb_pair[0])
-                    pair_0_distance = distances[pair_0]
-                    distances[(l,current_node+2)]=pair_0_distance
-    #                del distances[pair_0]
-                if l == hyb_pair[1]:
-                    pair_1_distance = 0
-                else:
-                    pair_1 = (hyb_pair[1],l)
-                    if pair_1 not in distances:
-                        pair_1 = (l,hyb_pair[1])
-                    pair_1_distance = distances[pair_1]
-                    distances[(l,current_node+3)]=pair_1_distance
-    #                del distances[pair_1]            
-                distances[(l,current_node+1)]=prob*pair_0_distance+(1-prob)*pair_1_distance
-                
-            if (hyb_pair[0],hyb_pair[1]) in distances:
-                distances[(current_node+2,current_node+3)]=distances[(hyb_pair[0],hyb_pair[1])]
-            else:
-                distances[(current_node+2,current_node+3)]=distances[(hyb_pair[1],hyb_pair[0])]
-            distances[(current_node+1,current_node+2)]=distances[(hyb_pair[0],current_node+1)]
-            distances[(current_node+1,current_node+3)]=distances[(hyb_pair[1],current_node+1)]
-
-
-            
-            remove_pairs = []
-            for pair in distances:
-                if hyb_pair[0] in pair or hyb_pair[1] in pair:
-                    remove_pairs +=[pair]
-            for pair in remove_pairs:
-                del distances[pair]
-
-            del leaf_rates[hyb_pair[0]]
-            del leaf_rates[hyb_pair[1]]
-            leaves.remove(hyb_pair[0])
-            leaves.remove(hyb_pair[1])
-            leaves.add(current_node+1)
-            leaves.add(current_node+2)
-            leaves.add(current_node+3)
-            current_node+=4 
-                
-                
-        
-        #Now extend all pendant edges of extant taxa
-        if len(leaves)==0:
-            break
-        for l in leaves:
-            pl = -1
-            for p in nw.predecessors(l):
-                pl = p
-            nw[pl][l]['length']+=extra_time
-            
-        #Compute the new rates
-        current_hybridization_rate = 0
-        if hyb_used:
-            for pair,distance in distances.items():
-                distances[pair]+=2*extra_time
-                current_hybridization_rate+=DistanceToRate(distances[pair],        
-                    hybridization_left_bound,
-                    hybridization_right_bound,
-                    hybridization_left_rate,
-                    hybridization_right_rate)
-        
-        total_rate = current_speciation_rate + current_extinction_rate + current_hgt_rate + current_hybridization_rate
-        
-        #Compute the time of the next event
-        extra_time    = np.random.exponential(1/total_rate)
-        current_time += extra_time
-
-    #The following corrects for overshooting the time limit
-    extra_time += time_limit-current_time
-    #nothing has happened yet, and there is only one node
-    if len(nw) == 1:
-        nw.add_weighted_edges_from([(0,1,time_limit)],weight = 'length')
-        leaves = set([1])
-    # each leaf has a parent node, and we can extend each parent edge to time_limit
-    else:
-        for l in leaves:
-            pl = -1
-            for p in nw.predecessors(l):
-                pl = p
-            nw[pl][l]['length']+=extra_time
-            
-    return nw,hybrid_nodes,leaves,no_of_extinct
-    
-
-
-######################## MAIN ########################
-
-
-
-import numpy as np
-import math
-import scipy.stats
-import random
-import networkx as nx
-import sys
-import itertools
-#from AddEdgesToTree import *
-from HeathNetwork_Tools import *
-
-##PARAMETERS
-edges = False
-only_extant = False
-
-params = {"time_limit"          : 1.0,
-    "taxa_limit"                : None,
-    "update_shape"              : 2.0,
-    "speciation_rate_mean"      : 2.0,
-    "speciation_rate_shape"     : 2.0,
-    "ext_used"                  : True,
-    "count_extinct"             : 0,
-    "extinction_rate_mean"      : 2.0,
-    "extinction_rate_shape"     : 2.0,
-    "hgt_used"                  : False,
-    "hgt_rate_mean"             : None,
-    "hgt_rate_shape"            : None,
-    "hgt_inheritance"           : 0.05,
-    "hyb_used"                  : False,
-    "hybridization_left_bound"  : None,
-    "hybridization_right_bound" : None,
-    "hybridization_left_rate"   : None,
-    "hybridization_right_rate"  : None,
-    "simple_output"             : False}
-##
-
-
-
-#random.gammavariate(alpha, beta)
-#shape and scale
-#On wiki,   alpha = k = `shape'   and    beta = theta = `scale'
-#Mean = alpha.beta
-#
-#Can also use numpy.random.gamma(shape, scale=1.0)
-
-############################### I/O ############################
-
-option_help = False
-i = 1
-while i < len(sys.argv):
-    arg= sys.argv[i]
-    if arg == "-ti" or arg == "--time":
-        i+=1
-        params["time_limit"] = float(sys.argv[i])
-    if arg == "-ta" or arg == "--taxa":
-        i+=1
-        params["taxa_limit"] = float(sys.argv[i])
-    if arg == "-ce" or arg == "--count_extinct":
-        params["count_extinct"] = 1
-    if arg == "-sp" or arg == "--speciation_parameters":
-        i+=1
-        params["speciation_rate_mean"] = float(sys.argv[i])
-        i+=1
-        speciation_rate_shape = float(sys.argv[i])  
-    if arg == "-noext" or arg == "--no_extinction":
-        params["ext_used"] = False  
-    if arg == "-oe" or arg == "--only_extant":
-        only_extant = True  
-    if arg == "-ext" or arg == "--extinction_parameters":
-        i+=1
-        params["extinction_rate_mean"] = float(sys.argv[i])
-        i+=1
-        params["extinction_rate_shape"] = float(sys.argv[i])    
-        if params["extinction_rate_mean"]==0:
-            params["ext_used"] = False
-    if arg == "-hgt" or arg == "--hgt_parameters":
-        i+=1
-        params["hgt_rate_mean"] = float(sys.argv[i])
-        i+=1
-        params["hgt_rate_shape"] = float(sys.argv[i])        
-        params["hgt_used"] = True
-    if arg == "-hyb" or arg == "--hybridization_factor":
-        i+=1
-        params["hybridization_left_bound"]  = float(sys.argv[i])
-        i+=1
-        params["hybridization_right_bound"] = float(sys.argv[i])
-        i+=1
-        params["hybridization_left_rate"]   = float(sys.argv[i])
-        i+=1
-        params["hybridization_right_rate"]  = float(sys.argv[i])
-        params["hyb_used"] = True
-    if arg == "-upd" or arg == "--update_shape_parameter":
-        i+=1
-        params["update_shape"] = float(sys.argv[i])
-    if arg == "-s" or arg == "--simple":
-        params["simple_output"] = True
-    if arg == "-h" or arg == "--help":
-        option_help = True
-    i += 1
-
-
-if option_help:
-    print("Runs a speciation-extinction-HGT-hybridization model for the given time (Default: ["+str(params["time_limit"])+"]) or until a certain number of extant taxa is reached. Each extant taxon has its own speciation, HGT, and extinction rates (1/mean_time_until_next_event). The hybridization rate of a pair of species is a function of the weighed distance between these species (sum of all up-down distances, weighed by their probability). There are prior speciation/extinction/HGT rate distributions, gamma distributions with a given mean and a shape parameter for speciation (Default: [mean="+str(params["speciation_rate_mean"])+", shape="+str(params["speciation_rate_shape"])+"]) and extinction (Default: [mean="+str(params["extinction_rate_mean"])+", shape="+str(params["extinction_rate_shape"])+"]), HGT is turned off. If a HGT event happens for a given taxon, another taxon (including itself) is chosen uniformly at random to donate genetic material (uniformly distributed contribution in [0,"+str(params["hgt_inheritance"])+"]). After speciation or hybridization, each rate of the new lineages is set by multiplying the (weighted mean) rate of the parent lineage(s) by a gamma-distributed factor with mean 1 and a shape parameter (Default: [shape="+str(params["update_shape"])+"]), and then accepting this rate with a probability proportional to the prior distribution for this rate. This gives an ultrametric network on the extant species. \n\nOptional arguments:\n -ti or --time followed by the total length (float) for the network.\n -ta or --taxa followed by the number of taxa at which the simulation stops. If all lineages go extinct before the given number of taxa is reached, another attempt is made.\n -ce or --count_extinct to also count the extinct taxa as part of the taxa limit.\n -oe or --only_extant to return the network restricted to the extant leaves.\n\nRates:\n -sp or --speciation_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the speciation rate.\n -ext or --extinction_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the extinction rate.\n -noext or --no_extinction to turn off extinction altogether.\n -hgt or --hgt_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the HGT rate.\n -upd or --update_shape_parameter followed by a shape parameter (float) for the update gamma distribution.\n -hyb or --hyb_factor followed by four floats for the piecewise linear dependence of hybridization rate on the distance:\n    left bound:  l\n    right bound: r\n    left rate:   rl\n    right rate:  rr.\n\n  |\nlr+---\n  |   \\\n  |    \\\n  |     \\\nrr+      -----\n  |\n 0+--+---+-----\n  0  l   r")
-    sys.exit()
-
-
-
-
-
-#Find a network
-if params["taxa_limit"]:
-    leaves = []
-    no_of_extinct = 0
-    while len(leaves)+params["count_extinct"]*no_of_extinct!=params["taxa_limit"]:
-        if not params["simple_output"]:
-            print("starting over")
-        network,hybrid_nodes,leaves,no_of_extinct = CalculateNetwork(**params)
-else:
-    print(params)
-    network,hybrid_nodes,leaves,no_of_extinct = CalculateNetwork(**params)
-
-#Restrict to extant leaves if wanted
-if only_extant:
-    network = RestrictToLeafSet(network,leaves)
-
-
-
-
-
-for e in network.edges:
-    info =""
-    if e[0] in hybrid_nodes:
-        info += "H"+str(hybrid_nodes[e[0]])
-    else:
-        info += str(e[0])
-    info += "  "
-    if e[1] in hybrid_nodes:
-        info += "H"+str(hybrid_nodes[e[1]])
-    else:
-        info += str(e[1])
-    print(info)#,network[e[0]][e[1]]['length']) 
-
-
-
-
-
-
-
-
-#### To use: argparse version:
-
-import argparse
-import sys
-
-parser = argparse.ArgumentParser(description="Runs a speciation-extinction-HGT-hybridization model.")
-
-parser.add_argument("-ti", "--time", dest="time_limit", type=float, help="Total length for the network")
-parser.add_argument("-ta", "--taxa", dest="taxa_limit", type=float, help="Number of taxa at which the simulation stops")
-parser.add_argument("-ce", "--count_extinct", action="store_true", help="Count extinct taxa as part of the taxa limit")
-parser.add_argument("-sp", "--speciation_parameters", nargs=2, type=float, metavar=("mean", "shape"), help="Mean and shape parameter for the gamma distribution of the speciation rate")
-parser.add_argument("-ext", "--extinction_parameters", nargs=2, type=float, metavar=("mean", "shape"), help="Mean and shape parameter for the gamma distribution of the extinction rate")
-parser.add_argument("-noext", "--no_extinction", action="store_true", help="Turn off extinction altogether")
-parser.add_argument("-hgt", "--hgt_parameters", nargs=2, type=float, metavar=("mean", "shape"), help="Mean and shape parameter for the gamma distribution of the HGT rate")
-parser.add_argument("-hyb", "--hybridization_factor", nargs=4, type=float, metavar=("l", "r", "rl", "rr"), help="Piecewise linear dependence of hybridization rate on the distance")
-parser.add_argument("-upd", "--update_shape_parameter", type=float, help="Shape parameter for the update gamma distribution")
-parser.add_argument("-s", "--simple", action="store_true", help="Enable simple output")
-parser.add_argument("-h", "--help", action="store_true", help="Show help message")
-
-args = parser.parse_args()
-
-params = {
-    "time_limit": args.time_limit,
-    "taxa_limit": args.taxa_limit,
-    "count_extinct": args.count_extinct,
-    "speciation_rate_mean": args.speciation_parameters[0] if args.speciation_parameters else None,
-    "speciation_rate_shape": args.speciation_parameters[1] if args.speciation_parameters else None,
-    "extinction_rate_mean": args.extinction_parameters[0] if args.extinction_parameters else None,
-    "extinction_rate_shape": args.extinction_parameters[1] if args.extinction_parameters else None,
-    "ext_used": not args.no_extinction,
-    "hgt_rate_mean": args.hgt_parameters[0] if args.hgt_parameters else None,
-    "hgt_rate_shape": args.hgt_parameters[1] if args.hgt_parameters else None,
-    "hgt_used": args.hgt_parameters is not None,
-    "hybridization_left_bound": args.hybridization_factor[0] if args.hybridization_factor else None,
-    "hybridization_right_bound": args.hybridization_factor[1] if args.hybridization_factor else None,
-    "hybridization_left_rate": args.hybridization_factor[2] if args.hybridization_factor else None,
-    "hybridization_right_rate": args.hybridization_factor[3] if args.hybridization_factor else None,
-    "hyb_used": args.hybridization_factor is not None,
-    "update_shape": args.update_shape_parameter,
-    "simple_output": args.simple
-}
+# import numpy as np
+# import math
+# import scipy.stats
+# import random
+# import networkx as nx
+# import sys
+# import itertools
+
+
+# #For each choice of reticulation arcs, calculate the distance between all pairs of taxa
+# #Add up all these distances for each pair, weighed by the probability of this embedded tree
+# #The hyb rates are e^(-hybridization_rate*sum_for_pair-offset) for each pair.
+# #####
+# #Updating distances between pairs can be done smartly:
+# #  for a speciation event, the distances simply increase by two times the time to speciation, and the new species copies the distances from its sister species
+# #  for an extinction event, the distances simply increase by two times the time to speciation, and the distances to the extinct species are removed.
+# #  for a HGT event, only the rates for the receiving taxon have to be updated. They can be computed from the distances to the receiving and the donating easily
+# #  for a hyb event, all paths go via exactly one of the parent species, so we can use those distances again.
+# def UpdateHybridizationRates():
+#     return False
+#     #This is done within the CalculateNetwork function
+
+
+# def GammaDistributionPDF(value,mean,shape):
+#     scale = mean/shape
+#     return scipy.stats.gamma.pdf(value,shape,0,scale)
+
+# def CalculateNewRate(parent_rate,prior_mean,prior_shape,update_shape):
+#     proposed_rate = parent_rate * random.gammavariate(update_shape, 1/update_shape)
+#     if random.random()<GammaDistributionPDF(proposed_rate,prior_mean,prior_shape)/GammaDistributionPDF(parent_rate,prior_mean,prior_shape):
+#         return proposed_rate
+#     return parent_rate
+
+
+# def CalculateAllNewRates(parent_rates, update_shape,
+#             speciation_rate_mean, speciation_rate_shape,
+#             ext_used, extinction_rate_mean, extinction_rate_shape,
+#             hgt_used, hgt_rate_mean, hgt_rate_shape
+#             ):
+#     sp_rate = CalculateNewRate(parent_rates[0],speciation_rate_mean,speciation_rate_shape,update_shape)
+#     ext_rate = 0
+#     if ext_used:
+#         ext_rate = CalculateNewRate(parent_rates[1],extinction_rate_mean,extinction_rate_shape,update_shape)
+#     hgt_rate = 0
+#     if hgt_used:
+#         hgt_rate = CalculateNewRate(parent_rates[2],hgt_rate_mean,hgt_rate_shape,update_shape)
+#     return (sp_rate,ext_rate,hgt_rate)
+
+# def DistanceToRate(distance,
+#         hybridization_left_bound,
+#         hybridization_right_bound,
+#         hybridization_left_rate,
+#         hybridization_right_rate
+#         ):
+#     #TODO Update this rate function, make it more of a gradual switch?
+#     if distance<=hybridization_left_bound:
+#         return hybridization_left_rate
+#     elif distance>=hybridization_right_bound:
+#         return hybridization_right_rate
+#     return hybridization_left_rate+(hybridization_right_rate-hybridization_left_rate)*(distance-hybridization_left_bound)/(hybridization_right_bound-hybridization_left_bound);
+
+
+# def RestrictToLeafSet(network, leaves_to_keep, suppress_trivial_blobs = False):
+#     #find leaves to remove
+#     leaves_to_keep = set(leaves_to_keep)
+#     remove_nodes = set()
+#     for v in network.nodes():
+#         if network.out_degree(v)==0 and v not in leaves_to_keep:
+#             remove_nodes.add(v)
+
+#     #remove the sinks that we don't want to keep
+#     while remove_nodes:
+#         removed_node = remove_nodes.pop()
+#         parents = list(network.predecessors(removed_node))
+#         network.remove_node(removed_node)
+#         for p in parents:
+#             if network.out_degree(p)==0:
+#                 remove_nodes.add(p)
+
+#     #optionally: suppress biconnected components with indegree-1 and outdegree-1
+#     if suppress_trivial_blobs:
+#         #TODO: write this function.
+#         #What to do with the length of the resulting arc? the blob may have multiple paths, do we average?
+#         print("suppressing trivial blobs is not implemented yet")
+
+
+#     #suppress degree-2 nodes
+#     network = SuppressDegree2(network)
+#     return network
+
+
+# def SuppressDegree2(network):
+#     to_remove =[]
+#     to_check = set(list(network.nodes())[:])
+#     while to_check:
+#         v=to_check.pop()
+#         if network.in_degree(v)==1 and network.out_degree(v)==1:
+#             to_remove      +=[v]
+#             parent          = list(network.predecessors(v))[0]
+#             child           = list(network.successors(v))[0]
+#             if network.has_edge(parent,child):
+#                 to_check.add(parent)
+#                 to_check.add(child)
+#             in_edge_length  = network[parent][v]['length']
+#             out_edge_length = network[v][child]['length']
+#             out_edge_prob   = network[v][child].get('prob')
+#             network.remove_edges_from([(parent,v),(v,child)])
+#             network.add_weighted_edges_from([(parent,child,in_edge_length+out_edge_length)],weight = 'length')
+#             if out_edge_prob!=None:
+#                 network[parent][child]['prob']=out_edge_prob
+#     network.remove_nodes_from(to_remove)
+#     return network
+
+
+# def CalculateNetwork(time_limit = 1.0,
+#         taxa_limit = None,
+#         update_shape = 2.0,
+#         speciation_rate_mean  = 2.0,
+#         speciation_rate_shape = 2.0,
+#         ext_used = True,
+#         count_extinct    = 0,
+#         extinction_rate_mean  = 2.0,
+#         extinction_rate_shape = 2.0,
+#         hgt_used = False,
+#         hgt_rate_mean   = None,
+#         hgt_rate_shape  = None,
+#         hgt_inheritance = 0.05,
+#         hyb_used = False,
+#         hybridization_left_bound  = None,
+#         hybridization_right_bound = None,
+#         hybridization_left_rate   = None,
+#         hybridization_right_rate  = None,
+#         simple_output = False             ):
+#     #Initiate the network
+#     nw = nx.DiGraph()
+#     nw.add_node(0)
+#     leaves = set([0])
+#     current_node = 1
+#     no_of_extinct = 0
+
+#     #Set initial rates and distances
+#     current_speciation_rate   = random.gammavariate(speciation_rate_shape, speciation_rate_mean/speciation_rate_shape)
+#     current_extinction_rate   = 0.0
+#     if ext_used:
+#         current_extinction_rate   = random.gammavariate(extinction_rate_shape, extinction_rate_mean/extinction_rate_shape)
+#     current_hgt_rate          = 0.0
+#     if hgt_used:
+#         current_hgt_rate      = random.gammavariate(hgt_rate_shape, hgt_rate_mean/hgt_rate_shape)
+#     current_hybridization_rate = float(0)
+#     #Force the first event to be a speciation
+#     total_rate = current_speciation_rate
+#     distances = dict()
+
+#     #Set the initial leaf rates per leaf
+#     leaf_rates = dict()
+#     leaf_rates[0]=(current_speciation_rate,current_extinction_rate,current_hgt_rate)
+
+#     #Pick a time for the first event
+#     extra_time = np.random.exponential(1/float(total_rate))
+#     current_time = extra_time
+
+#     #####First create the network as a MUL-tree, to make it easier to convert to Newick (not currently implemented)
+#     hybrid_nodes=dict()
+#     no_of_hybrids = 0
+
+
+#     while len(leaves)>0 and ((not taxa_limit and current_time<time_limit) or (taxa_limit and len(leaves)+count_extinct*no_of_extinct<taxa_limit)) :
+#         random_number     = random.random()
+#         splitting_leaf    = None
+#         extinction_leaf   = None
+#         hgt_donor_leaf    = None
+#         parent_acceptor   = None
+#         hgt_acceptor_leaf = None
+#         hyb_pair          = None
+#         if random_number < current_speciation_rate / total_rate:
+#             ######################
+#             #     Speciation     #
+#             ######################
+#             if not simple_output:
+#                 print("speciation")
+#             random_number = random.random()*current_speciation_rate
+#             for leaf,rates in leaf_rates.items():
+#                 if random_number < rates[0]:
+#                     splitting_leaf = leaf
+#                     break
+#                 random_number -= rates[0]
+#             if splitting_leaf == None:
+#                 if not simple_output:
+#                     print("ouch, speciation rate computed wrong")
+#             nw.add_weighted_edges_from([(splitting_leaf,current_node,0),(splitting_leaf,current_node+1,0)], weight = 'length')
+#             #Update the rates and distances
+#             #rates
+#             leaf_rates[current_node]=CalculateAllNewRates(leaf_rates[splitting_leaf],update_shape,
+#                 speciation_rate_mean, speciation_rate_shape,
+#                 ext_used, extinction_rate_mean, extinction_rate_shape,
+#                 hgt_used, hgt_rate_mean, hgt_rate_shape)
+#             leaf_rates[current_node+1]=CalculateAllNewRates(leaf_rates[splitting_leaf],update_shape,
+#                 speciation_rate_mean, speciation_rate_shape,
+#                 ext_used, extinction_rate_mean, extinction_rate_shape,
+#                 hgt_used, hgt_rate_mean, hgt_rate_shape)
+#             current_speciation_rate += leaf_rates[current_node][0]+leaf_rates[current_node+1][0]-leaf_rates[splitting_leaf][0]
+#             current_extinction_rate += leaf_rates[current_node][1]+leaf_rates[current_node+1][1]-leaf_rates[splitting_leaf][1]
+#             current_hgt_rate        += leaf_rates[current_node][2]+leaf_rates[current_node+1][2]-leaf_rates[splitting_leaf][2]
+#             #distances
+#             if hyb_used:
+#                 for l in leaves:
+#                     if l!=splitting_leaf:
+#                         pair = (splitting_leaf,l)
+#                         if pair in distances.keys():
+#                             new_distance = distances[pair]
+#                         else:
+#                             pair = (l,splitting_leaf)
+#                             new_distance = distances[pair]
+#                         distances[(l,current_node)]=new_distance
+#                         distances[(l,current_node+1)]=new_distance
+#                         del distances[pair]
+#                 distances[(current_node,current_node+1)]=0
+
+#             leaves.add(current_node)
+#             leaves.add(current_node+1)
+#             leaves.remove(splitting_leaf)
+#             del leaf_rates[splitting_leaf]
+#             current_node+=2
+
+
+#         elif random_number < (current_extinction_rate + current_speciation_rate) / total_rate:
+#             ######################
+#             #     Extinction     #
+#             ######################
+#             if not simple_output:
+#                 print("extinction")
+
+#             random_number = random.random()*current_extinction_rate
+#             for leaf,rates in leaf_rates.items():
+#                 if random_number < rates[1]:
+#                     extinction_leaf = leaf
+#                     break
+#                 random_number -= rates[1]
+#             if extinction_leaf == None:
+#                 if not simple_output:
+#                     print("ouch, extinction rate computed wrong")
+
+#             #Update the rates and distances
+#             #rates
+#             current_speciation_rate -= leaf_rates[extinction_leaf][0]
+#             current_extinction_rate -= leaf_rates[extinction_leaf][1]
+#             current_hgt_rate        -= leaf_rates[extinction_leaf][2]
+#             #distances
+#             if hyb_used:
+#                 for l in leaves:
+#                     if l!=extinction_leaf:
+#                         if (extinction_leaf,l) in distances.keys():
+#                             del distances[(extinction_leaf,l)]
+#                         else:
+#                             del distances[(l,extinction_leaf)]
+
+#             del leaf_rates[extinction_leaf]
+#             leaves.remove(extinction_leaf)
+#             no_of_extinct+=1
+
+#         elif random_number < (current_extinction_rate + current_speciation_rate + current_hgt_rate) / total_rate:
+#             ######################
+#             #      HGT event     #
+#             ######################
+#             if not simple_output:
+#                 print("HGT")
+
+#             random_number = random.random()*current_hgt_rate
+#             for leaf,rates in leaf_rates.items():
+#                 if random_number < rates[2]:
+#                     hgt_acceptor_leaf = leaf
+#                     break
+#                 random_number -= rates[2]
+#             if hgt_acceptor_leaf == None:
+#                 if not simple_output:
+#                     print("ouch, hgt rate computed wrong")
+#             if len(leaves)>1:
+#                 hgt_donor_leaf = random.sample(leaves-set([hgt_acceptor_leaf]),1)[0]
+#                 for p in nw.predecessors(hgt_acceptor_leaf):
+#                     parent_acceptor=p
+#                 nw.add_weighted_edges_from([(hgt_donor_leaf,hgt_acceptor_leaf,0),(hgt_donor_leaf,current_node,0),(hgt_acceptor_leaf,current_node+1,0)], weight = 'length')
+#                 prob = hgt_inheritance*random.random()
+#                 nw[parent_acceptor][hgt_acceptor_leaf]['prob'] = 1-prob
+#                 nw[hgt_donor_leaf][hgt_acceptor_leaf]['prob'] = prob
+
+#                 hybrid_nodes[hgt_acceptor_leaf]=no_of_hybrids
+#                 no_of_hybrids+=1
+#                 #Update the rates and distances
+#                 #rates
+#                 leaf_rates[current_node+1]=CalculateAllNewRates(tuple(prob*x + (1-prob)*y for x, y in zip(leaf_rates[hgt_acceptor_leaf], leaf_rates[hgt_donor_leaf])),update_shape,
+#                     speciation_rate_mean, speciation_rate_shape,
+#                     ext_used, extinction_rate_mean, extinction_rate_shape,
+#                     hgt_used, hgt_rate_mean, hgt_rate_shape)
+#                 leaf_rates[current_node]  =leaf_rates[hgt_donor_leaf]
+#                 current_speciation_rate += leaf_rates[current_node+1][0]-leaf_rates[hgt_acceptor_leaf][0]
+#                 current_extinction_rate += leaf_rates[current_node+1][1]-leaf_rates[hgt_acceptor_leaf][1]
+#                 current_hgt_rate        += leaf_rates[current_node+1][2]-leaf_rates[hgt_acceptor_leaf][2]
+#                 del leaf_rates[hgt_donor_leaf]
+#                 del leaf_rates[hgt_acceptor_leaf]
+#                 #distances
+#                 if hyb_used:
+#                     for l in leaves:
+#                         if l!=hgt_acceptor_leaf:
+#                             acceptor_pair = (hgt_acceptor_leaf,l)
+#                             if acceptor_pair in distances.keys():
+#                                 acceptor_distance = distances[acceptor_pair]
+#                             else:
+#                                 acceptor_pair = (l,hgt_acceptor_leaf)
+#                                 acceptor_distance = distances[acceptor_pair]
+#                             donor_pair = (l,hgt_donor_leaf)
+#                             donor_distance = 0.0
+#                             if l!=hgt_donor_leaf:
+#                                 if donor_pair in distances.keys():
+#                                     donor_distance = distances[donor_pair]
+#                                 else:
+#                                     donor_pair = (hgt_donor_leaf,l)
+#                                     donor_distance = distances[donor_pair]
+#                                 distances[(l,current_node)]=donor_distance
+#                                 del distances[donor_pair]
+#                             distances[(l,current_node+1)]=(1-prob)*acceptor_distance+prob*donor_distance
+#                             del distances[acceptor_pair]
+#                     distances[(current_node,current_node+1)]=distances[(hgt_donor_leaf,current_node+1)]
+#                     del distances[(hgt_donor_leaf,current_node+1)]
+#                 leaves.remove(hgt_donor_leaf)
+#                 leaves.remove(hgt_acceptor_leaf)
+#                 leaves.add(current_node)
+#                 leaves.add(current_node+1)
+#                 current_node+=2
+
+#     #        else:
+#     #            print("trying HGT with only one leaf")
+#     #             #Do nothing, there is only one leaf.
+
+
+#         else:
+#             ######################
+#             #    Hybridization   #
+#             ######################
+#             if not simple_output:
+#                 print("hybridization")
+#         	#i.e.: pick two leaf nodes, create a hybrid between these two leaves
+#             random_number = random.random()*current_hybridization_rate
+#             for pair,distance in distances.items():
+#         	    pair_rate = DistanceToRate(distance,
+#                     hybridization_left_bound,
+#                     hybridization_right_bound,
+#                     hybridization_left_rate,
+#                     hybridization_right_rate)
+#         	    if random_number<pair_rate:
+#         	        hyb_pair = pair
+#         	        break
+#         	    random_number -=pair_rate
+#             if hyb_pair == None and not simple_output:
+#                 if len(leaves)==1:
+#                     print("ah, no leaves for hyb")
+#                 else:
+#                     print("ouch, hybridization rate computed wrong")
+#             nw.add_weighted_edges_from([(current_node,current_node+1,0),(hyb_pair[0],current_node,0),(hyb_pair[1],current_node,0),(hyb_pair[0],current_node+2,0),(hyb_pair[1],current_node+3,0)],weight = 'length')
+#             prob = random.random()
+#             nw[hyb_pair[0]][current_node]['prob'] = prob
+#             nw[hyb_pair[1]][current_node]['prob'] = 1-prob
+#             hybrid_nodes[current_node]=no_of_hybrids
+#             no_of_hybrids+=1
+
+
+#             #Update the rates and distances
+#             #rates
+#             leaf_rates[current_node+1]  =CalculateAllNewRates(tuple(prob*x + (1-prob)*y for x, y in zip(leaf_rates[hyb_pair[0]], leaf_rates[hyb_pair[1]])),update_shape,
+#                     speciation_rate_mean, speciation_rate_shape,
+#                     ext_used, extinction_rate_mean, extinction_rate_shape,
+#                     hgt_used, hgt_rate_mean, hgt_rate_shape)
+#             leaf_rates[current_node+2]  =leaf_rates[hyb_pair[0]]
+#             leaf_rates[current_node+3]  =leaf_rates[hyb_pair[1]]
+#             current_speciation_rate += leaf_rates[current_node+1][0]
+#             current_extinction_rate += leaf_rates[current_node+1][1]
+#             current_hgt_rate        += leaf_rates[current_node+1][2]
+#             #distances
+#             #TODO FIXED?!: The order may still be wrong. It seems I already delete some distances when I still need them later.
+#             #These are probably the distances related to the hybrid parent species.
+#             for l in leaves:
+#                 if l == hyb_pair[0]:
+#                     pair_0_distance = 0
+#                 else:
+#                     pair_0 = (hyb_pair[0],l)
+#                     if pair_0 not in distances.keys():
+#                         pair_0 = (l,hyb_pair[0])
+#                     pair_0_distance = distances[pair_0]
+#                     distances[(l,current_node+2)]=pair_0_distance
+#     #                del distances[pair_0]
+#                 if l == hyb_pair[1]:
+#                     pair_1_distance = 0
+#                 else:
+#                     pair_1 = (hyb_pair[1],l)
+#                     if pair_1 not in distances:
+#                         pair_1 = (l,hyb_pair[1])
+#                     pair_1_distance = distances[pair_1]
+#                     distances[(l,current_node+3)]=pair_1_distance
+#     #                del distances[pair_1]
+#                 distances[(l,current_node+1)]=prob*pair_0_distance+(1-prob)*pair_1_distance
+
+#             if (hyb_pair[0],hyb_pair[1]) in distances:
+#                 distances[(current_node+2,current_node+3)]=distances[(hyb_pair[0],hyb_pair[1])]
+#             else:
+#                 distances[(current_node+2,current_node+3)]=distances[(hyb_pair[1],hyb_pair[0])]
+#             distances[(current_node+1,current_node+2)]=distances[(hyb_pair[0],current_node+1)]
+#             distances[(current_node+1,current_node+3)]=distances[(hyb_pair[1],current_node+1)]
+
+
+#             remove_pairs = []
+#             for pair in distances:
+#                 if hyb_pair[0] in pair or hyb_pair[1] in pair:
+#                     remove_pairs +=[pair]
+#             for pair in remove_pairs:
+#                 del distances[pair]
+
+#             del leaf_rates[hyb_pair[0]]
+#             del leaf_rates[hyb_pair[1]]
+#             leaves.remove(hyb_pair[0])
+#             leaves.remove(hyb_pair[1])
+#             leaves.add(current_node+1)
+#             leaves.add(current_node+2)
+#             leaves.add(current_node+3)
+#             current_node+=4
+
+
+#         #Now extend all pendant edges of extant taxa
+#         if len(leaves)==0:
+#             break
+#         for l in leaves:
+#             pl = -1
+#             for p in nw.predecessors(l):
+#                 pl = p
+#             nw[pl][l]['length']+=extra_time
+
+#         #Compute the new rates
+#         current_hybridization_rate = 0
+#         if hyb_used:
+#             for pair,distance in distances.items():
+#                 distances[pair]+=2*extra_time
+#                 current_hybridization_rate+=DistanceToRate(distances[pair],
+#                     hybridization_left_bound,
+#                     hybridization_right_bound,
+#                     hybridization_left_rate,
+#                     hybridization_right_rate)
+
+#         total_rate = current_speciation_rate + current_extinction_rate + current_hgt_rate + current_hybridization_rate
+
+#         #Compute the time of the next event
+#         extra_time    = np.random.exponential(1/total_rate)
+#         current_time += extra_time
+
+#     #The following corrects for overshooting the time limit
+#     extra_time += time_limit-current_time
+#     #nothing has happened yet, and there is only one node
+#     if len(nw) == 1:
+#         nw.add_weighted_edges_from([(0,1,time_limit)],weight = 'length')
+#         leaves = set([1])
+#     # each leaf has a parent node, and we can extend each parent edge to time_limit
+#     else:
+#         for l in leaves:
+#             pl = -1
+#             for p in nw.predecessors(l):
+#                 pl = p
+#             nw[pl][l]['length']+=extra_time
+
+#     return nw,hybrid_nodes,leaves,no_of_extinct
+
+
+# ######################## MAIN ########################
+
+
+# import numpy as np
+# import math
+# import scipy.stats
+# import random
+# import networkx as nx
+# import sys
+# import itertools
+# #from AddEdgesToTree import *
+# from HeathNetwork_Tools import *
+
+# ##PARAMETERS
+# edges = False
+# only_extant = False
+
+# params = {"time_limit"          : 1.0,
+#     "taxa_limit"                : None,
+#     "update_shape"              : 2.0,
+#     "speciation_rate_mean"      : 2.0,
+#     "speciation_rate_shape"     : 2.0,
+#     "ext_used"                  : True,
+#     "count_extinct"             : 0,
+#     "extinction_rate_mean"      : 2.0,
+#     "extinction_rate_shape"     : 2.0,
+#     "hgt_used"                  : False,
+#     "hgt_rate_mean"             : None,
+#     "hgt_rate_shape"            : None,
+#     "hgt_inheritance"           : 0.05,
+#     "hyb_used"                  : False,
+#     "hybridization_left_bound"  : None,
+#     "hybridization_right_bound" : None,
+#     "hybridization_left_rate"   : None,
+#     "hybridization_right_rate"  : None,
+#     "simple_output"             : False}
+# ##
+
+
+# #random.gammavariate(alpha, beta)
+# #shape and scale
+# #On wiki,   alpha = k = `shape'   and    beta = theta = `scale'
+# #Mean = alpha.beta
+# #
+# #Can also use numpy.random.gamma(shape, scale=1.0)
+
+# ############################### I/O ############################
+
+# option_help = False
+# i = 1
+# while i < len(sys.argv):
+#     arg= sys.argv[i]
+#     if arg == "-ti" or arg == "--time":
+#         i+=1
+#         params["time_limit"] = float(sys.argv[i])
+#     if arg == "-ta" or arg == "--taxa":
+#         i+=1
+#         params["taxa_limit"] = float(sys.argv[i])
+#     if arg == "-ce" or arg == "--count_extinct":
+#         params["count_extinct"] = 1
+#     if arg == "-sp" or arg == "--speciation_parameters":
+#         i+=1
+#         params["speciation_rate_mean"] = float(sys.argv[i])
+#         i+=1
+#         speciation_rate_shape = float(sys.argv[i])
+#     if arg == "-noext" or arg == "--no_extinction":
+#         params["ext_used"] = False
+#     if arg == "-oe" or arg == "--only_extant":
+#         only_extant = True
+#     if arg == "-ext" or arg == "--extinction_parameters":
+#         i+=1
+#         params["extinction_rate_mean"] = float(sys.argv[i])
+#         i+=1
+#         params["extinction_rate_shape"] = float(sys.argv[i])
+#         if params["extinction_rate_mean"]==0:
+#             params["ext_used"] = False
+#     if arg == "-hgt" or arg == "--hgt_parameters":
+#         i+=1
+#         params["hgt_rate_mean"] = float(sys.argv[i])
+#         i+=1
+#         params["hgt_rate_shape"] = float(sys.argv[i])
+#         params["hgt_used"] = True
+#     if arg == "-hyb" or arg == "--hybridization_factor":
+#         i+=1
+#         params["hybridization_left_bound"]  = float(sys.argv[i])
+#         i+=1
+#         params["hybridization_right_bound"] = float(sys.argv[i])
+#         i+=1
+#         params["hybridization_left_rate"]   = float(sys.argv[i])
+#         i+=1
+#         params["hybridization_right_rate"]  = float(sys.argv[i])
+#         params["hyb_used"] = True
+#     if arg == "-upd" or arg == "--update_shape_parameter":
+#         i+=1
+#         params["update_shape"] = float(sys.argv[i])
+#     if arg == "-s" or arg == "--simple":
+#         params["simple_output"] = True
+#     if arg == "-h" or arg == "--help":
+#         option_help = True
+#     i += 1
+
+
+# if option_help:
+#     print("Runs a speciation-extinction-HGT-hybridization model for the given time (Default: ["+str(params["time_limit"])+"]) or until a certain number of extant taxa is reached. Each extant taxon has its own speciation, HGT, and extinction rates (1/mean_time_until_next_event). The hybridization rate of a pair of species is a function of the weighed distance between these species (sum of all up-down distances, weighed by their probability). There are prior speciation/extinction/HGT rate distributions, gamma distributions with a given mean and a shape parameter for speciation (Default: [mean="+str(params["speciation_rate_mean"])+", shape="+str(params["speciation_rate_shape"])+"]) and extinction (Default: [mean="+str(params["extinction_rate_mean"])+", shape="+str(params["extinction_rate_shape"])+"]), HGT is turned off. If a HGT event happens for a given taxon, another taxon (including itself) is chosen uniformly at random to donate genetic material (uniformly distributed contribution in [0,"+str(params["hgt_inheritance"])+"]). After speciation or hybridization, each rate of the new lineages is set by multiplying the (weighted mean) rate of the parent lineage(s) by a gamma-distributed factor with mean 1 and a shape parameter (Default: [shape="+str(params["update_shape"])+"]), and then accepting this rate with a probability proportional to the prior distribution for this rate. This gives an ultrametric network on the extant species. \n\nOptional arguments:\n -ti or --time followed by the total length (float) for the network.\n -ta or --taxa followed by the number of taxa at which the simulation stops. If all lineages go extinct before the given number of taxa is reached, another attempt is made.\n -ce or --count_extinct to also count the extinct taxa as part of the taxa limit.\n -oe or --only_extant to return the network restricted to the extant leaves.\n\nRates:\n -sp or --speciation_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the speciation rate.\n -ext or --extinction_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the extinction rate.\n -noext or --no_extinction to turn off extinction altogether.\n -hgt or --hgt_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the HGT rate.\n -upd or --update_shape_parameter followed by a shape parameter (float) for the update gamma distribution.\n -hyb or --hyb_factor followed by four floats for the piecewise linear dependence of hybridization rate on the distance:\n    left bound:  l\n    right bound: r\n    left rate:   rl\n    right rate:  rr.\n\n  |\nlr+---\n  |   \\\n  |    \\\n  |     \\\nrr+      -----\n  |\n 0+--+---+-----\n  0  l   r")
+#     sys.exit()
+
+
+# #Find a network
+# if params["taxa_limit"]:
+#     leaves = []
+#     no_of_extinct = 0
+#     while len(leaves)+params["count_extinct"]*no_of_extinct!=params["taxa_limit"]:
+#         if not params["simple_output"]:
+#             print("starting over")
+#         network,hybrid_nodes,leaves,no_of_extinct = CalculateNetwork(**params)
+# else:
+#     print(params)
+#     network,hybrid_nodes,leaves,no_of_extinct = CalculateNetwork(**params)
+
+# #Restrict to extant leaves if wanted
+# if only_extant:
+#     network = RestrictToLeafSet(network,leaves)
+
+
+# for e in network.edges:
+#     info =""
+#     if e[0] in hybrid_nodes:
+#         info += "H"+str(hybrid_nodes[e[0]])
+#     else:
+#         info += str(e[0])
+#     info += "  "
+#     if e[1] in hybrid_nodes:
+#         info += "H"+str(hybrid_nodes[e[1]])
+#     else:
+#         info += str(e[1])
+#     print(info)#,network[e[0]][e[1]]['length'])
+
+
+# #### To use: argparse version:
+
+# import argparse
+# import sys
+
+# parser = argparse.ArgumentParser(description="Runs a speciation-extinction-HGT-hybridization model.")
+
+# parser.add_argument("-ti", "--time", dest="time_limit", type=float, help="Total length for the network")
+# parser.add_argument("-ta", "--taxa", dest="taxa_limit", type=float, help="Number of taxa at which the simulation stops")
+# parser.add_argument("-ce", "--count_extinct", action="store_true", help="Count extinct taxa as part of the taxa limit")
+# parser.add_argument("-sp", "--speciation_parameters", nargs=2, type=float, metavar=("mean", "shape"), help="Mean and shape parameter for the gamma distribution of the speciation rate")
+# parser.add_argument("-ext", "--extinction_parameters", nargs=2, type=float, metavar=("mean", "shape"), help="Mean and shape parameter for the gamma distribution of the extinction rate")
+# parser.add_argument("-noext", "--no_extinction", action="store_true", help="Turn off extinction altogether")
+# parser.add_argument("-hgt", "--hgt_parameters", nargs=2, type=float, metavar=("mean", "shape"), help="Mean and shape parameter for the gamma distribution of the HGT rate")
+# parser.add_argument("-hyb", "--hybridization_factor", nargs=4, type=float, metavar=("l", "r", "rl", "rr"), help="Piecewise linear dependence of hybridization rate on the distance")
+# parser.add_argument("-upd", "--update_shape_parameter", type=float, help="Shape parameter for the update gamma distribution")
+# parser.add_argument("-s", "--simple", action="store_true", help="Enable simple output")
+# parser.add_argument("-h", "--help", action="store_true", help="Show help message")
+
+# args = parser.parse_args()
+
+# params = {
+#     "time_limit": args.time_limit,
+#     "taxa_limit": args.taxa_limit,
+#     "count_extinct": args.count_extinct,
+#     "speciation_rate_mean": args.speciation_parameters[0] if args.speciation_parameters else None,
+#     "speciation_rate_shape": args.speciation_parameters[1] if args.speciation_parameters else None,
+#     "extinction_rate_mean": args.extinction_parameters[0] if args.extinction_parameters else None,
+#     "extinction_rate_shape": args.extinction_parameters[1] if args.extinction_parameters else None,
+#     "ext_used": not args.no_extinction,
+#     "hgt_rate_mean": args.hgt_parameters[0] if args.hgt_parameters else None,
+#     "hgt_rate_shape": args.hgt_parameters[1] if args.hgt_parameters else None,
+#     "hgt_used": args.hgt_parameters is not None,
+#     "hybridization_left_bound": args.hybridization_factor[0] if args.hybridization_factor else None,
+#     "hybridization_right_bound": args.hybridization_factor[1] if args.hybridization_factor else None,
+#     "hybridization_left_rate": args.hybridization_factor[2] if args.hybridization_factor else None,
+#     "hybridization_right_rate": args.hybridization_factor[3] if args.hybridization_factor else None,
+#     "hyb_used": args.hybridization_factor is not None,
+#     "update_shape": args.update_shape_parameter,
+#     "simple_output": args.simple
+# }
```

### Comparing `phylox-0.0.1/src/phylox/generators/lgt/Generator.py` & `phylox-0.0.2/src/phylox/generators/lgt/Generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,473 +1,433 @@
-#By Pons et al.
+# #By Pons et al.
 
-import matplotlib
-import networkx as nx
-import pylab as plt
-import random,numpy
-import itertools
-import os
-import numpy as np
-from networkx.drawing.nx_agraph import graphviz_layout
-
-
-
-def last_node(net):
-    return max(net.nodes())
-
-
-def speciate(net,leaf):
-    l = last_node(net)
-    net.add_edge(leaf,l+1)
-    net.add_edge(leaf,l+2)
-
-
-
-
-def lgt(net,leaf1,leaf2):
-    net.add_edge(leaf1,leaf2,secondary=True)
-    l = last_node(net)
-    net.add_edge(leaf1,l+1)
-    net.add_edge(leaf2,l+2)
-
-
-
-
-def draw(net):
-    positions = nx.drawing.nx_agraph.graphviz_layout(net, prog="dot")
-    # nx.draw(net, pos=graphviz_layout(net),prog='dot',args="-Grankdir=LR", with_labels=True)
-    nx.draw(net,positions,with_labels=True)
-    plt.show()
-
-
-
-
-def leaves(net):
-    return [u for u in net.nodes() if net.out_degree(u)==0]
-
-
-
-
-def non_trivial_blobs(net):
-    blobs = list(nx.biconnected_components(nx.Graph(net)))
-    return [bl for bl in blobs if len(bl) > 2]
-
-
-
-
-def internal_blobs(net):
-    internal_nodes = set([u for u in net.nodes() if net.out_degree(u)>0])
-    blobs = list(nx.biconnected_components(nx.Graph(net)))
-    blobs = [bl for bl in blobs if len(bl) > 2]
-    nodes_in_blobs = set().union(*blobs)
-    nodes_not_in_blobs = internal_nodes - nodes_in_blobs
-    blobs.extend([set([u]) for u in nodes_not_in_blobs])
-    return blobs
-
-
-
-
-def compute_hash(net):
-    mapping_blobs = {}
-    blobs = internal_blobs(net)
-    for blob in blobs:
-        for node in blob:
-            mapping_blobs[node] = blob
-    
-    mapping = {}
-    for l in leaves(net):
-        parent = list(net.predecessors(l))[0]
-        mapping[l] = mapping_blobs[parent]
-    return mapping
-
-
-
-
-def internal_and_external_pairs(net):
-    lvs = leaves(net)
-    pairs = [(l1,l2) for l1 in lvs for l2 in lvs if l1 != l2]
-    mapping = compute_hash(net)
-    internal_pairs = []
-    external_pairs = []
-    for pair in pairs:
-        if mapping[pair[0]] == mapping[pair[1]]:
-            internal_pairs.append(pair)
-        else:
-            external_pairs.append(pair)
-    return internal_pairs, external_pairs
-
-
-
-
-def random_leaf(net):
-    return random.choice(leaves(net))
-
-
-
-
-def random_pair(net,wint,wext):
-    int_pairs, ext_pairs = internal_and_external_pairs(net)
-    return random.choices(int_pairs+ext_pairs, weights=[wint]*len(int_pairs)+[wext]*len(ext_pairs))[0]
-
-
-
-
-def simulation_1(num_steps,prob_lgt,wint,wext):
-    net = nx.DiGraph()
-    net.add_edge(1,2)
-    net.add_edge(1,3)
-    for i in range(num_steps):
-        event = random.choices(['spec','lgt'],[1-prob_lgt, prob_lgt])[0]
-        #event = numpy.random.choice(['spec','lgt'],p=[1-prob_lgt, prob_lgt])
-        if event == 'spec':
-            l = random.choice(leaves(net))
-            speciate(net,l)
-        else:
-            pair = random_pair(net,wint,wext)
-            lgt(net,pair[0],pair[1])
-    return net
-
-
-
-def simulation_2(leaves_goal,prob_lgt,wint,wext):
-    net = nx.DiGraph()
-    net.add_edge(1,2)
-    net.add_edge(1,3)
-    leaves_no = 2
-    while leaves_no < leaves_goal:
-        event = random.choices(['spec','lgt'],[1-prob_lgt, prob_lgt])[0]
-        #event = numpy.random.choice(['spec','lgt'],p=[1-prob_lgt, prob_lgt])
-        if event == 'spec':
-            l = random.choice(leaves(net))
-            speciate(net,l)
-            leaves_no+=1
-        else:
-            pair = random_pair(net,wint,wext)
-            lgt(net,pair[0],pair[1])
-    return net
-
-
-
-
-def simulation_3(leaves_goal,retics_goal,wint,wext):
-    #pick a number of extant lineages for each LGT event independently
-    retics_at_lineage = dict()
-    for r in range(retics_goal):
-        lin = random.choice(range(2,leaves_goal+1))
-        if lin in retics_at_lineage:
-            retics_at_lineage[lin]+=1
-        else:
-            retics_at_lineage[lin]=1
-    net = nx.DiGraph()
-    net.add_edge(1,2)
-    net.add_edge(1,3)
-    if 2 in retics_at_lineage:
-        for j in range(retics_at_lineage[2]):
-            pair = random_pair(net,wint,wext)
-            lgt(net,pair[0],pair[1])
-    for i in range(3,leaves_goal+1):
-        l = random.choice(leaves(net))
-        speciate(net,l)
-        if i in retics_at_lineage:
-            for j in range(retics_at_lineage[i]):
-                pair = random_pair(net,wint,wext)
-                lgt(net,pair[0],pair[1])
-    return net
-
-
-
-
-
-def reticulations(G):
-    return [v for v in G.nodes() if G.in_degree(v)==2]
-    
-def local_level(G,bicc):
-    rets=list(set(reticulations(G)).intersection(bicc)) # reticulations present in the blob
-    if len(rets)==0:
-        return 0
-    else:
-        bicc_edges=[e for e in G.edges() if ((e[0] in bicc)&(e[1]in bicc))]
-        end_nodes=[e[1] for e in bicc_edges]
-        return len([ret for ret in rets if ret in end_nodes]) 
-
-
-
-
-
-
-def OutputNetwork(network,out_type,leaves = None):
-    output = ""
-    if out_type=="el":
-        for i,e in enumerate(network.edges):
-            if i!=0:
-                output+="\r\n"
-            output += str(e[0])+" "+str(e[1])
-    elif out_type=="pl":
-        #find number of leaves if necessary
-        if leaves == None:
-            leaves = 0
-            for v in network.nodes:
-                if network.out_degree(v)==0:
-                    leaves+=1
-         
-        #relabel nodes 
-        labelDict           = dict()
-        leaves_current      = 1
-        internal_current    = leaves+1
-        
-        for v in network.nodes:
-            if network.out_degree(v)==0:
-                labelDict[v]=leaves_current
-                leaves_current+=1
-            else:
-                labelDict[v]=internal_current
-                internal_current+=1
-                
-        #generate parent lists
-        for i,v in enumerate(network.nodes):
-            if i!=0:
-                output+="\r\n"
-            output += str(v)+";"
-            parentList=""
-            for p in network.predecessors(v):
-                parentList+=str(labelDict[p])+","
-            output+=parentList[:-1]
-    return output
-
-
-
-
-
-##################################
-########     ALL DATA     ########
-##################################
-
-"""
-number_of_experiments = 500
-values_of_n = [100]
-values_of_alpha = [0.0,0.1,0.2,0.3,0.4]
-values_of_beta = [0.01,0.1,1,10,100] #weight of outside blob pair, inside blob weight is 1
-foldername = "./Dataset_n_100/"
-
-
-for out_type in ["el","pl"]:
-    this_path = foldername+out_type
-    if not os.path.exists(this_path):
-        os.makedirs(this_path) 
-
-for (n, alpha, beta) in itertools.product(values_of_n, values_of_alpha, values_of_beta):
-    print(alpha,beta)
-    for i in range(number_of_experiments):
-        resG = simulation_2(n, alpha, 1, beta)
-        for out_type in ["el","pl"]:
-            filename = foldername+out_type+"/"+str(alpha)+"_"+str(beta)+"_"+str(i)
-            f=open(filename, 'w')
-            f.write(OutputNetwork(resG,out_type))
-            f.close()    
-"""
-        
-        
-##################################
-########   FIXED RETICS   ########
-##################################
-
-
-number_of_experiments = 500
-values_of_n     = [50]#[10,15,20,25] # [100]
-values_of_k     = [1,2,3,4,5,10,20,50,100,200,500]#[6,7,8,9,10]#[1,2,3,4,5]
-values_of_n_k   = list(itertools.product(values_of_n, values_of_k))
-values_of_alpha = [float(k)/(n+k+1) for n,k in values_of_n_k]#Making sure the desired number of retics is the mode of the binom distribution that determines it
-values_of_n_k_and_alpha     = zip(values_of_n_k,values_of_alpha)
-values_of_beta = [1.0,0.1,0.01]#[0.01,0.1,1,10,100] #weight of outside blob pair, inside blob weight is 1
-def foldername(n):
-    return "./Dataset_n_"+str(n)+"_fixed_k/"
-
-for n in values_of_n:
-    for out_type in ["el","pl"]:
-        this_path = foldername(n)+out_type
-        if not os.path.exists(this_path):
-            os.makedirs(this_path) 
-
-for (n_k_and_alpha, beta) in itertools.product(values_of_n_k_and_alpha, values_of_beta):
-    n_k,alpha=n_k_and_alpha
-    n,k = n_k
-    print(n,k,beta)
-    for i in range(number_of_experiments):
-#        print(k,beta,i)
-        resG=nx.DiGraph()
-        while len(reticulations(resG))!=k:
-# naive method:
-#            resG = simulation_1(n+k, alpha, 1, beta)
-# fast method:
-            resG = simulation_3(n  ,     k, 1, beta)
-        for out_type in ["el","pl"]:
-            filename = foldername(n)+out_type+"/"+str(k)+"_"+str(beta)+"_"+str(i)
-            f=open(filename, 'w')
-            f.write(OutputNetwork(resG,out_type))
-            f.close()    
-
-
-#Compare realistic data
-"""
-number_of_experiments = 500
-values_of_n_k       = [(4,5),(5,5),(6,2),(6,3),(6,4),(6,6),(7,4),(7,32),(8,3),(8,5),(9,3),(9,4),(9,5),(11,5),(13,1),(13,2),(13,6),(15,6),(16,4),(17,2),(21,6),(22,9),(24,2),(25,2),(28,5),(29,2),(39,11)]
-values_of_alpha = [float(i[1])/(i[0]+i[1]+1) for i in values_of_n_k]#Making sure the desired number of retics is the mode of the binom distribution that determines it
-values_of_n_k_and_alpha     = zip(values_of_n_k,values_of_alpha)
-values_of_beta = [0.01,0.1,1] #weight of outside blob pair, inside blob weight is 1
-foldername = "./Dataset_Realistic_Comparison/"
-
-
-
-for out_type in ["el","pl"]:
-    this_path = foldername+out_type
-    if not os.path.exists(this_path):
-        os.makedirs(this_path) 
-
-for (n_k_alpha, beta) in itertools.product(values_of_n_k_and_alpha, values_of_beta):
-    n_k,alpha=n_k_alpha
-    n,k=n_k
-    print(n,k,alpha,beta)
-    for i in range(number_of_experiments):
-#        print(k,beta,i)
-        resG=nx.DiGraph()
-        while len(reticulations(resG))!=k:
-# naive method:
-#            resG = simulation_1(n+k, alpha, 1, beta)
-# fast method:
-            resG = simulation_3(n  ,     k, 1, beta)
-        for out_type in ["el","pl"]:
-            filename = foldername+out_type+"/"+str(n)+"_"+str(k)+"_"+str(beta)+"_"+str(i)
-            f=open(filename, 'w')
-            f.write(OutputNetwork(resG,out_type))
-            f.close()    
-"""
-
-
-
-
-
-
-
-##################################
-########## PLOTTING STUFF ########
-##################################
-
-
-# In[33]:
-
-"""
-f = plt.figure()
-x_positions=range(len(values_of_beta))
-x_axis = values_of_beta
-symbols = "ox*+"
-i = 0
-dibs = [None]*4
-legends = [None]*4
-for n in values_of_n:
-    for alpha in values_of_alpha:
-        to_plot = [stats_numblobs[(n, alpha, beta)] for beta in values_of_beta]
-        dibs[i]=plt.scatter(x_positions, to_plot, marker = symbols[i], c='black')
-        legends[i] = "n=%d, alpha=%0.1f" % (n, alpha)
-        i += 1
-plt.xticks(x_positions, x_axis)
-plt.legend(dibs, legends)
-plt.xlabel('beta')
-plt.ylabel('avg number of nontrivial blobs')
-plt.show()
-f.savefig("fig10.pdf", bbox_inches='tight')
-
-
-# In[34]:
-
-
-f = plt.figure()
-x_positions=range(len(values_of_beta))
-x_axis = values_of_beta
-symbols = "ox*+"
-i = 0
-dibs = [None]*4
-legends = [None]*4
-for n in values_of_n:
-    for alpha in values_of_alpha:
-        to_plot = [stats_level[(n, alpha, beta)] for beta in values_of_beta]
-        dibs[i]=plt.scatter(x_positions, to_plot, marker = symbols[i], c='black')
-        legends[i] = "n=%d, alpha=%0.1f" % (n, alpha)
-        i += 1
-plt.xticks(x_positions, x_axis)
-plt.legend(dibs, legends)
-plt.xlabel('beta')
-plt.ylabel('avg level')
-plt.show()
-f.savefig("fig11.pdf", bbox_inches='tight')
-
-
-# In[35]:
-
-number_of_experiments2 = 500
-values_of_n2 = [10,20,30]
-values_of_alpha2 = [0,0.1,0.2,0.3,0.4]
-values_of_beta2 = [0.01, 1, 10]
-stats_level2 = {}
-stats_numblobs2 = {}
-
-for (n, alpha, beta) in itertools.product(values_of_n2, values_of_alpha2, values_of_beta2):
-    levels = []
-    numblobs = []
-    for _ in range(number_of_experiments):
-        resG = simulation(n, alpha, 1, beta)
-        bic_comp=list(nx.biconnected_components(nx.Graph(resG)))
-        rets_x_bicc=[local_level(resG,b) for b in bic_comp]
-        level=max(rets_x_bicc)
-        levels.append(level)
-        sparse=[1 for x in rets_x_bicc if x!=0]
-        numblobs.append(sum(sparse))
-    stats_level2[(n, alpha, beta)] = float(sum(levels))/len(levels)
-    stats_numblobs2[(n, alpha, beta)] = float(sum(numblobs))/len(numblobs)
-
-
-# In[ ]:
-
-
-f = plt.figure()
-x_positions=range(len(values_of_alpha2))
-x_axis = values_of_alpha2
-symbols = "ox*+"
-i = 0
-dibs = [None]*4
-legends = [None]*4
-for n in [10,30]:
-    for beta in [0.01,10]:
-        to_plot = [stats_level2[(n, alpha, beta)] for alpha in values_of_alpha2]
-        dibs[i]=plt.scatter(x_positions, to_plot, marker = symbols[i], c='black')
-        legends[i] = "n=%d, beta=%0.2f" % (n, beta)
-        i += 1
-plt.xticks(x_positions, x_axis)
-plt.legend(dibs, legends)
-plt.xlabel('alpha')
-plt.ylabel('avg level')
-plt.show()
-f.savefig("fig8.pdf", bbox_inches='tight')
-
-
-# In[ ]:
-
-
-f = plt.figure()
-x_positions=range(len(values_of_alpha2))
-x_axis = values_of_alpha2
-symbols = "ox*+"
-i = 0
-dibs = [None]*4
-legends = [None]*4
-for n in [10,30]:
-    for beta in [0.01,10]:
-        to_plot = [stats_numblobs2[(n, alpha, beta)] for alpha in values_of_alpha2]
-        dibs[i]=plt.scatter(x_positions, to_plot, marker = symbols[i], c='black')
-        legends[i] = "n=%d, beta=%0.2f" % (n, beta)
-        i += 1
-plt.xticks(x_positions, x_axis)
-plt.legend(dibs, legends)
-plt.xlabel('alpha')
-plt.ylabel('avg number of nontrivial blobs')
-plt.show()
-f.savefig("fig9.pdf", bbox_inches='tight')
-"""
+# import matplotlib
+# import networkx as nx
+# import pylab as plt
+# import random,numpy
+# import itertools
+# import os
+# import numpy as np
+# from networkx.drawing.nx_agraph import graphviz_layout
+
+
+# def last_node(net):
+#     return max(net.nodes())
+
+
+# def speciate(net,leaf):
+#     l = last_node(net)
+#     net.add_edge(leaf,l+1)
+#     net.add_edge(leaf,l+2)
+
+
+# def lgt(net,leaf1,leaf2):
+#     net.add_edge(leaf1,leaf2,secondary=True)
+#     l = last_node(net)
+#     net.add_edge(leaf1,l+1)
+#     net.add_edge(leaf2,l+2)
+
+
+# def draw(net):
+#     positions = nx.drawing.nx_agraph.graphviz_layout(net, prog="dot")
+#     # nx.draw(net, pos=graphviz_layout(net),prog='dot',args="-Grankdir=LR", with_labels=True)
+#     nx.draw(net,positions,with_labels=True)
+#     plt.show()
+
+
+# def leaves(net):
+#     return [u for u in net.nodes() if net.out_degree(u)==0]
+
+
+# def non_trivial_blobs(net):
+#     blobs = list(nx.biconnected_components(nx.Graph(net)))
+#     return [bl for bl in blobs if len(bl) > 2]
+
+
+# def internal_blobs(net):
+#     internal_nodes = set([u for u in net.nodes() if net.out_degree(u)>0])
+#     blobs = list(nx.biconnected_components(nx.Graph(net)))
+#     blobs = [bl for bl in blobs if len(bl) > 2]
+#     nodes_in_blobs = set().union(*blobs)
+#     nodes_not_in_blobs = internal_nodes - nodes_in_blobs
+#     blobs.extend([set([u]) for u in nodes_not_in_blobs])
+#     return blobs
+
+
+# def compute_hash(net):
+#     mapping_blobs = {}
+#     blobs = internal_blobs(net)
+#     for blob in blobs:
+#         for node in blob:
+#             mapping_blobs[node] = blob
+
+#     mapping = {}
+#     for l in leaves(net):
+#         parent = list(net.predecessors(l))[0]
+#         mapping[l] = mapping_blobs[parent]
+#     return mapping
+
+
+# def internal_and_external_pairs(net):
+#     lvs = leaves(net)
+#     pairs = [(l1,l2) for l1 in lvs for l2 in lvs if l1 != l2]
+#     mapping = compute_hash(net)
+#     internal_pairs = []
+#     external_pairs = []
+#     for pair in pairs:
+#         if mapping[pair[0]] == mapping[pair[1]]:
+#             internal_pairs.append(pair)
+#         else:
+#             external_pairs.append(pair)
+#     return internal_pairs, external_pairs
+
+
+# def random_leaf(net):
+#     return random.choice(leaves(net))
+
+
+# def random_pair(net,wint,wext):
+#     int_pairs, ext_pairs = internal_and_external_pairs(net)
+#     return random.choices(int_pairs+ext_pairs, weights=[wint]*len(int_pairs)+[wext]*len(ext_pairs))[0]
+
+
+# def simulation_1(num_steps,prob_lgt,wint,wext):
+#     net = nx.DiGraph()
+#     net.add_edge(1,2)
+#     net.add_edge(1,3)
+#     for i in range(num_steps):
+#         event = random.choices(['spec','lgt'],[1-prob_lgt, prob_lgt])[0]
+#         #event = numpy.random.choice(['spec','lgt'],p=[1-prob_lgt, prob_lgt])
+#         if event == 'spec':
+#             l = random.choice(leaves(net))
+#             speciate(net,l)
+#         else:
+#             pair = random_pair(net,wint,wext)
+#             lgt(net,pair[0],pair[1])
+#     return net
+
+
+# def simulation_2(leaves_goal,prob_lgt,wint,wext):
+#     net = nx.DiGraph()
+#     net.add_edge(1,2)
+#     net.add_edge(1,3)
+#     leaves_no = 2
+#     while leaves_no < leaves_goal:
+#         event = random.choices(['spec','lgt'],[1-prob_lgt, prob_lgt])[0]
+#         #event = numpy.random.choice(['spec','lgt'],p=[1-prob_lgt, prob_lgt])
+#         if event == 'spec':
+#             l = random.choice(leaves(net))
+#             speciate(net,l)
+#             leaves_no+=1
+#         else:
+#             pair = random_pair(net,wint,wext)
+#             lgt(net,pair[0],pair[1])
+#     return net
+
+
+# def simulation_3(leaves_goal,retics_goal,wint,wext):
+#     #pick a number of extant lineages for each LGT event independently
+#     retics_at_lineage = dict()
+#     for r in range(retics_goal):
+#         lin = random.choice(range(2,leaves_goal+1))
+#         if lin in retics_at_lineage:
+#             retics_at_lineage[lin]+=1
+#         else:
+#             retics_at_lineage[lin]=1
+#     net = nx.DiGraph()
+#     net.add_edge(1,2)
+#     net.add_edge(1,3)
+#     if 2 in retics_at_lineage:
+#         for j in range(retics_at_lineage[2]):
+#             pair = random_pair(net,wint,wext)
+#             lgt(net,pair[0],pair[1])
+#     for i in range(3,leaves_goal+1):
+#         l = random.choice(leaves(net))
+#         speciate(net,l)
+#         if i in retics_at_lineage:
+#             for j in range(retics_at_lineage[i]):
+#                 pair = random_pair(net,wint,wext)
+#                 lgt(net,pair[0],pair[1])
+#     return net
+
+
+# def reticulations(G):
+#     return [v for v in G.nodes() if G.in_degree(v)==2]
+
+# def local_level(G,bicc):
+#     rets=list(set(reticulations(G)).intersection(bicc)) # reticulations present in the blob
+#     if len(rets)==0:
+#         return 0
+#     else:
+#         bicc_edges=[e for e in G.edges() if ((e[0] in bicc)&(e[1]in bicc))]
+#         end_nodes=[e[1] for e in bicc_edges]
+#         return len([ret for ret in rets if ret in end_nodes])
+
+
+# def OutputNetwork(network,out_type,leaves = None):
+#     output = ""
+#     if out_type=="el":
+#         for i,e in enumerate(network.edges):
+#             if i!=0:
+#                 output+="\r\n"
+#             output += str(e[0])+" "+str(e[1])
+#     elif out_type=="pl":
+#         #find number of leaves if necessary
+#         if leaves == None:
+#             leaves = 0
+#             for v in network.nodes:
+#                 if network.out_degree(v)==0:
+#                     leaves+=1
+
+#         #relabel nodes
+#         labelDict           = dict()
+#         leaves_current      = 1
+#         internal_current    = leaves+1
+
+#         for v in network.nodes:
+#             if network.out_degree(v)==0:
+#                 labelDict[v]=leaves_current
+#                 leaves_current+=1
+#             else:
+#                 labelDict[v]=internal_current
+#                 internal_current+=1
+
+#         #generate parent lists
+#         for i,v in enumerate(network.nodes):
+#             if i!=0:
+#                 output+="\r\n"
+#             output += str(v)+";"
+#             parentList=""
+#             for p in network.predecessors(v):
+#                 parentList+=str(labelDict[p])+","
+#             output+=parentList[:-1]
+#     return output
+
+
+# ##################################
+# ########     ALL DATA     ########
+# ##################################
+
+# """
+# number_of_experiments = 500
+# values_of_n = [100]
+# values_of_alpha = [0.0,0.1,0.2,0.3,0.4]
+# values_of_beta = [0.01,0.1,1,10,100] #weight of outside blob pair, inside blob weight is 1
+# foldername = "./Dataset_n_100/"
+
+
+# for out_type in ["el","pl"]:
+#     this_path = foldername+out_type
+#     if not os.path.exists(this_path):
+#         os.makedirs(this_path)
+
+# for (n, alpha, beta) in itertools.product(values_of_n, values_of_alpha, values_of_beta):
+#     print(alpha,beta)
+#     for i in range(number_of_experiments):
+#         resG = simulation_2(n, alpha, 1, beta)
+#         for out_type in ["el","pl"]:
+#             filename = foldername+out_type+"/"+str(alpha)+"_"+str(beta)+"_"+str(i)
+#             f=open(filename, 'w')
+#             f.write(OutputNetwork(resG,out_type))
+#             f.close()
+# """
+
+
+# ##################################
+# ########   FIXED RETICS   ########
+# ##################################
+
+
+# number_of_experiments = 500
+# values_of_n     = [50]#[10,15,20,25] # [100]
+# values_of_k     = [1,2,3,4,5,10,20,50,100,200,500]#[6,7,8,9,10]#[1,2,3,4,5]
+# values_of_n_k   = list(itertools.product(values_of_n, values_of_k))
+# values_of_alpha = [float(k)/(n+k+1) for n,k in values_of_n_k]#Making sure the desired number of retics is the mode of the binom distribution that determines it
+# values_of_n_k_and_alpha     = zip(values_of_n_k,values_of_alpha)
+# values_of_beta = [1.0,0.1,0.01]#[0.01,0.1,1,10,100] #weight of outside blob pair, inside blob weight is 1
+# def foldername(n):
+#     return "./Dataset_n_"+str(n)+"_fixed_k/"
+
+# for n in values_of_n:
+#     for out_type in ["el","pl"]:
+#         this_path = foldername(n)+out_type
+#         if not os.path.exists(this_path):
+#             os.makedirs(this_path)
+
+# for (n_k_and_alpha, beta) in itertools.product(values_of_n_k_and_alpha, values_of_beta):
+#     n_k,alpha=n_k_and_alpha
+#     n,k = n_k
+#     print(n,k,beta)
+#     for i in range(number_of_experiments):
+# #        print(k,beta,i)
+#         resG=nx.DiGraph()
+#         while len(reticulations(resG))!=k:
+# # naive method:
+# #            resG = simulation_1(n+k, alpha, 1, beta)
+# # fast method:
+#             resG = simulation_3(n  ,     k, 1, beta)
+#         for out_type in ["el","pl"]:
+#             filename = foldername(n)+out_type+"/"+str(k)+"_"+str(beta)+"_"+str(i)
+#             f=open(filename, 'w')
+#             f.write(OutputNetwork(resG,out_type))
+#             f.close()
+
+
+# #Compare realistic data
+# """
+# number_of_experiments = 500
+# values_of_n_k       = [(4,5),(5,5),(6,2),(6,3),(6,4),(6,6),(7,4),(7,32),(8,3),(8,5),(9,3),(9,4),(9,5),(11,5),(13,1),(13,2),(13,6),(15,6),(16,4),(17,2),(21,6),(22,9),(24,2),(25,2),(28,5),(29,2),(39,11)]
+# values_of_alpha = [float(i[1])/(i[0]+i[1]+1) for i in values_of_n_k]#Making sure the desired number of retics is the mode of the binom distribution that determines it
+# values_of_n_k_and_alpha     = zip(values_of_n_k,values_of_alpha)
+# values_of_beta = [0.01,0.1,1] #weight of outside blob pair, inside blob weight is 1
+# foldername = "./Dataset_Realistic_Comparison/"
+
+
+# for out_type in ["el","pl"]:
+#     this_path = foldername+out_type
+#     if not os.path.exists(this_path):
+#         os.makedirs(this_path)
+
+# for (n_k_alpha, beta) in itertools.product(values_of_n_k_and_alpha, values_of_beta):
+#     n_k,alpha=n_k_alpha
+#     n,k=n_k
+#     print(n,k,alpha,beta)
+#     for i in range(number_of_experiments):
+# #        print(k,beta,i)
+#         resG=nx.DiGraph()
+#         while len(reticulations(resG))!=k:
+# # naive method:
+# #            resG = simulation_1(n+k, alpha, 1, beta)
+# # fast method:
+#             resG = simulation_3(n  ,     k, 1, beta)
+#         for out_type in ["el","pl"]:
+#             filename = foldername+out_type+"/"+str(n)+"_"+str(k)+"_"+str(beta)+"_"+str(i)
+#             f=open(filename, 'w')
+#             f.write(OutputNetwork(resG,out_type))
+#             f.close()
+# """
+
+
+# ##################################
+# ########## PLOTTING STUFF ########
+# ##################################
+
+
+# # In[33]:
+
+# """
+# f = plt.figure()
+# x_positions=range(len(values_of_beta))
+# x_axis = values_of_beta
+# symbols = "ox*+"
+# i = 0
+# dibs = [None]*4
+# legends = [None]*4
+# for n in values_of_n:
+#     for alpha in values_of_alpha:
+#         to_plot = [stats_numblobs[(n, alpha, beta)] for beta in values_of_beta]
+#         dibs[i]=plt.scatter(x_positions, to_plot, marker = symbols[i], c='black')
+#         legends[i] = "n=%d, alpha=%0.1f" % (n, alpha)
+#         i += 1
+# plt.xticks(x_positions, x_axis)
+# plt.legend(dibs, legends)
+# plt.xlabel('beta')
+# plt.ylabel('avg number of nontrivial blobs')
+# plt.show()
+# f.savefig("fig10.pdf", bbox_inches='tight')
+
+
+# # In[34]:
+
+
+# f = plt.figure()
+# x_positions=range(len(values_of_beta))
+# x_axis = values_of_beta
+# symbols = "ox*+"
+# i = 0
+# dibs = [None]*4
+# legends = [None]*4
+# for n in values_of_n:
+#     for alpha in values_of_alpha:
+#         to_plot = [stats_level[(n, alpha, beta)] for beta in values_of_beta]
+#         dibs[i]=plt.scatter(x_positions, to_plot, marker = symbols[i], c='black')
+#         legends[i] = "n=%d, alpha=%0.1f" % (n, alpha)
+#         i += 1
+# plt.xticks(x_positions, x_axis)
+# plt.legend(dibs, legends)
+# plt.xlabel('beta')
+# plt.ylabel('avg level')
+# plt.show()
+# f.savefig("fig11.pdf", bbox_inches='tight')
+
+
+# # In[35]:
+
+# number_of_experiments2 = 500
+# values_of_n2 = [10,20,30]
+# values_of_alpha2 = [0,0.1,0.2,0.3,0.4]
+# values_of_beta2 = [0.01, 1, 10]
+# stats_level2 = {}
+# stats_numblobs2 = {}
+
+# for (n, alpha, beta) in itertools.product(values_of_n2, values_of_alpha2, values_of_beta2):
+#     levels = []
+#     numblobs = []
+#     for _ in range(number_of_experiments):
+#         resG = simulation(n, alpha, 1, beta)
+#         bic_comp=list(nx.biconnected_components(nx.Graph(resG)))
+#         rets_x_bicc=[local_level(resG,b) for b in bic_comp]
+#         level=max(rets_x_bicc)
+#         levels.append(level)
+#         sparse=[1 for x in rets_x_bicc if x!=0]
+#         numblobs.append(sum(sparse))
+#     stats_level2[(n, alpha, beta)] = float(sum(levels))/len(levels)
+#     stats_numblobs2[(n, alpha, beta)] = float(sum(numblobs))/len(numblobs)
+
+
+# # In[ ]:
+
+
+# f = plt.figure()
+# x_positions=range(len(values_of_alpha2))
+# x_axis = values_of_alpha2
+# symbols = "ox*+"
+# i = 0
+# dibs = [None]*4
+# legends = [None]*4
+# for n in [10,30]:
+#     for beta in [0.01,10]:
+#         to_plot = [stats_level2[(n, alpha, beta)] for alpha in values_of_alpha2]
+#         dibs[i]=plt.scatter(x_positions, to_plot, marker = symbols[i], c='black')
+#         legends[i] = "n=%d, beta=%0.2f" % (n, beta)
+#         i += 1
+# plt.xticks(x_positions, x_axis)
+# plt.legend(dibs, legends)
+# plt.xlabel('alpha')
+# plt.ylabel('avg level')
+# plt.show()
+# f.savefig("fig8.pdf", bbox_inches='tight')
+
+
+# # In[ ]:
+
+
+# f = plt.figure()
+# x_positions=range(len(values_of_alpha2))
+# x_axis = values_of_alpha2
+# symbols = "ox*+"
+# i = 0
+# dibs = [None]*4
+# legends = [None]*4
+# for n in [10,30]:
+#     for beta in [0.01,10]:
+#         to_plot = [stats_numblobs2[(n, alpha, beta)] for alpha in values_of_alpha2]
+#         dibs[i]=plt.scatter(x_positions, to_plot, marker = symbols[i], c='black')
+#         legends[i] = "n=%d, beta=%0.2f" % (n, beta)
+#         i += 1
+# plt.xticks(x_positions, x_axis)
+# plt.legend(dibs, legends)
+# plt.xlabel('alpha')
+# plt.ylabel('avg number of nontrivial blobs')
+# plt.show()
+# f.savefig("fig9.pdf", bbox_inches='tight')
+# """
```

### Comparing `phylox-0.0.1/src/phylox/generators/mcmc/base.py` & `phylox-0.0.2/src/phylox/generators/mcmc/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,61 @@
-import networkx as nx
-import numpy as np
 import os
 import sys
-from phylox.isomorphism import count_automorphisms
-from phylox.rearrangement.movetype import MoveType
-from phylox.rearrangement.move import apply_move, Move
-from phylox.rearrangement.invertsequence import from_edge
+
+import networkx as nx
+import numpy as np
+
 from phylox.base import find_unused_node
 from phylox.exceptions import InvalidMoveDefinitionException, InvalidMoveException
+from phylox.isomorphism import count_automorphisms
+from phylox.rearrangement.invertsequence import from_edge
+from phylox.rearrangement.move import Move, apply_move
+from phylox.rearrangement.movetype import MoveType
 
 
 def acceptance_probability(
     network,
     result_network,
     move,
     move_type_probabilities,
     number_of_leaves=None,
     current_reticulation_number=None,
     symmetries=False,
 ):
-    current_reticulation_number = current_reticulation_number or network.reticulation_number
+    current_reticulation_number = (
+        current_reticulation_number or network.reticulation_number
+    )
     number_of_leaves = number_of_leaves or len(network.leaves)
     p = 0
     if move.move_type in [MoveType.TAIL, MoveType.HEAD]:
         p = 1
     if move.move_type == MoveType.VPLU:
-        no_edges_network = float(2 * number_of_leaves + 3 * current_reticulation_number - 1)
+        no_edges_network = float(
+            2 * number_of_leaves + 3 * current_reticulation_number - 1
+        )
         no_edges_network_after = no_edges_network + 3
         p = (
-            (move_type_probabilities[MoveType.VMIN] / move_type_probabilities[MoveType.VPLU])
+            (
+                move_type_probabilities[MoveType.VMIN]
+                / move_type_probabilities[MoveType.VPLU]
+            )
             * no_edges_network**2
             / (no_edges_network_after)
         )
     if move.move_type == MoveType.VMIN:
-        no_edges_network = float(2 * number_of_leaves + 3 * current_reticulation_number - 1)
+        no_edges_network = float(
+            2 * number_of_leaves + 3 * current_reticulation_number - 1
+        )
         no_edges_network_after = no_edges_network - 3
         if no_edges_network > 3:
             p = (
-                (move_type_probabilities[MoveType.VPLU] / move_type_probabilities[MoveType.VMIN])
+                (
+                    move_type_probabilities[MoveType.VPLU]
+                    / move_type_probabilities[MoveType.VMIN]
+                )
                 * no_edges_network
                 / (no_edges_network_after**2)
             )
     if symmetries:
         # correct for number of representations, i.e., symmetries.
         p *= count_automorphisms(network) / count_automorphisms(result_network)
     return p
@@ -95,21 +109,21 @@
                 symmetries=correct_symmetries,
             ):
                 non_moves += 1
                 continue
             if not (restriction_map is None or restriction_map(result_network)):
                 non_moves += 1
                 continue
-            if move.move_type == [MoveType.TAIL, MoveType.HEAD]:
+            if move.move_type in [MoveType.TAIL, MoveType.HEAD]:
                 network = result_network
             if move.move_type == MoveType.VPLU:
                 current_reticulation_number += 1
                 available_tree_nodes.discard(move.start_node)
                 available_reticulations.discard(move.end_node)
                 network = result_network
             if move.move_type == MoveType.VMIN:
                 current_reticulation_number -= 1
                 available_tree_nodes.add(move.removed_edge[0])
                 available_reticulations.add(move.removed_edge[1])
                 network = result_network
         sample.append(network)
-    return sample
+    return sample
```

### Comparing `phylox-0.0.1/src/phylox/generators/randomTC/RandomNetworks.py` & `phylox-0.0.2/src/phylox/generators/randomTC/RandomNetworks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,256 +1,251 @@
-import networkx as nx
-import random
-import matplotlib.pyplot as plt
-import os
-import ast
-import re
-import time
-
-random.seed(a=1234321)
-
-### For the tree child network containment paper by Murakami and Janssen
-
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########                  PHYLOGENETIC NETWORK CLASS               #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-# A class for phylogenetic networks
-class PhN:
-    def __init__(self, seq=None, newick=None):
-        # the actual graph
-        self.nw = nx.DiGraph()
-        # the set of leaf labels of the network
-        self.leaves = set()
-        # a dictionary giving the node for a given leaf label
-        self.labels = dict()
-        # the number of nodes in the graph
-        self.no_nodes = 0
-        self.leaf_nodes = dict()
-        self.TCS = seq
-        self.CPS = seq
-        self.newick = newick
-        self.reducible_pairs = set()
-        self.reticulated_cherries = set()
-        self.cherries = set()
-        if seq:
-            # Creates a phylogenetic network from a cherry picking sequence:
-            for pair in reversed(seq):
-                self.add_pair(*pair)
-
-    def Compute_Leaf_Nodes(self):
-        self.leaf_nodes = dict()
-        for v in self.labels:
-            self.leaf_nodes[self.labels[v]] = v
-
-    # A method for adding a pair, using the construction from a sequence
-    def add_pair(self, x, y):
-        if len(self.leaves) == 0:
-            self.nw.add_edges_from([(0, 1), (1, 2), (1, 3)])
-            self.leaves = set([x, y])
-            self.labels[x] = 2
-            self.labels[y] = 3
-            self.leaf_nodes[2] = x
-            self.leaf_nodes[3] = y
-            self.no_nodes = 4
-            return True
-        if y not in self.leaves:
-            return False
-        node_y = self.labels[y]
-        if x not in self.leaves:
-            self.nw.add_edges_from([(node_y, self.no_nodes), (node_y, self.no_nodes + 1)])
-            self.leaves.add(x)
-            self.leaf_nodes.pop(self.labels[y], False)
-            self.labels[y] = self.no_nodes
-            self.labels[x] = self.no_nodes + 1
-            self.leaf_nodes[self.no_nodes] = y
-            self.leaf_nodes[self.no_nodes + 1] = x
-            self.no_nodes += 2
-        else:
-            node_x = self.labels[x]
-            for parent in self.nw.predecessors(node_x):
-                px = parent
-            if self.nw.in_degree(px) > 1:
-                self.nw.add_edges_from([(node_y, px), (node_y, self.no_nodes)])
-                self.leaf_nodes.pop(self.labels[y], False)
-                self.labels[y] = self.no_nodes
-                self.leaf_nodes[self.no_nodes] = y
-                self.no_nodes += 1
-            else:
-                self.nw.add_edges_from([(node_y, node_x), (node_y, self.no_nodes), (node_x, self.no_nodes + 1)])
-                self.leaf_nodes.pop(self.labels[x], False)
-                self.leaf_nodes.pop(self.labels[y], False)
-                self.labels[y] = self.no_nodes
-                self.labels[x] = self.no_nodes + 1
-                self.leaf_nodes[self.no_nodes] = y
-                self.leaf_nodes[self.no_nodes + 1] = x
-                self.no_nodes += 2
-        return True
-
-
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########                       RANDOM NETWORKS                     #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-# A function that returns a tree-child sequence with a given number of leaves and reticulations
-def random_TC_sequence(leaves, retics):
-    current_leaves = set([1, 2])
-    seq = [(2, 1)]
-    not_forbidden = set([2])
-    leaves_left = leaves - 2
-    retics_left = retics
-
-    # Continue untill we added enough leaves and reticulations
-    while leaves_left > 0 or retics_left > 0:
-        # Decide if we add a leaf, or a reticulation
-        type_added = 'L'
-        if len(not_forbidden) > 0 and leaves_left > 0 and retics_left > 0:
-            if random.randint(0,
-                              leaves_left + retics_left - 1) < retics_left:  # probability of retic depends on number of retics left to add
-                #           if random.randint(0 , 1)<1:                                        #probability of retics and leaves are the same if both are an option
-                type_added = 'R'
-        elif len(not_forbidden) > 0 and retics_left > 0:
-            type_added = 'R'
-        elif leaves_left > 0:
-            type_added = 'L'
-        else:
-            return (False)
-
-        # Actually add the pair
-        if type_added == 'R':
-            first_element = random.choice(list(not_forbidden))
-            retics_left -= 1
-        if type_added == 'L':
-            first_element = len(current_leaves) + 1
-            leaves_left -= 1
-            current_leaves.add(first_element)
-            not_forbidden.add(first_element)
-
-        second_element = random.choice(list(current_leaves - set([first_element])))
-        not_forbidden.discard(second_element)
-        seq.append((first_element, second_element))
-
-    # reverse the sequence, as it was built in reverse order
-    seq = [pair for pair in reversed(seq)]
-    return (seq)
-
-
-# A function that returns a tree-child subsequence with a given number of reticulations
-def random_TC_subsequence(seq, r):
-    # First `uniformly at random' choose one pair per leaf, with that leaf as first element
-    leaves = dict()
-    indices = set()
-    for i, pair in enumerate(seq):
-        x = pair[0]
-        if x not in leaves:
-            indices.add(i)
-            leaves[x] = (1, i)
-        else:
-            if random.randint(0, leaves[x][0]) < 1:
-                indices.remove(leaves[x][1])
-                indices.add(i)
-                leaves[x] = (leaves[x][0] + 1, i)
-            else:
-                leaves[x] = (leaves[x][0] + 1, leaves[x][1])
-    # Add r reticulations with a max of the whole sequence
-    unused = set(range(len(seq))) - indices
-    for j in range(r):
-        new = random.choice(list(unused))
-        unused = unused - set([new])
-        indices.add(new)
-    newSeq = []
-    for i, pair in enumerate(seq):
-        if i in indices:
-            newSeq.append(pair)
-    return newSeq
-
-
-def make_a_lot_of_random_files(folder_name, edges=False):
-    try:
-        os.mkdir("./" + folder_name + "/")
-    except:
-        pass
-    f = open("./" + folder_name + "/hits_and_misses.txt", "w+")
-    f.write("index; subnetwork? \n")
-    f.close()
-    start = time.time()
-
-    maxLeavesRetics = 1000
-    stepLeavesRetics = 25
-    reps = 4
-
-    for leaves in range(stepLeavesRetics, maxLeavesRetics+1,stepLeavesRetics):
-        for reticulations in range(stepLeavesRetics, maxLeavesRetics+1,stepLeavesRetics):
-            for reticulationsSubnetwork in range(stepLeavesRetics, reticulations+1,stepLeavesRetics):
-                for rep in range(reps):
-        
-                    index1 = "0000000" + str(leaves)
-                    index1 = index1[-4:]
-                    index2 = "0000000" + str(reticulations)
-                    index2 = index2[-4:]
-                    index3 = "0000000" + str(reticulationsSubnetwork)
-                    index3 = index3[-4:]
-                    index = "n="+index1+"_k=" + index2+ "_kSub="+index3 + "_rep=" + str(rep)
-        
-                    print(index)
-                    if os.path.isfile("./" + folder_name + "/" + index + ".txt"):
-                        print("already exists")
-                    else:
-                        sequence = random_TC_sequence(leaves, reticulations)
-                        snw_or_not = 'yes'
-                        if rep < reps/2:
-                            subsequence = random_TC_sequence(leaves, reticulations)
-                            snw_or_not = 'no'
-                        else:
-                            subsequence = random_TC_subsequence(sequence, reticulationsSubnetwork)
-                        f = open("./" + folder_name + "/" + index + ".txt", "w+")
-                        if edges:
-                            # build network from sequences
-                            network = PhN(seq=sequence)
-                            subnetwork = PhN(seq=subsequence)
-                            # now change the labels
-                            for node in network.leaf_nodes:
-                                network.leaf_nodes[node] = "L" + str(network.leaf_nodes[node])
-                            for node in subnetwork.leaf_nodes:
-                                subnetwork.leaf_nodes[node] = "L" + str(subnetwork.leaf_nodes[node])
-                            network.nw = nx.relabel_nodes(network.nw, network.leaf_nodes)
-                            subnetwork.nw = nx.relabel_nodes(subnetwork.nw, subnetwork.leaf_nodes)
-                            # Write edges to file
-                            # f.write(str(network.nw.edges)+"\r\n")
-                            f.write(str(network.nw.edges()) + "\r\n")
-                            f.write(str(subnetwork.nw.edges()))
-                        else:
-                            # Write newick to file
-                            f.write(SeqToNewick(sequence) + "\r\n")
-                            f.write(SeqToNewick(subsequence))
-                        f.close()
-                        # write answer to seperate file
-                        f = open("./" + folder_name + "/hits_and_misses.txt", "a+")
-                        f.write(index + " ; " + snw_or_not + "\n")
-                        f.close()
-    end = time.time()
-    print("time elapsed:", end - start, "seconds")
-    
-
-
-
-
-
-
-#Name of the folder to put all input files in
-foldername = "tests"
-#make all the random input files
-make_a_lot_of_random_files(foldername, edges=True)
+# import networkx as nx
+# import random
+# import matplotlib.pyplot as plt
+# import os
+# import ast
+# import re
+# import time
+
+# random.seed(a=1234321)
+
+# ### For the tree child network containment paper by Murakami and Janssen
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########                  PHYLOGENETIC NETWORK CLASS               #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# # A class for phylogenetic networks
+# class PhN:
+#     def __init__(self, seq=None, newick=None):
+#         # the actual graph
+#         self.nw = nx.DiGraph()
+#         # the set of leaf labels of the network
+#         self.leaves = set()
+#         # a dictionary giving the node for a given leaf label
+#         self.labels = dict()
+#         # the number of nodes in the graph
+#         self.no_nodes = 0
+#         self.leaf_nodes = dict()
+#         self.TCS = seq
+#         self.CPS = seq
+#         self.newick = newick
+#         self.reducible_pairs = set()
+#         self.reticulated_cherries = set()
+#         self.cherries = set()
+#         if seq:
+#             # Creates a phylogenetic network from a cherry picking sequence:
+#             for pair in reversed(seq):
+#                 self.add_pair(*pair)
+
+#     def Compute_Leaf_Nodes(self):
+#         self.leaf_nodes = dict()
+#         for v in self.labels:
+#             self.leaf_nodes[self.labels[v]] = v
+
+#     # A method for adding a pair, using the construction from a sequence
+#     def add_pair(self, x, y):
+#         if len(self.leaves) == 0:
+#             self.nw.add_edges_from([(0, 1), (1, 2), (1, 3)])
+#             self.leaves = set([x, y])
+#             self.labels[x] = 2
+#             self.labels[y] = 3
+#             self.leaf_nodes[2] = x
+#             self.leaf_nodes[3] = y
+#             self.no_nodes = 4
+#             return True
+#         if y not in self.leaves:
+#             return False
+#         node_y = self.labels[y]
+#         if x not in self.leaves:
+#             self.nw.add_edges_from([(node_y, self.no_nodes), (node_y, self.no_nodes + 1)])
+#             self.leaves.add(x)
+#             self.leaf_nodes.pop(self.labels[y], False)
+#             self.labels[y] = self.no_nodes
+#             self.labels[x] = self.no_nodes + 1
+#             self.leaf_nodes[self.no_nodes] = y
+#             self.leaf_nodes[self.no_nodes + 1] = x
+#             self.no_nodes += 2
+#         else:
+#             node_x = self.labels[x]
+#             for parent in self.nw.predecessors(node_x):
+#                 px = parent
+#             if self.nw.in_degree(px) > 1:
+#                 self.nw.add_edges_from([(node_y, px), (node_y, self.no_nodes)])
+#                 self.leaf_nodes.pop(self.labels[y], False)
+#                 self.labels[y] = self.no_nodes
+#                 self.leaf_nodes[self.no_nodes] = y
+#                 self.no_nodes += 1
+#             else:
+#                 self.nw.add_edges_from([(node_y, node_x), (node_y, self.no_nodes), (node_x, self.no_nodes + 1)])
+#                 self.leaf_nodes.pop(self.labels[x], False)
+#                 self.leaf_nodes.pop(self.labels[y], False)
+#                 self.labels[y] = self.no_nodes
+#                 self.labels[x] = self.no_nodes + 1
+#                 self.leaf_nodes[self.no_nodes] = y
+#                 self.leaf_nodes[self.no_nodes + 1] = x
+#                 self.no_nodes += 2
+#         return True
+
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########                       RANDOM NETWORKS                     #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# # A function that returns a tree-child sequence with a given number of leaves and reticulations
+# def random_TC_sequence(leaves, retics):
+#     current_leaves = set([1, 2])
+#     seq = [(2, 1)]
+#     not_forbidden = set([2])
+#     leaves_left = leaves - 2
+#     retics_left = retics
+
+#     # Continue untill we added enough leaves and reticulations
+#     while leaves_left > 0 or retics_left > 0:
+#         # Decide if we add a leaf, or a reticulation
+#         type_added = 'L'
+#         if len(not_forbidden) > 0 and leaves_left > 0 and retics_left > 0:
+#             if random.randint(0,
+#                               leaves_left + retics_left - 1) < retics_left:  # probability of retic depends on number of retics left to add
+#                 #           if random.randint(0 , 1)<1:                                        #probability of retics and leaves are the same if both are an option
+#                 type_added = 'R'
+#         elif len(not_forbidden) > 0 and retics_left > 0:
+#             type_added = 'R'
+#         elif leaves_left > 0:
+#             type_added = 'L'
+#         else:
+#             return (False)
+
+#         # Actually add the pair
+#         if type_added == 'R':
+#             first_element = random.choice(list(not_forbidden))
+#             retics_left -= 1
+#         if type_added == 'L':
+#             first_element = len(current_leaves) + 1
+#             leaves_left -= 1
+#             current_leaves.add(first_element)
+#             not_forbidden.add(first_element)
+
+#         second_element = random.choice(list(current_leaves - set([first_element])))
+#         not_forbidden.discard(second_element)
+#         seq.append((first_element, second_element))
+
+#     # reverse the sequence, as it was built in reverse order
+#     seq = [pair for pair in reversed(seq)]
+#     return (seq)
+
+
+# # A function that returns a tree-child subsequence with a given number of reticulations
+# def random_TC_subsequence(seq, r):
+#     # First `uniformly at random' choose one pair per leaf, with that leaf as first element
+#     leaves = dict()
+#     indices = set()
+#     for i, pair in enumerate(seq):
+#         x = pair[0]
+#         if x not in leaves:
+#             indices.add(i)
+#             leaves[x] = (1, i)
+#         else:
+#             if random.randint(0, leaves[x][0]) < 1:
+#                 indices.remove(leaves[x][1])
+#                 indices.add(i)
+#                 leaves[x] = (leaves[x][0] + 1, i)
+#             else:
+#                 leaves[x] = (leaves[x][0] + 1, leaves[x][1])
+#     # Add r reticulations with a max of the whole sequence
+#     unused = set(range(len(seq))) - indices
+#     for j in range(r):
+#         new = random.choice(list(unused))
+#         unused = unused - set([new])
+#         indices.add(new)
+#     newSeq = []
+#     for i, pair in enumerate(seq):
+#         if i in indices:
+#             newSeq.append(pair)
+#     return newSeq
+
+
+# def make_a_lot_of_random_files(folder_name, edges=False):
+#     try:
+#         os.mkdir("./" + folder_name + "/")
+#     except:
+#         pass
+#     f = open("./" + folder_name + "/hits_and_misses.txt", "w+")
+#     f.write("index; subnetwork? \n")
+#     f.close()
+#     start = time.time()
+
+#     maxLeavesRetics = 1000
+#     stepLeavesRetics = 25
+#     reps = 4
+
+#     for leaves in range(stepLeavesRetics, maxLeavesRetics+1,stepLeavesRetics):
+#         for reticulations in range(stepLeavesRetics, maxLeavesRetics+1,stepLeavesRetics):
+#             for reticulationsSubnetwork in range(stepLeavesRetics, reticulations+1,stepLeavesRetics):
+#                 for rep in range(reps):
+
+#                     index1 = "0000000" + str(leaves)
+#                     index1 = index1[-4:]
+#                     index2 = "0000000" + str(reticulations)
+#                     index2 = index2[-4:]
+#                     index3 = "0000000" + str(reticulationsSubnetwork)
+#                     index3 = index3[-4:]
+#                     index = "n="+index1+"_k=" + index2+ "_kSub="+index3 + "_rep=" + str(rep)
+
+#                     print(index)
+#                     if os.path.isfile("./" + folder_name + "/" + index + ".txt"):
+#                         print("already exists")
+#                     else:
+#                         sequence = random_TC_sequence(leaves, reticulations)
+#                         snw_or_not = 'yes'
+#                         if rep < reps/2:
+#                             subsequence = random_TC_sequence(leaves, reticulations)
+#                             snw_or_not = 'no'
+#                         else:
+#                             subsequence = random_TC_subsequence(sequence, reticulationsSubnetwork)
+#                         f = open("./" + folder_name + "/" + index + ".txt", "w+")
+#                         if edges:
+#                             # build network from sequences
+#                             network = PhN(seq=sequence)
+#                             subnetwork = PhN(seq=subsequence)
+#                             # now change the labels
+#                             for node in network.leaf_nodes:
+#                                 network.leaf_nodes[node] = "L" + str(network.leaf_nodes[node])
+#                             for node in subnetwork.leaf_nodes:
+#                                 subnetwork.leaf_nodes[node] = "L" + str(subnetwork.leaf_nodes[node])
+#                             network.nw = nx.relabel_nodes(network.nw, network.leaf_nodes)
+#                             subnetwork.nw = nx.relabel_nodes(subnetwork.nw, subnetwork.leaf_nodes)
+#                             # Write edges to file
+#                             # f.write(str(network.nw.edges)+"\r\n")
+#                             f.write(str(network.nw.edges()) + "\r\n")
+#                             f.write(str(subnetwork.nw.edges()))
+#                         else:
+#                             # Write newick to file
+#                             f.write(SeqToNewick(sequence) + "\r\n")
+#                             f.write(SeqToNewick(subsequence))
+#                         f.close()
+#                         # write answer to seperate file
+#                         f = open("./" + folder_name + "/hits_and_misses.txt", "a+")
+#                         f.write(index + " ; " + snw_or_not + "\n")
+#                         f.close()
+#     end = time.time()
+#     print("time elapsed:", end - start, "seconds")
+
+
+# #Name of the folder to put all input files in
+# foldername = "tests"
+# #make all the random input files
+# make_a_lot_of_random_files(foldername, edges=True)
```

### Comparing `phylox-0.0.1/src/phylox/generators/zods/zods.py` & `phylox-0.0.2/src/phylox/generators/zods/zods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,159 +1,151 @@
-import numpy as np
-import random
-import networkx as nx
-import sys
-
-
-##PARAMETERS
-time_limit = 0.2
-speciation_rate = 20.0
-hybridization_rate = 1.0
-inheritence = True
-edges = True
-##
-
-
-
-###############################2. I/O############################
-
-i = 1
-while i < len(sys.argv):
-    arg= sys.argv[i]
-    if arg == "-t":
-        i+=1
-        time_limit = float(sys.argv[i])
-    if arg == "-sp":
-        i+=1
-        speciation_rate = float(sys.argv[i])
-    if arg == "-hyb":
-        i+=1
-        hybridization_rate = float(sys.argv[i])
-    if arg == "-no_inheritence":
-        inheritence = False
-    i += 1
-
-
-
-
-
-
-
-nw = nx.DiGraph()
-nw.add_node(0)
-leaves = set([0])
-current_node = 1
-
-extra_time = np.random.exponential(1/float(speciation_rate))
-current_time = extra_time
-current_speciation_rate    = float(speciation_rate)
-current_hybridization_rate = float(0)
-rate = current_speciation_rate + current_hybridization_rate
-
-#First create a MUL-tree
-hybrid_nodes=dict()
-no_of_hybrids = 0
-
-while current_time<time_limit:
-    if random.random() < current_speciation_rate / rate:
-        #speciate
-        splitting_leaf = random.choice(list(leaves))
-        nw.add_weighted_edges_from([(splitting_leaf,current_node,0),(splitting_leaf,current_node+1,0)], weight = 'length')
-        leaves.remove(splitting_leaf)
-        leaves.add(current_node)
-        leaves.add(current_node+1)
-        current_node+=2
-    else:
-        #Hybridize
-	#i.e.: pick two leaf nodes, merge those, and add a new leaf below this hybrid node.
-        merging = random.sample(leaves,2)
-        l0 = merging[0]
-        l1 = merging[1]
-        pl0 = -1
-        for p in nw.predecessors(l0):
-            pl0=p
-        pl1 = -1
-        for p in nw.predecessors(l1):
-            pl1=p
-        #If pl0==pl1, the new hybridization results in parallel edges.
-        if pl0 != pl1:
-            no_of_hybrids+=1
-            nw.add_weighted_edges_from([(l0,current_node,0)],weight = 'length')
-            leaves.remove(l0)
-            leaves.remove(l1)
-            leaves.add(current_node)
-            prob = random.random()
-            nw[pl0][l0]['prob'] = prob
-            nw[pl1][l1]['prob'] = 1-prob
-            hybrid_nodes[l0]=no_of_hybrids
-            hybrid_nodes[l1]=no_of_hybrids
-            current_node+=1 
-    #Now extend all pendant edges
-    for l in leaves:
-        pl = -1
-        for p in nw.predecessors(l):
-            pl = p
-        nw[pl][l]['length']+=extra_time
-    no_of_leaves = len(leaves)
-    current_speciation_rate    = float(speciation_rate*no_of_leaves)
-    current_hybridization_rate = float(hybridization_rate * (no_of_leaves * (no_of_leaves - 1))/2)
-    rate = current_speciation_rate + current_hybridization_rate
-    extra_time    = np.random.exponential(1/rate)
-    current_time += extra_time
-
-
-extra_time -= current_time-time_limit
-#nothing has happened yet, and there is only one node
-if len(nw) == 1:
-    nw.add_weighted_edges_from([(0,1,time_limit)],weight = 'length')
-    leaves = set([1])
-# each leaf has a parent node, and we can extend each parent edge to time_limit
-else:
-    for l in leaves:
-        pl = -1
-        for p in nw.predecessors(l):
-            pl = p
-        nw[pl][l]['length']+=extra_time
-
-
-############### NOW CONVERT TO NEWICK ##############
-
-def Newick_From_MULTree(tree,root,hybrid_nodes):
-    if tree.out_degree(root)==0:
-        if root in hybrid_nodes:
-            return "#H"+str(hybrid_nodes[root])
-        return str(root)
-    Newick = ""
-    for v in tree.successors(root):
-        Newick+= Newick_From_MULTree(tree,v,hybrid_nodes)+":"+str(tree[root][v]['length'])
-        if inheritence:
-            if v in hybrid_nodes:
-                Newick+="::"+str(tree[root][v]['prob'])
-        Newick+= ","
-    Newick = "("+Newick[:-1]+")"
-    if root in hybrid_nodes:
-        Newick += "#H"+str(hybrid_nodes[root])
-    return Newick
-
-
-print(Newick_From_MULTree(nw,0,hybrid_nodes)+";")
-inheritence = False
-print(Newick_From_MULTree(nw,0,hybrid_nodes)+";")
-if edges:
-    for e in nw.edges(data=True):
-        info = ""
-        if e[0] in hybrid_nodes:
-            info += "#H"+str(hybrid_nodes[e[0]])
-        else:
-            info += str(e[0])
-        info += ","
-        if e[1] in hybrid_nodes:
-            info += "#H"+str(hybrid_nodes[e[1]])
-        else:
-            info += str(e[1])
-        info += ","
-        info += str(e[2]['length']) + ",1.0" 
-        if 'prob' in e[2]:
-            info = info[:-3] + str(e[2]['prob'])
-        print(info) 
-
-
+# import numpy as np
+# import random
+# import networkx as nx
+# import sys
+
+
+# ##PARAMETERS
+# time_limit = 0.2
+# speciation_rate = 20.0
+# hybridization_rate = 1.0
+# inheritence = True
+# edges = True
+# ##
+
+
+# ###############################2. I/O############################
+
+# i = 1
+# while i < len(sys.argv):
+#     arg= sys.argv[i]
+#     if arg == "-t":
+#         i+=1
+#         time_limit = float(sys.argv[i])
+#     if arg == "-sp":
+#         i+=1
+#         speciation_rate = float(sys.argv[i])
+#     if arg == "-hyb":
+#         i+=1
+#         hybridization_rate = float(sys.argv[i])
+#     if arg == "-no_inheritence":
+#         inheritence = False
+#     i += 1
+
+
+# nw = nx.DiGraph()
+# nw.add_node(0)
+# leaves = set([0])
+# current_node = 1
+
+# extra_time = np.random.exponential(1/float(speciation_rate))
+# current_time = extra_time
+# current_speciation_rate    = float(speciation_rate)
+# current_hybridization_rate = float(0)
+# rate = current_speciation_rate + current_hybridization_rate
+
+# #First create a MUL-tree
+# hybrid_nodes=dict()
+# no_of_hybrids = 0
+
+# while current_time<time_limit:
+#     if random.random() < current_speciation_rate / rate:
+#         #speciate
+#         splitting_leaf = random.choice(list(leaves))
+#         nw.add_weighted_edges_from([(splitting_leaf,current_node,0),(splitting_leaf,current_node+1,0)], weight = 'length')
+#         leaves.remove(splitting_leaf)
+#         leaves.add(current_node)
+#         leaves.add(current_node+1)
+#         current_node+=2
+#     else:
+#         #Hybridize
+# 	#i.e.: pick two leaf nodes, merge those, and add a new leaf below this hybrid node.
+#         merging = random.sample(leaves,2)
+#         l0 = merging[0]
+#         l1 = merging[1]
+#         pl0 = -1
+#         for p in nw.predecessors(l0):
+#             pl0=p
+#         pl1 = -1
+#         for p in nw.predecessors(l1):
+#             pl1=p
+#         #If pl0==pl1, the new hybridization results in parallel edges.
+#         if pl0 != pl1:
+#             no_of_hybrids+=1
+#             nw.add_weighted_edges_from([(l0,current_node,0)],weight = 'length')
+#             leaves.remove(l0)
+#             leaves.remove(l1)
+#             leaves.add(current_node)
+#             prob = random.random()
+#             nw[pl0][l0]['prob'] = prob
+#             nw[pl1][l1]['prob'] = 1-prob
+#             hybrid_nodes[l0]=no_of_hybrids
+#             hybrid_nodes[l1]=no_of_hybrids
+#             current_node+=1
+#     #Now extend all pendant edges
+#     for l in leaves:
+#         pl = -1
+#         for p in nw.predecessors(l):
+#             pl = p
+#         nw[pl][l]['length']+=extra_time
+#     no_of_leaves = len(leaves)
+#     current_speciation_rate    = float(speciation_rate*no_of_leaves)
+#     current_hybridization_rate = float(hybridization_rate * (no_of_leaves * (no_of_leaves - 1))/2)
+#     rate = current_speciation_rate + current_hybridization_rate
+#     extra_time    = np.random.exponential(1/rate)
+#     current_time += extra_time
+
+
+# extra_time -= current_time-time_limit
+# #nothing has happened yet, and there is only one node
+# if len(nw) == 1:
+#     nw.add_weighted_edges_from([(0,1,time_limit)],weight = 'length')
+#     leaves = set([1])
+# # each leaf has a parent node, and we can extend each parent edge to time_limit
+# else:
+#     for l in leaves:
+#         pl = -1
+#         for p in nw.predecessors(l):
+#             pl = p
+#         nw[pl][l]['length']+=extra_time
+
+
+# ############### NOW CONVERT TO NEWICK ##############
+
+# def Newick_From_MULTree(tree,root,hybrid_nodes):
+#     if tree.out_degree(root)==0:
+#         if root in hybrid_nodes:
+#             return "#H"+str(hybrid_nodes[root])
+#         return str(root)
+#     Newick = ""
+#     for v in tree.successors(root):
+#         Newick+= Newick_From_MULTree(tree,v,hybrid_nodes)+":"+str(tree[root][v]['length'])
+#         if inheritence:
+#             if v in hybrid_nodes:
+#                 Newick+="::"+str(tree[root][v]['prob'])
+#         Newick+= ","
+#     Newick = "("+Newick[:-1]+")"
+#     if root in hybrid_nodes:
+#         Newick += "#H"+str(hybrid_nodes[root])
+#     return Newick
+
+
+# print(Newick_From_MULTree(nw,0,hybrid_nodes)+";")
+# inheritence = False
+# print(Newick_From_MULTree(nw,0,hybrid_nodes)+";")
+# if edges:
+#     for e in nw.edges(data=True):
+#         info = ""
+#         if e[0] in hybrid_nodes:
+#             info += "#H"+str(hybrid_nodes[e[0]])
+#         else:
+#             info += str(e[0])
+#         info += ","
+#         if e[1] in hybrid_nodes:
+#             info += "#H"+str(hybrid_nodes[e[1]])
+#         else:
+#             info += str(e[1])
+#         info += ","
+#         info += str(e[2]['length']) + ",1.0"
+#         if 'prob' in e[2]:
+#             info = info[:-3] + str(e[2]['prob'])
+#         print(info)
```

### Comparing `phylox-0.0.1/src/phylox/isomorphism/base.py` & `phylox-0.0.2/src/phylox/isomorphism/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,43 @@
+from copy import deepcopy
+
 import networkx as nx
+
 from phylox.dinetwork import LABEL_ATTR
-from copy import deepcopy
 
-ISOMETRY_LABEL_ATTR = 'isometry_label'
+ISOMETRY_LABEL_ATTR = "isometry_label"
 ISOMETRY_LABEL_TAG = "isometry_label_tag_"
 AUTOMORPHISM_LABEL_TAG = "automorphism_label_tag_"
 
 # Checks whether the nodes with the given attributes have the same label
 def same_isometry_labels(node1_attributes, node2_attributes):
     """
     Checks whether two nodes have the same label
 
     :param node1_attributes: the attributes of a node
     :param node2_attributes: the attributes of a node
     :return: True if the isometry label attribute ISOMETRY_LABEL_ATTR is the same, False otherwise.
     """
-    return node1_attributes.get(ISOMETRY_LABEL_ATTR) == node2_attributes.get(ISOMETRY_LABEL_ATTR)
+    return node1_attributes.get(ISOMETRY_LABEL_ATTR) == node2_attributes.get(
+        ISOMETRY_LABEL_ATTR
+    )
 
 
 # Checks whether the nodes with the given attributes have the same label
 def same_isometry_labels_and_labels(node1_attributes, node2_attributes):
     """
     Checks whether two nodes have the same label
 
     :param node1_attributes: the attributes of a node
     :param node2_attributes: the attributes of a node
     :return: True if the isometry label attribute ISOMETRY_LABEL_ATTR is the same, False otherwise.
     """
-    return node1_attributes.get(ISOMETRY_LABEL_ATTR) == node2_attributes.get(ISOMETRY_LABEL_ATTR) and \
-           node1_attributes.get(LABEL_ATTR) == node2_attributes.get(LABEL_ATTR)
+    return node1_attributes.get(ISOMETRY_LABEL_ATTR) == node2_attributes.get(
+        ISOMETRY_LABEL_ATTR
+    ) and node1_attributes.get(LABEL_ATTR) == node2_attributes.get(LABEL_ATTR)
 
 
 # Checks whether two networks are labeled isomorpgic
 def is_isomorphic(network1, network2, partial_isomorphism=None, ignore_labels=False):
     """
     Determines whether two networks are labeled isomorphic.
 
@@ -53,16 +58,21 @@
             return False
         nw1.nodes[corr[0]][ISOMETRY_LABEL_ATTR] = f"{ISOMETRY_LABEL_TAG}{i}"
         nw2.nodes[corr[1]][ISOMETRY_LABEL_ATTR] = f"{ISOMETRY_LABEL_TAG}{i}"
 
     return nx.is_isomorphic(nw1, nw2, node_match=same_labels)
 
 
-
-def _count_automorphisms(network, ignore_labels=False, partial_isomorphism=None, nodes_available=None, nodes_to_do=None):
+def _count_automorphisms(
+    network,
+    ignore_labels=False,
+    partial_isomorphism=None,
+    nodes_available=None,
+    nodes_to_do=None,
+):
     """
     Determines the number of automorphisms of a network.
 
     :param network: a phylogenetic network, i.e., a DAG with leaf labels.
     :param ignore_labels: if True, the automorphisms are counted without considering the labels of the nodes.
     :param partial_isomorphism: a partial isomorphism between the network and itself.
     :param nodes_available: the nodes that are available to be matched.
@@ -80,31 +90,33 @@
     while nodes_to_do:
         node_pair_to_remove = partial_isomorphism.pop()
         node_to_remove = node_pair_to_remove[0]
         nodes_to_do.remove(node_to_remove)
         matches = 1
         for try_to_match_node in nodes_available:
             if is_isomorphic(
-                network, 
-                network, 
-                partial_isomorphism=partial_isomorphism+[(node_to_remove, try_to_match_node)],
-                ignore_labels=ignore_labels
+                network,
+                network,
+                partial_isomorphism=partial_isomorphism
+                + [(node_to_remove, try_to_match_node)],
+                ignore_labels=ignore_labels,
             ):
                 matches += 1
         number_of_automorphisms *= matches
         nodes_available.append(node_to_remove)
     return number_of_automorphisms
 
+
 def count_automorphisms(network, ignore_labels=False):
     """
     Determines the number of automorphisms of a network.
 
     :param network: a phylogenetic network, i.e., a DAG with leaf labels.
     :param ignore_labels: if True, the automorphisms are counted without considering the labels of the nodes.
     :return: the number of automorphisms of the network.
     """
-    partial_isomorphism = [(a,a) for a in network.nodes()]
+    partial_isomorphism = [(a, a) for a in network.nodes()]
     return _count_automorphisms(
-        network, 
-        ignore_labels=ignore_labels, 
+        network,
+        ignore_labels=ignore_labels,
         partial_isomorphism=partial_isomorphism,
     )
```

### Comparing `phylox-0.0.1/src/phylox/networkproperties/properties.py` & `phylox-0.0.2/src/phylox/networkproperties/properties.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,89 @@
-def LeavesAndReticNumber(network):
-    """returns the number of leaves and reticulations in the network"""
-    num_r = 0
-    num_l = 0
-    for node in network.nodes():
-        if network.in_degree(node)>1:
-            num_r+=network.in_degree(node)-1
-        if network.out_degree(node)==0:
-            num_l+=1
-    return num_l,num_r
-
-def ReduciblePairs(network):
-    """returns the number of reducible pairs in the network
-    split up by number of cherries and number of reticulated cherries.
-    """
-    cherries            = []
-    reticulate_cherries = [] 
-    for node in network.nodes:
-        if network.out_degree(node)==0:
-            pair = IsSecondInPair(network,node)
-            if pair!=False:
-                for parent in network.predecessors(pair[0]):
-                    if network.out_degree(parent)==1:
-                        reticulate_cherries += [pair]
-                        break
-                else:
-                    cherries += [pair]
-    return(len(cherries)/2,len(reticulate_cherries))
-
-
-def BlobProperties(network):
-    """returns a list of all blobs of the network and their properties.
-    Each blob is a pair (blob_size, blob_level) where blob_size is the 
-    number of nodes in the blob and blob_level is the number of 
-    reticulations in the blob.
-    """
-    blob_properties = []
-    #For each biconnected component
-    for bicomponent in nx.biconnected_components(network.to_undirected()):
-        #A bicomponent is a blob if it consists of at least 2 nodes
-        if len(bicomponent)>2:
-#            blob = network.subgraph(bicomponent)
-            #count reticulations in blob
-            retics = 0
-            for node in bicomponent:
-                if network.in_degree(node)==2:
-                    retics+=1
-            blob_size = len(bicomponent)
-            blob_level = retics
-            blob_properties+=[(blob_size, blob_level)]
-    return blob_properties
-
-
-def B_2_Balance(network):
-    """returns the B_2 balance of the network"""
-    balance = 0
-    
-    #Initiate probabilities
-    root                = Root(network)
-    probabilities       = dict()
-    probabilities[root] = 1
-    highest_nodes       = []
-    for node in network.successors(root):
-        if network.in_degree(node)==1:
-            highest_nodes+=[node]
-    
-    
-    #Calculate the probabilities of reaching each node with a uniform random directed walk
-    while highest_nodes:
-        current_node = highest_nodes.pop()
-        # Calculate the probability of current_node
-        prob = 0
-        for parent in network.predecessors(current_node):
-            prob+= (1/float(network.out_degree(parent)))*probabilities[parent]
-        probabilities[current_node]=prob
-        
-        # Update the set of highest nodes
-        for child in network.successors(current_node):
-            for parent in network.predecessors(child):
-                if parent not in probabilities:
-                    break            
-            else:
-                highest_nodes+=[child]
-        
-        #
-        if network.out_degree(current_node)==0:
-            balance-=prob*math.log(prob, 2)
-              
-        
-    return balance
+# def LeavesAndReticNumber(network):
+#     """returns the number of leaves and reticulations in the network"""
+#     num_r = 0
+#     num_l = 0
+#     for node in network.nodes():
+#         if network.in_degree(node) > 1:
+#             num_r += network.in_degree(node) - 1
+#         if network.out_degree(node) == 0:
+#             num_l += 1
+#     return num_l, num_r
+
+
+# def ReduciblePairs(network):
+#     """returns the number of reducible pairs in the network
+#     split up by number of cherries and number of reticulated cherries.
+#     """
+#     cherries = []
+#     reticulate_cherries = []
+#     for node in network.nodes:
+#         if network.out_degree(node) == 0:
+#             pair = IsSecondInPair(network, node)
+#             if pair != False:
+#                 for parent in network.predecessors(pair[0]):
+#                     if network.out_degree(parent) == 1:
+#                         reticulate_cherries += [pair]
+#                         break
+#                 else:
+#                     cherries += [pair]
+#     return (len(cherries) / 2, len(reticulate_cherries))
+
+
+# def BlobProperties(network):
+#     """returns a list of all blobs of the network and their properties.
+#     Each blob is a pair (blob_size, blob_level) where blob_size is the
+#     number of nodes in the blob and blob_level is the number of
+#     reticulations in the blob.
+#     """
+#     blob_properties = []
+#     # For each biconnected component
+#     for bicomponent in nx.biconnected_components(network.to_undirected()):
+#         # A bicomponent is a blob if it consists of at least 2 nodes
+#         if len(bicomponent) > 2:
+#             #            blob = network.subgraph(bicomponent)
+#             # count reticulations in blob
+#             retics = 0
+#             for node in bicomponent:
+#                 if network.in_degree(node) == 2:
+#                     retics += 1
+#             blob_size = len(bicomponent)
+#             blob_level = retics
+#             blob_properties += [(blob_size, blob_level)]
+#     return blob_properties
+
+
+# def B_2_Balance(network):
+#     """returns the B_2 balance of the network"""
+#     balance = 0
+
+#     # Initiate probabilities
+#     root = Root(network)
+#     probabilities = dict()
+#     probabilities[root] = 1
+#     highest_nodes = []
+#     for node in network.successors(root):
+#         if network.in_degree(node) == 1:
+#             highest_nodes += [node]
+
+#     # Calculate the probabilities of reaching each node with a uniform random directed walk
+#     while highest_nodes:
+#         current_node = highest_nodes.pop()
+#         # Calculate the probability of current_node
+#         prob = 0
+#         for parent in network.predecessors(current_node):
+#             prob += (1 / float(network.out_degree(parent))) * probabilities[parent]
+#         probabilities[current_node] = prob
+
+#         # Update the set of highest nodes
+#         for child in network.successors(current_node):
+#             for parent in network.predecessors(child):
+#                 if parent not in probabilities:
+#                     break
+#             else:
+#                 highest_nodes += [child]
+
+#         #
+#         if network.out_degree(current_node) == 0:
+#             balance -= prob * math.log(prob, 2)
+
+#     return balance
```

### Comparing `phylox-0.0.1/src/phylox/parser.py` & `phylox-0.0.2/src/phylox/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,211 +1,198 @@
-import os
-import sys
-import math
-import re
-import ast
-import random
-import numpy as np
-import pandas as pd
-from pathlib import Path
-import multiprocessing
-from multiprocessing import Manager
-from ExtractNetworkProperties import *
-import itertools
-
-
-
-
-def Newick_To_Network(newick):
-    newick=newick[:-1]
-
-    #remove internal labels
-    newick = re.sub(r"I([\d]+)", "", newick)
-
-    #remove lengths
-    newick = re.sub(r"([\d]+)\.([\d]+)", "", newick)
-    newick = re.sub(r"E-[\d]+", "", newick)
-    newick = re.sub(r":", "", newick)
-
-    #make into list format
-    newick = newick.replace("(","[")
-    newick = newick.replace(")","]")
-    newick = re.sub(r"\]\#H([\d]+)", r",#R\1]", newick)
-    newick = re.sub(r"#([RH])([\d]+)", r"'#\1\2'", newick)
-
-
-    #add "" if necessary    
-    newick = re.sub(r"([ABCD])", r"'\1'", newick)
-    newick = re.sub(r" ", "", newick)
-    
-    
-    nestedtree = ast.literal_eval(newick)
-    edges, leaves, label_set, current_node = NestedList_To_Tree(nestedtree,1)
-    edges.append([0,1])
-    ret_labels = dict()
-    leaf_labels = dict()
-    for l in leaves:
-        if len(l)>2 and (l[:2]=="#H" or l[:2]=="#R"):
-            ret_labels[l[2:]]=[]
-        else:
-            leaf_labels[l]=[]
-    for l in label_set:
-        if len(l[0])>2 and (l[0][:2]=="#H" or l[0][:2]=="#R"):
-            if l[0][1]=='H':
-                ret_labels[l[0][2:]]+=[l[1]]
-            else:
-                ret_labels[l[0][2:]]=[l[1]]+ret_labels[l[0][2:]]
-        else:
-            leaf_labels[l[0]]+=[l[1]]
-    network = nx.DiGraph()        
-    network.add_edges_from(edges)
-    for retic in ret_labels:
-        r = ret_labels[retic]
-        receiving = r[0]
-        parent_receiving = 0
-        for p in network.predecessors(receiving):
-            parent_receiving = p
-        network.remove_node(receiving)
-        for v in r[1:]:
-            network.add_edge(v,parent_receiving)
-            network = nx.contracted_edge(network,(v,parent_receiving))
-            network.remove_edge(v,v)
-            parent_receiving = v
-    leaves = set()
-    for l in leaf_labels:
-         leaf_labels[l]=leaf_labels[l][0]
-         leaves.add(l)
-    return network, leaves, leaf_labels
-    
-    
-def NestedList_To_Tree(nestedList,next_node):
-    edges = []
-    leaves = set()
-    labels = []
-    top_node = next_node
-    current_node = next_node+1
-    for t in nestedList:
-        edges.append((top_node,current_node))
-        if type(t)==list: 
-            extra_edges, extra_leaves, extra_labels, current_node = NestedList_To_Tree(t,current_node)
-        else: 
-            extra_edges = []
-            extra_leaves = set([str(t)])
-            extra_labels = [[str(t), current_node]]
-            current_node+=1
-        edges = edges + extra_edges
-        leaves = leaves.union(extra_leaves)
-        labels = labels + extra_labels
-    return edges, leaves, labels, current_node
-
-
-
-
-network,_,leaf_labels = Newick_To_Network(newick_string)
-reverse_labels = {x:y for (y,x) in leaf_labels.items()}
-
-
-
-
-
-
-
-
-
-
-
-################################################################################
-################################################################################
-################################################################################
-########                                                           #############
-########                         I/O Functions                     #############
-########                                                           #############
-################################################################################
-################################################################################
-################################################################################
-
-
-########
-######## Convert Newick to a networkx Digraph with labels (and branch lengths)
-########
-# Write length newick: convert ":" to "," and then evaluate as list of lists using ast.literal_eval
-# Then, in each list, the node is followed by the length of the incoming arc.
-# This only works as long as each branch has length and all internal nodes are labeled.
-def Newick_To_Network(newick):
-    """
-    Converts a Newick string to a networkx DAG with leaf labels.
-
-    :param newick: a string in extended Newick format for phylogenetic networks.
-    :return: a phylogenetic network, i.e., a networkx digraph with leaf labels represented by the `label' node attribute.
-    """
-    # Ignore the ';'
-    newick = newick[:-1]
-    # If names are not in string format between ', add these.
-    if not "'" in newick and not '"' in newick:
-        newick = re.sub(r"\)#H([\d]+)", r",#R\1)", newick)
-        newick = re.sub(r"([,\(])([#a-zA-Z\d]+)", r"\1'\2", newick)
-        newick = re.sub(r"([#a-zA-Z\d])([,\(\)])", r"\1'\2", newick)
-    else:
-        newick = re.sub(r"\)#H([d]+)", r"'#R\1'\)", newick)
-    newick = newick.replace("(", "[")
-    newick = newick.replace(")", "]")
-    nestedtree = ast.literal_eval(newick)
-    edges, current_node = NestedList_To_Network(nestedtree, 0, 1)
-    network = nx.DiGraph()
-    network.add_edges_from(edges)
-    network = NetworkLeafToLabel(network)
-    return network
-
-
-# Returns a network in which the leaves have the original name as label, and all nodes have integer names.
-def NetworkLeafToLabel(network):
-    """
-    Renames the network nodes to integers, while storing the original node names in the `original' node attribute.
-
-    :param network: a phylogenetic network
-    :return: a phylogenetic network with original node names in the `original' node attribute.
-    """
-    for node in network.nodes():
-        if network.out_degree(node) == 0:
-            network.node[node]['label'] = node
-    return nx.convert_node_labels_to_integers(network, first_label=0, label_attribute='original')
-
-
-# Auxiliary function to convert list of lists to graph
-def NestedList_To_Network(nestedList, top_node, next_node):
-    """
-    Auxiliary function used to convert list of lists to graph.
-
-    :param nestedList: a nested list.
-    :param top_node: an integer, the node name of the top node of the network represented by the list.
-    :param next_node: an integer, the lowest integer not yet used as node name in the network.
-    :return: a set of edges of the network represented by the nested list, and an updated next_node.
-    """
-    edges = []
-    if type(nestedList) == list:
-        if type(nestedList[-1]) == str and len(nestedList[-1]) > 2 and nestedList[-1][:2] == '#R':
-            retic_node = '#H' + nestedList[-1][2:]
-            bottom_node = retic_node
-        else:
-            bottom_node = next_node
-            next_node += 1
-        edges.append((top_node, bottom_node))
-        for t in nestedList:
-            extra_edges, next_node = NestedList_To_Network(t, bottom_node, next_node)
-            edges = edges + extra_edges
-    else:
-        if not (len(nestedList) > 2 and nestedList[:2] == '#R'):
-            edges = [(top_node, nestedList)]
-    return edges, next_node
-
-
-# Sets the labels of the nodes of a network with a given label dictionary
-def Set_Labels(network, label_dict):
-    """
-    Sets the labels of the leaves of a network using a dictionary of labels.
-
-    :param network: a networkx digraph, a DAG.
-    :param label_dict: a dictionary, containing the labels (values) of the nodes of the network (keys).
-    :return: a phylogenetic network, obtained by labeling network with the labels.
-    """
-    for node, value in label_dict.items():
-        network.node[node]['label'] = value
+# import os
+# import sys
+# import math
+# import re
+# import ast
+# import random
+# import numpy as np
+# import pandas as pd
+# from pathlib import Path
+# import multiprocessing
+# from multiprocessing import Manager
+# from ExtractNetworkProperties import *
+# import itertools
+
+
+# def Newick_To_Network(newick):
+#     newick=newick[:-1]
+
+#     #remove internal labels
+#     newick = re.sub(r"I([\d]+)", "", newick)
+
+#     #remove lengths
+#     newick = re.sub(r"([\d]+)\.([\d]+)", "", newick)
+#     newick = re.sub(r"E-[\d]+", "", newick)
+#     newick = re.sub(r":", "", newick)
+
+#     #make into list format
+#     newick = newick.replace("(","[")
+#     newick = newick.replace(")","]")
+#     newick = re.sub(r"\]\#H([\d]+)", r",#R\1]", newick)
+#     newick = re.sub(r"#([RH])([\d]+)", r"'#\1\2'", newick)
+
+
+#     #add "" if necessary
+#     newick = re.sub(r"([ABCD])", r"'\1'", newick)
+#     newick = re.sub(r" ", "", newick)
+
+
+#     nestedtree = ast.literal_eval(newick)
+#     edges, leaves, label_set, current_node = NestedList_To_Tree(nestedtree,1)
+#     edges.append([0,1])
+#     ret_labels = dict()
+#     leaf_labels = dict()
+#     for l in leaves:
+#         if len(l)>2 and (l[:2]=="#H" or l[:2]=="#R"):
+#             ret_labels[l[2:]]=[]
+#         else:
+#             leaf_labels[l]=[]
+#     for l in label_set:
+#         if len(l[0])>2 and (l[0][:2]=="#H" or l[0][:2]=="#R"):
+#             if l[0][1]=='H':
+#                 ret_labels[l[0][2:]]+=[l[1]]
+#             else:
+#                 ret_labels[l[0][2:]]=[l[1]]+ret_labels[l[0][2:]]
+#         else:
+#             leaf_labels[l[0]]+=[l[1]]
+#     network = nx.DiGraph()
+#     network.add_edges_from(edges)
+#     for retic in ret_labels:
+#         r = ret_labels[retic]
+#         receiving = r[0]
+#         parent_receiving = 0
+#         for p in network.predecessors(receiving):
+#             parent_receiving = p
+#         network.remove_node(receiving)
+#         for v in r[1:]:
+#             network.add_edge(v,parent_receiving)
+#             network = nx.contracted_edge(network,(v,parent_receiving))
+#             network.remove_edge(v,v)
+#             parent_receiving = v
+#     leaves = set()
+#     for l in leaf_labels:
+#          leaf_labels[l]=leaf_labels[l][0]
+#          leaves.add(l)
+#     return network, leaves, leaf_labels
+
+
+# def NestedList_To_Tree(nestedList,next_node):
+#     edges = []
+#     leaves = set()
+#     labels = []
+#     top_node = next_node
+#     current_node = next_node+1
+#     for t in nestedList:
+#         edges.append((top_node,current_node))
+#         if type(t)==list:
+#             extra_edges, extra_leaves, extra_labels, current_node = NestedList_To_Tree(t,current_node)
+#         else:
+#             extra_edges = []
+#             extra_leaves = set([str(t)])
+#             extra_labels = [[str(t), current_node]]
+#             current_node+=1
+#         edges = edges + extra_edges
+#         leaves = leaves.union(extra_leaves)
+#         labels = labels + extra_labels
+#     return edges, leaves, labels, current_node
+
+
+# network,_,leaf_labels = Newick_To_Network(newick_string)
+# reverse_labels = {x:y for (y,x) in leaf_labels.items()}
+
+
+# ################################################################################
+# ################################################################################
+# ################################################################################
+# ########                                                           #############
+# ########                         I/O Functions                     #############
+# ########                                                           #############
+# ################################################################################
+# ################################################################################
+# ################################################################################
+
+
+# ########
+# ######## Convert Newick to a networkx Digraph with labels (and branch lengths)
+# ########
+# # Write length newick: convert ":" to "," and then evaluate as list of lists using ast.literal_eval
+# # Then, in each list, the node is followed by the length of the incoming arc.
+# # This only works as long as each branch has length and all internal nodes are labeled.
+# def Newick_To_Network(newick):
+#     """
+#     Converts a Newick string to a networkx DAG with leaf labels.
+
+#     :param newick: a string in extended Newick format for phylogenetic networks.
+#     :return: a phylogenetic network, i.e., a networkx digraph with leaf labels represented by the `label' node attribute.
+#     """
+#     # Ignore the ';'
+#     newick = newick[:-1]
+#     # If names are not in string format between ', add these.
+#     if not "'" in newick and not '"' in newick:
+#         newick = re.sub(r"\)#H([\d]+)", r",#R\1)", newick)
+#         newick = re.sub(r"([,\(])([#a-zA-Z\d]+)", r"\1'\2", newick)
+#         newick = re.sub(r"([#a-zA-Z\d])([,\(\)])", r"\1'\2", newick)
+#     else:
+#         newick = re.sub(r"\)#H([d]+)", r"'#R\1'\)", newick)
+#     newick = newick.replace("(", "[")
+#     newick = newick.replace(")", "]")
+#     nestedtree = ast.literal_eval(newick)
+#     edges, current_node = NestedList_To_Network(nestedtree, 0, 1)
+#     network = nx.DiGraph()
+#     network.add_edges_from(edges)
+#     network = NetworkLeafToLabel(network)
+#     return network
+
+
+# # Returns a network in which the leaves have the original name as label, and all nodes have integer names.
+# def NetworkLeafToLabel(network):
+#     """
+#     Renames the network nodes to integers, while storing the original node names in the `original' node attribute.
+
+#     :param network: a phylogenetic network
+#     :return: a phylogenetic network with original node names in the `original' node attribute.
+#     """
+#     for node in network.nodes():
+#         if network.out_degree(node) == 0:
+#             network.node[node]['label'] = node
+#     return nx.convert_node_labels_to_integers(network, first_label=0, label_attribute='original')
+
+
+# # Auxiliary function to convert list of lists to graph
+# def NestedList_To_Network(nestedList, top_node, next_node):
+#     """
+#     Auxiliary function used to convert list of lists to graph.
+
+#     :param nestedList: a nested list.
+#     :param top_node: an integer, the node name of the top node of the network represented by the list.
+#     :param next_node: an integer, the lowest integer not yet used as node name in the network.
+#     :return: a set of edges of the network represented by the nested list, and an updated next_node.
+#     """
+#     edges = []
+#     if type(nestedList) == list:
+#         if type(nestedList[-1]) == str and len(nestedList[-1]) > 2 and nestedList[-1][:2] == '#R':
+#             retic_node = '#H' + nestedList[-1][2:]
+#             bottom_node = retic_node
+#         else:
+#             bottom_node = next_node
+#             next_node += 1
+#         edges.append((top_node, bottom_node))
+#         for t in nestedList:
+#             extra_edges, next_node = NestedList_To_Network(t, bottom_node, next_node)
+#             edges = edges + extra_edges
+#     else:
+#         if not (len(nestedList) > 2 and nestedList[:2] == '#R'):
+#             edges = [(top_node, nestedList)]
+#     return edges, next_node
+
+
+# # Sets the labels of the nodes of a network with a given label dictionary
+# def Set_Labels(network, label_dict):
+#     """
+#     Sets the labels of the leaves of a network using a dictionary of labels.
+
+#     :param network: a networkx digraph, a DAG.
+#     :param label_dict: a dictionary, containing the labels (values) of the nodes of the network (keys).
+#     :return: a phylogenetic network, obtained by labeling network with the labels.
+#     """
+#     for node, value in label_dict.items():
+#         network.node[node]['label'] = value
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/exact_distance/base.py` & `phylox-0.0.2/src/phylox/rearrangement/exact_distance/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-def Depth_First(network1, network2, tail_moves=True, head_moves=True, max_time=False, show_bounds=True):
-    """
-    An implementation of Algorithm 1. Uses an iterated Depth First Search to simulate a Breath First Search.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param tail_moves: a boolean value determining whether tail moves are used.
-    :param head_moves: a boolean value determining whether head moves are used.
-    :param max_time: a float, a time limit for the function in seconds. If False, no time limit is used, and the function continues until it finds a sequence.
-    :param show_bounds: a boolean parameter, if True the current lower bounds are printed to the terminal, used for debugging.
-    :return: a shortest sequence of moves between the networks if it is found within the time limit, otherwise it returns an integer: a lower bound for the length of teh shortest sequence between the networks.
-    """
-    done = False
-    lower_bound = 0
-    stop_time = False
-    if max_time:
-        stop_time = time.time() + max_time
-    while not done:
-        output = Depth_First_Bounded(network1, network2, tail_moves=tail_moves, head_moves=head_moves,
-                                     max_depth=lower_bound, stop_time=stop_time)
-        if output == "timeout":
-            return lower_bound
-        elif type(output) == list:
-            return output
-        lower_bound += 1
-        if show_bounds:
-            print(lower_bound)
-
-
-# Finds a shortest sequence between network1 and network2 using DFS with bounded depth
-def Depth_First_Bounded(network1, network2, tail_moves=True, head_moves=True, max_depth=0, stop_time=False):
-    """
-    An subroutine of Algorithm 1. A depth-bounded Depth First Search used to simulate a Breath First Search.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param tail_moves: a boolean value determining whether tail moves are used.
-    :param head_moves: a boolean value determining whether head moves are used.
-    :param max_depth: a integer, the maximum depth for the search tree.
-    :param stop_time: a float, a time limit for the function in clock time. If False, no time limit is used, and the function continues until it finds a sequence.
-    :return: a shortest sequence of at most max_depth moves between the networks if it is found before the stop_time, otherwise it returns an False.
-    """
-    # If we cannot do any moves:
-    if not tail_moves and not head_moves:
-        if Isomorphic(network1, network2):
-            return 0
-        else:
-            return False
-    # Else, make a stack and search
-    stack = [[]]
-    while stack:
-        current_moves = stack.pop()
-        current_length = len(current_moves)
-        current_network = network1
-        for move in current_moves:
-            current_network = DoMove(current_network, *move)
-        if current_length == max_depth and Isomorphic(current_network, network2):
-            return current_moves
-        if current_length < max_depth:
-            validMoves = AllValidMoves(current_network, tail_moves=tail_moves, head_moves=head_moves)
-            for move in validMoves:
-                stack.append(current_moves + [move])
-        if stop_time and time.time() > stop_time:
-            return "timeout"
-    return False
-
-
-# Finds a shortest sequence between network1 and network2 using BFS
-def Breadth_First(network1, network2, tail_moves=True, head_moves=True, max_time=False):
-    """
-    A true BFS implementation to find a shortest sequence between two networks. This implementation uses too much memory, use Depth_First!
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param tail_moves: a boolean value determining whether tail moves are used.
-    :param head_moves: a boolean value determining whether head moves are used.
-    :param max_time: a float, a time limit for the function in seconds. If False, no time limit is used, and the function continues until it finds a sequence.
-    :return: a shortest sequence of moves between the networks if it is found within the time limit, otherwise it returns an integer: a lower bound for the length of teh shortest sequence between the networks.
-    """
-    # If we cannot do any moves:
-    if not tail_moves and not head_moves:
-        if Isomorphic(network1, network2):
-            return 0
-        else:
-            return False
-    # Else, make a queue and search
-    queue = deque([[]])
-    start_time = time.time()
-    while queue:
-        current_moves = queue.popleft()
-        current_network = network1
-        for move in current_moves:
-            current_network = DoMove(current_network, *move)
-        if Isomorphic(current_network, network2):
-            return current_moves
-        validMoves = AllValidMoves(current_network, tail_moves=tail_moves, head_moves=head_moves)
-        for move in validMoves:
-            queue.append(current_moves + [move])
-        if max_time and time.time() - start_time > max_time:
-            return len(current_moves)
-    return False
+# def Depth_First(network1, network2, tail_moves=True, head_moves=True, max_time=False, show_bounds=True):
+#     """
+#     An implementation of Algorithm 1. Uses an iterated Depth First Search to simulate a Breath First Search.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param tail_moves: a boolean value determining whether tail moves are used.
+#     :param head_moves: a boolean value determining whether head moves are used.
+#     :param max_time: a float, a time limit for the function in seconds. If False, no time limit is used, and the function continues until it finds a sequence.
+#     :param show_bounds: a boolean parameter, if True the current lower bounds are printed to the terminal, used for debugging.
+#     :return: a shortest sequence of moves between the networks if it is found within the time limit, otherwise it returns an integer: a lower bound for the length of teh shortest sequence between the networks.
+#     """
+#     done = False
+#     lower_bound = 0
+#     stop_time = False
+#     if max_time:
+#         stop_time = time.time() + max_time
+#     while not done:
+#         output = Depth_First_Bounded(network1, network2, tail_moves=tail_moves, head_moves=head_moves,
+#                                      max_depth=lower_bound, stop_time=stop_time)
+#         if output == "timeout":
+#             return lower_bound
+#         elif type(output) == list:
+#             return output
+#         lower_bound += 1
+#         if show_bounds:
+#             print(lower_bound)
+
+
+# # Finds a shortest sequence between network1 and network2 using DFS with bounded depth
+# def Depth_First_Bounded(network1, network2, tail_moves=True, head_moves=True, max_depth=0, stop_time=False):
+#     """
+#     An subroutine of Algorithm 1. A depth-bounded Depth First Search used to simulate a Breath First Search.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param tail_moves: a boolean value determining whether tail moves are used.
+#     :param head_moves: a boolean value determining whether head moves are used.
+#     :param max_depth: a integer, the maximum depth for the search tree.
+#     :param stop_time: a float, a time limit for the function in clock time. If False, no time limit is used, and the function continues until it finds a sequence.
+#     :return: a shortest sequence of at most max_depth moves between the networks if it is found before the stop_time, otherwise it returns an False.
+#     """
+#     # If we cannot do any moves:
+#     if not tail_moves and not head_moves:
+#         if Isomorphic(network1, network2):
+#             return 0
+#         else:
+#             return False
+#     # Else, make a stack and search
+#     stack = [[]]
+#     while stack:
+#         current_moves = stack.pop()
+#         current_length = len(current_moves)
+#         current_network = network1
+#         for move in current_moves:
+#             current_network = DoMove(current_network, *move)
+#         if current_length == max_depth and Isomorphic(current_network, network2):
+#             return current_moves
+#         if current_length < max_depth:
+#             validMoves = AllValidMoves(current_network, tail_moves=tail_moves, head_moves=head_moves)
+#             for move in validMoves:
+#                 stack.append(current_moves + [move])
+#         if stop_time and time.time() > stop_time:
+#             return "timeout"
+#     return False
+
+
+# # Finds a shortest sequence between network1 and network2 using BFS
+# def Breadth_First(network1, network2, tail_moves=True, head_moves=True, max_time=False):
+#     """
+#     A true BFS implementation to find a shortest sequence between two networks. This implementation uses too much memory, use Depth_First!
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param tail_moves: a boolean value determining whether tail moves are used.
+#     :param head_moves: a boolean value determining whether head moves are used.
+#     :param max_time: a float, a time limit for the function in seconds. If False, no time limit is used, and the function continues until it finds a sequence.
+#     :return: a shortest sequence of moves between the networks if it is found within the time limit, otherwise it returns an integer: a lower bound for the length of teh shortest sequence between the networks.
+#     """
+#     # If we cannot do any moves:
+#     if not tail_moves and not head_moves:
+#         if Isomorphic(network1, network2):
+#             return 0
+#         else:
+#             return False
+#     # Else, make a queue and search
+#     queue = deque([[]])
+#     start_time = time.time()
+#     while queue:
+#         current_moves = queue.popleft()
+#         current_network = network1
+#         for move in current_moves:
+#             current_network = DoMove(current_network, *move)
+#         if Isomorphic(current_network, network2):
+#             return current_moves
+#         validMoves = AllValidMoves(current_network, tail_moves=tail_moves, head_moves=head_moves)
+#         for move in validMoves:
+#             queue.append(current_moves + [move])
+#         if max_time and time.time() - start_time > max_time:
+#             return len(current_moves)
+#     return False
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/heuristics/cli_main.py` & `phylox-0.0.2/src/phylox/rearrangement/heuristics/cli_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,194 @@
-# These functions are implementations of the algorithms of Remie Janssen's PhD thesis
-
-from __future__ import print_function
-import networkx as nx
-from RearrDistance_Tools import *
-import ast
-import os
-import sys
-import re
-import time
-
-##PARAMETERS
-filename = None
-edges = False
-tailMoves = True
-headMoves = True
-bfSearch = False
-simple=False
-time_limit=False
-repeats=1
-runtime=False
-deep_dive=False
-randomNodes=False
-##
-
-
-
-###############################2. I/O############################
-option_help = False
-i = 1
-while i < len(sys.argv):
-    arg= sys.argv[i]
-    if arg == "-f" or arg == "--filename":
-        i+=1
-        filename = str(sys.argv[i])
-    if arg == "-tl" or arg == "--timelimit":
-        i+=1
-        time_limit = float(sys.argv[i])
-    if arg == "-e" or arg == "--edges":
-        edges = True
-    if arg == "-t" or arg == "--tail":
-        headMoves = False
-    if arg == "-h" or arg == "--head":
-        tailMoves = False
-    if arg == "-bfs" or arg == "--bfsearch":
-        bfSearch = True
-    if arg == "-dd" or arg == "--deepdive":
-        deep_dive = True    
-    if arg == "-s" or arg == "--simple":
-        simple = True
-    if arg == "-rt" or arg == "--runtime":
-        runtime = True
-    if arg == "-r" or arg == "--random":
-        randomNodes = True
-    if arg == "-rep" or arg == "--repeats":
-        i+=1
-        repeats = int(sys.argv[i])        
-    if arg == "-help" or arg == "--help":
-        option_help = True
-    i += 1
-
-if len(sys.argv)==1 or option_help or (deep_dive and bfSearch):
-    print("Mandatory arguments:\n -f or --filename followed by the filename of the file containing two networks \n\nOptional arguments:\n -e or --edges if the input file contains a list of edges in the form [(x1,y1),...,(xn,yn)] with xi and yi integers or strings in the form \"string\". If this option is not selected, the input is assumed to consist of two newick strings.\n -t or --tail for only using tail moves, instead of tail and head moves.\n -h or --head for only using head moves, instead of tail and head moves.\n -r or --random to pick random nodes whenever arbitrary nodes are required in the heuristics.\n -rt or --runtime to also record the runtime of the algorithm and the time to read the trees from file.\n -bfs or --bfsearch for using a breadth first search to find the an optimal sequence.\n -tl or --timelimit followed by a number of seconds to set a timelimit for the bfs. If no answer is found before the time runs out, the algorithm just returns a lower bound on the distance.\n\nThe output is given as a list of moves in the format:\n  moving_edge, moving_endpoint, to_edge")
-    sys.exit()
-
-
-
-
-####################################################
-####################################################
-####################################################
-#############                          #############
-#############           MAIN           #############
-#############                          #############
-####################################################
-####################################################
-####################################################
-
-
-if runtime:
-    time_start_reading = time.time()
-
-test = open(filename, "r")
-line1 = test.read()
-line1 = line1.split("\n")
-test.close()
-if edges:
-    N = nx.DiGraph()
-    M = nx.DiGraph()
-    N.add_edges_from(ast.literal_eval(line1[0]))
-    M.add_edges_from(ast.literal_eval(line1[1]))
-    rootN=Root(N)
-    if N.out_degree(rootN)==2:
-       N.add_edges_from([('rho',rootN)])
-    rootM=Root(M)
-    if M.out_degree(rootM)==2:
-       M.add_edges_from([('rho',rootM)])
-    N = NetworkLeafToLabel(N)
-    M = NetworkLeafToLabel(M)
-    label_attribute=None
-else:
-    N = Newick_To_Network(line1[0])
-    M = Newick_To_Network(line1[1])
-    if not simple:
-        print("The networks as list of edges, with node names as used in the computed sequence of moves")
-        print("Network 1:")
-        for e in N.edges():
-            label = N.node[e[1]].get('label')
-            if label:
-                print(str(e[0])+" "+str(e[1])+" = leaf: "+str(label))
-            else:
-                print(str(e[0])+" "+str(e[1]))
-        print("Network 2:")
-        for e in M.edges():
-            label = M.node[e[1]].get('label')
-            if label:
-                print(str(e[0])+" "+str(e[1])+" = leaf: "+str(label))
-            else:
-                print(str(e[0])+" "+str(e[1]))
-
-
-if runtime:
-    time_start_searching = time.time()
-
-
-if bfSearch:
-    if not simple:
-        print("Computing a shortest sequence using breadth first search.")
-        #Note, the code uses a DFS with incremented depth bound
-        #Otherwise, the queue gets too large for memory
-    sequence = Depth_First(N,M,tail_moves=tailMoves,head_moves=headMoves,max_time=time_limit,show_bounds=(not simple))
-elif deep_dive:
-    if not simple:
-        print("Computing a shortest sequence by passing the depth first search tree once, choosing the best branch (according to the GL algorithm) each time.")
-        #Note, the code uses a DFS with incremented depth bound
-        #Otherwise, the queue gets too large for memory
-    sequence = Deep_Dive_Scored(N,M,head_moves=headMoves)
-
-
-else:
-    if not tailMoves:
-        if not simple:
-            print("Computing a sequence using the `red-line' heuristic.")
-        if randomNodes:
-            if not simple:
-                print("Picking random nodes whenever arbitrary nodes are required.")
-            sequence = Red_Line_Random(N,M,repeats=repeats)
-        else:
-            sequence = Red_Line(N,M)
-    else: 
-        if not simple:
-            print("Computing a sequence using the `green-line' heuristic.")
-        if randomNodes:
-            if not simple:
-                print("Picking random nodes whenever arbitrary nodes are required.")
-            sequence = Green_Line_Random(N,M,head_moves=headMoves,repeats=repeats) 
-        else: 
-            sequence = Green_Line(N,M,head_moves=headMoves) 
-            
-if runtime:
-    time_stop_searching = time.time()
-    if simple:
-        print(";"+str(time_start_searching-time_start_reading)+";"+str(time_stop_searching-time_start_searching),end='')
-    else:
-        print("Reading the networks cost "+str(time_start_searching-time_start_reading)+" seconds.")
-        print("Finding the sequence cost "+str(time_stop_searching-time_start_searching)+" seconds.")
-
-
-
-           
-            
-if not simple:
-    print("Sequence:")
-if sequence==False:
-    if not simple:
-        print("There is no sequence between the networks.")
-    else:
-        print(";None;None",end='')
-    sys.exit()
-if type(sequence)==int:
-    if simple:
-        print(";>="+str(sequence)+";?",end='')
-    else:
-        print("No network was found within the time limit.")
-        print("The distance between the networks is at least: "+str(sequence))
-    sys.exit()
-if edges:
-    sequence = ReplaceNodeNamesByOriginal(N,sequence)
-    
-#Print the output 
-
-   
-if simple:
-    print(";"+str(len(sequence))+";"+str(sequence),end='')    
-else:
-    for move in sequence:
-        if len(move)==4:
-            print(str(move[0])+" "+str(move[1])+" "+str(move[3]))    
-        if len(move)==3:
-            print(str(move[0])+" "+str(move[1])+" "+str(move[2]))    
-    
-    
+# # These functions are implementations of the algorithms of Remie Janssen's PhD thesis
 
+# from __future__ import print_function
+# import networkx as nx
+# from RearrDistance_Tools import *
+# import ast
+# import os
+# import sys
+# import re
+# import time
+
+# ##PARAMETERS
+# filename = None
+# edges = False
+# tailMoves = True
+# headMoves = True
+# bfSearch = False
+# simple=False
+# time_limit=False
+# repeats=1
+# runtime=False
+# deep_dive=False
+# randomNodes=False
+# ##
+
+
+# ###############################2. I/O############################
+# option_help = False
+# i = 1
+# while i < len(sys.argv):
+#     arg= sys.argv[i]
+#     if arg == "-f" or arg == "--filename":
+#         i+=1
+#         filename = str(sys.argv[i])
+#     if arg == "-tl" or arg == "--timelimit":
+#         i+=1
+#         time_limit = float(sys.argv[i])
+#     if arg == "-e" or arg == "--edges":
+#         edges = True
+#     if arg == "-t" or arg == "--tail":
+#         headMoves = False
+#     if arg == "-h" or arg == "--head":
+#         tailMoves = False
+#     if arg == "-bfs" or arg == "--bfsearch":
+#         bfSearch = True
+#     if arg == "-dd" or arg == "--deepdive":
+#         deep_dive = True
+#     if arg == "-s" or arg == "--simple":
+#         simple = True
+#     if arg == "-rt" or arg == "--runtime":
+#         runtime = True
+#     if arg == "-r" or arg == "--random":
+#         randomNodes = True
+#     if arg == "-rep" or arg == "--repeats":
+#         i+=1
+#         repeats = int(sys.argv[i])
+#     if arg == "-help" or arg == "--help":
+#         option_help = True
+#     i += 1
+
+# if len(sys.argv)==1 or option_help or (deep_dive and bfSearch):
+#     print("Mandatory arguments:\n -f or --filename followed by the filename of the file containing two networks \n\nOptional arguments:\n -e or --edges if the input file contains a list of edges in the form [(x1,y1),...,(xn,yn)] with xi and yi integers or strings in the form \"string\". If this option is not selected, the input is assumed to consist of two newick strings.\n -t or --tail for only using tail moves, instead of tail and head moves.\n -h or --head for only using head moves, instead of tail and head moves.\n -r or --random to pick random nodes whenever arbitrary nodes are required in the heuristics.\n -rt or --runtime to also record the runtime of the algorithm and the time to read the trees from file.\n -bfs or --bfsearch for using a breadth first search to find the an optimal sequence.\n -tl or --timelimit followed by a number of seconds to set a timelimit for the bfs. If no answer is found before the time runs out, the algorithm just returns a lower bound on the distance.\n\nThe output is given as a list of moves in the format:\n  moving_edge, moving_endpoint, to_edge")
+#     sys.exit()
+
+
+# ####################################################
+# ####################################################
+# ####################################################
+# #############                          #############
+# #############           MAIN           #############
+# #############                          #############
+# ####################################################
+# ####################################################
+# ####################################################
+
+
+# if runtime:
+#     time_start_reading = time.time()
+
+# test = open(filename, "r")
+# line1 = test.read()
+# line1 = line1.split("\n")
+# test.close()
+# if edges:
+#     N = nx.DiGraph()
+#     M = nx.DiGraph()
+#     N.add_edges_from(ast.literal_eval(line1[0]))
+#     M.add_edges_from(ast.literal_eval(line1[1]))
+#     rootN=Root(N)
+#     if N.out_degree(rootN)==2:
+#        N.add_edges_from([('rho',rootN)])
+#     rootM=Root(M)
+#     if M.out_degree(rootM)==2:
+#        M.add_edges_from([('rho',rootM)])
+#     N = NetworkLeafToLabel(N)
+#     M = NetworkLeafToLabel(M)
+#     label_attribute=None
+# else:
+#     N = Newick_To_Network(line1[0])
+#     M = Newick_To_Network(line1[1])
+#     if not simple:
+#         print("The networks as list of edges, with node names as used in the computed sequence of moves")
+#         print("Network 1:")
+#         for e in N.edges():
+#             label = N.node[e[1]].get('label')
+#             if label:
+#                 print(str(e[0])+" "+str(e[1])+" = leaf: "+str(label))
+#             else:
+#                 print(str(e[0])+" "+str(e[1]))
+#         print("Network 2:")
+#         for e in M.edges():
+#             label = M.node[e[1]].get('label')
+#             if label:
+#                 print(str(e[0])+" "+str(e[1])+" = leaf: "+str(label))
+#             else:
+#                 print(str(e[0])+" "+str(e[1]))
+
+
+# if runtime:
+#     time_start_searching = time.time()
+
+
+# if bfSearch:
+#     if not simple:
+#         print("Computing a shortest sequence using breadth first search.")
+#         #Note, the code uses a DFS with incremented depth bound
+#         #Otherwise, the queue gets too large for memory
+#     sequence = Depth_First(N,M,tail_moves=tailMoves,head_moves=headMoves,max_time=time_limit,show_bounds=(not simple))
+# elif deep_dive:
+#     if not simple:
+#         print("Computing a shortest sequence by passing the depth first search tree once, choosing the best branch (according to the GL algorithm) each time.")
+#         #Note, the code uses a DFS with incremented depth bound
+#         #Otherwise, the queue gets too large for memory
+#     sequence = Deep_Dive_Scored(N,M,head_moves=headMoves)
+
+
+# else:
+#     if not tailMoves:
+#         if not simple:
+#             print("Computing a sequence using the `red-line' heuristic.")
+#         if randomNodes:
+#             if not simple:
+#                 print("Picking random nodes whenever arbitrary nodes are required.")
+#             sequence = Red_Line_Random(N,M,repeats=repeats)
+#         else:
+#             sequence = Red_Line(N,M)
+#     else:
+#         if not simple:
+#             print("Computing a sequence using the `green-line' heuristic.")
+#         if randomNodes:
+#             if not simple:
+#                 print("Picking random nodes whenever arbitrary nodes are required.")
+#             sequence = Green_Line_Random(N,M,head_moves=headMoves,repeats=repeats)
+#         else:
+#             sequence = Green_Line(N,M,head_moves=headMoves)
+
+# if runtime:
+#     time_stop_searching = time.time()
+#     if simple:
+#         print(";"+str(time_start_searching-time_start_reading)+";"+str(time_stop_searching-time_start_searching),end='')
+#     else:
+#         print("Reading the networks cost "+str(time_start_searching-time_start_reading)+" seconds.")
+#         print("Finding the sequence cost "+str(time_stop_searching-time_start_searching)+" seconds.")
+
+
+# if not simple:
+#     print("Sequence:")
+# if sequence==False:
+#     if not simple:
+#         print("There is no sequence between the networks.")
+#     else:
+#         print(";None;None",end='')
+#     sys.exit()
+# if type(sequence)==int:
+#     if simple:
+#         print(";>="+str(sequence)+";?",end='')
+#     else:
+#         print("No network was found within the time limit.")
+#         print("The distance between the networks is at least: "+str(sequence))
+#     sys.exit()
+# if edges:
+#     sequence = ReplaceNodeNamesByOriginal(N,sequence)
+
+# #Print the output
+
+
+# if simple:
+#     print(";"+str(len(sequence))+";"+str(sequence),end='')
+# else:
+#     for move in sequence:
+#         if len(move)==4:
+#             print(str(move[0])+" "+str(move[1])+" "+str(move[3]))
+#         if len(move)==3:
+#             print(str(move[0])+" "+str(move[1])+" "+str(move[2]))
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/heuristics/green_line_heuristic.py` & `phylox-0.0.2/src/phylox/rearrangement/heuristics/green_line_heuristic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,476 +1,476 @@
-def GL_Case1_rSPR(N, Np, up, isom_N_Np, isom_Np_N, randomNodes=False):
-    """
-    An implementation of Algorithm 2. Finds a sequence of rSPR moves that makes it possible to add the lowest reticulation up to the down-closed isomrophism.
-
-    :param N: a phylogenetic network.
-    :param Np: a phylogenetic network.
-    :param up: a lowest reticulation node of Np above the isomorphism.
-    :param isom_N_Np: a dictionary, containing a partial (down-closed) isomorphism map from N to Np. The inverse of isom_Np_N.
-    :param isom_Np_N: a dictionary, containing a partial (down-closed) isomorphism map from Np to N. The inverse of isom_N_Np.
-    :param randomNodes: a boolean value, determining whether the random version of this lemma is used.
-    :return: a list of rSPR moves in N, a list of rSPR moves in Np, a node of N, a node of Np. After performing the lists of moves on the networks, the nodes can be added to the isomorphism.
-    """
-    # use notation as in the paper
-    # ' is denoted p
-    xp = Child(Np, up)
-    x = isom_Np_N[xp]
-    z = Parent(N, x, exclude=isom_N_Np.keys(), randomNodes=randomNodes)
-
-    # Case1a: z is a reticulation
-    if N.in_degree(z) == 2:
-        return [], [], z, up
-    # Case1b: z is not a reticulation
-    # Find a retic v in N not in the isom yet
-    v = FindRetic(N, excludedSet=isom_N_Np.keys(), randomNodes=randomNodes)
-    u = None
-    for parent in N.predecessors(v):
-        if CheckValid(N, (parent, v), v, (z, x)):
-            if not randomNodes:
-                u = parent
-                break
-            elif u == None or random.getrandbits(1):
-                u = parent
-    # If v has an incoming arc (u,v) movable to (z,x), perform this move
-    if u != None:
-        return [((u, v), v, (z, x))], [], v, up
-    # if none of the moves is valid, this must be because
-    # v is already a reticulation above x with its movable incoming arc (u,v) with u=z.
-    return [], [], v, up
-
-
-def GL_Case1_Tail(N, Np, up, isom_N_Np, isom_Np_N, randomNodes=False):
-    """
-    An implementation of Algorithm 6. Finds a sequence of tail moves that makes it possible to add the lowest reticulation up to the down-closed isomrophism.
-
-    :param N: a phylogenetic network.
-    :param Np: a phylogenetic network.
-    :param up: a lowest reticulation node of Np above the isomorphism.
-    :param isom_N_Np: a dictionary, containing a partial (down-closed) isomorphism map from N to Np. The inverse of isom_Np_N.
-    :param isom_Np_N: a dictionary, containing a partial (down-closed) isomorphism map from Np to N. The inverse of isom_N_Np.
-    :param randomNodes: a boolean value, determining whether the random version of this lemma is used.
-    :return: a list of tail moves in N, a list of tail moves in Np, a node of N, a node of Np. After performing the lists of moves on the networks, the nodes can be added to the isomorphism. Returns false if the networks are not isomorphic with 2 leaves and 1 reticulation.
-    """
-    # use notation as in the paper
-    # ' is denoted p
-    xp = Child(Np, up)
-    x = isom_Np_N[xp]
-    z = Parent(N, x, exclude=isom_N_Np.keys(), randomNodes=randomNodes)
-    # Case1a: z is a reticulation
-    if N.in_degree(z) == 2:
-        return [], [], z, up
-    # Case1b: z is not a reticulation
-    # z is a tree node
-    if check_movable(N, (z, x), z):
-        # Case1bi: (z,x) is movable
-        # Find a reticulation u in N not in the isomorphism yet
-        # TODO: Can first check if the other parent of x suffices here, should heuristcally be better
-        u = FindRetic(N, excludedSet=isom_N_Np.keys(), randomNodes=randomNodes)
-        v = Child(N, u)
-        if v == x:
-            return [], [], u, up
-        # we may now assume v!=x
-        if z == v:
-            v = Child(N, z, exclude=[x])
-            w = Parent(N, u, randomNodes=randomNodes)
-            return [((z, v), z, (w, u))], [], u, up
-        w = Parent(N, u, exclude=[z], randomNodes=randomNodes)
-        return [((z, x), z, (u, v)), ((z, v), z, (w, u))], [], u, up
-    # Case1bii: (z,x) is not movable
-    c = Parent(N, z)
-    d = Child(N, z, exclude=[x])
-    # TODO: b does not have to exist if we have an outdeg-2 root, this could be c!
-    b = Parent(N, c)
-    if N.in_degree(b) != 0:
-        # Case1biiA: b is not the root of N
-        a = Parent(N, b, randomNodes=randomNodes)
-        # First do the move ((c,d),c,(a,b)), then Case1bi applies as (z,x) is now movable
-        newN = DoMove(N, (c, d), c, (a, b))
-        u = FindRetic(newN, excludedSet=isom_N_Np.keys(), randomNodes=randomNodes)
-        v = Child(newN, u)
-        if v == x:
-            # In this case, u is a reticulation parent of x and u is not in the isom. Hence, we can simply add it to the isom.
-            # Note: The tail move we did is not necessary!
-            # TODO: First check both parents of x for being a reticulation not in the isomorphism yet
-            return [], [], u, up
-        # we may now assume v!=x
-        if z == v:
-            # This only happens if z==v and u==b
-            # we move z up above the retic b as well, too
-            w = Parent(newN, b, randomNodes=randomNodes)
-            return [((c, d), c, (a, b)), ((z, d), z, (w, b))], [], u, up
-        w = Parent(newN, u, exclude=[z], randomNodes=randomNodes)
-        return [((c, d), c, (a, b)), ((z, x), z, (u, v)), ((z, v), z, (w, u))], [], u, up
-    # Case1biiB: b is the root of N
-    # Note: d is not in the isomorphism
-    e = Child(N, d)
-    if e == x:
-        return [], [], d, up
-    if N.out_degree(x) == 2:
-        s = Child(N, x)
-        t = Child(N, x, exclude=[s])
-        if s == e:
-            return [((x, t), x, (d, e))], [], d, up
-        if t == e:
-            return [((x, s), x, (d, e))], [], d, up
-        return [((x, s), x, (d, e)), ((x, e), x, (z, t)), ((x, t), x, (d, s))], [], d, up
-    if N.out_degree(e) == 2:
-        s = Child(N, e)
-        t = Child(N, e, exclude=[s])
-        if s == x:
-            return [((e, t), e, (z, x))], [], d, up
-        if t == x:
-            return [((e, s), e, (z, x))], [], d, up
-        return [((e, s), e, (z, x)), ((e, x), e, (d, t)), ((e, t), e, (z, s))], [], d, up
-    # neither are tree nodes, so both must be leaves
-    # In that case, there is no sequence between the two networks.
-    return [], [], None, None
-
-
-def GL_Case3(N, Np, up, isom_N_Np, isom_Np_N, randomNodes=False):
-    """
-    An implementation of Algorithm 3. Finds a sequence of tail moves that makes it possible to add the lowest tree node up to the down-closed isomrophism.
-
-    :param N: a phylogenetic network.
-    :param Np: a phylogenetic network.
-    :param up: a lowest tree node of Np above the isomorphism.
-    :param isom_N_Np: a dictionary, containing a partial (down-closed) isomorphism map from N to Np. The inverse of isom_Np_N.
-    :param isom_Np_N: a dictionary, containing a partial (down-closed) isomorphism map from Np to N. The inverse of isom_N_Np.
-    :param randomNodes: a boolean value, determining whether the random version of this lemma is used.
-    :return: a list of tail moves in N, a list of tail moves in Np, a node of N, a node of Np. After performing the lists of moves on the networks, the nodes can be added to the isomorphism.
-    """
-    # Find the children x' and y' of u'
-    xp, yp = list(Np.successors(up))
-    # Find the corresponding nodes x and y in N
-    x = isom_Np_N[xp]
-    y = isom_Np_N[yp]
-    # Find the set of common parents of x and y
-    parents_x = set(N.predecessors(x))
-    parents_y = set(N.predecessors(y))
-    common_parents = parents_x & parents_y
-    # Case3a: x and y have a common parent not in the isom
-    common_parents_not_Y = []
-    for parent in common_parents:
-        if parent not in isom_N_Np.keys():
-            # then parent can be mapped to up
-            common_parents_not_Y += [parent]
-            if not randomNodes:
-                return [], [], parent, up
-    if common_parents_not_Y:
-        return [], [], random.choice(common_parents_not_Y), up
-
-    # Case3b: x and y do not have a common parent in the isomorphism
-    # For both, find a parent not in the isomorphism yet
-    # TODO: preferably make them tree nodes
-    z_x = Parent(N, x, exclude=isom_N_Np.keys(), randomNodes=randomNodes)
-    z_y = Parent(N, y, exclude=isom_N_Np.keys(), randomNodes=randomNodes)
-
-    # Case3bi: (z_x,x) is movable
-    if CheckValid(N, (z_x, x), z_x, (z_y, y)):
-        return [((z_x, x), z_x, (z_y, y))], [], z_x, up
-    # Case3bii: (z_y,y) is movable
-    if CheckValid(N, (z_y, y), z_y, (z_x, x)):
-        return [((z_y, y), z_y, (z_x, x))], [], z_y, up
-    # Case3biii: Neither (z_x,x) nor (z_y,y) is movable
-
-    if N.in_degree(z_x) == 2 or N.in_degree(z_y) == 2:
-        return [], [], None, None
-    # Both these parents are tree nodes.
-    # This happens always in the non-random version, as otherwise there is a lowest reticulation node and we would be in Case 1 or 2.
-
-    # As both nodes are tree nodes and the arcs immovable, both arcs hang of the side of a triangle.
-    # Find the top node of the triangle for z_x
-    c_x = Parent(N, z_x)
-    b_x = Parent(N, c_x)
-
-    # Find the top node of the triangle for z_y
-    c_y = Parent(N, z_y)
-    #    print()
-    #    print(z_y,N.edges())
-
-    b_y = Parent(N, c_y)
-
-    if N.in_degree(b_x) == 0:
-        # c_x is the child of the root
-        # c_x!=c_y, so c_y is not the child of the root
-        # swap the roles of x and y
-        x, y = y, x
-        z_x, z_y = z_y, z_x
-        b_x, b_y = b_y, b_x
-        c_x, c_y = c_y, c_x
-    # c_x is not the child of the root
-    # find a parent of b_x, and the bottom node of the triangle d_x
-    a_x = Parent(N, b_x, randomNodes=randomNodes)
-    d_x = Child(N, c_x, exclude=[z_x])
-    return [((c_x, d_x), c_x, (a_x, b_x)), ((z_x, x), z_x, (z_y, y))], [], z_x, up
-
-
-def Green_Line(network1, network2, head_moves=True):
-    """
-    An implementation of Algorithm 4 and its tail move counterpart. Finds a sequence of tail/rSPR moves from network1 to network2 by building a down-closed isomorphism.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param head_moves: a boolean value determining whether head moves are allowed (if True we use rSPR moves, if False we only use tail moves).
-    :return: A list of tail/rSPR moves from network1 to network2. Returns False if such a sequence does not exist.
-    """
-    # Find the root and labels of the networks
-    root1 = Root(network1)
-    root2 = Root(network2)
-    label_dict_1 = Labels(network1)
-    label_dict_2 = Labels(network2)
-
-    # initialize isomorphism
-    isom_1_2 = dict()
-    isom_2_1 = dict()
-    isom_size = 0
-    for label, node1 in label_dict_1.items():
-        node2 = label_dict_2[label]
-        isom_1_2[node1] = node2
-        isom_2_1[node2] = node1
-        isom_size += 1
-
-    # Keep track of the size of the isomorphism and the size it is at the end of the green line algorithm
-    goal_size = len(network1) - 1
-
-    # init lists of sequence of moves
-    # list of (moving_edge,moving_endpoint,from_edge,to_edge)
-    seq_from_1 = []
-    seq_from_2 = []
-    # TODO keep track of lowest nodes? (Currently, the code does not do this, but it could speed up the code)
-
-    # Do the green line algorithm
-    while (isom_size < goal_size):
-        # Find lowest nodes above the isom in the networks:
-        lowest_tree_node_network1, lowest_retic_network1 = LowestReticAndTreeNodeAbove(network1, isom_1_2.keys())
-        lowest_tree_node_network2, lowest_retic_network2 = LowestReticAndTreeNodeAbove(network2, isom_2_1.keys())
-
-        ######################################
-        # Case1: a lowest retic in network1
-        if lowest_retic_network1 != None:
-            # use notation as in the paper network1 = N', network2 = N, where ' is denoted p
-            up = lowest_retic_network1
-            if head_moves:
-                moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case1_rSPR(network2,
-                                                                                                             network1,
-                                                                                                             up,
-                                                                                                             isom_2_1,
-                                                                                                             isom_1_2)
-            else:
-                moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case1_Tail(network2,
-                                                                                                             network1,
-                                                                                                             up,
-                                                                                                             isom_2_1,
-                                                                                                             isom_1_2)
-                if added_node_network_1 == None:
-                    return False
-        ######################################
-        # Case2: a lowest retic in network2
-        elif lowest_retic_network2 != None:
-            # use notation as in the paper network2 = N', network1 = N, where ' is denoted p
-            up = lowest_retic_network2
-            if head_moves:
-                moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case1_rSPR(network1,
-                                                                                                             network2,
-                                                                                                             up,
-                                                                                                             isom_1_2,
-                                                                                                             isom_2_1)
-            else:
-                moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case1_Tail(network1,
-                                                                                                             network2,
-                                                                                                             up,
-                                                                                                             isom_1_2,
-                                                                                                             isom_2_1)
-                if added_node_network_1 == None:
-                    return False
-
-                    ######################################
-        # Case3: a lowest tree node in network1
-        else:
-            # use notation as in the paper network1 = N, network2 = N'
-            up = lowest_tree_node_network2
-            moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case3(network1, network2,
-                                                                                                    up, isom_1_2,
-                                                                                                    isom_2_1)
-        # Now perform the moves and update the isomorphism
-        isom_1_2[added_node_network_1] = added_node_network_2
-        isom_2_1[added_node_network_2] = added_node_network_1
-        for move in moves_network_1:
-            seq_from_1.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
-            network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
-        for move in moves_network_2:
-            seq_from_2.append((move[0], move[1], From_Edge(network2, move[0], move[1]), move[2]))
-            network2 = DoMove(network2, move[0], move[1], move[2], check_validity=False)
-        isom_size += 1
-    # TESTING FOR CORRECTNESS WHILE RUNNING
-    #        if not Isomorphic(network1.subgraph(isom_1_2.keys()),network2.subgraph(isom_2_1.keys())):
-    #            print("not unlabeled isom")
-    #            print(seq_from_1)
-    #            print(seq_from_2)
-    #            print(network1.subgraph(isom_1_2.keys()).edges())
-    #            print(network2.subgraph(isom_2_1.keys()).edges())
-
-    # Add the root to the isomorphism, if it was there
-    isom_1_2[root1] = root2
-    isom_2_1[root2] = root1
-    # invert seq_from_2, rename to node names of network1, and append to seq_from_1
-    return seq_from_1 + ReplaceNodeNamesInMoveSequence(InvertMoveSequence(seq_from_2), isom_2_1)
-
-
-def Green_Line_Random(network1, network2, head_moves=True, repeats=1):
-    """
-    Finds a sequence of tail/rSPR moves from network1 to network2 by randomly building a down-closed isomorphism a number of times, and only keeping the shortest sequence.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param head_moves: a boolean value determining whether head moves are allowed (if True we use rSPR moves, if False we only use tail moves).
-    :param repeats: an integer, determining how many repeats of Green_Line_Random_Single are performed.
-    :return: A list of tail/rSPR moves from network1 to network2. Returns False if such a sequence does not exist.
-    """
-    best_seq = None
-    for i in range(repeats):
-        candidate_seq = Green_Line_Random_Single(network1, network2, head_moves=head_moves)
-        if candidate_seq == False:
-            return False
-        if best_seq == None or len(best_seq) > len(candidate_seq):
-            best_seq = candidate_seq
-    return best_seq
-
-
-def Green_Line_Random_Single(network1, network2, head_moves=True):
-    """
-    An implementation of Algorithm 5 and its tail move counterpart. Finds a sequence of tail/rSPR moves from network1 to network2 by randomly building a down-closed isomorphism.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param head_moves: a boolean value determining whether head moves are allowed (if True we use rSPR moves, if False we only use tail moves).
-    :return: A list of tail/rSPR moves from network1 to network2. Returns False if such a sequence does not exist.
-    """
-    # Find the root and labels of the networks
-    root1 = Root(network1)
-    root2 = Root(network2)
-    label_dict_1 = Labels(network1)
-    label_dict_2 = Labels(network2)
-
-    # initialize isomorphism
-    isom_1_2 = dict()
-    isom_2_1 = dict()
-    isom_size = 0
-    for label, node1 in label_dict_1.items():
-        node2 = label_dict_2[label]
-        isom_1_2[node1] = node2
-        isom_2_1[node2] = node1
-        isom_size += 1
-
-    # Keep track of the size of the isomorphism and the size it is at the end of the green line algorithm
-    goal_size = len(network1) - 1
-
-    # init lists of sequence of moves
-    # list of (moving_edge,moving_endpoint,from_edge,to_edge)
-    seq_from_1 = []
-    seq_from_2 = []
-    # TODO keep track of lowest nodes?
-
-    # Do the green line algorithm
-    while (isom_size < goal_size):
-        # Find all lowest nodes above the isom in the networks:
-        lowest_tree_node_network1, lowest_retic_network1 = LowestReticAndTreeNodeAbove(network1, isom_1_2.keys(),
-                                                                                       allnodes=True)
-        lowest_tree_node_network2, lowest_retic_network2 = LowestReticAndTreeNodeAbove(network2, isom_2_1.keys(),
-                                                                                       allnodes=True)
-
-        # Construct a list of all lowest nodes in a tuple with the corresponding network (in random order)
-        # I.e. If u is a lowest node of network one, it will appear in the list as (u,1)
-        lowest_nodes_network1 = [(u, 1) for u in lowest_tree_node_network1 + lowest_retic_network1]
-        lowest_nodes_network2 = [(u, 2) for u in lowest_tree_node_network2 + lowest_retic_network2]
-        candidate_lowest_nodes = lowest_nodes_network1 + lowest_nodes_network2
-        random.shuffle(candidate_lowest_nodes)
-
-        # As some cases do not give an addition to the isom, we continue trying lowest nodes until we find one that does.
-        for lowest_node, network_number in candidate_lowest_nodes:
-            ######################################
-            # Case1: a lowest retic in network1
-            if network_number == 1 and network1.in_degree(lowest_node) == 2:
-                # use notation as in the paper network1 = N', network2 = N, where ' is denoted p
-                up = lowest_node
-                if head_moves:
-                    moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case1_rSPR(
-                        network2, network1, up, isom_2_1, isom_1_2, randomNodes=True)
-                else:
-                    moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case1_Tail(
-                        network2, network1, up, isom_2_1, isom_1_2, randomNodes=True)
-                    if added_node_network_1 == None:
-                        # The networks are non-isom networks with 2 leaves and 1 reticulation
-                        return False
-                # This case always gives a node to add to the isom
-                break
-
-            ######################################
-            # Case2: a lowest retic in network2
-            elif network_number == 2 and network2.in_degree(lowest_node) == 2:
-                # use notation as in the paper network2 = N', network1 = N, where ' is denoted p
-                up = lowest_node
-                if head_moves:
-                    moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case1_rSPR(
-                        network1, network2, up, isom_1_2, isom_2_1, randomNodes=True)
-                else:
-                    moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case1_Tail(
-                        network1, network2, up, isom_1_2, isom_2_1, randomNodes=True)
-                    if added_node_network_1 == None:
-                        # The networks are non-isom networks with 2 leaves and 1 reticulation
-                        return False
-                        # This case always gives a node to add to the isom
-                break
-
-            ######################################
-            # Case3: a lowest tree node in network1
-            elif network_number == 2 and network2.out_degree(lowest_node) == 2:
-                # use notation as in the paper network1 = N, network2 = N'
-                up = lowest_node
-                moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case3(network1,
-                                                                                                        network2, up,
-                                                                                                        isom_1_2,
-                                                                                                        isom_2_1,
-                                                                                                        randomNodes=True)
-                # If we can add a node to the isom, added_node_network_2 has a value
-                if added_node_network_2:
-                    break
-
-            ######################################
-            # Case3': a lowest tree node in network2
-            else:
-                # use notation as in the paper network1 = N, network2 = N'
-                up = lowest_node
-                moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case3(network2,
-                                                                                                        network1, up,
-                                                                                                        isom_2_1,
-                                                                                                        isom_1_2,
-                                                                                                        randomNodes=True)
-                # If we can add a node to the isom, added_node_network_2 has a value
-                if added_node_network_2:
-                    break
-
-        # Now perform the moves and update the isomorphism
-        isom_1_2[added_node_network_1] = added_node_network_2
-        isom_2_1[added_node_network_2] = added_node_network_1
-        for move in moves_network_1:
-            seq_from_1.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
-            network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
-        for move in moves_network_2:
-            seq_from_2.append((move[0], move[1], From_Edge(network2, move[0], move[1]), move[2]))
-            network2 = DoMove(network2, move[0], move[1], move[2], check_validity=False)
-        isom_size += 1
-    # TESTING FOR CORRECTNESS WHILE RUNNING
-    #        if not Isomorphic(network1.subgraph(isom_1_2.keys()),network2.subgraph(isom_2_1.keys())):
-    #            print("not unlabeled isom")
-    #            print(seq_from_1)
-    #            print(seq_from_2)
-    #            print(isom_1_2)
-    #            print(network1.subgraph(isom_1_2.keys()).edges())
-    #            print(network2.subgraph(isom_2_1.keys()).edges())
-
-    # Add the root to the isomorphism, if it was there
-    isom_1_2[root1] = root2
-    isom_2_1[root2] = root1
+# def GL_Case1_rSPR(N, Np, up, isom_N_Np, isom_Np_N, randomNodes=False):
+#     """
+#     An implementation of Algorithm 2. Finds a sequence of rSPR moves that makes it possible to add the lowest reticulation up to the down-closed isomrophism.
+
+#     :param N: a phylogenetic network.
+#     :param Np: a phylogenetic network.
+#     :param up: a lowest reticulation node of Np above the isomorphism.
+#     :param isom_N_Np: a dictionary, containing a partial (down-closed) isomorphism map from N to Np. The inverse of isom_Np_N.
+#     :param isom_Np_N: a dictionary, containing a partial (down-closed) isomorphism map from Np to N. The inverse of isom_N_Np.
+#     :param randomNodes: a boolean value, determining whether the random version of this lemma is used.
+#     :return: a list of rSPR moves in N, a list of rSPR moves in Np, a node of N, a node of Np. After performing the lists of moves on the networks, the nodes can be added to the isomorphism.
+#     """
+#     # use notation as in the paper
+#     # ' is denoted p
+#     xp = Child(Np, up)
+#     x = isom_Np_N[xp]
+#     z = Parent(N, x, exclude=isom_N_Np.keys(), randomNodes=randomNodes)
+
+#     # Case1a: z is a reticulation
+#     if N.in_degree(z) == 2:
+#         return [], [], z, up
+#     # Case1b: z is not a reticulation
+#     # Find a retic v in N not in the isom yet
+#     v = FindRetic(N, excludedSet=isom_N_Np.keys(), randomNodes=randomNodes)
+#     u = None
+#     for parent in N.predecessors(v):
+#         if CheckValid(N, (parent, v), v, (z, x)):
+#             if not randomNodes:
+#                 u = parent
+#                 break
+#             elif u == None or random.getrandbits(1):
+#                 u = parent
+#     # If v has an incoming arc (u,v) movable to (z,x), perform this move
+#     if u != None:
+#         return [((u, v), v, (z, x))], [], v, up
+#     # if none of the moves is valid, this must be because
+#     # v is already a reticulation above x with its movable incoming arc (u,v) with u=z.
+#     return [], [], v, up
+
+
+# def GL_Case1_Tail(N, Np, up, isom_N_Np, isom_Np_N, randomNodes=False):
+#     """
+#     An implementation of Algorithm 6. Finds a sequence of tail moves that makes it possible to add the lowest reticulation up to the down-closed isomrophism.
+
+#     :param N: a phylogenetic network.
+#     :param Np: a phylogenetic network.
+#     :param up: a lowest reticulation node of Np above the isomorphism.
+#     :param isom_N_Np: a dictionary, containing a partial (down-closed) isomorphism map from N to Np. The inverse of isom_Np_N.
+#     :param isom_Np_N: a dictionary, containing a partial (down-closed) isomorphism map from Np to N. The inverse of isom_N_Np.
+#     :param randomNodes: a boolean value, determining whether the random version of this lemma is used.
+#     :return: a list of tail moves in N, a list of tail moves in Np, a node of N, a node of Np. After performing the lists of moves on the networks, the nodes can be added to the isomorphism. Returns false if the networks are not isomorphic with 2 leaves and 1 reticulation.
+#     """
+#     # use notation as in the paper
+#     # ' is denoted p
+#     xp = Child(Np, up)
+#     x = isom_Np_N[xp]
+#     z = Parent(N, x, exclude=isom_N_Np.keys(), randomNodes=randomNodes)
+#     # Case1a: z is a reticulation
+#     if N.in_degree(z) == 2:
+#         return [], [], z, up
+#     # Case1b: z is not a reticulation
+#     # z is a tree node
+#     if check_movable(N, (z, x), z):
+#         # Case1bi: (z,x) is movable
+#         # Find a reticulation u in N not in the isomorphism yet
+#         # TODO: Can first check if the other parent of x suffices here, should heuristcally be better
+#         u = FindRetic(N, excludedSet=isom_N_Np.keys(), randomNodes=randomNodes)
+#         v = Child(N, u)
+#         if v == x:
+#             return [], [], u, up
+#         # we may now assume v!=x
+#         if z == v:
+#             v = Child(N, z, exclude=[x])
+#             w = Parent(N, u, randomNodes=randomNodes)
+#             return [((z, v), z, (w, u))], [], u, up
+#         w = Parent(N, u, exclude=[z], randomNodes=randomNodes)
+#         return [((z, x), z, (u, v)), ((z, v), z, (w, u))], [], u, up
+#     # Case1bii: (z,x) is not movable
+#     c = Parent(N, z)
+#     d = Child(N, z, exclude=[x])
+#     # TODO: b does not have to exist if we have an outdeg-2 root, this could be c!
+#     b = Parent(N, c)
+#     if N.in_degree(b) != 0:
+#         # Case1biiA: b is not the root of N
+#         a = Parent(N, b, randomNodes=randomNodes)
+#         # First do the move ((c,d),c,(a,b)), then Case1bi applies as (z,x) is now movable
+#         newN = DoMove(N, (c, d), c, (a, b))
+#         u = FindRetic(newN, excludedSet=isom_N_Np.keys(), randomNodes=randomNodes)
+#         v = Child(newN, u)
+#         if v == x:
+#             # In this case, u is a reticulation parent of x and u is not in the isom. Hence, we can simply add it to the isom.
+#             # Note: The tail move we did is not necessary!
+#             # TODO: First check both parents of x for being a reticulation not in the isomorphism yet
+#             return [], [], u, up
+#         # we may now assume v!=x
+#         if z == v:
+#             # This only happens if z==v and u==b
+#             # we move z up above the retic b as well, too
+#             w = Parent(newN, b, randomNodes=randomNodes)
+#             return [((c, d), c, (a, b)), ((z, d), z, (w, b))], [], u, up
+#         w = Parent(newN, u, exclude=[z], randomNodes=randomNodes)
+#         return [((c, d), c, (a, b)), ((z, x), z, (u, v)), ((z, v), z, (w, u))], [], u, up
+#     # Case1biiB: b is the root of N
+#     # Note: d is not in the isomorphism
+#     e = Child(N, d)
+#     if e == x:
+#         return [], [], d, up
+#     if N.out_degree(x) == 2:
+#         s = Child(N, x)
+#         t = Child(N, x, exclude=[s])
+#         if s == e:
+#             return [((x, t), x, (d, e))], [], d, up
+#         if t == e:
+#             return [((x, s), x, (d, e))], [], d, up
+#         return [((x, s), x, (d, e)), ((x, e), x, (z, t)), ((x, t), x, (d, s))], [], d, up
+#     if N.out_degree(e) == 2:
+#         s = Child(N, e)
+#         t = Child(N, e, exclude=[s])
+#         if s == x:
+#             return [((e, t), e, (z, x))], [], d, up
+#         if t == x:
+#             return [((e, s), e, (z, x))], [], d, up
+#         return [((e, s), e, (z, x)), ((e, x), e, (d, t)), ((e, t), e, (z, s))], [], d, up
+#     # neither are tree nodes, so both must be leaves
+#     # In that case, there is no sequence between the two networks.
+#     return [], [], None, None
+
+
+# def GL_Case3(N, Np, up, isom_N_Np, isom_Np_N, randomNodes=False):
+#     """
+#     An implementation of Algorithm 3. Finds a sequence of tail moves that makes it possible to add the lowest tree node up to the down-closed isomrophism.
+
+#     :param N: a phylogenetic network.
+#     :param Np: a phylogenetic network.
+#     :param up: a lowest tree node of Np above the isomorphism.
+#     :param isom_N_Np: a dictionary, containing a partial (down-closed) isomorphism map from N to Np. The inverse of isom_Np_N.
+#     :param isom_Np_N: a dictionary, containing a partial (down-closed) isomorphism map from Np to N. The inverse of isom_N_Np.
+#     :param randomNodes: a boolean value, determining whether the random version of this lemma is used.
+#     :return: a list of tail moves in N, a list of tail moves in Np, a node of N, a node of Np. After performing the lists of moves on the networks, the nodes can be added to the isomorphism.
+#     """
+#     # Find the children x' and y' of u'
+#     xp, yp = list(Np.successors(up))
+#     # Find the corresponding nodes x and y in N
+#     x = isom_Np_N[xp]
+#     y = isom_Np_N[yp]
+#     # Find the set of common parents of x and y
+#     parents_x = set(N.predecessors(x))
+#     parents_y = set(N.predecessors(y))
+#     common_parents = parents_x & parents_y
+#     # Case3a: x and y have a common parent not in the isom
+#     common_parents_not_Y = []
+#     for parent in common_parents:
+#         if parent not in isom_N_Np.keys():
+#             # then parent can be mapped to up
+#             common_parents_not_Y += [parent]
+#             if not randomNodes:
+#                 return [], [], parent, up
+#     if common_parents_not_Y:
+#         return [], [], random.choice(common_parents_not_Y), up
+
+#     # Case3b: x and y do not have a common parent in the isomorphism
+#     # For both, find a parent not in the isomorphism yet
+#     # TODO: preferably make them tree nodes
+#     z_x = Parent(N, x, exclude=isom_N_Np.keys(), randomNodes=randomNodes)
+#     z_y = Parent(N, y, exclude=isom_N_Np.keys(), randomNodes=randomNodes)
+
+#     # Case3bi: (z_x,x) is movable
+#     if CheckValid(N, (z_x, x), z_x, (z_y, y)):
+#         return [((z_x, x), z_x, (z_y, y))], [], z_x, up
+#     # Case3bii: (z_y,y) is movable
+#     if CheckValid(N, (z_y, y), z_y, (z_x, x)):
+#         return [((z_y, y), z_y, (z_x, x))], [], z_y, up
+#     # Case3biii: Neither (z_x,x) nor (z_y,y) is movable
+
+#     if N.in_degree(z_x) == 2 or N.in_degree(z_y) == 2:
+#         return [], [], None, None
+#     # Both these parents are tree nodes.
+#     # This happens always in the non-random version, as otherwise there is a lowest reticulation node and we would be in Case 1 or 2.
+
+#     # As both nodes are tree nodes and the arcs immovable, both arcs hang of the side of a triangle.
+#     # Find the top node of the triangle for z_x
+#     c_x = Parent(N, z_x)
+#     b_x = Parent(N, c_x)
+
+#     # Find the top node of the triangle for z_y
+#     c_y = Parent(N, z_y)
+#     #    print()
+#     #    print(z_y,N.edges())
+
+#     b_y = Parent(N, c_y)
+
+#     if N.in_degree(b_x) == 0:
+#         # c_x is the child of the root
+#         # c_x!=c_y, so c_y is not the child of the root
+#         # swap the roles of x and y
+#         x, y = y, x
+#         z_x, z_y = z_y, z_x
+#         b_x, b_y = b_y, b_x
+#         c_x, c_y = c_y, c_x
+#     # c_x is not the child of the root
+#     # find a parent of b_x, and the bottom node of the triangle d_x
+#     a_x = Parent(N, b_x, randomNodes=randomNodes)
+#     d_x = Child(N, c_x, exclude=[z_x])
+#     return [((c_x, d_x), c_x, (a_x, b_x)), ((z_x, x), z_x, (z_y, y))], [], z_x, up
+
+
+# def Green_Line(network1, network2, head_moves=True):
+#     """
+#     An implementation of Algorithm 4 and its tail move counterpart. Finds a sequence of tail/rSPR moves from network1 to network2 by building a down-closed isomorphism.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param head_moves: a boolean value determining whether head moves are allowed (if True we use rSPR moves, if False we only use tail moves).
+#     :return: A list of tail/rSPR moves from network1 to network2. Returns False if such a sequence does not exist.
+#     """
+#     # Find the root and labels of the networks
+#     root1 = Root(network1)
+#     root2 = Root(network2)
+#     label_dict_1 = Labels(network1)
+#     label_dict_2 = Labels(network2)
+
+#     # initialize isomorphism
+#     isom_1_2 = dict()
+#     isom_2_1 = dict()
+#     isom_size = 0
+#     for label, node1 in label_dict_1.items():
+#         node2 = label_dict_2[label]
+#         isom_1_2[node1] = node2
+#         isom_2_1[node2] = node1
+#         isom_size += 1
+
+#     # Keep track of the size of the isomorphism and the size it is at the end of the green line algorithm
+#     goal_size = len(network1) - 1
+
+#     # init lists of sequence of moves
+#     # list of (moving_edge,moving_endpoint,from_edge,to_edge)
+#     seq_from_1 = []
+#     seq_from_2 = []
+#     # TODO keep track of lowest nodes? (Currently, the code does not do this, but it could speed up the code)
+
+#     # Do the green line algorithm
+#     while (isom_size < goal_size):
+#         # Find lowest nodes above the isom in the networks:
+#         lowest_tree_node_network1, lowest_retic_network1 = LowestReticAndTreeNodeAbove(network1, isom_1_2.keys())
+#         lowest_tree_node_network2, lowest_retic_network2 = LowestReticAndTreeNodeAbove(network2, isom_2_1.keys())
+
+#         ######################################
+#         # Case1: a lowest retic in network1
+#         if lowest_retic_network1 != None:
+#             # use notation as in the paper network1 = N', network2 = N, where ' is denoted p
+#             up = lowest_retic_network1
+#             if head_moves:
+#                 moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case1_rSPR(network2,
+#                                                                                                              network1,
+#                                                                                                              up,
+#                                                                                                              isom_2_1,
+#                                                                                                              isom_1_2)
+#             else:
+#                 moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case1_Tail(network2,
+#                                                                                                              network1,
+#                                                                                                              up,
+#                                                                                                              isom_2_1,
+#                                                                                                              isom_1_2)
+#                 if added_node_network_1 == None:
+#                     return False
+#         ######################################
+#         # Case2: a lowest retic in network2
+#         elif lowest_retic_network2 != None:
+#             # use notation as in the paper network2 = N', network1 = N, where ' is denoted p
+#             up = lowest_retic_network2
+#             if head_moves:
+#                 moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case1_rSPR(network1,
+#                                                                                                              network2,
+#                                                                                                              up,
+#                                                                                                              isom_1_2,
+#                                                                                                              isom_2_1)
+#             else:
+#                 moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case1_Tail(network1,
+#                                                                                                              network2,
+#                                                                                                              up,
+#                                                                                                              isom_1_2,
+#                                                                                                              isom_2_1)
+#                 if added_node_network_1 == None:
+#                     return False
+
+#                     ######################################
+#         # Case3: a lowest tree node in network1
+#         else:
+#             # use notation as in the paper network1 = N, network2 = N'
+#             up = lowest_tree_node_network2
+#             moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case3(network1, network2,
+#                                                                                                     up, isom_1_2,
+#                                                                                                     isom_2_1)
+#         # Now perform the moves and update the isomorphism
+#         isom_1_2[added_node_network_1] = added_node_network_2
+#         isom_2_1[added_node_network_2] = added_node_network_1
+#         for move in moves_network_1:
+#             seq_from_1.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
+#             network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
+#         for move in moves_network_2:
+#             seq_from_2.append((move[0], move[1], From_Edge(network2, move[0], move[1]), move[2]))
+#             network2 = DoMove(network2, move[0], move[1], move[2], check_validity=False)
+#         isom_size += 1
+#     # TESTING FOR CORRECTNESS WHILE RUNNING
+#     #        if not Isomorphic(network1.subgraph(isom_1_2.keys()),network2.subgraph(isom_2_1.keys())):
+#     #            print("not unlabeled isom")
+#     #            print(seq_from_1)
+#     #            print(seq_from_2)
+#     #            print(network1.subgraph(isom_1_2.keys()).edges())
+#     #            print(network2.subgraph(isom_2_1.keys()).edges())
+
+#     # Add the root to the isomorphism, if it was there
+#     isom_1_2[root1] = root2
+#     isom_2_1[root2] = root1
+#     # invert seq_from_2, rename to node names of network1, and append to seq_from_1
+#     return seq_from_1 + ReplaceNodeNamesInMoveSequence(InvertMoveSequence(seq_from_2), isom_2_1)
+
+
+# def Green_Line_Random(network1, network2, head_moves=True, repeats=1):
+#     """
+#     Finds a sequence of tail/rSPR moves from network1 to network2 by randomly building a down-closed isomorphism a number of times, and only keeping the shortest sequence.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param head_moves: a boolean value determining whether head moves are allowed (if True we use rSPR moves, if False we only use tail moves).
+#     :param repeats: an integer, determining how many repeats of Green_Line_Random_Single are performed.
+#     :return: A list of tail/rSPR moves from network1 to network2. Returns False if such a sequence does not exist.
+#     """
+#     best_seq = None
+#     for i in range(repeats):
+#         candidate_seq = Green_Line_Random_Single(network1, network2, head_moves=head_moves)
+#         if candidate_seq == False:
+#             return False
+#         if best_seq == None or len(best_seq) > len(candidate_seq):
+#             best_seq = candidate_seq
+#     return best_seq
+
+
+# def Green_Line_Random_Single(network1, network2, head_moves=True):
+#     """
+#     An implementation of Algorithm 5 and its tail move counterpart. Finds a sequence of tail/rSPR moves from network1 to network2 by randomly building a down-closed isomorphism.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param head_moves: a boolean value determining whether head moves are allowed (if True we use rSPR moves, if False we only use tail moves).
+#     :return: A list of tail/rSPR moves from network1 to network2. Returns False if such a sequence does not exist.
+#     """
+#     # Find the root and labels of the networks
+#     root1 = Root(network1)
+#     root2 = Root(network2)
+#     label_dict_1 = Labels(network1)
+#     label_dict_2 = Labels(network2)
+
+#     # initialize isomorphism
+#     isom_1_2 = dict()
+#     isom_2_1 = dict()
+#     isom_size = 0
+#     for label, node1 in label_dict_1.items():
+#         node2 = label_dict_2[label]
+#         isom_1_2[node1] = node2
+#         isom_2_1[node2] = node1
+#         isom_size += 1
+
+#     # Keep track of the size of the isomorphism and the size it is at the end of the green line algorithm
+#     goal_size = len(network1) - 1
+
+#     # init lists of sequence of moves
+#     # list of (moving_edge,moving_endpoint,from_edge,to_edge)
+#     seq_from_1 = []
+#     seq_from_2 = []
+#     # TODO keep track of lowest nodes?
+
+#     # Do the green line algorithm
+#     while (isom_size < goal_size):
+#         # Find all lowest nodes above the isom in the networks:
+#         lowest_tree_node_network1, lowest_retic_network1 = LowestReticAndTreeNodeAbove(network1, isom_1_2.keys(),
+#                                                                                        allnodes=True)
+#         lowest_tree_node_network2, lowest_retic_network2 = LowestReticAndTreeNodeAbove(network2, isom_2_1.keys(),
+#                                                                                        allnodes=True)
+
+#         # Construct a list of all lowest nodes in a tuple with the corresponding network (in random order)
+#         # I.e. If u is a lowest node of network one, it will appear in the list as (u,1)
+#         lowest_nodes_network1 = [(u, 1) for u in lowest_tree_node_network1 + lowest_retic_network1]
+#         lowest_nodes_network2 = [(u, 2) for u in lowest_tree_node_network2 + lowest_retic_network2]
+#         candidate_lowest_nodes = lowest_nodes_network1 + lowest_nodes_network2
+#         random.shuffle(candidate_lowest_nodes)
+
+#         # As some cases do not give an addition to the isom, we continue trying lowest nodes until we find one that does.
+#         for lowest_node, network_number in candidate_lowest_nodes:
+#             ######################################
+#             # Case1: a lowest retic in network1
+#             if network_number == 1 and network1.in_degree(lowest_node) == 2:
+#                 # use notation as in the paper network1 = N', network2 = N, where ' is denoted p
+#                 up = lowest_node
+#                 if head_moves:
+#                     moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case1_rSPR(
+#                         network2, network1, up, isom_2_1, isom_1_2, randomNodes=True)
+#                 else:
+#                     moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case1_Tail(
+#                         network2, network1, up, isom_2_1, isom_1_2, randomNodes=True)
+#                     if added_node_network_1 == None:
+#                         # The networks are non-isom networks with 2 leaves and 1 reticulation
+#                         return False
+#                 # This case always gives a node to add to the isom
+#                 break
+
+#             ######################################
+#             # Case2: a lowest retic in network2
+#             elif network_number == 2 and network2.in_degree(lowest_node) == 2:
+#                 # use notation as in the paper network2 = N', network1 = N, where ' is denoted p
+#                 up = lowest_node
+#                 if head_moves:
+#                     moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case1_rSPR(
+#                         network1, network2, up, isom_1_2, isom_2_1, randomNodes=True)
+#                 else:
+#                     moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case1_Tail(
+#                         network1, network2, up, isom_1_2, isom_2_1, randomNodes=True)
+#                     if added_node_network_1 == None:
+#                         # The networks are non-isom networks with 2 leaves and 1 reticulation
+#                         return False
+#                         # This case always gives a node to add to the isom
+#                 break
+
+#             ######################################
+#             # Case3: a lowest tree node in network1
+#             elif network_number == 2 and network2.out_degree(lowest_node) == 2:
+#                 # use notation as in the paper network1 = N, network2 = N'
+#                 up = lowest_node
+#                 moves_network_1, moves_network_2, added_node_network_1, added_node_network_2 = GL_Case3(network1,
+#                                                                                                         network2, up,
+#                                                                                                         isom_1_2,
+#                                                                                                         isom_2_1,
+#                                                                                                         randomNodes=True)
+#                 # If we can add a node to the isom, added_node_network_2 has a value
+#                 if added_node_network_2:
+#                     break
+
+#             ######################################
+#             # Case3': a lowest tree node in network2
+#             else:
+#                 # use notation as in the paper network1 = N, network2 = N'
+#                 up = lowest_node
+#                 moves_network_2, moves_network_1, added_node_network_2, added_node_network_1 = GL_Case3(network2,
+#                                                                                                         network1, up,
+#                                                                                                         isom_2_1,
+#                                                                                                         isom_1_2,
+#                                                                                                         randomNodes=True)
+#                 # If we can add a node to the isom, added_node_network_2 has a value
+#                 if added_node_network_2:
+#                     break
+
+#         # Now perform the moves and update the isomorphism
+#         isom_1_2[added_node_network_1] = added_node_network_2
+#         isom_2_1[added_node_network_2] = added_node_network_1
+#         for move in moves_network_1:
+#             seq_from_1.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
+#             network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
+#         for move in moves_network_2:
+#             seq_from_2.append((move[0], move[1], From_Edge(network2, move[0], move[1]), move[2]))
+#             network2 = DoMove(network2, move[0], move[1], move[2], check_validity=False)
+#         isom_size += 1
+#     # TESTING FOR CORRECTNESS WHILE RUNNING
+#     #        if not Isomorphic(network1.subgraph(isom_1_2.keys()),network2.subgraph(isom_2_1.keys())):
+#     #            print("not unlabeled isom")
+#     #            print(seq_from_1)
+#     #            print(seq_from_2)
+#     #            print(isom_1_2)
+#     #            print(network1.subgraph(isom_1_2.keys()).edges())
+#     #            print(network2.subgraph(isom_2_1.keys()).edges())
+
+#     # Add the root to the isomorphism, if it was there
+#     isom_1_2[root1] = root2
+#     isom_2_1[root2] = root1
 
-    # invert seq_from_2, rename to node names of network1, and append to seq_from_1
-    return seq_from_1 + ReplaceNodeNamesInMoveSequence(InvertMoveSequence(seq_from_2), isom_2_1)
+#     # invert seq_from_2, rename to node names of network1, and append to seq_from_1
+#     return seq_from_1 + ReplaceNodeNamesInMoveSequence(InvertMoveSequence(seq_from_2), isom_2_1)
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/heuristics/heuristic_tools.py` & `phylox-0.0.2/src/phylox/rearrangement/heuristics/heuristic_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,275 +1,275 @@
-# Returns all nodes below a given node (including the node itself)
-def AllBelow(network, node):
-    """
-    Finds all nodes below a given node in a network.
-
-    :param network: a phylogenetic network.
-    :param node: a node in the network.
-    :return: all nodes in the network that are below the chosen node, including this node.
-    """
-    lengths = nx.single_source_shortest_path_length(network, node)
-    return lengths.keys()
-
-
-# Find the lowest nodes above a given set.
-# The excluded set must include all leaves.
-def LowestReticAndTreeNodeAbove(network, excludedSet, allnodes=False):
-    """
-    Finds a list of lowest tree nodes and a list of lowest reticulation nodes above a given set of nodes.
-
-    :param network: a phylogenetic network.
-    :param excludedSet: a set of nodes of the network.
-    :param allnodes: a boolean value that determines whether we try to find all lowest nodes (True) or only one lowest node of each type (False, Default).
-    :return: A list of tree nodes and a list of reticulation nodes, so that each element of these lists has all their children in the excludedSet. If not allNodes, then these lists have length at most 1.
-    """
-    retic = None
-    tree_node = None
-    lowest_retics = []
-    lowest_tree_nodes = []
-    for node in network.nodes():
-        if node not in excludedSet:
-            for c in network.successors(node):
-                if c not in excludedSet:
-                    break
-            # else runs if the loop was not ended by a break
-            # this happens exactly when all of the children are in excludedSet
-            else:
-                if network.out_degree(node) == 2:
-                    if allnodes:
-                        lowest_tree_nodes += [node]
-                    elif tree_node == None:
-                        # For simplicity in description, take the FIRST lowest tree node that we encounter (sim. for the reticulations)
-                        tree_node = node
-                elif network.in_degree(node) == 2:
-                    if allnodes:
-                        lowest_retics += [node]
-                    elif retic == None:
-                        retic = node
-                if not allnodes and tree_node != None and retic != None:
-                    # stop if both types of lowest nodes are found
-                    break
-    if allnodes:
-        return lowest_tree_nodes, lowest_retics
-    return tree_node, retic
-
-
-# Find the highest nodes below a given set.
-# The excluded set must include the root.
-def HighestNodesBelow(network, excludedSet, allnodes=False):
-    """
-    Finds a list of highest tree nodes and a list of highest reticulation nodes below a given set of nodes.
-
-    :param network: a phylogenetic network.
-    :param excludedSet: a set of nodes of the network.
-    :param allnodes: a boolean value that determines whether we try to find all highest nodes (True) or only one highest node of each type (False, Default).
-    :return: A list of tree nodes and a list of reticulation nodes, so that each element of these lists has all their parents in the excludedSet. If not allNodes, then these lists have length at most 1.
-    """
-    retic = None
-    tree_node = None
-    highest_retics = []
-    highest_tree_nodes = []
-    for node in network.nodes():
-        if node not in excludedSet:
-            for c in network.predecessors(node):
-                if c not in excludedSet:
-                    break
-            # else runs if the loop was not ended by a break
-            # this happens exactly when all of the parents are in excludedSet
-            else:
-                if network.out_degree(node) == 2:
-                    if allnodes:
-                        highest_tree_nodes += [node]
-                    elif tree_node == None:
-                        # For simplicity in description, take the FIRST highest tree node that we encounter (sim. for the reticulations and leaves)
-                        tree_node = node
-                elif network.in_degree(node) == 2:
-                    if allnodes:
-                        highest_retics += [node]
-                    elif retic == None:
-                        retic = node
-                if not allnodes and retic != None and tree_node != None:
-                    # stop if all types of highest nodes are found
-                    break
-    if allnodes:
-        return highest_tree_nodes, highest_retics
-    return tree_node, retic
-
-
-def FindTreeNode(network, excludedSet=[], randomNodes=False):
-    """
-    Finds a (random) tree node in a network.
-
-    :param network: a phylogenetic network.
-    :param excludedSet: a set of nodes of the network.
-    :param randomNodes: a boolean value.
-    :return: a tree node of the network not in the excludedSet, or None if no such node exists. If randomNodes, then a tree node is selected from all candidates uniformly at random.
-    """
-    all_found = []
-    for node in network.nodes():
-        if node not in excludedSet and network.out_degree(node) == 2 and network.in_degree(node) == 1:
-            if randomNodes:
-                all_found += [node]
-            else:
-                return node
-    if all_found and randomNodes:
-        return random.choice(all_found)
-    return None
-
-
-def FindLeaf(network, excludedSet=[], excludedParents=[], randomNodes=False):
-    """
-    Finds a (random) leaf in a network.
-
-    :param network: a phylogenetic network.
-    :param excludedSet: a set of nodes of the network.
-    :param excludedParents: a set of nodes of the network.
-    :param randomNodes: a boolean value.
-    :return: a leaf of the network not in the excludedSet so that its parent is nt in excludedParents, or None if no such node exists. If randomNodes, then a leaf is selected from all candidates uniformly at random.
-    """
-    all_found = []
-    for node in network.nodes():
-        parent = Parent(network, node)
-        if network.out_degree(node) == 0 and parent not in excludedParents and node not in excludedSet:
-            if randomNodes:
-                all_found += [node]
-            else:
-                return node
-    if all_found and randomNodes:
-        return random.choice(all_found)
-    return None
-
-
-def FindRetic(network, excludedSet=[], randomNodes=False):
-    """
-    Finds a (random) reticulation in a network.
-
-    :param network: a phylogenetic network.
-    :param excludedSet: a set of nodes of the network.
-    :param randomNodes: a boolean value.
-    :return: a reticulation node of the network not in the excludedSet, or None if no such node exists. If randomNodes, then a reticulation is selected from all candidates uniformly at random.
-    """
-    all_found = []
-    for node in network.nodes():
-        if node not in excludedSet and network.in_degree(node) == 2:
-            if randomNodes:
-                all_found += [node]
-            else:
-                return node
-    if all_found and randomNodes:
-        return random.choice(all_found)
-    return None
-
-
-def Parent(network, node, exclude=[], randomNodes=False):
-    """
-    Finds a parent of a node in a network.
-
-    :param network: a phylogenetic network.
-    :param node: a node in the network.
-    :param exclude: a set of nodes of the network.
-    :param randomNodes: a boolean value.
-    :return: a parent of node that is not in the set of nodes exclude. If randomNodes, then this parent is selected uniformly at random from all candidates.
-    """
-    parent = None
-    for p in network.predecessors(node):
-        if p not in exclude:
-            if not randomNodes:
-                return p
-            elif parent == None or random.getrandbits(1):
-                # As there are at most two parents, we can simply replace the previous parent with probability .5 to get a random parent
-                parent = p
-    return parent
-
-
-def Child(network, node, exclude=[], randomNodes=False):
-    """
-    Finds a child node of a node in a network.
-
-    :param network: a phylogenetic network.
-    :param node: a node in the network.
-    :param exclude: a set of nodes of the network.
-    :param randomNodes: a boolean value.
-    :return: a child of node that is not in the set of nodes exclude. If randomNodes, then this child node is selected uniformly at random from all candidates.
-    """
-    child = None
-    for c in network.successors(node):
-        if c not in exclude:
-            if not randomNodes:
-                return c
-            elif child == None or random.getrandbits(1):
-                # As there are at most two children, we can simply replace the previous child with probability .5 to get a random parent
-                child = c
-    return child
-
-
-# Returns the root of a network
-def Root(network):
-    """
-    Finds the root of a phylogenetic network.
-
-    :param network: a phylogenetic network.
-    :return: the root node of this network.
-    """
-    for node in network.nodes():
-        if network.in_degree(node) == 0:
-            return node
-    return None
-
-
-# Returns a dictionary with node labels, keyed by the labels
-def Labels(network):
-    """
-    Returns the correspondence between the leaves and the leaf-labels of a given network
-
-    :param network: a phylogenetic network
-    :return: a dictionary, where the keys are labels and the values are nodes of the network.
-    """
-    label_dict = dict()
-    for node in network.nodes():
-        node_label = network.node[node].get('label')
-        if node_label:
-            label_dict[node_label] = node
-    return label_dict
-
-
-    # Find a sequence by choosing the move that most decreases the upper bound on the number of moves
-# This works as long as we can always decrease the bound.
-# E.g.1, this upper bound can be the length of the sequence given by Green_Line(N1,N2), the bound can always decrease after one move, if we take the move from the GL sequence (IMPLEMENTED)
-# TODO E.g.2, take the upper bound given by this algorithm with bound Green_Line
-def Deep_Dive_Scored(network1, network2, head_moves=True, bound_heuristic=Green_Line):
-    """
-    An experimental method that returns a sequence of tail/rSPR moves from network1 to network2, using the isomorphism-building heuristic for the chosen type of moves.
-
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param head_moves: a boolean value that determines whether head moves are used in addition to tail moves. If True we use rSPR moves, if False we use only tail moves.
-    :param bound_heuristic: a heuristic that finds a sequence between the networks quickly.
-    :return: a sequence of moves from network1 to network2.
-    """
-    if Isomorphic(network1, network2):
-        return []
-    seq = []
-    current_network = network1
-    current_best = []
-    for move in bound_heuristic(network1, network2, head_moves=head_moves):
-        current_best += [(move[0], move[1], move[3])]
-    if not current_best:
-        return False
-    done = False
-    current_length = 0
-    while not done:
-        candidate_moves = AllValidMoves(current_network, tail_moves=True, head_moves=head_moves)
-        for move in candidate_moves:
-            candidate_network = DoMove(current_network, *move)
-            if Isomorphic(candidate_network, network2):
-                return current_best[:current_length] + [move]
-            candidate_sequence = bound_heuristic(candidate_network, network2, head_moves=head_moves)
-            if current_length + len(candidate_sequence) + 1 < len(current_best):
-                current_best = current_best[:current_length] + [move]
-                for move2 in candidate_sequence:
-                    current_best += [(move2[0], move2[1], move2[3])]
-        next_move = current_best[current_length]
-        current_network = DoMove(current_network, *next_move)
-        current_length += 1
-    return True
+# # Returns all nodes below a given node (including the node itself)
+# def AllBelow(network, node):
+#     """
+#     Finds all nodes below a given node in a network.
+
+#     :param network: a phylogenetic network.
+#     :param node: a node in the network.
+#     :return: all nodes in the network that are below the chosen node, including this node.
+#     """
+#     lengths = nx.single_source_shortest_path_length(network, node)
+#     return lengths.keys()
+
+
+# # Find the lowest nodes above a given set.
+# # The excluded set must include all leaves.
+# def LowestReticAndTreeNodeAbove(network, excludedSet, allnodes=False):
+#     """
+#     Finds a list of lowest tree nodes and a list of lowest reticulation nodes above a given set of nodes.
+
+#     :param network: a phylogenetic network.
+#     :param excludedSet: a set of nodes of the network.
+#     :param allnodes: a boolean value that determines whether we try to find all lowest nodes (True) or only one lowest node of each type (False, Default).
+#     :return: A list of tree nodes and a list of reticulation nodes, so that each element of these lists has all their children in the excludedSet. If not allNodes, then these lists have length at most 1.
+#     """
+#     retic = None
+#     tree_node = None
+#     lowest_retics = []
+#     lowest_tree_nodes = []
+#     for node in network.nodes():
+#         if node not in excludedSet:
+#             for c in network.successors(node):
+#                 if c not in excludedSet:
+#                     break
+#             # else runs if the loop was not ended by a break
+#             # this happens exactly when all of the children are in excludedSet
+#             else:
+#                 if network.out_degree(node) == 2:
+#                     if allnodes:
+#                         lowest_tree_nodes += [node]
+#                     elif tree_node == None:
+#                         # For simplicity in description, take the FIRST lowest tree node that we encounter (sim. for the reticulations)
+#                         tree_node = node
+#                 elif network.in_degree(node) == 2:
+#                     if allnodes:
+#                         lowest_retics += [node]
+#                     elif retic == None:
+#                         retic = node
+#                 if not allnodes and tree_node != None and retic != None:
+#                     # stop if both types of lowest nodes are found
+#                     break
+#     if allnodes:
+#         return lowest_tree_nodes, lowest_retics
+#     return tree_node, retic
+
+
+# # Find the highest nodes below a given set.
+# # The excluded set must include the root.
+# def HighestNodesBelow(network, excludedSet, allnodes=False):
+#     """
+#     Finds a list of highest tree nodes and a list of highest reticulation nodes below a given set of nodes.
+
+#     :param network: a phylogenetic network.
+#     :param excludedSet: a set of nodes of the network.
+#     :param allnodes: a boolean value that determines whether we try to find all highest nodes (True) or only one highest node of each type (False, Default).
+#     :return: A list of tree nodes and a list of reticulation nodes, so that each element of these lists has all their parents in the excludedSet. If not allNodes, then these lists have length at most 1.
+#     """
+#     retic = None
+#     tree_node = None
+#     highest_retics = []
+#     highest_tree_nodes = []
+#     for node in network.nodes():
+#         if node not in excludedSet:
+#             for c in network.predecessors(node):
+#                 if c not in excludedSet:
+#                     break
+#             # else runs if the loop was not ended by a break
+#             # this happens exactly when all of the parents are in excludedSet
+#             else:
+#                 if network.out_degree(node) == 2:
+#                     if allnodes:
+#                         highest_tree_nodes += [node]
+#                     elif tree_node == None:
+#                         # For simplicity in description, take the FIRST highest tree node that we encounter (sim. for the reticulations and leaves)
+#                         tree_node = node
+#                 elif network.in_degree(node) == 2:
+#                     if allnodes:
+#                         highest_retics += [node]
+#                     elif retic == None:
+#                         retic = node
+#                 if not allnodes and retic != None and tree_node != None:
+#                     # stop if all types of highest nodes are found
+#                     break
+#     if allnodes:
+#         return highest_tree_nodes, highest_retics
+#     return tree_node, retic
+
+
+# def FindTreeNode(network, excludedSet=[], randomNodes=False):
+#     """
+#     Finds a (random) tree node in a network.
+
+#     :param network: a phylogenetic network.
+#     :param excludedSet: a set of nodes of the network.
+#     :param randomNodes: a boolean value.
+#     :return: a tree node of the network not in the excludedSet, or None if no such node exists. If randomNodes, then a tree node is selected from all candidates uniformly at random.
+#     """
+#     all_found = []
+#     for node in network.nodes():
+#         if node not in excludedSet and network.out_degree(node) == 2 and network.in_degree(node) == 1:
+#             if randomNodes:
+#                 all_found += [node]
+#             else:
+#                 return node
+#     if all_found and randomNodes:
+#         return random.choice(all_found)
+#     return None
+
+
+# def FindLeaf(network, excludedSet=[], excludedParents=[], randomNodes=False):
+#     """
+#     Finds a (random) leaf in a network.
+
+#     :param network: a phylogenetic network.
+#     :param excludedSet: a set of nodes of the network.
+#     :param excludedParents: a set of nodes of the network.
+#     :param randomNodes: a boolean value.
+#     :return: a leaf of the network not in the excludedSet so that its parent is nt in excludedParents, or None if no such node exists. If randomNodes, then a leaf is selected from all candidates uniformly at random.
+#     """
+#     all_found = []
+#     for node in network.nodes():
+#         parent = Parent(network, node)
+#         if network.out_degree(node) == 0 and parent not in excludedParents and node not in excludedSet:
+#             if randomNodes:
+#                 all_found += [node]
+#             else:
+#                 return node
+#     if all_found and randomNodes:
+#         return random.choice(all_found)
+#     return None
+
+
+# def FindRetic(network, excludedSet=[], randomNodes=False):
+#     """
+#     Finds a (random) reticulation in a network.
+
+#     :param network: a phylogenetic network.
+#     :param excludedSet: a set of nodes of the network.
+#     :param randomNodes: a boolean value.
+#     :return: a reticulation node of the network not in the excludedSet, or None if no such node exists. If randomNodes, then a reticulation is selected from all candidates uniformly at random.
+#     """
+#     all_found = []
+#     for node in network.nodes():
+#         if node not in excludedSet and network.in_degree(node) == 2:
+#             if randomNodes:
+#                 all_found += [node]
+#             else:
+#                 return node
+#     if all_found and randomNodes:
+#         return random.choice(all_found)
+#     return None
+
+
+# def Parent(network, node, exclude=[], randomNodes=False):
+#     """
+#     Finds a parent of a node in a network.
+
+#     :param network: a phylogenetic network.
+#     :param node: a node in the network.
+#     :param exclude: a set of nodes of the network.
+#     :param randomNodes: a boolean value.
+#     :return: a parent of node that is not in the set of nodes exclude. If randomNodes, then this parent is selected uniformly at random from all candidates.
+#     """
+#     parent = None
+#     for p in network.predecessors(node):
+#         if p not in exclude:
+#             if not randomNodes:
+#                 return p
+#             elif parent == None or random.getrandbits(1):
+#                 # As there are at most two parents, we can simply replace the previous parent with probability .5 to get a random parent
+#                 parent = p
+#     return parent
+
+
+# def Child(network, node, exclude=[], randomNodes=False):
+#     """
+#     Finds a child node of a node in a network.
+
+#     :param network: a phylogenetic network.
+#     :param node: a node in the network.
+#     :param exclude: a set of nodes of the network.
+#     :param randomNodes: a boolean value.
+#     :return: a child of node that is not in the set of nodes exclude. If randomNodes, then this child node is selected uniformly at random from all candidates.
+#     """
+#     child = None
+#     for c in network.successors(node):
+#         if c not in exclude:
+#             if not randomNodes:
+#                 return c
+#             elif child == None or random.getrandbits(1):
+#                 # As there are at most two children, we can simply replace the previous child with probability .5 to get a random parent
+#                 child = c
+#     return child
+
+
+# # Returns the root of a network
+# def Root(network):
+#     """
+#     Finds the root of a phylogenetic network.
+
+#     :param network: a phylogenetic network.
+#     :return: the root node of this network.
+#     """
+#     for node in network.nodes():
+#         if network.in_degree(node) == 0:
+#             return node
+#     return None
+
+
+# # Returns a dictionary with node labels, keyed by the labels
+# def Labels(network):
+#     """
+#     Returns the correspondence between the leaves and the leaf-labels of a given network
+
+#     :param network: a phylogenetic network
+#     :return: a dictionary, where the keys are labels and the values are nodes of the network.
+#     """
+#     label_dict = dict()
+#     for node in network.nodes():
+#         node_label = network.node[node].get('label')
+#         if node_label:
+#             label_dict[node_label] = node
+#     return label_dict
+
+
+#     # Find a sequence by choosing the move that most decreases the upper bound on the number of moves
+# # This works as long as we can always decrease the bound.
+# # E.g.1, this upper bound can be the length of the sequence given by Green_Line(N1,N2), the bound can always decrease after one move, if we take the move from the GL sequence (IMPLEMENTED)
+# # TODO E.g.2, take the upper bound given by this algorithm with bound Green_Line
+# def Deep_Dive_Scored(network1, network2, head_moves=True, bound_heuristic=Green_Line):
+#     """
+#     An experimental method that returns a sequence of tail/rSPR moves from network1 to network2, using the isomorphism-building heuristic for the chosen type of moves.
+
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param head_moves: a boolean value that determines whether head moves are used in addition to tail moves. If True we use rSPR moves, if False we use only tail moves.
+#     :param bound_heuristic: a heuristic that finds a sequence between the networks quickly.
+#     :return: a sequence of moves from network1 to network2.
+#     """
+#     if Isomorphic(network1, network2):
+#         return []
+#     seq = []
+#     current_network = network1
+#     current_best = []
+#     for move in bound_heuristic(network1, network2, head_moves=head_moves):
+#         current_best += [(move[0], move[1], move[3])]
+#     if not current_best:
+#         return False
+#     done = False
+#     current_length = 0
+#     while not done:
+#         candidate_moves = AllValidMoves(current_network, tail_moves=True, head_moves=head_moves)
+#         for move in candidate_moves:
+#             candidate_network = DoMove(current_network, *move)
+#             if Isomorphic(candidate_network, network2):
+#                 return current_best[:current_length] + [move]
+#             candidate_sequence = bound_heuristic(candidate_network, network2, head_moves=head_moves)
+#             if current_length + len(candidate_sequence) + 1 < len(current_best):
+#                 current_best = current_best[:current_length] + [move]
+#                 for move2 in candidate_sequence:
+#                     current_best += [(move2[0], move2[1], move2[3])]
+#         next_move = current_best[current_length]
+#         current_network = DoMove(current_network, *next_move)
+#         current_length += 1
+#     return True
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/heuristics/red_line_heuristic.py` & `phylox-0.0.2/src/phylox/rearrangement/heuristics/red_line_heuristic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,514 +1,514 @@
-# Code used for cases 1 and 2 in the head move red line algorithm
-# returns moves1,moves2,addedNode1,addedNode2
-def RL_Case1(N1, N2, x_1, isom_N1_N2, isom_N2_N1, randomNodes=False):
-    """
-    An implementation of Algorithm 7. Finds a sequence of head moves that makes it possible to add the highest tree node x_1 to the up-closed isomrophism.
-
-    :param N1: a phylogenetic network.
-    :param N2: a phylogenetic network.
-    :param x_1: a tree node in N1.
-    :param isom_N1_N2: a dictionary, containing a partial (up-closed) isomorphism map from N1 to N2. The inverse of isom_N2_N1.
-    :param isom_N2_N1: a dictionary, containing a partial (up-closed) isomorphism map from N2 to N1. The inverse of isom_N1_N2.
-    :param randomNodes: a boolean value, determining whether the random version of this algorithm is used.
-    :return: a list of head moves in N1, a list of head moves in N2, a node of N1, a node of N2. After applying the moves to the networks, the nodes can be added to the up-closed isomorphism.
-    """
-    p_1 = Parent(N1, x_1)
-    p_2 = isom_N1_N2[p_1]
-    x_2 = Child(N2, p_2, exclude=isom_N2_N1.keys(), randomNodes=randomNodes)
-    if N2.out_degree(x_2) == 2:
-        #        print("Case tree")
-        return [], [], x_1, x_2
-    elif N2.in_degree(x_2) == 2:
-        #        print("Case retic")
-        c_2 = FindTreeNode(N2, excludedSet=isom_N2_N1.keys(), randomNodes=randomNodes)
-        t_2 = Parent(N2, c_2)
-        b_2 = Child(N2, c_2, exclude=[x_2], randomNodes=randomNodes)
-        #        print(x_1,p_1,p_2,x_2,c_2,t_2,b_2)
-        # TODO: Not in the latex algo, just a minor improvement:
-        # If the other child $c_2$ of $p_2$ is a retic, then we can add it.
-        if p_2 == t_2:
-            return [], [], x_1, c_2
-        if check_movable(N2, (p_2, x_2), x_2):
-            q_2 = Parent(N2, x_2, exclude=[p_2])
-            if x_2 == t_2:
-                #                print("(p,x) movable and x=t")
-                return [], [((q_2, x_2), x_2, (c_2, b_2))], x_1, c_2
-            else:
-                #                print("(p,x) movable and x!=t")
-                return [], [((p_2, x_2), x_2, (t_2, c_2)), ((t_2, x_2), x_2, (c_2, b_2))], x_1, c_2
-        else:
-            d_2 = Child(N2, x_2)
-            z_2 = Parent(N2, x_2, exclude=[p_2])
-            # Find a leaf with parent not equal to d_2
-            l_2 = FindLeaf(N2, excludedParents=[d_2], randomNodes=randomNodes)
-            w_2 = Parent(N2, l_2)
-            #            print("other")
-            #            print(d_2,z_2,w_2,l_2)
-            if l_2 == b_2:  # after the first move, b_2 is not a child of c_2 anymore, so we fix this by taking the other child of c_2 as b_2
-                b_2 = Child(N2, c_2, exclude=[l_2, x_2], randomNodes=randomNodes)
-            if d_2 == t_2:  # i.e., if, after the first move, x_2 is the parent of c_2
-                return [], [((z_2, d_2), d_2, (w_2, l_2)), ((z_2, x_2), x_2, (c_2, b_2))], x_1, c_2
-            else:
-                return [], [((z_2, d_2), d_2, (w_2, l_2)), ((p_2, x_2), x_2, (t_2, c_2)),
-                            ((t_2, x_2), x_2, (c_2, b_2))], x_1, c_2
-    else:
-        #        print("Case leaf")
-        c_2 = FindTreeNode(N2, excludedSet=isom_N2_N1.keys(), randomNodes=randomNodes)
-        t_2 = Parent(N2, c_2)
-
-        if p_2 == t_2:
-            #            print("no move")
-            return [], [], x_1, c_2
-
-            # Find a reticulation arc (s_2,r_2) that can be moved to (p_2,x_2)
-        # No randomness required, because this arc will end up at its original position again.
-        s_2 = None
-        r_2 = None
-        for node in N2.nodes():
-            if N2.in_degree(node) == 2:
-                for parent in N2.predecessors(node):
-                    if parent != p_2 and check_movable(N2, (parent, node), node):
-                        s_2 = parent
-                        r_2 = node
-            if s_2 != None:
-                break
-        q_2 = Parent(N2, r_2, exclude=[s_2])
-        w_2 = Child(N2, r_2)
-        #        print(p_2,x_2,t_2,c_2,s_2,q_2,r_2,w_2)
-        if r_2 == p_2:
-            #            print("r=p")
-            if s_2 == t_2:
-                return [], [((q_2, p_2), p_2, (t_2, c_2))], x_1, c_2
-            elif q_2 == t_2:
-                return [], [((s_2, p_2), p_2, (t_2, c_2))], x_1, c_2
-            else:
-                return [], [((s_2, p_2), p_2, (t_2, c_2)), ((t_2, p_2), p_2, (q_2, x_2)),
-                            ((q_2, p_2), p_2, (s_2, c_2))], x_1, c_2
-        if r_2 == t_2:
-            #            print("r=t")
-            if p_2 == q_2:
-                return [], [((s_2, r_2), r_2, (p_2, x_2))], x_1, c_2
-            else:
-                return [], [((s_2, r_2), r_2, (p_2, x_2)), ((p_2, r_2), r_2, (q_2, c_2)),
-                            ((q_2, r_2), r_2, (s_2, x_2))], x_1, c_2
-        if s_2 != t_2:
-            #            print("s!=t")
-            return [], [((s_2, r_2), r_2, (p_2, x_2)), ((p_2, r_2), r_2, (t_2, c_2)), ((t_2, r_2), r_2, (s_2, x_2)),
-                        ((s_2, r_2), r_2, (q_2, w_2))], x_1, c_2
-        else:
-            #            print("other")
-            return [], [((s_2, r_2), r_2, (p_2, x_2)), ((p_2, r_2), r_2, (s_2, c_2)),
-                        ((s_2, r_2), r_2, (q_2, w_2))], x_1, c_2
-
-        # Code used for case 3 in the head move red line algorithm
-
-
-# returns moves1,moves2,addedNode1,addedNode2
-def RL_Case3(N1, N2, x_1, isom_N1_N2, isom_N2_N1, randomNodes=False):
-    """
-    An implementation of Algorithm 8. Finds a sequence of head moves that makes it possible to add the highest reticulation x_1 to the up-closed isomrophism.
-
-    :param N1: a phylogenetic network.
-    :param N2: a phylogenetic network.
-    :param x_1: a highest reticulation node in N1.
-    :param isom_N1_N2: a dictionary, containing a partial (up-closed) isomorphism map from N1 to N2. The inverse of isom_N2_N1.
-    :param isom_N2_N1: a dictionary, containing a partial (up-closed) isomorphism map from N2 to N1. The inverse of isom_N1_N2.
-    :param randomNodes: a boolean value, determining whether the random version of this algorithm is used.
-    :return: a list of head moves in N1, a list of head moves in N2, a node of N1, a node of N2. After applying the moves to the networks, the nodes can be added to the up-closed isomorphism.
-    """
-    p_1 = Parent(N1, x_1)
-    q_1 = Parent(N1, x_1, exclude=[p_1])
-    p_2 = isom_N1_N2[p_1]
-    cp_2 = Child(N2, p_2, exclude=isom_N2_N1.keys(), randomNodes=randomNodes)
-    q_2 = isom_N1_N2[q_1]
-    cq_2 = Child(N2, q_2, exclude=isom_N2_N1.keys(), randomNodes=randomNodes)
-
-    # at least one tree node, so give up
-    if N2.out_degree(cp_2) == 2 or N2.out_degree(cq_2) == 2:
-        # The proof does not provide a sequence when at least of the nodes cp_2 or cq_2 is a tree node
-        # TODO: If one of (p_2,cp_2) or (q_2,cq_2) is movable, we can still do something quite similar to what follows in the last case
-        return [], [], None, None
-    # Case 3ai
-    if cp_2 == cq_2:
-        #        print("no move")
-        return [], [], x_1, cp_2
-    # Case 3av
-    elif N2.out_degree(cp_2) == 0 and N2.out_degree(cq_2) == 0:
-        #        print("both leaves")
-        # Find a head-movable arc (s_2,r_2)
-        # As each reticulation node has a movable arc, we pick a random reticulation, and then a random movable arc incident to this node
-        r_2 = FindRetic(N2, excludedSet=isom_N2_N1.keys(), randomNodes=randomNodes)
-        s_2 = None
-        for parent in N2.predecessors(r_2):
-            if check_movable(N2, (parent, r_2), r_2):
-                if not randomNodes:
-                    s_2 = parent
-                    break
-                elif s_2 == None or random.getrandbits(1):
-                    s_2 = parent
-        if s_2 == p_2:
-            #            print("s=p")
-            return [], [((s_2, r_2), r_2, (q_2, cq_2)), ((q_2, r_2), r_2, (p_2, cp_2))], x_1, r_2
-        else:
-            #            print("s!=p")
-            return [], [((s_2, r_2), r_2, (p_2, cp_2)), ((p_2, r_2), r_2, (q_2, cq_2))], x_1, r_2
-    # Cases 3a(ii, iii, iv)
-    else:
-        #        print("at least one non-leaf")
-        if nx.has_path(N2, cq_2, cp_2) or N2.out_degree(cp_2) == 0:
-            # Swap p and q
-            q_2, p_2 = p_2, q_2
-            cp_2, cq_2 = cq_2, cp_2
-        #        print(p_2 , q_2, cp_2, cq_2)
-        if check_movable(N2, (p_2, cp_2), cp_2):
-            #            print("movable cp_2")
-            return [], [((p_2, cp_2), cp_2, (q_2, cq_2))], x_1, cp_2
-        else:
-            #            print("immovable cp_2")
-            z = Child(N2, cp_2)
-            t = Parent(N2, cp_2, exclude=[p_2])
-            if t == q_2:
-                return [], [], x_1, cp_2
-            return [], [((cp_2, z), z, (q_2, cq_2)), ((t, cp_2), cp_2, (z, cq_2))], x_1, z
-
-
-# Permutes the leaves of a network so that it becomes leaf isomorphic, provided the networks were already (non-labeled) ismorphic
-def Permute_Leaves_Head(network1, network2, isom_1_2, isom_2_1, label_dict_1, label_dict_2):
-    """
-    An implementation of Algorithm 9. Determines a sequence of head moves that makes two isomorphic networks labeled isomorphic.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param isom_1_2: a dictionary, containing a partial (up-closed) isomorphism map from network1 to network2. The inverse of isom_2_1.
-    :param isom_2_1: a dictionary, containing a partial (up-closed) isomorphism map from network2 to network1. The inverse of isom_1_2.
-    :param label_dict_1: a dictionary, containing the correspondence of nodes of network1 with the leaf labels: keys are labels and values are nodes.
-    :param label_dict_2: a dictionary, containing the correspondence of nodes of network2 with the leaf labels: keys are labels and values are nodes.
-    :return: a list of head moves that turns network1 into network2.
-    """
-    #    for i,k in isom_1_2.items():
-    #        print(i,k)
-    sequence = []
-    # labeldict[label]=leaf
-    Y = list(label_dict_1.values())
-    cycles = []
-    while len(Y) > 0:
-        y1_1 = Y.pop()
-        y_2 = isom_1_2[y1_1]
-        cycle = [y1_1]
-        while network2.node[y_2].get('label') != network1.node[cycle[0]].get('label'):
-            y_new_1 = label_dict_1[network2.node[y_2].get('label')]
-            #            if len(set(network1.predecessors(cycle[-1]))&set(network1.predecessors(y_new_1)))==0:#cycle[-1] and y_new_1 have NO common parent
-            #                cycle+=[y_new_1]
-            cycle += [y_new_1]
-
-            y_2 = isom_1_2[y_new_1]
-            Y.remove(y_new_1)
-        if len(cycle) > 1:
-            cycles += [list(reversed(cycle))]
-    #    print("cycles",cycles)
-
-    t = None
-    r = None
-    for node in network1:
-        if network1.in_degree(node) == 2:
-            for parent in network1.predecessors(node):
-                if check_movable(network1, (parent, node), node):
-                    t = parent
-                    r = node
-        if r:
-            break
-    c_last = Child(network1, r)  # In the proof: c', the child of r in N
-    s_last = Parent(network1, r, exclude=[t])
-
-    for cycle in cycles:
-        c = cycle
-
-        # shift the cycle by one of t is the parent of the last leaf in the cycle
-        if t in network1.predecessors(cycle[-1]):
-            c = [cycle[-1]] + cycle[:-1]
-
-        # Skip the first move if the head r of the moving arc is already above the last leaf in the cycle
-        p_last = Parent(network1, c[-1])
-        if r != p_last:
-            move = ((t, r), r, (p_last, c[-1]))
-            sequence.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
-            network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
-        moved_arc = (t, r)
-
-        c_last_before = c_last
-
-        for i in reversed(range(len(c))):
-            p_i = Parent(network1, r, exclude=[moved_arc[0]])
-            p_im1 = Parent(network1, c[i - 1])
-            # if p_i==p_im1, then two consecutive leaves are in a cherry, and we can skip one of them.
-            if p_i == p_im1:
-                continue
-            #                print("do nothing, swapping a cherry")
-            else:
-                move = ((p_i, r), r, (p_im1, c[i - 1]))
-                sequence.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
-                network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
-                moved_arc = (p_i, r)
-            # If c in the `original position' (s,c) of (t,r) is permuted by the cycle, then we need to change this original position accordingly
-            if c[i] == c_last_before:
-                c_last = c[i - 1]
-
-    # Put the moving arc back to its original position
-    # The proof does this for every cycle, but can also be done once at the end
-    if (s_last, c_last) in network1.edges():
-        # (t,r) might already be back at this position
-        move = ((t, r), r, (s_last, c_last))
-        sequence.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
-        network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
-
-    #    print("isomorphic", Isomorphic(network1,network2))
-    #    for s in sequence:
-    #        print(s[0])
-    return sequence
-
-
-# A heuristic for finding a head move sequence between two networks.
-def Red_Line(network1, network2):
-    """
-    An implementation of Algorithm 10. Finds a sequence of head moves from network1 to network2 by building an up-closed isomorphism.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :return: A list of head moves from network1 to network2.
-    """
-    # Find the root and labels of the networks
-    root1 = Root(network1)
-    root2 = Root(network2)
-    label_dict_1 = Labels(network1)
-    label_dict_2 = Labels(network2)
-
-    # initialize isomorphism
-    isom_1_2 = dict()
-    isom_1_2[root1] = root2
-    isom_2_1 = dict()
-    isom_2_1[root2] = root1
-    isom_size = 1
-
-    # Check if the roots are of the same type
-    if network1.out_degree(root1) != network2.out_degree(root2):
-        return False
-
-    # Keep track of the size of the isomorphism and the size it is at the end of the red line algorithm
-    goal_size = len(network1) - len(label_dict_1)
-
-    # init lists of sequence of moves
-    # list of (moving_edge,moving_endpoint,from_edge,to_edge)
-    seq_from_1 = []
-    seq_from_2 = []
-    # TODO keep track of highest nodes?
-
-    # Do the red line algorithm
-    while (isom_size < goal_size):
-        highest_tree_node_network1, highest_retic_network1 = HighestNodesBelow(network1, isom_1_2.keys())
-        highest_tree_node_network2, highest_retic_network2 = HighestNodesBelow(network2, isom_2_1.keys())
-
-        # Case1
-        if highest_tree_node_network1 != None:
-            moves_network_1, moves_network_2, added_node_network1, added_node_network2 = RL_Case1(network1, network2,
-                                                                                                  highest_tree_node_network1,
-                                                                                                  isom_1_2, isom_2_1)
-        # Case2
-        elif highest_tree_node_network2 != None:
-            moves_network_2, moves_network_1, added_node_network2, added_node_network1 = RL_Case1(network2, network1,
-                                                                                                  highest_tree_node_network2,
-                                                                                                  isom_2_1, isom_1_2)
-        # Case3
-        else:
-            moves_network_1, moves_network_2, added_node_network1, added_node_network2 = RL_Case3(network1, network2,
-                                                                                                  highest_retic_network1,
-                                                                                                  isom_1_2, isom_2_1)
-
-        # Now perform the moves and update the isomorphism
-        isom_1_2[added_node_network1] = added_node_network2
-        isom_2_1[added_node_network2] = added_node_network1
-        for move in moves_network_1:
-            seq_from_1.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
-            network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
-        for move in moves_network_2:
-            seq_from_2.append((move[0], move[1], From_Edge(network2, move[0], move[1]), move[2]))
-            network2 = DoMove(network2, move[0], move[1], move[2], check_validity=False)
-        isom_size += 1
-    # TESTING FOR CORRECTNESS WHILE RUNNING
-    #        if not nx.is_isomorphic(network1.subgraph(isom_1_2.keys()),network2.subgraph(isom_2_1.keys())):
-    #            print("not unlabeled isom")
-    #            print(seq_from_1)
-    #            print(seq_from_2)
-    #            print(network1.subgraph(isom_1_2.keys()).edges())
-    #            print(network2.subgraph(isom_2_1.keys()).edges())
-
-    # TODO Debugging, remove after for speed
-    #    if not nx.is_isomorphic(network1,network2):
-    #        print("not unlabeled isom")
-    #        print(network1.edges())
-    #        print(network2.edges())
-    #    else:
-    #        print("unlabeled isomorphic :)")
-
-    # Add the leaves to the isomorphism
-    for node_1 in network1.nodes():
-        if network1.out_degree(node_1) == 0:
-            parent_1 = Parent(network1, node_1)
-            parent_2 = isom_1_2[parent_1]
-            node_2 = Child(network2, parent_2, exclude=isom_2_1.keys())
-            isom_1_2[node_1] = node_2
-            isom_2_1[node_2] = node_1
-
-    # Permute the leaves
-    seq_permute = Permute_Leaves_Head(network1, network2, isom_1_2, isom_2_1, label_dict_1, label_dict_2)
-
-    # invert seq_from_2, rename to node names of network1, and append to seq_from_1
-    return seq_from_1 + seq_permute + ReplaceNodeNamesInMoveSequence(InvertMoveSequence(seq_from_2), isom_2_1)
-
-
-def Red_Line_Random(network1, network2, repeats=1):
-    """
-    Finds a sequence of head moves from network1 to network2 by randomly building an up-closed isomorphism a number of times, and only keeping the shortest sequence.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :param repeats: an integer, determining how many repeats of Red_Line_Random_Single are performed.
-    :return: A list of head moves from network1 to network2.
-    """
-    best_seq = None
-    for i in range(repeats):
-        candidate_seq = Red_Line_Random_Single(network1, network2)
-        if best_seq == None or len(best_seq) > len(candidate_seq):
-            best_seq = candidate_seq
-    return best_seq
-
-
-def Red_Line_Random_Single(network1, network2):
-    """
-    An implementation of Algorithm 11. Finds a sequence of head moves from network1 to network2 by building randomly an up-closed isomorphism.
-
-    :param network1: a phylogenetic network.
-    :param network2: a phylogenetic network.
-    :return: A list of head moves from network1 to network2.
-    """
-    # Find the root and labels of the networks
-    root1 = Root(network1)
-    root2 = Root(network2)
-    label_dict_1 = Labels(network1)
-    label_dict_2 = Labels(network2)
-
-    # initialize isomorphism
-    isom_1_2 = dict()
-    isom_1_2[root1] = root2
-    isom_2_1 = dict()
-    isom_2_1[root2] = root1
-    isom_size = 1
-
-    # Check if the roots are of the same type
-    if network1.out_degree(root1) != network2.out_degree(root2):
-        return False
-
-    # Keep track of the size of the isomorphism and the size it is at the end of the red line algorithm
-    goal_size = len(network1) - len(label_dict_1)
-
-    # init lists of sequence of moves
-    # list of (moving_edge,moving_endpoint,from_edge,to_edge)
-    seq_from_1 = []
-    seq_from_2 = []
-    # TODO keep track of highest nodes?
-
-    # Do the red line algorithm
-    while (isom_size < goal_size):
-        highest_tree_node_network1, highest_retic_network1 = HighestNodesBelow(network1, isom_1_2.keys(), allnodes=True)
-        highest_tree_node_network2, highest_retic_network2 = HighestNodesBelow(network2, isom_2_1.keys(), allnodes=True)
-
-        # Construct a list of all highest nodes in a tuple with the corresponding network (in random order)
-        # I.e. If u is a highest node of network one, it will appear in the list as (u,1)
-        highest_nodes_network1 = [(u, 1) for u in highest_tree_node_network1 + highest_retic_network1]
-        highest_nodes_network2 = [(u, 2) for u in highest_tree_node_network2 + highest_retic_network2]
-        candidate_highest_nodes = highest_nodes_network1 + highest_nodes_network2
-        random.shuffle(candidate_highest_nodes)
-
-        # As some cases do not give an addition to the isom, we continue trying lowest nodes until we find one that does.
-        for highest_node, network_number in candidate_highest_nodes:
-            u = highest_node
-            # Case1
-            if network_number == 1 and network1.in_degree(u) == 1:
-                #                print("Case 1")
-                moves_network_1, moves_network_2, added_node_network1, added_node_network2 = RL_Case1(network1,
-                                                                                                      network2, u,
-                                                                                                      isom_1_2,
-                                                                                                      isom_2_1,
-                                                                                                      randomNodes=True)
-                break
-            # Case2
-            elif network_number == 2 and network2.in_degree(u) == 1:
-                #                print("Case 2")
-                moves_network_2, moves_network_1, added_node_network2, added_node_network1 = RL_Case1(network2,
-                                                                                                      network1, u,
-                                                                                                      isom_2_1,
-                                                                                                      isom_1_2,
-                                                                                                      randomNodes=True)
-                break
-            # Case3
-            elif network_number == 1 and network1.in_degree(u) == 2:
-                #                print("Case 3")
-                moves_network_1, moves_network_2, added_node_network1, added_node_network2 = RL_Case3(network1,
-                                                                                                      network2, u,
-                                                                                                      isom_1_2,
-                                                                                                      isom_2_1,
-                                                                                                      randomNodes=True)
-                if added_node_network2:
-                    break
-            # Case3'
-            elif network_number == 2 and network2.in_degree(u) == 2:
-                #                print("Case 3'")
-                moves_network_2, moves_network_1, added_node_network2, added_node_network1 = RL_Case3(network2,
-                                                                                                      network1, u,
-                                                                                                      isom_2_1,
-                                                                                                      isom_1_2,
-                                                                                                      randomNodes=True)
-                if added_node_network2:
-                    break
-
-        # Now perform the moves and update the isomorphism
-        isom_1_2[added_node_network1] = added_node_network2
-        isom_2_1[added_node_network2] = added_node_network1
-        for move in moves_network_1:
-            seq_from_1.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
-            network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
-        for move in moves_network_2:
-            seq_from_2.append((move[0], move[1], From_Edge(network2, move[0], move[1]), move[2]))
-            network2 = DoMove(network2, move[0], move[1], move[2], check_validity=False)
-        isom_size += 1
-    # TESTING FOR CORRECTNESS WHILE RUNNING
-    #        if not nx.is_isomorphic(network1.subgraph(isom_1_2.keys()),network2.subgraph(isom_2_1.keys())):
-    #            print("not unlabeled isom")
-    #            print(seq_from_1)
-    #            print(seq_from_2)
-    #            print(network1.subgraph(isom_1_2.keys()).edges())
-    #            print(network2.subgraph(isom_2_1.keys()).edges())
-    #            print(network1.edges())
-    #            print(network2.edges())
-
-    # TODO Debugging, remove after for speed
-    #    if not nx.is_isomorphic(network1,network2):
-    #        print("not unlabeled isom")
-    #        print(network1.edges())
-    #        print(network2.edges())
-    #    else:
-    #        print("unlabeled isomorphic :)")
-
-    # Add the leaves to the isomorphism
-    for node_1 in network1.nodes():
-        if network1.out_degree(node_1) == 0:
-            parent_1 = Parent(network1, node_1)
-            parent_2 = isom_1_2[parent_1]
-            node_2 = Child(network2, parent_2, exclude=isom_2_1.keys())
-            isom_1_2[node_1] = node_2
-            isom_2_1[node_2] = node_1
+# # Code used for cases 1 and 2 in the head move red line algorithm
+# # returns moves1,moves2,addedNode1,addedNode2
+# def RL_Case1(N1, N2, x_1, isom_N1_N2, isom_N2_N1, randomNodes=False):
+#     """
+#     An implementation of Algorithm 7. Finds a sequence of head moves that makes it possible to add the highest tree node x_1 to the up-closed isomrophism.
+
+#     :param N1: a phylogenetic network.
+#     :param N2: a phylogenetic network.
+#     :param x_1: a tree node in N1.
+#     :param isom_N1_N2: a dictionary, containing a partial (up-closed) isomorphism map from N1 to N2. The inverse of isom_N2_N1.
+#     :param isom_N2_N1: a dictionary, containing a partial (up-closed) isomorphism map from N2 to N1. The inverse of isom_N1_N2.
+#     :param randomNodes: a boolean value, determining whether the random version of this algorithm is used.
+#     :return: a list of head moves in N1, a list of head moves in N2, a node of N1, a node of N2. After applying the moves to the networks, the nodes can be added to the up-closed isomorphism.
+#     """
+#     p_1 = Parent(N1, x_1)
+#     p_2 = isom_N1_N2[p_1]
+#     x_2 = Child(N2, p_2, exclude=isom_N2_N1.keys(), randomNodes=randomNodes)
+#     if N2.out_degree(x_2) == 2:
+#         #        print("Case tree")
+#         return [], [], x_1, x_2
+#     elif N2.in_degree(x_2) == 2:
+#         #        print("Case retic")
+#         c_2 = FindTreeNode(N2, excludedSet=isom_N2_N1.keys(), randomNodes=randomNodes)
+#         t_2 = Parent(N2, c_2)
+#         b_2 = Child(N2, c_2, exclude=[x_2], randomNodes=randomNodes)
+#         #        print(x_1,p_1,p_2,x_2,c_2,t_2,b_2)
+#         # TODO: Not in the latex algo, just a minor improvement:
+#         # If the other child $c_2$ of $p_2$ is a retic, then we can add it.
+#         if p_2 == t_2:
+#             return [], [], x_1, c_2
+#         if check_movable(N2, (p_2, x_2), x_2):
+#             q_2 = Parent(N2, x_2, exclude=[p_2])
+#             if x_2 == t_2:
+#                 #                print("(p,x) movable and x=t")
+#                 return [], [((q_2, x_2), x_2, (c_2, b_2))], x_1, c_2
+#             else:
+#                 #                print("(p,x) movable and x!=t")
+#                 return [], [((p_2, x_2), x_2, (t_2, c_2)), ((t_2, x_2), x_2, (c_2, b_2))], x_1, c_2
+#         else:
+#             d_2 = Child(N2, x_2)
+#             z_2 = Parent(N2, x_2, exclude=[p_2])
+#             # Find a leaf with parent not equal to d_2
+#             l_2 = FindLeaf(N2, excludedParents=[d_2], randomNodes=randomNodes)
+#             w_2 = Parent(N2, l_2)
+#             #            print("other")
+#             #            print(d_2,z_2,w_2,l_2)
+#             if l_2 == b_2:  # after the first move, b_2 is not a child of c_2 anymore, so we fix this by taking the other child of c_2 as b_2
+#                 b_2 = Child(N2, c_2, exclude=[l_2, x_2], randomNodes=randomNodes)
+#             if d_2 == t_2:  # i.e., if, after the first move, x_2 is the parent of c_2
+#                 return [], [((z_2, d_2), d_2, (w_2, l_2)), ((z_2, x_2), x_2, (c_2, b_2))], x_1, c_2
+#             else:
+#                 return [], [((z_2, d_2), d_2, (w_2, l_2)), ((p_2, x_2), x_2, (t_2, c_2)),
+#                             ((t_2, x_2), x_2, (c_2, b_2))], x_1, c_2
+#     else:
+#         #        print("Case leaf")
+#         c_2 = FindTreeNode(N2, excludedSet=isom_N2_N1.keys(), randomNodes=randomNodes)
+#         t_2 = Parent(N2, c_2)
+
+#         if p_2 == t_2:
+#             #            print("no move")
+#             return [], [], x_1, c_2
+
+#             # Find a reticulation arc (s_2,r_2) that can be moved to (p_2,x_2)
+#         # No randomness required, because this arc will end up at its original position again.
+#         s_2 = None
+#         r_2 = None
+#         for node in N2.nodes():
+#             if N2.in_degree(node) == 2:
+#                 for parent in N2.predecessors(node):
+#                     if parent != p_2 and check_movable(N2, (parent, node), node):
+#                         s_2 = parent
+#                         r_2 = node
+#             if s_2 != None:
+#                 break
+#         q_2 = Parent(N2, r_2, exclude=[s_2])
+#         w_2 = Child(N2, r_2)
+#         #        print(p_2,x_2,t_2,c_2,s_2,q_2,r_2,w_2)
+#         if r_2 == p_2:
+#             #            print("r=p")
+#             if s_2 == t_2:
+#                 return [], [((q_2, p_2), p_2, (t_2, c_2))], x_1, c_2
+#             elif q_2 == t_2:
+#                 return [], [((s_2, p_2), p_2, (t_2, c_2))], x_1, c_2
+#             else:
+#                 return [], [((s_2, p_2), p_2, (t_2, c_2)), ((t_2, p_2), p_2, (q_2, x_2)),
+#                             ((q_2, p_2), p_2, (s_2, c_2))], x_1, c_2
+#         if r_2 == t_2:
+#             #            print("r=t")
+#             if p_2 == q_2:
+#                 return [], [((s_2, r_2), r_2, (p_2, x_2))], x_1, c_2
+#             else:
+#                 return [], [((s_2, r_2), r_2, (p_2, x_2)), ((p_2, r_2), r_2, (q_2, c_2)),
+#                             ((q_2, r_2), r_2, (s_2, x_2))], x_1, c_2
+#         if s_2 != t_2:
+#             #            print("s!=t")
+#             return [], [((s_2, r_2), r_2, (p_2, x_2)), ((p_2, r_2), r_2, (t_2, c_2)), ((t_2, r_2), r_2, (s_2, x_2)),
+#                         ((s_2, r_2), r_2, (q_2, w_2))], x_1, c_2
+#         else:
+#             #            print("other")
+#             return [], [((s_2, r_2), r_2, (p_2, x_2)), ((p_2, r_2), r_2, (s_2, c_2)),
+#                         ((s_2, r_2), r_2, (q_2, w_2))], x_1, c_2
+
+#         # Code used for case 3 in the head move red line algorithm
+
+
+# # returns moves1,moves2,addedNode1,addedNode2
+# def RL_Case3(N1, N2, x_1, isom_N1_N2, isom_N2_N1, randomNodes=False):
+#     """
+#     An implementation of Algorithm 8. Finds a sequence of head moves that makes it possible to add the highest reticulation x_1 to the up-closed isomrophism.
+
+#     :param N1: a phylogenetic network.
+#     :param N2: a phylogenetic network.
+#     :param x_1: a highest reticulation node in N1.
+#     :param isom_N1_N2: a dictionary, containing a partial (up-closed) isomorphism map from N1 to N2. The inverse of isom_N2_N1.
+#     :param isom_N2_N1: a dictionary, containing a partial (up-closed) isomorphism map from N2 to N1. The inverse of isom_N1_N2.
+#     :param randomNodes: a boolean value, determining whether the random version of this algorithm is used.
+#     :return: a list of head moves in N1, a list of head moves in N2, a node of N1, a node of N2. After applying the moves to the networks, the nodes can be added to the up-closed isomorphism.
+#     """
+#     p_1 = Parent(N1, x_1)
+#     q_1 = Parent(N1, x_1, exclude=[p_1])
+#     p_2 = isom_N1_N2[p_1]
+#     cp_2 = Child(N2, p_2, exclude=isom_N2_N1.keys(), randomNodes=randomNodes)
+#     q_2 = isom_N1_N2[q_1]
+#     cq_2 = Child(N2, q_2, exclude=isom_N2_N1.keys(), randomNodes=randomNodes)
+
+#     # at least one tree node, so give up
+#     if N2.out_degree(cp_2) == 2 or N2.out_degree(cq_2) == 2:
+#         # The proof does not provide a sequence when at least of the nodes cp_2 or cq_2 is a tree node
+#         # TODO: If one of (p_2,cp_2) or (q_2,cq_2) is movable, we can still do something quite similar to what follows in the last case
+#         return [], [], None, None
+#     # Case 3ai
+#     if cp_2 == cq_2:
+#         #        print("no move")
+#         return [], [], x_1, cp_2
+#     # Case 3av
+#     elif N2.out_degree(cp_2) == 0 and N2.out_degree(cq_2) == 0:
+#         #        print("both leaves")
+#         # Find a head-movable arc (s_2,r_2)
+#         # As each reticulation node has a movable arc, we pick a random reticulation, and then a random movable arc incident to this node
+#         r_2 = FindRetic(N2, excludedSet=isom_N2_N1.keys(), randomNodes=randomNodes)
+#         s_2 = None
+#         for parent in N2.predecessors(r_2):
+#             if check_movable(N2, (parent, r_2), r_2):
+#                 if not randomNodes:
+#                     s_2 = parent
+#                     break
+#                 elif s_2 == None or random.getrandbits(1):
+#                     s_2 = parent
+#         if s_2 == p_2:
+#             #            print("s=p")
+#             return [], [((s_2, r_2), r_2, (q_2, cq_2)), ((q_2, r_2), r_2, (p_2, cp_2))], x_1, r_2
+#         else:
+#             #            print("s!=p")
+#             return [], [((s_2, r_2), r_2, (p_2, cp_2)), ((p_2, r_2), r_2, (q_2, cq_2))], x_1, r_2
+#     # Cases 3a(ii, iii, iv)
+#     else:
+#         #        print("at least one non-leaf")
+#         if nx.has_path(N2, cq_2, cp_2) or N2.out_degree(cp_2) == 0:
+#             # Swap p and q
+#             q_2, p_2 = p_2, q_2
+#             cp_2, cq_2 = cq_2, cp_2
+#         #        print(p_2 , q_2, cp_2, cq_2)
+#         if check_movable(N2, (p_2, cp_2), cp_2):
+#             #            print("movable cp_2")
+#             return [], [((p_2, cp_2), cp_2, (q_2, cq_2))], x_1, cp_2
+#         else:
+#             #            print("immovable cp_2")
+#             z = Child(N2, cp_2)
+#             t = Parent(N2, cp_2, exclude=[p_2])
+#             if t == q_2:
+#                 return [], [], x_1, cp_2
+#             return [], [((cp_2, z), z, (q_2, cq_2)), ((t, cp_2), cp_2, (z, cq_2))], x_1, z
+
+
+# # Permutes the leaves of a network so that it becomes leaf isomorphic, provided the networks were already (non-labeled) ismorphic
+# def Permute_Leaves_Head(network1, network2, isom_1_2, isom_2_1, label_dict_1, label_dict_2):
+#     """
+#     An implementation of Algorithm 9. Determines a sequence of head moves that makes two isomorphic networks labeled isomorphic.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param isom_1_2: a dictionary, containing a partial (up-closed) isomorphism map from network1 to network2. The inverse of isom_2_1.
+#     :param isom_2_1: a dictionary, containing a partial (up-closed) isomorphism map from network2 to network1. The inverse of isom_1_2.
+#     :param label_dict_1: a dictionary, containing the correspondence of nodes of network1 with the leaf labels: keys are labels and values are nodes.
+#     :param label_dict_2: a dictionary, containing the correspondence of nodes of network2 with the leaf labels: keys are labels and values are nodes.
+#     :return: a list of head moves that turns network1 into network2.
+#     """
+#     #    for i,k in isom_1_2.items():
+#     #        print(i,k)
+#     sequence = []
+#     # labeldict[label]=leaf
+#     Y = list(label_dict_1.values())
+#     cycles = []
+#     while len(Y) > 0:
+#         y1_1 = Y.pop()
+#         y_2 = isom_1_2[y1_1]
+#         cycle = [y1_1]
+#         while network2.node[y_2].get('label') != network1.node[cycle[0]].get('label'):
+#             y_new_1 = label_dict_1[network2.node[y_2].get('label')]
+#             #            if len(set(network1.predecessors(cycle[-1]))&set(network1.predecessors(y_new_1)))==0:#cycle[-1] and y_new_1 have NO common parent
+#             #                cycle+=[y_new_1]
+#             cycle += [y_new_1]
+
+#             y_2 = isom_1_2[y_new_1]
+#             Y.remove(y_new_1)
+#         if len(cycle) > 1:
+#             cycles += [list(reversed(cycle))]
+#     #    print("cycles",cycles)
+
+#     t = None
+#     r = None
+#     for node in network1:
+#         if network1.in_degree(node) == 2:
+#             for parent in network1.predecessors(node):
+#                 if check_movable(network1, (parent, node), node):
+#                     t = parent
+#                     r = node
+#         if r:
+#             break
+#     c_last = Child(network1, r)  # In the proof: c', the child of r in N
+#     s_last = Parent(network1, r, exclude=[t])
+
+#     for cycle in cycles:
+#         c = cycle
+
+#         # shift the cycle by one of t is the parent of the last leaf in the cycle
+#         if t in network1.predecessors(cycle[-1]):
+#             c = [cycle[-1]] + cycle[:-1]
+
+#         # Skip the first move if the head r of the moving arc is already above the last leaf in the cycle
+#         p_last = Parent(network1, c[-1])
+#         if r != p_last:
+#             move = ((t, r), r, (p_last, c[-1]))
+#             sequence.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
+#             network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
+#         moved_arc = (t, r)
+
+#         c_last_before = c_last
+
+#         for i in reversed(range(len(c))):
+#             p_i = Parent(network1, r, exclude=[moved_arc[0]])
+#             p_im1 = Parent(network1, c[i - 1])
+#             # if p_i==p_im1, then two consecutive leaves are in a cherry, and we can skip one of them.
+#             if p_i == p_im1:
+#                 continue
+#             #                print("do nothing, swapping a cherry")
+#             else:
+#                 move = ((p_i, r), r, (p_im1, c[i - 1]))
+#                 sequence.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
+#                 network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
+#                 moved_arc = (p_i, r)
+#             # If c in the `original position' (s,c) of (t,r) is permuted by the cycle, then we need to change this original position accordingly
+#             if c[i] == c_last_before:
+#                 c_last = c[i - 1]
+
+#     # Put the moving arc back to its original position
+#     # The proof does this for every cycle, but can also be done once at the end
+#     if (s_last, c_last) in network1.edges():
+#         # (t,r) might already be back at this position
+#         move = ((t, r), r, (s_last, c_last))
+#         sequence.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
+#         network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
+
+#     #    print("isomorphic", Isomorphic(network1,network2))
+#     #    for s in sequence:
+#     #        print(s[0])
+#     return sequence
+
+
+# # A heuristic for finding a head move sequence between two networks.
+# def Red_Line(network1, network2):
+#     """
+#     An implementation of Algorithm 10. Finds a sequence of head moves from network1 to network2 by building an up-closed isomorphism.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :return: A list of head moves from network1 to network2.
+#     """
+#     # Find the root and labels of the networks
+#     root1 = Root(network1)
+#     root2 = Root(network2)
+#     label_dict_1 = Labels(network1)
+#     label_dict_2 = Labels(network2)
+
+#     # initialize isomorphism
+#     isom_1_2 = dict()
+#     isom_1_2[root1] = root2
+#     isom_2_1 = dict()
+#     isom_2_1[root2] = root1
+#     isom_size = 1
+
+#     # Check if the roots are of the same type
+#     if network1.out_degree(root1) != network2.out_degree(root2):
+#         return False
+
+#     # Keep track of the size of the isomorphism and the size it is at the end of the red line algorithm
+#     goal_size = len(network1) - len(label_dict_1)
+
+#     # init lists of sequence of moves
+#     # list of (moving_edge,moving_endpoint,from_edge,to_edge)
+#     seq_from_1 = []
+#     seq_from_2 = []
+#     # TODO keep track of highest nodes?
+
+#     # Do the red line algorithm
+#     while (isom_size < goal_size):
+#         highest_tree_node_network1, highest_retic_network1 = HighestNodesBelow(network1, isom_1_2.keys())
+#         highest_tree_node_network2, highest_retic_network2 = HighestNodesBelow(network2, isom_2_1.keys())
+
+#         # Case1
+#         if highest_tree_node_network1 != None:
+#             moves_network_1, moves_network_2, added_node_network1, added_node_network2 = RL_Case1(network1, network2,
+#                                                                                                   highest_tree_node_network1,
+#                                                                                                   isom_1_2, isom_2_1)
+#         # Case2
+#         elif highest_tree_node_network2 != None:
+#             moves_network_2, moves_network_1, added_node_network2, added_node_network1 = RL_Case1(network2, network1,
+#                                                                                                   highest_tree_node_network2,
+#                                                                                                   isom_2_1, isom_1_2)
+#         # Case3
+#         else:
+#             moves_network_1, moves_network_2, added_node_network1, added_node_network2 = RL_Case3(network1, network2,
+#                                                                                                   highest_retic_network1,
+#                                                                                                   isom_1_2, isom_2_1)
+
+#         # Now perform the moves and update the isomorphism
+#         isom_1_2[added_node_network1] = added_node_network2
+#         isom_2_1[added_node_network2] = added_node_network1
+#         for move in moves_network_1:
+#             seq_from_1.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
+#             network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
+#         for move in moves_network_2:
+#             seq_from_2.append((move[0], move[1], From_Edge(network2, move[0], move[1]), move[2]))
+#             network2 = DoMove(network2, move[0], move[1], move[2], check_validity=False)
+#         isom_size += 1
+#     # TESTING FOR CORRECTNESS WHILE RUNNING
+#     #        if not nx.is_isomorphic(network1.subgraph(isom_1_2.keys()),network2.subgraph(isom_2_1.keys())):
+#     #            print("not unlabeled isom")
+#     #            print(seq_from_1)
+#     #            print(seq_from_2)
+#     #            print(network1.subgraph(isom_1_2.keys()).edges())
+#     #            print(network2.subgraph(isom_2_1.keys()).edges())
+
+#     # TODO Debugging, remove after for speed
+#     #    if not nx.is_isomorphic(network1,network2):
+#     #        print("not unlabeled isom")
+#     #        print(network1.edges())
+#     #        print(network2.edges())
+#     #    else:
+#     #        print("unlabeled isomorphic :)")
+
+#     # Add the leaves to the isomorphism
+#     for node_1 in network1.nodes():
+#         if network1.out_degree(node_1) == 0:
+#             parent_1 = Parent(network1, node_1)
+#             parent_2 = isom_1_2[parent_1]
+#             node_2 = Child(network2, parent_2, exclude=isom_2_1.keys())
+#             isom_1_2[node_1] = node_2
+#             isom_2_1[node_2] = node_1
+
+#     # Permute the leaves
+#     seq_permute = Permute_Leaves_Head(network1, network2, isom_1_2, isom_2_1, label_dict_1, label_dict_2)
+
+#     # invert seq_from_2, rename to node names of network1, and append to seq_from_1
+#     return seq_from_1 + seq_permute + ReplaceNodeNamesInMoveSequence(InvertMoveSequence(seq_from_2), isom_2_1)
+
+
+# def Red_Line_Random(network1, network2, repeats=1):
+#     """
+#     Finds a sequence of head moves from network1 to network2 by randomly building an up-closed isomorphism a number of times, and only keeping the shortest sequence.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :param repeats: an integer, determining how many repeats of Red_Line_Random_Single are performed.
+#     :return: A list of head moves from network1 to network2.
+#     """
+#     best_seq = None
+#     for i in range(repeats):
+#         candidate_seq = Red_Line_Random_Single(network1, network2)
+#         if best_seq == None or len(best_seq) > len(candidate_seq):
+#             best_seq = candidate_seq
+#     return best_seq
+
+
+# def Red_Line_Random_Single(network1, network2):
+#     """
+#     An implementation of Algorithm 11. Finds a sequence of head moves from network1 to network2 by building randomly an up-closed isomorphism.
+
+#     :param network1: a phylogenetic network.
+#     :param network2: a phylogenetic network.
+#     :return: A list of head moves from network1 to network2.
+#     """
+#     # Find the root and labels of the networks
+#     root1 = Root(network1)
+#     root2 = Root(network2)
+#     label_dict_1 = Labels(network1)
+#     label_dict_2 = Labels(network2)
+
+#     # initialize isomorphism
+#     isom_1_2 = dict()
+#     isom_1_2[root1] = root2
+#     isom_2_1 = dict()
+#     isom_2_1[root2] = root1
+#     isom_size = 1
+
+#     # Check if the roots are of the same type
+#     if network1.out_degree(root1) != network2.out_degree(root2):
+#         return False
+
+#     # Keep track of the size of the isomorphism and the size it is at the end of the red line algorithm
+#     goal_size = len(network1) - len(label_dict_1)
+
+#     # init lists of sequence of moves
+#     # list of (moving_edge,moving_endpoint,from_edge,to_edge)
+#     seq_from_1 = []
+#     seq_from_2 = []
+#     # TODO keep track of highest nodes?
+
+#     # Do the red line algorithm
+#     while (isom_size < goal_size):
+#         highest_tree_node_network1, highest_retic_network1 = HighestNodesBelow(network1, isom_1_2.keys(), allnodes=True)
+#         highest_tree_node_network2, highest_retic_network2 = HighestNodesBelow(network2, isom_2_1.keys(), allnodes=True)
+
+#         # Construct a list of all highest nodes in a tuple with the corresponding network (in random order)
+#         # I.e. If u is a highest node of network one, it will appear in the list as (u,1)
+#         highest_nodes_network1 = [(u, 1) for u in highest_tree_node_network1 + highest_retic_network1]
+#         highest_nodes_network2 = [(u, 2) for u in highest_tree_node_network2 + highest_retic_network2]
+#         candidate_highest_nodes = highest_nodes_network1 + highest_nodes_network2
+#         random.shuffle(candidate_highest_nodes)
+
+#         # As some cases do not give an addition to the isom, we continue trying lowest nodes until we find one that does.
+#         for highest_node, network_number in candidate_highest_nodes:
+#             u = highest_node
+#             # Case1
+#             if network_number == 1 and network1.in_degree(u) == 1:
+#                 #                print("Case 1")
+#                 moves_network_1, moves_network_2, added_node_network1, added_node_network2 = RL_Case1(network1,
+#                                                                                                       network2, u,
+#                                                                                                       isom_1_2,
+#                                                                                                       isom_2_1,
+#                                                                                                       randomNodes=True)
+#                 break
+#             # Case2
+#             elif network_number == 2 and network2.in_degree(u) == 1:
+#                 #                print("Case 2")
+#                 moves_network_2, moves_network_1, added_node_network2, added_node_network1 = RL_Case1(network2,
+#                                                                                                       network1, u,
+#                                                                                                       isom_2_1,
+#                                                                                                       isom_1_2,
+#                                                                                                       randomNodes=True)
+#                 break
+#             # Case3
+#             elif network_number == 1 and network1.in_degree(u) == 2:
+#                 #                print("Case 3")
+#                 moves_network_1, moves_network_2, added_node_network1, added_node_network2 = RL_Case3(network1,
+#                                                                                                       network2, u,
+#                                                                                                       isom_1_2,
+#                                                                                                       isom_2_1,
+#                                                                                                       randomNodes=True)
+#                 if added_node_network2:
+#                     break
+#             # Case3'
+#             elif network_number == 2 and network2.in_degree(u) == 2:
+#                 #                print("Case 3'")
+#                 moves_network_2, moves_network_1, added_node_network2, added_node_network1 = RL_Case3(network2,
+#                                                                                                       network1, u,
+#                                                                                                       isom_2_1,
+#                                                                                                       isom_1_2,
+#                                                                                                       randomNodes=True)
+#                 if added_node_network2:
+#                     break
+
+#         # Now perform the moves and update the isomorphism
+#         isom_1_2[added_node_network1] = added_node_network2
+#         isom_2_1[added_node_network2] = added_node_network1
+#         for move in moves_network_1:
+#             seq_from_1.append((move[0], move[1], From_Edge(network1, move[0], move[1]), move[2]))
+#             network1 = DoMove(network1, move[0], move[1], move[2], check_validity=False)
+#         for move in moves_network_2:
+#             seq_from_2.append((move[0], move[1], From_Edge(network2, move[0], move[1]), move[2]))
+#             network2 = DoMove(network2, move[0], move[1], move[2], check_validity=False)
+#         isom_size += 1
+#     # TESTING FOR CORRECTNESS WHILE RUNNING
+#     #        if not nx.is_isomorphic(network1.subgraph(isom_1_2.keys()),network2.subgraph(isom_2_1.keys())):
+#     #            print("not unlabeled isom")
+#     #            print(seq_from_1)
+#     #            print(seq_from_2)
+#     #            print(network1.subgraph(isom_1_2.keys()).edges())
+#     #            print(network2.subgraph(isom_2_1.keys()).edges())
+#     #            print(network1.edges())
+#     #            print(network2.edges())
+
+#     # TODO Debugging, remove after for speed
+#     #    if not nx.is_isomorphic(network1,network2):
+#     #        print("not unlabeled isom")
+#     #        print(network1.edges())
+#     #        print(network2.edges())
+#     #    else:
+#     #        print("unlabeled isomorphic :)")
+
+#     # Add the leaves to the isomorphism
+#     for node_1 in network1.nodes():
+#         if network1.out_degree(node_1) == 0:
+#             parent_1 = Parent(network1, node_1)
+#             parent_2 = isom_1_2[parent_1]
+#             node_2 = Child(network2, parent_2, exclude=isom_2_1.keys())
+#             isom_1_2[node_1] = node_2
+#             isom_2_1[node_2] = node_1
 
-    # Permute the leaves
-    seq_permute = Permute_Leaves_Head(network1, network2, isom_1_2, isom_2_1, label_dict_1, label_dict_2)
+#     # Permute the leaves
+#     seq_permute = Permute_Leaves_Head(network1, network2, isom_1_2, isom_2_1, label_dict_1, label_dict_2)
 
-    # invert seq_from_2, rename to node names of network1, and append to seq_from_1
-    return seq_from_1 + seq_permute + ReplaceNodeNamesInMoveSequence(InvertMoveSequence(seq_from_2), isom_2_1)
+#     # invert seq_from_2, rename to node names of network1, and append to seq_from_1
+#     return seq_from_1 + seq_permute + ReplaceNodeNamesInMoveSequence(InvertMoveSequence(seq_from_2), isom_2_1)
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/invertsequence.py` & `phylox-0.0.2/src/phylox/rearrangement/invertsequence.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,47 +10,47 @@
     :return: a pair of nodes (p,c) where p and c are a parent and child of the moving_endpoint such that they are both not part of the moving_edge.
     """
     other_parent = network.parent(moving_endpoint, exclude=moving_edge)
     other_child = network.child(moving_endpoint, exclude=moving_edge)
     return (other_parent, other_child)
 
 
-def InvertMoveSequence(seq):
-    """
-    Inverts a sequence of moves.
-
-    :param seq: a list of moves, where each moves is in the format (moving_edge,moving_endpoint,from_edge,to_edge).
-    :return: the inverse list of moves.
-    """
-    newSeq = []
-    for move in reversed(seq):
-        moving_edge, moving_endpoint, from_edge, to_edge = move
-        newSeq.append((moving_edge, moving_endpoint, to_edge, from_edge))
-    return newSeq
-
-
-def ReplaceNodeNamesInMoveSequence(seq, isom):
-    """
-    Renames the nodes in a sequence of moves using an isomorphism mapping between two networks.
-
-    :param seq: a list of moves, implicitly using the nodes of a network.
-    :param isom: a dictionary, containing a bijective mapping from nodes of the networks to another set.
-    :return: a list of moves where the nodes are replaced by their image under the isom mapping.
-    """
-    if type(seq) == int:
-        return isom[seq]
-    return list(map(lambda x: ReplaceNodeNamesInMoveSequence(x, isom), seq))
-
-
-def ReplaceNodeNamesByOriginal(network, seq):
-    """
-    Renames the nodes in a sequence of moves by their original names as given in the input. These are stored as a node attribute 'original'.
-
-    :param network: a phylogenetic network.
-    :param seq: a sequence of moves on teh network.
-    :return: a list of moves on the network using the original node names as used in the input.
-    """
-    if type(seq) == int:
-        return network.node[seq]['original']
-    if seq == 'rho':
-        return "rho"
-    return list(map(lambda x: ReplaceNodeNamesByOriginal(network, x), seq))
+# def InvertMoveSequence(seq):
+#     """
+#     Inverts a sequence of moves.
+
+#     :param seq: a list of moves, where each moves is in the format (moving_edge,moving_endpoint,from_edge,to_edge).
+#     :return: the inverse list of moves.
+#     """
+#     newSeq = []
+#     for move in reversed(seq):
+#         moving_edge, moving_endpoint, from_edge, to_edge = move
+#         newSeq.append((moving_edge, moving_endpoint, to_edge, from_edge))
+#     return newSeq
+
+
+# def ReplaceNodeNamesInMoveSequence(seq, isom):
+#     """
+#     Renames the nodes in a sequence of moves using an isomorphism mapping between two networks.
+
+#     :param seq: a list of moves, implicitly using the nodes of a network.
+#     :param isom: a dictionary, containing a bijective mapping from nodes of the networks to another set.
+#     :return: a list of moves where the nodes are replaced by their image under the isom mapping.
+#     """
+#     if type(seq) == int:
+#         return isom[seq]
+#     return list(map(lambda x: ReplaceNodeNamesInMoveSequence(x, isom), seq))
+
+
+# def ReplaceNodeNamesByOriginal(network, seq):
+#     """
+#     Renames the nodes in a sequence of moves by their original names as given in the input. These are stored as a node attribute 'original'.
+
+#     :param network: a phylogenetic network.
+#     :param seq: a sequence of moves on teh network.
+#     :return: a list of moves on the network using the original node names as used in the input.
+#     """
+#     if type(seq) == int:
+#         return network.node[seq]['original']
+#     if seq == 'rho':
+#         return "rho"
+#     return list(map(lambda x: ReplaceNodeNamesByOriginal(network, x), seq))
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/movability.py` & `phylox-0.0.2/src/phylox/rearrangement/movability.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # These functions are implementations of the algorithms of Remie Janssen's PhD thesis
 
-import networkx as nx
+import ast
 import random
-import sys
-from copy import deepcopy
-from collections import deque
 import re
-import ast
+import sys
 import time
+from collections import deque
+from copy import deepcopy
 
-from phylox.rearrangement.movetype import MoveType
-from phylox.exceptions import InvalidMoveException, InvalidMoveDefinitionException
+import networkx as nx
 
+from phylox.exceptions import InvalidMoveDefinitionException, InvalidMoveException
+from phylox.rearrangement.movetype import MoveType
 
 
 def check_valid(network, move):
     """
     Checks whether a move is valid.
 
     :param move: a move of type Move
@@ -44,66 +44,40 @@
         # move.is_type(MoveType.HEAD)
         if nx.has_path(network, move.target[1], move.moving_edge[0]):
             raise InvalidMoveException("reattachment would create a cycle")
         if move.target[0] == move.moving_edge[0]:
             raise InvalidMoveException("reattachment creates parallel edges")
     elif move.is_type(MoveType.VPLU):
         if move.start_node in network.nodes:
-            raise InvalidMoveException(
-                "Start node must not be in the network."
-            )
+            raise InvalidMoveException("Start node must not be in the network.")
         if move.end_node in network.nodes:
-            raise InvalidMoveException(
-                "End node must not be in the network."
-            )
-        if nx.has_path(network, move.end_edge[1], move.start_edge[0]) or move.start_edge == move.end_edge:
+            raise InvalidMoveException("End node must not be in the network.")
+        if (
+            nx.has_path(network, move.end_edge[1], move.start_edge[0])
+            or move.start_edge == move.end_edge
+        ):
             raise InvalidMoveException("end node is reachable from start node")
     elif move.is_type(MoveType.VMIN):
         parent_0 = network.parent(move.removed_edge[0], exclude=[move.removed_edge[1]])
         child_0 = network.child(move.removed_edge[0], exclude=[move.removed_edge[1]])
         parent_1 = network.parent(move.removed_edge[1], exclude=[move.removed_edge[0]])
         child_1 = network.child(move.removed_edge[1], exclude=[move.removed_edge[0]])
-        if parent_0==parent_1 and child_0==child_1:
+        if parent_0 == parent_1 and child_0 == child_1:
             raise InvalidMoveException("removal creates parallel edges")
-        if not (check_movable(network, move.removed_edge, move.removed_edge[0]) and check_movable(network, move.removed_edge, move.removed_edge[1])):
+        if not (
+            check_movable(network, move.removed_edge, move.removed_edge[0])
+            and check_movable(network, move.removed_edge, move.removed_edge[1])
+        ):
             raise InvalidMoveException("removal creates parallel edges")
         if network.out_degree(move.removed_edge[1]) == 0:
             raise InvalidMoveException("removes a leaf")
     else:
-        raise InvalidMoveException("Only rSPR and vertical moves are supported currently")
-
-
-
-# Returns all valid moves in the network
-# List of moves in format (moving_edge,moving_endpoint,to_edge)
-# change move options to move_type
-def all_valid_moves(network, tail_moves=True, head_moves=True):
-    """
-    Finds all valid moves of a certain type in a network.
-
-    :param network: a phylogenetic network.
-    :param tail_moves: boolean value that determines whether tail moves are used (Default: True).
-    :param head_moves: boolean value that determines whether head moves are used (Default: True).
-    :return: A list of all valid tail/head/rSPR moves in the network.
-    """
-    validMoves = []
-    headOrTail = []
-    if tail_moves:
-        headOrTail.append(0)
-    if head_moves:
-        headOrTail.append(1)
-    for moving_edge in network.edges():
-        for to_edge in network.edges():
-            for end in headOrTail:
-                if CheckValid(network, moving_edge, moving_edge[end], to_edge) and moving_edge[
-                    end] not in to_edge:  # Last part is to prevent valid moves that result in isomorphic networks. TODO: To use this for internally labeled networks, remove this condition
-                    validMoves.append((moving_edge, moving_edge[end], to_edge))
-    return validMoves
-
-
+        raise InvalidMoveException(
+            "Only rSPR and vertical moves are supported currently"
+        )
 
 
 # Checks whether an endpoint of an edge is movable.
 def check_movable(network, moving_edge, moving_endpoint):
     """
     Checks whether an endpoint of an edge is movable in a network.
 
@@ -122,12 +96,14 @@
         if network.out_degree(moving_endpoint) in (0, 2):
             # cannot move the head if it is a tree node or leaf
             return False
     else:
         # Moving endpoint is not part of the moving edge
         return False
     # Now check for triangles, by finding the other parent and child of the moving endpoint
-    parent_of_moving_endpoint = network.parent(moving_endpoint, exclude=[moving_edge[0]])
+    parent_of_moving_endpoint = network.parent(
+        moving_endpoint, exclude=[moving_edge[0]]
+    )
     child_of_moving_endpoint = network.child(moving_endpoint, exclude=[moving_edge[1]])
     # if there is an edge from the parent to the child, there is a triangle
     # Otherwise, it is a movable edge
     return not network.has_edge(parent_of_moving_endpoint, child_of_moving_endpoint)
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/move.py` & `phylox-0.0.2/src/phylox/rearrangement/move.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from phylox.exceptions import InvalidMoveDefinitionException, InvalidMoveException
-from phylox.rearrangement.movetype import MoveType
 from copy import deepcopy
-from phylox.rearrangement.movability import check_valid
+
+import numpy as np
+
 from phylox.base import find_unused_node
+from phylox.exceptions import InvalidMoveDefinitionException, InvalidMoveException
 from phylox.rearrangement.invertsequence import from_edge
-import numpy as np
+from phylox.rearrangement.movability import check_valid
+from phylox.rearrangement.movetype import MoveType
+
 
 def apply_move(network, move):
     """
     Apply a move to the network, not in place.
     returns True if successful, and False otherwise.
     """
     check_valid(network, move)
@@ -30,29 +33,44 @@
                 (move.target[0], move.moving_node),
                 (move.moving_node, move.target[1]),
                 move.origin,
             ]
         )
         return new_network
     elif move.move_type in [MoveType.VPLU]:
-        new_network.remove_edges_from([move.start_edge, move.end_edge])        
-        new_network.add_edges_from([(move.start_edge[0], move.start_node), (move.start_node, move.start_edge[1]),(move.end_edge[0], move.end_node), (move.end_node, move.end_edge[1]), (move.start_node,move.end_node)])
+        new_network.remove_edges_from([move.start_edge, move.end_edge])
+        new_network.add_edges_from(
+            [
+                (move.start_edge[0], move.start_node),
+                (move.start_node, move.start_edge[1]),
+                (move.end_edge[0], move.end_node),
+                (move.end_node, move.end_edge[1]),
+                (move.start_node, move.end_node),
+            ]
+        )
         return new_network
     elif move.move_type in [MoveType.VMIN]:
         parent_0 = network.parent(move.removed_edge[0], exclude=[move.removed_edge[1]])
         child_0 = network.child(move.removed_edge[0], exclude=[move.removed_edge[1]])
         parent_1 = network.parent(move.removed_edge[1], exclude=[move.removed_edge[0]])
         child_1 = network.child(move.removed_edge[1], exclude=[move.removed_edge[0]])
-        new_network.remove_edges_from([(parent_0, move.removed_edge[0]), (move.removed_edge[0], child_0),(parent_1, move.removed_edge[1]), (move.removed_edge[1], child_1), move.removed_edge])
+        new_network.remove_edges_from(
+            [
+                (parent_0, move.removed_edge[0]),
+                (move.removed_edge[0], child_0),
+                (parent_1, move.removed_edge[1]),
+                (move.removed_edge[1], child_1),
+                move.removed_edge,
+            ]
+        )
         new_network.add_edges_from([(parent_0, child_0), (parent_1, child_1)])
         return new_network
     elif move.move_type in [MoveType.NONE]:
         return network
-    raise InvalidMove("only tail or head moves are currently valid.")
-
+    raise InvalidMoveException("only tail or head moves are currently valid.")
 
 
 def apply_move_sequence(network, seq_moves):
     for move in seq_moves:
         network = apply_move(network, move)
     return network
 
@@ -103,15 +121,17 @@
         elif self.move_type == MoveType.VPLU:
             try:
                 self.start_edge = kwargs["start_edge"]
                 self.end_edge = kwargs["end_edge"]
                 self.start_node = kwargs.get("start_node", None)
                 self.end_node = kwargs.get("end_node", None)
                 network = kwargs.get("network", None)
-                if (self.start_node is None or self.end_node is None) and network is None:
+                if (
+                    self.start_node is None or self.end_node is None
+                ) and network is None:
                     raise InvalidMoveDefinitionException(
                         "Either a start_node and end_node, or a network must be given."
                     )
                 if self.start_node is None:
                     self.start_node = find_unused_node(network)
                 if self.end_node is None:
                     self.end_node = find_unused_node(network, exclude=[self.start_node])
@@ -130,16 +150,14 @@
             except KeyError:
                 raise InvalidMoveDefinitionException(
                     "Missing removed_edge in definition."
                 )
         else:
             raise InvalidMoveDefinitionException("Invalid move type.")
 
-
-
     def is_type(self, move_type):
         if self.move_type == MoveType.ALL:
             return True
         if (
             self.move_type == MoveType.NONE
             or (
                 move_type == MoveType.RSPR
@@ -155,15 +173,20 @@
 
     @classmethod
     def random_move(
         cls,
         network,
         available_tree_nodes=None,
         available_reticulations=None,
-        move_type_probabilities={MoveType.TAIL: 0.4, MoveType.HEAD: 0.4, MoveType.VPLU: 0.1, MoveType.VMIN: 0.1},
+        move_type_probabilities={
+            MoveType.TAIL: 0.4,
+            MoveType.HEAD: 0.4,
+            MoveType.VPLU: 0.1,
+            MoveType.VMIN: 0.1,
+        },
     ):
         available_tree_nodes = available_tree_nodes or []
         available_reticulations = available_reticulations or []
         edges = list(network.edges())
         num_edges = len(edges)
         move_type_probabilities_keys = list(move_type_probabilities.keys())
         movetype_index = np.random.choice(
@@ -172,19 +195,34 @@
         movetype = move_type_probabilities_keys[movetype_index]
         if movetype in [MoveType.TAIL, MoveType.HEAD]:
             moving_edge = edges[np.random.choice(num_edges)]
             target = edges[np.random.choice(num_edges)]
             moving_endpoint_index = 0 if movetype == MoveType.TAIL else 1
             moving_endpoint = moving_edge[moving_endpoint_index]
             origin = from_edge(network, moving_edge, moving_endpoint=moving_endpoint)
-            return Move(move_type=movetype, origin=origin, moving_edge=moving_edge, target=target)
+            return Move(
+                move_type=movetype,
+                origin=origin,
+                moving_edge=moving_edge,
+                target=target,
+            )
         elif movetype == MoveType.VPLU:
-            available_reticulations = list(available_reticulations) or [find_unused_node(network)]
-            available_tree_nodes = list(available_tree_nodes) or [find_unused_node(network, exclude=available_reticulations)]
+            available_reticulations = list(available_reticulations) or [
+                find_unused_node(network)
+            ]
+            available_tree_nodes = list(available_tree_nodes) or [
+                find_unused_node(network, exclude=available_reticulations)
+            ]
             start_edge = edges[np.random.choice(num_edges)]
             end_edge = edges[np.random.choice(num_edges)]
             start_node = np.random.choice(available_tree_nodes)
             end_node = np.random.choice(available_reticulations)
-            return Move(move_type=movetype, start_edge=start_edge, end_edge=end_edge, start_node=start_node, end_node=end_node)
+            return Move(
+                move_type=movetype,
+                start_edge=start_edge,
+                end_edge=end_edge,
+                start_node=start_node,
+                end_node=end_node,
+            )
         elif movetype == MoveType.VMIN:
             removed_edge = edges[np.random.choice(num_edges)]
             return Move(move_type=movetype, removed_edge=removed_edge)
```

### Comparing `phylox-0.0.1/src/phylox/rearrangement/rearrangementproblem.py` & `phylox-0.0.2/src/phylox/rearrangement/rearrangementproblem.py`

 * *Files identical despite different names*

### Comparing `phylox-0.0.1/src/phylox.egg-info/SOURCES.txt` & `phylox-0.0.2/src/phylox.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/phylox/__init__.py
 src/phylox/base.py
 src/phylox/dinetwork.py
 src/phylox/parser.py
 src/phylox.egg-info/PKG-INFO
 src/phylox.egg-info/SOURCES.txt
 src/phylox.egg-info/dependency_links.txt
+src/phylox.egg-info/requires.txt
 src/phylox.egg-info/top_level.txt
 src/phylox/cherrypicking/CPH.py
 src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py
 src/phylox/cherrypicking/NetworkContainment.py
 src/phylox/cherrypicking/__init__.py
 src/phylox/cherrypicking/base.py
 src/phylox/classes/__init__.py
```

### Comparing `phylox-0.0.1/tests/test_dinetwork.py` & `phylox-0.0.2/tests/test_dinetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 
-from phylox import DiNetwork, LABEL_ATTR
+from phylox import LABEL_ATTR, DiNetwork
+
 
 class TestDiNetwork(unittest.TestCase):
     def test_init(self):
         network = DiNetwork()
         self.assertEqual(list(network.edges), [])
         self.assertEqual(list(network.nodes), [])
 
@@ -15,15 +16,15 @@
             labels=[(1, "a"), (2, "b"), (3, "c")],
         )
         self.assertCountEqual(list(network.nodes), [1, 2, 3])
         self.assertCountEqual(list(network.edges), [(1, 2), (2, 3)])
         self.assertEqual(network.nodes[1][LABEL_ATTR], "a")
         self.assertEqual(network.nodes[2][LABEL_ATTR], "b")
         self.assertEqual(network.nodes[3][LABEL_ATTR], "c")
-        
+
     def test_leaves(self):
         network = DiNetwork(
             edges=[(1, 2), (2, 3)],
             labels=[(1, "a"), (2, "b"), (3, "c")],
         )
         self.assertEqual(network.leaves, {3})
 
@@ -36,27 +37,27 @@
 
     def test_reticulation_number(self):
         network = DiNetwork(
             edges=[(1, 2), (2, 3), (2, 4), (3, 4), (3, 5), (4, 6)],
             labels=[(5, "a"), (6, "b")],
         )
         self.assertEqual(network.reticulation_number, 1)
-    
+
     def test_child(self):
         network = DiNetwork(
             edges=[(1, 2), (2, 3), (2, 4), (3, 4), (3, 5), (4, 6)],
             labels=[(5, "a"), (6, "b")],
         )
         self.assertIn(network.child(2), [3, 4])
         self.assertEqual(network.child(2, exclude=[3]), 4)
         self.assertEqual(network.child(2, exclude=[3, 4]), None)
         self.assertIn(network.child(2, randomNodes=True), [3, 4])
         self.assertEqual(network.child(2, exclude=[3], randomNodes=True), 4)
         self.assertEqual(network.child(2, exclude=[3, 4], randomNodes=True), None)
-    
+
     def test_parent(self):
         network = DiNetwork(
             edges=[(1, 2), (2, 3), (2, 4), (3, 4), (3, 5), (4, 6)],
             labels=[(5, "a"), (6, "b")],
         )
         self.assertIn(network.parent(4), [2, 3])
         self.assertEqual(network.parent(4, exclude=[2]), 3)
@@ -72,19 +73,19 @@
         )
         self.assertFalse(network.is_tree_node(1))
         self.assertTrue(network.is_tree_node(2))
         self.assertTrue(network.is_tree_node(3))
         self.assertFalse(network.is_tree_node(4))
         self.assertFalse(network.is_tree_node(5))
         self.assertFalse(network.is_tree_node(6))
-    
+
     def test_is_reticulation(self):
         network = DiNetwork(
             edges=[(1, 2), (2, 3), (2, 4), (3, 4), (3, 5), (4, 6)],
             labels=[(5, "a"), (6, "b")],
         )
         self.assertFalse(network.is_reticulation(1))
         self.assertFalse(network.is_reticulation(2))
         self.assertFalse(network.is_reticulation(3))
         self.assertTrue(network.is_reticulation(4))
         self.assertFalse(network.is_reticulation(5))
-        self.assertFalse(network.is_reticulation(6))
+        self.assertFalse(network.is_reticulation(6))
```

