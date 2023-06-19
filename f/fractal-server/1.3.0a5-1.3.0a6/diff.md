# Comparing `tmp/fractal_server-1.3.0a5.tar.gz` & `tmp/fractal_server-1.3.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.0a5.tar", max compression
+gzip compressed data, was "fractal_server-1.3.0a6.tar", max compression
```

## Comparing `fractal_server-1.3.0a5.tar` & `fractal_server-1.3.0a6.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a5/LICENSE
--rw-r--r--   0        0        0     2100 2023-06-13 09:35:14.156721 fractal_server-1.3.0a5/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a5/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-06-13 10:03:02.349510 fractal_server-1.3.0a5/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-05-25 12:06:55.503794 fractal_server-1.3.0a5/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a5/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a5/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a5/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a5/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     7616 2023-06-13 09:35:05.784830 fractal_server-1.3.0a5/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     7624 2023-05-23 13:25:45.067972 fractal_server-1.3.0a5/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a5/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a5/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    15800 2023-06-13 09:35:05.784830 fractal_server-1.3.0a5/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    12501 2023-05-29 15:02:27.725371 fractal_server-1.3.0a5/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a5/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a5/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-29 08:51:11.986940 fractal_server-1.3.0a5/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a5/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2355 2023-05-29 08:51:11.986940 fractal_server-1.3.0a5/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2563 2023-05-29 09:51:02.494983 fractal_server-1.3.0a5/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1119 2023-05-29 08:51:11.986940 fractal_server-1.3.0a5/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1591 2023-06-08 09:21:57.166713 fractal_server-1.3.0a5/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5948 2023-06-08 09:22:21.105956 fractal_server-1.3.0a5/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a5/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8969 2023-05-15 10:36:57.758906 fractal_server-1.3.0a5/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19523 2023-06-08 09:22:21.105956 fractal_server-1.3.0a5/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a5/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.3.0a5/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a5/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a5/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19861 2023-05-12 06:48:40.382595 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42200 2023-05-18 09:57:35.703959 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-06-08 08:33:26.930560 fractal_server-1.3.0a5/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a5/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a5/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a5/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a5/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a5/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a5/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a5/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a5/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a5/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a5/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       57 2023-05-26 06:41:57.297956 fractal_server-1.3.0a5/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-05-26 06:41:57.297956 fractal_server-1.3.0a5/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      425 2023-05-26 06:49:50.432129 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1624 2023-06-12 09:13:31.352825 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     4082 2023-06-12 09:13:31.356825 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3551 2023-05-26 06:49:50.436129 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1179 2023-05-26 06:49:50.444129 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     2719 2023-06-12 09:13:31.364825 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     3306 2023-06-12 09:13:31.368826 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1216 2023-05-26 06:49:50.448129 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     3896 2023-05-26 06:49:50.452129 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a5/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-06-12 09:12:04.406676 fractal_server-1.3.0a5/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-12 09:12:04.406676 fractal_server-1.3.0a5/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-05-26 06:41:57.297956 fractal_server-1.3.0a5/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-05-26 06:41:57.297956 fractal_server-1.3.0a5/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-12 09:12:04.406676 fractal_server-1.3.0a5/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-06-12 09:12:04.406676 fractal_server-1.3.0a5/fractal_server/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-05-26 06:41:57.297956 fractal_server-1.3.0a5/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-05-26 06:41:57.297956 fractal_server-1.3.0a5/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1255 2023-06-06 07:10:27.608505 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2806 2023-05-26 06:49:50.864124 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1238 2023-05-26 06:49:50.868124 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2685 2023-05-26 06:49:50.868124 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a5/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a5/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a5/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-12 09:12:04.406676 fractal_server-1.3.0a5/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a5/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a5/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-05-26 06:41:57.297956 fractal_server-1.3.0a5/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-06-12 09:12:04.410676 fractal_server-1.3.0a5/fractal_server/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-05-26 06:41:57.297956 fractal_server-1.3.0a5/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a5/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12164 2023-05-12 12:34:32.122055 fractal_server-1.3.0a5/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a5/fractal_server/logger.py
--rw-r--r--   0        0        0     5849 2023-05-26 06:42:41.017595 fractal_server-1.3.0a5/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a5/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a5/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a5/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2023-06-08 09:21:57.166713 fractal_server-1.3.0a5/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     8770 2023-05-29 15:02:27.725371 fractal_server-1.3.0a5/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0      746 2023-06-08 09:21:57.166713 fractal_server-1.3.0a5/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a5/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a5/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a5/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    17581 2023-06-12 14:10:58.230055 fractal_server-1.3.0a5/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a5/fractal_server/utils.py
--rw-r--r--   0        0        0     2689 2023-06-13 10:03:02.349510 fractal_server-1.3.0a5/pyproject.toml
--rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 fractal_server-1.3.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a6/LICENSE
+-rw-r--r--   0        0        0     2100 2023-06-13 11:33:49.890135 fractal_server-1.3.0a6/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a6/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-06-19 06:52:18.228019 fractal_server-1.3.0a6/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-05-25 12:06:55.503794 fractal_server-1.3.0a6/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a6/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a6/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a6/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a6/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     7616 2023-06-13 11:33:49.890135 fractal_server-1.3.0a6/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     7624 2023-05-23 13:25:45.067972 fractal_server-1.3.0a6/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a6/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a6/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    15912 2023-06-15 09:47:58.010806 fractal_server-1.3.0a6/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    12501 2023-05-29 15:02:27.725371 fractal_server-1.3.0a6/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a6/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a6/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-29 08:51:11.986940 fractal_server-1.3.0a6/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a6/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2355 2023-05-29 08:51:11.986940 fractal_server-1.3.0a6/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2563 2023-05-29 09:51:02.494983 fractal_server-1.3.0a6/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1119 2023-05-29 08:51:11.986940 fractal_server-1.3.0a6/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1591 2023-06-08 09:21:57.166713 fractal_server-1.3.0a6/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5861 2023-06-15 13:41:34.921597 fractal_server-1.3.0a6/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a6/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8969 2023-05-15 10:36:57.758906 fractal_server-1.3.0a6/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19523 2023-06-08 09:22:21.105956 fractal_server-1.3.0a6/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a6/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3245 2023-06-15 13:41:34.921597 fractal_server-1.3.0a6/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a6/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a6/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19766 2023-06-15 13:41:34.921597 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42200 2023-05-18 09:57:35.703959 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-06-08 08:33:26.930560 fractal_server-1.3.0a6/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a6/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a6/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a6/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a6/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a6/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a6/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a6/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       57 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      425 2023-05-26 06:49:50.432129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1624 2023-06-12 09:13:31.352825 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     4082 2023-06-12 09:13:31.356825 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3551 2023-05-26 06:49:50.436129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1179 2023-05-26 06:49:50.444129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     2719 2023-06-12 09:13:31.364825 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     3306 2023-06-12 09:13:31.368826 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1216 2023-05-26 06:49:50.448129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     3896 2023-05-26 06:49:50.452129 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1255 2023-06-15 11:41:13.549879 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2806 2023-05-26 06:49:50.864124 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1349 2023-06-15 11:41:13.553879 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2685 2023-05-26 06:49:50.868124 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a6/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-12 09:12:04.406676 fractal_server-1.3.0a6/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a6/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-06-12 09:12:04.410676 fractal_server-1.3.0a6/fractal_server/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-05-26 06:41:57.297956 fractal_server-1.3.0a6/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a6/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12432 2023-06-15 13:41:27.513642 fractal_server-1.3.0a6/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a6/fractal_server/logger.py
+-rw-r--r--   0        0        0     5935 2023-06-15 13:41:27.513642 fractal_server-1.3.0a6/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a6/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a6/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a6/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2023-06-08 09:21:57.166713 fractal_server-1.3.0a6/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     8770 2023-05-29 15:02:27.725371 fractal_server-1.3.0a6/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0      746 2023-06-08 09:21:57.166713 fractal_server-1.3.0a6/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a6/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a6/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a6/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    17581 2023-06-12 14:10:58.230055 fractal_server-1.3.0a6/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a6/fractal_server/utils.py
+-rw-r--r--   0        0        0     2704 2023-06-19 06:52:18.228019 fractal_server-1.3.0a6/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 fractal_server-1.3.0a6/PKG-INFO
```

### Comparing `fractal_server-1.3.0a5/LICENSE` & `fractal_server-1.3.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/README.md` & `fractal_server-1.3.0a6/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/__main__.py` & `fractal_server-1.3.0a6/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/alembic.ini` & `fractal_server-1.3.0a6/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/api/__init__.py` & `fractal_server-1.3.0a6/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.0a6/fractal_server/app/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.0a6/fractal_server/app/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.0a6/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.0a6/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.0a6/fractal_server/app/api/v1/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,17 +384,20 @@
     db_task = await _get_task_check_owner(task_id=task_id, user=user, db=db)
 
     update = task_update.dict(exclude_unset=True)
     for key, value in update.items():
         if isinstance(value, str):
             setattr(db_task, key, value)
         elif isinstance(value, dict):
