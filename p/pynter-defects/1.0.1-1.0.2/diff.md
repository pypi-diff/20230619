# Comparing `tmp/pynter-defects-1.0.1.tar.gz` & `tmp/pynter-defects-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynter-defects-1.0.1.tar", last modified: Thu Jun 15 16:31:06 2023, max compression
+gzip compressed data, was "pynter-defects-1.0.2.tar", last modified: Mon Jun 19 09:32:07 2023, max compression
```

## Comparing `pynter-defects-1.0.1.tar` & `pynter-defects-1.0.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:06.096874 pynter-defects-1.0.1/
--rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-15 16:31:06.088874 pynter-defects-1.0.1/PKG-INFO
--rwxrwxr-x   0 villa     (1123) villa     (1123)      299 2022-01-18 18:41:16.000000 pynter-defects-1.0.1/README.md
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:03.884925 pynter-defects-1.0.1/pynter/
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1793 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/__init__.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:03.992923 pynter-defects-1.0.1/pynter/automations/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/automations/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     6625 2023-05-30 14:13:48.000000 pynter-defects-1.0.1/pynter/automations/core.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    20887 2023-05-30 14:17:51.000000 pynter-defects-1.0.1/pynter/automations/vasp.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:04.352914 pynter-defects-1.0.1/pynter/cli/
--rw-rw-r--   0 villa     (1123) villa     (1123)     3416 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3410 2023-05-31 09:10:02.000000 pynter-defects-1.0.1/pynter/cli/automations.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6876 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/config.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    17275 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     5371 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/hpc.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6375 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/inputs.py
--rwxrwxr--   0 villa     (1123) villa     (1123)     1493 2023-06-05 15:11:39.000000 pynter-defects-1.0.1/pynter/cli/main.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1732 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/materials_project.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     4062 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/phase_diagram.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     7896 2023-05-31 09:33:54.000000 pynter-defects-1.0.1/pynter/cli/plotter.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3782 2023-06-02 14:17:35.000000 pynter-defects-1.0.1/pynter/cli/slurm.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1452 2023-06-05 09:25:02.000000 pynter-defects-1.0.1/pynter/cli/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:04.424913 pynter-defects-1.0.1/pynter/data/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/data/__init__.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:04.512911 pynter-defects-1.0.1/pynter/data/database/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        3 2020-11-13 14:36:46.000000 pynter-defects-1.0.1/pynter/data/database/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     2179 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/data/database/creator.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     5713 2022-01-18 18:41:16.000000 pynter-defects-1.0.1/pynter/data/database/query.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    29512 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/data/datasets.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    11765 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/data/jobs.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:04.980900 pynter-defects-1.0.1/pynter/defects/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/defects/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    45917 2023-06-02 12:11:11.000000 pynter-defects-1.0.1/pynter/defects/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    10821 2023-05-03 16:47:07.000000 pynter-defects-1.0.1/pynter/defects/corrections.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    35277 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/defects/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6471 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/defects/elasticity.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    11914 2023-05-31 16:46:23.000000 pynter-defects-1.0.1/pynter/defects/entries.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    15353 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/defects/plotter.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.112897 pynter-defects-1.0.1/pynter/defects/pmg/
--rwxrwxr-x   0 villa     (1123) villa     (1123)    24611 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_core.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    39163 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_corrections.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    60074 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_utils.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    39933 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/pmg/pmg_dos.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    12053 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/defects/structure.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    19876 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/defects/thermodynamics.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)      994 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.212895 pynter-defects-1.0.1/pynter/phase_diagram/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/phase_diagram/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    32436 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/phase_diagram/chempots.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     7430 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/phase_diagram/plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10388 2023-06-15 16:23:42.000000 pynter-defects-1.0.1/pynter/phase_diagram/thermodynamics.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.312892 pynter-defects-1.0.1/pynter/slurm/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/slurm/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9065 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/slurm/interface.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10416 2023-06-12 14:42:45.000000 pynter-defects-1.0.1/pynter/slurm/job_script.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1486 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/slurm/job_status.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.528887 pynter-defects-1.0.1/pynter/testing/
--rw-rw-r--   0 villa     (1123) villa     (1123)     2363 2023-06-15 16:23:42.000000 pynter-defects-1.0.1/pynter/testing/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6067 2023-06-15 16:23:42.000000 pynter-defects-1.0.1/pynter/testing/core.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     2574 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/data.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1285 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1493 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/phase_diagram.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      988 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/slurm.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      916 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/structure.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     4923 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/vasp.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.680884 pynter-defects-1.0.1/pynter/tools/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/tools/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1038 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/tools/format.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     7422 2023-06-02 12:18:36.000000 pynter-defects-1.0.1/pynter/tools/materials_project.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      251 2022-01-18 18:41:18.000000 pynter-defects-1.0.1/pynter/tools/plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9866 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/tools/structure.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     8433 2023-05-31 15:51:51.000000 pynter-defects-1.0.1/pynter/tools/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.884879 pynter-defects-1.0.1/pynter/vasp/
--rwxrwxr-x   0 villa     (1123) villa     (1123)      872 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/vasp/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9438 2022-01-18 18:41:18.000000 pynter-defects-1.0.1/pynter/vasp/analysis.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10352 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/vasp/default_inputs.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    36627 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/vasp/jobs.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     6192 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/vasp/plotter.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.904878 pynter-defects-1.0.1/pynter/vasp/pmg/
--rw-rw-r--   0 villa     (1123) villa     (1123)   183623 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    51500 2023-06-05 12:14:41.000000 pynter-defects-1.0.1/pynter/vasp/schemes.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     3845 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/vasp/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:06.072875 pynter-defects-1.0.1/pynter_defects.egg-info/
--rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/PKG-INFO
--rw-rw-r--   0 villa     (1123) villa     (1123)     2037 2023-06-15 16:31:03.000000 pynter-defects-1.0.1/pynter_defects.egg-info/SOURCES.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)        1 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/dependency_links.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       48 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/entry_points.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       89 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/requires.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       23 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/top_level.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       38 2023-06-15 16:31:06.100874 pynter-defects-1.0.1/setup.cfg
--rw-rw-r--   0 villa     (1123) villa     (1123)      703 2023-06-15 16:30:04.000000 pynter-defects-1.0.1/setup.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.276624 pynter-defects-1.0.2/
+-rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-19 09:32:07.276624 pynter-defects-1.0.2/PKG-INFO
+-rwxrwxr-x   0 villa     (1123) villa     (1123)      731 2023-06-16 16:30:53.000000 pynter-defects-1.0.2/README.md
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.288646 pynter-defects-1.0.2/pynter/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     1793 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/__init__.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.316645 pynter-defects-1.0.2/pynter/automations/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/automations/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     6625 2023-05-30 14:13:48.000000 pynter-defects-1.0.2/pynter/automations/core.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    20887 2023-05-30 14:17:51.000000 pynter-defects-1.0.2/pynter/automations/vasp.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.496641 pynter-defects-1.0.2/pynter/cli/
+-rw-rw-r--   0 villa     (1123) villa     (1123)     3416 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/analysis.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     3410 2023-05-31 09:10:02.000000 pynter-defects-1.0.2/pynter/cli/automations.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     6964 2023-06-16 17:17:43.000000 pynter-defects-1.0.2/pynter/cli/config.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    17275 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/defects.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     5371 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/hpc.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     6375 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/inputs.py
+-rwxrwxr--   0 villa     (1123) villa     (1123)     2039 2023-06-16 17:20:40.000000 pynter-defects-1.0.2/pynter/cli/main.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     1732 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/materials_project.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     4062 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/phase_diagram.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     7896 2023-05-31 09:33:54.000000 pynter-defects-1.0.2/pynter/cli/plotter.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     3782 2023-06-02 14:17:35.000000 pynter-defects-1.0.2/pynter/cli/slurm.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     1452 2023-06-05 09:25:02.000000 pynter-defects-1.0.2/pynter/cli/utils.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.524641 pynter-defects-1.0.2/pynter/data/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/data/__init__.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.580639 pynter-defects-1.0.2/pynter/data/database/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        3 2020-11-13 14:36:46.000000 pynter-defects-1.0.2/pynter/data/database/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     2179 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/data/database/creator.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     5713 2022-01-18 18:41:16.000000 pynter-defects-1.0.2/pynter/data/database/query.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    29512 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/data/datasets.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    11765 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/data/jobs.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.724636 pynter-defects-1.0.2/pynter/defects/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/defects/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    45917 2023-06-02 12:11:11.000000 pynter-defects-1.0.2/pynter/defects/analysis.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    10821 2023-05-03 16:47:07.000000 pynter-defects-1.0.2/pynter/defects/corrections.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    35277 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/defects/defects.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     6471 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/defects/elasticity.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    11914 2023-05-31 16:46:23.000000 pynter-defects-1.0.2/pynter/defects/entries.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    15353 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/defects/plotter.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.804635 pynter-defects-1.0.2/pynter/defects/pmg/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    24611 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_core.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    39163 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_corrections.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    60074 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_utils.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    39933 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/pmg/pmg_dos.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    12053 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/defects/structure.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    19876 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/defects/thermodynamics.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)      994 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/utils.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.864633 pynter-defects-1.0.2/pynter/phase_diagram/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/phase_diagram/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    32436 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/phase_diagram/chempots.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     7430 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/phase_diagram/plotter.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    10388 2023-06-15 16:23:42.000000 pynter-defects-1.0.2/pynter/phase_diagram/thermodynamics.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.920632 pynter-defects-1.0.2/pynter/slurm/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/slurm/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     9065 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/slurm/interface.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    10416 2023-06-12 14:42:45.000000 pynter-defects-1.0.2/pynter/slurm/job_script.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     1486 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/slurm/job_status.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.004630 pynter-defects-1.0.2/pynter/testing/
+-rw-rw-r--   0 villa     (1123) villa     (1123)     2363 2023-06-15 16:23:42.000000 pynter-defects-1.0.2/pynter/testing/__init__.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     6067 2023-06-15 16:23:42.000000 pynter-defects-1.0.2/pynter/testing/core.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     2574 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/data.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     1285 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/defects.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     1493 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/phase_diagram.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)      988 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/slurm.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)      916 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/structure.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     4923 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/vasp.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.084628 pynter-defects-1.0.2/pynter/tools/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/tools/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     1038 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/tools/format.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     7422 2023-06-02 12:18:36.000000 pynter-defects-1.0.2/pynter/tools/materials_project.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)      251 2022-01-18 18:41:18.000000 pynter-defects-1.0.2/pynter/tools/plotter.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     9866 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/tools/structure.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     8433 2023-05-31 15:51:51.000000 pynter-defects-1.0.2/pynter/tools/utils.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.224625 pynter-defects-1.0.2/pynter/vasp/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)      872 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/vasp/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     9438 2022-01-18 18:41:18.000000 pynter-defects-1.0.2/pynter/vasp/analysis.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    10352 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/vasp/default_inputs.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    36627 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/vasp/jobs.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     6192 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/vasp/plotter.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.228625 pynter-defects-1.0.2/pynter/vasp/pmg/
+-rw-rw-r--   0 villa     (1123) villa     (1123)   183623 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    51500 2023-06-05 12:14:41.000000 pynter-defects-1.0.2/pynter/vasp/schemes.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     3845 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/vasp/utils.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.272624 pynter-defects-1.0.2/pynter_defects.egg-info/
+-rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/PKG-INFO
+-rw-rw-r--   0 villa     (1123) villa     (1123)     2037 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/SOURCES.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)        1 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/dependency_links.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)       48 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/entry_points.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)       89 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/requires.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)       18 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/top_level.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)       38 2023-06-19 09:32:07.276624 pynter-defects-1.0.2/setup.cfg
+-rw-rw-r--   0 villa     (1123) villa     (1123)      703 2023-06-19 09:17:15.000000 pynter-defects-1.0.2/setup.py
```

### Comparing `pynter-defects-1.0.1/pynter/__init__.py` & `pynter-defects-1.0.2/pynter/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/automations/core.py` & `pynter-defects-1.0.2/pynter/automations/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/automations/vasp.py` & `pynter-defects-1.0.2/pynter/automations/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/analysis.py` & `pynter-defects-1.0.2/pynter/cli/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/automations.py` & `pynter-defects-1.0.2/pynter/cli/automations.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/config.py` & `pynter-defects-1.0.2/pynter/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,34 @@
                                default=None,metavar='',dest='exclude')
     parser_configure.add_argument('-i','--info',action='store_true',help='Print configuration files paths',
                                default=False,dest='info')
     parser_configure.set_defaults(func=create_config)
     
     return
   
