# Comparing `tmp/shepherd_core-2023.6.4.tar.gz` & `tmp/shepherd_core-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.6.4.tar", last modified: Thu Jun 15 00:28:00 2023, max compression
+gzip compressed data, was "shepherd_core-2023.6.5.tar", last modified: Mon Jun 19 10:58:09 2023, max compression
```

## Comparing `shepherd_core-2023.6.4.tar` & `shepherd_core-2023.6.5.tar`

### file list

```diff
@@ -1,117 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.237828 shepherd_core-2023.6.4/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.237828 shepherd_core-2023.6.4/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.237828 shepherd_core-2023.6.4/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.241828 shepherd_core-2023.6.4/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/firmware_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_source_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/doc_virtual_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.241828 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/target_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.245828 shepherd_core-2023.6.4/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.249828 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/testbed_fixture.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.249828 shepherd_core-2023.6.4/shepherd_core/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/fw_tools/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/fw_tools/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.249828 shepherd_core-2023.6.4/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.249828 shepherd_core-2023.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/tests/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_data_faulty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_meas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_meas_faulty1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_meas_faulty2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_emulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_harvester.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_testbed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_virtsource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_testbed_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/tests/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/fw_tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/fw_tools/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/fw_tools/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/tests/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/vsource/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/vsource/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/vsource/test_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.440589 shepherd_core-2023.6.5/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.440589 shepherd_core-2023.6.5/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.440589 shepherd_core-2023.6.5/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.444590 shepherd_core-2023.6.5/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/firmware_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_source_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/doc_virtual_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.444590 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/target_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.444590 shepherd_core-2023.6.5/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.444590 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/testbed_fixture.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.448591 shepherd_core-2023.6.5/shepherd_core/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/fw_tools/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/fw_tools/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/fw_tools/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.448591 shepherd_core-2023.6.5/shepherd_core/testbed_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/testbed_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/testbed_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/testbed_client/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/testbed_client/user_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.448591 shepherd_core-2023.6.5/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.448591 shepherd_core-2023.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_testbed_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/tests/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/vsource/test_harvester.py
```

### Comparing `shepherd_core-2023.6.4/setup.cfg` & `shepherd_core-2023.6.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 	h5py
 	numpy
 	pyYAML
 	chromalog
 	pydantic[email]<2.0.0
 	tqdm
 	scipy
+	intelhex
 
 [options.extras_require]
 elf = 
 	pwntools
 dev = 
 	black
 	pylint
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/calibration_hw_def.py` & `shepherd_core-2023.6.5/shepherd_core/calibration_hw_def.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/__init__.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from pathlib import Path
-from typing import Optional
-
 from .base.calibration import CalibrationCape
 from .base.calibration import CalibrationEmulator
 from .base.calibration import CalibrationHarvester
 from .base.calibration import CalibrationPair
 from .base.calibration import CalibrationSeries
 from .base.content import ContentModel
-from .base.fixture import Fixtures
 from .base.shepherd import ShpModel
 from .base.wrapper import Wrapper
 from .content.energy_environment import EnergyDType
 from .content.energy_environment import EnergyEnvironment
 from .content.firmware import Firmware
 from .content.firmware import FirmwareDType
 from .content.virtual_harvester import VirtualHarvesterConfig
@@ -30,15 +26,14 @@
     "CalibrationCape",
     "CalibrationEmulator",
     "CalibrationHarvester",
     "CalibrationSeries",
     "CalibrationPair",
     "ContentModel",
     "ShpModel",
-    "Fixtures",
     "Wrapper",
     # User Content
     "Experiment",
     "TargetConfig",
     "Firmware",
     "FirmwareDType",
     "SystemLogging",
@@ -47,22 +42,8 @@
     "GpioActuation",
     "GpioEvent",
     "GpioLevel",
     "EnergyEnvironment",
     "EnergyDType",
     "VirtualSourceConfig",
     "VirtualHarvesterConfig",
-    # test-container & placeholder
-    "fixtures",
 ]
-
-
-class FixtureSet:
-    def __init__(self):
-        self.path = Path(__file__) / "fixtures"
-
-    def load(self, path: Optional[Path] = None) -> None:
-        if path:
-            self.path = path
-
-
-fixtures = FixtureSet()
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/base/cal_measurement.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/base/calibration.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/base/content.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/base/content.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/base/fixture.py` & `shepherd_core-2023.6.5/shepherd_core/testbed_client/fixtures.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import copy
+import os
 from pathlib import Path
+from typing import Dict
 from typing import Optional
 
 import yaml
 
-from ...logger import logger
-from .wrapper import Wrapper
+from ..data_models.base.wrapper import Wrapper
+from ..logger import logger
 
 # Proposed field-name:
 # - inheritance
 # - inherit_from  <-- current choice
 # - inheritor
 # - hereditary
 # - based_on
 
 
-class Fixtures:
+class Fixture:
     """Current implementation of a file-based database"""
 