-            current_dict = deepcopy(getattr(db_task, key))
-            current_dict.update(value)
-            setattr(db_task, key, current_dict)
+            if key == "args_schema":
+                setattr(db_task, key, value)
+            else:
+                current_dict = deepcopy(getattr(db_task, key))
+                current_dict.update(value)
+                setattr(db_task, key, current_dict)
         else:
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=f"Invalid {type(value)=} for {key=}",
             )
 
     await db.commit()
```

### Comparing `fractal_server-1.3.0a5/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.0a6/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/db/__init__.py` & `fractal_server-1.3.0a6/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/models/job.py` & `fractal_server-1.3.0a6/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/models/project.py` & `fractal_server-1.3.0a6/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/models/security.py` & `fractal_server-1.3.0a6/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/models/state.py` & `fractal_server-1.3.0a6/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/models/task.py` & `fractal_server-1.3.0a6/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/models/workflow.py` & `fractal_server-1.3.0a6/fractal_server/app/models/workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,24 +87,14 @@
     def is_parallel(self) -> bool:
         return self.task.is_parallel
 
     @property
     def parallelization_level(self) -> Union[str, None]:
         return self.task.parallelization_level
 
-    @property
-    def overridden_meta(self) -> dict:
-        """
-        Return a combination of self.meta (higher priority) and self.task.meta
-        (lower priority) key-value pairs.
-        """
-        res = self.task.meta.copy() or {}
-        res.update(self.meta or {})
-        return res
-
 
 class Workflow(_WorkflowBase, SQLModel, table=True):
     """
     Workflow
 
     Attributes:
         id:
@@ -172,16 +162,22 @@
         actual_args = default_args.copy()
         if args is not None:
             for k, v in args.items():
                 actual_args[k] = v
         if not actual_args:
             actual_args = None
 
+        # Combine meta (higher priority) and db_task.meta (lower priority)
+        wt_meta = db_task.meta.copy() or {}
+        wt_meta.update(meta or {})
+        if not wt_meta:
+            wt_meta = None
+
         # Create DB entry
-        wf_task = WorkflowTask(task_id=task_id, args=actual_args, meta=meta)
+        wf_task = WorkflowTask(task_id=task_id, args=actual_args, meta=wt_meta)
         db.add(wf_task)
         self.task_list.insert(order, wf_task)
         self.task_list.reorder()  # type: ignore
         if commit:
             await db.commit()
             await db.refresh(wf_task)
         return wf_task
```

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_common.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_local/_local_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,19 +59,18 @@
 ) -> LocalBackendConfig:
     """
     Prepare a `LocalBackendConfig` configuration object
 
     The sources for `parallel_tasks_per_job` attributes, starting from the
     highest-priority one, are
 
