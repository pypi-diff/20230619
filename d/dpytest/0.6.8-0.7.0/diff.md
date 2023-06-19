# Comparing `tmp/dpytest-0.6.8.tar.gz` & `tmp/dpytest-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpytest-0.6.8.tar", last modified: Fri Jun 16 13:44:32 2023, max compression
+gzip compressed data, was "dpytest-0.7.0.tar", last modified: Mon Jun 19 15:42:27 2023, max compression
```

## Comparing `dpytest-0.6.8.tar` & `dpytest-0.7.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.928949 dpytest-0.6.8/
--rw-rw-rw-   0        0        0     2276 2023-06-16 13:33:41.000000 dpytest-0.6.8/HISTORY.md
--rw-rw-rw-   0        0        0     1102 2023-06-16 08:31:44.000000 dpytest-0.6.8/LICENSE
--rw-rw-rw-   0        0        0      228 2023-06-16 08:31:44.000000 dpytest-0.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5750 2023-06-16 13:44:32.929950 dpytest-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-06-16 08:31:44.000000 dpytest-0.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.627543 dpytest-0.6.8/discord/
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.635936 dpytest-0.6.8/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.715954 dpytest-0.6.8/discord/ext/test/
--rw-rw-rw-   0        0        0      586 2023-06-16 13:31:24.000000 dpytest-0.6.8/discord/ext/test/__init__.py
--rw-rw-rw-   0        0        0      541 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/_types.py
--rw-rw-rw-   0        0        0    41690 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/backend.py
--rw-rw-rw-   0        0        0     1992 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/callbacks.py
--rw-rw-rw-   0        0        0    20502 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/factories.py
--rw-rw-rw-   0        0        0    14745 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/runner.py
--rw-rw-rw-   0        0        0     3873 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/state.py
--rw-rw-rw-   0        0        0     1870 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/utils.py
--rw-rw-rw-   0        0        0    10242 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/verify.py
--rw-rw-rw-   0        0        0     1355 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/voice.py
--rw-rw-rw-   0        0        0     1605 2023-06-16 08:31:44.000000 dpytest-0.6.8/discord/ext/test/websocket.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.720953 dpytest-0.6.8/docs/
--rw-rw-rw-   0        0        0     2957 2023-06-16 13:31:24.000000 dpytest-0.6.8/docs/conf.py
--rw-rw-rw-   0        0        0      796 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.754952 dpytest-0.6.8/docs/modules/
--rw-rw-rw-   0        0        0       64 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/backend.rst
--rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/callbacks.rst
--rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/factories.rst
--rw-rw-rw-   0        0        0      171 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/index.rst
--rw-rw-rw-   0        0        0       61 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/runner.rst
--rw-rw-rw-   0        0        0       58 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/state.rst
--rw-rw-rw-   0        0        0       58 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/utils.rst
--rw-rw-rw-   0        0        0       61 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/verify.rst
--rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/modules/websocket.rst
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.765949 dpytest-0.6.8/docs/tutorials/
--rw-rw-rw-   0        0        0     1707 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/tutorials/getting_started.rst
--rw-rw-rw-   0        0        0      310 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/tutorials/index.rst
--rw-rw-rw-   0        0        0     5008 2023-06-16 08:31:44.000000 dpytest-0.6.8/docs/tutorials/using_pytest.rst
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.815949 dpytest-0.6.8/dpytest.egg-info/
--rw-rw-rw-   0        0        0     5750 2023-06-16 13:44:32.000000 dpytest-0.6.8/dpytest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-06-16 13:44:32.000000 dpytest-0.6.8/dpytest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 13:44:32.000000 dpytest-0.6.8/dpytest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-06-16 13:44:32.000000 dpytest-0.6.8/dpytest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 13:44:32.000000 dpytest-0.6.8/dpytest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1532 2023-06-16 13:28:27.000000 dpytest-0.6.8/pyproject.toml
--rw-rw-rw-   0        0        0      514 2023-06-16 13:44:32.941952 dpytest-0.6.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.903951 dpytest-0.6.8/tests/
--rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.913949 dpytest-0.6.8/tests/data/
--rw-rw-rw-   0        0        0     3561 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/data/loremimpsum.txt
--rw-rw-rw-   0        0        0    48027 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/data/unit-tests.jpg
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.916973 dpytest-0.6.8/tests/internal/
--rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/internal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:44:32.926954 dpytest-0.6.8/tests/internal/cogs/
--rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/internal/cogs/__init__.py
--rw-rw-rw-   0        0        0      330 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/internal/cogs/echo.py
--rw-rw-rw-   0        0        0      352 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/internal/cogs/greeting.py
--rw-rw-rw-   0        0        0      809 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_activity.py
--rw-rw-rw-   0        0        0      948 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_create_channel.py
--rw-rw-rw-   0        0        0      508 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_dmchannel.py
--rw-rw-rw-   0        0        0      552 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_edit.py
--rw-rw-rw-   0        0        0      442 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_fetch_message.py
--rw-rw-rw-   0        0        0     1800 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_get.py
--rw-rw-rw-   0        0        0      735 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_get_channel_history.py
--rw-rw-rw-   0        0        0      783 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_member.py
--rw-rw-rw-   0        0        0     1386 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_mentions.py
--rw-rw-rw-   0        0        0     1192 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_message.py
--rw-rw-rw-   0        0        0     2333 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_permissions.py
--rw-rw-rw-   0        0        0     1789 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_reactions.py
--rw-rw-rw-   0        0        0     1926 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_role.py
--rw-rw-rw-   0        0        0      509 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_send.py
--rw-rw-rw-   0        0        0     3102 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_utils.py
--rw-rw-rw-   0        0        0     1684 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_verify_embed.py
--rw-rw-rw-   0        0        0     1146 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_verify_file.py
--rw-rw-rw-   0        0        0     1675 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_verify_message.py
--rw-rw-rw-   0        0        0      754 2023-06-16 08:31:44.000000 dpytest-0.6.8/tests/test_voice.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:27.069952 dpytest-0.7.0/
+-rw-rw-rw-   0        0        0     3071 2023-06-19 15:39:03.000000 dpytest-0.7.0/HISTORY.md
+-rw-rw-rw-   0        0        0     1102 2023-06-16 08:31:44.000000 dpytest-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0      228 2023-06-16 08:31:44.000000 dpytest-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6545 2023-06-19 15:42:27.069952 dpytest-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-06-16 08:31:44.000000 dpytest-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:26.774309 dpytest-0.7.0/discord/
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:26.774309 dpytest-0.7.0/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:26.838848 dpytest-0.7.0/discord/ext/test/
+-rw-rw-rw-   0        0        0      586 2023-06-19 15:42:07.000000 dpytest-0.7.0/discord/ext/test/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-06-16 08:31:44.000000 dpytest-0.7.0/discord/ext/test/_types.py
+-rw-rw-rw-   0        0        0    41690 2023-06-16 08:31:44.000000 dpytest-0.7.0/discord/ext/test/backend.py
+-rw-rw-rw-   0        0        0     1992 2023-06-16 08:31:44.000000 dpytest-0.7.0/discord/ext/test/callbacks.py
+-rw-rw-rw-   0        0        0    20552 2023-06-19 12:19:41.000000 dpytest-0.7.0/discord/ext/test/factories.py
+-rw-rw-rw-   0        0        0    16074 2023-06-19 15:39:03.000000 dpytest-0.7.0/discord/ext/test/runner.py
+-rw-rw-rw-   0        0        0     3873 2023-06-16 08:31:44.000000 dpytest-0.7.0/discord/ext/test/state.py
+-rw-rw-rw-   0        0        0     1870 2023-06-16 08:31:44.000000 dpytest-0.7.0/discord/ext/test/utils.py
+-rw-rw-rw-   0        0        0    10191 2023-06-19 12:18:41.000000 dpytest-0.7.0/discord/ext/test/verify.py
+-rw-rw-rw-   0        0        0     1355 2023-06-16 08:31:44.000000 dpytest-0.7.0/discord/ext/test/voice.py
+-rw-rw-rw-   0        0        0     1605 2023-06-16 08:31:44.000000 dpytest-0.7.0/discord/ext/test/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:26.852850 dpytest-0.7.0/docs/
+-rw-rw-rw-   0        0        0     2957 2023-06-19 15:42:07.000000 dpytest-0.7.0/docs/conf.py
+-rw-rw-rw-   0        0        0      796 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:26.877849 dpytest-0.7.0/docs/modules/
+-rw-rw-rw-   0        0        0       64 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/backend.rst
+-rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/callbacks.rst
+-rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/factories.rst
+-rw-rw-rw-   0        0        0      171 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/index.rst
+-rw-rw-rw-   0        0        0       61 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/runner.rst
+-rw-rw-rw-   0        0        0       58 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/state.rst
+-rw-rw-rw-   0        0        0       58 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/utils.rst
+-rw-rw-rw-   0        0        0       61 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/verify.rst
+-rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/modules/websocket.rst
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:26.889850 dpytest-0.7.0/docs/tutorials/
+-rw-rw-rw-   0        0        0     1707 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/tutorials/getting_started.rst
+-rw-rw-rw-   0        0        0      310 2023-06-16 08:31:44.000000 dpytest-0.7.0/docs/tutorials/index.rst
+-rw-rw-rw-   0        0        0     4993 2023-06-19 12:18:41.000000 dpytest-0.7.0/docs/tutorials/using_pytest.rst
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:26.954382 dpytest-0.7.0/dpytest.egg-info/
+-rw-rw-rw-   0        0        0     6545 2023-06-19 15:42:26.000000 dpytest-0.7.0/dpytest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1556 2023-06-19 15:42:26.000000 dpytest-0.7.0/dpytest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:42:26.000000 dpytest-0.7.0/dpytest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-06-19 15:42:26.000000 dpytest-0.7.0/dpytest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 15:42:26.000000 dpytest-0.7.0/dpytest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1532 2023-06-16 13:28:27.000000 dpytest-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0      514 2023-06-19 15:42:27.072953 dpytest-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:27.047953 dpytest-0.7.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-06-19 12:18:41.000000 dpytest-0.7.0/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:27.053953 dpytest-0.7.0/tests/data/
+-rw-rw-rw-   0        0        0     3561 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/data/loremimpsum.txt
+-rw-rw-rw-   0        0        0    48027 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/data/unit-tests.jpg
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:27.060954 dpytest-0.7.0/tests/internal/
+-rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/internal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:42:27.066951 dpytest-0.7.0/tests/internal/cogs/
+-rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/internal/cogs/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-06-19 15:39:03.000000 dpytest-0.7.0/tests/internal/cogs/echo.py
+-rw-rw-rw-   0        0        0      352 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/internal/cogs/greeting.py
+-rw-rw-rw-   0        0        0      809 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_activity.py
+-rw-rw-rw-   0        0        0     4104 2023-06-19 15:39:03.000000 dpytest-0.7.0/tests/test_configure.py
+-rw-rw-rw-   0        0        0      948 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_create_channel.py
+-rw-rw-rw-   0        0        0      520 2023-06-19 15:39:02.000000 dpytest-0.7.0/tests/test_dmchannel.py
+-rw-rw-rw-   0        0        0      555 2023-06-19 15:39:03.000000 dpytest-0.7.0/tests/test_edit.py
+-rw-rw-rw-   0        0        0      442 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_fetch_message.py
+-rw-rw-rw-   0        0        0     1800 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_get.py
+-rw-rw-rw-   0        0        0      735 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_get_channel_history.py
+-rw-rw-rw-   0        0        0      783 2023-06-19 15:39:03.000000 dpytest-0.7.0/tests/test_member_join.py
+-rw-rw-rw-   0        0        0     1413 2023-06-19 15:39:03.000000 dpytest-0.7.0/tests/test_mentions.py
+-rw-rw-rw-   0        0        0     1103 2023-06-19 15:39:03.000000 dpytest-0.7.0/tests/test_message.py
+-rw-rw-rw-   0        0        0     2333 2023-06-19 14:48:53.000000 dpytest-0.7.0/tests/test_permissions.py
+-rw-rw-rw-   0        0        0     1789 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_reactions.py
+-rw-rw-rw-   0        0        0     1926 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_role.py
+-rw-rw-rw-   0        0        0      509 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_send.py
+-rw-rw-rw-   0        0        0     3102 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0     1684 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_verify_embed.py
+-rw-rw-rw-   0        0        0     1146 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_verify_file.py
+-rw-rw-rw-   0        0        0     1675 2023-06-19 12:08:07.000000 dpytest-0.7.0/tests/test_verify_message.py
+-rw-rw-rw-   0        0        0      754 2023-06-16 08:31:44.000000 dpytest-0.7.0/tests/test_voice.py
```

### Comparing `dpytest-0.6.8/HISTORY.md` & `dpytest-0.7.0/HISTORY.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,36 @@
 # History
 
