# Comparing `tmp/dvc-3.0.0a2.tar.gz` & `tmp/dvc-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-3.0.0a2.tar", last modified: Wed Jun  7 06:07:19 2023, max compression
+gzip compressed data, was "dvc-3.1.0.tar", last modified: Sun Jun 18 22:22:43 2023, max compression
```

## Comparing `dvc-3.0.0a2.tar` & `dvc-3.1.0.tar`

### file list

```diff
@@ -1,684 +1,688 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.994876 dvc-3.0.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.858869 dvc-3.0.0a2/.dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.dvc/config
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.dvcignore
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.858869 dvc-3.0.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.858869 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/epic_story.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.858869 dvc-3.0.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/packages.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/plugin_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-07 06:07:00.000000 dvc-3.0.0a2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-07 06:07:00.000000 dvc-3.0.0a2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-07 06:07:00.000000 dvc-3.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-06-07 06:07:19.994876 dvc-3.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-06-07 06:07:00.000000 dvc-3.0.0a2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.862869 dvc-3.0.0a2/dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc/_dvc_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.866870 dvc-3.0.0a2/dvc/api/
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    11606 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2089 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cachemgr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.866870 dvc-3.0.0a2/dvc/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     7647 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.874870 dvc-3.0.0a2/dvc/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3963 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.878870 dvc-3.0.0a2/dvc/commands/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/exec_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3481 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/install.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.878870 dvc-3.0.0a2/dvc/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/ls/ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/params.py
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.878870 dvc-3.0.0a2/dvc/commands/queue/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/kill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/start.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/stop.py
--rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/repro.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/compare.py
--rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    10948 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dagascii.py
--rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/data_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.882870 dvc-3.0.0a2/dvc/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dependency/param.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dependency/repo.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/env.py
--rw-r--r--   0 runner    (1001) docker     (122)    10109 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.882870 dvc-3.0.0a2/dvc/fs/
--rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    13922 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/git.py
--rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.882870 dvc-3.0.0a2/dvc/machine/
--rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.882870 dvc-3.0.0a2/dvc/machine/backend/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/machine/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/machine/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/machine/backend/terraform.py
--rw-r--r--   0 runner    (1001) docker     (122)    43972 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.886870 dvc-3.0.0a2/dvc/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)    13884 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/parsing/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/parsing/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.886870 dvc-3.0.0a2/dvc/render/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.886870 dvc-3.0.0a2/dvc/render/converter/
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/converter/image.py
--rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/converter/vega.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/match.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.898871 dvc-3.0.0a2/dvc/repo/
--rw-r--r--   0 runner    (1001) docker     (122)    18486 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7135 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     4457 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.902871 dvc-3.0.0a2/dvc/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.902871 dvc-3.0.0a2/dvc/repo/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25405 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/executor/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7923 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/executor/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/executor/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/push.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.906871 dvc-3.0.0a2/dvc/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/refs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     6331 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/stash.py
--rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/get.py
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    21484 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/index.py
--rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/ls_url.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.906871 dvc-3.0.0a2/dvc/repo/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/metrics/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/metrics/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     8225 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/open_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.906871 dvc-3.0.0a2/dvc/repo/params/
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/params/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/params/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.906871 dvc-3.0.0a2/dvc/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/plots/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     7492 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    14157 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/worktree.py
--rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.910872 dvc-3.0.0a2/dvc/stage/
--rw-r--r--   0 runner    (1001) docker     (122)    24712 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9042 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     7439 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/params.py
--rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6907 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)     8571 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.914872 dvc-3.0.0a2/dvc/testing/
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4088 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/api_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.914872 dvc-3.0.0a2/dvc/testing/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.914872 dvc-3.0.0a2/dvc/testing/benchmarks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.914872 dvc-3.0.0a2/dvc/testing/benchmarks/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.918872 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_exp_show.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_help.py
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_push.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.918872 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/test_modify_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.918872 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/use_cases/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/path_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/remote_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/tmp_dir.py
--rw-r--r--   0 runner    (1001) docker     (122)    13091 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/workspace_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.922872 dvc-3.0.0a2/dvc/ui/
--rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ui/_rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ui/pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ui/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.926872 dvc-3.0.0a2/dvc/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-07 06:07:03.000000 dvc-3.0.0a2/dvc/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/pkg.py
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.926872 dvc-3.0.0a2/dvc/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_py.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.866870 dvc-3.0.0a2/dvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17038 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-06-07 06:07:00.000000 dvc-3.0.0a2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.926872 dvc-3.0.0a2/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/build.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      231 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/build_package.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.930873 dvc-3.0.0a2/scripts/fpm/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/after-install.sh
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/after-remove.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/notarize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.930873 dvc-3.0.0a2/scripts/innosetup/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/addSymLinkPermissions.ps1
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/addsymlink.iss
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/build.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/dvc.ico.dvc
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/dvc_left.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/dvc_up.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/modpath.iss
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/setup.iss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.934873 dvc-3.0.0a2/scripts/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/build.py
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.934873 dvc-3.0.0a2/scripts/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-asyncssh.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.system.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc_task.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-fsspec.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-pydrive2.py
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/sign.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 06:07:19.994876 dvc-3.0.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.938873 dvc-3.0.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/dir_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.950873 dvc-3.0.0a2/tests/func/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.950873 dvc-3.0.0a2/tests/func/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.950873 dvc-3.0.0a2/tests/func/artifacts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/artifacts/test_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.950873 dvc-3.0.0a2/tests/func/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.954874 dvc-3.0.0a2/tests/func/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/data/db/test_index.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.954874 dvc-3.0.0a2/tests/func/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/executor/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    26286 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)    13387 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4928 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_save.py
--rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_set_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_stash_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/machine/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/machine/test_machine_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/machine/test_machine_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7730 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/metrics/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/metrics/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/params/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8161 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/params/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/params/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7479 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11227 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/test_foreach.py
--rw-r--r--   0 runner    (1001) docker     (122)     5484 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/test_interpolated_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/test_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.962874 dvc-3.0.0a2/tests/func/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/plots/test_modify.py
--rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/plots/test_show.py
--rw-r--r--   0 runner    (1001) docker     (122)    31717 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    24438 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     8738 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    16609 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_data_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    18824 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    11755 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     7554 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_external_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)    14728 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)    11109 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    20867 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)     7625 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     5558 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     5046 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    17911 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_merge_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_move.py
--rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_odb.py
--rw-r--r--   0 runner    (1001) docker     (122)    15547 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)    10062 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (122)    33140 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_root.py
--rw-r--r--   0 runner    (1001) docker     (122)    20564 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_run_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     9415 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_stage_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_used_objs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_virtual_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.962874 dvc-3.0.0a2/tests/func/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/utils/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/utils/test_strict_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.962874 dvc-3.0.0a2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.962874 dvc-3.0.0a2/tests/integration/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/plots/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    13779 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/plots/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/plots/test_repo_plots_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/test_studio_live_experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.966874 dvc-3.0.0a2/tests/remotes/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.966874 dvc-3.0.0a2/tests/remotes/git-init/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/git_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/user.key
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes_env.sample
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.970874 dvc-3.0.0a2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.970874 dvc-3.0.0a2/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/cli/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.978875 dvc-3.0.0a2/tests/unit/command/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.978875 dvc-3.0.0a2/tests/unit/command/ls/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/ls/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/ls/test_ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_compat_flag.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)    11210 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    11627 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4010 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.978875 dvc-3.0.0a2/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.982875 dvc-3.0.0a2/tests/unit/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/data/db/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.982875 dvc-3.0.0a2/tests/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/dependency/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/dependency/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.982875 dvc-3.0.0a2/tests/unit/fs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7345 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    19095 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_dvc_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.982875 dvc-3.0.0a2/tests/unit/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.986875 dvc-3.0.0a2/tests/unit/output/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/test_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/test_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/test_output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.986875 dvc-3.0.0a2/tests/unit/remote/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/test_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/test_webdav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/test_webhdfs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.986875 dvc-3.0.0a2/tests/unit/render/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/test_image_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/test_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/test_vega_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.986875 dvc-3.0.0a2/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/queue/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/queue/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/test_executor_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/test_open_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/test_reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/test_scm_context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/scm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/scm/test_scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/stage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6074 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_loader_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_serialize_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_serialize_pipeline_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     3705 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_hashinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     8869 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_tabular_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/ui/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/ui/test_console.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/ui/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/ui/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.994876 dvc-3.0.0a2/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.994876 dvc-3.0.0a2/tests/unit/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/serialize/test_python.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/serialize/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/serialize/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.994876 dvc-3.0.0a2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.142194 dvc-3.1.0/.dvc/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-18 22:22:24.000000 dvc-3.1.0/.dvc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-06-18 22:22:24.000000 dvc-3.1.0/.dvc/config
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-18 22:22:24.000000 dvc-3.1.0/.dvcignore
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-18 22:22:24.000000 dvc-3.1.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-18 22:22:24.000000 dvc-3.1.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-18 22:22:24.000000 dvc-3.1.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-18 22:22:24.000000 dvc-3.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.142194 dvc-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.142194 dvc-3.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/ISSUE_TEMPLATE/epic_story.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.142194 dvc-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/packages.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/plugin_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-18 22:22:24.000000 dvc-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-18 22:22:24.000000 dvc-3.1.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-18 22:22:24.000000 dvc-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-18 22:22:24.000000 dvc-3.1.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-18 22:22:24.000000 dvc-3.1.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-18 22:22:24.000000 dvc-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-18 22:22:24.000000 dvc-3.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-18 22:22:24.000000 dvc-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-18 22:22:43.214195 dvc-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-06-18 22:22:24.000000 dvc-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.146194 dvc-3.1.0/dvc/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-18 22:22:29.000000 dvc-3.1.0/dvc/_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-18 22:22:42.000000 dvc-3.1.0/dvc/_dvc_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.150194 dvc-3.1.0/dvc/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9904 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11924 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cachemgr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.150194 dvc-3.1.0/dvc/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     7614 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.154194 dvc-3.1.0/dvc/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.154194 dvc-3.1.0/dvc/commands/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/exec_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3481 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3672 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/install.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/ls/ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/commands/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/kill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/start.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/stop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11039 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dagascii.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11333 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/data_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5148 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dependency/param.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dependency/repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9622 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13922 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4981 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/machine/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/machine/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/machine/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/machine/backend/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45816 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)    13884 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/parsing/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/parsing/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/render/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/render/converter/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/converter/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/converter/vega.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/match.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.166194 dvc-3.1.0/dvc/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)    18691 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7017 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4248 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1934 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.166194 dvc-3.1.0/dvc/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.166194 dvc-3.1.0/dvc/repo/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25373 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/executor/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/executor/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/executor/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/push.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/refs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/stash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23105 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/ls_url.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/repo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/metrics/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/metrics/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8230 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/open_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/repo/params/
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/params/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/params/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/plots/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13769 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/worktree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9221 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7462 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7116 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4128 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/api_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_exp_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/path_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/remote_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/tmp_dir.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12070 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/workspace_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/dvc/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ui/_rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ui/pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ui/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/dvc/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/dvc/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_py.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.150194 dvc-3.1.0/dvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17145 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8683 2023-06-18 22:22:24.000000 dvc-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/build-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/build.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      226 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/build_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/scripts/fpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/after-install.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/after-remove.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/notarize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.182194 dvc-3.1.0/scripts/innosetup/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/addSymLinkPermissions.ps1
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/addsymlink.iss
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/dvc.ico.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/dvc_left.bmp.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/dvc_up.bmp.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/modpath.iss
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/setup.iss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.182194 dvc-3.1.0/scripts/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.182194 dvc-3.1.0/scripts/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-asyncssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.system.py
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-pydrive2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/sign.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-18 22:22:43.214195 dvc-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.186195 dvc-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/dir_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8061 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/artifacts/test_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3425 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/data/db/test_index.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/executor/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26286 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13387 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4928 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_set_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_stash_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/machine/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/machine/test_machine_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/machine/test_machine_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7730 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/metrics/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/metrics/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/params/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8161 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/params/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/params/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7479 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11227 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/test_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5484 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/test_interpolated_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/plots/test_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/plots/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/func/repro/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/repro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33140 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/repro/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/repro/test_repro_allow_missing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/repro/test_repro_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30138 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23047 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9505 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16589 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_data_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19044 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12234 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7976 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_external_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10535 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21031 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17911 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_merge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_odb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20611 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_run_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_stage_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_used_objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_virtual_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/func/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/utils/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/utils/test_strict_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/integration/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/plots/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13823 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/plots/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/plots/test_repo_plots_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/test_studio_live_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/remotes/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/remotes/git-init/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/git_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/user.key
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes_env.sample
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.202195 dvc-3.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.202195 dvc-3.1.0/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/cli/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/command/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/ls/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/ls/test_ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_compat_flag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11210 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11627 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/data/db/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/dependency/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/dependency/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7345 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19226 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_dvc_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/output/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/test_output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/test_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/test_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/test_webhdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/render/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/test_image_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/test_vega_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/queue/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/queue/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/test_executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/test_open_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/test_reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/test_scm_context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/scm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/scm/test_scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/unit/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6074 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_loader_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_serialize_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_serialize_pipeline_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_hashinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8740 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4168 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_tabular_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/unit/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/ui/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/ui/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/ui/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/unit/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/serialize/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/serialize/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/serialize/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/utils/plots.py
```

### Comparing `dvc-3.0.0a2/.git-blame-ignore-revs` & `dvc-3.1.0/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/.github/ISSUE_TEMPLATE/bug_report.md` & `dvc-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/.github/ISSUE_TEMPLATE/epic_story.md` & `dvc-3.1.0/.github/ISSUE_TEMPLATE/epic_story.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/.github/workflows/codeql.yml` & `dvc-3.1.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/.github/workflows/packages.yaml` & `dvc-3.1.0/.github/workflows/packages.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/.github/workflows/plugin_tests.yaml` & `dvc-3.1.0/.github/workflows/plugin_tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/.github/workflows/tests.yaml` & `dvc-3.1.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/.pre-commit-config.yaml` & `dvc-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/.pre-commit-hooks.yaml` & `dvc-3.1.0/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/CODE_OF_CONDUCT.md` & `dvc-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/LICENSE` & `dvc-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/PKG-INFO` & `dvc-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.0.0a2
+Version: 3.1.0
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.0.0a2/README.rst` & `dvc-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/_debug.py` & `dvc-3.1.0/dvc/_debug.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/analytics.py` & `dvc-3.1.0/dvc/analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/annotations.py` & `dvc-3.1.0/dvc/annotations.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/api/data.py` & `dvc-3.1.0/dvc/api/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 def open(  # noqa, pylint: disable=redefined-builtin
     path: str,
     repo: Optional[str] = None,
     rev: Optional[str] = None,
     remote: Optional[str] = None,
     mode: str = "r",
     encoding: Optional[str] = None,
+    config: Optional[Dict[str, Any]] = None,
 ):
     """
     Opens a file tracked in a DVC project.
 
     This function may only be used as a context manager (using the `with`
     keyword, as shown in the examples).
 
@@ -110,14 +111,16 @@
             Defaults to "r" (read).
             Mirrors the namesake parameter in builtin `open()`_.
             Only reading `mode` is supported.
         encoding(str, optional): `Codec`_ used to decode the file contents.
             Defaults to None.
             This should only be used in text mode.
             Mirrors the namesake parameter in builtin `open()`_.
+        config(dict, optional): config to be passed to the DVC repository.
+            Defaults to None.
 
     Returns:
         _OpenContextManager: A context manager that generatse a corresponding
             `file object`_.
             The exact type of file object depends on the mode used.
             For more details, please refer to Python's `open()`_ built-in,
             which is used under the hood.
@@ -205,22 +208,32 @@
     args = (path,)
     kwargs = {
         "repo": repo,
         "remote": remote,
         "rev": rev,
         "mode": mode,
         "encoding": encoding,
+        "config": config,
     }
     return _OpenContextManager(_open, args, kwargs)
 
 
-def _open(path, repo=None, rev=None, remote=None, mode="r", encoding=None):
-    repo_kwargs: Dict[str, Any] = {"subrepos": True, "uninitialized": True}
+def _open(path, repo=None, rev=None, remote=None, mode="r", encoding=None, config=None):
     if remote:
-        repo_kwargs["config"] = {"core": {"remote": remote}}
+        if config is not None:
+            raise ValueError(
+                "can't specify both `remote` and `config` at the same time"
+            )
+        config = {"core": {"remote": remote}}
+
+    repo_kwargs: Dict[str, Any] = {
+        "subrepos": True,
+        "uninitialized": True,
+        "config": config,
+    }
 
     with Repo.open(repo, rev=rev, **repo_kwargs) as _repo:
         with _wrap_exceptions(_repo, path):
             import os
             from typing import TYPE_CHECKING, Union
 
             from dvc.exceptions import IsADirectoryError as DvcIsADirectoryError
@@ -247,17 +260,23 @@
                     yield fobj
             except FileNotFoundError as exc:
                 raise FileMissingError(path) from exc
             except IsADirectoryError as exc:
                 raise DvcIsADirectoryError(f"'{path}' is a directory") from exc
 
 
-def read(path, repo=None, rev=None, remote=None, mode="r", encoding=None):
+def read(path, repo=None, rev=None, remote=None, mode="r", encoding=None, config=None):
     """
     Returns the contents of a tracked file (by DVC or Git). For Git repos, HEAD
     is used unless a rev argument is supplied. The default remote is tried
     unless a remote argument is supplied.
     """
     with open(
-        path, repo=repo, rev=rev, remote=remote, mode=mode, encoding=encoding
+        path,
+        repo=repo,
+        rev=rev,
+        remote=remote,
+        mode=mode,
+        encoding=encoding,
+        config=config,
     ) as fd:
         return fd.read()
```

### Comparing `dvc-3.0.0a2/dvc/api/experiments.py` & `dvc-3.1.0/dvc/api/experiments.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 def exp_show(
     repo: Optional[str] = None,
     revs: Optional[Union[str, List[str]]] = None,
     num: int = 1,
     param_deps: bool = False,
     force: bool = False,
+    config: Optional[Dict] = None,
 ) -> List[Dict]:
     """Get DVC experiments tracked in `repo`.
 
     Without arguments, this function will retrieve all experiments derived from
     the Git `HEAD`.
 
     See the options below to customize the experiments retrieved.
@@ -95,21 +96,23 @@
         force (bool, optional): force re-collection of experiments instead of
             loading from internal experiments cache.
             DVC caches `exp_show` data for completed experiments to improve
             performance of subsequent calls.
             When `force` is specified, DVC will reload all experiment data and
             ignore any previously cached results.
             Defaults to `False`.
+        config (dict, optional): config to be passed through to DVC project.
+            Defaults to `None`.
 
     Returns:
         List[Dict]: Each item in the list will contain a dictionary with
             the info for an individual experiment.
             See Examples below.
     """
-    with Repo.open(repo) as _repo:
+    with Repo.open(repo, config=config) as _repo:
         experiments = _repo.experiments.show(
             revs=revs,
             num=num,
             param_deps=param_deps,
             force=force,
         )
         td, _ = tabulate(experiments, fill_value=None)
```

### Comparing `dvc-3.0.0a2/dvc/api/scm.py` & `dvc-3.1.0/dvc/api/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/api/show.py` & `dvc-3.1.0/dvc/api/show.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     return processed
 
 
 def metrics_show(
     *targets: str,
     repo: Optional[str] = None,
     rev: Optional[str] = None,
+    config: Optional[Dict] = None,
 ) -> Dict:
     """Get metrics tracked in `repo`.
 
     Without arguments, this function will retrieve all metrics from all tracked
     metric files, for the current working tree.
 
     See the options below to restrict the metrics retrieved.
@@ -65,14 +66,16 @@
         rev (str, optional): Name of the `Git revision`_ to retrieve metrics
             from.
             Defaults to `None`.
             An example of git revision can be a branch or tag name, a commit
             hash or a dvc experiment name.
             If `repo` is not a Git repo, this option is ignored.
             If `None`, the current working tree will be used.
+        config (dict, optional): config to be passed through to DVC project.
+            Defaults to `None`.
 
     Returns:
         Dict: See Examples below.
 
     Examples:
 
         - No arguments.
@@ -132,15 +135,15 @@
         }
 
 
     .. _Git revision:
         https://git-scm.com/docs/revisions
     """
 
-    with Repo.open(repo) as _repo:
+    with Repo.open(repo, config=config) as _repo:
         metrics = _repo.metrics.show(
             targets=targets,
             revs=rev if rev is None else [rev],
             onerror=_onerror_raise,
         )
 
     metrics = _postprocess(metrics)
@@ -153,14 +156,15 @@
 
 def params_show(
     *targets: str,
     repo: Optional[str] = None,
     stages: Optional[Union[str, Iterable[str]]] = None,
     rev: Optional[str] = None,
     deps: bool = False,
+    config: Optional[Dict] = None,
 ) -> Dict:
     """Get parameters tracked in `repo`.
 
     Without arguments, this function will retrieve all params from all tracked
     parameter files, for the current working tree.
 
     See the options below to restrict the parameters retrieved.
@@ -191,14 +195,16 @@
             An example of git revision can be a branch or tag name, a commit
             hash or a dvc experiment name.
             If `repo` is not a Git repo, this option is ignored.
             If `None`, the current working tree will be used.
         deps (bool, optional): Whether to retrieve only parameters that are
             stage dependencies or not.
             Defaults to `False`.
+        config (dict, optional): config to be passed through to DVC project.
+            Defaults to `None`.
 
     Returns:
         Dict: See Examples below.
 
     Examples:
 
         - No arguments.
@@ -375,15 +381,15 @@
     .. _Git revision:
         https://git-scm.com/docs/revisions
 
     """
     if isinstance(stages, str):
         stages = [stages]
 
-    with Repo.open(repo) as _repo:
+    with Repo.open(repo, config=config) as _repo:
         params = _repo.params.show(
             revs=rev if rev is None else [rev],
             targets=targets,
             deps=deps,
             onerror=_onerror_raise,
             stages=stages,
         )
```

### Comparing `dvc-3.0.0a2/dvc/cli/__init__.py` & `dvc-3.1.0/dvc/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,25 +71,25 @@
         else:
             _log_unknown_exceptions()
         return None
 
     from dvc.fs import AuthError, ConfigError, RemoteMissingDepsError
 
     if isinstance(exc, RemoteMissingDepsError):
-        from dvc.utils.pkg import PKG
+        from dvc import PKG
 
         proto = exc.protocol
         by_pkg = {
             "pip": f"pip install 'dvc[{proto}]'",
             "conda": f"conda install -c conda-forge dvc-{proto}",
         }
 
-        cmd = by_pkg.get(PKG)
-        if cmd:
+        if PKG in by_pkg:
             link = format_link("https://dvc.org/doc/install")
+            cmd = by_pkg.get(PKG)
             hint = (
                 "To install dvc with those dependencies, run:\n"
                 "\n"
                 f"\t{cmd}\n"
                 "\n"
                 f"See {link} for more info."
             )
@@ -186,16 +186,15 @@
 
         if level is not None:
             set_loggers_level(level)
 
         if level and level <= logging.DEBUG:
             from platform import platform, python_implementation, python_version
 
-            from dvc import __version__
-            from dvc.utils.pkg import PKG
+            from dvc import PKG, __version__
 
             pyv = " ".join([python_implementation(), python_version()])
             pkg = f" ({PKG})" if PKG else ""
             logger.debug("v%s%s, %s on %s", __version__, pkg, pyv, platform())
             logger.debug("command: %s", " ".join(argv or sys.argv))
 
         logger.trace(args)  # type: ignore[attr-defined]
```

### Comparing `dvc-3.0.0a2/dvc/cli/command.py` & `dvc-3.1.0/dvc/cli/command.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/cli/completion.py` & `dvc-3.1.0/dvc/cli/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/cli/parser.py` & `dvc-3.1.0/dvc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/cli/utils.py` & `dvc-3.1.0/dvc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/add.py` & `dvc-3.1.0/dvc/commands/add.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,14 @@
             message += "--to-remote" if args.to_remote else "--out"
             if len(args.targets) != 1:
                 invalid_opt = "multiple targets"
             elif args.glob:
                 invalid_opt = "--glob option"
             elif args.no_commit:
                 invalid_opt = "--no-commit option"
-            elif args.external:
-                invalid_opt = "--external option"
         else:
             message = "{option} can't be used without --to-remote"
             if args.remote:
                 invalid_opt = "--remote"
             elif args.remote_jobs:
                 invalid_opt = "--remote-jobs"
 
@@ -45,15 +43,14 @@
             logger.exception("")
             return 1
 
         try:
             self.repo.add(
                 self.args.targets,
                 no_commit=self.args.no_commit,
-                external=self.args.external,
                 glob=self.args.glob,
                 out=self.args.out,
                 remote=self.args.remote,
                 to_remote=self.args.to_remote,
                 remote_jobs=self.args.remote_jobs,
                 force=self.args.force,
             )
@@ -79,20 +76,14 @@
     parser.add_argument(
         "--no-commit",
         action="store_true",
         default=False,
         help="Don't put files/directories into cache.",
     )
     parser.add_argument(
-        "--external",
-        action="store_true",
-        default=False,
-        help="Allow targets that are outside of the DVC repository.",
-    )
-    parser.add_argument(
         "--glob",
         action="store_true",
         default=False,
         help="Allows targets containing shell-style wildcards.",
     )
     parser.add_argument(
         "-o",
```

### Comparing `dvc-3.0.0a2/dvc/commands/cache.py` & `dvc-3.1.0/dvc/commands/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import os
 
 from dvc.cli import completion
+from dvc.cli.command import CmdBase
 from dvc.cli.utils import append_doc_link, fix_subparsers
 from dvc.commands.config import CmdConfig
 from dvc.ui import ui
 
 
 class CmdCacheDir(CmdConfig):
     def run(self):
@@ -32,14 +33,22 @@
                 del conf["cache"]["dir"]
             else:
                 self._check(conf, False, "cache")
                 conf["cache"]["dir"] = self.args.value
         return 0
 
 
+class CmdCacheMigrate(CmdBase):
+    def run(self):
+        from dvc.cachemgr import migrate_2_to_3
+
+        migrate_2_to_3(self.repo, dry=self.args.dry)
+        return 0
+
+
 def add_parser(subparsers, parent_parser):
     from dvc.commands.config import parent_config_parser
 
     CACHE_HELP = "Manage cache settings."
 
     cache_parser = subparsers.add_parser(
         "cache",
@@ -50,16 +59,14 @@
     )
 
     cache_subparsers = cache_parser.add_subparsers(
         dest="cmd",
         help="Use `dvc cache CMD --help` for command-specific help.",
     )
 
-    fix_subparsers(cache_subparsers)
-
     parent_cache_config_parser = argparse.ArgumentParser(
         add_help=False, parents=[parent_config_parser]
     )
     CACHE_DIR_HELP = "Configure cache directory location."
 
     cache_dir_parser = cache_subparsers.add_parser(
         "dir",
@@ -82,7 +89,27 @@
             "to the current directory and saved to config relative to the "
             "config file location. If no path is provided, it returns the "
             "current cache directory."
         ),
         nargs="?",
     ).complete = completion.DIR
     cache_dir_parser.set_defaults(func=CmdCacheDir)
+
+    CACHE_MIGRATE_HELP = "Migrate cached files to the DVC 3.0 cache location."
+    cache_migrate_parser = cache_subparsers.add_parser(
+        "migrate",
+        parents=[parent_parser],
+        description=append_doc_link(CACHE_HELP, "cache/migrate"),
+        help=CACHE_MIGRATE_HELP,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    cache_migrate_parser.add_argument(
+        "--dry",
+        help=(
+            "Only print actions which would be taken without actually migrating "
+            "any data."
+        ),
+        action="store_true",
+    )
+    cache_migrate_parser.set_defaults(func=CmdCacheMigrate)
+
+    fix_subparsers(cache_subparsers)
```

### Comparing `dvc-3.0.0a2/dvc/commands/check_ignore.py` & `dvc-3.1.0/dvc/commands/check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/checkout.py` & `dvc-3.1.0/dvc/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/commit.py` & `dvc-3.1.0/dvc/commands/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/completion.py` & `dvc-3.1.0/dvc/commands/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/config.py` & `dvc-3.1.0/dvc/commands/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/daemon.py` & `dvc-3.1.0/dvc/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/dag.py` & `dvc-3.1.0/dvc/commands/dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/data.py` & `dvc-3.1.0/dvc/commands/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/data_sync.py` & `dvc-3.1.0/dvc/commands/data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/destroy.py` & `dvc-3.1.0/dvc/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/diff.py` & `dvc-3.1.0/dvc/commands/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/__init__.py` & `dvc-3.1.0/dvc/commands/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/apply.py` & `dvc-3.1.0/dvc/commands/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/branch.py` & `dvc-3.1.0/dvc/commands/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/clean.py` & `dvc-3.1.0/dvc/commands/experiments/clean.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/diff.py` & `dvc-3.1.0/dvc/commands/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/exec_run.py` & `dvc-3.1.0/dvc/commands/experiments/exec_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/ls.py` & `dvc-3.1.0/dvc/commands/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/pull.py` & `dvc-3.1.0/dvc/commands/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/push.py` & `dvc-3.1.0/dvc/commands/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/queue_worker.py` & `dvc-3.1.0/dvc/commands/experiments/queue_worker.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/remove.py` & `dvc-3.1.0/dvc/commands/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/run.py` & `dvc-3.1.0/dvc/commands/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/save.py` & `dvc-3.1.0/dvc/commands/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/experiments/show.py` & `dvc-3.1.0/dvc/commands/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/freeze.py` & `dvc-3.1.0/dvc/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/gc.py` & `dvc-3.1.0/dvc/commands/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/get.py` & `dvc-3.1.0/dvc/commands/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/get_url.py` & `dvc-3.1.0/dvc/commands/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/git_hook.py` & `dvc-3.1.0/dvc/commands/git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/imp.py` & `dvc-3.1.0/dvc/commands/imp.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         from dvc.scm import CloneError
 
         try:
             self.repo.imp(
                 self.args.url,
                 self.args.path,
                 out=self.args.out,
-                fname=self.args.file,
                 rev=self.args.rev,
                 no_exec=self.args.no_exec,
                 no_download=self.args.no_download,
                 jobs=self.args.jobs,
             )
         except CloneError:
             logger.exception("failed to import '%s'", self.args.path)
@@ -65,19 +64,14 @@
     ).complete = completion.DIR
     import_parser.add_argument(
         "--rev",
         nargs="?",
         help="Git revision (e.g. SHA, branch, tag)",
         metavar="<commit>",
     )
-    import_parser.add_argument(
-        "--file",
-        help="Specify name of the .dvc file this command will generate.",
-        metavar="<filename>",
-    )
     no_download_exec_group = import_parser.add_mutually_exclusive_group()
     no_download_exec_group.add_argument(
         "--no-exec",
         action="store_true",
         default=False,
         help="Only create .dvc file without actually importing target data.",
     )
```

### Comparing `dvc-3.0.0a2/dvc/commands/imp_url.py` & `dvc-3.1.0/dvc/commands/imp_url.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 class CmdImportUrl(CmdBase):
     def run(self):
         try:
             self.repo.imp_url(
                 self.args.url,
                 out=self.args.out,
-                fname=self.args.file,
                 no_exec=self.args.no_exec,
                 no_download=self.args.no_download,
                 remote=self.args.remote,
                 to_remote=self.args.to_remote,
                 jobs=self.args.jobs,
                 force=self.args.force,
                 version_aware=self.args.version_aware,
@@ -61,19 +60,14 @@
             "remote://remote_name/path/to/file/or/dir (see `dvc remote`)"
         ),
     )
     import_parser.add_argument(
         "out", nargs="?", help="Destination path to put files to."
     ).complete = completion.DIR
     import_parser.add_argument(
-        "--file",
-        help="Specify name of the .dvc file this command will generate.",
-        metavar="<filename>",
-    ).complete = completion.DIR
-    import_parser.add_argument(
         "--to-remote",
         action="store_true",
         default=False,
         help="Download it directly to the remote",
     )
     import_parser.add_argument(
         "-r",
```

### Comparing `dvc-3.0.0a2/dvc/commands/init.py` & `dvc-3.1.0/dvc/commands/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/install.py` & `dvc-3.1.0/dvc/commands/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/ls/__init__.py` & `dvc-3.1.0/dvc/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/ls/ls_colors.py` & `dvc-3.1.0/dvc/commands/ls/ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/ls_url.py` & `dvc-3.1.0/dvc/commands/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/machine.py` & `dvc-3.1.0/dvc/commands/machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/metrics.py` & `dvc-3.1.0/dvc/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/move.py` & `dvc-3.1.0/dvc/commands/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/params.py` & `dvc-3.1.0/dvc/commands/params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/plots.py` & `dvc-3.1.0/dvc/commands/plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/queue/__init__.py` & `dvc-3.1.0/dvc/commands/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/queue/kill.py` & `dvc-3.1.0/dvc/commands/queue/kill.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/queue/logs.py` & `dvc-3.1.0/dvc/commands/queue/logs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/queue/remove.py` & `dvc-3.1.0/dvc/commands/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/queue/start.py` & `dvc-3.1.0/dvc/commands/queue/start.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/queue/status.py` & `dvc-3.1.0/dvc/commands/queue/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/queue/stop.py` & `dvc-3.1.0/dvc/commands/queue/stop.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/remote.py` & `dvc-3.1.0/dvc/commands/remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/remove.py` & `dvc-3.1.0/dvc/commands/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/repro.py` & `dvc-3.1.0/dvc/commands/repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/root.py` & `dvc-3.1.0/dvc/commands/root.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/stage.py` & `dvc-3.1.0/dvc/commands/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/status.py` & `dvc-3.1.0/dvc/commands/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/unprotect.py` & `dvc-3.1.0/dvc/commands/unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/update.py` & `dvc-3.1.0/dvc/commands/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/commands/version.py` & `dvc-3.1.0/dvc/commands/version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/compare.py` & `dvc-3.1.0/dvc/compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/config.py` & `dvc-3.1.0/dvc/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/config_schema.py` & `dvc-3.1.0/dvc/config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,21 +150,21 @@
         Optional("autostage", default=False): Bool,
         Optional("experiments"): Bool,  # obsoleted
         Optional("check_update", default=True): Bool,
         "site_cache_dir": str,
         "machine": Lower,
     },
     "cache": {
-        "local": str,
-        "s3": str,
-        "gs": str,
-        "hdfs": str,
-        "webhdfs": str,
-        "ssh": str,
-        "azure": str,
+        "local": str,  # obsoleted
+        "s3": str,  # obsoleted
+        "gs": str,  # obsoleted
+        "hdfs": str,  # obsoleted
+        "webhdfs": str,  # obsoleted
+        "ssh": str,  # obsoleted
+        "azure": str,  # obsoleted
         # This is for default local cache
         "dir": str,
         **LOCAL_COMMON,
     },
     "remote": {
         str: ByUrl(
             {
```

### Comparing `dvc-3.0.0a2/dvc/daemon.py` & `dvc-3.1.0/dvc/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/dagascii.py` & `dvc-3.1.0/dvc/dagascii.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/dependency/__init__.py` & `dvc-3.1.0/dvc/dependency/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
 
 def loadd_from(stage, d_list):
     ret = []
     for d in d_list:
         p = d.pop(Output.PARAM_PATH, None)
         files = d.pop(Output.PARAM_FILES, None)
-        ret.append(_get(stage, p, d, files=files))
+        hash_name = d.pop(Output.PARAM_HASH, None)
+        ret.append(_get(stage, p, d, files=files, hash_name=hash_name))
     return ret
 
 
 def loads_from(stage, s_list, erepo=None, fs_config=None):
     assert isinstance(s_list, list)
     info = {RepoDependency.PARAM_REPO: erepo} if erepo else {}
     return [
```

### Comparing `dvc-3.0.0a2/dvc/dependency/base.py` & `dvc-3.1.0/dvc/dependency/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/dependency/param.py` & `dvc-3.1.0/dvc/dependency/param.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             hash_info = HashInfo(
                 self.PARAM_PARAMS,
                 params,  # type: ignore[arg-type]
             )
         repo = repo or stage.repo
         path = path or os.path.join(repo.root_dir, self.DEFAULT_PARAMS_FILE)
         super().__init__(stage, path, repo=repo)
+        self.hash_name = self.PARAM_PARAMS
         self.hash_info = hash_info
 
     def dumpd(self, **kwargs):
         ret = super().dumpd()
         if not self.hash_info:
             ret[self.PARAM_PARAMS] = self.params or {}
         return ret
```

### Comparing `dvc-3.0.0a2/dvc/dependency/repo.py` & `dvc-3.1.0/dvc/dependency/repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def _make_fs(
         self, rev: Optional[str] = None, locked: bool = True
     ) -> "DVCFileSystem":
         from dvc.fs import DVCFileSystem
 
         config = {"cache": self.repo.config["cache"]}
-        config["cache"]["dir"] = self.repo.cache.local.path
+        config["cache"]["dir"] = self.repo.cache.local_cache_dir
 
         return DVCFileSystem(
             url=self.def_repo[self.PARAM_URL],
             rev=rev or self._get_rev(locked=locked),
             subrepos=True,
             config=config,
         )
```

### Comparing `dvc-3.0.0a2/dvc/dirs.py` & `dvc-3.1.0/dvc/dirs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/dvcfile.py` & `dvc-3.1.0/dvc/dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/env.py` & `dvc-3.1.0/dvc/env.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/exceptions.py` & `dvc-3.1.0/dvc/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,29 +295,14 @@
 
 
 class URLMissingError(DvcException):
     def __init__(self, url):
         super().__init__(f"The path '{url}' does not exist")
 
 
-class RemoteCacheRequiredError(DvcException):
-    def __init__(self, scheme, fs_path):
-        super().__init__(
-            (
-                "Current operation was unsuccessful because '{}' requires "
-                "existing cache on '{}' remote. See {} for information on how "
-                "to set up remote cache."
-            ).format(
-                fs_path,
-                scheme,
-                format_link("https://man.dvc.org/config#cache"),
-            )
-        )
-
-
 class IsADirectoryError(DvcException):  # noqa,pylint:disable=redefined-builtin
     """Raised when a file operation is requested on a directory."""
 
 
 class NoOutputOrStageError(DvcException):
     """
     Raised when the target is neither an output nor a stage name in dvc.yaml