-    1. Properties in `wftask.meta`;
-    2. Properties in `wftask.task.meta` (this is already included in
-       overridden_meta);
-    3. The general content of the local-backend configuration file;
-    4. The default value (`None`).
+    1. Properties in `wftask.meta` (which, for `WorkflowTask`s added through
+       `Workflow.insert_task`, also includes `wftask.task.meta`);
+    2. The general content of the local-backend configuration file;
+    3. The default value (`None`).
 
     Arguments:
         wftask:
             WorkflowTask for which the backend configuration is is to be
             prepared.
         config_path:
             Path of local-backend configuration file; if `None`, use
@@ -80,16 +79,16 @@
     Returns:
         A local-backend configuration object
     """
 
     key = "parallel_tasks_per_job"
     default = None
 
-    if wftask.overridden_meta and key in wftask.overridden_meta.keys():
-        parallel_tasks_per_job = wftask.overridden_meta[key]
+    if wftask.meta and key in wftask.meta:
+        parallel_tasks_per_job = wftask.meta[key]
     else:
         if not config_path:
             settings = Inject(get_settings)
             config_path = settings.FRACTAL_LOCAL_CONFIG_FILE
         if config_path is None:
             parallel_tasks_per_job = default
         else:
@@ -100,9 +99,8 @@
             except ValidationError as e:
                 raise LocalBackendConfigError(
                     f"Error while loading {config_path=}. "
                     f"Original error:\n{str(e)}"
                 )
 
             parallel_tasks_per_job = env.get(key, default)
-
     return LocalBackendConfig(parallel_tasks_per_job=parallel_tasks_per_job)
```

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -466,16 +466,17 @@
     Prepare a `SlurmConfig` configuration object
 
     The sources for `SlurmConfig` attributes, in increasing priority order, are
 
     1. The general content of the Fractal SLURM configuration file.
     2. The GPU-specific content of the Fractal SLURM configuration file, if
         appropriate.
-    3. Properties in `wftask.task.meta`.
-    4. Properties in `wftask.meta`.
+    3. Properties in `wftask.meta` (which, for `WorkflowTask`s added through
+       `Workflow.insert_task`, also includes `wftask.task.meta`);
+
 
     Arguments:
         wftask:
             WorkflowTask for which the SLURM configuration is is to be
             prepared.
         workflow_dir:
             Server-owned directory to store all task-execution-related relevant
@@ -490,16 +491,15 @@
 
     Returns:
         slurm_config:
             The SlurmConfig object
     """
 
     logger.debug(
-        "[get_slurm_config] WorkflowTask/Task meta attribute: "
-        f"{wftask.overridden_meta=}"
+        "[get_slurm_config] WorkflowTask meta attribute: " f"{wftask.meta=}"
     )
 
     # Incorporate slurm_env.default_slurm_config
     slurm_env = load_slurm_config_file(config_path=config_path)
     slurm_dict = slurm_env.default_slurm_config.dict(
         exclude_unset=True, exclude={"mem"}
     )