-    
+
 def create_config(args):
+    run_config(exclude=args.exclude,info=args.info)
+    return
+  
+def run_config(exclude=None,info=False):
     
     filename_config = 'config.yml'
     filename_vasp = 'vasp.yml'
     filepath = os.path.join(os.getenv("HOME"),'.pynter')
     
     # print configuration files path
-    if args.info:
+    if info:
         print('Path of general configuration file: %s' %(os.path.join(filepath,filename_config)))
         print('Path of vasp configuration file: %s' %(os.path.join(filepath,filename_vasp)))
         return
 
     # Set config.yml
-    if args.exclude != filename_config:
-        print('Set up configuration file for pynter...\n\n')
+    if exclude != filename_config:
+        print('\nSet up configuration file for pynter...\n')
         print('Path of configuration file is: %s' %filepath)
         if not os.path.exists(filepath):
             os.makedirs(filepath)
         
         filename = filename_config
         
         print('Begin setup\n')
@@ -223,15 +227,15 @@
       'Xe': 'Xe',
       'Y': 'Y_sv',
       'Yb': 'Yb_2',
       'Zn': 'Zn',
       'Zr': 'Zr_sv'}}
     
     # set vasp.yml
-    if args.exclude != filename_vasp:
+    if exclude != filename_vasp:
     
         filename = filename_vasp
         
         with open(os.path.join(filepath,filename),'w+') as f:
             yaml.dump(vasp_default,f) 
         
         print(f'Vasp default file {filename} written in {filepath}')