-    def __init__(self, file_path: Path, model_name: str):
-        self.path: Path = file_path.resolve()
-        self.name: str = model_name
-        self.elements_by_name: dict = {}
-        self.elements_by_id: dict = {}
-        with open(self.path) as fix_data:
-            fixtures = yaml.safe_load(fix_data)
-            for fixture in fixtures:
-                if not isinstance(fixture, dict):
-                    continue
-                fwrap = Wrapper(**fixture)
-                if fwrap.datatype.lower() != model_name.lower():
-                    continue
-                if "name" not in fwrap.parameters:
-                    continue
-                name = str(fwrap.parameters["name"]).lower()
-                _id = fwrap.parameters["id"]
-                data = fwrap.parameters
-                # ⤷ TODO: could get easier if not model_name but class used
-                self.elements_by_name[name] = data
-                self.elements_by_id[_id] = data
-        # for iterator
+    def __init__(self, model_type: str):
+        self.model_type: str = model_type.lower()
+        self.elements_by_name: Dict[str, dict] = {}
+        self.elements_by_id: Dict[int, dict] = {}
+        # Iterator reset
         self._iter_index: int = 0
         self._iter_list: list = list(self.elements_by_name.values())
 
+    def insert(self, data: Wrapper) -> None:
+        # ⤷ TODO: could get easier
+        #    - when not model_name but class used
+        #    - use doubleref name->id->data (safes RAM)
+        if data.datatype.lower() != self.model_type.lower():
+            return
+        if "name" not in data.parameters:
+            return
+        name = str(data.parameters["name"]).lower()
+        _id = data.parameters["id"]
+        data = data.parameters
+        self.elements_by_name[name] = data
+        self.elements_by_id[_id] = data
+        # update iterator
+        self._iter_list: list = list(self.elements_by_name.values())
+
     def __getitem__(self, key) -> dict:
         key = key.lower()
-        if key.lower() in self.elements_by_name:
-            return self.elements_by_name[key.lower()]
+        if key in self.elements_by_name:
+            return self.elements_by_name[key]
         if key in self.elements_by_id:
             return self.elements_by_id[key]
-        raise ValueError(f"{self.name} '{key}' not found!")
+        raise ValueError(f"{self.model_type} '{key}' not found!")
 
     def __iter__(self):
         self._iter_index = 0
         self._iter_list = list(self.elements_by_name.values())
         return self
 
     def __next__(self):
@@ -86,23 +87,24 @@
                     )
                 if base_name == fixture_name:
                     raise ValueError(
                         f"Inheritance-Circle detected ({base_name} == {fixture_name})",
                     )
                 chain.append(base_name)
             fixture_base = copy.copy(self[fixture_name])
-            logger.debug("'%s' will inherit from '%s'", self.name, fixture_name)
+            logger.debug("'%s' will inherit from '%s'", self.model_type, fixture_name)
             fixture_base["name"] = fixture_name
             chain.append(fixture_name)
             base_dict, chain = self.inheritance(values=fixture_base, chain=chain)
             for key, value in values.items():
                 # keep previous entries
                 base_dict[key] = value
             values = base_dict
 
+        # TODO: cleanup and simplify - use fill_mode() and line up with web-interface
         elif "name" in values and values.get("name").lower() in self.elements_by_name:
             fixture_name = values.get("name").lower()
             fixture_base = copy.copy(self.elements_by_name[fixture_name])
             post_process = True
 
         elif values.get("id") in self.elements_by_id:
             _id = values["id"]
@@ -119,23 +121,101 @@
                 chain.append(fixture_base["name"])
                 values, chain = self.inheritance(values=fixture_base, chain=chain)
             else:
                 values = fixture_base
 
         return values, chain
 
-    def lookup(self, values: dict) -> dict:
-        """init by name/id for none existing instances raise Exception"""
-        if len(values) == 1 and list(values.keys())[0] in ["id", "name"]:
-            value = list(values.values())[0]
-            if isinstance(value, str) and value.lower() in self.elements_by_name:
-                values = {"name": value}
-            elif isinstance(value, int) and value in self.elements_by_id:
-                values = {"id": value}
-            else:
-                raise ValueError(
-                    f"Initialization of {self.name} by name or ID failed - {values} is unknown!"
-                )
-        return values
+    @staticmethod
+    def fill_model(model: dict, base: dict) -> dict:
+        base = copy.copy(base)
+        for key, value in model.items():
+            # keep previous entries
+            base[key] = value
+        return base
+
+    def query_id(self, _id: int) -> dict:
+        if isinstance(_id, int) and _id in self.elements_by_id:
+            return self.elements_by_id[_id]
+        else:
+            raise ValueError(
+                f"Initialization of {self.model_type} by ID failed - {_id} is unknown!"
+            )
+
+    def query_name(self, name: str):
+        if isinstance(name, str) and name.lower() in self.elements_by_name:
+            return self.elements_by_name[name.lower()]
+        else:
+            raise ValueError(
+                f"Initialization of {self.model_type} by name failed - {name} is unknown!"
+            )
+
+
+class Fixtures:
+    suffix = ".yaml"
+
+    def __init__(self, file_path: Optional[Path] = None):
+        if file_path is None:
+            self.file_path = Path(__file__).parent.parent.resolve() / "data_models"
+        else:
+            self.file_path = file_path
+        self.components: Dict[str, Fixture] = {}
+
+        if self.file_path.is_file():
+            files = [self.file_path]
+        elif self.file_path.is_dir():
+            files = get_files(self.file_path, self.suffix)
+        else:
+            raise ValueError("Path must either be file or directory (or empty)")
+
+        for file in files:
+            self.insert_file(file)
+
+    def insert_file(self, file: Path):
+        with open(file) as fd:
+            fixtures = yaml.safe_load(fd)
+            for fixture in fixtures:
+                if not isinstance(fixture, dict):
+                    continue
+                fix_wrap = Wrapper(**fixture)
+                self.insert_model(fix_wrap)
+
+    def insert_model(self, data: Wrapper):
+        fix_type = data.datatype.lower()
+        if self.components.get(fix_type) is None:
+            self.components[fix_type] = Fixture(model_type=fix_type)
+        self.components[fix_type].insert(data)
+
+    def __getitem__(self, key) -> Fixture:
+        key = key.lower()
+        if key in self.components:
+            return self.components[key]
+        raise ValueError(f"Component '{key}' not found!")
+
+    def keys(self):  # -> _dict_keys[Any, Any]:
+        return self.components.keys()
+
+    def to_file(self, file: Path):
+        raise RuntimeError("Not Implemented, TODO")
+
 