@@ -519,60 +519,58 @@
     )
 
     # GPU-related options
     # Notes about priority:
     # 1. This block of definitions takes priority over other definitions from
     #    slurm_env which are not under the `needs_gpu` subgroup
     # 2. This block of definitions has lower priority than whatever comes next
-    #    (i.e. from WorkflowTask.overridden_meta).
-    needs_gpu = wftask.overridden_meta.get("needs_gpu", False)
+    #    (i.e. from WorkflowTask.meta).
+    needs_gpu = wftask.meta.get("needs_gpu", False)
     logger.debug(f"[get_slurm_config] {needs_gpu=}")
     if needs_gpu:
         for key, value in slurm_env.gpu_slurm_config.dict(
             exclude_unset=True, exclude={"mem"}
         ).items():
             slurm_dict[key] = value
         if slurm_env.gpu_slurm_config.mem:
             slurm_dict["mem_per_task_MB"] = slurm_env.gpu_slurm_config.mem
 
     # Number of CPUs per task, for multithreading
-    if "cpus_per_task" in wftask.overridden_meta.keys():
-        cpus_per_task = int(wftask.overridden_meta["cpus_per_task"])
+    if "cpus_per_task" in wftask.meta:
+        cpus_per_task = int(wftask.meta["cpus_per_task"])
         slurm_dict["cpus_per_task"] = cpus_per_task
 
     # Required memory per task, in MB
-    if "mem" in wftask.overridden_meta.keys():
-        raw_mem = wftask.overridden_meta["mem"]
+    if "mem" in wftask.meta:
+        raw_mem = wftask.meta["mem"]
         mem_per_task_MB = _parse_mem_value(raw_mem)
         slurm_dict["mem_per_task_MB"] = mem_per_task_MB
 
     # Job name
     job_name = wftask.task.name.replace(" ", "_")
     slurm_dict["job_name"] = job_name
 
     # Optional SLURM arguments and extra lines
     for key in ["time", "account", "gres", "constraint"]:
-        value = wftask.overridden_meta.get(key, None)
+        value = wftask.meta.get(key, None)
         if value:
             slurm_dict[key] = value