```

### Comparing `pynter-defects-1.0.1/pynter/cli/defects.py` & `pynter-defects-1.0.2/pynter/cli/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/hpc.py` & `pynter-defects-1.0.2/pynter/cli/hpc.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/inputs.py` & `pynter-defects-1.0.2/pynter/cli/inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/materials_project.py` & `pynter-defects-1.0.2/pynter/cli/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/phase_diagram.py` & `pynter-defects-1.0.2/pynter/cli/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/plotter.py` & `pynter-defects-1.0.2/pynter/cli/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/slurm.py` & `pynter-defects-1.0.2/pynter/cli/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/cli/utils.py` & `pynter-defects-1.0.2/pynter/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/data/database/creator.py` & `pynter-defects-1.0.2/pynter/data/database/creator.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/data/database/query.py` & `pynter-defects-1.0.2/pynter/data/database/query.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/data/datasets.py` & `pynter-defects-1.0.2/pynter/data/datasets.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/data/jobs.py` & `pynter-defects-1.0.2/pynter/data/jobs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/analysis.py` & `pynter-defects-1.0.2/pynter/defects/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/corrections.py` & `pynter-defects-1.0.2/pynter/defects/corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/defects.py` & `pynter-defects-1.0.2/pynter/defects/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/elasticity.py` & `pynter-defects-1.0.2/pynter/defects/elasticity.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/entries.py` & `pynter-defects-1.0.2/pynter/defects/entries.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/plotter.py` & `pynter-defects-1.0.2/pynter/defects/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_core.py` & `pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_corrections.py` & `pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_utils.py` & `pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/pmg/pmg_dos.py` & `pynter-defects-1.0.2/pynter/defects/pmg/pmg_dos.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/structure.py` & `pynter-defects-1.0.2/pynter/defects/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/thermodynamics.py` & `pynter-defects-1.0.2/pynter/defects/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/defects/utils.py` & `pynter-defects-1.0.2/pynter/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/phase_diagram/chempots.py` & `pynter-defects-1.0.2/pynter/phase_diagram/chempots.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/phase_diagram/plotter.py` & `pynter-defects-1.0.2/pynter/phase_diagram/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/phase_diagram/thermodynamics.py` & `pynter-defects-1.0.2/pynter/phase_diagram/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/slurm/interface.py` & `pynter-defects-1.0.2/pynter/slurm/interface.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/slurm/job_script.py` & `pynter-defects-1.0.2/pynter/slurm/job_script.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/slurm/job_status.py` & `pynter-defects-1.0.2/pynter/slurm/job_status.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/testing/__init__.py` & `pynter-defects-1.0.2/pynter/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/testing/core.py` & `pynter-defects-1.0.2/pynter/testing/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/testing/data.py` & `pynter-defects-1.0.2/pynter/testing/data.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/testing/defects.py` & `pynter-defects-1.0.2/pynter/testing/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/testing/phase_diagram.py` & `pynter-defects-1.0.2/pynter/testing/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/testing/slurm.py` & `pynter-defects-1.0.2/pynter/testing/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/testing/structure.py` & `pynter-defects-1.0.2/pynter/testing/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/testing/vasp.py` & `pynter-defects-1.0.2/pynter/testing/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/tools/format.py` & `pynter-defects-1.0.2/pynter/tools/format.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/tools/materials_project.py` & `pynter-defects-1.0.2/pynter/tools/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/tools/structure.py` & `pynter-defects-1.0.2/pynter/tools/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/tools/utils.py` & `pynter-defects-1.0.2/pynter/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/vasp/__init__.py` & `pynter-defects-1.0.2/pynter/vasp/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/vasp/analysis.py` & `pynter-defects-1.0.2/pynter/vasp/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/vasp/default_inputs.py` & `pynter-defects-1.0.2/pynter/vasp/default_inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/vasp/jobs.py` & `pynter-defects-1.0.2/pynter/vasp/jobs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/vasp/plotter.py` & `pynter-defects-1.0.2/pynter/vasp/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/vasp/pmg/pmg_electronic_structure_plotter.py` & `pynter-defects-1.0.2/pynter/vasp/pmg/pmg_electronic_structure_plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/vasp/schemes.py` & `pynter-defects-1.0.2/pynter/vasp/schemes.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter/vasp/utils.py` & `pynter-defects-1.0.2/pynter/vasp/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/pynter_defects.egg-info/SOURCES.txt` & `pynter-defects-1.0.2/pynter_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.1/setup.py` & `pynter-defects-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: villa
 """
 
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='pynter-defects',
-    version='1.0.1',
+    version='1.0.2',
     author='Lorenzo Villa',
     description='Tools for atomistic calculations',
     packages=find_namespace_packages(exclude=["pynter.*.tests", "pynter.*.*.tests"]),
     install_requires=[
         'ase',
         'pymatgen>=2023.3.23',
         'pymatgen-analysis-defects>=2023.3.25',
```

