# Comparing `tmp/scythe-cli-0.8.1.tar.gz` & `tmp/scythe_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scythe-cli-0.8.1.tar", max compression
+gzip compressed data, was "scythe_cli-1.0.0.tar", max compression
```

## Comparing `scythe-cli-0.8.1.tar` & `scythe_cli-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,23 @@
--rw-r--r--   0        0        0     2171 2021-09-21 02:40:49.661848 scythe-cli-0.8.1/README.md
--rw-r--r--   0        0        0      639 2021-10-01 18:02:25.547109 scythe-cli-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      207 2021-10-01 18:00:36.697753 scythe-cli-0.8.1/src/scythe/__init__.py
--rw-r--r--   0        0        0     1953 2021-10-01 18:00:40.957729 scythe-cli-0.8.1/src/scythe/cache.py
--rw-r--r--   0        0        0     3607 2021-10-01 18:00:40.957729 scythe-cli-0.8.1/src/scythe/cli/__init__.py
--rw-r--r--   0        0        0     2552 2021-10-01 18:00:36.697753 scythe-cli-0.8.1/src/scythe/cli/atomic.py
--rw-r--r--   0        0        0      684 2021-10-01 18:00:36.697753 scythe-cli-0.8.1/src/scythe/cli/projects.py
--rw-r--r--   0        0        0     2659 2021-10-01 18:00:40.957729 scythe-cli-0.8.1/src/scythe/cli/running.py
--rw-r--r--   0        0        0     2470 2021-10-01 18:00:36.697753 scythe-cli-0.8.1/src/scythe/cli/stats.py
--rw-r--r--   0        0        0     3948 2021-10-01 18:01:19.697508 scythe-cli-0.8.1/src/scythe/cli/timer.py
--rw-r--r--   0        0        0       39 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/clock/__init__.py
--rw-r--r--   0        0        0     1462 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/clock/clock.py
--rw-r--r--   0        0        0     4674 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/clock/numbers.py
--rw-r--r--   0        0        0     1174 2021-10-01 18:00:40.957729 scythe-cli-0.8.1/src/scythe/decos.py
--rw-r--r--   0        0        0     1919 2021-10-01 18:00:40.957729 scythe-cli-0.8.1/src/scythe/harvest_api.py
--rw-r--r--   0        0        0     1123 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/helpers.py
--rw-r--r--   0        0        0      863 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/sync.py
--rw-r--r--   0        0        0       55 2021-10-01 18:01:38.380731 scythe-cli-0.8.1/src/scythe/ui/__init__.py
--rw-r--r--   0        0        0      771 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/ui/_helpers.py
--rw-r--r--   0        0        0     1283 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/ui/_init.py
--rw-r--r--   0        0        0     1259 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/ui/_menu.py
--rw-r--r--   0        0        0      468 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/ui/data_types.py
--rw-r--r--   0        0        0     1118 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/ui/main.py
--rw-r--r--   0        0        0     2096 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/ui/running.py
--rw-r--r--   0        0        0     1395 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/ui/ui.py
--rw-r--r--   0        0        0     2627 2021-10-01 18:00:36.701086 scythe-cli-0.8.1/src/scythe/utils.py
--rw-r--r--   0        0        0     3159 2021-10-01 18:02:39.855880 scythe-cli-0.8.1/setup.py
--rw-r--r--   0        0        0     2737 2021-10-01 18:02:39.856121 scythe-cli-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-04-01 04:53:11.923617 scythe_cli-1.0.0/README.md
+-rw-r--r--   0        0        0      906 2023-06-19 01:47:29.176073 scythe_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-04-01 04:53:11.926950 scythe_cli-1.0.0/scythe_cli/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/application/__init__.py
+-rw-r--r--   0        0        0     2708 2023-06-17 18:30:54.415252 scythe_cli-1.0.0/scythe_cli/application/application.py
+-rw-r--r--   0        0        0     3761 2023-06-17 05:39:35.404656 scythe_cli-1.0.0/scythe_cli/application/quickstart.py
+-rw-r--r--   0        0        0     1820 2023-06-17 05:39:33.414672 scythe_cli-1.0.0/scythe_cli/application/timers.py
+-rw-r--r--   0        0        0       54 2023-06-17 04:43:26.019412 scythe_cli-1.0.0/scythe_cli/console.py
+-rw-r--r--   0        0        0      556 2023-06-17 03:59:43.092914 scythe_cli-1.0.0/scythe_cli/constants.py
+-rw-r--r--   0        0        0     9330 2023-06-19 01:35:56.348376 scythe_cli-1.0.0/scythe_cli/harvest.py
+-rw-r--r--   0        0        0     3667 2023-06-19 01:42:32.798498 scythe_cli-1.0.0/scythe_cli/ui/apps.py
+-rw-r--r--   0        0        0      246 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/ui/styles/app.css
+-rw-r--r--   0        0        0      639 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/ui/styles/timer-container.css
+-rw-r--r--   0        0        0      893 2023-06-19 01:33:10.186369 scythe_cli-1.0.0/scythe_cli/ui/styles/timer-modal.css
+-rw-r--r--   0        0        0      888 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/ui/styles/timer.css
+-rw-r--r--   0        0        0      147 2023-06-17 18:46:28.388935 scythe_cli-1.0.0/scythe_cli/ui/widgets/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-22 00:56:50.311829 scythe_cli-1.0.0/scythe_cli/ui/widgets/actions.py
+-rw-r--r--   0        0        0     4775 2023-06-19 01:24:39.446966 scythe_cli-1.0.0/scythe_cli/ui/widgets/timer.py
+-rw-r--r--   0        0        0     4513 2023-06-19 01:42:25.861888 scythe_cli-1.0.0/scythe_cli/ui/widgets/timer_container.py
+-rw-r--r--   0        0        0     5877 2023-06-19 01:43:45.151241 scythe_cli-1.0.0/scythe_cli/ui/widgets/timer_modal.py
+-rw-r--r--   0        0        0     2146 2023-06-18 17:17:49.220101 scythe_cli-1.0.0/scythe_cli/utils.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 scythe_cli-1.0.0/setup.py
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 scythe_cli-1.0.0/PKG-INFO
```