+## 0.7.0
+
+⚠️ Warning ⚠️:
+
+This can be **breaking** :
+
+The `configure` function has changed.
+It nows accepts either an `int` (like in the previous version) OR a `list` of `string` for the parameters `guilds`, `text_channels`, `voice_channels` and `members`.
+But the names of the parameters had to be changed.
+
+`num_guilds`, `num_text_channels`, `num_voice_channels`, `num_members` are DERECATED.
+
+Example:
+
+```python
+    dpytest.configure(bot,
+                      guilds=["CoolGuild", "LameGuild"],
+                      text_channels=["Fruits", "Videogames"],
+                      voice_channels=2,
+                      members=["Joe", "Jack", "William", "Averell"])
+```
+
+Other changes:
+
+- fixes in typing
+- add `content_type` to `dict_from_attachment()`
+
 ## 0.6.8
 
 Test agains discord.py 2.3
 
 ## 0.6.7
 
 Fix bug in channel_history
```

### Comparing `dpytest-0.6.8/LICENSE` & `dpytest-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/PKG-INFO` & `dpytest-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpytest
-Version: 0.6.8
+Version: 0.7.0
 Summary: A package that assists in writing tests for discord.py
 Author-email: Rune Tynan <runetynan@gmail.com>
 Maintainer: CraftSpider, Sergeileduc
 License: The MIT License (MIT)
         
         Copyright (c) 2018-2019 CraftSpider
         