```

### Comparing `dvc-3.0.0a2/dvc/fs/__init__.py` & `dvc-3.1.0/dvc/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/fs/callbacks.py` & `dvc-3.1.0/dvc/fs/callbacks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/fs/data.py` & `dvc-3.1.0/dvc/fs/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/fs/dvc.py` & `dvc-3.1.0/dvc/fs/dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/fs/git.py` & `dvc-3.1.0/dvc/fs/git.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/ignore.py` & `dvc-3.1.0/dvc/ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/info.py` & `dvc-3.1.0/dvc/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 import itertools
 import os
 import pathlib
 import platform
 
 import psutil
 
-from dvc import __version__
+from dvc import PKG, __version__
 from dvc.exceptions import NotDvcRepoError
 from dvc.fs import Schemes, generic, get_fs_cls, get_fs_config, registry
 from dvc.repo import Repo
 from dvc.scm import SCMError
 from dvc.utils import error_link
-from dvc.utils.pkg import PKG
 
 SUBPROJECTS = (
     "dvc_data",
     "dvc_objects",
     "dvc_render",
     "dvc_task",
     "scmrepo",
@@ -64,15 +63,15 @@
     return "\n".join(info)
 
 
 def _get_caches(cache):
     caches = (
         cache_type
         for cache_type, cache_instance in cache.by_scheme()
-        if cache_instance and cache_type != "repo"
+        if cache_instance and cache_type not in ("repo", "legacy")
     )
 
     # Caches will be always non-empty including the local cache
     return ", ".join(caches)
 
 
 def _get_remotes(config):
```

### Comparing `dvc-3.0.0a2/dvc/lock.py` & `dvc-3.1.0/dvc/lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/logger.py` & `dvc-3.1.0/dvc/logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/machine/__init__.py` & `dvc-3.1.0/dvc/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/machine/backend/base.py` & `dvc-3.1.0/dvc/machine/backend/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/machine/backend/terraform.py` & `dvc-3.1.0/dvc/machine/backend/terraform.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/output.py` & `dvc-3.1.0/dvc/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from dvc.exceptions import (
     CacheLinkError,
     CheckoutError,
     CollectCacheError,
     ConfirmRemoveError,
     DvcException,
     MergeError,
-    RemoteCacheRequiredError,
 )
 from dvc.utils.objects import cached_property
 from dvc_data.hashfile import check as ocheck
 from dvc_data.hashfile import load as oload
 from dvc_data.hashfile.build import build
 from dvc_data.hashfile.checkout import checkout
 from dvc_data.hashfile.db import HashFileDB, add_update_tree
+from dvc_data.hashfile.hash import DEFAULT_ALGORITHM
 from dvc_data.hashfile.hash_info import HashInfo
 from dvc_data.hashfile.istextfile import istextfile
 from dvc_data.hashfile.meta import Meta
 from dvc_data.hashfile.transfer import transfer as otransfer
 from dvc_data.hashfile.tree import Tree, du
 from dvc_objects.errors import ObjectFormatError
 
@@ -60,24 +60,24 @@
     None,
     And(str, Length(max=0), SetTo(None)),
     And(Any(str, And(int, Coerce(str))), Length(min=3)),
 )
 
 # NOTE: currently there are only 3 possible checksum names:
 #
-#    1) md5 (LOCAL, SSH);
+#    1) md5 (LOCAL, SSH) (actually DVC 2.x md5-dos2unix)
 #    2) etag (S3, GS, OSS, AZURE, HTTP);
 #    3) checksum (HDFS);
 #
 # so when a few types of outputs share the same name, we only need
 # specify it once.
 HDFS_PARAM_CHECKSUM = "checksum"
 S3_PARAM_CHECKSUM = "etag"
 CHECKSUMS_SCHEMA = {
-    LocalFileSystem.PARAM_CHECKSUM: CHECKSUM_SCHEMA,
+    "md5": CHECKSUM_SCHEMA,  # DVC 2.x md5-dos2unix
     HDFS_PARAM_CHECKSUM: CHECKSUM_SCHEMA,
     S3_PARAM_CHECKSUM: CASE_SENSITIVE_CHECKSUM_SCHEMA,
 }
 
 
 def _get(stage, path, **kwargs):
     return Output(stage, path, **kwargs)
@@ -91,27 +91,29 @@
         metric = d.pop(Output.PARAM_METRIC, False)
         plot = d.pop(Output.PARAM_PLOT, False)
         persist = d.pop(Output.PARAM_PERSIST, False)
         remote = d.pop(Output.PARAM_REMOTE, None)
         annot = {field: d.pop(field, None) for field in ANNOTATION_FIELDS}
         files = d.pop(Output.PARAM_FILES, None)
         push = d.pop(Output.PARAM_PUSH, True)