-    def load_from_testbed(self):
-        pass  # TODO
+def get_files(start_path: Path, suffix: str, recursion_depth: int = 0) -> list:
+    if recursion_depth == 0:
+        suffix = suffix.lower().split(".")[-1]
+    dir_items = os.scandir(start_path)
+    recursion_depth += 1
+    files = []
+
+    for item in dir_items:
+        if item.is_dir():
+            files += get_files(item.path, suffix, recursion_depth)
+            continue
+        else:
+            item_name = str(item.name).lower()
+            item_ext = item_name.split(".")[-1]
+            if item_ext == suffix and item_ext != item_name:
+                files.append(item.path)
+            if suffix == "" and item_ext == item_name:
+                files.append(item.path)
+    if recursion_depth == 1 and len(files) > 0:
+        logger.debug(" -> got %s files with the suffix '%s'", len(files), suffix)
+    return files
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/base/shepherd.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/content/energy_environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from enum import Enum
 from pathlib import Path
 
 from pydantic import PositiveFloat
 from pydantic import root_validator
 
+from ...testbed_client import tb_client
 from ..base.content import ContentModel
-from ..base.fixture import Fixtures
-
-fixture_path = Path(__file__).resolve().with_name("energy_environment_fixture.yaml")
-fixtures = Fixtures(fixture_path, "EnergyEnvironment")
 
 
 class EnergyDType(str, Enum):
     ivsample = "ivsample"
     ivsamples = "ivsample"
     ivcurve = "ivcurve"
     ivcurves = "ivcurve"
@@ -31,10 +28,10 @@
     energy_Ws: PositiveFloat
     valid: bool = False
 
     # TODO: scale up/down voltage/current
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, _ = fixtures.inheritance(values)
+        values, _ = tb_client.try_completing_model(cls.__name__, values)
+        values = tb_client.fill_in_user_data(values)
         return values
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/content/energy_environment_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/content/energy_environment_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/cape.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+from datetime import date
+from datetime import datetime
 from enum import Enum
-from pathlib import Path
+from typing import Optional
 from typing import Union
 
-from pydantic import constr
+from pydantic import Field
 from pydantic import root_validator
 
-from ..base.content import ContentModel
-from ..base.fixture import Fixtures
-from ..testbed.mcu import MCU
+from ...testbed_client import tb_client
+from ..base.content import IdInt
+from ..base.content import NameStr
+from ..base.content import SafeStr
+from ..base.shepherd import ShpModel
+
+
+class TargetPort(str, Enum):
+    A = "A"
+    B = "B"
+    a = "A"
+    b = "B"
+
+
+class Cape(ShpModel, title="Shepherd-Cape"):
+    """meta-data representation of a testbed-component (physical object)"""
+
+    id: IdInt  # noqa: A003
+    name: NameStr
+    version: NameStr
+    description: SafeStr
+    comment: Optional[SafeStr] = None
+    # TODO: wake_interval, calibration
 
-fixture_path = Path(__file__).resolve().with_name("firmware_fixture.yaml")
-fixtures = Fixtures(fixture_path, "firmware")
+    created: Union[date, datetime] = Field(default_factory=datetime.now)
+    calibrated: Union[date, datetime, None] = None
 
-
-class FirmwareDType(str, Enum):
-    base64_hex = "hex"
-    base64_elf = "elf"
-    path_hex = "path_hex"
-    path_elf = "path_elf"
-
-
-class Firmware(ContentModel, title="Firmware of Target"):
-    """meta-data representation of a data-component"""
-
-    # General Metadata & Ownership -> ContentModel
-
-    mcu: MCU
-
-    data: Union[constr(min_length=3, max_length=1_000_000), Path]
-    data_type: FirmwareDType
+    def __str__(self):
+        return self.name
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, _ = fixtures.inheritance(values)
+        values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/content/firmware_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/content/firmware_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from enum import Enum
-from pathlib import Path
 from typing import Optional
 from typing import Tuple
 
 from pydantic import confloat
 from pydantic import conint
 from pydantic import root_validator
 
 from ...commons import samplerate_sps_default
 from ...logger import logger
+from ...testbed_client import tb_client
 from ..base.calibration import CalibrationHarvester
 from ..base.content import ContentModel
-from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 from .energy_environment import EnergyDType
 
-fixture_path = Path(__file__).resolve().with_name("virtual_harvester_fixture.yaml")
-fixtures = Fixtures(fixture_path, "VirtualHarvesterConfig")
-
 
 class AlgorithmDType(str, Enum):
     isc_voc = "isc_voc"
     ivcurve = ("ivcurve",)
     ivcurves = ("ivcurve",)
     cv = "cv"
     constant = "cv"