@@ -65,14 +65,41 @@
 
 ## Documentation
 
 Documentation can be found at [dpytest.readthedocs.io](https://dpytest.readthedocs.io/en/latest/), including examples and tutorials
 
 # History
 
+## 0.7.0
+
+⚠️ Warning ⚠️:
+
+This can be **breaking** :
+
+The `configure` function has changed.
+It nows accepts either an `int` (like in the previous version) OR a `list` of `string` for the parameters `guilds`, `text_channels`, `voice_channels` and `members`.
+But the names of the parameters had to be changed.
+
+`num_guilds`, `num_text_channels`, `num_voice_channels`, `num_members` are DERECATED.
+
+Example:
+
+```python
+    dpytest.configure(bot,
+                      guilds=["CoolGuild", "LameGuild"],
+                      text_channels=["Fruits", "Videogames"],
+                      voice_channels=2,
+                      members=["Joe", "Jack", "William", "Averell"])
+```
+
+Other changes:
+
+- fixes in typing
+- add `content_type` to `dict_from_attachment()`
+
 ## 0.6.8
 
 Test agains discord.py 2.3
 
 ## 0.6.7
 
 Fix bug in channel_history
```

### Comparing `dpytest-0.6.8/README.md` & `dpytest-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/discord/ext/test/__init__.py` & `dpytest-0.7.0/discord/ext/test/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __title__ = "dpytest"
 __author__ = "Rune Tynan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2018-2019 CraftSpider"
-__version__ = "0.6.8"
+__version__ = "0.7.0"
 
 from . import backend as backend
 
 from .runner import *
 
 from .utils import embed_eq as embed_eq
 from .utils import activity_eq as activity_eq
```

### Comparing `dpytest-0.6.8/discord/ext/test/_types.py` & `dpytest-0.7.0/discord/ext/test/_types.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/discord/ext/test/backend.py` & `dpytest-0.7.0/discord/ext/test/backend.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/discord/ext/test/callbacks.py` & `dpytest-0.7.0/discord/ext/test/callbacks.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/discord/ext/test/factories.py` & `dpytest-0.7.0/discord/ext/test/factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
         filename: str,
         size: int,
         url: str,
         proxy_url: str,
         id_num: int = -1,
         height: typing.Optional[int] = None,
         width: typing.Optional[int] = None,
-        content_type: typing.Optional[int] = None
+        content_type: typing.Optional[str] = None
 ) -> _types.JsonDict:
     if id_num < 0:
         id_num = make_id()
     return {
         'id': id_num,
         'filename': filename,
         'size': size,
@@ -480,14 +480,15 @@
         'id': attachment.id,
         'filename': attachment.filename,
         'size': attachment.size,
         'url': attachment.url,
         'proxy_url': attachment.proxy_url,
         'height': attachment.height,
         'width': attachment.width,
+        'content_type': attachment.content_type,
     }
 
 
 # TODO: dict_from_emoji and make_emoji_dict
 
 def make_emoji_dict():
     pass
