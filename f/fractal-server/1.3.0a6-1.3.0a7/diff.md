# Comparing `tmp/fractal_server-1.3.0a6.tar.gz` & `tmp/fractal_server-1.3.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.0a6.tar", max compression
+gzip compressed data, was "fractal_server-1.3.0a7.tar", max compression
```

## Comparing `fractal_server-1.3.0a6.tar` & `fractal_server-1.3.0a7.tar`

### file list

```diff
@@ -1,135 +1,137 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a6/LICENSE
--rw-r--r--   0        0        0     2100 2023-06-13 11:33:49.890135 fractal_server-1.3.0a6/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a6/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-06-19 06:52:18.228019 fractal_server-1.3.0a6/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-05-25 12:06:55.503794 fractal_server-1.3.0a6/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a6/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a6/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a6/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a6/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     7616 2023-06-13 11:33:49.890135 fractal_server-1.3.0a6/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     7624 2023-05-23 13:25:45.067972 fractal_server-1.3.0a6/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a6/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a6/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    15912 2023-06-15 09:47:58.010806 fractal_server-1.3.0a6/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    12501 2023-05-29 15:02:27.725371 fractal_server-1.3.0a6/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a6/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a6/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-29 08:51:11.986940 fractal_server-1.3.0a6/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a6/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2355 2023-05-29 08:51:11.986940 fractal_server-1.3.0a6/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2563 2023-05-29 09:51:02.494983 fractal_server-1.3.0a6/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1119 2023-05-29 08:51:11.986940 fractal_server-1.3.0a6/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1591 2023-06-08 09:21:57.166713 fractal_server-1.3.0a6/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5861 2023-06-15 13:41:34.921597 fractal_server-1.3.0a6/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a6/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8969 2023-05-15 10:36:57.758906 fractal_server-1.3.0a6/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19523 2023-06-08 09:22:21.105956 fractal_server-1.3.0a6/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a6/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3245 2023-06-15 13:41:34.921597 fractal_server-1.3.0a6/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a6/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a6/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19766 2023-06-15 13:41:34.921597 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42200 2023-05-18 09:57:35.703959 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-06-08 08:33:26.930560 fractal_server-1.3.0a6/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a6/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a6/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a6/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a6/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a6/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a6/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a6/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       57 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      425 2023-05-26 06:49:50.432129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1624 2023-06-12 09:13:31.352825 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     4082 2023-06-12 09:13:31.356825 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3551 2023-05-26 06:49:50.436129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1179 2023-05-26 06:49:50.444129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     2719 2023-06-12 09:13:31.364825 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     3306 2023-06-12 09:13:31.368826 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1216 2023-05-26 06:49:50.448129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     3896 2023-05-26 06:49:50.452129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1255 2023-06-15 11:41:13.549879 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2806 2023-05-26 06:49:50.864124 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1349 2023-06-15 11:41:13.553879 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2685 2023-05-26 06:49:50.868124 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a6/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-06-12 09:12:04.410676 fractal_server-1.3.0a6/fractal_server/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a6/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12432 2023-06-15 13:41:27.513642 fractal_server-1.3.0a6/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a6/fractal_server/logger.py
--rw-r--r--   0        0        0     5935 2023-06-15 13:41:27.513642 fractal_server-1.3.0a6/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a6/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a6/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a6/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2023-06-08 09:21:57.166713 fractal_server-1.3.0a6/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     8770 2023-05-29 15:02:27.725371 fractal_server-1.3.0a6/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0      746 2023-06-08 09:21:57.166713 fractal_server-1.3.0a6/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a6/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a6/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a6/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    17581 2023-06-12 14:10:58.230055 fractal_server-1.3.0a6/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a6/fractal_server/utils.py
--rw-r--r--   0        0        0     2704 2023-06-19 06:52:18.228019 fractal_server-1.3.0a6/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 fractal_server-1.3.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a7/LICENSE
+-rw-r--r--   0        0        0     2100 2023-06-19 09:13:19.197654 fractal_server-1.3.0a7/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a7/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-06-19 14:50:41.774116 fractal_server-1.3.0a7/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-05-25 12:06:55.503794 fractal_server-1.3.0a7/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a7/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a7/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a7/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a7/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     7616 2023-06-19 09:13:19.197654 fractal_server-1.3.0a7/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     7624 2023-05-23 13:25:45.067972 fractal_server-1.3.0a7/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a7/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a7/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    15912 2023-06-19 09:13:19.197654 fractal_server-1.3.0a7/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    12501 2023-05-29 15:02:27.725371 fractal_server-1.3.0a7/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a7/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a7/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-29 08:51:11.986940 fractal_server-1.3.0a7/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a7/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2355 2023-05-29 08:51:11.986940 fractal_server-1.3.0a7/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2563 2023-05-29 09:51:02.494983 fractal_server-1.3.0a7/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1119 2023-05-29 08:51:11.986940 fractal_server-1.3.0a7/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1591 2023-06-19 14:50:22.446330 fractal_server-1.3.0a7/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5861 2023-06-19 09:13:19.197654 fractal_server-1.3.0a7/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a7/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0    10102 2023-06-19 11:56:16.860753 fractal_server-1.3.0a7/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19523 2023-06-08 09:22:21.105956 fractal_server-1.3.0a7/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a7/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3245 2023-06-19 09:13:19.197654 fractal_server-1.3.0a7/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a7/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a7/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19766 2023-06-19 09:13:19.197654 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42200 2023-05-18 09:57:35.703959 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-06-08 08:33:26.930560 fractal_server-1.3.0a7/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a7/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a7/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a7/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a7/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a7/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a7/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a7/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a7/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a7/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a7/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       57 2023-05-26 06:41:57.297956 fractal_server-1.3.0a7/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-05-26 06:41:57.297956 fractal_server-1.3.0a7/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      425 2023-05-26 06:49:50.432129 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1624 2023-06-12 09:13:31.352825 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     4082 2023-06-12 09:13:31.356825 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3551 2023-05-26 06:49:50.436129 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1179 2023-05-26 06:49:50.444129 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     2719 2023-06-12 09:13:31.364825 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     3306 2023-06-12 09:13:31.368826 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1216 2023-05-26 06:49:50.448129 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     3896 2023-05-26 06:49:50.452129 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a7/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-06-12 09:12:04.406676 fractal_server-1.3.0a7/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-12 09:12:04.406676 fractal_server-1.3.0a7/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-05-26 06:41:57.297956 fractal_server-1.3.0a7/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-05-26 06:41:57.297956 fractal_server-1.3.0a7/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-12 09:12:04.406676 fractal_server-1.3.0a7/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-12 09:12:04.406676 fractal_server-1.3.0a7/fractal_server/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-05-26 06:41:57.297956 fractal_server-1.3.0a7/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-05-26 06:41:57.297956 fractal_server-1.3.0a7/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1255 2023-06-15 11:41:13.549879 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2806 2023-05-26 06:49:50.864124 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1349 2023-06-15 11:41:13.553879 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2685 2023-05-26 06:49:50.868124 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a7/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a7/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a7/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-12 09:12:04.406676 fractal_server-1.3.0a7/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a7/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a7/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-05-26 06:41:57.297956 fractal_server-1.3.0a7/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-06-12 09:12:04.410676 fractal_server-1.3.0a7/fractal_server/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-05-26 06:41:57.297956 fractal_server-1.3.0a7/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a7/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12432 2023-06-19 09:13:19.197654 fractal_server-1.3.0a7/fractal_server/config.py
+-rwxr-xr-x   0        0        0      187 2023-06-19 12:01:37.838943 fractal_server-1.3.0a7/fractal_server/doit.sh
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a7/fractal_server/logger.py
+-rw-r--r--   0        0        0     5935 2023-06-19 09:13:19.197654 fractal_server-1.3.0a7/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a7/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-06-19 14:49:54.798636 fractal_server-1.3.0a7/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a7/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2023-06-08 09:21:57.166713 fractal_server-1.3.0a7/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     8770 2023-05-29 15:02:27.725371 fractal_server-1.3.0a7/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0      840 2023-06-19 12:12:30.266204 fractal_server-1.3.0a7/fractal_server/migrations/versions/f3270beadc68_.py
+-rw-r--r--   0        0        0      746 2023-06-08 09:21:57.166713 fractal_server-1.3.0a7/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a7/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a7/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a7/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    17581 2023-06-12 14:10:58.230055 fractal_server-1.3.0a7/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a7/fractal_server/utils.py
+-rw-r--r--   0        0        0     2704 2023-06-19 14:50:41.774116 fractal_server-1.3.0a7/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 fractal_server-1.3.0a7/PKG-INFO
```

### Comparing `fractal_server-1.3.0a6/LICENSE` & `fractal_server-1.3.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/README.md` & `fractal_server-1.3.0a7/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/__main__.py` & `fractal_server-1.3.0a7/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/alembic.ini` & `fractal_server-1.3.0a7/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/api/__init__.py` & `fractal_server-1.3.0a7/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.0a7/fractal_server/app/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.0a7/fractal_server/app/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.0a7/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.0a7/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.0a7/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.0a7/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/db/__init__.py` & `fractal_server-1.3.0a7/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/models/job.py` & `fractal_server-1.3.0a7/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/models/project.py` & `fractal_server-1.3.0a7/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/models/security.py` & `fractal_server-1.3.0a7/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/models/state.py` & `fractal_server-1.3.0a7/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/models/task.py` & `fractal_server-1.3.0a7/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/models/workflow.py` & `fractal_server-1.3.0a7/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,102 +98,114 @@
             Cache directory (namely a path where the user can write); for the
             slurm backend, this is used as a base directory for
             `job.working_dir_user`.
         slurm_user:
             The username to impersonate for the workflow execution, for the
             slurm backend.
     """
+    with next(DB.get_sync_db()) as db_sync:
 
-    db_sync = next(DB.get_sync_db())
+        job: ApplyWorkflow = db_sync.get(ApplyWorkflow, job_id)
+        if not job:
+            raise ValueError("Cannot fetch job from database")
+        input_dataset: Dataset = db_sync.get(Dataset, input_dataset_id)
+        if not input_dataset:
+            raise ValueError("Cannot fetch input_dataset from database")
+        output_dataset: Dataset = db_sync.get(Dataset, output_dataset_id)
+        if not output_dataset:
+            raise ValueError("Cannot fetch output_dataset from database")
+        workflow: Workflow = db_sync.get(Workflow, workflow_id)
+        if not workflow:
+            raise ValueError("Cannot fetch workflow from database")
+
+        # Select backend
+        settings = Inject(get_settings)
+        FRACTAL_RUNNER_BACKEND = settings.FRACTAL_RUNNER_BACKEND
+        process_workflow = get_process_workflow()
+
+        # Prepare some of process_workflow arguments
+        input_paths = input_dataset.paths
+        output_path = output_dataset.paths[0]
+        workflow_id = workflow.id
 
-    job: ApplyWorkflow = db_sync.get(ApplyWorkflow, job_id)
-    if not job:
-        raise ValueError("Cannot fetch job from database")
-    input_dataset: Dataset = db_sync.get(Dataset, input_dataset_id)
-    if not input_dataset:
-        raise ValueError("Cannot fetch input_dataset from database")
-    output_dataset: Dataset = db_sync.get(Dataset, output_dataset_id)
-    if not output_dataset:
-        raise ValueError("Cannot fetch output_dataset from database")
-    workflow: Workflow = db_sync.get(Workflow, workflow_id)
-    if not workflow:
-        raise ValueError("Cannot fetch workflow from database")
-
-    # Select backend
-    settings = Inject(get_settings)
-    FRACTAL_RUNNER_BACKEND = settings.FRACTAL_RUNNER_BACKEND
-    process_workflow = get_process_workflow()
-
-    # Prepare some of process_workflow arguments
-    input_paths = input_dataset.paths
-    output_path = output_dataset.paths[0]
-    workflow_id = workflow.id
-
-    # Define and create server-side working folder
-    project_id = workflow.project_id
-    WORKFLOW_DIR = (
-        settings.FRACTAL_RUNNER_WORKING_BASE_DIR  # type: ignore
-        / f"proj_{project_id:07d}_wf_{workflow_id:07d}_job_{job_id:07d}"
-    ).resolve()
-    if not WORKFLOW_DIR.exists():
+        # Define and create server-side working folder
+        project_id = workflow.project_id
+        timestamp_string = get_timestamp().strftime("%Y%m%d_%H%M%S")
+        WORKFLOW_DIR = (
+            settings.FRACTAL_RUNNER_WORKING_BASE_DIR  # type: ignore
+            / (
+                f"proj_{project_id:07d}_wf_{workflow_id:07d}_job_{job_id:07d}"
+                f"_{timestamp_string}"
+            )
+        ).resolve()
+
+        if WORKFLOW_DIR.exists():
+            raise RuntimeError(f"Workflow dir {WORKFLOW_DIR} already exists.")
+
+        # Create WORKFLOW_DIR with 755 permissions
         original_umask = os.umask(0)
         WORKFLOW_DIR.mkdir(parents=True, mode=0o755)
         os.umask(original_umask)
 
-    # Define and create user-side working folder, if needed
-    if FRACTAL_RUNNER_BACKEND == "local":
-        WORKFLOW_DIR_USER = WORKFLOW_DIR
-    elif FRACTAL_RUNNER_BACKEND == "slurm":
-        timestamp_string = get_timestamp().strftime("%Y%m%d_%H%M%S")
-
-        from ._slurm._subprocess_run_as_user import _mkdir_as_user
-
-        WORKFLOW_DIR_USER = (
-            Path(user_cache_dir) / f"{timestamp_string}_{WORKFLOW_DIR.name}"
-        ).resolve()
-        _mkdir_as_user(folder=str(WORKFLOW_DIR_USER), user=slurm_user)
-    else:
-        raise ValueError(f"{FRACTAL_RUNNER_BACKEND=} not supported")
-
-    # Update db
-    job.working_dir = WORKFLOW_DIR.as_posix()
-    job.working_dir_user = WORKFLOW_DIR_USER.as_posix()
-    job.status = JobStatusType.RUNNING
-    db_sync.merge(job)
-    db_sync.commit()
-
-    # Write logs
-    logger_name = f"WF{workflow_id}_job{job_id}"
-    log_file_path = WORKFLOW_DIR / "workflow.log"
-    logger = set_logger(
-        logger_name=logger_name,
-        log_file_path=log_file_path,
-    )
-    logger.info(
-        f'Start execution of workflow "{workflow.name}"; '
-        f"more logs at {str(log_file_path)}"
-    )
-    logger.debug(f"fractal_server.__VERSION__: {__VERSION__}")
-    logger.debug(f"FRACTAL_RUNNER_BACKEND: {FRACTAL_RUNNER_BACKEND}")
-    logger.debug(f"slurm_user: {slurm_user}")
-    logger.debug(f"worker_init: {worker_init}")
-    logger.debug(f"input metadata: {input_dataset.meta}")
-    logger.debug(f"input_paths: {input_paths}")
-    logger.debug(f"output_path: {output_path}")
-    logger.debug(f"job.id: {job.id}")
-    logger.debug(f"job.working_dir: {str(WORKFLOW_DIR)}")
-    logger.debug(f"job.workflow_dir_user: {str(WORKFLOW_DIR_USER)}")
-    logger.debug(f'START workflow "{workflow.name}"')
-
-    # Note: from the docs, "The Session.close() method does not prevent the
-    # Session from being used again"
-    # (https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.Session.close)
-    db_sync.close()
+        # Define and create user-side working folder, if needed
+        if FRACTAL_RUNNER_BACKEND == "local":
+            WORKFLOW_DIR_USER = WORKFLOW_DIR
+        elif FRACTAL_RUNNER_BACKEND == "slurm":
+
+            from ._slurm._subprocess_run_as_user import _mkdir_as_user
+
+            WORKFLOW_DIR_USER = (
+                Path(user_cache_dir) / f"{WORKFLOW_DIR.name}"
+            ).resolve()
+            _mkdir_as_user(folder=str(WORKFLOW_DIR_USER), user=slurm_user)
+        else:
+            raise ValueError(f"{FRACTAL_RUNNER_BACKEND=} not supported")
+
+        # Update db
+        job.working_dir = WORKFLOW_DIR.as_posix()
+        job.working_dir_user = WORKFLOW_DIR_USER.as_posix()
+        job.status = JobStatusType.RUNNING
+        db_sync.merge(job)
+        db_sync.commit()
+        # Write logs
+        logger_name = f"WF{workflow_id}_job{job_id}"
+        log_file_path = WORKFLOW_DIR / "workflow.log"
+        logger = set_logger(
+            logger_name=logger_name,
+            log_file_path=log_file_path,
+        )
+        logger.info(
+            f'Start execution of workflow "{workflow.name}"; '
+            f"more logs at {str(log_file_path)}"
+        )
+        logger.debug(f"fractal_server.__VERSION__: {__VERSION__}")
+        logger.debug(f"FRACTAL_RUNNER_BACKEND: {FRACTAL_RUNNER_BACKEND}")
+        logger.debug(f"slurm_user: {slurm_user}")
+        logger.debug(f"worker_init: {worker_init}")
+        logger.debug(f"input metadata: {input_dataset.meta}")
+        logger.debug(f"input_paths: {input_paths}")
+        logger.debug(f"output_path: {output_path}")
+        logger.debug(f"job.id: {job.id}")
+        logger.debug(f"job.working_dir: {str(WORKFLOW_DIR)}")
+        logger.debug(f"job.workflow_dir_user: {str(WORKFLOW_DIR_USER)}")
+        logger.debug(f'START workflow "{workflow.name}"')
 
     try:
+        # "The Session.close() method does not prevent the Session from being
+        # used again. The Session itself does not actually have a distinct
+        # “closed” state; it merely means the Session will release all database
+        # connections and ORM objects."
+        # (https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.Session.close).
+        #
+        # We close the session before the (possibly long) process_workflow
+        # call, to make sure all DB connections are released. The reason why we
+        # are not using a context manager within the try block is that we also
+        # need access to db_sync in the except branches.
+        db_sync = next(DB.get_sync_db())
+        db_sync.close()
 
         output_dataset.meta = await process_workflow(
             workflow=workflow,
             input_paths=input_paths,
             output_path=output_path,
             input_metadata=input_dataset.meta,
             slurm_user=slurm_user,
@@ -214,15 +226,16 @@
 
         job.status = JobStatusType.DONE
         job.end_timestamp = get_timestamp()
         with log_file_path.open("r") as f:
             logs = f.read()
         job.log = logs
         db_sync.merge(job)
-
+        close_job_logger(logger)
+        db_sync.commit()
     except TaskExecutionError as e:
 
         logger.debug(f'FAILED workflow "{workflow.name}", TaskExecutionError.')
         logger.info(f'Workflow "{workflow.name}" failed (TaskExecutionError).')
 
         job.status = JobStatusType.FAILED
         job.end_timestamp = get_timestamp()
@@ -231,33 +244,34 @@
         job.log = (
             f"TASK ERROR:"
             f"Task id: {e.workflow_task_id} ({e.task_name}), "
             f"{e.workflow_task_order=}\n"
             f"TRACEBACK:\n{exception_args_string}"
         )
         db_sync.merge(job)
-
+        close_job_logger(logger)
+        db_sync.commit()
     except JobExecutionError as e:
 
         logger.debug(f'FAILED workflow "{workflow.name}", JobExecutionError.')
         logger.info(f'Workflow "{workflow.name}" failed (JobExecutionError).')
 
         job.status = JobStatusType.FAILED
         job.end_timestamp = get_timestamp()
         error = e.assemble_error()
         job.log = f"JOB ERROR:\nTRACEBACK:\n{error}"
         db_sync.merge(job)
-
+        close_job_logger(logger)
+        db_sync.commit()
     except Exception as e:
 
         logger.debug(f'FAILED workflow "{workflow.name}", unknown error.')
         logger.info(f'Workflow "{workflow.name}" failed (unkwnon error).')
 
         job.status = JobStatusType.FAILED
         job.end_timestamp = get_timestamp()
         job.log = f"UNKNOWN ERROR\nOriginal error: {str(e)}"
         db_sync.merge(job)
-
-    finally:
         close_job_logger(logger)
         db_sync.commit()
+    finally:
         db_sync.close()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_common.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/runner/common.py` & `fractal_server-1.3.0a7/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/app/security/__init__.py` & `fractal_server-1.3.0a7/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.0a7/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.0a7/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/README.md` & `fractal_server-1.3.0a7/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.3.0a7/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/project.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/state.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/task.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/task_collection.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/user.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.0a7/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a7/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.0a7/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.3.0a7/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.0a7/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.0a7/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/test_task.py` & `fractal_server-1.3.0a7/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/test_task_collection.py` & `fractal_server-1.3.0a7/fractal_server/common/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.0a7/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.0a7/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/config.py` & `fractal_server-1.3.0a7/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/logger.py` & `fractal_server-1.3.0a7/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/main.py` & `fractal_server-1.3.0a7/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/migrations/env.py` & `fractal_server-1.3.0a7/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.0a7/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-1.3.0a7/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-1.3.0a7/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-1.3.0a7/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/syringe.py` & `fractal_server-1.3.0a7/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/tasks/collection.py` & `fractal_server-1.3.0a7/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/fractal_server/utils.py` & `fractal_server-1.3.0a7/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a6/pyproject.toml` & `fractal_server-1.3.0a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.0a6"
+version = "1.3.0a7"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -73,15 +73,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.0a6"
+current_version = "1.3.0a7"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.0a6/PKG-INFO` & `fractal_server-1.3.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.0a6
+Version: 1.3.0a7
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