@@ -66,16 +62,16 @@
 
     # Underlying recorder
     wait_cycles: conint(ge=0, le=100) = 1
     # ⤷ first cycle: ADC-Sampling & DAC-Writing, further steps: waiting
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values, chain = tb_client.try_completing_model(cls.__name__, values)
+        values = tb_client.fill_in_user_data(values)
         if values["name"] == "neutral":
             # TODO: same test is later done in calc_algorithm_num() again
             raise ValueError("Resulting Harvester can't be neutral")
         logger.debug("VHrv-Inheritances: %s", chain)
         return values
 
     @root_validator(pre=False)
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_harvester_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_harvester_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-from pathlib import Path
-
 from pydantic import confloat
 from pydantic import conint
 from pydantic import conlist
 from pydantic import root_validator
 
 from ...commons import samplerate_sps_default
 from ...logger import logger
+from ...testbed_client import tb_client
 from .. import ShpModel
 from ..base.content import ContentModel
-from ..base.fixture import Fixtures
 from .virtual_harvester import HarvesterPRUConfig
 from .virtual_harvester import VirtualHarvesterConfig
 
-fixture_path = Path(__file__).resolve().with_name("virtual_source_fixture.yaml")
-fixtures = Fixtures(fixture_path, "VirtualSourceConfig")
-
 
 class VirtualSourceConfig(ContentModel, title="Config for the virtual Source"):
     """The virtual Source uses the energy environment (file)
     for supplying the Target Node during the experiment.
     If not already done, the energy will be harvested and then converted.
     The converter-stage is software defined and offers:
       buck-boost-combinations,
@@ -104,16 +99,16 @@
     ) = 12 * [1.00]
     # ⤷ array[12] depending on output_current
     LUT_output_I_min_log2_nA: conint(ge=0, le=20) = 0
     # ⤷ 2^8 = 256 nA -> LUT[0] is for inputs < 256 nA, see notes on LUT_input for explanation
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values, chain = tb_client.try_completing_model(cls.__name__, values)
+        values = tb_client.fill_in_user_data(values)
         logger.debug("VSrc-Inheritances: %s", chain)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # trigger stricter test of harv-parameters
         HarvesterPRUConfig.from_vhrv(values.get("harvester"), for_emu=True)
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_source_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_source_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/doc_virtual_source.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/doc_virtual_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from pathlib import Path
 
 from pydantic import Field
 from pydantic import confloat
 from pydantic import conlist
 from pydantic import root_validator
 
-from shepherd_core.data_models import Fixtures
-from shepherd_core.data_models import ShpModel
-
 from .. import logger
+from ..data_models import Fixture
+from ..data_models import ShpModel
 from .content import VirtualHarvesterConfig
 
 fixture_path = Path(__file__).resolve().with_name("content/virtual_source_fixture.yaml")
-fixtures = Fixtures(fixture_path, "content.VirtualSource")
+fixtures = Fixture(fixture_path, "content.VirtualSource")
 
 
 @DeprecationWarning
 class VirtualSourceDoc(ShpModel, title="Virtual Source (Documented, Testversion)"):
     # General Config
     name: str = Field(
         title="Name of Virtual Source",
@@ -221,11 +220,11 @@
         default=0,
         ge=0,
         le=20,
     )
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, chain = fixtures.inheritance(values)
+        values = fixtures.try_completing_model(values)
+        values, chain = fixtures.try_inheritance(values)
         logger.debug("VSrc-Inheritances: %s", chain)
         return values
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/experiment/observer_features.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/experiment/target_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class TargetConfig(ShpModel, title="Target Config"):
     """Configuration for Target Nodes (DuT)"""
 
     target_IDs: conlist(item_type=IdInt, min_items=1, max_items=64)
     custom_IDs: Optional[conlist(item_type=IdInt16, min_items=1, max_items=64)]
     # ⤷ will replace 'const uint16_t SHEPHERD_NODE_ID' in firmware
+    #   if no custom ID is provided, the original ID of target is used
 
     energy_env: EnergyEnvironment  # alias: input
     virtual_source: VirtualSourceConfig = VirtualSourceConfig(name="neutral")
     target_delays: Optional[conlist(item_type=conint(ge=0), min_items=1, max_items=64)]
     # ⤷ individual starting times -> allows to use the same environment
 
     firmware1: Firmware
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/task/emulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 from typing import Union
 
 from pydantic import confloat
 from pydantic import conint
 from pydantic import root_validator
 from pydantic import validate_arguments
 
-from shepherd_core.data_models.testbed import Testbed
-
 from ..base.content import IdInt
 from ..base.shepherd import ShpModel
 from ..content.virtual_source import VirtualSourceConfig
 from ..experiment.experiment import Experiment
 from ..experiment.observer_features import GpioActuation
 from ..experiment.observer_features import GpioTracing
 from ..experiment.observer_features import PowerTracing
 from ..experiment.observer_features import SystemLogging
+from ..testbed import Testbed
 from ..testbed.cape import TargetPort
 
 
 class Compression(str, Enum):
     lzf = "lzf"  # not native hdf5
     gzip1 = 1  # higher compr & load
     gzip = 1
@@ -74,17 +73,15 @@
     voltage_aux: Union[confloat(ge=0, le=4.5), str] = 0
     # ⤷ aux_voltage options:
     #   - 0-4.5 for specific const Voltage (0 V = disabled),
     #   - "buffer" will output intermediate voltage (storage cap of vsource),
     #   - "main" will mirror main target voltage
 
     # sub-elements, could be partly moved to emulation
-    virtual_source: VirtualSourceConfig = VirtualSourceConfig(
-        name="neutral"
-    )  # {"name": "neutral"}
+    virtual_source: VirtualSourceConfig = VirtualSourceConfig(name="neutral")
     # ⤷ Use the desired setting for the virtual source,
     #   provide parameters or name like BQ25570
 
     power_tracing: Optional[PowerTracing] = PowerTracing()
     gpio_tracing: Optional[GpioTracing] = GpioTracing()
     gpio_actuation: Optional[GpioActuation] = None
     sys_logging: Optional[SystemLogging] = SystemLogging()
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/task/firmware_mod.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ..testbed.target import IdInt16
 from ..testbed.target import MCUPort
 
 
 class FirmwareModTask(ShpModel):
     """Config for Task that adds the custom ID to the firmware & stores it into a file"""
 
-    data: Union[constr(min_length=3, max_length=1_000_000), Path]
+    data: Union[constr(min_length=3, max_length=8_000_000), Path]
     data_type: FirmwareDType
     custom_id: Optional[IdInt16]
     firmware_file: Path
 
     verbose: conint(ge=0, le=4) = 2
     # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/task/harvest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/task/observer_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/task/programming.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/task/programming.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/cape_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/cape_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/gpio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from enum import Enum
-from pathlib import Path
 from typing import Optional
 
 from pydantic import conint
 from pydantic import constr
 from pydantic import root_validator
 
+from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
-from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 
-fixture_path = Path(__file__).resolve().with_name("gpio_fixture.yaml")
-fixtures = Fixtures(fixture_path, "gpio")
-
 
 class Direction(str, Enum):
     Input = "IN"
     IN = "IN"
     Output = "OUT"
     OUT = "OUT"
     Bidirectional = "IO"
@@ -42,16 +38,15 @@
     pin_sys: Optional[constr(max_length=10)] = None
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, _ = fixtures.inheritance(values)
+        values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # ensure that either pru or sys is used, otherwise instance is considered faulty
         no_pru = (values.get("reg_pru") is None) or (values.get("pin_pru") is None)
         no_sys = (values.get("reg_sys") is None) or (values.get("pin_sys") is None)
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/gpio_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/gpio_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/mcu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from enum import Enum
-from pathlib import Path
 from typing import Optional
 
 from pydantic import confloat
 from pydantic import conint
 from pydantic import root_validator
 
+from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
-from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 
-fixture_path = Path(__file__).resolve().with_name("mcu_fixture.yaml")
-fixtures = Fixtures(fixture_path, "mcu")
-
 
 class ProgrammerProtocol(str, Enum):
     SWD = "SWD"
     swd = "SWD"
     SBW = "SBW"
     sbw = "SBW"
     JTAG = "JTAG"
@@ -45,10 +41,9 @@
     # ⤷ can't be FW-Object (circular import)
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, _ = fixtures.inheritance(values)
+        values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/mcu_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/mcu_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/observer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from datetime import datetime
-from pathlib import Path
 from typing import Optional
 
 from pydantic import Field
 from pydantic import IPvAnyAddress
 from pydantic import confloat
 from pydantic import constr
 from pydantic import root_validator
 
+from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
-from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 from .cape import Cape
 from .cape import TargetPort
 from .target import Target
 
-fixture_path = Path(__file__).resolve().with_name("observer_fixture.yaml")
-fixtures = Fixtures(fixture_path, "observer")
-
 MACStr = constr(max_length=17, regex=r"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$")
 
 
 class Observer(ShpModel, title="Shepherd-Sheep"):
     """meta-data representation of a testbed-component (physical object)"""
 
     id: IdInt  # noqa: A003
@@ -48,16 +44,15 @@
     alive_last: Optional[datetime]
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, _ = fixtures.inheritance(values)
+        values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         has_cape = values.get("cape") is not None
         has_target = (values.get("target_a") is not None) or (
             values.get("target_b") is not None
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/observer_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/observer_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/target.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from datetime import datetime
-from pathlib import Path
 from typing import Optional
 from typing import Union
 
 from pydantic import Field
 from pydantic import conint
 from pydantic import root_validator
 
+from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
-from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 from .mcu import MCU
 
-fixture_path = Path(__file__).resolve().with_name("target_fixture.yaml")
-fixtures = Fixtures(fixture_path, "target")
-
 IdInt16 = conint(ge=0, lt=2**16)
 
 MCUPort = conint(ge=1, le=2)
 
 
 class Target(ShpModel, title="Target Node (DuT)"):
     """meta-data representation of a testbed-component (physical object)"""
@@ -42,16 +38,15 @@
     # TODO programming pins per mcu should be here (or better in Cape)
 
     def __str__(self):
         return self.name
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)
-        values, _ = fixtures.inheritance(values)
+        values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
 
     @root_validator(pre=False)
     def post_correction(cls, values: dict) -> dict:
         if isinstance(values.get("mcu1"), str):
             values["mcu1"] = MCU(name=values["mcu1"])
             # ⤷ this will raise if default is faulty
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/target_fixture.yaml` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/target_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/testbed.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 from pathlib import Path
 from typing import Optional
 
 from pydantic import HttpUrl
 from pydantic import conlist
 from pydantic import root_validator
 
+from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
-from ..base.fixture import Fixtures
 from ..base.shepherd import ShpModel
 from .observer import Observer
 
-fixture_path = Path(__file__).resolve().with_name("testbed_fixture.yaml")
-fixtures = Fixtures(fixture_path, "testbed")
-
 
 class Testbed(ShpModel):
     """meta-data representation of a testbed-component (physical object)"""
 
     id: IdInt  # noqa: A003
     name: NameStr
     description: SafeStr
@@ -35,16 +32,15 @@
     # ⤷ storage layout: root_path/content_type/group/owner/[object]
 
     prep_duration: timedelta = timedelta(minutes=5)
     # TODO: one BBone is currently time-keeper
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
-        values = fixtures.lookup(values)  # TODO: load from url
-        values, _ = fixtures.inheritance(values)
+        values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         observers = []
         ips = []
         macs = []
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/fw_tools/converter.py` & `shepherd_core-2023.6.5/shepherd_core/fw_tools/converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/fw_tools/patcher.py` & `shepherd_core-2023.6.5/shepherd_core/fw_tools/patcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,79 @@
-import os
 from pathlib import Path
 from typing import Optional
 
-from elftools.common.exceptions import ELFError
 from pwnlib.elf import ELF
 from pydantic import conint
 from pydantic import validate_arguments
 
 from ..commons import uid_len_default
 from ..commons import uid_str_default
 from ..logger import logger as log
+from .validation import is_elf
 
 
 @validate_arguments
 def find_symbol(file_elf: Path, symbol: str) -> bool:
-    if symbol is None or not os.path.isfile(file_elf):
+    if symbol is None or not is_elf(file_elf):
         return False
-    try:
-        elf = ELF(path=file_elf)
-    except ELFError:
-        log.debug(
-            "File %s is not ELF - Magic number does not match", symbol, file_elf.name
-        )
-        return False
-
+    elf = ELF(path=file_elf)
     try:
         elf.symbols[symbol]
     except KeyError:
         log.debug("Symbol '%s' not found in ELF-File %s", symbol, file_elf.name)
         return False
     log.debug(
         "Symbol '%s' found in ELF-File %s, arch=%s, order=%s",
         symbol,
         file_elf.name,
         elf.arch,
         elf.endian,
     )
+    elf.close()
     return True
 
 
 @validate_arguments
 def read_symbol(
     file_elf: Path, symbol: str, length: int = uid_len_default
 ) -> Optional[int]:
     """interpreted as int"""
     if not find_symbol(file_elf, symbol):
         return None
     elf = ELF(path=file_elf)
     addr = elf.symbols[symbol]
     value_raw = elf.read(address=addr, count=length)[-length:]
+    elf.close()
     return int.from_bytes(bytes=value_raw, byteorder=elf.endian, signed=False)
 
 
 def read_uid(file_elf: Path) -> Optional[int]:
     return read_symbol(file_elf, symbol=uid_str_default, length=uid_len_default)
 
 
+def read_arch(file_elf: Path) -> Optional[str]:
+    if not is_elf(file_elf):
+        return None
+    elf = ELF(path=file_elf)
+    if "exec" in elf.elftype.lower():
+        return elf.arch.lower()
+    log.error("ELF is not Executable")
+    return None
+
+
 @validate_arguments
 def modify_symbol_value(
     file_elf: Path,
     symbol: str,
     value: conint(ge=0, lt=2 ** (8 * uid_len_default)),
     overwrite: bool = False,
 ) -> Optional[Path]:
     """replaces value of symbol in ELF-File, hardcoded for uint16_t (2 byte)
     testbed uses FN to patch firmware with custom target-ID