```

### Comparing `dpytest-0.6.8/discord/ext/test/runner.py` & `dpytest-0.7.0/discord/ext/test/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -351,25 +351,28 @@
         Get the current runner configuration
 
     :return: Current runner config
     """
     return _cur_config
 
 
-def configure(client: discord.Client, num_guilds: int = 1, num_text_channels: int = 1,
-              num_voice_channels: int = 1, num_members: int = 1) -> None:
+def configure(client: discord.Client,
+              guilds: typing.Union[int, typing.List[str]] = 1,
+              text_channels: typing.Union[int, typing.List[str]] = 1,
+              voice_channels: typing.Union[int, typing.List[str]] = 1,
+              members: typing.Union[int, typing.List[str]] = 1) -> None:
     """
         Set up the runner configuration. This should be done before any tests are run.
 
     :param client: Client to configure with. Should be the bot/client that is going to be tested.
-    :param num_guilds: Number of guilds to start the configuration with. Default is 1
-    :param num_text_channels: Number of text channels in each guild to start with. Default is 1
-    :param num_voice_channels: Number of voice channels in each guild to start with. Default is 1.
-    :param num_members: Number of members in each guild (other than the client) to start with. Default is 1.
-    """
+    :param guilds: Number or list of names of guilds to start the configuration with. Default is 1
+    :param text_channels: Number or list of names of text channels in each guild to start with. Default is 1
+    :param voice_channels: Number or list of names of voice channels in each guild to start with. Default is 1.
+    :param members: Number or list of names of members in each guild (other than the client) to start with. Default is 1.
+    """   # noqa: E501
 
     global _cur_config
 
     if not isinstance(client, discord.Client):
         raise TypeError("Runner client must be an instance of discord.Client")
     if isinstance(client, discord.AutoShardedClient):
         raise TypeError("Sharded clients not yet supported")
@@ -393,30 +396,57 @@
 
     # Configure global callbacks
     callbacks.set_callback(_message_callback, "send_message")
     callbacks.set_callback(_edit_member_callback, "edit_member")
 
     back.get_state().stop_dispatch()
 