+        hash_name = d.pop(Output.PARAM_HASH, None)
         ret.append(
             _get(
                 stage,
                 p,
                 info=d,
                 cache=cache,
                 metric=metric,
                 plot=plot,
                 persist=persist,
                 remote=remote,
                 **annot,
                 files=files,
                 push=push,
+                hash_name=hash_name,
             )
         )
     return ret
 
 
 def loads_from(
     stage,
@@ -223,25 +225,37 @@
     cloud_meta = entry.pop(Output.PARAM_CLOUD, {})
     if remote_name := first(cloud_meta):
         entry.update(cloud_meta[remote_name])
         entry[Meta.PARAM_REMOTE] = remote_name
     return entry
 
 
-def _serialize_tree_obj_to_files(obj: "Tree") -> List[Dict[str, Any]]:
+def _serialize_tree_obj_to_files(obj: Tree) -> List[Dict[str, Any]]:
     key = obj.PARAM_RELPATH
     return sorted(
         (
-            {key: posixpath.sep.join(parts), **hi.to_dict(), **meta.to_dict()}
+            {
+                key: posixpath.sep.join(parts),
+                **_serialize_hi_to_dict(hi),
+                **meta.to_dict(),
+            }
             for parts, meta, hi in obj
         ),
         key=itemgetter(key),
     )
 
 
+def _serialize_hi_to_dict(hash_info: Optional[HashInfo]) -> Dict[str, Any]:
+    if hash_info:
+        if hash_info.name == "md5-dos2unix":
+            return {"md5": hash_info.value}
+        return hash_info.to_dict()
+    return {}
+
+
 class OutputDoesNotExistError(DvcException):
     def __init__(self, path):
         msg = f"output '{path}' does not exist"
         super().__init__(msg)
 
 
 class OutputIsNotFileOrDirError(DvcException):
@@ -293,14 +307,15 @@
     PARAM_PLOT_Y_LABEL = "y_label"
     PARAM_PLOT_TITLE = "title"
     PARAM_PLOT_HEADER = "header"
     PARAM_PERSIST = "persist"
     PARAM_REMOTE = "remote"
     PARAM_PUSH = "push"
     PARAM_CLOUD = "cloud"
+    PARAM_HASH = "hash"
 
     DoesNotExistError: Type[DvcException] = OutputDoesNotExistError
     IsNotFileOrDirError: Type[DvcException] = OutputIsNotFileOrDirError
     IsStageFileError: Type[DvcException] = OutputIsStageFileError
     IsIgnoredError: Type[DvcException] = OutputIsIgnoredError
 
     def __init__(  # noqa: PLR0913
@@ -317,14 +332,15 @@
         labels=None,
         meta=None,
         remote=None,
         repo=None,
         fs_config=None,
         files: Optional[List[Dict[str, Any]]] = None,
         push: bool = True,
+        hash_name: Optional[str] = DEFAULT_ALGORITHM,
     ):
         self.annot = Annotation(
             desc=desc, type=type, labels=labels or [], meta=meta or {}
         )
         self.repo = stage.repo if not repo and stage else repo
         meta_d = merge_file_meta_from_cloud(info or {})
         meta = Meta.from_dict(meta_d)
@@ -388,24 +404,37 @@
 
         if self.fs.version_aware:
             _, version_id = self.fs.path.coalesce_version(
                 self.def_path, self.meta.version_id
             )
             self.meta.version_id = version_id
 
+        self.hash_name, self.hash_info = self._compute_hash_info_from_meta(hash_name)
+        self._compute_meta_hash_info_from_files()
+
+    def _compute_hash_info_from_meta(
+        self, hash_name: Optional[str]
+    ) -> Tuple[str, HashInfo]:
         if self.is_in_repo:
-            self.hash_name = "md5"
+            if hash_name is None:
+                # Legacy 2.x output, use "md5-dos2unix" but read "md5" from
+                # file meta
+                hash_name = "md5-dos2unix"
+                meta_name = "md5"
+            else:
+                meta_name = hash_name
         else:
-            self.hash_name = self.fs.PARAM_CHECKSUM
+            hash_name = meta_name = self.fs.PARAM_CHECKSUM
+        assert hash_name
 
-        self.hash_info = HashInfo(
-            name=self.hash_name,
-            value=getattr(self.meta, self.hash_name, None),
+        hash_info = HashInfo(
+            name=hash_name,
+            value=getattr(self.meta, meta_name, None),
         )
-        self._compute_meta_hash_info_from_files()
+        return hash_name, hash_info
 
     def _compute_meta_hash_info_from_files(self) -> None:
         if self.files:
             tree = Tree.from_list(self.files, hash_name=self.hash_name)
             tree.digest(with_meta=True)
             self.odb = HashFileDB(tree.fs, tree.path + ".odb")
             self.odb.add(tree.path, tree.fs, tree.hash_info.value)
@@ -413,15 +442,15 @@
             self.hash_info = tree.hash_info
             self.meta.isdir = True
             self.meta.nfiles = len(self.files)
             self.meta.size = sum(filter(None, (f.get("size") for f in self.files)))
             self.meta.remote = first(f.get("remote") for f in self.files)
         elif self.meta.nfiles or self.hash_info and self.hash_info.isdir:
             self.meta.isdir = True
-            if not self.hash_info and self.hash_name != "md5":
+            if not self.hash_info and self.hash_name not in ("md5", "md5-dos2unix"):
                 md5 = getattr(self.meta, "md5", None)
                 if md5:
                     self.hash_info = HashInfo("md5", md5)
 
     def _parse_path(self, fs, fs_path):
         parsed = urlparse(self.def_path)
         if (
@@ -477,32 +506,40 @@
         if urlparse(self.def_path).scheme == "remote":
             return False
 
         if self.fs.path.isabs(self.def_path):
             return False
 
         return self.repo and self.fs.path.isin(
-            self.fs.path.realpath(self.fs_path),
+            self.fs_path,
             self.repo.root_dir,
         )
 
     @property
     def use_scm_ignore(self):
         if not self.is_in_repo:
             return False
 
         return self.use_cache or self.stage.is_repo_import
 
     @property
     def cache(self):
-        odb_name = "repo" if self.is_in_repo else self.protocol
-        odb = getattr(self.repo.cache, odb_name)
-        if self.use_cache and odb is None:
-            raise RemoteCacheRequiredError(self.fs.protocol, self.fs_path)
-        return odb
+        from dvc.cachemgr import LEGACY_HASH_NAMES
+
+        assert self.is_in_repo
+        odb_name = "legacy" if self.hash_name in LEGACY_HASH_NAMES else "repo"
+        return getattr(self.repo.cache, odb_name)
+
+    @property
+    def local_cache(self):
+        from dvc.cachemgr import LEGACY_HASH_NAMES
+
+        if self.hash_name in LEGACY_HASH_NAMES:
+            return self.repo.cache.legacy
+        return self.repo.cache.local
 
     @property
     def cache_path(self):
         return self.cache.fs.unstrip_protocol(
             self.cache.oid_to_path(self.hash_info.value)
         )
 
@@ -510,15 +547,15 @@
         _, hash_info = self._get_hash_meta()
         return hash_info
 
     def _get_hash_meta(self):
         if self.use_cache:
             odb = self.cache
         else:
-            odb = self.repo.cache.local
+            odb = self.local_cache
         _, meta, obj = build(
             odb,
             self.fs_path,
             self.fs,
             self.hash_name,
             ignore=self.dvcignore,
             dry_run=not self.use_cache,
@@ -651,25 +688,27 @@
             logger.warning("'%s' is empty.", self)
 
         self.ignore()
 
         if self.metric:
             self.verify_metric()
 
+        if self.hash_name == "md5-dos2unix":
+            self.hash_name = "md5"
         if self.use_cache:
             _, self.meta, self.obj = build(
                 self.cache,
                 self.fs_path,
                 self.fs,
                 self.hash_name,
                 ignore=self.dvcignore,
             )
         else:
             _, self.meta, self.obj = build(
-                self.repo.cache.local,
+                self.local_cache,
                 self.fs_path,
                 self.fs,
                 self.hash_name,
                 ignore=self.dvcignore,
                 dry_run=True,
             )
             if not self.IS_DEPENDENCY:
@@ -760,32 +799,42 @@
             {save_obj.hash_info} | {oid for _, _, oid in save_obj},
             shallow=True,
             hardlink=hardlink,
         )
         return checkout_obj
 
     def dumpd(self, **kwargs):  # noqa: C901, PLR0912
+        from dvc.cachemgr import LEGACY_HASH_NAMES
+
         ret: Dict[str, Any] = {}
         with_files = (
             (not self.IS_DEPENDENCY or self.stage.is_import)
             and self.hash_info.isdir
             and (kwargs.get("with_files") or self.files is not None)
         )
 
         if not with_files:
             meta_d = self.meta.to_dict()
             meta_d.pop("isdir", None)
-            ret.update(self.hash_info.to_dict())
+            if self.hash_name in LEGACY_HASH_NAMES:
+                # 2.x checksums get serialized with file meta
+                name = "md5" if self.hash_name == "md5-dos2unix" else self.hash_name
+                ret.update({name: self.hash_info.value})
+            else:
+                ret.update(self.hash_info.to_dict())
             ret.update(split_file_meta_from_cloud(meta_d))
 
         if self.is_in_repo:
             path = self.fs.path.as_posix(relpath(self.fs_path, self.stage.wdir))
         else:
             path = self.def_path
 
+        if self.hash_name not in LEGACY_HASH_NAMES:
+            ret[self.PARAM_HASH] = "md5"
+
         ret[self.PARAM_PATH] = path
 
         if not self.IS_DEPENDENCY:
             ret.update(self.annot.to_dict())
             if not self.use_cache:
                 ret[self.PARAM_CACHE] = self.use_cache
 
@@ -957,15 +1006,15 @@
 
         upload = not (update and from_fs.isdir(from_info))
         jobs = jobs or min((from_fs.jobs, odb.fs.jobs))
         staging, self.meta, obj = build(
             odb,
             from_info,
             from_fs,
-            "md5",
+            DEFAULT_ALGORITHM,
             upload=upload,
             no_progress_bar=no_progress_bar,
         )
         otransfer(
             staging,
             odb,
             {obj.hash_info},
@@ -1098,15 +1147,17 @@
             if not obj:
                 obj = self.cache.get(self.hash_info.value)
 
         if not obj:
             return {}
 
         if self.remote:
-            remote = self.repo.cloud.get_remote_odb(name=self.remote)
+            remote = self.repo.cloud.get_remote_odb(
+                name=self.remote, hash_name=self.hash_name
+            )
         else:
             remote = None
 
         return {remote: self._named_obj_ids(obj)}
 
     def _named_obj_ids(self, obj):
         name = str(self)
@@ -1137,21 +1188,22 @@
         my = self.dumpd()
         other = out.dumpd()
 
         ignored = [
             self.hash_name,
             Meta.PARAM_SIZE,
             Meta.PARAM_NFILES,
+            Output.PARAM_HASH,
         ]
 
         for opt in ignored:
             my.pop(opt, None)
             other.pop(opt, None)
 
-        if my != other:
+        if my != other or self.hash_name != out.hash_name:
             raise MergeError("unable to auto-merge outputs with different options")
 
         if not out.is_dir_checksum:
             raise MergeError("unable to auto-merge outputs that are not directories")
 
     def merge(self, ancestor, other, allowed=None):
         from dvc_data.hashfile.tree import MergeError as TreeMergeError
@@ -1279,15 +1331,15 @@
         path = path or self.fs_path
         if self.hash_info and not self.is_dir_checksum and self.fs_path != path:
             raise DvcException(
                 f"Cannot modify '{self}' which is being tracked as a file"
             )
 
         assert self.repo
-        cache = self.cache if self.use_cache else self.repo.cache.local
+        cache = self.cache if self.use_cache else self.local_cache
         assert isinstance(cache, HashFileDB)
 
         new: "HashFile"
         try:
             assert self.hash_name
             staging, meta, obj = build(
                 cache,
@@ -1406,14 +1458,15 @@
 
 ARTIFACT_SCHEMA = {
     **CHECKSUMS_SCHEMA,
     **META_SCHEMA,
     Required(Output.PARAM_PATH): str,
     Output.PARAM_PERSIST: bool,
     Output.PARAM_CLOUD: CLOUD_SCHEMA,
+    Output.PARAM_HASH: str,
 }
 
 DIR_FILES_SCHEMA: Dict[str, Any] = {
     **CHECKSUMS_SCHEMA,
     **META_SCHEMA,
     Required(Tree.PARAM_RELPATH): str,
     Output.PARAM_CLOUD: CLOUD_SCHEMA,
```

### Comparing `dvc-3.0.0a2/dvc/parsing/__init__.py` & `dvc-3.1.0/dvc/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/parsing/context.py` & `dvc-3.1.0/dvc/parsing/context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/parsing/interpolate.py` & `dvc-3.1.0/dvc/parsing/interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/pathspec_math.py` & `dvc-3.1.0/dvc/pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/progress.py` & `dvc-3.1.0/dvc/progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/prompt.py` & `dvc-3.1.0/dvc/prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/render/convert.py` & `dvc-3.1.0/dvc/render/convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/render/converter/__init__.py` & `dvc-3.1.0/dvc/render/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/render/converter/image.py` & `dvc-3.1.0/dvc/render/converter/image.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/render/converter/vega.py` & `dvc-3.1.0/dvc/render/converter/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/render/match.py` & `dvc-3.1.0/dvc/render/match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/__init__.py` & `dvc-3.1.0/dvc/repo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,22 @@
         if self._data_index is None:
             index_dir = os.path.join(self.site_cache_dir, "index", "data")
             os.makedirs(index_dir, exist_ok=True)
             self._data_index = DataIndex.open(os.path.join(index_dir, "db.db"))
 
         return self._data_index
 
+    def drop_data_index(self) -> None:
+        try:
+            self.data_index.delete_node(("tree",))
+        except KeyError:
+            pass
+        self.data_index.commit()
+        self._reset()
+
     def __repr__(self):
         return f"{self.__class__.__name__}: '{self.root_dir}'"
 
     @classmethod
     def find_root(cls, root=None, fs=None) -> str:
         from dvc.fs import LocalFileSystem, localfs
 
@@ -416,16 +424,16 @@
     def unprotect(self, target):
         return self.cache.repo.unprotect(target)
 
     def _ignore(self):
         flist = [self.config.files["local"]]
         if tmp_dir := self.tmp_dir:
             flist.append(tmp_dir)
-        if path_isin(self.cache.repo.path, self.root_dir):
-            flist.append(self.cache.repo.path)
+        if path_isin(self.cache.legacy.path, self.root_dir):
+            flist.append(self.cache.legacy.path)
 
         for file in flist:
             self.scm_context.ignore(file)
 
     def brancher(self, *args, **kwargs):
         from dvc.repo.brancher import brancher
```

### Comparing `dvc-3.0.0a2/dvc/repo/add.py` & `dvc-3.1.0/dvc/repo/add.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     "Run the pipeline or use 'dvc commit' to force update it."
 )
 
 
 def get_or_create_stage(
     repo: "Repo",
     target: str,
-    external: bool = False,
     out: Optional[str] = None,
     to_remote: bool = False,
     force: bool = False,
 ) -> StageInfo:
     if out:
         target = resolve_output(target, out, force=force)
     path, wdir, out = resolve_paths(repo, target, always_local=to_remote and not out)
@@ -75,15 +74,14 @@
     except OutputNotFoundError:
         stage = repo.stage.create(
             single_stage=True,
             validate=False,
             fname=path,
             wdir=wdir,
             outs=[out],
-            external=external,
             force=force,
         )
         return StageInfo(stage, output_exists=False)
 
 
 OVERLAPPING_CHILD_FMT = (
     "Cannot add '{out}', because it is overlapping with other "
@@ -195,15 +193,14 @@
 
 @locked
 @scm_context
 def add(
     repo: "Repo",
     targets: Union["StrOrBytesPath", Iterator["StrOrBytesPath"]],
     no_commit: bool = False,
-    external: bool = False,
     glob: bool = False,
     out: Optional[str] = None,
     remote: Optional[str] = None,
     to_remote: bool = False,
     remote_jobs: Optional[int] = None,
     force: bool = False,
 ) -> List["Stage"]:
@@ -211,15 +208,14 @@
     if not add_targets:
         return []
 
     stages_with_targets = {
         target: get_or_create_stage(
             repo,
             target,
-            external=external,
             out=out,
             to_remote=to_remote,
             force=force,
         )
         for target in add_targets
     }
```

### Comparing `dvc-3.0.0a2/dvc/repo/artifacts.py` & `dvc-3.1.0/dvc/repo/artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/brancher.py` & `dvc-3.1.0/dvc/repo/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/checkout.py` & `dvc-3.1.0/dvc/repo/checkout.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,17 +70,15 @@
     allow_missing=False,
     **kwargs,
 ):
     from dvc import prompt
     from dvc.fs.callbacks import Callback
     from dvc.repo.index import build_data_index
     from dvc.stage.exceptions import StageFileBadNameError, StageFileDoesNotExistError
-    from dvc_data.hashfile.checkout import CheckoutError as IndexCheckoutError
-    from dvc_data.index.checkout import ADD, DELETE, MODIFY
-    from dvc_data.index.checkout import checkout as icheckout
+    from dvc_data.index.checkout import ADD, DELETE, MODIFY, apply, compare
 
     stats: Dict[str, List[str]] = {
         "added": [],
         "deleted": [],
         "modified": [],
     }
     if not targets:
@@ -115,53 +113,50 @@
     ) as cb:
         old = build_data_index(
             view, self.root_dir, self.fs, compute_hash=True, callback=cb
         )
 
     new = view.data["repo"]
 
-    for out in view.outs:
-        out.changed_cache()
+    with Callback.as_tqdm_callback(
+        desc="Comparing indexes",
+        unit="entry",
+    ) as cb:
+        diff = compare(old, new, relink=relink, delete=True, callback=cb)
+
+    failed = []
+
+    def checkout_onerror(src_path, dest_path, _exc):
+        logger.debug(
+            "failed to create {%s} from {%s}", dest_path, src_path, exc_info=True
+        )
+        failed.append(dest_path)
 
     with Callback.as_tqdm_callback(
         unit="file",
         desc="Checkout",
     ) as cb:
-        try:
-            changes = icheckout(
-                new,
-                self.root_dir,
-                self.fs,
-                old=old,
-                callback=cb,
-                delete=True,
-                prompt=prompt.confirm,
-                update_meta=False,
-                relink=relink,
-                force=force,
-                allow_missing=allow_missing,
-                state=self.state,
-                **kwargs,
-            )
-        except IndexCheckoutError as exc:
-            raise CheckoutError(exc.paths, {}) from exc
+        changes = apply(
+            diff,
+            self.root_dir,
+            self.fs,
+            callback=cb,
+            prompt=prompt.confirm,
+            update_meta=False,
+            force=force,
+            onerror=checkout_onerror,
+            state=self.state,
+            **kwargs,
+        )
 
     out_changes = _build_out_changes(view, changes)
 
     typ_map = {ADD: "added", DELETE: "deleted", MODIFY: "modified"}
     for key, typ in out_changes.items():
         out_path = self.fs.path.join(self.root_dir, *key)
         self.state.save_link(out_path, self.fs)
         stats[typ_map[typ]].append(_fspath_dir(out_path))
 
-    failed = []
-    for out in view.outs:
-        if not out.use_cache:
-            continue
-
-        if not out.hash_info:
-            failed.append(_fspath_dir(out.fs_path))
-
-    if not allow_missing and failed:
+    if failed and not allow_missing:
         raise CheckoutError(failed, stats)
 
     return stats
```

### Comparing `dvc-3.0.0a2/dvc/repo/collect.py` & `dvc-3.1.0/dvc/repo/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/commit.py` & `dvc-3.1.0/dvc/repo/commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             f"unable to commit changed {stage}. Use `-f|--force` to force."
         )
 
 
 @locked
 def commit(
     self,
-    target,
+    target=None,
     with_deps=False,
     recursive=False,
     force=False,
     allow_missing=False,
     data_only=False,
     relink=True,
 ):
```

### Comparing `dvc-3.0.0a2/dvc/repo/data.py` & `dvc-3.1.0/dvc/repo/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/destroy.py` & `dvc-3.1.0/dvc/repo/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/diff.py` & `dvc-3.1.0/dvc/repo/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,12 +152,17 @@
         old_missing = missing_targets.get(a_rev, set())
         new_missing = missing_targets.get(b_rev, set())
 
         # check for overlapping missing targets between a_rev and b_rev
         for target in old_missing & new_missing:
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), target)
 
-    old = indexes[a_rev]
-    new = indexes[b_rev]
+    if len(indexes.keys()) == 1:
+        # both a_rev and b_rev point to the same sha, nothing to compare
+        old = None
+        new = None
+    else:
+        old = indexes[a_rev]
+        new = indexes[b_rev]
 
     with ui.status("Calculating diff"):
         return _diff(old, new, with_missing=with_missing)
```

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/__init__.py` & `dvc-3.1.0/dvc/repo/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/apply.py` & `dvc-3.1.0/dvc/repo/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/branch.py` & `dvc-3.1.0/dvc/repo/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/brancher.py` & `dvc-3.1.0/dvc/repo/experiments/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/cache.py` & `dvc-3.1.0/dvc/repo/experiments/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/collect.py` & `dvc-3.1.0/dvc/repo/experiments/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/diff.py` & `dvc-3.1.0/dvc/repo/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/exceptions.py` & `dvc-3.1.0/dvc/repo/experiments/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/executor/base.py` & `dvc-3.1.0/dvc/repo/experiments/executor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,15 +511,14 @@
 
             if not repro_dry:
                 dvc_checkout(
                     dvc,
                     targets=targets,
                     with_deps=targets is not None,
                     force=True,
-                    quiet=True,
                     allow_missing=True,
                     recursive=kwargs.get("recursive", False),
                 )
 
             stages = dvc_reproduce(
                 dvc,
                 *args,
```

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/executor/local.py` & `dvc-3.1.0/dvc/repo/experiments/executor/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             with open(local_config, "wb") as fobj:
                 conf_obj.write(fobj)
 
     def init_cache(
         self, repo: "Repo", rev: str, run_cache: bool = True  # noqa: ARG002
     ):
         """Initialize DVC cache."""
-        self._update_config({"cache": {"dir": repo.cache.repo.path}})
+        self._update_config({"cache": {"dir": repo.cache.local_cache_dir}})
 
     def cleanup(self, infofile: Optional[str] = None):
         super().cleanup(infofile)
         logger.debug("Removing tmpdir '%s'", self.root_dir)
         remove(self.root_dir)
 
     @classmethod
```

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/executor/ssh.py` & `dvc-3.1.0/dvc/repo/experiments/executor/ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/ls.py` & `dvc-3.1.0/dvc/repo/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/pull.py` & `dvc-3.1.0/dvc/repo/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/push.py` & `dvc-3.1.0/dvc/repo/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/queue/base.py` & `dvc-3.1.0/dvc/repo/experiments/queue/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/queue/celery.py` & `dvc-3.1.0/dvc/repo/experiments/queue/celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/queue/remove.py` & `dvc-3.1.0/dvc/repo/experiments/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/queue/tasks.py` & `dvc-3.1.0/dvc/repo/experiments/queue/tasks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/queue/tempdir.py` & `dvc-3.1.0/dvc/repo/experiments/queue/tempdir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/queue/utils.py` & `dvc-3.1.0/dvc/repo/experiments/queue/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/queue/workspace.py` & `dvc-3.1.0/dvc/repo/experiments/queue/workspace.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/refs.py` & `dvc-3.1.0/dvc/repo/experiments/refs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/remove.py` & `dvc-3.1.0/dvc/repo/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/run.py` & `dvc-3.1.0/dvc/repo/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/save.py` & `dvc-3.1.0/dvc/repo/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/serialize.py` & `dvc-3.1.0/dvc/repo/experiments/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
         rev = rev or repo.get_rev()
         assert rev
         # NOTE: _gather_params/_gather_metrics return defaultdict which is not
         # supported in dataclasses.asdict() on all python releases
         # see https://bugs.python.org/issue35540
         params = dict(_gather_params(repo, deps=param_deps, onerror=onerror))
+        params = {k: dict(v) for k, v in params.items()}
         metrics = dict(
             _gather_metrics(
                 repo,
                 targets=None,
                 rev=rev[:7],
                 recursive=False,
                 onerror=onerror_collect,
```

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/show.py` & `dvc-3.1.0/dvc/repo/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/stash.py` & `dvc-3.1.0/dvc/repo/experiments/stash.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/experiments/utils.py` & `dvc-3.1.0/dvc/repo/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/fetch.py` & `dvc-3.1.0/dvc/repo/gc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,198 +1,144 @@
 import logging
-from contextlib import suppress
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import TYPE_CHECKING, List, Optional, Set, Tuple
 
-from dvc.config import NoRemoteError
-from dvc.exceptions import DownloadError
-from dvc.fs import Schemes
+from dvc.exceptions import InvalidArgumentError
 
 from . import locked
 
 if TYPE_CHECKING:
-    from dvc.data_cloud import Remote
     from dvc.repo import Repo
-    from dvc.types import TargetType
-    from dvc_data.hashfile.db import HashFileDB
-    from dvc_data.hashfile.transfer import TransferResult
+    from dvc_data.hashfile.hash_info import HashInfo
+    from dvc_objects.db import ObjectDB
 
 logger = logging.getLogger(__name__)
 
 
-@locked
-def fetch(  # noqa: C901, PLR0913
-    self,
-    targets=None,
-    jobs=None,
-    remote=None,
-    all_branches=False,
-    with_deps=False,
-    all_tags=False,
-    recursive=False,
-    all_commits=False,
-    run_cache=False,
-    revs=None,
-    odb: Optional["HashFileDB"] = None,
-) -> int:
-    """Download data items from a cloud and imported repositories
-
-    Returns:
-        int: number of successfully downloaded files
-
-    Raises:
-        DownloadError: thrown when there are failed downloads, either
-            during `cloud.pull` or trying to fetch imported files
-
-        config.NoRemoteError: thrown when downloading only local files and no
-            remote is configured
-    """
-    from dvc.repo.imports import save_imports
-    from dvc_data.hashfile.transfer import TransferResult
-
-    if isinstance(targets, str):
-        targets = [targets]
-
-    worktree_remote: Optional["Remote"] = None
-    with suppress(NoRemoteError):
-        _remote = self.cloud.get_remote(name=remote)
-        if _remote.worktree or _remote.fs.version_aware:
-            worktree_remote = _remote
-
-    failed_count = 0
-    transferred_count = 0
-
-    try:
-        if run_cache:
-            self.stage_cache.pull(remote)
-    except DownloadError as exc:
-        failed_count += exc.amount
-
-    no_remote_msg: Optional[str] = None
-    result = TransferResult(set(), set())
-    try:
-        if worktree_remote is not None:
-            transferred_count += _fetch_worktree(
-                self,
-                worktree_remote,
-                revs=revs,
-                all_branches=all_branches,
-                all_tags=all_tags,
-                all_commits=all_commits,
-                targets=targets,
-                jobs=jobs,
-                with_deps=with_deps,
-                recursive=recursive,
-            )
-        else:
-            d, f = _fetch(
-                self,
-                targets,
-                all_branches=all_branches,
-                all_tags=all_tags,
-                all_commits=all_commits,
-                with_deps=with_deps,
-                force=True,
-                remote=remote,
-                jobs=jobs,
-                recursive=recursive,
-                revs=revs,
-                odb=odb,
-            )
-            result.transferred.update(d)
-            result.failed.update(f)
-    except NoRemoteError as exc:
-        no_remote_msg = str(exc)
-
-    for rev in self.brancher(
-        revs=revs,
-        all_branches=all_branches,
-        all_tags=all_tags,
-        all_commits=all_commits,
-    ):
-        imported = save_imports(
-            self,
-            targets,
-            unpartial=not rev or rev == "workspace",
-            recursive=recursive,
+def _validate_args(**kwargs):
+    not_in_remote = kwargs.pop("not_in_remote", None)
+    cloud = kwargs.pop("cloud", None)
+    remote = kwargs.pop("remote", None)
+    if remote and not (cloud or not_in_remote):
+        raise InvalidArgumentError("`--remote` requires `--cloud` or `--not-in-remote`")
+    if not_in_remote and cloud:
+        raise InvalidArgumentError(
+            "`--not-in-remote` and `--cloud` are mutually exclusive"
         )
-        result.transferred.update(imported)
-        result.failed.difference_update(imported)
-
-    failed_count += len(result.failed)
-
-    if failed_count:
-        if no_remote_msg:
-            logger.error(no_remote_msg)
-        raise DownloadError(failed_count)
+    if not any(kwargs.values()):
+        raise InvalidArgumentError(
+            "Either of `-w|--workspace`, `-a|--all-branches`, `-T|--all-tags` "
+            "`--all-experiments`, `--all-commits`, `--date` or `--rev` "
+            "needs to be set."
+        )
+    if kwargs.get("num") and not kwargs.get("rev"):
+        raise InvalidArgumentError("`--num` can only be used alongside `--rev`")
 
-    transferred_count += len(result.transferred)
-    return transferred_count
 
+def _used_obj_ids_not_in_remote(repo, default_remote, jobs, remote_odb_to_obj_ids):
+    used_obj_ids = set()
+    remote_oids = set()
+    for remote_odb, obj_ids in remote_odb_to_obj_ids:
+        if remote_odb is None:
+            remote_odb = repo.cloud.get_remote_odb(default_remote, "gc --not-in-remote")
 
-def _fetch(
-    repo: "Repo",
-    targets: "TargetType",
-    remote: Optional[str] = None,
-    jobs: Optional[int] = None,
-    odb: Optional["HashFileDB"] = None,
-    **kwargs,
-) -> "TransferResult":
-    from dvc_data.hashfile.transfer import TransferResult
-
-    result = TransferResult(set(), set())
-    used = repo.used_objs(
-        targets,
-        remote=remote,
-        jobs=jobs,
-        **kwargs,
-    )
-    if odb:
-        all_ids = set()
-        for _odb, obj_ids in used.items():
-            all_ids.update(obj_ids)
-        d, f = repo.cloud.pull(
-            all_ids,
-            jobs=jobs,
-            remote=remote,
-            odb=odb,
+        remote_oids.update(
+            remote_odb.list_oids_exists({x.value for x in obj_ids}, jobs=jobs)
         )
-        result.transferred.update(d)
-        result.failed.update(f)
-    else:
-        for src_odb, obj_ids in sorted(
-            used.items(),
-            key=lambda item: item[0] is not None
-            and item[0].fs.protocol == Schemes.MEMORY,
-        ):
-            d, f = repo.cloud.pull(
-                obj_ids,
-                jobs=jobs,
-                remote=remote,
-                odb=src_odb,
-            )
-            result.transferred.update(d)
-            result.failed.update(f)
-    return result
+        used_obj_ids.update(obj_ids)
+    return {obj for obj in used_obj_ids if obj.value not in remote_oids}
 
 
-def _fetch_worktree(
-    repo: "Repo",
-    remote: "Remote",
-    revs: Optional[Sequence[str]] = None,
+@locked
+def gc(  # noqa: PLR0912, PLR0913, C901
+    self: "Repo",
     all_branches: bool = False,
+    cloud: bool = False,
+    remote: Optional[str] = None,
+    with_deps: bool = False,
     all_tags: bool = False,
     all_commits: bool = False,
-    targets: Optional["TargetType"] = None,
+    all_experiments: bool = False,
+    force: bool = False,
     jobs: Optional[int] = None,
-    **kwargs,
-) -> int:
-    from dvc.repo.worktree import fetch_worktree
-
-    downloaded = 0
-    for _ in repo.brancher(
-        revs=revs,
-        all_branches=all_branches,
+    repos: Optional[List[str]] = None,
+    workspace: bool = False,
+    commit_date: Optional[str] = None,
+    rev: Optional[str] = None,
+    num: Optional[int] = None,
+    not_in_remote: bool = False,
+):
+    # require `workspace` to be true to come into effect.
+    # assume `workspace` to be enabled if any of `all_tags`, `all_commits`,
+    # `all_experiments` or `all_branches` are enabled.
+    _validate_args(
+        workspace=workspace,
         all_tags=all_tags,
         all_commits=all_commits,
-    ):
-        downloaded += fetch_worktree(repo, remote, targets=targets, jobs=jobs, **kwargs)
-    return downloaded
+        all_branches=all_branches,
+        all_experiments=all_experiments,
+        commit_date=commit_date,
+        rev=rev,
+        num=num,
+        cloud=cloud,
+        not_in_remote=not_in_remote,
+    )
+
+    from contextlib import ExitStack
+
+    from dvc.repo import Repo
+    from dvc_data.hashfile.db import get_index
+    from dvc_data.hashfile.gc import gc as ogc
+
+    if not repos:
+        repos = []
+    all_repos = [Repo(path) for path in repos]
+
+    odb_to_obj_ids: List[Tuple[Optional["ObjectDB"], Set["HashInfo"]]] = []
+
+    with ExitStack() as stack:
+        for repo in all_repos:
+            stack.enter_context(repo.lock)
+
+        for repo in [*all_repos, self]:
+            for odb, obj_ids in repo.used_objs(
+                all_branches=all_branches,
+                with_deps=with_deps,
+                all_tags=all_tags,
+                all_commits=all_commits,
+                all_experiments=all_experiments,
+                commit_date=commit_date,
+                remote=remote,
+                force=force,
+                jobs=jobs,
+                revs=[rev] if rev else None,
+                num=num or 1,
+            ).items():
+                odb_to_obj_ids.append((odb, obj_ids))
+
+    if not odb_to_obj_ids:
+        odb_to_obj_ids = [(None, set())]
+
+    if not_in_remote:
+        used_obj_ids = _used_obj_ids_not_in_remote(self, remote, jobs, odb_to_obj_ids)
+    else:
+        used_obj_ids = set()
+        for _, obj_ids in odb_to_obj_ids:
+            used_obj_ids.update(obj_ids)
+
+    for scheme, odb in self.cache.by_scheme():
+        if not odb:
+            continue
+        removed = ogc(odb, used_obj_ids, jobs=jobs)
+        if not removed:
+            logger.info("No unused '%s' cache to remove.", scheme)
+
+    if not cloud:
+        return
+
+    for remote_odb, obj_ids in odb_to_obj_ids:
+        if remote_odb is None:
+            remote_odb = repo.cloud.get_remote_odb(remote, "gc -c")
+        removed = ogc(remote_odb, obj_ids, jobs=jobs)
+        if removed:
+            get_index(remote_odb).clear()
+        else:
+            logger.info("No unused cache to remove from remote.")
```

### Comparing `dvc-3.0.0a2/dvc/repo/get.py` & `dvc-3.1.0/dvc/repo/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/get_url.py` & `dvc-3.1.0/dvc/repo/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/graph.py` & `dvc-3.1.0/dvc/repo/graph.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/imp_url.py` & `dvc-3.1.0/dvc/repo/imp_url.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 @locked
 @scm_context
 def imp_url(  # noqa: C901, PLR0913
     self: "Repo",
     url,
     out=None,
-    fname=None,
     erepo=None,
     frozen=True,
     no_download=False,
     no_exec=False,
     remote=None,
     to_remote=False,
     jobs=None,
@@ -54,15 +53,15 @@
         if fs_config is None:
             fs_config = {}
         fs_config["version_aware"] = True
 
     stage = self.stage.create(
         single_stage=True,
         validate=False,
-        fname=fname or path,
+        fname=path,
         wdir=wdir,
         deps=[url],
         outs=[out],
         erepo=erepo,
         fs_config=fs_config,
     )
```

### Comparing `dvc-3.0.0a2/dvc/repo/imports.py` & `dvc-3.1.0/dvc/repo/imports.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+from functools import partial
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, List, Set, Tuple, Union
 
 if TYPE_CHECKING:
     from dvc.dependency.base import Dependency
     from dvc.repo import Repo
     from dvc.repo.index import Index, IndexView
@@ -13,41 +14,51 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 def unfetched_view(
     index: "Index", targets: "TargetType", unpartial: bool = False, **kwargs
-) -> Tuple["IndexView", List["Dependency"]]:
+) -> Tuple["IndexView", "IndexView", List["Dependency"]]:
     """Return index view of imports which have not been fetched.
 
     Returns:
-        Tuple in the form (view, changed_deps) where changed_imports is a list
-        of import dependencies that cannot be fetched due to changed data
-        source.
+        Tuple in the form (legacy_view, view, changed_deps) where changed_imports is a
+        list of import dependencies that cannot be fetched due to changed data source.
     """
+    from dvc.cachemgr import LEGACY_HASH_NAMES
+
     changed_deps: List["Dependency"] = []
 
-    def need_fetch(stage: "Stage") -> bool:
+    def need_fetch(stage: "Stage", legacy: bool = False) -> bool:
         if not stage.is_import or (stage.is_partial_import and not unpartial):
             return False
 
         out = stage.outs[0]
         if not out.changed_cache():
             return False
 
         dep = stage.deps[0]
         if dep.changed_checksum():
             changed_deps.append(dep)
             return False
 
-        return True
+        if out.hash_name in LEGACY_HASH_NAMES and legacy:
+            return True
+        if out.hash_name not in LEGACY_HASH_NAMES and not legacy:
+            return True
+        return False
 
+    legacy_unfetched = index.targets_view(
+        targets,
+        stage_filter=partial(need_fetch, legacy=True),
+        **kwargs,
+    )
     unfetched = index.targets_view(targets, stage_filter=need_fetch, **kwargs)
-    return unfetched, changed_deps
+    return legacy_unfetched, unfetched, changed_deps
 
 
 def partial_view(index: "Index", targets: "TargetType", **kwargs) -> "IndexView":
     return index.targets_view(
         targets,
         stage_filter=lambda s: s.is_partial_import,
         **kwargs,
@@ -85,44 +96,49 @@
 
     Imports which are already cached will not be downloaded.
 
     Returns:
         Objects which were downloaded from source location.
     """
     from dvc.stage.exceptions import DataSourceChanged
-    from dvc_data.index import checkout, md5, save
+    from dvc_data.index import md5, save
+    from dvc_data.index.checkout import apply, compare
     from dvc_objects.fs.callbacks import Callback
 
     downloaded: Set["HashInfo"] = set()
 
-    unfetched, changed = unfetched_view(
+    legacy_unfetched, unfetched, changed = unfetched_view(
         repo.index, targets, unpartial=unpartial, **kwargs
     )
     for dep in changed:
         logger.warning(str(DataSourceChanged(f"{dep.stage} ({dep})")))
 
-    data_view = unfetched.data["repo"]
-    if len(data_view):
-        cache = repo.cache.local
-        if not cache.fs.exists(cache.path):
-            os.makedirs(cache.path)
-        with TemporaryDirectory(dir=cache.path) as tmpdir:
-            with Callback.as_tqdm_callback(
-                desc="Downloading imports from source",
-                unit="files",
-            ) as cb:
-                checkout(data_view, tmpdir, cache.fs, callback=cb, storage="remote")
-            md5(data_view)
-            save(data_view, odb=cache, hardlink=True)
-
-        downloaded.update(
-            entry.hash_info
-            for _, entry in data_view.iteritems()
-            if entry.meta is not None
-            and not entry.meta.isdir
-            and entry.hash_info is not None
-        )
+    for view, cache in [
+        (legacy_unfetched, repo.cache.legacy),
+        (unfetched, repo.cache.local),
+    ]:
+        data_view = view.data["repo"]
+        if len(data_view):
+            if not cache.fs.exists(cache.path):
+                os.makedirs(cache.path)
+            with TemporaryDirectory(dir=cache.path) as tmpdir:
+                with Callback.as_tqdm_callback(
+                    desc="Downloading imports from source",
+                    unit="files",
+                ) as cb:
+                    diff = compare(None, data_view)
+                    apply(diff, tmpdir, cache.fs, callback=cb, storage="remote")
+                md5(data_view, name=cache.hash_name)
+                save(data_view, odb=cache, hardlink=True)
+
+            downloaded.update(
+                entry.hash_info
+                for _, entry in data_view.iteritems()
+                if entry.meta is not None
+                and not entry.meta.isdir
+                and entry.hash_info is not None
+            )
 
     if unpartial:
         unpartial_imports(partial_view(repo.index, targets, **kwargs))
 
     return downloaded
```

### Comparing `dvc-3.0.0a2/dvc/repo/index.py` & `dvc-3.1.0/dvc/repo/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,28 +132,33 @@
             meta=out.meta,
             hash_info=out.hash_info,
         )
 
         if out.stage.is_import and not out.stage.is_repo_import:
             dep = out.stage.deps[0]
             entry.meta = dep.meta
-            entry.hash_info = dep.hash_info
+            if out.hash_info:
+                entry.hash_info = out.hash_info
+            else:
+                # partial import
+                entry.hash_info = dep.hash_info
 
         # FIXME PyGTrie-based DataIndex doesn't remove entry.key during
         # index.add, so we have to set the entry manually here to make
         # index.view() work correctly.
         index[(*prefix, ws, *key)] = entry
 
     for ws, key in parents:
         index[(*prefix, ws, *key)] = DataIndexEntry(
             key=key, meta=Meta(isdir=True), loaded=True
         )
 
 
 def _load_storage_from_out(storage_map, key, out):
+    from dvc.cachemgr import LEGACY_HASH_NAMES
     from dvc.config import NoRemoteError
     from dvc_data.index import FileStorage, ObjectStorage
 
     if out.odb:
         storage_map.add_data(ObjectStorage(key, out.odb))
     storage_map.add_cache(ObjectStorage(key, out.cache))
     try:
@@ -164,20 +169,36 @@
                     key=key,
                     fs=remote.fs,
                     path=remote.fs.path.join(remote.path, *key),
                     index=remote.index,
                 )
             )
         else:
-            storage_map.add_remote(ObjectStorage(key, remote.odb, index=remote.index))
+            odb = (
+                remote.legacy_odb if out.hash_name in LEGACY_HASH_NAMES else remote.odb
+            )
+            storage_map.add_remote(ObjectStorage(key, odb, index=remote.index))
     except NoRemoteError:
         pass
 
     if out.stage.is_import:
         dep = out.stage.deps[0]
+        if not out.hash_info:
+            from fsspec.utils import tokenize
+
+            # partial import
+            storage_map.add_cache(
+                FileStorage(
+                    key,
+                    out.cache.fs,
+                    out.cache.fs.path.join(
+                        out.cache.path, "fs", dep.fs.protocol, tokenize(dep.fs_path)
+                    ),
+                )
+            )
         storage_map.add_remote(FileStorage(key, dep.fs, dep.fs_path))
 
 
 class Index:
     def __init__(
         self,
         repo: "Repo",
@@ -570,14 +591,31 @@
             if filter_info and out.fs.path.isin(filter_info, out.fs_path):
                 key = key + out.fs.path.relparts(filter_info, out.fs_path)
             ret[workspace].add(key)
 
         return dict(ret)
 
     @cached_property
+    def data_tree(self):
+        from dvc_data.hashfile.tree import Tree
+
+        tree = Tree()
+        for out in self.outs:
+            if not out.use_cache:
+                continue
+
+            ws, key = out.index_key
+
+            tree.add((ws, *key), out.meta, out.hash_info)
+
+        tree.digest()
+
+        return tree
+
+    @cached_property
     def data(self) -> Dict[str, Union["DataIndex", "DataIndexView"]]:
         from dvc_data.index import DataIndex, view
 
         def key_filter(workspace: str, key: "DataIndexKey"):
             try:
                 prefixes = self._data_prefixes[workspace]
                 return key in prefixes.explicit or any(
@@ -618,49 +656,52 @@
 
         for key_len in range(1, len(key)):
             parents.add(key[:key_len])
 
         if not fs.exists(out_path):
             continue
 
+        hash_name = _get_entry_hash_name(index, workspace, key)
         try:
             out_entry = build_entry(
                 out_path,
                 fs,
                 compute_hash=compute_hash,
                 state=index.repo.state,
+                hash_name=hash_name,
             )
         except FileNotFoundError:
-            continue
+            out_entry = DataIndexEntry()
 
         out_entry.key = key
         data.add(out_entry)
         callback.relative_update(1)
 
         if not out_entry.meta or not out_entry.meta.isdir:
             continue
 
         for entry in build_entries(
             out_path,
             fs,
             compute_hash=compute_hash,
             state=index.repo.state,
             ignore=ignore,
+            hash_name=hash_name,
         ):
             if not entry.key or entry.key == ("",):
                 # NOTE: whether the root will be returned by build_entries
                 # depends on the filesystem (e.g. local doesn't, but s3 does).
                 continue
 
             entry.key = key + entry.key
             data.add(entry)
             callback.relative_update(1)
 
         if compute_hash:
-            tree_meta, tree = build_tree(data, key)
+            tree_meta, tree = build_tree(data, key, name=hash_name)
             out_entry.meta = tree_meta
             out_entry.hash_info = tree.hash_info
             out_entry.loaded = True
             data.add(out_entry)
             callback.relative_update(1)
 
     for key in parents:
@@ -668,7 +709,21 @@
         if not fs.exists(parent_path):
             continue
         direntry = DataIndexEntry(key=key, meta=Meta(isdir=True), loaded=True)
         data.add(direntry)
         callback.relative_update(1)
 
     return data
+
+
+def _get_entry_hash_name(
+    index: Union["Index", "IndexView"], workspace: str, key: "DataIndexKey"
+) -> str:
+    from dvc_data.hashfile.hash import DEFAULT_ALGORITHM
+
+    try:
+        src_entry = index.data[workspace][key]
+        if src_entry.hash_info and src_entry.hash_info.name:
+            return src_entry.hash_info.name
+    except KeyError:
+        pass
+    return DEFAULT_ALGORITHM
```

### Comparing `dvc-3.0.0a2/dvc/repo/init.py` & `dvc-3.1.0/dvc/repo/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/install.py` & `dvc-3.1.0/dvc/repo/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/ls.py` & `dvc-3.1.0/dvc/repo/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/ls_url.py` & `dvc-3.1.0/dvc/repo/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/metrics/diff.py` & `dvc-3.1.0/dvc/repo/metrics/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/metrics/show.py` & `dvc-3.1.0/dvc/repo/metrics/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/move.py` & `dvc-3.1.0/dvc/repo/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/open_repo.py` & `dvc-3.1.0/dvc/repo/open_repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         name = repo.config["core"].get("remote")
         if not name:
             # Fill the empty upstream entry with a new remote pointing to the
             # original repo's cache location.
             name = "auto-generated-upstream"
             return {
                 "core": {"remote": name},
-                "remote": {name: {"url": repo.cache.local.path}},
+                "remote": {name: {"url": repo.cache.local_cache_dir}},
             }
 
         # Use original remote to make sure that we are using correct url,
         # credential paths, etc if they are relative to the config location.
         return {"remote": {name: repo.config["remote"][name]}}
     finally:
         repo.close()
```

### Comparing `dvc-3.0.0a2/dvc/repo/params/diff.py` & `dvc-3.1.0/dvc/repo/params/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/params/show.py` & `dvc-3.1.0/dvc/repo/params/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/plots/__init__.py` & `dvc-3.1.0/dvc/repo/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/plots/diff.py` & `dvc-3.1.0/dvc/repo/plots/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/pull.py` & `dvc-3.1.0/dvc/repo/pull.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import logging
-from typing import TYPE_CHECKING, Optional
 
 from dvc.repo import locked
 from dvc.utils import glob_targets
 
-if TYPE_CHECKING:
-    from dvc_objects.db import ObjectDB
-
 logger = logging.getLogger(__name__)
 
 
 @locked
 def pull(  # noqa: PLR0913
     self,
     targets=None,
@@ -20,15 +16,14 @@
     with_deps=False,
     all_tags=False,
     force=False,
     recursive=False,
     all_commits=False,
     run_cache=False,
     glob=False,
-    odb: Optional["ObjectDB"] = None,
     allow_missing=False,
 ):
     if isinstance(targets, str):
         targets = [targets]
 
     expanded_targets = glob_targets(targets, glob=glob)
 
@@ -38,15 +33,14 @@
         remote=remote,
         all_branches=all_branches,
         all_tags=all_tags,
         all_commits=all_commits,
         with_deps=with_deps,
         recursive=recursive,
         run_cache=run_cache,
-        odb=odb,
     )
     stats = self.checkout(
         targets=expanded_targets,
         with_deps=with_deps,
         force=force,
         recursive=recursive,
         allow_missing=allow_missing,
```

### Comparing `dvc-3.0.0a2/dvc/repo/push.py` & `dvc-3.1.0/dvc/repo/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/remove.py` & `dvc-3.1.0/dvc/repo/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/reproduce.py` & `dvc-3.1.0/dvc/repo/reproduce.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,24 +159,25 @@
                  A                                       E
 
     The derived evaluation of _downstream_ B would be: [B, D, E]
     """
     steps = _get_steps(graph, stages, downstream, single_item)
 
     force_downstream = kwargs.pop("force_downstream", False)
-    result = []
+    result: List["Stage"] = []
     unchanged: List["Stage"] = []
     # `ret` is used to add a cosmetic newline.
     ret: List["Stage"] = []
 
     for stage in steps:
         if ret:
             logger.info("")
 
         try:
+            kwargs["upstream"] = result + unchanged
             ret = _reproduce_stage(stage, **kwargs)
 
             if len(ret) == 0:
                 unchanged.extend([stage])
             elif force_downstream:
                 # NOTE: we are walking our pipeline from the top to the
                 # bottom. If one stage is changed, it will be reproduced,
```

### Comparing `dvc-3.0.0a2/dvc/repo/run.py` & `dvc-3.1.0/dvc/repo/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/scm_context.py` & `dvc-3.1.0/dvc/repo/scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/stage.py` & `dvc-3.1.0/dvc/repo/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/status.py` & `dvc-3.1.0/dvc/repo/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/trie.py` & `dvc-3.1.0/dvc/repo/trie.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/update.py` & `dvc-3.1.0/dvc/repo/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/repo/worktree.py` & `dvc-3.1.0/dvc/repo/worktree.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,50 +100,23 @@
     repo: "Repo", name: Optional[str], default: "Remote", command: str
 ) -> "Remote":
     if name in (None, default.name):
         return default
     return repo.cloud.get_remote(name, command)
 
 
-def fetch_worktree(
-    repo: "Repo",
-    remote: "Remote",
-    targets: Optional["TargetType"] = None,
-    jobs: Optional[int] = None,
-    **kwargs: Any,
-) -> int:
-    from dvc_data.index import save
-
-    transferred = 0
-    for remote_name, view in worktree_view_by_remotes(
-        repo.index, push=True, targets=targets, **kwargs
-    ):
-        remote_obj = _get_remote(repo, remote_name, remote, "fetch")
-        index = view.data["repo"]
-        total = len(index)
-        with Callback.as_tqdm_callback(
-            unit="file",
-            desc=f"Fetching from remote {remote_obj.name!r}",
-            disable=total == 0,
-        ) as cb:
-            cb.set_size(total)
-            transferred += save(index, callback=cb, jobs=jobs, storage="remote")
-    return transferred
-
-
 def push_worktree(
     repo: "Repo",
     remote: "Remote",
     targets: Optional["TargetType"] = None,
     jobs: Optional[int] = None,
     **kwargs: Any,
 ) -> int:
     from dvc.repo.index import build_data_index
-    from dvc_data.index import checkout
-    from dvc_data.index.checkout import VersioningNotSupported
+    from dvc_data.index.checkout import VersioningNotSupported, apply, compare
 
     pushed = 0
     stages: Set["Stage"] = set()
 
     for remote_name, view in worktree_view_by_remotes(
         repo.index, push=True, targets=targets, **kwargs
     ):
@@ -161,32 +134,41 @@
             diff_kwargs: Dict[str, Any] = {
                 "meta_only": True,
                 "meta_cmp_key": partial(_meta_checksum, remote_obj.fs),
             }
         else:
             diff_kwargs = {}
 
+        with Callback.as_tqdm_callback(
+            unit="entry",
+            desc=f"Comparing indexes for remote {remote_obj.name!r}",
+        ) as cb:
+            diff = compare(
+                old_index,
+                new_index,
+                callback=cb,
+                delete=remote_obj.worktree,
+                **diff_kwargs,
+            )
+
         total = len(new_index)
         with Callback.as_tqdm_callback(
             unit="file",
             desc=f"Pushing to remote {remote_obj.name!r}",
             disable=total == 0,
         ) as cb:
             cb.set_size(total)
             try:
-                stats = checkout(
-                    new_index,
+                stats = apply(
+                    diff,
                     remote_obj.path,
                     remote_obj.fs,
-                    old=old_index,
-                    delete=remote_obj.worktree,
                     callback=cb,
                     latest_only=remote_obj.worktree,
                     jobs=jobs,
-                    **diff_kwargs,
                 )
                 pushed += sum(len(changes) for changes in stats.values())
             except VersioningNotSupported:
                 logger.exception("")
                 raise DvcException(
                     f"remote {remote_obj.name!r} does not support versioning"
                 ) from None
@@ -338,31 +320,41 @@
 
 def _fetch_out_changes(
     out: "Output",
     local_index: Union["DataIndex", "DataIndexView"],
     remote_index: Union["DataIndex", "DataIndexView"],
     remote: "Remote",
 ):
-    from dvc_data.index import checkout
+    from dvc_data.index.checkout import apply, compare
 
     old, new = _get_diff_indexes(out, local_index, remote_index)
+
+    with Callback.as_tqdm_callback(
+        unit="entry",
+        desc="Comparing indexes",
+    ) as cb:
+        diff = compare(
+            old,
+            new,
+            delete=True,
+            meta_only=True,
+            meta_cmp_key=partial(_meta_checksum, remote.fs),
+            callback=cb,
+        )
+
     total = len(new)
     with Callback.as_tqdm_callback(
         unit="file", desc=f"Updating '{out}'", disable=total == 0
     ) as cb:
         cb.set_size(total)
-        checkout(
-            new,
+        apply(
+            diff,
             out.repo.root_dir,
             out.fs,
-            old=old,
-            delete=True,
             update_meta=False,
-            meta_only=True,
-            meta_cmp_key=partial(_meta_checksum, remote.fs),
             storage="data",
             callback=cb,
         )
         out.save()
 
 
 def _get_diff_indexes(
```

### Comparing `dvc-3.0.0a2/dvc/rwlock.py` & `dvc-3.1.0/dvc/rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/schema.py` & `dvc-3.1.0/dvc/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 DATA_SCHEMA = {
     **CHECKSUMS_SCHEMA,
     **META_SCHEMA,
     Required("path"): str,
     Output.PARAM_CLOUD: CLOUD_SCHEMA,
     Output.PARAM_FILES: [DIR_FILES_SCHEMA],
+    Output.PARAM_HASH: str,
 }
 LOCK_FILE_STAGE_SCHEMA = {
     Required(StageParams.PARAM_CMD): Any(str, list),
     StageParams.PARAM_DEPS: [DATA_SCHEMA],
     StageParams.PARAM_PARAMS: {str: {str: object}},
     StageParams.PARAM_OUTS: [DATA_SCHEMA],
 }
```

### Comparing `dvc-3.0.0a2/dvc/scm.py` & `dvc-3.1.0/dvc/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/stage/__init__.py` & `dvc-3.1.0/dvc/stage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,28 +85,27 @@
 
 @dataclass
 class RawData:
     parametrized: bool = False
     generated_from: Optional[str] = None
 
 
-def create_stage(cls: Type[_T], repo, path, external=False, **kwargs) -> _T:
+def create_stage(cls: Type[_T], repo, path, **kwargs) -> _T:
     from dvc.dvcfile import check_dvcfile_path
 
     wdir = os.path.abspath(kwargs.get("wdir", None) or os.curdir)
     path = os.path.abspath(path)
 
     check_dvcfile_path(repo, path)
     check_stage_path(repo, wdir, is_wdir=kwargs.get("wdir"))
     check_stage_path(repo, os.path.dirname(path))
 
     stage = loads_from(cls, repo, path, wdir, kwargs)
     fill_stage_outputs(stage, **kwargs)
-    if not external:
-        check_no_externals(stage)
+    check_no_externals(stage)
     fill_stage_dependencies(
         stage, **project(kwargs, ["deps", "erepo", "params", "fs_config"])
     )
     check_circular_dependency(stage)
     check_duplicated_arguments(stage)
 
     return stage
@@ -291,30 +290,41 @@
 
         env: Env = {}
         if self.repo:
             env.update({DVC_ROOT: self.repo.root_dir})
 
         return env
 
-    def changed_deps(self, allow_missing: bool = False) -> bool:
+    def changed_deps(
+        self, allow_missing: bool = False, upstream: Optional[List] = None
+    ) -> bool:
         if self.frozen:
             return False
 
         if self.is_callback or self.always_changed:
             return True
 
-        return self._changed_deps(allow_missing=allow_missing)
+        return self._changed_deps(allow_missing=allow_missing, upstream=upstream)
 
     @rwlocked(read=["deps"])
-    def _changed_deps(self, allow_missing: bool = False) -> bool:
+    def _changed_deps(
+        self, allow_missing: bool = False, upstream: Optional[List] = None
+    ) -> bool:
         for dep in self.deps:
             status = dep.status()
             if status:
                 if allow_missing and status[str(dep)] == "deleted":
-                    continue
+                    if upstream and any(
+                        dep.fs_path == out.fs_path and dep.hash_info != out.hash_info
+                        for stage in upstream
+                        for out in stage.outs
+                    ):
+                        status[str(dep)] = "modified"
+                    else:
+                        continue
                 logger.debug(
                     "Dependency '%s' of %s changed because it is '%s'.",
                     dep,
                     self,
                     status[str(dep)],
                 )
                 return True
@@ -340,20 +350,22 @@
     def changed_stage(self) -> bool:
         changed = self.md5 != self.compute_md5()
         if changed:
             logger.debug(self._changed_stage_entry())
         return changed
 
     @rwlocked(read=["deps", "outs"])
-    def changed(self, allow_missing: bool = False) -> bool:
+    def changed(
+        self, allow_missing: bool = False, upstream: Optional[List] = None
+    ) -> bool:
         is_changed = (
             # Short-circuit order: stage md5 is fast,
             # deps are expected to change
             self.changed_stage()
-            or self.changed_deps(allow_missing=allow_missing)
+            or self.changed_deps(allow_missing=allow_missing, upstream=upstream)
             or self.changed_outs(allow_missing=allow_missing)
         )
         if is_changed:
             logger.debug("%s changed.", self)
         return is_changed
 
     @rwlocked(write=["outs"])
@@ -400,15 +412,17 @@
             out.checkout(force=force)
             out.ignore()
 
     @rwlocked(read=["deps"], write=["outs"])
     def reproduce(self, interactive=False, **kwargs) -> Optional["Stage"]:
         if not (
             kwargs.get("force", False)
-            or self.changed(kwargs.get("allow_missing", False))
+            or self.changed(
+                kwargs.get("allow_missing", False), kwargs.pop("upstream", None)
+            )
         ):
             if not isinstance(self, PipelineStage) and self.is_data_source:
                 logger.info("'%s' didn't change, skipping", self.addressing)
             else:
                 logger.info("Stage '%s' didn't change, skipping", self.addressing)
             return None
```

### Comparing `dvc-3.0.0a2/dvc/stage/cache.py` & `dvc-3.1.0/dvc/stage/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,20 @@
         return False
 
     for dep in stage.deps:
         if not (dep.protocol == "local" and dep.def_path and dep.get_hash()):
             return False
 
     for out in stage.outs:
-        if out.protocol != "local" or not out.def_path or out.persist:
+        if (
+            out.protocol != "local"
+            or not out.def_path
+            or out.persist
+            or not out.is_in_repo
+        ):
             return False
 
     return True
 
 
 def _get_stage_hash(stage):
     from .serialize import to_single_stage_lockfile
@@ -56,15 +61,15 @@
     assert _can_hash(stage)
     return _get_cache_hash(to_single_stage_lockfile(stage), key=True)
 
 
 class StageCache:
     def __init__(self, repo):
         self.repo = repo
-        self.cache_dir = os.path.join(self.repo.cache.local.path, "runs")
+        self.cache_dir = os.path.join(self.repo.cache.legacy.path, "runs")
 
     def _get_cache_dir(self, key):
         return os.path.join(self.cache_dir, key[:2], key)
 
     def _get_cache_path(self, key, value):
         return os.path.join(self._get_cache_dir(key), value)
 
@@ -108,40 +113,39 @@
         stage = create_stage(
             PipelineStage,
             repo=self.repo,
             path="dvc.yaml",
             cmd=cache["cmd"],
             wdir=wdir,
             outs=[out["path"] for out in cache["outs"]],
-            external=True,
         )
         StageLoader.fill_from_lock(stage, cache)
         return stage
 
     @contextmanager
     def _cache_type_copy(self):
-        cache_types = self.repo.cache.local.cache_types
-        self.repo.cache.local.cache_types = ["copy"]
+        cache_types = self.repo.cache.legacy.cache_types
+        self.repo.cache.legacy.cache_types = ["copy"]
         try:
             yield
         finally:
-            self.repo.cache.local.cache_types = cache_types
+            self.repo.cache.legacy.cache_types = cache_types
 
     def _uncached_outs(self, stage, cache):
         # NOTE: using temporary stage to avoid accidentally modifying original
         # stage and to workaround `commit/checkout` not working for uncached
         # outputs.
         cached_stage = self._create_stage(cache, wdir=stage.wdir)
 
         outs_no_cache = [out.def_path for out in stage.outs if not out.use_cache]
 
         # NOTE: using copy link to make it look like a git-tracked file
         with self._cache_type_copy():
             for out in cached_stage.outs:
-                if out.def_path in outs_no_cache:
+                if out.def_path in outs_no_cache and out.is_in_repo:
                     yield out
 
     def save(self, stage):
         from .serialize import to_single_stage_lockfile
 
         if not _can_hash(stage):
             return
@@ -162,22 +166,22 @@
         from dvc.schema import COMPILED_LOCK_FILE_STAGE_SCHEMA
         from dvc.utils.serialize import dump_yaml
 
         # sanity check
         COMPILED_LOCK_FILE_STAGE_SCHEMA(cache)
 
         path = self._get_cache_path(cache_key, cache_value)
-        local_fs = self.repo.cache.local.fs
+        local_fs = self.repo.cache.legacy.fs
         parent = local_fs.path.parent(path)
-        self.repo.cache.local.makedirs(parent)
+        self.repo.cache.legacy.makedirs(parent)
         tmp = local_fs.path.join(parent, fs.utils.tmp_fname())
         assert os.path.exists(parent)
         assert os.path.isdir(parent)
         dump_yaml(tmp, cache)
-        self.repo.cache.local.move(tmp, path)
+        self.repo.cache.legacy.move(tmp, path)
 
     def restore(self, stage, run_cache=True, pull=False, dry=False):
         from .serialize import to_single_stage_lockfile
 
         if not _can_hash(stage):
             raise RunCacheNotFoundError(stage)
 
@@ -254,20 +258,24 @@
                 bytes=True,
             ) as cb:
                 func(from_fs, src, to_fs, dst, callback=cb)
             ret.append((parent_name, src_name))
         return ret
 
     def push(self, remote: Optional[str], odb: Optional["ObjectDB"] = None):
-        dest_odb = odb or self.repo.cloud.get_remote_odb(remote, "push --run-cache")
-        return self.transfer(self.repo.cache.local, dest_odb)
+        dest_odb = odb or self.repo.cloud.get_remote_odb(
+            remote, "push --run-cache", hash_name="md5-dos2unix"
+        )
+        return self.transfer(self.repo.cache.legacy, dest_odb)
 
     def pull(self, remote: Optional[str], odb: Optional["ObjectDB"] = None):
-        odb = odb or self.repo.cloud.get_remote_odb(remote, "fetch --run-cache")
-        return self.transfer(odb, self.repo.cache.local)
+        odb = odb or self.repo.cloud.get_remote_odb(
+            remote, "fetch --run-cache", hash_name="md5-dos2unix"
+        )
+        return self.transfer(odb, self.repo.cache.legacy)
 
     def get_used_objs(self, used_run_cache, *args, **kwargs):
         """Return used cache for the specified run-cached stages."""
         from collections import defaultdict
 
         used_objs = defaultdict(set)
         for key, value in used_run_cache:
```

### Comparing `dvc-3.0.0a2/dvc/stage/decorators.py` & `dvc-3.1.0/dvc/stage/decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/stage/exceptions.py` & `dvc-3.1.0/dvc/stage/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/stage/imports.py` & `dvc-3.1.0/dvc/stage/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/stage/loader.py` & `dvc-3.1.0/dvc/stage/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Tuple
 
 from funcy import get_in, lcat, once, project
 
 from dvc import dependency, output
 from dvc.parsing import FOREACH_KWD, JOIN, EntryNotFound
 from dvc.utils.objects import cached_property
-from dvc_data.hashfile.hash_info import HashInfo
 from dvc_data.hashfile.meta import Meta
 
 from . import PipelineStage, Stage, loads_from
 from .exceptions import StageNameUnspecified, StageNotFound
 from .params import StageParams
 from .utils import fill_stage_dependencies, resolve_paths
 
 if TYPE_CHECKING:
     from dvc.dvcfile import ProjectFile, SingleStageFile
-    from dvc.output import Output
 
 logger = logging.getLogger(__name__)
 
 
 class StageLoader(Mapping):
     def __init__(
         self,
@@ -48,15 +46,15 @@
 
     @staticmethod
     def fill_from_lock(stage, lock_data=None):
         """Fill values for params, checksums for outs and deps from lock."""
         if not lock_data:
             return
 
-        from dvc.output import merge_file_meta_from_cloud
+        from dvc.output import Output, merge_file_meta_from_cloud
 
         assert isinstance(lock_data, dict)
         items: Iterable[Tuple[str, "Output"]] = chain(
             ((StageParams.PARAM_DEPS, dep) for dep in stage.deps),
             ((StageParams.PARAM_OUTS, out) for out in stage.outs),
         )
 
@@ -69,17 +67,20 @@
             if isinstance(item, dependency.ParamsDependency):
                 item.fill_values(get_in(lock_data, [stage.PARAM_PARAMS, path]))
                 continue
             info = get_in(checksums, [key, path], {})
             info = info.copy()
             info.pop("path", None)
 
+            hash_name = info.pop(Output.PARAM_HASH, None)
             item.meta = Meta.from_dict(merge_file_meta_from_cloud(info))
-            hash_value = getattr(item.meta, item.hash_name, None)
-            item.hash_info = HashInfo(item.hash_name, hash_value)
+            # pylint: disable-next=protected-access
+            item.hash_name, item.hash_info = item._compute_hash_info_from_meta(
+                hash_name
+            )
             files = get_in(checksums, [key, path, item.PARAM_FILES], None)
             if files:
                 item.files = [merge_file_meta_from_cloud(f) for f in files]
             # pylint: disable-next=protected-access
             item._compute_meta_hash_info_from_files()
 
     @classmethod
```

### Comparing `dvc-3.0.0a2/dvc/stage/run.py` & `dvc-3.1.0/dvc/stage/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/stage/serialize.py` & `dvc-3.1.0/dvc/stage/serialize.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,33 +145,40 @@
         (stage.PARAM_ALWAYS_CHANGED, stage.always_changed),
         (stage.PARAM_META, stage.meta),
     ]
     return {stage.name: OrderedDict([(key, value) for key, value in res if value])}
 
 
 def to_single_stage_lockfile(stage: "Stage", **kwargs) -> dict:
-    from dvc.output import _serialize_tree_obj_to_files, split_file_meta_from_cloud
+    from dvc.cachemgr import LEGACY_HASH_NAMES
+    from dvc.output import (
+        _serialize_hi_to_dict,
+        _serialize_tree_obj_to_files,
+        split_file_meta_from_cloud,
+    )
     from dvc_data.hashfile.tree import Tree
 
     assert stage.cmd
 
     def _dumpd(item: "Output"):
         ret: Dict[str, Any] = {item.PARAM_PATH: item.def_path}
+        if item.hash_name not in LEGACY_HASH_NAMES:
+            ret[item.PARAM_HASH] = "md5"
         if item.hash_info.isdir and kwargs.get("with_files"):
             obj = item.obj or item.get_obj()
             if obj:
                 assert isinstance(obj, Tree)
                 ret[item.PARAM_FILES] = [
                     split_file_meta_from_cloud(f)
                     for f in _serialize_tree_obj_to_files(obj)
                 ]
         else:
             meta_d = item.meta.to_dict()
             meta_d.pop("isdir", None)
-            ret.update(item.hash_info.to_dict())
+            ret.update(_serialize_hi_to_dict(item.hash_info))
             ret.update(split_file_meta_from_cloud(meta_d))
         return ret
 
     res = OrderedDict([("cmd", stage.cmd)])
     params, deps = split_params_deps(stage)
     deps, outs = (
         [_dumpd(item) for item in sorted(items, key=attrgetter("def_path"))]
```

### Comparing `dvc-3.0.0a2/dvc/stage/utils.py` & `dvc-3.1.0/dvc/stage/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,36 +83,32 @@
     assert not stage.deps
     stage.deps = []
     stage.deps += loads_from(stage, deps or [], erepo=erepo, fs_config=fs_config)
     stage.deps += loads_params(stage, params or [])
 
 
 def check_no_externals(stage):
-    from urllib.parse import urlparse
-
     from dvc.utils import format_link
 
-    # NOTE: preventing users from accidentally using external outputs. See
-    # https://github.com/iterative/dvc/issues/1545 for more details.
-
-    def _is_external(out):
-        # NOTE: in case of `remote://` notation, the user clearly knows that
-        # this is an advanced feature and so we shouldn't error-out.
-        if out.is_in_repo or urlparse(out.def_path).scheme == "remote":
+    def _is_cached_external(out):
+        if out.is_in_repo or not out.use_cache:
             return False
         return True
 
-    outs = [str(out) for out in stage.outs if _is_external(out)]
+    outs = [str(out) for out in stage.outs if _is_cached_external(out)]
     if not outs:
         return
 
     str_outs = ", ".join(outs)
-    link = format_link("https://dvc.org/doc/user-guide/managing-external-data")
+    link = format_link(
+        "https://dvc.org/doc/user-guide/pipelines/external-dependencies-and-outputs"
+    )
     raise StageExternalOutputsError(
-        f"Output(s) outside of DVC project: {str_outs}. See {link} for more info."
+        f"Cached output(s) outside of DVC project: {str_outs}. "
+        f"See {link} for more info."
     )
 
 
 def check_circular_dependency(stage):
     from dvc.exceptions import CircularDependencyError
 
     circular_dependencies = {d.fs_path for d in stage.deps} & {
```

### Comparing `dvc-3.0.0a2/dvc/testing/README.rst` & `dvc-3.1.0/dvc/testing/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/api_tests.py` & `dvc-3.1.0/dvc/testing/api_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 # pylint: disable=unused-argument
 
 
 class TestAPI:
     def test_get_url(self, tmp_dir, dvc, remote):
         tmp_dir.dvc_gen("foo", "foo")
 
-        expected_url = (remote / "ac/bd18db4cc2f85cedef654fccc4a4d8").url
+        expected_url = (
+            remote / "files" / "md5" / "ac/bd18db4cc2f85cedef654fccc4a4d8"
+        ).url
         assert api.get_url("foo") == expected_url
 
     def test_open(self, tmp_dir, dvc, remote):
         tmp_dir.dvc_gen(
             {
                 "foo": "foo-text",
                 "dir": {"bar": "bar-text"},
```

### Comparing `dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_checkout.py` & `dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_data_status.py` & `dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_plots.py` & `dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/test_modify_data.py` & `dvc-3.1.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     # Move some files to create a partial dataset
     os.makedirs("partial-copy")
     for f in glob.glob("*", root_dir=dataset, recursive=True):  # type: ignore[call-arg]
         if random.random() > 0.5:  # noqa: S311 # nosec
             shutil.move(dataset / f, tmp_dir / "partial-copy" / f)
 
     # Add/push partial dataset
-    dvc.add(str(dataset))
-    dvc.push()
+    bench_dvc("add", dataset)
+    bench_dvc("push")
 
     # Add more files to the dataset
     shutil.copytree("partial-copy", dataset, dirs_exist_ok=True)
 
     # Benchmark operations for adding files to a dataset
     bench_dvc("add", dataset, name="partial-add")
     bench_dvc("push", name="partial-add")
@@ -35,16 +35,16 @@
     bench_dvc("gc", "-f", "-w", "-c", name="cloud-noop")
 
 
 @pytest.mark.skipif(sys.version_info < (3, 10), reason="requires 3.10 glob.glob")
 def test_partial_remove(bench_dvc, tmp_dir, dvc, dataset, remote):
     random.seed(5232)
     # Add/push full dataset
-    dvc.add(str(dataset))
-    dvc.push()
+    bench_dvc("add", dataset)
+    bench_dvc("push")
 
     # Remove some files
     for f in glob.glob("*", root_dir=dataset, recursive=True):  # type: ignore[call-arg]
         if random.random() > 0.5:  # noqa: S311 # nosec
             if os.path.isfile(dataset / f):
                 os.remove(dataset / f)
             elif os.path.isdir(dataset / f):
```

### Comparing `dvc-3.0.0a2/dvc/testing/benchmarks/fixtures.py` & `dvc-3.1.0/dvc/testing/benchmarks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/benchmarks/plugin.py` & `dvc-3.1.0/dvc/testing/benchmarks/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/cloud.py` & `dvc-3.1.0/dvc/testing/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/fixtures.py` & `dvc-3.1.0/dvc/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/path_info.py` & `dvc-3.1.0/dvc/testing/path_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/plugin.py` & `dvc-3.1.0/dvc/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/remote_tests.py` & `dvc-3.1.0/dvc/testing/remote_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/tmp_dir.py` & `dvc-3.1.0/dvc/testing/tmp_dir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/testing/workspace_tests.py` & `dvc-3.1.0/dvc/testing/workspace_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,21 @@
             assert (tmp_dir / "dir.dvc").read_text() == (
                 f"md5: {stage_md5}\n"
                 "frozen: true\n"
                 "deps:\n"
                 f"- md5: {dir_md5}\n"
                 "  size: 11\n"
                 "  nfiles: 2\n"
+                "  hash: md5\n"
                 "  path: remote://workspace/dir\n"
                 "outs:\n"
                 "- md5: b6dcab6ccd17ca0a8bf4a215a37d14cc.dir\n"
                 "  size: 11\n"
                 "  nfiles: 2\n"
+                "  hash: md5\n"
                 "  path: dir\n"
             )
 
     @pytest.fixture
     def is_object_storage(self):
         pytest.skip()
 
@@ -144,59 +146,18 @@
         remote_version_aware.gen({"data_dir": {"subdir": {"file": "file"}}})
         dvc.imp_url("remote://upstream/data_dir", version_aware=True, no_download=True)
         stage = first(dvc.index.stages)
         assert not stage.outs[0].can_push
 
         dvc.pull()
         assert (tmp_dir / "data_dir" / "subdir" / "file").read_text() == "file"
-        assert dvc.status() == {}
-
-
-class TestAdd:
-    @pytest.fixture
-    def hash_name(self):
-        pytest.skip()
-
-    @pytest.fixture
-    def hash_value(self):
-        pytest.skip()
-
-    @pytest.fixture
-    def dir_hash_value(self):
-        pytest.skip()
-
-    def test_add(self, tmp_dir, dvc, workspace, hash_name, hash_value):
-        from dvc.stage.exceptions import StageExternalOutputsError
-
-        workspace.gen("file", "file")
-
-        with pytest.raises(StageExternalOutputsError):
-            dvc.add(workspace.url)
-
-        dvc.add("remote://workspace/file")
-        assert (tmp_dir / "file.dvc").read_text() == (
-            "outs:\n"
-            f"- {hash_name}: {hash_value}\n"
-            "  size: 4\n"
-            "  path: remote://workspace/file\n"
-        )
-        assert (workspace / "file").read_text() == "file"
-        assert (
-            workspace / "cache" / hash_value[:2] / hash_value[2:]
-        ).read_text() == "file"
 
+        dvc.commit(force=True)
         assert dvc.status() == {}
 
-    # pylint: disable-next=unused-argument
-    def test_add_dir(self, tmp_dir, dvc, workspace, hash_name, dir_hash_value):
-        workspace.gen({"dir": {"file": "file", "subdir": {"subfile": "subfile"}}})
-
-        dvc.add("remote://workspace/dir")
-        assert (workspace / "cache" / dir_hash_value[:2] / dir_hash_value[2:]).is_file()
-
 
 def match_files(fs, entries, expected):
     entries_content = {(fs.path.normpath(d["path"]), d["isdir"]) for d in entries}
     expected_content = {(fs.path.normpath(d["path"]), d["isdir"]) for d in expected}
     assert entries_content == expected_content
 
 
@@ -297,15 +258,17 @@
         assert len(stage.deps) == 0
         assert len(stage.outs) == 1
 
         hash_info = stage.outs[0].hash_info
         meta = stage.outs[0].meta
         assert hash_info.name == "md5"
         assert hash_info.value == "acbd18db4cc2f85cedef654fccc4a4d8"
-        assert (remote / "ac" / "bd18db4cc2f85cedef654fccc4a4d8").read_text() == "foo"
+        assert (
+            remote / "files" / "md5" / "ac" / "bd18db4cc2f85cedef654fccc4a4d8"
+        ).read_text() == "foo"
         assert meta.size == len("foo")
 
     def test_import_url_to_remote_file(self, tmp_dir, dvc, workspace, remote):
         workspace.gen("foo", "foo")
 
         url = "remote://workspace/foo"
         stage = dvc.imp_url(url, to_remote=True)
@@ -317,15 +280,17 @@
         assert len(stage.deps) == 1
         assert stage.deps[0].def_path == url
         assert len(stage.outs) == 1
 
         hash_info = stage.outs[0].hash_info
         assert hash_info.name == "md5"
         assert hash_info.value == "acbd18db4cc2f85cedef654fccc4a4d8"
-        assert (remote / "ac" / "bd18db4cc2f85cedef654fccc4a4d8").read_text() == "foo"
+        assert (
+            remote / "files" / "md5" / "ac" / "bd18db4cc2f85cedef654fccc4a4d8"
+        ).read_text() == "foo"
         assert stage.outs[0].meta.size == len("foo")
 
     def test_import_url_to_remote_dir(self, tmp_dir, dvc, workspace, remote):
         import json
 
         workspace.gen(
             {
@@ -347,20 +312,24 @@
         assert stage.deps[0].def_path == url
         assert len(stage.outs) == 1
 
         hash_info = stage.outs[0].hash_info
         assert hash_info.name == "md5"
         assert hash_info.value == "55d05978954d1b2cd7b06aedda9b9e43.dir"
         file_parts = json.loads(
-            (remote / "55" / "d05978954d1b2cd7b06aedda9b9e43.dir").read_text()
+            (
+                remote / "files" / "md5" / "55" / "d05978954d1b2cd7b06aedda9b9e43.dir"
+            ).read_text()
         )
 
         assert len(file_parts) == 3
         assert {file_part["relpath"] for file_part in file_parts} == {
             "foo",
             "bar",
             "sub_dir/baz",
         }
 
         for file_part in file_parts:
             md5 = file_part["md5"]
-            assert (remote / md5[:2] / md5[2:]).read_text() == file_part["relpath"]
+            assert (
+                remote / "files" / "md5" / md5[:2] / md5[2:]
+            ).read_text() == file_part["relpath"]
```

### Comparing `dvc-3.0.0a2/dvc/ui/__init__.py` & `dvc-3.1.0/dvc/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/ui/_rich_progress.py` & `dvc-3.1.0/dvc/ui/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/ui/pager.py` & `dvc-3.1.0/dvc/ui/pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/ui/table.py` & `dvc-3.1.0/dvc/ui/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/updater.py` & `dvc-3.1.0/dvc/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import os
 import sys
 import time
 from typing import TYPE_CHECKING, Optional
 
 from packaging import version
 
-from dvc import __version__
-from dvc.utils.pkg import PKG
+from dvc import PKG, __version__
 
 if TYPE_CHECKING:
     from dvc.ui import RichText
 
 logger = logging.getLogger(__name__)
```

### Comparing `dvc-3.0.0a2/dvc/utils/__init__.py` & `dvc-3.1.0/dvc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/cli_parse.py` & `dvc-3.1.0/dvc/utils/cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/collections.py` & `dvc-3.1.0/dvc/utils/collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/diff.py` & `dvc-3.1.0/dvc/utils/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/fs.py` & `dvc-3.1.0/dvc/utils/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/humanize.py` & `dvc-3.1.0/dvc/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/hydra.py` & `dvc-3.1.0/dvc/utils/hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/serialize/__init__.py` & `dvc-3.1.0/dvc/utils/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/serialize/_common.py` & `dvc-3.1.0/dvc/utils/serialize/_common.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/serialize/_json.py` & `dvc-3.1.0/dvc/utils/serialize/_json.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/serialize/_py.py` & `dvc-3.1.0/dvc/utils/serialize/_py.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/serialize/_toml.py` & `dvc-3.1.0/dvc/utils/serialize/_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/serialize/_yaml.py` & `dvc-3.1.0/dvc/utils/serialize/_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/strictyaml.py` & `dvc-3.1.0/dvc/utils/strictyaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/studio.py` & `dvc-3.1.0/dvc/utils/studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/table.py` & `dvc-3.1.0/dvc/utils/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc/utils/threadpool.py` & `dvc-3.1.0/dvc/utils/threadpool.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/dvc.egg-info/PKG-INFO` & `dvc-3.1.0/dvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.0.0a2
+Version: 3.1.0
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.0.0a2/dvc.egg-info/SOURCES.txt` & `dvc-3.1.0/dvc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 .github/workflows/benchmarks.yaml
 .github/workflows/codeql.yml
 .github/workflows/packages.yaml
 .github/workflows/plugin_tests.yaml
 .github/workflows/tests.yaml
 dvc/__init__.py
 dvc/__main__.py
+dvc/_build.py
 dvc/_debug.py
 dvc/_dvc_version.py
 dvc/analytics.py
 dvc/annotations.py
+dvc/build.py
 dvc/cachemgr.py
 dvc/compare.py
 dvc/config.py
 dvc/config_schema.py
 dvc/daemon.py
 dvc/dagascii.py
 dvc/data_cloud.py
@@ -289,24 +291,22 @@
 dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
 dvc/ui/__init__.py
 dvc/ui/_rich_progress.py
 dvc/ui/pager.py
 dvc/ui/table.py
 dvc/utils/.gitignore
 dvc/utils/__init__.py
-dvc/utils/build.py
 dvc/utils/cli_parse.py
 dvc/utils/collections.py
 dvc/utils/diff.py
 dvc/utils/flatten.py
 dvc/utils/fs.py
 dvc/utils/humanize.py
 dvc/utils/hydra.py
 dvc/utils/objects.py
-dvc/utils/pkg.py
 dvc/utils/plots.py
 dvc/utils/strictyaml.py
 dvc/utils/studio.py
 dvc/utils/table.py
 dvc/utils/threadpool.py
 dvc/utils/serialize/__init__.py
 dvc/utils/serialize/_common.py
@@ -383,15 +383,14 @@
 tests/func/test_merge_driver.py
 tests/func/test_move.py
 tests/func/test_odb.py
 tests/func/test_remote.py
 tests/func/test_remove.py
 tests/func/test_repo.py
 tests/func/test_repo_index.py
-tests/func/test_repro.py
 tests/func/test_root.py
 tests/func/test_run.py
 tests/func/test_run_cache.py
 tests/func/test_scm.py
 tests/func/test_scm_context.py
 tests/func/test_stage.py
 tests/func/test_stage_load.py
@@ -443,14 +442,18 @@
 tests/func/parsing/test_foreach.py
 tests/func/parsing/test_interpolated_entry.py
 tests/func/parsing/test_resolver.py
 tests/func/plots/__init__.py
 tests/func/plots/test_diff.py
 tests/func/plots/test_modify.py
 tests/func/plots/test_show.py
+tests/func/repro/__init__.py
+tests/func/repro/test_repro.py
+tests/func/repro/test_repro_allow_missing.py
+tests/func/repro/test_repro_pull.py
 tests/func/utils/__init__.py
 tests/func/utils/test_hydra.py
 tests/func/utils/test_strict_yaml.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/test_studio_live_experiments.py
 tests/integration/plots/__init__.py
```

### Comparing `dvc-3.0.0a2/dvc.egg-info/requires.txt` & `dvc-3.1.0/dvc.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 colorama>=0.3.9
 configobj>=5.0.6
 distro>=1.3
 dpath<3,>=2.1.0
-dvc-data<0.55,>=0.54.3
+dvc-data<2.1.0,>=2.0.2
 dvc-http>=2.29.0
 dvc-render<1,>=0.3.1
 dvc-studio-client<1,>=0.9.2
-dvc-task<1,>=0.2.1
+dvc-task<1,>=0.3.0
 flatten_dict<1,>=0.4.1
 flufl.lock>=5
 funcy>=1.14
 grandalf<1,>=0.7
 hydra-core>=1.1
 iterative-telemetry>=0.0.7
 networkx>=2.5
@@ -61,15 +61,15 @@
 types-toml
 types-tqdm
 
 [oss]
 dvc-oss==2.19
 
 [s3]
-dvc-s3==2.22.0
+dvc-s3==2.23.0
 
 [ssh]
 dvc-ssh<3,>=2.22.1
 
 [ssh_gssapi]
 dvc-ssh[gssapi]<3,>=2.22.1
 
@@ -84,15 +84,15 @@
 [tests]
 dvc[testing]
 beautifulsoup4>=4.4
 dvc-ssh
 filelock
 flaky
 pytest<8,>=7
-pytest-cov
+pytest-cov>=4.1.0
 pytest-docker<2,>=1
 pytest-lazy-fixture
 pytest-mock
 pytest-test-utils
 pytest-timeout>=2
 pytest-xdist>=3.2
```

### Comparing `dvc-3.0.0a2/pyproject.toml` & `dvc-3.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 ]
 dynamic = ["version"]
 dependencies = [
     "colorama>=0.3.9",
     "configobj>=5.0.6",
     "distro>=1.3",
     "dpath<3,>=2.1.0",
-    "dvc-data>=0.54.3,<0.55",
+    "dvc-data>=2.0.2,<2.1.0",
     "dvc-http>=2.29.0",
     "dvc-render>=0.3.1,<1",
     "dvc-studio-client>=0.9.2,<1",
-    "dvc-task>=0.2.1,<1",
+    "dvc-task>=0.3.0,<1",
     "flatten_dict<1,>=0.4.1",
     "flufl.lock>=5",
     "funcy>=1.14",
     "grandalf<1,>=0.7",
     "hydra-core>=1.1",
     "iterative-telemetry>=0.0.7",
     "networkx>=2.5",
@@ -61,14 +61,15 @@
     "shtab<2,>=1.3.4",
     "tabulate>=0.8.7",
     "tomlkit>=0.11.1",
     "tqdm<5,>=4.63.1",
     "voluptuous>=0.11.7",
     "zc.lockfile>=1.2.1",
 ]
+
 [project.optional-dependencies]
 all = ["dvc[azure,gdrive,gs,hdfs,oss,s3,ssh,webdav,webhdfs]"]
 azure = ["dvc-azure>=2.21.2"]
 dev = ["dvc[azure,gdrive,gs,hdfs,lint,oss,s3,ssh,terraform,tests,webdav,webhdfs]"]
 gdrive = ["dvc-gdrive==2.19.2"]
 gs = ["dvc-gs==2.22.1"]
 hdfs = ["dvc-hdfs==2.19"]
@@ -79,15 +80,15 @@
     "types-psutil",
     "types-requests",
     "types-tabulate",
     "types-toml",
     "types-tqdm",
 ]
 oss = ["dvc-oss==2.19"]
-s3 = ["dvc-s3==2.22.0"]
+s3 = ["dvc-s3==2.23.0"]
 ssh = ["dvc-ssh>=2.22.1,<3"]
 ssh_gssapi = ["dvc-ssh[gssapi]>=2.22.1,<3"]
 terraform = ["tpi[ssh]>=2.1"]
 testing = [
   "pytest-test-utils",
   "pytest-benchmark[histogram]",
   "pytest-virtualenv",
@@ -95,35 +96,39 @@
 tests = [
     "dvc[testing]",
     "beautifulsoup4>=4.4",
     "dvc-ssh",
     "filelock",
     "flaky",
     "pytest<8,>=7",
-    "pytest-cov",
+    "pytest-cov>=4.1.0",
     "pytest-docker>=1,<2",
     "pytest-lazy-fixture",
     "pytest-mock",
     "pytest-test-utils",
     "pytest-timeout>=2",
     "pytest-xdist>=3.2",
     'pywin32>=225; sys_platform == "win32"', # optional test dependency
     'tzdata; sys_platform == "win32"',  # for testing with celery
 ]
 webdav = ["dvc-webdav==2.19.1"]
 webhdfs = ["dvc-webhdfs==2.19"]
 webhdfs_kerberos = ["dvc-webhdfs[kerberos]==2.19"]
+
 [project.urls]
 Documentation = "https://dvc.org/doc"
 Issues = "https://github.com/iterative/dvc/issues"
 Source = "https://github.com/iterative/dvc"
+
 [project.scripts]
 dvc = "dvc.cli:main"
+
 [project.entry-points."fsspec.specs"]
 dvc = "dvc.api:DVCFileSystem"
+
 [project.entry-points."pytest11"]
 dvc-testing = "dvc.testing.plugin"
 
 [tool.setuptools]
 license-files = ["LICENSE"]
 
 [tool.setuptools.packages.find]
@@ -139,35 +144,24 @@
 
 [tool.pytest.ini_options]
 addopts = "-ra --cov-config pyproject.toml --dist worksteal"
 filterwarnings = [
     "error::ResourceWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
     "error::pytest_mock.PytestMockWarning",
-    # remove when aiobotocore supports botocore>=1.29.13
-    "ignore:'cgi' is deprecated and slated for removal in Python 3.13:DeprecationWarning",
-    # also relates to botocore, but looks like it's not going to be fixed
     # https://github.com/boto/botocore/issues/2744
     "ignore:'urllib3.contrib.pyopenssl' module is deprecated:DeprecationWarning",
-    # ruamel.yaml: https://sourceforge.net/p/ruamel-yaml/tickets/452/
     # google.cloud: https://github.com/googleapis/python-storage/issues/1000
     # google.logging: https://github.com/googleapis/python-logging/issues/730
     # Also happens with `zc.lockfile`.
     "ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning",
-    # see https://github.com/celery/kombu/issues/1339
-    # and https://github.com/celery/celery/issues/7528
-    # drop when celery==5.3 && kombu==5.3 releases
-    "ignore:SelectableGroups dict interface is deprecated:DeprecationWarning",
     # tpi imports pkg_resources
     "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
     # see https://github.com/networkx/networkx/issues/5723.
     "ignore:nx.nx_pydot.* depends on the pydot package, which has.*known issues and is not actively maintained:DeprecationWarning",
-    # remove when new version of pytest-cov gets released
-    # https://github.com/pytest-dev/pytest-cov/issues/557
-    "ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated:DeprecationWarning",
 ]
 log_level = "debug"
 markers = [
     "needs_internet: Might need network access for the tests",
     "studio: Tests verifying contract between DVC and Studio",
     "vscode: Tests verifying contract between DVC and VSCode plugin",
 ]
```

### Comparing `dvc-3.0.0a2/scripts/build.py` & `dvc-3.1.0/scripts/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 parser.add_argument("--sign-installer", default=False, action="store_true")
 parser.add_argument("--installer-id")
 parser.add_argument("--notarize", default=False, action="store_true")
 parser.add_argument("--apple-id-username")
 parser.add_argument("--apple-id-password")
 args = parser.parse_args()
 
-(dvc / "utils" / "build.py").write_text(f'PKG = "{args.pkg}"')
+(dvc / "_build.py").write_text(f'PKG = "{args.pkg}"')
 
 if not (dvc / "_dvc_version.py").exists():
     raise Exception("no version info found")
 
 check_call(
     ["python", "build.py"],
     cwd=pyinstaller,
```

### Comparing `dvc-3.0.0a2/scripts/fpm/build.py` & `dvc-3.1.0/scripts/fpm/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/fpm/notarize.py` & `dvc-3.1.0/scripts/fpm/notarize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/fpm/sign.py` & `dvc-3.1.0/scripts/fpm/sign.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/innosetup/addSymLinkPermissions.ps1` & `dvc-3.1.0/scripts/innosetup/addSymLinkPermissions.ps1`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/innosetup/addsymlink.iss` & `dvc-3.1.0/scripts/innosetup/addsymlink.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/innosetup/build.py` & `dvc-3.1.0/scripts/innosetup/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/innosetup/modpath.iss` & `dvc-3.1.0/scripts/innosetup/modpath.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/innosetup/setup.iss` & `dvc-3.1.0/scripts/innosetup/setup.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/pyinstaller/build.py` & `dvc-3.1.0/scripts/pyinstaller/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.py` & `dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/scripts/pyinstaller/sign.py` & `dvc-3.1.0/scripts/pyinstaller/sign.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/conftest.py` & `dvc-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/dir_helpers.py` & `dvc-3.1.0/tests/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/api/test_data.py` & `dvc-3.1.0/tests/func/api/test_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def test_get_url_external(tmp_dir, erepo_dir, cloud):
     erepo_dir.add_remote(config=cloud.config)
     with erepo_dir.chdir():
         erepo_dir.dvc_gen("foo", "foo", commit="add foo")
 
     # Using file url to force clone to tmp repo
     repo_url = f"file://{erepo_dir.as_posix()}"
-    expected_url = (cloud / "ac/bd18db4cc2f85cedef654fccc4a4d8").url
+    expected_url = (cloud / "files" / "md5" / "ac/bd18db4cc2f85cedef654fccc4a4d8").url
     assert api.get_url("foo", repo=repo_url) == expected_url
 
 
 def test_get_url_requires_dvc(tmp_dir, scm):
     tmp_dir.scm_gen({"foo": "foo"}, commit="initial")
 
     with pytest.raises(OutputNotFoundError, match="output 'foo'"):
@@ -162,38 +162,50 @@
     )
 
 
 def test_get_url_granular(tmp_dir, dvc, cloud):
     tmp_dir.add_remote(config=cloud.config)
     tmp_dir.dvc_gen({"dir": {"foo": "foo", "bar": "bar", "nested": {"file": "file"}}})
 
-    expected_url = (cloud / "5f" / "c28ea78987408341668eba6525ebd1.dir").url
+    expected_url = (
+        cloud / "files" / "md5" / "5f" / "c28ea78987408341668eba6525ebd1.dir"
+    ).url
     assert api.get_url("dir") == expected_url
 
-    expected_url = (cloud / "ac" / "bd18db4cc2f85cedef654fccc4a4d8").url
+    expected_url = (
+        cloud / "files" / "md5" / "ac" / "bd18db4cc2f85cedef654fccc4a4d8"
+    ).url
     assert api.get_url("dir/foo") == expected_url
 
-    expected_url = (cloud / "37" / "b51d194a7513e45b56f6524f2d51f2").url
+    expected_url = (
+        cloud / "files" / "md5" / "37" / "b51d194a7513e45b56f6524f2d51f2"
+    ).url
     assert api.get_url("dir/bar") == expected_url
 
-    expected_url = (cloud / "8c" / "7dd922ad47494fc02c388e12c00eac").url
+    expected_url = (
+        cloud / "files" / "md5" / "8c" / "7dd922ad47494fc02c388e12c00eac"
+    ).url
     assert api.get_url(os.path.join("dir", "nested", "file")) == expected_url
 
 
 def test_get_url_subrepos(tmp_dir, scm, local_cloud):
     subrepo = tmp_dir / "subrepo"
     make_subrepo(subrepo, scm, config=local_cloud.config)
     with subrepo.chdir():
         subrepo.dvc_gen({"dir": {"foo": "foo"}, "bar": "bar"}, commit="add files")
         subrepo.dvc.push()
 
-    expected_url = os.fspath(local_cloud / "ac" / "bd18db4cc2f85cedef654fccc4a4d8")
+    expected_url = os.fspath(
+        local_cloud / "files" / "md5" / "ac" / "bd18db4cc2f85cedef654fccc4a4d8"
+    )
     assert api.get_url(os.path.join("subrepo", "dir", "foo")) == expected_url
 
-    expected_url = os.fspath(local_cloud / "37" / "b51d194a7513e45b56f6524f2d51f2")
+    expected_url = os.fspath(
+        local_cloud / "files" / "md5" / "37" / "b51d194a7513e45b56f6524f2d51f2"
+    )
     assert api.get_url("subrepo/bar") == expected_url
 
 
 def test_open_from_remote(tmp_dir, erepo_dir, cloud, local_cloud):
     erepo_dir.add_remote(config=cloud.config, name="other")
     erepo_dir.add_remote(config=local_cloud.config, default=True)
     erepo_dir.dvc_gen({"dir": {"foo": "foo content"}}, commit="create file")
@@ -202,7 +214,40 @@
 
     with api.open(
         os.path.join("dir", "foo"),
         repo=f"file://{erepo_dir.as_posix()}",
         remote="other",
     ) as fd:
         assert fd.read() == "foo content"
+
+    with api.open(
+        os.path.join("dir", "foo"),
+        repo=f"file://{erepo_dir.as_posix()}",
+        config={"core": {"remote": "other"}},
+    ) as fd:
+        assert fd.read() == "foo content"
+
+
+def test_read_from_remote(tmp_dir, erepo_dir, cloud, local_cloud):
+    erepo_dir.add_remote(config=cloud.config, name="other")
+    erepo_dir.add_remote(config=local_cloud.config, default=True)
+    erepo_dir.dvc_gen({"dir": {"foo": "foo content"}}, commit="create file")
+    erepo_dir.dvc.push(remote="other")
+    remove(erepo_dir.dvc.cache.local.path)
+
+    assert (
+        api.read(
+            os.path.join("dir", "foo"),
+            repo=f"file://{erepo_dir.as_posix()}",
+            remote="other",
+        )
+        == "foo content"
+    )
+
+    assert (
+        api.read(
+            os.path.join("dir", "foo"),
+            repo=f"file://{erepo_dir.as_posix()}",
+            config={"core": {"remote": "other"}},
+        )
+        == "foo content"
+    )
```

### Comparing `dvc-3.0.0a2/tests/func/api/test_experiments.py` & `dvc-3.1.0/tests/func/api/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/api/test_scm.py` & `dvc-3.1.0/tests/func/api/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/api/test_show.py` & `dvc-3.1.0/tests/func/api/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/artifacts/test_artifacts.py` & `dvc-3.1.0/tests/func/artifacts/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/data/db/test_index.py` & `dvc-3.1.0/tests/func/data/db/test_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dvc.exceptions import DownloadError, UploadError
 from dvc.utils.fs import remove
 from dvc_data.hashfile.db import get_index
 
 
 @pytest.fixture
-def index(dvc, local_remote, mocker):
+def index(tmp_dir, dvc, local_remote):
     odb = dvc.cloud.get_remote_odb("upstream")
     return get_index(odb)
 
 
 def test_indexed_on_status(tmp_dir, dvc, index):
     foo = tmp_dir.dvc_gen({"foo": "foo content"})[0].outs[0]
     bar = tmp_dir.dvc_gen({"bar": {"baz": "baz content"}})[0].outs[0]
@@ -54,31 +54,21 @@
     assert not list(index.hashes())
 
 
 def test_clear_on_download_err(tmp_dir, dvc, index, mocker):
     out = tmp_dir.dvc_gen({"dir": {"foo": "foo content"}})[0].outs[0]
     dvc.push()
 
+    assert list(index.hashes())
+
     for _, _, hi in out.obj:
         remove(dvc.cache.local.get(hi.value).path)
+        remove(dvc.cloud.get_remote().odb.get(hi.value).path)
     remove(out.fs_path)
 
-    assert list(index.hashes())
-
-    def unreliable_download(_from_fs, from_info, _to_fs, to_info, **kwargs):
-        on_error = kwargs["on_error"]
-        assert on_error
-        if isinstance(from_info, str):
-            from_info = [from_info]
-        if isinstance(to_info, str):
-            to_info = [to_info]
-        for from_i, to_i in zip(from_info, to_info):
-            on_error(from_i, to_i, Exception())
-
-    mocker.patch("dvc_objects.fs.generic.transfer", unreliable_download)
     with pytest.raises(DownloadError):
         dvc.pull()
     assert not list(index.hashes())
 
 
 def test_partial_upload(tmp_dir, dvc, index, mocker):
     from dvc_objects.fs import generic
```

### Comparing `dvc-3.0.0a2/tests/func/experiments/conftest.py` & `dvc-3.1.0/tests/func/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/executor/test_ssh.py` & `dvc-3.1.0/tests/func/experiments/executor/test_ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_apply.py` & `dvc-3.1.0/tests/func/experiments/test_apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_diff.py` & `dvc-3.1.0/tests/func/experiments/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_experiments.py` & `dvc-3.1.0/tests/func/experiments/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_queue.py` & `dvc-3.1.0/tests/func/experiments/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_remote.py` & `dvc-3.1.0/tests/func/experiments/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_remove.py` & `dvc-3.1.0/tests/func/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_save.py` & `dvc-3.1.0/tests/func/experiments/test_save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_set_params.py` & `dvc-3.1.0/tests/func/experiments/test_set_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_show.py` & `dvc-3.1.0/tests/func/experiments/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_stash_exp.py` & `dvc-3.1.0/tests/func/experiments/test_stash_exp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/experiments/test_utils.py` & `dvc-3.1.0/tests/func/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/machine/conftest.py` & `dvc-3.1.0/tests/func/machine/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/machine/test_machine_config.py` & `dvc-3.1.0/tests/func/machine/test_machine_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/machine/test_machine_status.py` & `dvc-3.1.0/tests/func/machine/test_machine_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/metrics/test_diff.py` & `dvc-3.1.0/tests/func/metrics/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/metrics/test_show.py` & `dvc-3.1.0/tests/func/metrics/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/params/test_diff.py` & `dvc-3.1.0/tests/func/params/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/params/test_show.py` & `dvc-3.1.0/tests/func/params/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/parsing/__init__.py` & `dvc-3.1.0/tests/func/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/parsing/test_errors.py` & `dvc-3.1.0/tests/func/parsing/test_errors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/parsing/test_foreach.py` & `dvc-3.1.0/tests/func/parsing/test_foreach.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/parsing/test_interpolated_entry.py` & `dvc-3.1.0/tests/func/parsing/test_interpolated_entry.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/parsing/test_resolver.py` & `dvc-3.1.0/tests/func/parsing/test_resolver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/plots/test_diff.py` & `dvc-3.1.0/tests/func/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/plots/test_modify.py` & `dvc-3.1.0/tests/func/plots/test_modify.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/plots/test_show.py` & `dvc-3.1.0/tests/func/plots/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_add.py` & `dvc-3.1.0/tests/func/test_add.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import errno
 import filecmp
 import os
 import shutil
 import stat
 import textwrap
-from unittest.mock import call
 
 import pytest
 
 import dvc_data
 from dvc.cachemgr import CacheManager
 from dvc.cli import main
 from dvc.config import ConfigError
@@ -18,15 +17,14 @@
 from dvc.output import (
     OutputAlreadyTrackedError,
     OutputDoesNotExistError,
     OutputIsStageFileError,
 )
 from dvc.stage import Stage
 from dvc.stage.exceptions import StageExternalOutputsError, StagePathNotFoundError
-from dvc.testing.workspace_tests import TestAdd
 from dvc.utils.fs import path_isin
 from dvc.utils.serialize import YAMLFileCorruptedError
 from dvc_data.hashfile.hash import file_md5
 from dvc_data.hashfile.hash_info import HashInfo
 from tests.utils import get_gitignore_content
 
 
@@ -47,14 +45,15 @@
 
     assert (tmp_dir / "foo.dvc").parse() == {
         "outs": [
             {
                 "md5": "acbd18db4cc2f85cedef654fccc4a4d8",
                 "path": "foo",
                 "size": 3,
+                "hash": "md5",
             }
         ]
     }
 
 
 @pytest.mark.skipif(os.name == "nt", reason="can't set exec bit on Windows")
 def test_add_executable(tmp_dir, dvc):
@@ -66,14 +65,15 @@
     assert (tmp_dir / "foo.dvc").parse() == {
         "outs": [
             {
                 "md5": "acbd18db4cc2f85cedef654fccc4a4d8",
                 "path": "foo",
                 "size": 3,
                 "isexec": True,
+                "hash": "md5",
             }
         ]
     }
     assert os.stat("foo").st_mode & stat.S_IEXEC
 
 
 def test_add_unicode(tmp_dir, dvc):
@@ -228,62 +228,14 @@
         assert stage.relpath in expected_rel_paths
 
         # Current dir should not be taken into account
         assert stage.wdir == os.path.dirname(stage.path)
         assert stage.outs[0].def_path in expected_def_paths
 
 
-class TestAddExternal(TestAdd):
-    @pytest.fixture
-    def hash_name(self):
-        return "md5"
-
-    @pytest.fixture
-    def hash_value(self):
-        return "8c7dd922ad47494fc02c388e12c00eac"
-
-    @pytest.fixture
-    def dir_hash_value(self):
-        return "b6dcab6ccd17ca0a8bf4a215a37d14cc.dir"
-
-
-def test_add_external_relpath(tmp_dir, dvc, local_cloud):
-    (fpath,) = local_cloud.gen("file", "file")
-    rel = os.path.relpath(fpath)
-
-    with pytest.raises(StageExternalOutputsError):
-        dvc.add(rel)
-
-    dvc.add(rel, external=True)
-    assert (tmp_dir / "file.dvc").read_text() == (
-        "outs:\n"
-        "- md5: 8c7dd922ad47494fc02c388e12c00eac\n"
-        "  size: 4\n"
-        f"  path: {rel}\n"
-    )
-    assert fpath.read_text() == "file"
-    assert dvc.status() == {}
-
-
-def test_add_local_remote_file(tmp_dir, dvc):
-    """
-    Making sure that 'remote' syntax is handled properly for local outs.
-    """
-    tmp_dir.gen({"foo": "foo", "bar": "bar"})
-    tmp_dir.add_remote(url=tmp_dir.fs_path, name="myremote")
-
-    assert main(["add", "remote://myremote/foo"]) == 0
-    d = (tmp_dir / "foo.dvc").load_yaml()
-    assert d["outs"][0]["path"] == "remote://myremote/foo"
-
-    assert main(["add", (tmp_dir / "bar").fs_path]) == 0
-    d = (tmp_dir / "bar.dvc").load_yaml()
-    assert d["outs"][0]["path"] == "bar"
-
-
 def test_cmd_add(tmp_dir, dvc):
     tmp_dir.gen("foo", "foo")
     ret = main(["add", "foo"])
     assert ret == 0
 
     ret = main(["add", "non-existing-file"])
     assert ret != 0
@@ -674,16 +626,16 @@
 def test_add_optimization_for_hardlink_on_empty_files(tmp_dir, dvc, mocker):
     dvc.cache.local.cache_types = ["hardlink"]
     tmp_dir.gen({"foo": "", "bar": "", "lorem": "lorem", "ipsum": "ipsum"})
     m = mocker.spy(LocalFileSystem, "is_hardlink")
     stages = dvc.add(["foo", "bar", "lorem", "ipsum"])
 
     assert m.call_count == 8
-    assert m.call_args != call(tmp_dir / "foo")
-    assert m.call_args != call(tmp_dir / "bar")
+    assert m.call_args != mocker.call(tmp_dir / "foo")
+    assert m.call_args != mocker.call(tmp_dir / "bar")
 
     for stage in stages[:2]:
         # hardlinks are not created for empty files
         assert not system.is_hardlink(stage.outs[0].fs_path)
 
     for stage in stages[2:]:
         assert system.is_hardlink(stage.outs[0].fs_path)
@@ -725,53 +677,53 @@
     assert (tmp_dir / "dir" / "foo.dvc").exists()
     assert not (tmp_dir / "dir" / "foo").is_symlink()
     assert not (tmp_dir / "dir" / "bar").is_symlink()
     assert (tmp_dir / "dir" / "foo").read_text() == "bar"
     assert (tmp_dir / "dir" / "bar").read_text() == "bar"
 
     assert (
-        tmp_dir / ".dvc" / "cache" / "37" / "b51d194a7513e45b56f6524f2d51f2"
+        tmp_dir
+        / ".dvc"
+        / "cache"
+        / "files"
+        / "md5"
+        / "37"
+        / "b51d194a7513e45b56f6524f2d51f2"
     ).read_text() == "bar"
     assert not (
-        tmp_dir / ".dvc" / "cache" / "37" / "b51d194a7513e45b56f6524f2d51f2"
+        tmp_dir
+        / ".dvc"
+        / "cache"
+        / "files"
+        / "md5"
+        / "37"
+        / "b51d194a7513e45b56f6524f2d51f2"
     ).is_symlink()
 
     # Test that subsequent add succeeds
     # See https://github.com/iterative/dvc/issues/4654
     dvc.add(os.path.join("dir", "foo"))
 
 
-@pytest.mark.parametrize("external", [True, False])
-def test_add_symlink_dir(make_tmp_dir, tmp_dir, dvc, external):
-    if external:
-        data_dir = make_tmp_dir("data")
-        data_dir.gen({"foo": "foo"})
-        target = os.fspath(data_dir)
-    else:
-        tmp_dir.gen({"data": {"foo": "foo"}})
-        target = os.path.join(".", "data")
+def test_add_symlink_dir(make_tmp_dir, tmp_dir, dvc):
+    tmp_dir.gen({"data": {"foo": "foo"}})
+    target = os.path.join(".", "data")
 
     tmp_dir.gen({"data": {"foo": "foo"}})
 
     (tmp_dir / "dir").symlink_to(target)
 
     msg = "Cannot add files inside symlinked directories to DVC"
     with pytest.raises(DvcException, match=msg):
         dvc.add("dir")
 
 
-@pytest.mark.parametrize("external", [True, False])
-def test_add_file_in_symlink_dir(make_tmp_dir, tmp_dir, dvc, external):
-    if external:
-        data_dir = make_tmp_dir("data")
-        data_dir.gen({"dir": {"foo": "foo"}})
-        target = os.fspath(data_dir / "dir")
-    else:
-        tmp_dir.gen({"data": {"foo": "foo"}})
-        target = os.path.join(".", "data")
+def test_add_file_in_symlink_dir(make_tmp_dir, tmp_dir, dvc):
+    tmp_dir.gen({"data": {"foo": "foo"}})
+    target = os.path.join(".", "data")
 
     (tmp_dir / "dir").symlink_to(target)
 
     msg = "Cannot add files inside symlinked directories to DVC"
     with pytest.raises(DvcException, match=msg):
         dvc.add(os.path.join("dir", "foo"))
 
@@ -786,15 +738,21 @@
     dvc.add("foo")
     err = capsys.readouterr()[1]
     assert "reconfigure cache types" in err
 
     assert (tmp_dir / "foo").exists()
     assert (tmp_dir / "foo.dvc").exists()
     assert (
-        tmp_dir / ".dvc" / "cache" / "ac" / "bd18db4cc2f85cedef654fccc4a4d8"
+        tmp_dir
+        / ".dvc"
+        / "cache"
+        / "files"
+        / "md5"
+        / "ac"
+        / "bd18db4cc2f85cedef654fccc4a4d8"
     ).read_text() == "foo"
 
 
 def test_add_preserve_fields(tmp_dir, dvc):
     text = textwrap.dedent(
         """\
         # top comment
```

### Comparing `dvc-3.0.0a2/tests/func/test_analytics.py` & `dvc-3.1.0/tests/func/test_analytics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from unittest.mock import call
 
 import pytest
 
 from dvc.analytics import _scm_in_use, collect_and_send_report
 from dvc.cli import main
 from dvc.repo import Repo
 from tests.utils import ANY
@@ -36,15 +35,15 @@
 
 def test_collect_and_send_report(mocker, dvc, mock_daemon):
     mock_post = mocker.patch("requests.post")
     collect_and_send_report()
 
     assert mock_daemon.call_count == 1
     assert mock_post.call_count == 1
-    assert mock_post.call_args == call(
+    assert mock_post.call_args == mocker.call(
         "https://analytics.dvc.org",
         json=ANY(dict),
         headers={"content-type": "application/json"},
         timeout=5,
     )
```

### Comparing `dvc-3.0.0a2/tests/func/test_check_ignore.py` & `dvc-3.1.0/tests/func/test_check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_checkout.py` & `dvc-3.1.0/tests/func/test_checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,60 +60,14 @@
 
     assert main(["checkout", "--force", "foo.dvc"]) == 0
     assert main(["checkout", "--force", "data.dvc"]) == 0
     assert (tmp_dir / "foo").read_text() == "foo"
     assert (tmp_dir / "data").read_text() == {"file": "file"}
 
 
-def test_checkout_corrupted_cache_file(tmp_dir, dvc):
-    (foo_stage,) = tmp_dir.dvc_gen("foo", "foo")
-    cache = foo_stage.outs[0].cache_path
-
-    os.chmod(cache, 0o644)
-    with open(cache, "a", encoding="utf-8") as fd:
-        fd.write("1")
-
-    with pytest.raises(CheckoutError):
-        dvc.checkout(force=True, relink=True)
-
-    assert not os.path.isfile("foo")
-    assert not os.path.isfile(cache)
-
-
-def test_checkout_corrupted_cache_dir(tmp_dir, dvc):
-    from dvc_data.hashfile import load
-
-    tmp_dir.gen("data", {"foo": "foo", "bar": "bar"})
-    # NOTE: using 'copy' so that cache and link don't have same inode
-    ret = main(["config", "cache.type", "copy"])
-    assert ret == 0
-
-    dvc.config.load()
-
-    stages = dvc.add("data")
-    assert len(stages) == 1
-    assert len(stages[0].outs) == 1
-    out = stages[0].outs[0]
-
-    # NOTE: modifying cache file for one of the files inside the directory
-    # to check if dvc will detect that the cache is corrupted.
-    obj = load(dvc.cache.local, out.hash_info)
-    _, _, entry_oid = list(obj)[0]
-    cache = dvc.cache.local.oid_to_path(entry_oid.value)
-
-    os.chmod(cache, 0o644)
-    with open(cache, "w+", encoding="utf-8") as fobj:
-        fobj.write("1")
-
-    with pytest.raises(CheckoutError):
-        dvc.checkout(force=True, relink=True)
-
-    assert not os.path.exists(cache)
-
-
 def test_remove_files_when_checkout(tmp_dir, dvc, scm):
     # add the file into a separate branch
     scm.checkout("branch", True)
     ret = main(["checkout", "--force"])
     assert ret == 0
     tmp_dir.dvc_gen("file_in_a_branch", "random text", commit="add file")
 
@@ -325,16 +279,16 @@
 
     assert system.is_symlink("foo")
     old_foo_link = os.path.realpath("foo")
 
     assert system.is_symlink(os.path.join("data", "file"))
     old_data_link = os.path.realpath(os.path.join("data", "file"))
 
-    old_cache_dir = dvc.cache.local.path
-    new_cache_dir = old_cache_dir + "_new"
+    old_cache_dir = str(tmp_dir / ".dvc" / "cache")
+    new_cache_dir = str(tmp_dir / ".dvc" / "cache_new")
     os.rename(old_cache_dir, new_cache_dir)
 
     ret = main(["cache", "dir", new_cache_dir])
     assert ret == 0
 
     ret = main(["checkout", "-f"])
     assert ret == 0
@@ -366,38 +320,33 @@
     "link, link_test_func",
     [("hardlink", system.is_hardlink), ("symlink", system.is_symlink)],
 )
 def test_checkout_relink(tmp_dir, dvc, link, link_test_func):
     dvc.cache.local.cache_types = [link]
 
     tmp_dir.dvc_gen({"dir": {"data": "text"}})
-    dvc.unprotect("dir/data")
-    assert not link_test_func("dir/data")
-
-    stats = dvc.checkout(["dir.dvc"], relink=True)
-    assert stats == empty_checkout
-    assert link_test_func("dir/data")
 
+    data_file = os.path.join("dir", "data")
 
-@pytest.mark.parametrize("link", ["hardlink", "symlink", "copy"])
-def test_checkout_relink_protected(tmp_dir, dvc, link):
-    dvc.cache.local.cache_types = [link]
+    # NOTE: Windows symlink perms don't propagate to the target
+    if not (os.name == "nt" and link == "symlink"):
+        assert not os.access(data_file, os.W_OK)
 
-    tmp_dir.dvc_gen("foo", "foo")
-    dvc.unprotect("foo")
-    assert os.access("foo", os.W_OK)
+    dvc.unprotect(data_file)
+    assert os.access(data_file, os.W_OK)
+    assert not link_test_func(data_file)
 
-    stats = dvc.checkout(["foo.dvc"], relink=True)
+    stats = dvc.checkout(["dir.dvc"], relink=True)
     assert stats == empty_checkout
+    assert link_test_func(data_file)
 
-    # NOTE: Windows symlink perms don't propagate to the target
-    if link == "copy" or (link == "symlink" and os.name == "nt"):
-        assert os.access("foo", os.W_OK)
-    else:
-        assert not os.access("foo", os.W_OK)
+    # NOTE: Windows symlink perms don't propagate to the target and
+    # hardlink was chmod-ed during relink to be deleted
+    if not (os.name == "nt" and link in ["symlink", "hardlink"]):
+        assert not os.access(data_file, os.W_OK)
 
 
 @pytest.mark.parametrize(
     "target",
     [os.path.join("dir", "subdir"), os.path.join("dir", "subdir", "file")],
 )
 def test_partial_checkout(tmp_dir, dvc, target):
@@ -797,14 +746,15 @@
     (stage,) = tmp_dir.dvc_gen({"data": {"foo": "foo"}})
     tmp_dir.gen(
         "data.dvc",
         textwrap.dedent(
             f"""\
         outs:
         - md5: {stage.outs[0].hash_info.value}
+          hash: md5
           path: data
         """
         ),
     )
     remove("data")
     dvc.checkout()
     assert (tmp_dir / "data").read_text() == {"foo": "foo"}
```

### Comparing `dvc-3.0.0a2/tests/func/test_cli.py` & `dvc-3.1.0/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_commit.py` & `dvc-3.1.0/tests/func/test_commit.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,15 @@
           labels:
           - label1
           - label2
           meta:
             key1: value1
             key2: value2
           remote: testremote
+          hash: md5
         meta: some metadata
     """
     )
     tmp_dir.gen("foo.dvc", text)
     tmp_dir.dvc_gen("foo", "foo", commit=False)
     dvc.commit("foo")
     assert (tmp_dir / "foo.dvc").read_text() == textwrap.dedent(
@@ -73,14 +74,15 @@
           labels:
           - label1
           - label2
           meta:
             key1: value1
             key2: value2
           remote: testremote
+          hash: md5
           md5: acbd18db4cc2f85cedef654fccc4a4d8
           size: 3
         meta: some metadata
     """
     )
 
 
@@ -125,20 +127,23 @@
     dvc.commit(stage.path, force=True)
     assert dvc.status(stage.path) == {}
 
 
 def test_commit_granular_output(tmp_dir, dvc):
     dvc.run(
         name="mystage",
-        cmd=["echo foo>foo", "echo bar>bar"],
+        cmd=[
+            "python -c \"open('foo', 'wb').write(b'foo\\n')\"",
+            "python -c \"open('bar', 'wb').write(b'bar\\n')\"",
+        ],
         outs=["foo", "bar"],
         no_commit=True,
     )
 
-    cache = tmp_dir / ".dvc" / "cache"
+    cache = tmp_dir / ".dvc" / "cache" / "files" / "md5"
     assert not list(cache.glob("*/*"))
 
     dvc.commit("foo")
     assert list(cache.glob("*/*")) == [cache / "d3" / "b07384d113edec49eaa6238ad5ff00"]
 
 
 def test_commit_granular_output_file(tmp_dir, dvc):
@@ -171,15 +176,15 @@
                 "bar": "bar",
                 "subdir": {"subfoo": "subfoo", "subbar": "subbar"},
             }
         }
     )
     dvc.add("data", no_commit=True)
 
-    cache = tmp_dir / ".dvc" / "cache"
+    cache = tmp_dir / ".dvc" / "cache" / "files" / "md5"
 
     assert set(cache.glob("*/*")) == set()
 
     dvc.commit(os.path.join("data", "foo"))
     assert set(cache.glob("*/*")) == {
         cache / "1a" / "ca2c799df82929bbdd976557975546.dir",
         cache / "ac" / "bd18db4cc2f85cedef654fccc4a4d8",
@@ -244,14 +249,15 @@
 def test_commit_updates_to_cloud_versioning_dir(tmp_dir, dvc):
     data_dvc = tmp_dir / "data.dvc"
     data_dvc.dump(
         {
             "outs": [
                 {
                     "path": "data",
+                    "hash": "md5",
                     "files": [
                         {
                             "size": 3,
                             "version_id": "WYRG4BglP7pD.gEoJP6a4AqOhl.FRA.h",
                             "etag": "acbd18db4cc2f85cedef654fccc4a4d8",
                             "md5": "acbd18db4cc2f85cedef654fccc4a4d8",
                             "relpath": "bar",
@@ -276,14 +282,15 @@
 
     dvc.commit("data", force=True)
 
     assert (tmp_dir / "data.dvc").parse() == {
         "outs": [
             {
                 "path": "data",
+                "hash": "md5",
                 "files": [
                     {
                         "size": 4,
                         "md5": "224e2539f52203eb33728acd228b4432",
                         "relpath": "bar",
                     },
                     {
@@ -293,7 +300,25 @@
                         "md5": "acbd18db4cc2f85cedef654fccc4a4d8",
                         "relpath": "foo",
                     },
                 ],
             }
         ]
     }
+
+
+def test_commit_dos2unix(tmp_dir, dvc):
+    tmp_dir.gen("foo", "foo")
+    (tmp_dir / "foo.dvc").dump(
+        {
+            "outs": [
+                {"path": "foo", "md5": "acbd18db4cc2f85cedef654fccc4a4d8", "size": 3},
+            ]
+        }
+    )
+    legacy_content = (tmp_dir / "foo.dvc").read_text()
+
+    dvc.commit("foo.dvc")
+    assert (tmp_dir / "foo.dvc").read_text() == legacy_content
+    dvc.commit("foo.dvc", force=True)
+    content = (tmp_dir / "foo.dvc").read_text()
+    assert "hash: md5" in content
```

### Comparing `dvc-3.0.0a2/tests/func/test_config.py` & `dvc-3.1.0/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_data_cloud.py` & `dvc-3.1.0/tests/func/test_data_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,16 @@
     # purge cache
     dvc.cache.local.clear()
 
     header = (
         "Some of the cache files do not exist "
         "neither locally nor on remote. Missing cache files:\n"
     )
-    foo = "name: bar, md5: 37b51d194a7513e45b56f6524f2d51f2\n"
-    bar = "name: foo, md5: acbd18db4cc2f85cedef654fccc4a4d8\n"
+    foo = "md5: 37b51d194a7513e45b56f6524f2d51f2\n"
+    bar = "md5: acbd18db4cc2f85cedef654fccc4a4d8\n"
 
     caplog.clear()
     dvc.push()
     assert header in caplog.text
     assert foo in caplog.text
     assert bar in caplog.text
 
@@ -193,24 +193,24 @@
     remove("file")
     remove("dir")
     dvc.cache.local.clear()
 
     hash_spy = mocker.spy(dvc_data.hashfile.hash, "file_md5")
 
     dvc.pull()
-    # NOTE: 1 is for index.data_tree building
-    assert hash_spy.call_count == 1
+    # NOTE: 2 are for index.data_tree building
+    assert hash_spy.call_count == 3
 
     # Removing cache will invalidate existing state entries
     dvc.cache.local.clear()
 
     dvc.config["remote"]["upstream"]["verify"] = True
 
     dvc.pull()
-    assert hash_spy.call_count == 6
+    assert hash_spy.call_count == 10
 
 
 @flaky(max_runs=3, min_passes=1)
 @pytest.mark.parametrize(
     "erepo", [pytest.lazy_fixture("git_dir"), pytest.lazy_fixture("erepo_dir")]
 )
 def test_pull_git_imports(tmp_dir, dvc, scm, erepo):
@@ -264,15 +264,15 @@
 
 def test_pull_partial_import(tmp_dir, dvc, local_workspace):
     local_workspace.gen("file", "file content")
     dst = tmp_dir / "file"
     stage = dvc.imp_url("remote://workspace/file", os.fspath(dst), no_download=True)
 
     result = dvc.pull("file")
-    assert result["fetched"] == 1
+    assert result["fetched"] == 0
     assert dst.exists()
 
     assert stage.outs[0].get_hash().value == "d10b4c3ff123b26dc068d43a8bef2d23"
 
 
 def test_pull_external_dvc_imports_mixed(tmp_dir, dvc, scm, erepo_dir, local_remote):
     with erepo_dir.chdir():
@@ -466,28 +466,28 @@
     # pushing everything so as we can check pull/fetch only downloads
     # from specified targets
     dvc.push()
     clean(["foo", "bar"], dvc)
 
     dvc.pull("copy-foo-bar")
     assert (tmp_dir / "bar").exists()
-    assert len(recurse_list_dir(dvc.cache.local.path)) == 2
+    assert len(recurse_list_dir(dvc.cache.local.path)) == 1
     clean(["bar"], dvc)
 
     dvc.fetch("copy-foo-bar")
-    assert len(recurse_list_dir(dvc.cache.local.path)) == 2
+    assert len(recurse_list_dir(dvc.cache.local.path)) == 1
 
 
 def test_pull_partial(tmp_dir, dvc, local_remote):
     tmp_dir.dvc_gen({"foo": {"bar": {"baz": "baz"}, "spam": "spam"}})
     dvc.push()
     clean(["foo"], dvc)
 
     stats = dvc.pull(os.path.join("foo", "bar"))
-    assert stats["fetched"] == 1
+    assert stats["fetched"] == 3
     assert (tmp_dir / "foo").read_text() == {"bar": {"baz": "baz"}}
 
 
 def test_output_remote(tmp_dir, dvc, make_remote):
     make_remote("default", default=True)
     make_remote("for_foo", default=False)
     make_remote("for_data", default=False)
```

### Comparing `dvc-3.0.0a2/tests/func/test_data_status.py` & `dvc-3.1.0/tests/func/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_diff.py` & `dvc-3.1.0/tests/func/test_diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 
     tmp_dir.dvc_gen("file", "text")
 
     with pytest.raises(NoSCMError):
         dvc.diff()
 
 
+def test_same_rev(tmp_dir, scm, dvc):
+    tmp_dir.dvc_gen("file", "text", commit="add file")
+
+    assert not dvc.diff("HEAD", "HEAD")
+    assert not dvc.diff("HEAD", "master")
+    assert not dvc.diff("master", "HEAD")
+
+
 def test_added(tmp_dir, scm, dvc):
     tmp_dir.dvc_gen("file", "text")
 
     assert dvc.diff() == {
         "added": [{"path": "file", "hash": digest("text")}],
         "deleted": [],
         "modified": [],
```

### Comparing `dvc-3.0.0a2/tests/func/test_dvcfile.py` & `dvc-3.1.0/tests/func/test_dvcfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,7 +398,19 @@
         },
     )
     plots = list(dvc.plots.collect())
     top_level_plots = plots[0]["workspace"]["definitions"]["data"]["dvc.yaml"]["data"]
     assert all(
         name in top_level_plots for name in ("path/to/plot", "path/to/another/plot")
     )
+
+
+def test_dvcfile_dos2unix(tmp_dir, dvc):
+    from dvc_data.hashfile.hash import HashInfo
+
+    (tmp_dir / "foo.dvc").dump({"outs": [{"md5": "abc123", "size": 3, "path": "foo"}]})
+    orig_content = (tmp_dir / "foo.dvc").read_text()
+    stage = dvc.stage.load_one("foo.dvc")
+    assert stage.outs[0].hash_name == "md5-dos2unix"
+    assert stage.outs[0].hash_info == HashInfo("md5-dos2unix", "abc123")
+    stage.dump()
+    assert (tmp_dir / "foo.dvc").read_text() == orig_content
```

### Comparing `dvc-3.0.0a2/tests/func/test_external_repo.py` & `dvc-3.1.0/tests/func/test_external_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from unittest.mock import ANY
 
 from dvc.repo.open_repo import CLONES
 from dvc.repo.open_repo import _external_repo as external_repo
 from dvc.scm import Git
 from dvc.testing.tmp_dir import make_subrepo
 from dvc.utils import relpath
 from dvc.utils.fs import remove
@@ -136,15 +135,17 @@
     url = os.fspath(erepo_dir)
     clone_spy = mocker.spy(Git, "clone")
 
     with external_repo(url, rev="branch") as repo:
         with repo.dvcfs.open("file") as fd:
             assert fd.read() == "branch"
 
-    clone_spy.assert_called_with(url, ANY, shallow_branch="branch", progress=ANY)
+    clone_spy.assert_called_with(
+        url, mocker.ANY, shallow_branch="branch", progress=mocker.ANY
+    )
 
     path, _ = CLONES[url]
     CLONES[url] = (path, True)
 
     mock_fetch = mocker.patch.object(Git, "fetch")
     with external_repo(url) as repo:
         with repo.dvcfs.open("file") as fd:
@@ -161,15 +162,17 @@
     url = os.fspath(erepo_dir)
 
     clone_spy = mocker.spy(Git, "clone")
     with external_repo(url, rev="v1") as repo:
         with repo.dvcfs.open("file") as fd:
             assert fd.read() == "foo"
 
-    clone_spy.assert_called_with(url, ANY, shallow_branch="v1", progress=ANY)
+    clone_spy.assert_called_with(
+        url, mocker.ANY, shallow_branch="v1", progress=mocker.ANY
+    )
 
     path, _ = CLONES[url]
     CLONES[url] = (path, True)
 
     mock_fetch = mocker.patch.object(Git, "fetch")
     with external_repo(url, rev="master") as repo:
         with repo.dvcfs.open("file") as fd:
@@ -210,18 +213,28 @@
         transfer(
             staging,
             repo.cache.local,
             {obj.hash_info},
             shallow=False,
             hardlink=True,
         )
+        if os.name == "nt":
+            expected_gitignore_path = (
+                cache_dir / "d5" / "61e684092f0ff908aa82ee9cc1e594"
+            )
+            expected_dir_path = cache_dir / "0d" / "2086760aea091f1504eafc8843bb18.dir"
+        else:
+            expected_gitignore_path = (
+                cache_dir / "94" / "7d2b84e5aa88170e80dff467a5bfb6"
+            )
+            expected_dir_path = cache_dir / "e1" / "d9e8eae5374860ae025ec84cfd85c7.dir"
         assert set(cache_dir.glob("??/*")) == {
-            cache_dir / "e1" / "d9e8eae5374860ae025ec84cfd85c7.dir",
+            expected_dir_path,
+            expected_gitignore_path,
             cache_dir / "37" / "b51d194a7513e45b56f6524f2d51f2",
-            cache_dir / "94" / "7d2b84e5aa88170e80dff467a5bfb6",
             cache_dir / "ac" / "bd18db4cc2f85cedef654fccc4a4d8",
         }
 
 
 def test_subrepos_are_ignored_for_git_tracked_dirs(tmp_dir, erepo_dir):
     subrepo = erepo_dir / "dir" / "subrepo"
     make_subrepo(subrepo, erepo_dir.scm)
```

### Comparing `dvc-3.0.0a2/tests/func/test_fs.py` & `dvc-3.1.0/tests/func/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_gc.py` & `dvc-3.1.0/tests/func/test_gc.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,34 +247,14 @@
 
     # remove pipeline file and lockfile and check
     load_file(dvc, PROJECT_FILE).remove(force=True)
     dvc.gc(workspace=True, force=True)
     assert _count_files(dvc.cache.local.path) == 0
 
 
-def test_gc_external_output(tmp_dir, dvc, workspace):
-    workspace.gen({"foo": "foo", "bar": "bar"})
-
-    (foo_stage,) = dvc.add("remote://workspace/foo")
-    (bar_stage,) = dvc.add("remote://workspace/bar")
-
-    foo_hash = foo_stage.outs[0].hash_info.value
-    bar_hash = bar_stage.outs[0].hash_info.value
-
-    assert (workspace / "cache" / foo_hash[:2] / foo_hash[2:]).read_text() == "foo"
-    assert (workspace / "cache" / bar_hash[:2] / bar_hash[2:]).read_text() == "bar"
-
-    (tmp_dir / "foo.dvc").unlink()
-
-    dvc.gc(workspace=True)
-
-    assert not (workspace / "cache" / foo_hash[:2] / foo_hash[2:]).exists()
-    assert (workspace / "cache" / bar_hash[:2] / bar_hash[2:]).read_text() == "bar"
-
-
 def test_gc_all_experiments(tmp_dir, scm, dvc):
     from dvc.repo.experiments.refs import ExpRefInfo
 
     (foo,) = tmp_dir.dvc_gen("foo", "foo", commit="foo")
     foo_hash = foo.outs[0].hash_info.value
 
     tmp_dir.dvc_gen("foo", "bar", commit="bar")
@@ -284,17 +264,19 @@
     baz_hash = baz.outs[0].hash_info.value
 
     ref = ExpRefInfo(baseline, "exp")
     scm.set_ref(str(ref), scm.get_rev())
 
     dvc.gc(all_experiments=True, force=True)
 
-    assert not (tmp_dir / ".dvc" / "cache" / foo_hash[:2] / foo_hash[2:]).exists()
+    assert not (
+        tmp_dir / ".dvc" / "cache" / "files" / "md5" / foo_hash[:2] / foo_hash[2:]
+    ).exists()
     assert (
-        tmp_dir / ".dvc" / "cache" / baz_hash[:2] / baz_hash[2:]
+        tmp_dir / ".dvc" / "cache" / "files" / "md5" / baz_hash[:2] / baz_hash[2:]
     ).read_text() == "baz"
 
 
 def test_gc_rev_num(tmp_dir, scm, dvc):
     num = 2
 
     hashes = {}
@@ -302,15 +284,17 @@
         i_str = str(i)
         f = tmp_dir.dvc_gen("foo", i_str, commit=i_str)
         hashes[i] = f[0].outs[0].hash_info.value
 
     dvc.gc(rev="HEAD", num=num, force=True)
 
     for n, i in enumerate(reversed(range(4))):
-        cache = tmp_dir / ".dvc" / "cache" / hashes[i][:2] / hashes[i][2:]
+        cache = (
+            tmp_dir / ".dvc" / "cache" / "files" / "md5" / hashes[i][:2] / hashes[i][2:]
+        )
         if n >= num:
             assert not cache.exists()
         else:
             assert cache.read_text() == str(i)
 
 
 def test_date(tmp_dir, scm, dvc):
@@ -412,14 +396,15 @@
     dvc.config["remote"]["other_remote"] = {"url": other_storage}
 
     text = textwrap.dedent(
         """\
         outs:
         - path: foo
           remote: other_remote
+          hash: md5
     """
     )
     tmp_dir.gen("foo.dvc", text)
     tmp_dir.dvc_gen("foo", "foo")
     dvc.push()
 
     mocked_remove = mocker.spy(LocalFileSystem, "remove")
@@ -443,14 +428,15 @@
     dvc.config["remote"]["other_remote"] = {"url": other_storage}
 
     text = textwrap.dedent(
         """\
         outs:
         - path: foo
           remote: other_remote
+          hash: md5
     """
     )
     tmp_dir.gen("foo.dvc", text)
     tmp_dir.dvc_gen("foo", "foo")
     dvc.push()
     tmp_dir.dvc_gen("foo", "bar")
```

### Comparing `dvc-3.0.0a2/tests/func/test_get.py` & `dvc-3.1.0/tests/func/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,28 +125,14 @@
 
 
 def test_get_a_dvc_file(tmp_dir, erepo_dir):
     with pytest.raises(GetDVCFileError):
         Repo.get(os.fspath(erepo_dir), "some_file.dvc")
 
 
-# https://github.com/iterative/dvc/pull/2837#discussion_r352123053
-def test_get_full_dvc_path(tmp_dir, erepo_dir, tmp_path_factory):
-    path = tmp_path_factory.mktemp("ext")
-    external_data = path / "ext_data"
-    external_data.write_text("ext_data")
-
-    with erepo_dir.chdir():
-        erepo_dir.dvc.add(os.fspath(external_data), external=True)
-        erepo_dir.scm_add("ext_data.dvc", commit="add external data")
-
-    Repo.get(os.fspath(erepo_dir), os.fspath(external_data), "ext_data_imported")
-    assert (tmp_dir / "ext_data_imported").read_text() == "ext_data"
-
-
 def test_non_cached_output(tmp_dir, erepo_dir):
     src = "non_cached_file"
     dst = src + "_imported"
 
     with erepo_dir.chdir():
         erepo_dir.dvc.run(
             outs_no_cache=[src], cmd="echo hello > non_cached_file", name="gen"
```

### Comparing `dvc-3.0.0a2/tests/func/test_get_url.py` & `dvc-3.1.0/tests/func/test_get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_ignore.py` & `dvc-3.1.0/tests/func/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_import.py` & `dvc-3.1.0/tests/func/test_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,21 +237,26 @@
             + len(b"baz contents")
             + len((erepo_dir / "foo" / ".gitignore").read_bytes())
         )
 
     dvc.imp(os.fspath(erepo_dir), "foo", "foo_imported", no_download=True)
 
     dvc.pull(["foo_imported.dvc"])
-    assert (tmp_dir / "foo_imported").exists
+    assert (tmp_dir / "foo_imported").exists()
     assert (tmp_dir / "foo_imported" / "bar").read_bytes() == b"bar"
     assert (tmp_dir / "foo_imported" / "baz").read_bytes() == b"baz contents"
 
-    stage = load_file(dvc, "foo_imported.dvc").stage
+    dvc.commit(force=True)
 
-    assert stage.outs[0].hash_info.value == "bdb8641831d8fcb03939637e09011c21.dir"
+    stage = load_file(dvc, "foo_imported.dvc").stage
+    if os.name == "nt":
+        expected_hash = "2e798234df5f782340ac3ce046f8dfae.dir"
+    else:
+        expected_hash = "bdb8641831d8fcb03939637e09011c21.dir"
+    assert stage.outs[0].hash_info.value == expected_hash
 
     assert stage.outs[0].meta.size == size
     assert stage.outs[0].meta.nfiles == 3
     assert stage.outs[0].meta.isdir
 
 
 def test_pull_import_no_download_rev_lock(
```

### Comparing `dvc-3.0.0a2/tests/func/test_import_url.py` & `dvc-3.1.0/tests/func/test_import_url.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,30 +59,14 @@
 
     # force override
     ret = main(["import-url", "foo", "bar", "--force"])
     assert ret == 0
     assert os.path.exists("bar.dvc")
 
 
-def test_import_filename(tmp_dir, dvc, cloud):
-    external_source = cloud / "file"
-    (cloud / "file").write_text("content", encoding="utf-8")
-    ret = main(["import-url", "--file", "bar.dvc", external_source.fs_path])
-    assert ret == 0
-    assert (tmp_dir / "bar.dvc").exists()
-
-    (tmp_dir / "bar.dvc").unlink()
-    (tmp_dir / "sub").mkdir()
-
-    path = tmp_dir / "sub" / "bar.dvc"
-    ret = main(["import-url", "--file", path.fs_path, external_source.fs_path, "out"])
-    assert ret == 0
-    assert path.exists()
-
-
 @pytest.mark.parametrize("dname", [".", "dir", "dir/subdir"])
 def test_import_url_to_dir(dname, tmp_dir, dvc):
     tmp_dir.gen({"data_dir": {"file": "file content"}})
     src = os.path.join("data_dir", "file")
 
     os.makedirs(dname, exist_ok=True)
 
@@ -120,15 +104,15 @@
     dst = tmp_dir / "file"
     assert not dst.exists()
 
 
 class TestImport(_TestImport):
     @pytest.fixture
     def stage_md5(self):
-        return "dc24e1271084ee317ac3c2656fb8812b"
+        return "7033ee831f78a4dfec2fc71405516067"
 
     @pytest.fixture
     def dir_md5(self):
         return "b6dcab6ccd17ca0a8bf4a215a37d14cc.dir"
 
     @pytest.fixture
     def is_object_storage(self):
@@ -162,27 +146,29 @@
         """\
         # top comment
         desc: top desc
         deps:
         - path: foo # dep comment
           md5: acbd18db4cc2f85cedef654fccc4a4d8
           size: 3
+          hash: md5
         outs:
         - path: bar # out comment
           desc: out desc
           type: mytype
           labels:
           - label1
           - label2
           meta:
             key: value
           md5: acbd18db4cc2f85cedef654fccc4a4d8
           size: 3
+          hash: md5
         meta: some metadata
-        md5: be7ade0aa89cc8d56e320867a9de9740
+        md5: 8fc199641730e3f512deac0bd9a0e0b6
         frozen: true
     """
     )
 
 
 def test_import_url_to_remote_absolute(tmp_dir, make_tmp_dir, dvc, local_remote):
     tmp_abs_dir = make_tmp_dir("abs")
@@ -242,16 +228,17 @@
     dst = tmp_dir / "file"
     dvc.imp_url("remote://workspace/file", os.fspath(dst), no_download=True)
 
     dvc.pull(["file.dvc"])
 
     assert dst.exists()
 
-    stage = load_file(dvc, "file.dvc").stage
+    dvc.commit(force=True)
 
+    stage = load_file(dvc, "file.dvc").stage
     assert stage.outs[0].hash_info.value == "d10b4c3ff123b26dc068d43a8bef2d23"
     assert stage.outs[0].meta.size == 12
 
 
 def test_import_url_fs_config(tmp_dir, dvc, workspace, mocker):
     import dvc.fs as dvc_fs
```

### Comparing `dvc-3.0.0a2/tests/func/test_init.py` & `dvc-3.1.0/tests/func/test_init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_install.py` & `dvc-3.1.0/tests/func/test_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,17 @@
 
         with dvc.config.edit() as conf:
             conf["remote"]["store"] = {"url": os.fspath(storage_path)}
             conf["core"]["remote"] = "store"
         tmp_dir.dvc_gen("file", "file_content", "commit message")
 
         file_checksum = file_md5("file", dvc.fs)
-        expected_storage_path = storage_path / file_checksum[:2] / file_checksum[2:]
+        expected_storage_path = (
+            storage_path / "files" / "md5" / file_checksum[:2] / file_checksum[2:]
+        )
 
         scm.gitpython.repo.clone(os.fspath(git_remote))
         scm.gitpython.repo.create_remote("origin", os.fspath(git_remote))
 
         dvc.install()
 
         assert not expected_storage_path.is_file()
@@ -112,14 +114,15 @@
     # NOTE: dvc shouldn't checkout automatically as it might take a long time
     assert (tmp_dir / "data").read_text() == {"bar": "bar"}
     assert (tmp_dir / "data.dvc").read_text() == (
         "outs:\n"
         "- md5: 5ea40360f5b4ec688df672a4db9c17d1.dir\n"
         "  size: 6\n"
         "  nfiles: 2\n"
+        "  hash: md5\n"
         "  path: data\n"
     )
 
     dvc.checkout("data.dvc")
     assert (tmp_dir / "data").read_text() == {"foo": "foo", "bar": "bar"}
 
 
@@ -147,14 +150,15 @@
     # NOTE: dvc shouldn't checkout automatically as it might take a long time
     assert (tmp_dir / "data").read_text() == {"master": "master", "two": "two"}
     assert (tmp_dir / "data.dvc").read_text() == (
         "outs:\n"
         "- md5: 839ef9371606817569c1ee0e5f4ed233.dir\n"
         "  size: 12\n"
         "  nfiles: 3\n"
+        "  hash: md5\n"
         "  path: data\n"
     )
 
     dvc.checkout("data.dvc")
     assert (tmp_dir / "data").read_text() == {
         "master": "master",
         "one": "one",
```

### Comparing `dvc-3.0.0a2/tests/func/test_lock.py` & `dvc-3.1.0/tests/func/test_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_lockfile.py` & `dvc-3.1.0/tests/func/test_lockfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,20 @@
     initial_content = read_lock_file()
     lock = initial_content["stages"]["copy-first-line"]
 
     # lock stage key order:
     assert list(lock.keys()) == ["cmd", "deps", "outs"]
 
     # `path` key appear first and then the `md5`
-    assert all(list(dep.keys()) == ["path", "md5", "size"] for dep in lock["deps"])
-    assert all(list(out.keys()) == ["path", "md5", "size"] for out in lock["outs"])
+    assert all(
+        list(dep.keys()) == ["path", "hash", "md5", "size"] for dep in lock["deps"]
+    )
+    assert all(
+        list(out.keys()) == ["path", "hash", "md5", "size"] for out in lock["outs"]
+    )
 
     # deps are always sorted by the file path naming
     assert list(map(itemgetter("path"), lock["deps"])) == sorted(deps)
 
     # outs are too
     assert list(map(itemgetter("path"), lock["outs"])) == [
         d + "-1" for d in sorted(deps)
```

### Comparing `dvc-3.0.0a2/tests/func/test_ls.py` & `dvc-3.1.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_merge_driver.py` & `dvc-3.1.0/tests/func/test_merge_driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,18 +123,24 @@
 
     assert error in caplog.text
 
 
 def test_merge_different_output_options(tmp_dir, dvc, caplog):
     (tmp_dir / "ancestor").touch()
 
-    (tmp_dir / "our").write_text("outs:\n- md5: f123456789.dir\n  path: path\n")
+    (tmp_dir / "our").write_text(
+        "outs:\n- md5: f123456789.dir\n  hash: md5\n  path: path\n"
+    )
 
     (tmp_dir / "their").write_text(
-        "outs:\n- md5: f987654321.dir\n  path: path\n  cache: false\n"
+        "outs:\n"
+        "- md5: f987654321.dir\n"
+        "  hash: md5\n"
+        "  path: path\n"
+        "  cache: false\n"
     )
 
     assert (
         main(
             [
                 "git-hook",
                 "merge-driver",
@@ -152,17 +158,21 @@
     error = "unable to auto-merge outputs with different options"
     assert error in caplog.text
 
 
 def test_merge_file(tmp_dir, dvc, caplog):
     (tmp_dir / "ancestor").touch()
 
-    (tmp_dir / "our").write_text("outs:\n- md5: f123456789.dir\n  path: path\n")
+    (tmp_dir / "our").write_text(
+        "outs:\n- md5: f123456789.dir\n  hash: md5\n  path: path\n"
+    )
 
-    (tmp_dir / "their").write_text("outs:\n- md5: f987654321\n  path: path\n")
+    (tmp_dir / "their").write_text(
+        "outs:\n- md5: f987654321\n  hash: md5\n  path: path\n"
+    )
 
     assert (
         main(
             [
                 "git-hook",
                 "merge-driver",
                 "--ancestor",
@@ -182,20 +192,24 @@
 
 def test_merge_non_dvc_add(tmp_dir, dvc, caplog):
     (tmp_dir / "ancestor").touch()
 
     (tmp_dir / "our").write_text(
         "outs:\n"
         "- md5: f123456789.dir\n"
+        "  hash: md5\n"
         "  path: path\n"
         "- md5: ff123456789.dir\n"
+        "  hash: md5\n"
         "  path: another\n"
     )
 
-    (tmp_dir / "their").write_text("outs:\n- md5: f987654321\n  path: path\n")
+    (tmp_dir / "their").write_text(
+        "outs:\n- md5: f987654321\n  hash: md5\n  path: path\n"
+    )
 
     assert (
         main(
             [
                 "git-hook",
                 "merge-driver",
                 "--ancestor",
```

### Comparing `dvc-3.0.0a2/tests/func/test_move.py` & `dvc-3.1.0/tests/func/test_move.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,12 +190,13 @@
     dvc.move("foo", "bar")
     res = (tmp_dir / "bar.dvc").read_text()
     assert res == textwrap.dedent(
         """\
         outs:
         - md5: acbd18db4cc2f85cedef654fccc4a4d8
           size: 3
+          hash: md5
           path: bar
         meta:
           custom_key: 42
     """
     )
```

### Comparing `dvc-3.0.0a2/tests/func/test_odb.py` & `dvc-3.1.0/tests/func/test_odb.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,25 +77,14 @@
         }
     )
 
     assert not os.path.exists(".dvc/cache")
     assert len(os.listdir(cache_dir)) != 0
 
 
-def test_remote_cache_references(tmp_dir, dvc):
-    with dvc.config.edit() as conf:
-        conf["remote"]["storage"] = {"url": "ssh://user@localhost:23"}
-        conf["remote"]["cache"] = {"url": "remote://storage/tmp"}
-        conf["cache"]["ssh"] = "cache"
-
-    dvc.cache = CacheManager(dvc)
-
-    assert dvc.cache.ssh.path == "/tmp"
-
-
 def test_shared_cache_dir(tmp_dir):
     cache_dir = os.path.abspath(os.path.join(os.curdir, "cache"))
     for d in ["dir1", "dir2"]:
         os.mkdir(d)
         with (tmp_dir / d).chdir():
             ret = main(["init", "--no-scm"])
             assert ret == 0
@@ -109,21 +98,21 @@
 
             ret = main(["add", "common", "unique"])
             assert ret == 0
 
     assert not os.path.exists(os.path.join("dir1", ".dvc", "cache"))
     assert not os.path.exists(os.path.join("dir2", ".dvc", "cache"))
     assert os.path.exists(
-        os.path.join(cache_dir, "dc", "f6c2fa538b445a3a095255c3641dfc")
+        os.path.join(cache_dir, "files", "md5", "dc", "f6c2fa538b445a3a095255c3641dfc")
     )
     assert os.path.exists(
-        os.path.join(cache_dir, "b4", "333c8cfa2ebba7ef20ec6c3265902b")
+        os.path.join(cache_dir, "files", "md5", "b4", "333c8cfa2ebba7ef20ec6c3265902b")
     )
     assert os.path.exists(
-        os.path.join(cache_dir, "9e", "fab2399c7c560b34de477b9aa0a465")
+        os.path.join(cache_dir, "files", "md5", "9e", "fab2399c7c560b34de477b9aa0a465")
     )
 
 
 def test_cache_link_type(tmp_dir, scm, dvc):
     with dvc.config.edit() as conf:
         conf["cache"]["type"] = "reflink,copy"
     dvc.cache = CacheManager(dvc)
@@ -161,15 +150,15 @@
     rel = os.path.join("..", dname)
     config = configobj.ConfigObj(dvc.config.files["repo"])
     assert config["cache"]["dir"] == rel.replace("\\", "/")
 
     tmp_dir.dvc_gen({"foo": "foo"})
 
     assert os.path.exists(
-        os.path.join(cache_dir, "ac", "bd18db4cc2f85cedef654fccc4a4d8")
+        os.path.join(cache_dir, "files", "md5", "ac", "bd18db4cc2f85cedef654fccc4a4d8")
     )
 
 
 def test_default_cache_type(dvc):
     assert dvc.cache.local.cache_types == ["reflink", "copy"]
```

### Comparing `dvc-3.0.0a2/tests/func/test_remote.py` & `dvc-3.1.0/tests/func/test_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import errno
 import itertools
 import os
 import stat
-from unittest.mock import patch
 
 import configobj
 import pytest
 
 from dvc.cli import main
 from dvc.config import Config
-from dvc.exceptions import DownloadError, RemoteCacheRequiredError, UploadError
+from dvc.exceptions import DownloadError, UploadError
 from dvc.utils.fs import remove
 
 
 def test_remote(dvc):
     remotes = ["a", "b", "c"]
 
     assert main(["remote", "list"]) == 0
@@ -124,42 +123,45 @@
     ret = main(["remote", "add", remote_name, local_cloud.url])
     assert ret == 0
 
     ret = main(["push", "-r", remote_name])
     assert ret == 0
 
 
-def test_dir_hash_should_be_key_order_agnostic(tmp_dir, dvc):
+def test_dir_hash_should_be_key_order_agnostic(tmp_dir, dvc, mocker):
     from dvc_data.hashfile.build import build
     from dvc_data.hashfile.tree import Tree
 
     tmp_dir.gen({"data": {"1": "1 content", "2": "2 content"}})
 
     path = (tmp_dir / "data").fs_path
 
     tree = Tree.from_list([{"relpath": "1", "md5": "1"}, {"relpath": "2", "md5": "2"}])
     tree.digest()
-    with patch("dvc_data.hashfile.build._build_tree", return_value=(None, tree)):
-        _, _, obj = build(dvc.cache.local, path, dvc.cache.local.fs, "md5")
-        hash1 = obj.hash_info
+
+    mocker.patch("dvc_data.hashfile.build._build_tree", return_value=(None, tree))
+
+    _, _, obj = build(dvc.cache.local, path, dvc.cache.local.fs, "md5")
+    hash1 = obj.hash_info
 
     # remove the raw dir obj to force building the tree on the next build call
     dvc.cache.local.fs.remove(dvc.cache.local.oid_to_path(hash1.as_raw().value))
 
     tree = Tree.from_list([{"md5": "1", "relpath": "1"}, {"md5": "2", "relpath": "2"}])
     tree.digest()
-    with patch("dvc_data.hashfile.build._build_tree", return_value=(None, tree)):
-        _, _, obj = build(dvc.cache.local, path, dvc.cache.local.fs, "md5")
-        hash2 = obj.hash_info
+
+    # NOTE: _build_tree already patched above
+    _, _, obj = build(dvc.cache.local, path, dvc.cache.local.fs, "md5")
+    hash2 = obj.hash_info
 
     assert hash1 == hash2
 
 
 def test_partial_push_n_pull(  # noqa: C901
-    tmp_dir, dvc, tmp_path_factory, local_remote
+    tmp_dir, dvc, tmp_path_factory, local_remote, mocker
 ):
     from dvc_objects.fs import generic
 
     foo = tmp_dir.dvc_gen({"foo": "foo content"})[0].outs[0]
     bar = tmp_dir.dvc_gen({"bar": "bar content"})[0].outs[0]
     baz = tmp_dir.dvc_gen({"baz": {"foo": "foo content"}})[0].outs[0]
 
@@ -186,22 +188,23 @@
             ):
                 if on_error:
                     on_error(from_i, to_i, Exception("stop foo"))
                 del from_info[i]
                 del to_info[i]
         return original(from_fs, from_info, to_fs, to_info, **kwargs)
 
-    with patch.object(generic, "transfer", unreliable_upload):
-        with pytest.raises(UploadError) as upload_error_info:
-            dvc.push()
-        assert upload_error_info.value.amount == 2
-
-        assert not odb.exists(foo.hash_info.value)
-        assert odb.exists(bar.hash_info.value)
-        assert not odb.exists(baz.hash_info.value)
+    mock_upload = mocker.patch.object(generic, "transfer", unreliable_upload)
+    with pytest.raises(UploadError) as upload_error_info:
+        dvc.push()
+    assert upload_error_info.value.amount == 2
+
+    assert not odb.exists(foo.hash_info.value)
+    assert odb.exists(bar.hash_info.value)
+    assert not odb.exists(baz.hash_info.value)
+    mocker.stop(mock_upload)
 
     # Push everything and delete local cache
     dvc.push()
     dvc.cache.local.clear()
 
     baz._collect_used_dir_cache()
 
@@ -211,20 +214,21 @@
         if isinstance(from_info, str):
             from_info = [from_info]
         if isinstance(to_info, str):
             to_info = [to_info]
         for from_i, to_i in zip(from_info, to_info):
             on_error(from_i, to_i, Exception())
 
-    with patch.object(generic, "transfer", unreliable_download):
-        with pytest.raises(DownloadError) as download_error_info:
-            dvc.pull()
-        # error count should be len(.dir + standalone file checksums)
-        # since files inside dir are ignored if dir cache entry is missing
-        assert download_error_info.value.amount == 2
+    mock_download = mocker.patch.object(generic, "transfer", unreliable_download)
+    with pytest.raises(DownloadError) as download_error_info:
+        dvc.pull()
+    # error count should be len(.dir + standalone file checksums)
+    # since files inside dir are ignored if dir cache entry is missing
+    assert download_error_info.value.amount == 2
+    mocker.stop(mock_download)
 
 
 def test_raise_on_too_many_open_files(
     tmp_dir, dvc, tmp_path_factory, mocker, local_remote
 ):
     tmp_dir.dvc_gen({"file": "file content"})
 
@@ -253,30 +257,14 @@
     assert dvc.config["remote"]["myremote"] == {
         "url": "http://example.com/path",
         "user": "xxx",
         "verify": False,
     }
 
 
-def test_external_dir_resource_on_no_cache(tmp_dir, dvc, tmp_path_factory):
-    # https://github.com/iterative/dvc/issues/2647, is some situations
-    # (external dir dependency) cache is required to calculate dir md5
-    external_dir = tmp_path_factory.mktemp("external_dir")
-    file = external_dir / "file"
-
-    dvc.cache.local = None
-    with pytest.raises(RemoteCacheRequiredError):
-        dvc.run(
-            cmd=f"echo content > {file}",
-            outs=[os.fspath(file)],
-            name="echo",
-            external=True,
-        )
-
-
 def test_push_order(tmp_dir, dvc, tmp_path_factory, mocker, local_remote):
     from dvc_objects.fs import generic
 
     foo = tmp_dir.dvc_gen({"foo": {"bar": "bar content"}})[0].outs[0]
     tmp_dir.dvc_gen({"baz": "baz content"})
 
     mocked_upload = mocker.spy(generic, "transfer")
```

### Comparing `dvc-3.0.0a2/tests/func/test_remove.py` & `dvc-3.1.0/tests/func/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_repo.py` & `dvc-3.1.0/tests/func/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_repo_index.py` & `dvc-3.1.0/tests/func/test_repo_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,56 +139,47 @@
 
     # check that our hack can be disabled
     dvc._skip_graph_checks = False
     Index(dvc).check_graph()
     assert mock_build_graph.called
 
 
-def get_index(dvc, rev):
-    if rev:
-        brancher = dvc.brancher(revs=[rev])
-        if rev != "workspace":
-            assert next(brancher) == "workspace"
-        next(brancher)
-    return Index.from_repo(dvc)
-
-
-@pytest.mark.parametrize("rev", ["workspace", "HEAD"])
-def test_used_objs(tmp_dir, scm, dvc, run_copy, rev):
+def test_used_objs(tmp_dir, scm, dvc, run_copy):
     from dvc_data.hashfile.hash_info import HashInfo
 
     dvc.scm_context.autostage = True
     tmp_dir.dvc_gen({"dir": {"subdir": {"file": "file"}}, "foo": "foo"})
     run_copy("foo", "bar", name="copy-foo-bar")
     scm.commit("commit")
 
-    index = get_index(dvc, rev)
-
-    expected_objs = [
-        HashInfo(
-            name="md5",
-            value="acbd18db4cc2f85cedef654fccc4a4d8",
-            obj_name="bar",
-        ),
-        HashInfo(
-            name="md5",
-            value="8c7dd922ad47494fc02c388e12c00eac",
-            obj_name="dir/subdir/file",
-        ),
-        HashInfo(
-            name="md5",
-            value="d28c9e28591aeb7e303dc6772ffa6f6b.dir",
-            obj_name="dir",
-        ),
-    ]
-
-    assert index.used_objs() == {None: set(expected_objs)}
-    assert index.used_objs("dir") == {None: set(expected_objs[1:])}
-    assert index.used_objs(".", recursive=True) == {None: set(expected_objs)}
-    assert index.used_objs("copy-foo-bar", with_deps=True) == {None: {expected_objs[0]}}
+    for _ in dvc.brancher(revs=["HEAD"]):
+        expected_objs = [
+            HashInfo(
+                name="md5",
+                value="acbd18db4cc2f85cedef654fccc4a4d8",
+                obj_name="bar",
+            ),
+            HashInfo(
+                name="md5",
+                value="8c7dd922ad47494fc02c388e12c00eac",
+                obj_name="dir/subdir/file",
+            ),
+            HashInfo(
+                name="md5",
+                value="d28c9e28591aeb7e303dc6772ffa6f6b.dir",
+                obj_name="dir",
+            ),
+        ]
+
+        assert dvc.index.used_objs() == {None: set(expected_objs)}
+        assert dvc.index.used_objs("dir") == {None: set(expected_objs[1:])}
+        assert dvc.index.used_objs(".", recursive=True) == {None: set(expected_objs)}
+        assert dvc.index.used_objs("copy-foo-bar", with_deps=True) == {
+            None: {expected_objs[0]}
+        }
 
 
 def test_view_granular_dir(tmp_dir, scm, dvc, run_copy):
     tmp_dir.dvc_gen(
         {"dir": {"subdir": {"in-subdir": "in-subdir"}, "in-dir": "in-dir"}},
         commit="init",
     )
```

### Comparing `dvc-3.0.0a2/tests/func/test_repro.py` & `dvc-3.1.0/tests/func/repro/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_run.py` & `dvc-3.1.0/tests/func/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -530,26 +530,27 @@
     bar_hash = "37b51d194a7513e45b56f6524f2d51f2"
 
     local_workspace.gen("foo", "foo")
     dvc.run(
         name="mystage",
         cmd="mycmd",
         deps=["remote://workspace/foo"],
-        outs=["remote://workspace/bar"],
+        outs_no_cache=["remote://workspace/bar"],
         no_exec=True,
     )
 
     dvc_yaml = (
         "stages:\n"
         "  mystage:\n"
         "    cmd: mycmd\n"
         "    deps:\n"
         "    - remote://workspace/foo\n"
         "    outs:\n"
-        "    - remote://workspace/bar\n"
+        "    - remote://workspace/bar:\n"
+        "        cache: false\n"
     )
 
     assert (tmp_dir / "dvc.yaml").read_text() == dvc_yaml
     assert not (tmp_dir / "dvc.lock").exists()
 
     local_workspace.gen("bar", "bar")
     dvc.commit("dvc.yaml", force=True)
@@ -558,27 +559,27 @@
     assert (tmp_dir / "dvc.lock").read_text() == (
         "schema: '2.0'\n"
         "stages:\n"
         "  mystage:\n"
         "    cmd: mycmd\n"
         "    deps:\n"
         "    - path: remote://workspace/foo\n"
+        "      hash: md5\n"
         f"      {hash_name}: {foo_hash}\n"
         "      size: 3\n"
         "    outs:\n"
         "    - path: remote://workspace/bar\n"
+        "      hash: md5\n"
         f"      {hash_name}: {bar_hash}\n"
         "      size: 3\n"
     )
 
     assert (local_workspace / "foo").read_text() == "foo"
     assert (local_workspace / "bar").read_text() == "bar"
-    assert (
-        local_workspace / "cache" / bar_hash[:2] / bar_hash[2:]
-    ).read_text() == "bar"
+    assert not (local_workspace / "cache").exists()
 
 
 def test_rerun_callback(dvc):
     def run_callback(force=False):
         return dvc.run(cmd="echo content > out", force=force, name="echo")
 
     assert run_callback() is not None
```

### Comparing `dvc-3.0.0a2/tests/func/test_run_cache.py` & `dvc-3.1.0/tests/func/test_run_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_scm.py` & `dvc-3.1.0/tests/func/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_scm_context.py` & `dvc-3.1.0/tests/func/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_stage.py` & `dvc-3.1.0/tests/func/test_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,39 +135,51 @@
     data = {
         "desc": "stage desc",
         "meta": {"key1": "value1", "key2": "value2"},
         "outs": [
             {
                 "md5": "d3b07384d113edec49eaa6238ad5ff00",
                 "size": 4,
+                "hash": "md5",
                 "path": "foo",
                 "desc": "foo desc",
                 "type": "mytype",
                 "labels": ["get-started", "dataset-registry"],
                 "meta": {"key1": "value1"},
             }
         ],
     }
     (tmp_dir / "foo.dvc").dump(data)
     stage = dvc.stage.load_one("foo.dvc")
-    assert compute_md5(stage) == "1822617147b53ae6f9eb4b3c87c0b6f3"
+    assert compute_md5(stage) == "cde267b60ef5a00e9a35cc1999ab83a3"
     assert (
-        dict_md5({"outs": [{"md5": "d3b07384d113edec49eaa6238ad5ff00", "path": "foo"}]})
-        == "1822617147b53ae6f9eb4b3c87c0b6f3"
+        dict_md5(
+            {
+                "outs": [
+                    {
+                        "md5": "d3b07384d113edec49eaa6238ad5ff00",
+                        "hash": "md5",
+                        "path": "foo",
+                    }
+                ]
+            }
+        )
+        == "cde267b60ef5a00e9a35cc1999ab83a3"
     )
 
 
 def test_meta_desc_is_preserved(tmp_dir, dvc):
     data = {
         "desc": "stage desc",
         "meta": {"key1": "value1", "key2": "value2"},
         "outs": [
             {
                 "md5": "d3b07384d113edec49eaa6238ad5ff00",
                 "size": 4,
+                "hash": "md5",
                 "path": "foo",
                 "desc": "foo desc",
                 "type": "mytype",
                 "labels": ["get-started", "dataset-registry"],
                 "meta": {"key": "value"},
             }
         ],
```

### Comparing `dvc-3.0.0a2/tests/func/test_stage_load.py` & `dvc-3.1.0/tests/func/test_stage_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_state.py` & `dvc-3.1.0/tests/func/test_state.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_status.py` & `dvc-3.1.0/tests/func/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_unprotect.py` & `dvc-3.1.0/tests/func/test_unprotect.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 
 def test_unprotect(tmp_dir, dvc):
     tmp_dir.gen("foo", "foo")
 
     dvc.cache.local.cache_types = ["hardlink"]
     dvc.add("foo")
-    cache = os.path.join(".dvc", "cache", "ac", "bd18db4cc2f85cedef654fccc4a4d8")
+    cache = os.path.join(
+        ".dvc", "cache", "files", "md5", "ac", "bd18db4cc2f85cedef654fccc4a4d8"
+    )
     assert not os.access("foo", os.W_OK)
     assert not os.access(cache, os.W_OK)
 
     dvc.unprotect("foo")
     assert os.access("foo", os.W_OK)
 
     if os.name == "nt":
```

### Comparing `dvc-3.0.0a2/tests/func/test_update.py` & `dvc-3.1.0/tests/func/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_used_objs.py` & `dvc-3.1.0/tests/func/test_used_objs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_utils.py` & `dvc-3.1.0/tests/func/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_version.py` & `dvc-3.1.0/tests/func/test_version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/test_virtual_directory.py` & `dvc-3.1.0/tests/func/test_virtual_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     assert dvc.push() == 3
     dvc.cache.local.clear()
     shutil.rmtree("dir")
 
     assert dvc.pull("dir/subdir") == M.dict(
         added=[join("dir", "")],
-        fetched=1,
+        fetched=3,
     )
     assert (tmp_dir / "dir").read_text() == {"subdir": {"lorem": "lorem"}}
 
     tmp_dir.gen({"dir": {"subdir": {"ipsum": "ipsum"}}})
     (stage,) = dvc.add("dir/subdir/ipsum")
 
     out = stage.outs[0]
```

### Comparing `dvc-3.0.0a2/tests/func/utils/test_hydra.py` & `dvc-3.1.0/tests/func/utils/test_hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/func/utils/test_strict_yaml.py` & `dvc-3.1.0/tests/func/utils/test_strict_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/integration/plots/conftest.py` & `dvc-3.1.0/tests/integration/plots/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/integration/plots/test_plots.py` & `dvc-3.1.0/tests/integration/plots/test_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,15 @@
         _, json_result, split_json_result = call(capsys, subcommand=s)
         errors = [
             {
                 "name": p,
                 "source": p,
                 "rev": "workspace",
                 "type": "FileNotFoundError",
-                "msg": "",
+                "msg": f"[Errno 2] No storage files available: '{p}'",
             }
             for p in [
                 "linear.json",
                 "confusion.json",
                 "image.png",
             ]
         ]
```

### Comparing `dvc-3.0.0a2/tests/integration/plots/test_repo_plots_api.py` & `dvc-3.1.0/tests/integration/plots/test_repo_plots_api.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/integration/test_studio_live_experiments.py` & `dvc-3.1.0/tests/integration/test_studio_live_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/remotes/git_server.py` & `dvc-3.1.0/tests/remotes/git_server.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/remotes/user.key` & `dvc-3.1.0/tests/remotes/user.key`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/remotes_env.sample` & `dvc-3.1.0/tests/remotes_env.sample`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/scripts.py` & `dvc-3.1.0/tests/scripts.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import shutil
 import sys
 
 if os.path.isfile(sys.argv[1]):
     shutil.copyfile(sys.argv[1], sys.argv[2])
 else:
     shutil.copytree(sys.argv[1], sys.argv[2])
-"""
+""".replace(
+    "\r\n", "\n"
+)
 
 
 def _add_script(tmp_dir, path, contents=""):
-    script, *_ = tmp_dir.gen(path, contents)
+    script, *_ = tmp_dir.gen(path, contents.encode("utf-8"))
     if hasattr(tmp_dir, "scm"):
         tmp_dir.scm_add(path, commit=f"add {path}")
     return script.fs_path
 
 
 @pytest.fixture
 def append_foo_script(tmp_dir):
@@ -26,15 +28,17 @@
         "append_foo.py",
         """
 import sys
 from pathlib import Path
 
 with Path(sys.argv[1]).open("a+", encoding="utf-8") as f:
     f.write("foo")
-""",
+""".replace(
+            "\r\n", "\n"
+        ),
     )
 
 
 @pytest.fixture
 def copy_script(
     tmp_dir,
 ):
@@ -51,9 +55,11 @@
         tmp_dir,
         "head.py",
         """
 import sys
 for file in sys.argv[1:]:
     with open(file) as f, open(file +"-1","w+") as w:
         w.write(f.readline())
-""",
+""".replace(
+            "\r\n", "\n"
+        ),
     )
```

### Comparing `dvc-3.0.0a2/tests/unit/cli/test_main.py` & `dvc-3.1.0/tests/unit/cli/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         (None, "Please report this bug to"),
         ("pip", "pip install 'dvc[proto]'"),
         ("conda", "conda install -c conda-forge dvc-proto"),
     ],
 )
 def test_remote_missing_deps_are_correctly_reported(tmp_dir, caplog, mocker, pkg, msg):
     error = RemoteMissingDepsError(FileSystem(), "proto", "proto://", ["deps"])
-    mocker.patch("dvc.utils.pkg.PKG", pkg)
+    mocker.patch("dvc.PKG", pkg)
     mocker.patch(
         "dvc.cli.parse_args",
         return_value=Namespace(
             func=raiser(error),
             quiet=False,
             verbose=True,
         ),
```

### Comparing `dvc-3.0.0a2/tests/unit/command/ls/test_ls.py` & `dvc-3.1.0/tests/unit/command/ls/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/ls/test_ls_colors.py` & `dvc-3.1.0/tests/unit/command/ls/test_ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_add.py` & `dvc-3.1.0/tests/unit/command/test_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 
 def test_add(mocker, dvc):
     cli_args = parse_args(
         [
             "add",
             "--no-commit",
-            "--external",
             "--glob",
             "data",
         ]
     )
     assert cli_args.func == CmdAdd
 
     cmd = cli_args.func(cli_args)
@@ -21,15 +20,14 @@
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         ["data"],
         no_commit=True,
         glob=True,
-        external=True,
         out=None,
         remote=None,
         to_remote=False,
         remote_jobs=None,
         force=False,
     )
 
@@ -53,15 +51,14 @@
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         ["s3://bucket/foo"],
         no_commit=False,
         glob=False,
-        external=False,
         out="bar",
         remote="remote",
         to_remote=True,
         remote_jobs=None,
         force=False,
     )
```

### Comparing `dvc-3.0.0a2/tests/unit/command/test_cache.py` & `dvc-3.1.0/tests/unit/command/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_checkout.py` & `dvc-3.1.0/tests/unit/command/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_compat_flag.py` & `dvc-3.1.0/tests/unit/command/test_compat_flag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_config.py` & `dvc-3.1.0/tests/unit/command/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_dag.py` & `dvc-3.1.0/tests/unit/command/test_dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_data_status.py` & `dvc-3.1.0/tests/unit/command/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_data_sync.py` & `dvc-3.1.0/tests/unit/command/test_data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_diff.py` & `dvc-3.1.0/tests/unit/command/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_experiments.py` & `dvc-3.1.0/tests/unit/command/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_gc.py` & `dvc-3.1.0/tests/unit/command/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_get.py` & `dvc-3.1.0/tests/unit/command/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_git_hook.py` & `dvc-3.1.0/tests/unit/command/test_git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_imp.py` & `dvc-3.1.0/tests/unit/command/test_imp.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,14 @@
     cli_args = parse_args(
         [
             "import",
             "repo_url",
             "src",
             "--out",
             "out",
-            "--file",
-            "file",
             "--rev",
             "version",
             "--jobs",
             "3",
         ]
     )
     assert cli_args.func == CmdImport
@@ -25,15 +23,14 @@
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         "repo_url",
         path="src",
         out="out",
-        fname="file",
         rev="version",
         no_exec=False,
         no_download=False,
         jobs=3,
     )
 
 
@@ -41,16 +38,14 @@
     cli_args = parse_args(
         [
             "import",
             "repo_url",
             "src",
             "--out",
             "out",
-            "--file",
-            "file",
             "--rev",
             "version",
             "--no-exec",
         ]
     )
 
     cmd = cli_args.func(cli_args)
@@ -58,15 +53,14 @@
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         "repo_url",
         path="src",
         out="out",
-        fname="file",
         rev="version",
         no_exec=True,
         no_download=False,
         jobs=None,
     )
 
 
@@ -74,16 +68,14 @@
     cli_args = parse_args(
         [
             "import",
             "repo_url",
             "src",
             "--out",
             "out",
-            "--file",
-            "file",
             "--rev",
             "version",
             "--no-download",
         ]
     )
 
     cmd = cli_args.func(cli_args)
@@ -91,13 +83,12 @@
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         "repo_url",
         path="src",
         out="out",
-        fname="file",
         rev="version",
         no_exec=False,
         no_download=True,
         jobs=None,
     )
```

### Comparing `dvc-3.0.0a2/tests/unit/command/test_imp_url.py` & `dvc-3.1.0/tests/unit/command/test_imp_url.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,31 +9,28 @@
 
 def test_import_url(mocker):
     cli_args = parse_args(
         [
             "import-url",
             "src",
             "out",
-            "--file",
-            "file",
             "--jobs",
             "4",
         ]
     )
     assert cli_args.func == CmdImportUrl
 
     cmd = cli_args.func(cli_args)
     m = mocker.patch.object(cmd.repo, "imp_url", autospec=True)
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         "src",
         out="out",
-        fname="file",
         no_exec=False,
         no_download=False,
         remote=None,
         to_remote=False,
         jobs=4,
         force=False,
         version_aware=False,
@@ -66,28 +63,25 @@
 def test_import_url_no_exec_download_flags(mocker, flag, expected):
     cli_args = parse_args(
         [
             "import-url",
             flag,
             "src",
             "out",
-            "--file",
-            "file",
         ]
     )
 
     cmd = cli_args.func(cli_args)
     m = mocker.patch.object(cmd.repo, "imp_url", autospec=True)
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         "src",
         out="out",
-        fname="file",
         remote=None,
         to_remote=False,
         jobs=None,
         force=False,
         version_aware=False,
         **expected,
     )
@@ -110,15 +104,14 @@
     m = mocker.patch.object(cmd.repo, "imp_url", autospec=True)
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         "s3://bucket/foo",
         out="bar",
-        fname=None,
         no_exec=False,
         no_download=False,
         remote="remote",
         to_remote=True,
         jobs=None,
         force=False,
         version_aware=False,
```

### Comparing `dvc-3.0.0a2/tests/unit/command/test_ls_url.py` & `dvc-3.1.0/tests/unit/command/test_ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_machine.py` & `dvc-3.1.0/tests/unit/command/test_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from unittest.mock import call
 
 import configobj
 import pytest
 
 from dvc.cli import parse_args
 from dvc.commands.machine import (
     CmdMachineAdd,
@@ -73,15 +72,15 @@
     m.assert_called_once_with("foo")
 
     cli_args = parse_args(["machine", "status"])
     cmd = cli_args.func(cli_args)
     m = mocker.patch.object(cmd.repo.machine, "status", autospec=True, return_value=[])
     assert cmd.run() == 0
     assert m.call_count == 2
-    m.assert_has_calls([call("foo"), call("myaws")])
+    m.assert_has_calls([mocker.call("foo"), mocker.call("myaws")])
 
 
 def test_destroy(tmp_dir, dvc, mocker):
     cli_args = parse_args(["machine", "destroy", "foo"])
     assert cli_args.func == CmdMachineDestroy
 
     cmd = cli_args.func(cli_args)
```

### Comparing `dvc-3.0.0a2/tests/unit/command/test_metrics.py` & `dvc-3.1.0/tests/unit/command/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_params.py` & `dvc-3.1.0/tests/unit/command/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_plots.py` & `dvc-3.1.0/tests/unit/command/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_queue.py` & `dvc-3.1.0/tests/unit/command/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_repro.py` & `dvc-3.1.0/tests/unit/command/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_stage.py` & `dvc-3.1.0/tests/unit/command/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_status.py` & `dvc-3.1.0/tests/unit/command/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/command/test_update.py` & `dvc-3.1.0/tests/unit/command/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/data/db/test_local.py` & `dvc-3.1.0/tests/unit/data/db/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/dependency/test_params.py` & `dvc-3.1.0/tests/unit/dependency/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/fs/test_azure.py` & `dvc-3.1.0/tests/unit/fs/test_azure.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/fs/test_data.py` & `dvc-3.1.0/tests/unit/fs/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/fs/test_dvc.py` & `dvc-3.1.0/tests/unit/fs/test_dvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import posixpath
 import shutil
-from unittest import mock
 
 import pytest
 
 from dvc.fs import localfs
 from dvc.fs.dvc import DVCFileSystem
 from dvc.testing.tmp_dir import make_subrepo
 from dvc_data.hashfile.build import build
@@ -342,41 +341,43 @@
         def f(*args, **kwargs):
             r = method(*args, **kwargs)
             assert r.root_dir == ret_val.root_dir
             return r
 
         return f
 
-    with mock.patch.object(
+    mock_subrepo1 = mocker.patch.object(
         fs.fs, "_get_repo", side_effect=assert_fs_belongs_to_repo(subrepo1.dvc)
-    ):
-        assert fs.exists("dir/repo/foo") is True
-        assert fs.exists("dir/repo/bar") is False
+    )
+    assert fs.exists("dir/repo/foo") is True
+    assert fs.exists("dir/repo/bar") is False
 
-        assert fs.isfile("dir/repo/foo") is True
-        assert fs.isfile("dir/repo/dir1/bar") is True
-        assert fs.isfile("dir/repo/dir1") is False
-
-        assert fs.isdir("dir/repo/dir1") is True
-        assert fs.isdir("dir/repo/dir1/bar") is False
-        assert fs.isdvc("dir/repo/foo") is True
+    assert fs.isfile("dir/repo/foo") is True
+    assert fs.isfile("dir/repo/dir1/bar") is True
+    assert fs.isfile("dir/repo/dir1") is False
+
+    assert fs.isdir("dir/repo/dir1") is True
+    assert fs.isdir("dir/repo/dir1/bar") is False
+    assert fs.isdvc("dir/repo/foo") is True
+    mocker.stop(mock_subrepo1)
 
-    with mock.patch.object(
+    mock_subrepo2 = mocker.patch.object(
         fs.fs, "_get_repo", side_effect=assert_fs_belongs_to_repo(subrepo2.dvc)
-    ):
-        assert fs.exists("dir/repo2/lorem") is True
-        assert fs.exists("dir/repo2/ipsum") is False
+    )
+    assert fs.exists("dir/repo2/lorem") is True
+    assert fs.exists("dir/repo2/ipsum") is False
 
-        assert fs.isfile("dir/repo2/lorem") is True
-        assert fs.isfile("dir/repo2/dir2/ipsum") is True
-        assert fs.isfile("dir/repo2/dir2") is False
-
-        assert fs.isdir("dir/repo2/dir2") is True
-        assert fs.isdir("dir/repo2/dir2/ipsum") is False
-        assert fs.isdvc("dir/repo2/lorem") is True
+    assert fs.isfile("dir/repo2/lorem") is True
+    assert fs.isfile("dir/repo2/dir2/ipsum") is True
+    assert fs.isfile("dir/repo2/dir2") is False
+
+    assert fs.isdir("dir/repo2/dir2") is True
+    assert fs.isdir("dir/repo2/dir2/ipsum") is False
+    assert fs.isdvc("dir/repo2/lorem") is True
+    mocker.stop(mock_subrepo2)
 
 
 @pytest.mark.parametrize(
     "dvcfiles,extra_expected",
     [
         (False, []),
         (
@@ -538,15 +539,19 @@
             os.path.join("dir", "foo.dvc"),
         ]
     )
     tmp_dir.scm.commit("add dir")
 
     fs = DVCFileSystem(repo=dvc)
     _, _, obj = build(dvc.cache.local, "dir", fs, "md5")
-    assert obj.hash_info == HashInfo("md5", "e1d9e8eae5374860ae025ec84cfd85c7.dir")
+    if os.name == "nt":
+        expected_hash = "0d2086760aea091f1504eafc8843bb18.dir"
+    else:
+        expected_hash = "e1d9e8eae5374860ae025ec84cfd85c7.dir"
+    assert obj.hash_info == HashInfo("md5", expected_hash)
 
 
 def test_get_hash_dirty_file(tmp_dir, dvc):
     from dvc_data.hashfile import check
     from dvc_data.hashfile.hash import hash_file
 
     tmp_dir.dvc_gen("file", "file")
```

### Comparing `dvc-3.0.0a2/tests/unit/fs/test_dvc_info.py` & `dvc-3.1.0/tests/unit/fs/test_dvc_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/fs/test_fs.py` & `dvc-3.1.0/tests/unit/fs/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/fs/test_path.py` & `dvc-3.1.0/tests/unit/fs/test_path.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/fs/test_s3.py` & `dvc-3.1.0/tests/unit/fs/test_s3.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/fs/test_tree.py` & `dvc-3.1.0/tests/unit/fs/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/machine/test_machine.py` & `dvc-3.1.0/tests/unit/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/output/test_load.py` & `dvc-3.1.0/tests/unit/output/test_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/output/test_local.py` & `dvc-3.1.0/tests/unit/output/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/output/test_output.py` & `dvc-3.1.0/tests/unit/output/test_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
             "md5": "acbd18db4cc2f85cedef654fccc4a4d8",
             "relpath": "foo",
         },
     ]
     out = Output(stage, "path", files=files)
 
     dumpd = out.dumpd()
-    assert dumpd == {"path": "path", "files": files}
+    assert dumpd == {"path": "path", "hash": "md5", "files": files}
 
 
 def test_version_aware_is_set_based_on_files(mocker):
     import dvc.fs as dvc_fs
 
     get_fs_config = mocker.spy(dvc_fs, "get_fs_config")
```

### Comparing `dvc-3.0.0a2/tests/unit/remote/test_oss.py` & `dvc-3.1.0/tests/unit/remote/test_oss.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/remote/test_remote.py` & `dvc-3.1.0/tests/unit/remote/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/remote/test_webdav.py` & `dvc-3.1.0/tests/unit/remote/test_webdav.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/remote/test_webhdfs.py` & `dvc-3.1.0/tests/unit/remote/test_webhdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/render/test_convert.py` & `dvc-3.1.0/tests/unit/render/test_convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/render/test_image_converter.py` & `dvc-3.1.0/tests/unit/render/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/render/test_match.py` & `dvc-3.1.0/tests/unit/render/test_match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/render/test_vega_converter.py` & `dvc-3.1.0/tests/unit/render/test_vega_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/experiments/conftest.py` & `dvc-3.1.0/tests/unit/repo/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/experiments/queue/test_celery.py` & `dvc-3.1.0/tests/unit/repo/experiments/queue/test_celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/experiments/queue/test_remove.py` & `dvc-3.1.0/tests/unit/repo/experiments/queue/test_remove.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from unittest.mock import call
-
 from dvc.repo.experiments.queue.base import QueueDoneResult
 
 
 def test_remove_queued(test_queue, mocker):
     queued_test = ["queue1", "queue2", "queue3"]
 
     stash_dict = {}
@@ -33,15 +31,19 @@
     remove_revs_mocker.assert_called_once_with([stash_dict["queue2"]])
     remove_revs_mocker.reset_mock()
     reject_mocker.reset_mock()
 
     assert test_queue.clear(queued=True) == queued_test
     remove_revs_mocker.assert_called_once_with(list(stash_dict.values()))
     reject_mocker.assert_has_calls(
-        [call("msg_queue1"), call("msg_queue2"), call("msg_queue3")]
+        [
+            mocker.call("msg_queue1"),
+            mocker.call("msg_queue2"),
+            mocker.call("msg_queue3"),
+        ]
     )
 
 
 def test_remove_done(test_queue, mocker):
     from funcy import concat
 
     failed_test = ["failed1", "failed2", "failed3"]
@@ -80,27 +82,29 @@
     purge_mocker = mocker.patch.object(test_queue.celery, "purge")
 
     assert test_queue.remove(["failed3", "success2"]) == [
         "failed3",
         "success2",
     ]
     remove_revs_mocker.assert_called_once_with([stash_dict["failed3"]])
-    purge_mocker.assert_has_calls([call("msg_failed3"), call("msg_success2")])
+    purge_mocker.assert_has_calls(
+        [mocker.call("msg_failed3"), mocker.call("msg_success2")]
+    )
 
     remove_revs_mocker.reset_mock()
     purge_mocker.reset_mock()
 
     assert set(test_queue.clear(success=True, failed=True)) == set(failed_test) | set(
         success_test
     )
     purge_mocker.assert_has_calls(
         [
-            call("msg_failed1"),
-            call("msg_failed2"),
-            call("msg_failed3"),
-            call("msg_success1"),
-            call("msg_success2"),
-            call("msg_success3"),
+            mocker.call("msg_failed1"),
+            mocker.call("msg_failed2"),
+            mocker.call("msg_failed3"),
+            mocker.call("msg_success1"),
+            mocker.call("msg_success2"),
+            mocker.call("msg_success3"),
         ],
         any_order=True,
     )
     remove_revs_mocker.assert_called_once_with(list(stash_dict.values()))
```

### Comparing `dvc-3.0.0a2/tests/unit/repo/experiments/test_executor_status.py` & `dvc-3.1.0/tests/unit/repo/experiments/test_executor_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/experiments/test_remove.py` & `dvc-3.1.0/tests/unit/repo/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/experiments/test_utils.py` & `dvc-3.1.0/tests/unit/repo/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/plots/test_diff.py` & `dvc-3.1.0/tests/unit/repo/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/test_open_repo.py` & `dvc-3.1.0/tests/unit/repo/test_open_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from unittest.mock import call
 
 import pytest
 
 from dvc.repo.open_repo import _external_repo as external_repo
 from dvc.testing.tmp_dir import make_subrepo
 
 
@@ -30,15 +29,15 @@
 
         list(repo.dvcfs.walk("", ignore_subrepos=False))  # drain
         assert spy.call_count == len(subrepos)
 
         paths = ["/" + path.replace("\\", "/") for path in subrepo_paths]
         spy.assert_has_calls(
             [
-                call(
+                mocker.call(
                     path,
                     fs=repo.fs,
                     scm=repo.scm,
                     repo_factory=repo.dvcfs.fs.repo_factory,
                 )
                 for path in paths
             ],
@@ -51,15 +50,15 @@
     tmp_dir, scm, mocker, make_tmp_dir, root_is_dvc
 ):
     if root_is_dvc:
         make_subrepo(tmp_dir, scm)
 
     subrepo = tmp_dir / "subrepo"
     make_subrepo(subrepo, scm)
-    local_cache = subrepo.dvc.cache.local.path
+    local_cache = subrepo.dvc.cache.local_cache_dir
 
     tmp_dir.scm_gen("bar", "bar", commit="add bar")
     subrepo.dvc_gen("foo", "foo", commit="add foo")
 
     cache_dir = make_tmp_dir("temp-cache")
     with external_repo(
         str(tmp_dir),
@@ -71,20 +70,18 @@
 
         list(repo.dvcfs.walk("", ignore_subrepos=False))  # drain
         assert spy.call_count == 1
         subrepo = spy.spy_return
 
         assert repo.url == str(tmp_dir)
         assert repo.config["cache"]["dir"] == str(cache_dir)
-        assert repo.cache.local.path == str(cache_dir)
-        assert subrepo.cache.local.path == str(cache_dir)
+        assert repo.cache.local.path == os.path.join(cache_dir, "files", "md5")
+        assert subrepo.cache.local.path == os.path.join(cache_dir, "files", "md5")
 
         assert repo.config["cache"]["type"] == ["symlink"]
         assert repo.cache.local.cache_types == ["symlink"]
         assert subrepo.cache.local.cache_types == ["symlink"]
 
         assert subrepo.config["remote"]["auto-generated-upstream"]["url"] == local_cache
         if root_is_dvc:
-            main_cache = tmp_dir.dvc.cache.local.path
-            assert repo.config["remote"]["auto-generated-upstream"]["url"] == str(
-                main_cache
-            )
+            main_cache = tmp_dir.dvc.cache.local_cache_dir
+            assert repo.config["remote"]["auto-generated-upstream"]["url"] == main_cache
```

### Comparing `dvc-3.0.0a2/tests/unit/repo/test_repo.py` & `dvc-3.1.0/tests/unit/repo/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/test_reproduce.py` & `dvc-3.1.0/tests/unit/repo/test_reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/repo/test_scm_context.py` & `dvc-3.1.0/tests/unit/repo/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/scm/test_scm.py` & `dvc-3.1.0/tests/unit/scm/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/stage/test_cache.py` & `dvc-3.1.0/tests/unit/stage/test_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
     assert not (tmp_dir / "out").exists()
     assert not (tmp_dir / "dvc.yaml").exists()
     assert not (tmp_dir / "dvc.lock").exists()
 
     cache_dir = os.path.join(
         dvc.stage_cache.cache_dir,
-        "4b",
-        "4b495dc2b14e1ca5bd5f2765a99ddd8785523a8342efe6bcadac012c2db01165",
+        "c7",
+        "c7a85d71de1912c43d9c5b6218c71630d6277e8fc11e4ccf5e12b3c202234838",
     )
     cache_file = os.path.join(
         cache_dir,
-        "78c427104a8e20216031c36d9c7620733066fff33ada254ad3fca551c1f8152b",
+        "5e2824029f8da9ef6c57131a638ceb65f27c02f16c85d71e85671c27daed0501",
     )
 
     assert os.path.isdir(cache_dir)
     assert os.listdir(cache_dir) == [os.path.basename(cache_file)]
     assert os.path.isfile(cache_file)
 
     run_spy = mocker.patch("dvc.stage.run.cmd_run")
@@ -75,15 +75,15 @@
     cache_dir = os.path.join(
         dvc.stage_cache.cache_dir,
         "8f",
         "8fdb377d1b4c0a303b788771b122dfba9bbbbc43f14ce41d35715cf4fea08459",
     )
     cache_file = os.path.join(
         cache_dir,
-        "202ea269108bf98bea3e15f978e7929864728956c9df8d927a5c7d74fc4fedc8",
+        "9ce1963a69beb1299800188647cd960b7afff101be19fd46226e32bb8be8ee44",
     )
 
     assert os.path.isdir(cache_dir)
     assert os.listdir(cache_dir) == [os.path.basename(cache_file)]
     assert os.path.isfile(cache_file)
 
     run_spy = mocker.patch("dvc.stage.run.cmd_run")
@@ -118,20 +118,20 @@
 
     assert not (tmp_dir / "wdir" / "out").exists()
     assert not (tmp_dir / "wdir" / "dvc.yaml").exists()
     assert not (tmp_dir / "wdir" / "dvc.lock").exists()
 
     cache_dir = os.path.join(
         dvc.stage_cache.cache_dir,
-        "b5",
-        "b5d5548c43725139aa3419eb50717e062fe9b81f866f401fd6fd778d2a97822d",
+        "6a",
+        "6ad5cce3347e9e96c77d4353d84e5c8cae8c9151c486c4ea3d3d79e9051800f1",
     )
     cache_file = os.path.join(
         cache_dir,
-        "e0a59f6a5bd193032a4d1500abd89c9b08a2e9b26c724015e0bc6374295a3b9f",
+        "1fa3e1a9f785f8364ad185d62bd0813ce8794afcfc79410e985eac0443cc5462",
     )
 
     assert os.path.isdir(cache_dir)
     assert os.listdir(cache_dir) == [os.path.basename(cache_file)]
     assert os.path.isfile(cache_file)
 
     run_spy = mocker.patch("dvc.stage.run.cmd_run")
@@ -158,22 +158,22 @@
 
     dvc.cache = CacheManager(dvc)
 
     assert not os.path.exists(dvc.cache.local.path)
 
     run_copy("foo", "bar", name="copy-foo-bar")
 
-    parent_cache_dir = os.path.join(dvc.stage_cache.cache_dir, "fd")
+    parent_cache_dir = os.path.join(dvc.stage_cache.cache_dir, "6d")
     cache_dir = os.path.join(
         parent_cache_dir,
-        "fdbe7847136ebe88f59a29ee5a568f893cab031f74f7d3ab050828b53fd0033a",
+        "6d4c6de74e7c0d60d2122e2063b4724a8c78a6799def6c7cf5093f45e7f2f3b7",
     )
     cache_file = os.path.join(
         cache_dir,
-        "8716052b2074f5acf1a379529d47d6ef1c1f50c2281a7489b8d7ce251f234f86",
+        "435e34f80692059e79ec53346cbfe29fd9ee65b62f5f06f17f5950ce5a7408ea",
     )
 
     # sanity check
     assert os.path.isdir(cache_dir)
     assert os.listdir(cache_dir) == [os.path.basename(cache_file)]
     assert os.path.isfile(cache_file)
```

### Comparing `dvc-3.0.0a2/tests/unit/stage/test_loader_pipeline_file.py` & `dvc-3.1.0/tests/unit/stage/test_loader_pipeline_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     return {"cmd": "command", "deps": ["foo"], "outs": ["bar"]}
 
 
 @pytest.fixture
 def lock_data():
     return {
         "cmd": "command",
-        "deps": [{"path": "foo", "md5": "foo_checksum"}],
-        "outs": [{"path": "bar", "md5": "bar_checksum"}],
+        "deps": [{"path": "foo", "md5": "foo_checksum", "hash": "md5"}],
+        "outs": [{"path": "bar", "md5": "bar_checksum", "hash": "md5"}],
     }
 
 
 def test_fill_from_lock_deps_outs(dvc, lock_data):
     stage = create_stage(PipelineStage, dvc, PROJECT_FILE, deps=["foo"], outs=["bar"])
 
     for item in chain(stage.deps, stage.outs):
@@ -42,15 +42,17 @@
 
     assert not stage.outs[0].meta.isexec
 
     StageLoader.fill_from_lock(
         stage,
         {
             "cmd": "command",
-            "outs": [{"path": "foo", "md5": "foo_checksum", "isexec": True}],
+            "outs": [
+                {"path": "foo", "md5": "foo_checksum", "isexec": True, "hash": "md5"}
+            ],
         },
     )
 
     assert stage.outs[0].def_path == "foo"
     assert stage.outs[0].hash_info == HashInfo("md5", "foo_checksum")
     assert stage.outs[0].meta.isexec
 
@@ -249,7 +251,24 @@
     dvcfile.lockfile_contents = {"stage": lock_data}
 
     assert len(dvcfile.stages) == 1
     assert "stage" in dvcfile.stages
     assert "stage1" not in dvcfile.stages
     assert dvcfile.stages.keys() == {"stage"}
     assert isinstance(dvcfile.stages["stage"], PipelineStage)
+
+
+def test_fill_from_lock_dos2unix(dvc):
+    lock_data = {
+        "cmd": "command",
+        "deps": [{"path": "foo", "md5": "foo_checksum"}],
+        "outs": [{"path": "bar", "md5": "bar_checksum"}],
+    }
+    stage = create_stage(PipelineStage, dvc, PROJECT_FILE, deps=["foo"], outs=["bar"])
+
+    for item in chain(stage.deps, stage.outs):
+        assert not item.hash_info
+
+    StageLoader.fill_from_lock(stage, lock_data)
+
+    assert stage.deps[0].hash_info == HashInfo("md5-dos2unix", "foo_checksum")
+    assert stage.outs[0].hash_info == HashInfo("md5-dos2unix", "bar_checksum")
```

### Comparing `dvc-3.0.0a2/tests/unit/stage/test_run.py` & `dvc-3.1.0/tests/unit/stage/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/stage/test_serialize_pipeline_file.py` & `dvc-3.1.0/tests/unit/stage/test_serialize_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/stage/test_serialize_pipeline_lock.py` & `dvc-3.1.0/tests/unit/stage/test_serialize_pipeline_lock.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,31 +29,38 @@
 
 def test_lock_deps(dvc):
     stage = create_stage(PipelineStage, dvc, deps=["input"], **kwargs)
     stage.deps[0].hash_info = HashInfo("md5", "md-five")
     assert to_single_stage_lockfile(stage) == OrderedDict(
         [
             ("cmd", "command"),
-            ("deps", [OrderedDict([("path", "input"), ("md5", "md-five")])]),
+            (
+                "deps",
+                [OrderedDict([("hash", "md5"), ("path", "input"), ("md5", "md-five")])],
+            ),
         ]
     )
 
 
 def test_lock_deps_order(dvc):
     stage = create_stage(PipelineStage, dvc, deps=["input1", "input0"], **kwargs)
     stage.deps[0].hash_info = HashInfo("md5", "md-one1")
     stage.deps[1].hash_info = HashInfo("md5", "md-zer0")
     assert to_single_stage_lockfile(stage) == OrderedDict(
         [
             ("cmd", "command"),
             (
                 "deps",
                 [
-                    OrderedDict([("path", "input0"), ("md5", "md-zer0")]),
-                    OrderedDict([("path", "input1"), ("md5", "md-one1")]),
+                    OrderedDict(
+                        [("hash", "md5"), ("path", "input0"), ("md5", "md-zer0")]
+                    ),
+                    OrderedDict(
+                        [("hash", "md5"), ("path", "input1"), ("md5", "md-one1")]
+                    ),
                 ],
             ),
         ]
     )
 
 
 def test_lock_params(dvc):
@@ -130,15 +137,18 @@
 @pytest.mark.parametrize("typ", ["plots", "metrics", "outs"])
 def test_lock_outs(dvc, typ):
     stage = create_stage(PipelineStage, dvc, **{typ: ["input"]}, **kwargs)
     stage.outs[0].hash_info = HashInfo("md5", "md-five")
     assert to_single_stage_lockfile(stage) == OrderedDict(
         [
             ("cmd", "command"),
-            ("outs", [OrderedDict([("path", "input"), ("md5", "md-five")])]),
+            (
+                "outs",
+                [OrderedDict([("hash", "md5"), ("path", "input"), ("md5", "md-five")])],
+            ),
         ]
     )
 
 
 @pytest.mark.parametrize("typ", ["plots", "metrics", "outs"])
 def test_lock_outs_isexec(dvc, typ):
     stage = create_stage(PipelineStage, dvc, **{typ: ["input"]}, **kwargs)
@@ -148,14 +158,15 @@
         [
             ("cmd", "command"),
             (
                 "outs",
                 [
                     OrderedDict(
                         [
+                            ("hash", "md5"),
                             ("path", "input"),
                             ("md5", "md-five"),
                             ("isexec", True),
                         ]
                     )
                 ],
             ),
@@ -170,31 +181,43 @@
     stage.outs[1].hash_info = HashInfo("md5", "md-zer0")
     assert to_single_stage_lockfile(stage) == OrderedDict(
         [
             ("cmd", "command"),
             (
                 "outs",
                 [
-                    OrderedDict([("path", "input0"), ("md5", "md-zer0")]),
-                    OrderedDict([("path", "input1"), ("md5", "md-one1")]),
+                    OrderedDict(
+                        [("hash", "md5"), ("path", "input0"), ("md5", "md-zer0")]
+                    ),
+                    OrderedDict(
+                        [("hash", "md5"), ("path", "input1"), ("md5", "md-one1")]
+                    ),
                 ],
             ),
         ]
     )
 
 
 def test_dump_nondefault_hash(dvc):
     stage = create_stage(PipelineStage, dvc, deps=["s3://dvc-temp/file"], **kwargs)
     stage.deps[0].hash_info = HashInfo("md5", "value")
     assert to_single_stage_lockfile(stage) == OrderedDict(
         [
             ("cmd", "command"),
             (
                 "deps",
-                [OrderedDict([("path", "s3://dvc-temp/file"), ("md5", "value")])],
+                [
+                    OrderedDict(
+                        [
+                            ("hash", "md5"),
+                            ("path", "s3://dvc-temp/file"),
+                            ("md5", "value"),
+                        ]
+                    )
+                ],
             ),
         ]
     )
 
 
 def test_order(dvc):
     stage = create_stage(
@@ -210,32 +233,32 @@
     deps[0].hash_info = HashInfo("md5", "md-five")
     params[0].hash_info = HashInfo("params", {"foo-param": "value"})
     stage.outs[0].hash_info = HashInfo("md5", "md5-output")
 
     assert to_single_stage_lockfile(stage) == OrderedDict(
         [
             ("cmd", "command"),
-            ("deps", [{"path": "input", "md5": "md-five"}]),
+            ("deps", [{"hash": "md5", "path": "input", "md5": "md-five"}]),
             ("params", {"params.yaml": {"foo-param": "value"}}),
-            ("outs", [{"path": "output", "md5": "md5-output"}]),
+            ("outs", [{"hash": "md5", "path": "output", "md5": "md5-output"}]),
         ]
     )
 
 
 def test_to_lockfile(dvc):
     stage = create_stage(PipelineStage, dvc, deps=["input"], **kwargs)
     stage.deps[0].hash_info = HashInfo("md5", "md-five")
     entry = to_lockfile(stage)
     assert len(entry) == 1
     _Schema(LOCKFILE_STAGES_SCHEMA)(entry)
     assert entry == {
         "something": OrderedDict(
             [
                 ("cmd", "command"),
-                ("deps", [{"path": "input", "md5": "md-five"}]),
+                ("deps", [{"hash": "md5", "path": "input", "md5": "md-five"}]),
             ]
         )
     }
 
 
 def test_to_single_stage_lockfile_cloud_versioning_dir(dvc):
     stage = create_stage(PipelineStage, dvc, outs=["dir"], **kwargs)
@@ -255,8 +278,8 @@
             "md5": "acbd18db4cc2f85cedef654fccc4a4d8",
             "relpath": "foo",
         },
     ]
     stage.outs[0].files = files
     e = _to_single_stage_lockfile(stage, with_files=True)
     assert Schema(e)
-    assert e["outs"][0] == {"path": "dir", "files": files}
+    assert e["outs"][0] == {"hash": "md5", "path": "dir", "files": files}
```

### Comparing `dvc-3.0.0a2/tests/unit/stage/test_stage.py` & `dvc-3.1.0/tests/unit/stage/test_stage.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,9 +116,12 @@
 
     with pytest.raises(StageExternalOutputsError):
         create_stage(Stage, dvc, "path.dvc", outs=[os.fspath(foo)])
 
     with dvc.config.edit() as conf:
         conf["remote"]["myremote"] = {"url": os.fspath(tmp_path)}
 
-    create_stage(Stage, dvc, "path.dvc", outs=["remote://myremote/foo"])
-    create_stage(Stage, dvc, "path.dvc", outs=[os.fspath(foo)], external=True)
+    with pytest.raises(StageExternalOutputsError):
+        create_stage(Stage, dvc, "path.dvc", outs=["remote://myremote/foo"])
+
+    create_stage(Stage, dvc, "path.dvc", outs_no_cache=["remote://myremote/foo"])
+    create_stage(Stage, dvc, "path.dvc", outs_no_cache=[os.fspath(foo)])
```

### Comparing `dvc-3.0.0a2/tests/unit/stage/test_utils.py` & `dvc-3.1.0/tests/unit/stage/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_analytics.py` & `dvc-3.1.0/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_collect.py` & `dvc-3.1.0/tests/unit/test_collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_compare.py` & `dvc-3.1.0/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_config.py` & `dvc-3.1.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_context.py` & `dvc-3.1.0/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_daemon.py` & `dvc-3.1.0/tests/unit/test_daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_dvcfile.py` & `dvc-3.1.0/tests/unit/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_ignore.py` & `dvc-3.1.0/tests/unit/test_ignore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 import os
-from unittest.mock import MagicMock, mock_open, patch
 
 import pytest
 
 from dvc.ignore import DvcIgnorePatterns
 
 
-def mock_dvcignore(dvcignore_path, patterns):
-    from dvc.fs import localfs
-
-    fs = MagicMock()
-    fs.path = localfs.path
-    fs.sep = localfs.sep
-    with patch.object(fs, "open", mock_open(read_data="\n".join(patterns))):
-        return DvcIgnorePatterns.from_file(dvcignore_path, fs, "mocked")
-
-
 @pytest.mark.parametrize(
     "file_to_ignore_relpath, patterns,  expected_match",
     [
         # all rules from https://git-scm.com/docs/gitignore
         ("to_ignore", ["to_ignore"], True),
         ("dont_ignore.txt", ["dont_ignore"], False),
         # A blank line matches no files, so it can serve as a separator for
@@ -170,21 +159,29 @@
         (
             os.path.join("rel", "path", "path2", "to_ignore"),
             ["rel/***/to_ignore"],
             False,
         ),
     ],
 )
-def test_match_ignore_from_file(file_to_ignore_relpath, patterns, expected_match):
+def test_match_ignore_from_file(
+    file_to_ignore_relpath, patterns, expected_match, mocker
+):
+    from dvc.fs import localfs
+
     dvcignore_path = os.path.join(
         os.path.sep, "full", "path", "to", "ignore", "file", ".dvcignore"
     )
     dvcignore_dirname = os.path.dirname(dvcignore_path)
 
-    ignore_file = mock_dvcignore(dvcignore_path, patterns)
+    fs = mocker.MagicMock()
+    fs.path = localfs.path
+    fs.sep = localfs.sep
+    mocker.patch.object(fs, "open", mocker.mock_open(read_data="\n".join(patterns)))
+    ignore_file = DvcIgnorePatterns.from_file(dvcignore_path, fs, "mocked")
 
     assert (
         ignore_file.matches(dvcignore_dirname, file_to_ignore_relpath) == expected_match
     )
 
 
 @pytest.mark.parametrize("sub_dir", ["", "dir"])
```

### Comparing `dvc-3.0.0a2/tests/unit/test_imports.py` & `dvc-3.1.0/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_info.py` & `dvc-3.1.0/tests/unit/test_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     return remotes
 
 
 @pytest.mark.parametrize("scm_init", [True, False])
 def test_info_in_repo(scm_init, tmp_dir):
     tmp_dir.init(scm=scm_init, dvc=True)
     # Create `.dvc/cache`, that is needed to check supported link types.
-    os.mkdir(tmp_dir.dvc.cache.local.path)
+    os.makedirs(tmp_dir.dvc.cache.local.path)
 
     dvc_info = get_dvc_info()
 
     assert re.search(rf"DVC version: {DVC_VERSION_REGEX}", dvc_info)
     assert re.search(f"Platform: {PYTHON_VERSION_REGEX} on .*", dvc_info)
     for subproject in SUBPROJECTS:
         assert re.search(rf"{subproject} = .*", dvc_info)
@@ -81,22 +81,18 @@
     shutil.rmtree(dvc.scm.dir)
     dvc_info = get_dvc_info()
 
     assert "Repo: dvc, git (broken)" in dvc_info
 
 
 def test_caches(tmp_dir, dvc, caplog):
-    tmp_dir.add_remote(name="sshcache", url="ssh://example.com/path", default=False)
-    with tmp_dir.dvc.config.edit() as conf:
-        conf["cache"]["ssh"] = "sshcache"
-
     dvc_info = get_dvc_info()
 
     # Order of cache types is runtime dependent
-    assert re.search("Caches: (local, ssh|ssh, local)", dvc_info)
+    assert re.search("Caches: local", dvc_info)
 
 
 def test_remotes_empty(tmp_dir, dvc, caplog):
     # No remotes are configured
     dvc_info = get_dvc_info()
 
     assert "Remotes: None" in dvc_info
@@ -109,15 +105,15 @@
 
     dvc_info = get_dvc_info()
 
     assert re.search("Remotes: (ssh, azure|azure, ssh)", dvc_info)
 
 
 def test_fs_info_in_repo(tmp_dir, dvc, caplog):
-    os.mkdir(dvc.cache.local.path)
+    os.makedirs(dvc.cache.local.path)
     dvc_info = get_dvc_info()
 
     assert re.search(r"Cache directory: .* on .*", dvc_info)
     assert re.search(r"Workspace directory: .* on .*", dvc_info)
 
 
 def test_info_outside_of_repo(tmp_dir, caplog):
```

### Comparing `dvc-3.0.0a2/tests/unit/test_interpolate.py` & `dvc-3.1.0/tests/unit/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_lockfile.py` & `dvc-3.1.0/tests/unit/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_logger.py` & `dvc-3.1.0/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_metrics.py` & `dvc-3.1.0/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_params.py` & `dvc-3.1.0/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_pathspec_math.py` & `dvc-3.1.0/tests/unit/test_pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_progress.py` & `dvc-3.1.0/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_rwlock.py` & `dvc-3.1.0/tests/unit/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_tabular_data.py` & `dvc-3.1.0/tests/unit/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/test_updater.py` & `dvc-3.1.0/tests/unit/test_updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/ui/test_console.py` & `dvc-3.1.0/tests/unit/ui/test_console.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/ui/test_pager.py` & `dvc-3.1.0/tests/unit/ui/test_pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/ui/test_table.py` & `dvc-3.1.0/tests/unit/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/serialize/test_python.py` & `dvc-3.1.0/tests/unit/utils/serialize/test_python.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/serialize/test_toml.py` & `dvc-3.1.0/tests/unit/utils/serialize/test_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/serialize/test_yaml.py` & `dvc-3.1.0/tests/unit/utils/serialize/test_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/test_cli_parse.py` & `dvc-3.1.0/tests/unit/utils/test_cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/test_collections.py` & `dvc-3.1.0/tests/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/test_executors.py` & `dvc-3.1.0/tests/unit/utils/test_executors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/test_fs.py` & `dvc-3.1.0/tests/unit/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/test_humanize.py` & `dvc-3.1.0/tests/unit/utils/test_humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/test_studio.py` & `dvc-3.1.0/tests/unit/utils/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/unit/utils/test_utils.py` & `dvc-3.1.0/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/utils/__init__.py` & `dvc-3.1.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a2/tests/utils/asserts.py` & `dvc-3.1.0/tests/utils/asserts.py`

 * *Files identical despite different names*