-    NOTE: overwrites provided file
+    NOTE: can overwrite provided file
 
     """
     if not find_symbol(file_elf, symbol):
         return None
     elf = ELF(path=file_elf)
     addr = elf.symbols[symbol]
     value_raw = elf.read(address=addr, count=uid_len_default)[-uid_len_default:]
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/logger.py` & `shepherd_core-2023.6.5/shepherd_core/logger.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/reader.py` & `shepherd_core-2023.6.5/shepherd_core/reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2023.6.5/shepherd_core/vsource/virtual_converter_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 - bitshifted values (ie. _n28) are converted to float without shift
 
 """
 
 import math
 from typing import Optional
 
-from shepherd_core import CalibrationEmulator
-from shepherd_core.data_models.content.virtual_source import LUT_SIZE
-from shepherd_core.data_models.content.virtual_source import ConverterPRUConfig
+from ..data_models import CalibrationEmulator
+from ..data_models.content.virtual_source import LUT_SIZE
+from ..data_models.content.virtual_source import ConverterPRUConfig
 
 
 class PruCalibration:
     """part of calibration.h"""
 
     def __init__(self, cal_emu: Optional[CalibrationEmulator] = None):
         self.cal = cal_emu if cal_emu else CalibrationEmulator()
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2023.6.5/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2023.6.5/shepherd_core/vsource/virtual_source_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 - step 1 to a virtualization of emulation
 
 NOTE: DO NOT OPTIMIZE -> stay close to original code-base
 
 """
 from typing import Optional
 
-from shepherd_core import CalibrationEmulator
-
+from ..data_models import CalibrationEmulator
 from ..data_models import EnergyDType
 from ..data_models import VirtualSourceConfig
 from ..data_models.content.virtual_harvester import HarvesterPRUConfig
 from ..data_models.content.virtual_source import ConverterPRUConfig
 from .virtual_converter_model import PruCalibration
 from .virtual_converter_model import VirtualConverterModel
 from .virtual_harvester_model import VirtualHarvesterModel
```

### Comparing `shepherd_core-2023.6.4/shepherd_core/writer.py` & `shepherd_core-2023.6.5/shepherd_core/writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/shepherd_core.egg-info/SOURCES.txt` & `shepherd_core-2023.6.5/shepherd_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 ./shepherd_core/writer.py
 ./shepherd_core/data_models/__init__.py
 ./shepherd_core/data_models/doc_virtual_source.py
 ./shepherd_core/data_models/base/__init__.py
 ./shepherd_core/data_models/base/cal_measurement.py
 ./shepherd_core/data_models/base/calibration.py
 ./shepherd_core/data_models/base/content.py
-./shepherd_core/data_models/base/fixture.py
 ./shepherd_core/data_models/base/shepherd.py
 ./shepherd_core/data_models/base/wrapper.py
 ./shepherd_core/data_models/content/__init__.py
 ./shepherd_core/data_models/content/energy_environment.py
 ./shepherd_core/data_models/content/energy_environment_fixture.yaml
 ./shepherd_core/data_models/content/firmware.py
 ./shepherd_core/data_models/content/firmware_fixture.yaml
@@ -48,14 +47,19 @@
 ./shepherd_core/data_models/testbed/target.py
 ./shepherd_core/data_models/testbed/target_fixture.yaml
 ./shepherd_core/data_models/testbed/testbed.py
 ./shepherd_core/data_models/testbed/testbed_fixture.yaml
 ./shepherd_core/fw_tools/__init__.py
 ./shepherd_core/fw_tools/converter.py
 ./shepherd_core/fw_tools/patcher.py
+./shepherd_core/fw_tools/validation.py
+./shepherd_core/testbed_client/__init__.py
+./shepherd_core/testbed_client/client.py
+./shepherd_core/testbed_client/fixtures.py
+./shepherd_core/testbed_client/user_model.py
 ./shepherd_core/vsource/__init__.py
 ./shepherd_core/vsource/virtual_converter_model.py
 ./shepherd_core/vsource/virtual_harvester_model.py
 ./shepherd_core/vsource/virtual_source_model.py
 ./tests/__init__.py
 ./tests/conftest.py
 ./tests/test_cal_hw.py
@@ -85,14 +89,15 @@
 ./tests/data_models/test_task_models.py
 ./tests/data_models/test_testbed_fixtures.py
 ./tests/data_models/test_testbed_models.py
 ./tests/fw_tools/__init__.py
 ./tests/fw_tools/conftest.py
 ./tests/fw_tools/test_converter.py
 ./tests/fw_tools/test_patcher.py
+./tests/fw_tools/test_validation.py
 ./tests/vsource/__init__.py
 ./tests/vsource/conftest.py
 ./tests/vsource/test_converter.py
 ./tests/vsource/test_harvester.py
 shepherd_core.egg-info/PKG-INFO
 shepherd_core.egg-info/SOURCES.txt
 shepherd_core.egg-info/dependency_links.txt
```

### Comparing `shepherd_core-2023.6.4/tests/conftest.py` & `shepherd_core-2023.6.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/example_cal_data.yaml` & `shepherd_core-2023.6.5/tests/data_models/example_cal_data.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/example_cal_data_faulty.yaml` & `shepherd_core-2023.6.5/tests/data_models/example_cal_data_faulty.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/example_cal_meas.yaml` & `shepherd_core-2023.6.5/tests/data_models/example_cal_meas.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/example_cal_meas_faulty1.yaml` & `shepherd_core-2023.6.5/tests/data_models/example_cal_meas_faulty1.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/example_cal_meas_faulty2.yaml` & `shepherd_core-2023.6.5/tests/data_models/example_cal_meas_faulty2.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/example_config_emulator.yaml` & `shepherd_core-2023.6.5/tests/data_models/example_config_emulator.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/example_config_harvester.yaml` & `shepherd_core-2023.6.5/tests/data_models/example_config_harvester.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/example_config_virtsource.yaml` & `shepherd_core-2023.6.5/tests/data_models/example_config_virtsource.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/test_base_models.py` & `shepherd_core-2023.6.5/tests/data_models/test_base_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/test_content_fixtures.py` & `shepherd_core-2023.6.5/tests/data_models/test_content_fixtures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 from shepherd_core.data_models.content.energy_environment import EnergyEnvironment
-from shepherd_core.data_models.content.energy_environment import fixtures as fix_ee
 from shepherd_core.data_models.content.firmware import Firmware
-from shepherd_core.data_models.content.firmware import fixtures as fix_firmware
 from shepherd_core.data_models.content.virtual_harvester import HarvesterPRUConfig
 from shepherd_core.data_models.content.virtual_harvester import VirtualHarvesterConfig
-from shepherd_core.data_models.content.virtual_harvester import fixtures as fix_hrv
 from shepherd_core.data_models.content.virtual_source import ConverterPRUConfig
 from shepherd_core.data_models.content.virtual_source import VirtualSourceConfig
-from shepherd_core.data_models.content.virtual_source import fixtures as fix_src
+from shepherd_core.testbed_client.fixtures import Fixtures
 
 
 def test_testbed_fixture_energy_environment() -> None:
-    for fix in fix_ee:
+    for fix in Fixtures()["EnergyEnvironment"]:
         EnergyEnvironment(name=fix["name"])
         EnergyEnvironment(id=fix["id"])
 
 
 def test_testbed_fixture_firmware() -> None:
-    for fix in fix_firmware:
+    for fix in Fixtures()["Firmware"]:
         _id = fix["id"]
         if _id in [1001, 1002]:
             continue
         Firmware(name=fix["name"])
         Firmware(id=fix["id"])
 
 
 def test_experiment_fixture_vsrc() -> None:
-    for fix in fix_src:
+    for fix in Fixtures()["VirtualSourceConfig"]:
         vsrc = VirtualSourceConfig(name=fix["name"])
         VirtualSourceConfig(id=fix["id"])
         ConverterPRUConfig.from_vsrc(vsrc, log_intermediate_node=False)
         ConverterPRUConfig.from_vsrc(vsrc, log_intermediate_node=True)
 
 
 def test_experiment_fixture_vhrv() -> None:
-    for fix in fix_hrv:
+    for fix in Fixtures()["VirtualHarvesterConfig"]:
         if fix["name"] == "neutral":
             continue
         vhrv = VirtualHarvesterConfig(name=fix["name"])
         VirtualHarvesterConfig(id=fix["id"])
         HarvesterPRUConfig.from_vhrv(vhrv, for_emu=False)
         if int(fix["id"]) >= 1030:
             HarvesterPRUConfig.from_vhrv(vhrv, for_emu=True)
```

### Comparing `shepherd_core-2023.6.4/tests/data_models/test_content_models.py` & `shepherd_core-2023.6.5/tests/data_models/test_content_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+from pathlib import Path
+
 import pytest
 from pydantic import ValidationError
 
+from shepherd_core import fw_tools
 from shepherd_core.data_models.content import EnergyDType
 from shepherd_core.data_models.content import EnergyEnvironment
 from shepherd_core.data_models.content import Firmware
 from shepherd_core.data_models.content import FirmwareDType
 from shepherd_core.data_models.content import VirtualHarvesterConfig
 from shepherd_core.data_models.content import VirtualSourceConfig
 from shepherd_core.data_models.content.virtual_source import ConverterPRUConfig
 from shepherd_core.data_models.testbed import MCU
 
+from .conftest import files_elf
+
 
 def test_content_model_ee_min1() -> None:
     EnergyEnvironment(
         id=9999,
         name="some",
         data_path="./file",
         data_type="isc_voc",
@@ -45,14 +50,36 @@
         data="xyz",
         data_type=FirmwareDType.base64_hex,
         owner="Obelix",
         group="Gaul",
     )
 
 
+@pytest.mark.parametrize("path_elf", files_elf)
+def test_content_model_fw_from_elf(path_elf: Path) -> None:
+    Firmware.from_firmware(
+        file=path_elf,
+        name="dome",
+        owner="Obelix",
+        group="Gaul",
+    )
+
+
+@pytest.mark.parametrize("path_elf", files_elf)
+def test_content_model_fw_from_hex(path_elf: Path, tmp_path: Path) -> None:
+    path_hex = (tmp_path / (path_elf.stem + ".hex")).resolve()
+    path_hex = fw_tools.elf_to_hex(path_elf, path_hex)
+    Firmware.from_firmware(
+        file=path_hex,
+        name="dome",
+        owner="Obelix",
+        group="Gaul",
+    )
+
+
 def test_content_model_hrv_min() -> None:
     hrv = VirtualHarvesterConfig(
         id=9999,
         name="whatever",
         owner="jane",
         group="wayne",
         algorithm="mppt_opt",
```

### Comparing `shepherd_core-2023.6.4/tests/data_models/test_examples.py` & `shepherd_core-2023.6.5/tests/data_models/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/test_experiment_models.py` & `shepherd_core-2023.6.5/tests/data_models/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/test_task_generation.py` & `shepherd_core-2023.6.5/tests/data_models/test_task_generation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/test_task_models.py` & `shepherd_core-2023.6.5/tests/data_models/test_task_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/data_models/test_testbed_models.py` & `shepherd_core-2023.6.5/tests/data_models/test_testbed_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/fw_tools/test_converter.py` & `shepherd_core-2023.6.5/tests/fw_tools/test_converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/fw_tools/test_patcher.py` & `shepherd_core-2023.6.5/tests/fw_tools/test_patcher.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/test_cal_hw.py` & `shepherd_core-2023.6.5/tests/test_cal_hw.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/test_examples.py` & `shepherd_core-2023.6.5/tests/test_examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,13 +13,14 @@
 
 
 examples = [
     "model_tester.py",
     "vsource_simulation.py",
     "vharvester_simulation.py",
     "firmware_modification.py",
+    "firmware_model.py",
 ]
 
 
 @pytest.mark.parametrize("file", examples)
 def test_example_scripts(example_path: Path, file: str) -> None:
     subprocess.check_call(f"python {example_path / file}", shell=True)
```

### Comparing `shepherd_core-2023.6.4/tests/test_reader.py` & `shepherd_core-2023.6.5/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/test_writer.py` & `shepherd_core-2023.6.5/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/vsource/conftest.py` & `shepherd_core-2023.6.5/tests/vsource/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/vsource/test_converter.py` & `shepherd_core-2023.6.5/tests/vsource/test_converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.4/tests/vsource/test_harvester.py` & `shepherd_core-2023.6.5/tests/vsource/test_harvester.py`

 * *Files identical despite different names*