-    guilds = []
-    for num in range(num_guilds):
-        guild = back.make_guild(f"Test Guild {num}")
-        guilds.append(guild)
-
-    channels = []
-    members = []
-    for guild in guilds:
-        for num in range(num_text_channels):
-            channel = back.make_text_channel(f"TextChannel_{num}", guild)
-            channels.append(channel)
-        for num in range(num_voice_channels):
-            channel = back.make_voice_channel(f"VoiceChannel_{num}", guild)
-            channels.append(channel)
-        for num in range(num_members):
-            user = back.make_user(f"TestUser{str(num)}", f"{num + 1:04}")
-            member = back.make_member(user, guild, nick=user.name + f"_{str(num)}_nick")
-            members.append(member)
-        back.make_member(back.get_state().user, guild, nick=client.user.name + "_nick")
+    _guilds = []
+    if isinstance(guilds, int):
+        for num in range(guilds):
+            guild = back.make_guild(f"Test Guild {num}")
+            _guilds.append(guild)
+    if isinstance(guilds, list):
+        for guild_name in guilds:
+            guild = back.make_guild(guild_name)
+            _guilds.append(guild)
+
+    _channels = []
+    _members = []
+    for guild in _guilds:
+        # Text channels
+        if isinstance(text_channels, int):
+            for num in range(text_channels):
+                channel = back.make_text_channel(f"TextChannel_{num}", guild)
+                _channels.append(channel)
+        if isinstance(text_channels, list):
+            for chan in text_channels:
+                channel = back.make_text_channel(chan, guild)
+                _channels.append(channel)
+
+        # Voice channels
+        if isinstance(voice_channels, int):
+            for num in range(voice_channels):
+                channel = back.make_voice_channel(f"VoiceChannel_{num}", guild)
+                _channels.append(channel)
+        if isinstance(voice_channels, list):
+            for chan in voice_channels:
+                channel = back.make_voice_channel(chan, guild)
+                _channels.append(channel)
+
+        # Members
+        if isinstance(members, int):
+            for num in range(members):
+                user = back.make_user(f"TestUser{str(num)}", f"{num + 1:04}")
+                member = back.make_member(user, guild, nick=f"{user.name}_{str(num)}_nick")
+                _members.append(member)
+        if isinstance(members, list):
+            for num, name in enumerate(members):
+                user = back.make_user(name, f"{num + 1:04}")
+                member = back.make_member(user, guild, nick=f"{user.name}_{str(num)}_nick")
+                _members.append(member)
+
+        back.make_member(back.get_state().user, guild, nick=f"{client.user.name}_nick")
 
     back.get_state().start_dispatch()
 
-    _cur_config = RunnerConfig(client, guilds, channels, members)
+    _cur_config = RunnerConfig(client, _guilds, _channels, _members)
```

### Comparing `dpytest-0.6.8/discord/ext/test/state.py` & `dpytest-0.7.0/discord/ext/test/state.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/discord/ext/test/utils.py` & `dpytest-0.7.0/discord/ext/test/utils.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/discord/ext/test/verify.py` & `dpytest-0.7.0/discord/ext/test/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,23 +208,20 @@
         self._used = True
 
         bot_act = get_config().guilds[0].me.activity
 
         if self._activity is not _undefined:
             return activity_eq(self._activity, bot_act)
 