-    extra_lines = wftask.overridden_meta.get("extra_lines", [])
+    extra_lines = wftask.meta.get("extra_lines", [])
     extra_lines = slurm_dict.get("extra_lines", []) + extra_lines
     if len(set(extra_lines)) != len(extra_lines):
         logger.debug(
             "[get_slurm_config] Removing repeated elements "
             f"from {extra_lines=}."
         )
         extra_lines = list(set(extra_lines))
     slurm_dict["extra_lines"] = extra_lines
 
     # Job-batching parameters (if None, they will be determined heuristically)
-    tasks_per_job = wftask.overridden_meta.get("tasks_per_job", None)
-    parallel_tasks_per_job = wftask.overridden_meta.get(
-        "parallel_tasks_per_job", None
-    )
+    tasks_per_job = wftask.meta.get("tasks_per_job", None)
+    parallel_tasks_per_job = wftask.meta.get("parallel_tasks_per_job", None)
     slurm_dict["tasks_per_job"] = tasks_per_job
     slurm_dict["parallel_tasks_per_job"] = parallel_tasks_per_job
 
     # Put everything together
     logger.debug(
         "[get_slurm_config] Now create a SlurmConfig object based "
         f"on {slurm_dict=}"
```

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/runner/common.py` & `fractal_server-1.3.0a6/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/app/security/__init__.py` & `fractal_server-1.3.0a6/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.0a6/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.0a6/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/README.md` & `fractal_server-1.3.0a6/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.3.0a6/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/project.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/state.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/task.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/task_collection.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/user.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.0a6/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 07:08:01 2023 UTC, .py size: 1420 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 51db 7e64 8c05 0000  o.......Q.~d....
+00000000: 6f0d 0d0a 0000 0000 64e1 8664 8c05 0000  o.......d..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
```

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 06:41:57 2023 UTC, .py size: 773 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 6f0d 0d0a 0000 0000 b554 7064 0503 0000  o........Tpd....
+00000000: 6f0d 0d0a 0000 0000 64e1 8664 c803 0000  o.......d..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
 00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
 00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
 000000a0: 7272 6f72 2901 da0e 5461 736b 436f 6c6c  rror)...TaskColl
 000000b0: 6563 7450 6970 6300 0000 0000 0000 0000  ectPipc.........
 000000c0: 0000 0002 0000 0008 0000 0043 0000 0073  ...........C...s
-000000d0: 7a01 0000 7400 6401 6402 8d01 7d00 7401  z...t.d.d...}.t.
+000000d0: bc01 0000 7400 6401 6402 8d01 7d00 7401  ....t.d.d...}.t.
 000000e0: 7c00 8301 0100 7c00 7328 6403 6404 6405  |.....|.s(d.d.d.
 000000f0: 7402 a003 a100 7600 7318 7404 a005 7c00  t.....v.s.t...|.
 00000100: a101 721d 7404 a006 7c00 a101 6e01 6405  ..r.t...|...n.d.
 00000110: 6901 1600 7d01 7407 7404 a008 7c01 a101  i...}.t.t...|...
 00000120: 8301 8201 7400 6406 6402 8d01 7d00 7401  ....t.d.d...}.t.
 00000130: 7c00 8301 0100 7c00 7350 6403 6404 6405  |.....|.sPd.d.d.
 00000140: 7402 a003 a100 7600 7340 7404 a005 7c00  t.....v.s@t...|.
@@ -27,52 +27,59 @@
 000001a0: 0100 0100 5900 0100 7409 a00a 740b a101  ....Y...t...t...
 000001b0: 8f0d 0100 7400 6408 6402 8d01 7d00 5700  ....t.d.d...}.W.
 000001c0: 6400 0400 0400 8303 0100 6e08 3100 737f  d.........n.1.s.
 000001d0: 7701 0100 0100 0100 5900 0100 7409 a00a  w.......Y...t...
 000001e0: 740b a101 8f0e 0100 7400 6401 6409 640a  t.......t.d.d.d.
 000001f0: 8d02 7d00 5700 6400 0400 0400 8303 0100  ..}.W.d.........
 00000200: 6e08 3100 739a 7701 0100 0100 0100 5900  n.1.s.w.......Y.
-00000210: 0100 7409 a00a 740b a101 8f0f 0100 7400  ..t...t.......t.
+00000210: 0100 7409 a00a 740b a101 8f0e 0100 7400  ..t...t.......t.
 00000220: 6401 6400 640a 8d02 7d00 5700 6400 0400  d.d.d...}.W.d...
-00000230: 0400 8303 0100 6400 5300 3100 73b6 7701  ......d.S.1.s.w.
-00000240: 0100 0100 0100 5900 0100 6400 5300 290b  ......Y...d.S.).
-00000250: 4e7a 0c73 6f6d 652d 7061 636b 6167 6529  Nz.some-package)
-00000260: 01da 0770 6163 6b61 6765 7a0e 6173 7365  ...packagez.asse
-00000270: 7274 2025 2870 7930 2973 da03 7079 30da  rt %(py0)s..py0.
-00000280: 0163 7a11 2f73 6f6d 652f 7061 636b 6167  .cz./some/packag
-00000290: 652e 7768 6c7a 0c73 6f6d 652f 7061 636b  e.whlz.some/pack
-000002a0: 6167 657a 142f 736f 6d65 2f70 6163 6b61  agez./some/packa
-000002b0: 6765 2e74 6172 2e67 7ada 0029 0272 0500  ge.tar.gz..).r..
-000002c0: 0000 da0e 7061 636b 6167 655f 6578 7472  ....package_extr
-000002d0: 6173 290c 7204 0000 0072 0200 0000 da0c  as).r....r......
-000002e0: 4070 795f 6275 696c 7469 6e73 da06 6c6f  @py_builtins..lo
-000002f0: 6361 6c73 da0a 4070 7974 6573 745f 6172  cals..@pytest_ar
-00000300: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
-00000310: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
-00000320: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
-00000330: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
-00000340: 7870 6c61 6e61 7469 6f6e da06 7079 7465  xplanation..pyte
-00000350: 7374 da06 7261 6973 6573 7203 0000 0029  st..raisesr....)
-00000360: 0272 0700 0000 da0b 4070 795f 666f 726d  .r......@py_form
-00000370: 6174 31a9 0072 1400 0000 fa58 2f68 6f6d  at1..r.....X/hom
-00000380: 652f 746f 6d6d 6173 6f2f 4672 6163 7461  e/tommaso/Fracta
-00000390: 6c2f 6672 6163 7461 6c2d 7365 7276 6572  l/fractal-server
-000003a0: 2f66 7261 6374 616c 5f73 6572 7665 722f  /fractal_server/
-000003b0: 636f 6d6d 6f6e 2f74 6573 7473 2f74 6573  common/tests/tes
-000003c0: 745f 7461 736b 5f63 6f6c 6c65 6374 696f  t_task_collectio
-000003d0: 6e2e 7079 da13 7465 7374 5f54 6173 6b43  n.py..test_TaskC
-000003e0: 6f6c 6c65 6374 5069 7008 0000 0073 2400  ollectPip....s$.
-000003f0: 0000 0a02 0801 3e01 0a01 0801 3e01 0c02  ......>.....>...
-00000400: 0c01 1cff 0c02 0c01 1cff 0c02 0e01 1cff  ................
-00000410: 0c02 0e01 22ff 7216 0000 0029 0eda 0862  ....".r....)...b
-00000420: 7569 6c74 696e 7372 0a00 0000 da19 5f70  uiltinsr......_p
-00000430: 7974 6573 742e 6173 7365 7274 696f 6e2e  ytest.assertion.
-00000440: 7265 7772 6974 65da 0961 7373 6572 7469  rewrite..asserti
-00000450: 6f6e da07 7265 7772 6974 6572 0c00 0000  on..rewriter....
-00000460: 7211 0000 00da 0864 6576 746f 6f6c 7372  r......devtoolsr
-00000470: 0200 0000 da17 7079 6461 6e74 6963 2e65  ......pydantic.e
-00000480: 7272 6f72 5f77 7261 7070 6572 7372 0300  rror_wrappersr..
-00000490: 0000 da07 7363 6865 6d61 7372 0400 0000  ....schemasr....
-000004a0: 7216 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-000004b0: 1400 0000 7215 0000 00da 083c 6d6f 6475  ....r......<modu
-000004c0: 6c65 3e01 0000 0073 0a00 0000 2200 0c01  le>....s...."...
-000004d0: 0c01 0c02 0c03                           ......
+00000230: 0400 8303 0100 6e08 3100 73b5 7701 0100  ......n.1.s.w...
+00000240: 0100 0100 5900 0100 7400 6401 6900 640b  ....Y...t.d.i.d.
+00000250: 8d02 7d00 7409 a00a 740b a101 8f0f 0100  ..}.t...t.......
+00000260: 7400 6401 640c 640b 8d02 7d00 5700 6400  t.d.d.d...}.W.d.
+00000270: 0400 0400 8303 0100 6400 5300 3100 73d7  ........d.S.1.s.
+00000280: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
+00000290: 290d 4e7a 0c73 6f6d 652d 7061 636b 6167  ).Nz.some-packag
+000002a0: 6529 01da 0770 6163 6b61 6765 7a0e 6173  e)...packagez.as
+000002b0: 7365 7274 2025 2870 7930 2973 da03 7079  sert %(py0)s..py
+000002c0: 30da 0163 7a11 2f73 6f6d 652f 7061 636b  0..cz./some/pack
+000002d0: 6167 652e 7768 6c7a 0c73 6f6d 652f 7061  age.whlz.some/pa
+000002e0: 636b 6167 657a 142f 736f 6d65 2f70 6163  ckagez./some/pac
+000002f0: 6b61 6765 2e74 6172 2e67 7ada 0029 0272  kage.tar.gz..).r
+00000300: 0500 0000 da0e 7061 636b 6167 655f 6578  ......package_ex
+00000310: 7472 6173 2902 7205 0000 00da 1770 696e  tras).r......pin
+00000320: 6e65 645f 7061 636b 6167 655f 7665 7273  ned_package_vers
+00000330: 696f 6e73 e901 0000 0029 0c72 0400 0000  ions.....).r....
+00000340: 7202 0000 00da 0c40 7079 5f62 7569 6c74  r......@py_built
+00000350: 696e 73da 066c 6f63 616c 73da 0a40 7079  ins..locals..@py
+00000360: 7465 7374 5f61 72da 185f 7368 6f75 6c64  test_ar.._should
+00000370: 5f72 6570 725f 676c 6f62 616c 5f6e 616d  _repr_global_nam
+00000380: 65da 095f 7361 6665 7265 7072 da0e 4173  e.._saferepr..As
+00000390: 7365 7274 696f 6e45 7272 6f72 da13 5f66  sertionError.._f
+000003a0: 6f72 6d61 745f 6578 706c 616e 6174 696f  ormat_explanatio
+000003b0: 6eda 0670 7974 6573 74da 0672 6169 7365  n..pytest..raise
+000003c0: 7372 0300 0000 2902 7207 0000 00da 0b40  sr....).r......@
+000003d0: 7079 5f66 6f72 6d61 7431 a900 7216 0000  py_format1..r...
+000003e0: 00fa 582f 686f 6d65 2f74 6f6d 6d61 736f  ..X/home/tommaso
+000003f0: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
+00000400: 2d73 6572 7665 722f 6672 6163 7461 6c5f  -server/fractal_
+00000410: 7365 7276 6572 2f63 6f6d 6d6f 6e2f 7465  server/common/te
+00000420: 7374 732f 7465 7374 5f74 6173 6b5f 636f  sts/test_task_co
+00000430: 6c6c 6563 7469 6f6e 2e70 79da 1374 6573  llection.py..tes
+00000440: 745f 5461 736b 436f 6c6c 6563 7450 6970  t_TaskCollectPip
+00000450: 0800 0000 732c 0000 000a 0208 013e 010a  ....s,.......>..
+00000460: 0108 013e 010c 020c 011c ff0c 020c 011c  ...>............
+00000470: ff0c 020e 011c ff0c 020e 011c ff0c 030c  ................
+00000480: 010e 0122 ff72 1800 0000 290e da08 6275  ...".r....)...bu
+00000490: 696c 7469 6e73 720c 0000 00da 195f 7079  iltinsr......_py
+000004a0: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
+000004b0: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
+000004c0: 6eda 0772 6577 7269 7465 720e 0000 0072  n..rewriter....r
+000004d0: 1300 0000 da08 6465 7674 6f6f 6c73 7202  ......devtoolsr.
+000004e0: 0000 00da 1770 7964 616e 7469 632e 6572  .....pydantic.er
+000004f0: 726f 725f 7772 6170 7065 7273 7203 0000  ror_wrappersr...
+00000500: 00da 0773 6368 656d 6173 7204 0000 0072  ...schemasr....r
+00000510: 1800 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
+00000520: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000530: 653e 0100 0000 730a 0000 0022 000c 010c  e>....s...."....
+00000540: 010c 020c 03                             .....
```

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a6/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.0a6/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.3.0a6/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.0a6/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.0a6/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/test_task.py` & `fractal_server-1.3.0a6/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/test_task_collection.py` & `fractal_server-1.3.0a6/fractal_server/common/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.0a6/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.0a6/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/config.py` & `fractal_server-1.3.0a6/fractal_server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,23 @@
     Admin default password, used upon creation of the first superuser during
     server startup.
 
     **IMPORTANT**: After the server startup, you should always edit the default
     admin credentials.
     """
 
+    FRACTAL_DEFAULT_ADMIN_USERNAME: str = "admin"
+    """
+    Admin default username, used upon creation of the first superuser during
+    server startup.
+
+    **IMPORTANT**: After the server startup, you should always edit the default
+    admin credentials.
+    """
+
     FRACTAL_TASKS_DIR: Optional[Path]
     """
     Directory under which all the tasks will be saved.
     """
 
     FRACTAL_RUNNER_BACKEND: Literal["local", "slurm"] = "local"
     """
```