-        if self._name is not _undefined:
-            if self._name != bot_act.name:
-                return False
-        if self._url is not _undefined:
-            if self._url != bot_act.url:
-                return False
-        if self._type is not _undefined:
-            if self._type != bot_act.type:
-                return False
+        if self._name is not _undefined and self._name != bot_act.name:
+            return False
+        if self._url is not _undefined and self._url != bot_act.url:
+            return False
+        if self._type is not _undefined and self._type != bot_act.type:
+            return False
 
         return True
 
     def matches(self, activity) -> 'VerifyActivity':
         """
             Ensure that the bot activity exactly matches the passed activity. Most restrictive possible check.
```

### Comparing `dpytest-0.6.8/discord/ext/test/voice.py` & `dpytest-0.7.0/discord/ext/test/voice.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/discord/ext/test/websocket.py` & `dpytest-0.7.0/discord/ext/test/websocket.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/docs/conf.py` & `dpytest-0.7.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'dpytest'
 copyright = '2020, CraftSpider'
 author = 'CraftSpider'
 
 # The full version, including alpha/beta/rc tags
-release = '0.6.8'
+release = '0.7.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `dpytest-0.6.8/docs/index.rst` & `dpytest-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/docs/tutorials/getting_started.rst` & `dpytest-0.7.0/docs/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/docs/tutorials/using_pytest.rst` & `dpytest-0.7.0/docs/tutorials/using_pytest.rst`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
         await b._async_setup_hook()
         dpytest.configure(b)
         return b
 
 
     @pytest_asyncio.fixture(autouse=True)
     async def cleanup():
-        yield
         await dpytest.empty_queue()
 
 
     def pytest_sessionfinish(session, exitstatus):
         """ Code to execute after all tests. """
 
         # dat files are created when using attachements
```

### Comparing `dpytest-0.6.8/dpytest.egg-info/PKG-INFO` & `dpytest-0.7.0/dpytest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpytest
-Version: 0.6.8
+Version: 0.7.0
 Summary: A package that assists in writing tests for discord.py
 Author-email: Rune Tynan <runetynan@gmail.com>
 Maintainer: CraftSpider, Sergeileduc
 License: The MIT License (MIT)
         
         Copyright (c) 2018-2019 CraftSpider
         
@@ -65,14 +65,41 @@
 
 ## Documentation
 
 Documentation can be found at [dpytest.readthedocs.io](https://dpytest.readthedocs.io/en/latest/), including examples and tutorials
 
 # History
 
+## 0.7.0
+
+⚠️ Warning ⚠️:
+
+This can be **breaking** :
+
+The `configure` function has changed.
+It nows accepts either an `int` (like in the previous version) OR a `list` of `string` for the parameters `guilds`, `text_channels`, `voice_channels` and `members`.
+But the names of the parameters had to be changed.
+
+`num_guilds`, `num_text_channels`, `num_voice_channels`, `num_members` are DERECATED.
+
+Example:
+
+```python
+    dpytest.configure(bot,
+                      guilds=["CoolGuild", "LameGuild"],
+                      text_channels=["Fruits", "Videogames"],
+                      voice_channels=2,
+                      members=["Joe", "Jack", "William", "Averell"])
+```
+
+Other changes:
+
+- fixes in typing
+- add `content_type` to `dict_from_attachment()`
+
 ## 0.6.8
 
 Test agains discord.py 2.3
 
 ## 0.6.7
 
 Fix bug in channel_history
```

### Comparing `dpytest-0.6.8/dpytest.egg-info/SOURCES.txt` & `dpytest-0.7.0/dpytest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,22 @@
 dpytest.egg-info/SOURCES.txt
 dpytest.egg-info/dependency_links.txt
 dpytest.egg-info/requires.txt
 dpytest.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_activity.py
+tests/test_configure.py
 tests/test_create_channel.py
 tests/test_dmchannel.py
 tests/test_edit.py
 tests/test_fetch_message.py
 tests/test_get.py
 tests/test_get_channel_history.py
-tests/test_member.py
+tests/test_member_join.py
 tests/test_mentions.py
 tests/test_message.py
 tests/test_permissions.py
 tests/test_reactions.py
 tests/test_role.py
 tests/test_send.py
 tests/test_utils.py
```

### Comparing `dpytest-0.6.8/pyproject.toml` & `dpytest-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/setup.cfg` & `dpytest-0.7.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.8
+current_version = 0.7.0
 commit = True
 tag = True
 
 [tool:pytest]
 junit_family = xunit1
 testpaths = tests
 markers =
```

### Comparing `dpytest-0.6.8/tests/conftest.py` & `dpytest-0.7.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
     dpytest.configure(b)
     return b
 
 
 @pytest_asyncio.fixture(autouse=True)
 async def cleanup():
-    yield
     await dpytest.empty_queue()
 
 
 def pytest_sessionfinish(session, exitstatus):
     """ Code to execute after all tests. """
 
     # dat files are created when using attachements
```

### Comparing `dpytest-0.6.8/tests/data/loremimpsum.txt` & `dpytest-0.7.0/tests/data/loremimpsum.txt`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/data/unit-tests.jpg` & `dpytest-0.7.0/tests/data/unit-tests.jpg`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_activity.py` & `dpytest-0.7.0/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_create_channel.py` & `dpytest-0.7.0/tests/test_create_channel.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_edit.py` & `dpytest-0.7.0/tests/test_edit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 00000000: 0d0a 696d 706f 7274 2070 7974 6573 740d  ..import pytest.
 00000010: 0a69 6d70 6f72 7420 6469 7363 6f72 642e  .import discord.
-00000020: 6578 742e 7465 7374 2061 7320 7465 7374  ext.test as test
-00000030: 2020 2320 6e6f 7161 3a20 4634 3031 0d0a    # noqa: F401..
-00000040: 0d0a 0d0a 4070 7974 6573 742e 6d61 726b  ....@pytest.mark
-00000050: 2e61 7379 6e63 696f 0d0a 6173 796e 6320  .asyncio..async 
-00000060: 6465 6620 7465 7374 5f65 6469 7428 626f  def test_edit(bo
-00000070: 7429 3a0d 0a20 2020 2067 7569 6c64 203d  t):..    guild =
-00000080: 2062 6f74 2e67 7569 6c64 735b 305d 0d0a   bot.guilds[0]..
-00000090: 2020 2020 6368 616e 6e65 6c20 3d20 6775      channel = gu
-000000a0: 696c 642e 6368 616e 6e65 6c73 5b30 5d0d  ild.channels[0].
-000000b0: 0a0d 0a20 2020 206d 6573 203d 2061 7761  ...    mes = awa
-000000c0: 6974 2063 6861 6e6e 656c 2e73 656e 6428  it channel.send(
-000000d0: 2254 6573 7420 4d65 7373 6167 6522 290d  "Test Message").
-000000e0: 0a20 2020 2070 6572 7369 7374 6564 5f6d  .    persisted_m
-000000f0: 6573 3120 3d20 6177 6169 7420 6368 616e  es1 = await chan
-00000100: 6e65 6c2e 6665 7463 685f 6d65 7373 6167  nel.fetch_messag
-00000110: 6528 6d65 732e 6964 290d 0a20 2020 2065  e(mes.id)..    e
-00000120: 6469 7465 645f 6d65 7320 3d20 6177 6169  dited_mes = awai
-00000130: 7420 6d65 732e 6564 6974 2863 6f6e 7465  t mes.edit(conte
-00000140: 6e74 3d22 4e65 7720 4d65 7373 6167 6522  nt="New Message"
-00000150: 290d 0a20 2020 2070 6572 7369 7374 6564  )..    persisted
-00000160: 5f6d 6573 3220 3d20 6177 6169 7420 6368  _mes2 = await ch
-00000170: 616e 6e65 6c2e 6665 7463 685f 6d65 7373  annel.fetch_mess
-00000180: 6167 6528 6d65 732e 6964 290d 0a0d 0a20  age(mes.id).... 
-00000190: 2020 2061 7373 6572 7420 6564 6974 6564     assert edited
-000001a0: 5f6d 6573 2e63 6f6e 7465 6e74 203d 3d20  _mes.content == 
-000001b0: 224e 6577 204d 6573 7361 6765 220d 0a20  "New Message".. 
-000001c0: 2020 2061 7373 6572 7420 7065 7273 6973     assert persis
-000001d0: 7465 645f 6d65 7331 2e63 6f6e 7465 6e74  ted_mes1.content
-000001e0: 203d 3d20 2254 6573 7420 4d65 7373 6167   == "Test Messag
-000001f0: 6522 0d0a 2020 2020 6173 7365 7274 2070  e"..    assert p
-00000200: 6572 7369 7374 6564 5f6d 6573 322e 636f  ersisted_mes2.co
-00000210: 6e74 656e 7420 3d3d 2022 4e65 7720 4d65  ntent == "New Me
-00000220: 7373 6167 6522 0d0a                      ssage"..
+00000020: 6578 742e 7465 7374 2061 7320 6470 7974  ext.test as dpyt
+00000030: 6573 7420 2023 206e 6f71 613a 2046 3430  est  # noqa: F40
+00000040: 310d 0a0d 0a0d 0a40 7079 7465 7374 2e6d  1......@pytest.m
+00000050: 6172 6b2e 6173 796e 6369 6f0d 0a61 7379  ark.asyncio..asy
+00000060: 6e63 2064 6566 2074 6573 745f 6564 6974  nc def test_edit
+00000070: 2862 6f74 293a 0d0a 2020 2020 6775 696c  (bot):..    guil
+00000080: 6420 3d20 626f 742e 6775 696c 6473 5b30  d = bot.guilds[0
+00000090: 5d0d 0a20 2020 2063 6861 6e6e 656c 203d  ]..    channel =
+000000a0: 2067 7569 6c64 2e63 6861 6e6e 656c 735b   guild.channels[
+000000b0: 305d 0d0a 0d0a 2020 2020 6d65 7320 3d20  0]....    mes = 
+000000c0: 6177 6169 7420 6368 616e 6e65 6c2e 7365  await channel.se
+000000d0: 6e64 2822 5465 7374 204d 6573 7361 6765  nd("Test Message
+000000e0: 2229 0d0a 2020 2020 7065 7273 6973 7465  ")..    persiste
+000000f0: 645f 6d65 7331 203d 2061 7761 6974 2063  d_mes1 = await c
+00000100: 6861 6e6e 656c 2e66 6574 6368 5f6d 6573  hannel.fetch_mes
+00000110: 7361 6765 286d 6573 2e69 6429 0d0a 2020  sage(mes.id)..  
+00000120: 2020 6564 6974 6564 5f6d 6573 203d 2061    edited_mes = a
+00000130: 7761 6974 206d 6573 2e65 6469 7428 636f  wait mes.edit(co
+00000140: 6e74 656e 743d 224e 6577 204d 6573 7361  ntent="New Messa
+00000150: 6765 2229 0d0a 2020 2020 7065 7273 6973  ge")..    persis
+00000160: 7465 645f 6d65 7332 203d 2061 7761 6974  ted_mes2 = await
+00000170: 2063 6861 6e6e 656c 2e66 6574 6368 5f6d   channel.fetch_m
+00000180: 6573 7361 6765 286d 6573 2e69 6429 0d0a  essage(mes.id)..
+00000190: 0d0a 2020 2020 6173 7365 7274 2065 6469  ..    assert edi
+000001a0: 7465 645f 6d65 732e 636f 6e74 656e 7420  ted_mes.content 
+000001b0: 3d3d 2022 4e65 7720 4d65 7373 6167 6522  == "New Message"
+000001c0: 0d0a 2020 2020 6173 7365 7274 2070 6572  ..    assert per
+000001d0: 7369 7374 6564 5f6d 6573 312e 636f 6e74  sisted_mes1.cont
+000001e0: 656e 7420 3d3d 2022 5465 7374 204d 6573  ent == "Test Mes
+000001f0: 7361 6765 220d 0a20 2020 2061 7373 6572  sage"..    asser
+00000200: 7420 7065 7273 6973 7465 645f 6d65 7332  t persisted_mes2
+00000210: 2e63 6f6e 7465 6e74 203d 3d20 224e 6577  .content == "New
+00000220: 204d 6573 7361 6765 220d 0a               Message"..
```

### Comparing `dpytest-0.6.8/tests/test_get.py` & `dpytest-0.7.0/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_get_channel_history.py` & `dpytest-0.7.0/tests/test_get_channel_history.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_member.py` & `dpytest-0.7.0/tests/test_member_join.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_mentions.py` & `dpytest-0.7.0/tests/test_mentions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 
 import pytest
-import discord.ext.test as test
+import discord.ext.test as dpytest
 
 
 @pytest.mark.asyncio
 async def test_user_mention(bot):
     guild = bot.guilds[0]
-    mes = await test.message(f"<@{guild.me.id}>")
+    mes = await dpytest.message(f"<@{guild.me.id}>")
 
     assert len(mes.mentions) == 1
     assert mes.mentions[0] == guild.me
 
-    mes = await test.message("Not a mention in sight")
+    mes = await dpytest.message("Not a mention in sight")
 
     assert len(mes.mentions) == 0
 
 
 @pytest.mark.asyncio
 async def test_role_mention(bot):
     guild = bot.guilds[0]
     role = await guild.create_role(name="Test Role")
-    mes = await test.message(f"<@&{role.id}>")
+    mes = await dpytest.message(f"<@&{role.id}>")
 
     assert len(mes.role_mentions) == 1
     assert mes.role_mentions[0] == role
 
-    mes = await test.message("Not a mention in sight")
+    mes = await dpytest.message("Not a mention in sight")
 
     assert len(mes.role_mentions) == 0
 
 
 @pytest.mark.asyncio
 async def test_channel_mention(bot):
     guild = bot.guilds[0]
     channel = guild.channels[0]
-    mes = await test.message(f"<#{channel.id}>")
+    mes = await dpytest.message(f"<#{channel.id}>")
 
     assert len(mes.channel_mentions) == 1
     assert mes.channel_mentions[0] == channel
 
-    mes = await test.message("Not a mention in sight")
+    mes = await dpytest.message("Not a mention in sight")
 
     assert len(mes.channel_mentions) == 0
 
 
 @pytest.mark.asyncio
 async def test_bot_mention(bot):
-    mes = await test.message(f"<@{bot.user.id}>")
+    mes = await dpytest.message(f"<@{bot.user.id}>")
 
     assert len(mes.mentions) == 1
     assert mes.mentions[0] == bot.user
 
-    mes = await test.message("Not a mention in sight")
+    mes = await dpytest.message("Not a mention in sight")
 
     assert len(mes.mentions) == 0
```

### Comparing `dpytest-0.6.8/tests/test_message.py` & `dpytest-0.7.0/tests/test_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import discord
 import pytest
 import discord.ext.test as dpytest
 
 
 @pytest.mark.asyncio
-async def test_member_join(bot):
-    """Dont use this in your code, it's just dummy test.
-    Use verify_message() instead of 'get_message' and 'message.content'
+async def test_messasge(bot):
+    """Test make_message_dict from factory.
     """
     guild = bot.guilds[0]
     author: discord.Member = guild.members[0]
     channel = guild.channels[0]
     attach: discord.Attachment = discord.Attachment(
         state=dpytest.back.get_state(),
         data=dpytest.back.facts.make_attachment_dict(
```

### Comparing `dpytest-0.6.8/tests/test_permissions.py` & `dpytest-0.7.0/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_reactions.py` & `dpytest-0.7.0/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_role.py` & `dpytest-0.7.0/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_utils.py` & `dpytest-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_verify_embed.py` & `dpytest-0.7.0/tests/test_verify_embed.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_verify_file.py` & `dpytest-0.7.0/tests/test_verify_file.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_verify_message.py` & `dpytest-0.7.0/tests/test_verify_message.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.8/tests/test_voice.py` & `dpytest-0.7.0/tests/test_voice.py`

 * *Files identical despite different names*