### Comparing `fractal_server-1.3.0a5/fractal_server/logger.py` & `fractal_server-1.3.0a6/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/main.py` & `fractal_server-1.3.0a6/fractal_server/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,12 +178,13 @@
     """
     Register the starup calls
 
     If the calls raise any error, the application startup is aborted.
     """
     settings = Inject(get_settings)
     await _create_first_user(
-        settings.FRACTAL_DEFAULT_ADMIN_EMAIL,
-        settings.FRACTAL_DEFAULT_ADMIN_PASSWORD,
-        True,
+        email=settings.FRACTAL_DEFAULT_ADMIN_EMAIL,
+        password=settings.FRACTAL_DEFAULT_ADMIN_PASSWORD,
+        is_superuser=True,
+        username=settings.FRACTAL_DEFAULT_ADMIN_USERNAME,
     )
     await __on_startup()
```

### Comparing `fractal_server-1.3.0a5/fractal_server/migrations/env.py` & `fractal_server-1.3.0a6/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.0a6/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-1.3.0a6/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-1.3.0a6/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-1.3.0a6/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/syringe.py` & `fractal_server-1.3.0a6/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/tasks/collection.py` & `fractal_server-1.3.0a6/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/fractal_server/utils.py` & `fractal_server-1.3.0a6/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a5/pyproject.toml` & `fractal_server-1.3.0a6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.0a5"
+version = "1.3.0a6"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -19,14 +19,15 @@
 sqlmodel = "^0.0.8"
 aiosqlite = "^0.17.0"
 fastapi-users = {extras = ["oauth"], version = "^10.1"}
 alembic = "^1.9.1"
 uvicorn = "^0.20.0"
 sqlalchemy = "^1.4"
 SQLAlchemy-Utils = "^0.38.3"
+greenlet = "*"
 pydantic = ">=1.10.8"
 
 clusterfutures = { version = "^0.5", optional = true}
 cloudpickle = {version = ">=2.2.1 <2.3.0", optional = true}
 
 asyncpg = { version = "^0.27.0", optional = true }
 psycopg2 = { version = "^2.9.5", optional = true }
@@ -72,15 +73,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.0a5"
+current_version = "1.3.0a6"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.0a5/PKG-INFO` & `fractal_server-1.3.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.0a5
+Version: 1.3.0a6
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -19,14 +19,15 @@
 Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
 Requires-Dist: alembic (>=1.9.1,<2.0.0)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0) ; extra == "postgres"
 Requires-Dist: cloudpickle (>=2.2.1,<2.3.0) ; extra == "slurm"
 Requires-Dist: clusterfutures (>=0.5,<0.6) ; extra == "slurm"
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: fastapi-users[oauth] (>=10.1,<11.0)
+Requires-Dist: greenlet
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "gunicorn"
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
 Requires-Dist: pydantic (>=1.10.8)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
```

