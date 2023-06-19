# Comparing `tmp/rips-2023.3.0.1.tar.gz` & `tmp/rips-2023.6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rips-2023.3.0.1.tar", last modified: Thu Mar 16 13:46:20 2023, max compression
+gzip compressed data, was "dist\rips-2023.6.0.1.tar", last modified: Mon Jun 19 12:49:47 2023, max compression
```

## Comparing `rips-2023.3.0.1.tar` & `rips-2023.6.0.1.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 13:46:20.000000 rips-2023.3.0.1/
--rw-rw-rw-   0        0        0      560 2021-03-03 12:14:39.000000 rips-2023.3.0.1/LICENSE
--rw-rw-rw-   0        0        0       75 2021-03-03 12:14:39.000000 rips-2023.3.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1039 2023-03-16 13:46:20.000000 rips-2023.3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      190 2021-03-03 12:14:39.000000 rips-2023.3.0.1/README.md
--rw-rw-rw-   0        0        0      201 2021-03-03 12:14:39.000000 rips-2023.3.0.1/autoformat_pep8.txt
--rw-rw-rw-   0        0        0     1164 2021-03-03 12:14:39.000000 rips-2023.3.0.1/create_pip_package.txt
--rw-rw-rw-   0        0        0       37 2021-03-03 12:14:39.000000 rips-2023.3.0.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips/
-drwxrwxrwx   0        0        0        0 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips/PythonExamples/
--rw-rw-rw-   0        0        0     1495 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/all_cases.py
--rw-rw-rw-   0        0        0     1267 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/all_simulation_wells.py
--rw-rw-rw-   0        0        0      606 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/all_wells.py
--rw-rw-rw-   0        0        0      801 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/alter_wbs_plot.py
--rw-rw-rw-   0        0        0      685 2023-02-10 10:50:44.000000 rips-2023.3.0.1/rips/PythonExamples/case_grid_group.py
--rw-rw-rw-   0        0        0     1016 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/case_info_streaming_example.py
--rw-rw-rw-   0        0        0      509 2021-11-18 07:34:03.000000 rips-2023.3.0.1/rips/PythonExamples/cell_result_data.py
--rw-rw-rw-   0        0        0     1785 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/command_example.py
--rw-rw-rw-   0        0        0     4227 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/create_and_export_stim_plan_model.py
--rw-rw-rw-   0        0        0     2433 2022-04-05 06:32:53.000000 rips-2023.3.0.1/rips/PythonExamples/create_intersection.py
--rw-rw-rw-   0        0        0     3735 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/create_surface_from_thermal_fracture.py
--rw-rw-rw-   0        0        0     1433 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/create_wbs_plot.py
--rw-rw-rw-   0        0        0     3230 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/error_handling.py
--rw-rw-rw-   0        0        0     1171 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/export_contour_maps.py
--rw-rw-rw-   0        0        0      654 2021-08-17 13:58:38.000000 rips-2023.3.0.1/rips/PythonExamples/export_plots.py
--rw-rw-rw-   0        0        0     1598 2021-09-02 13:22:54.000000 rips-2023.3.0.1/rips/PythonExamples/export_snapshots.py
--rw-rw-rw-   0        0        0      701 2023-02-10 14:16:08.000000 rips-2023.3.0.1/rips/PythonExamples/export_well_path_completions.py
--rw-rw-rw-   0        0        0     2671 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/generate_ensemble_of_well_logs.py
--rw-rw-rw-   0        0        0     2056 2021-08-23 10:48:10.000000 rips-2023.3.0.1/rips/PythonExamples/generate_ensemble_surface.py
--rw-rw-rw-   0        0        0     1149 2021-08-31 13:17:57.000000 rips-2023.3.0.1/rips/PythonExamples/generate_ensemble_surface_optimized.py
--rw-rw-rw-   0        0        0      590 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/grid_information.py
--rw-rw-rw-   0        0        0     1073 2022-03-22 10:18:39.000000 rips-2023.3.0.1/rips/PythonExamples/headless_plot_export.py
--rw-rw-rw-   0        0        0     2370 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/import_fractures_on_well.py
--rw-rw-rw-   0        0        0     1403 2022-10-25 08:32:28.000000 rips-2023.3.0.1/rips/PythonExamples/import_thermal_fracture_on_well.py
--rw-rw-rw-   0        0        0     1327 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/import_well_paths_and_logs.py
--rw-rw-rw-   0        0        0     1997 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/input_prop_test_async.py
--rw-rw-rw-   0        0        0     1223 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/input_prop_test_sync.py
--rw-rw-rw-   0        0        0      302 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/instance_example.py
--rw-rw-rw-   0        0        0     1315 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/launch_load_case_snapshot_exit.py
--rw-rw-rw-   0        0        0      465 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/launch_with_commandline_options.py
--rw-rw-rw-   0        0        0     1131 2021-09-01 05:50:56.000000 rips-2023.3.0.1/rips/PythonExamples/load_case.py
--rw-rw-rw-   0        0        0     1057 2021-08-16 06:21:02.000000 rips-2023.3.0.1/rips/PythonExamples/modeled_well_path.py
--rw-rw-rw-   0        0        0     1725 2021-08-16 06:21:02.000000 rips-2023.3.0.1/rips/PythonExamples/modeled_well_path_lateral.py
--rw-rw-rw-   0        0        0      467 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/new_summary_plot.py
--rw-rw-rw-   0        0        0      692 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/open_project.py
--rw-rw-rw-   0        0        0      393 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/replace_case.py
--rw-rw-rw-   0        0        0      894 2021-09-29 06:17:01.000000 rips-2023.3.0.1/rips/PythonExamples/save_project.py
--rw-rw-rw-   0        0        0      768 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/selected_cases.py
--rw-rw-rw-   0        0        0     2536 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/selected_cells.py
--rw-rw-rw-   0        0        0      379 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/set_cell_result.py
--rw-rw-rw-   0        0        0      861 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/set_flow_diagnostics_result.py
--rw-rw-rw-   0        0        0     1444 2021-11-18 11:24:26.000000 rips-2023.3.0.1/rips/PythonExamples/set_grid_properties.py
--rw-rw-rw-   0        0        0     1279 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/soil_average_async.py
--rw-rw-rw-   0        0        0      845 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/soil_average_sync.py
--rw-rw-rw-   0        0        0     2110 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/soil_porv_async.py
--rw-rw-rw-   0        0        0     1120 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/PythonExamples/soil_porv_sync.py
--rw-rw-rw-   0        0        0      460 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/summary_cases.py
--rw-rw-rw-   0        0        0     1710 2022-03-28 07:02:00.000000 rips-2023.3.0.1/rips/PythonExamples/summary_vectors.py
--rw-rw-rw-   0        0        0     1256 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/PythonExamples/surface_import.py
--rw-rw-rw-   0        0        0     1056 2021-08-31 13:16:54.000000 rips-2023.3.0.1/rips/PythonExamples/view_example.py
--rw-rw-rw-   0        0        0      679 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/__init__.py
--rw-rw-rw-   0        0        0    45546 2021-11-18 06:43:06.000000 rips-2023.3.0.1/rips/case.py
--rw-rw-rw-   0        0        0     2118 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/contour_map.py
-drwxrwxrwx   0        0        0        0 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips/generated/
--rw-rw-rw-   0        0        0     7280 2023-03-07 13:46:24.000000 rips-2023.3.0.1/rips/generated/App_pb2.py
--rw-rw-rw-   0        0        0     6724 2023-03-07 13:46:24.000000 rips-2023.3.0.1/rips/generated/App_pb2_grpc.py
--rw-rw-rw-   0        0        0    40186 2023-03-07 13:46:31.000000 rips-2023.3.0.1/rips/generated/Case_pb2.py
--rw-rw-rw-   0        0        0    19104 2023-03-07 13:46:31.000000 rips-2023.3.0.1/rips/generated/Case_pb2_grpc.py
--rw-rw-rw-   0        0        0   154980 2023-03-07 13:46:37.000000 rips-2023.3.0.1/rips/generated/Commands_pb2.py
--rw-rw-rw-   0        0        0     3360 2023-03-07 13:46:37.000000 rips-2023.3.0.1/rips/generated/Commands_pb2_grpc.py
--rw-rw-rw-   0        0        0    14439 2023-03-07 13:46:41.000000 rips-2023.3.0.1/rips/generated/Definitions_pb2.py
--rw-rw-rw-   0        0        0      159 2023-03-07 13:46:41.000000 rips-2023.3.0.1/rips/generated/Definitions_pb2_grpc.py
--rw-rw-rw-   0        0        0     5614 2023-03-07 13:46:47.000000 rips-2023.3.0.1/rips/generated/Grid_pb2.py
--rw-rw-rw-   0        0        0     5401 2023-03-07 13:46:47.000000 rips-2023.3.0.1/rips/generated/Grid_pb2_grpc.py
--rw-rw-rw-   0        0        0    21334 2023-03-07 13:46:54.000000 rips-2023.3.0.1/rips/generated/NNCProperties_pb2.py
--rw-rw-rw-   0        0        0     7334 2023-03-07 13:46:54.000000 rips-2023.3.0.1/rips/generated/NNCProperties_pb2_grpc.py
--rw-rw-rw-   0        0        0    37075 2023-03-07 13:46:59.000000 rips-2023.3.0.1/rips/generated/PdmObject_pb2.py
--rw-rw-rw-   0        0        0    13870 2023-03-07 13:46:59.000000 rips-2023.3.0.1/rips/generated/PdmObject_pb2_grpc.py
--rw-rw-rw-   0        0        0     3755 2023-03-07 13:47:03.000000 rips-2023.3.0.1/rips/generated/Project_pb2.py
--rw-rw-rw-   0        0        0     9869 2023-03-07 13:47:03.000000 rips-2023.3.0.1/rips/generated/Project_pb2_grpc.py
--rw-rw-rw-   0        0        0    19898 2023-03-07 13:47:09.000000 rips-2023.3.0.1/rips/generated/Properties_pb2.py
--rw-rw-rw-   0        0        0    10631 2023-03-07 13:47:09.000000 rips-2023.3.0.1/rips/generated/Properties_pb2_grpc.py
--rw-rw-rw-   0        0        0      775 2023-03-13 18:38:42.000000 rips-2023.3.0.1/rips/generated/RiaVersionInfo.py
--rw-rw-rw-   0        0        0    11113 2023-03-07 13:47:14.000000 rips-2023.3.0.1/rips/generated/SimulationWell_pb2.py
--rw-rw-rw-   0        0        0     4307 2023-03-07 13:47:14.000000 rips-2023.3.0.1/rips/generated/SimulationWell_pb2_grpc.py
--rw-rw-rw-   0        0        0    79853 2023-03-16 05:46:16.000000 rips-2023.3.0.1/rips/generated/generated_classes.py
--rw-rw-rw-   0        0        0     3647 2021-11-18 11:24:26.000000 rips-2023.3.0.1/rips/grid.py
--rw-rw-rw-   0        0        0     2368 2023-02-10 10:50:44.000000 rips-2023.3.0.1/rips/gridcasegroup.py
--rw-rw-rw-   0        0        0     1511 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/grpc_retry_interceptor.py
--rw-rw-rw-   0        0        0    14846 2022-10-04 12:14:47.000000 rips-2023.3.0.1/rips/instance.py
--rw-rw-rw-   0        0        0    17137 2022-02-08 18:45:33.000000 rips-2023.3.0.1/rips/pdmobject.py
--rw-rw-rw-   0        0        0      832 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/plot.py
--rw-rw-rw-   0        0        0    11987 2021-09-29 07:44:28.000000 rips-2023.3.0.1/rips/project.py
--rw-rw-rw-   0        0        0       59 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/resinsight_classes.py
--rw-rw-rw-   0        0        0     2508 2022-02-08 18:45:33.000000 rips-2023.3.0.1/rips/retry_policy.py
--rw-rw-rw-   0        0        0     2515 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/simulation_well.py
-drwxrwxrwx   0        0        0        0 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips/tests/
--rw-rw-rw-   0        0        0     1428 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/tests/conftest.py
--rw-rw-rw-   0        0        0      207 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/tests/dataroot.py
--rw-rw-rw-   0        0        0     8964 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/tests/test_cases.py
--rw-rw-rw-   0        0        0      875 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/tests/test_commands.py
--rw-rw-rw-   0        0        0     2317 2022-02-21 12:46:35.000000 rips-2023.3.0.1/rips/tests/test_create_well_path.py
--rw-rw-rw-   0        0        0     3601 2023-01-09 14:51:12.000000 rips-2023.3.0.1/rips/tests/test_grids.py
--rw-rw-rw-   0        0        0     1198 2022-09-28 06:53:25.000000 rips-2023.3.0.1/rips/tests/test_launch.py
--rw-rw-rw-   0        0        0     2596 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/tests/test_nnc_properties.py
--rw-rw-rw-   0        0        0     3042 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/tests/test_project.py
--rw-rw-rw-   0        0        0     4516 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/tests/test_properties.py
--rw-rw-rw-   0        0        0     1816 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/tests/test_simulation_wells.py
--rw-rw-rw-   0        0        0     4574 2023-01-24 09:05:18.000000 rips-2023.3.0.1/rips/tests/test_summary_cases.py
--rw-rw-rw-   0        0        0     1019 2021-08-17 12:15:16.000000 rips-2023.3.0.1/rips/tests/test_surfaces.py
--rw-rw-rw-   0        0        0     1522 2023-02-01 07:57:21.000000 rips-2023.3.0.1/rips/tests/test_well_log_extraction.py
--rw-rw-rw-   0        0        0     3343 2022-02-08 18:45:33.000000 rips-2023.3.0.1/rips/tests/test_wells.py
--rw-rw-rw-   0        0        0      678 2021-10-14 08:34:07.000000 rips-2023.3.0.1/rips/tests/test_wells_path_completions.py
--rw-rw-rw-   0        0        0     7612 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/view.py
--rw-rw-rw-   0        0        0     2356 2021-03-03 12:14:39.000000 rips-2023.3.0.1/rips/well_log_plot.py
-drwxrwxrwx   0        0        0        0 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips.egg-info/
--rw-rw-rw-   0        0        0     1039 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3901 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-16 13:46:20.000000 rips-2023.3.0.1/rips.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 13:46:20.000000 rips-2023.3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-03-13 18:38:42.000000 rips-2023.3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/
+-rw-rw-rw-   0        0        0      560 2021-03-03 12:14:39.000000 rips-2023.6.0.1/LICENSE
+-rw-rw-rw-   0        0        0       75 2021-03-03 12:14:39.000000 rips-2023.6.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1039 2023-06-19 12:49:47.000000 rips-2023.6.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2021-03-03 12:14:39.000000 rips-2023.6.0.1/README.md
+-rw-rw-rw-   0        0        0      201 2021-03-03 12:14:39.000000 rips-2023.6.0.1/autoformat_pep8.txt
+-rw-rw-rw-   0        0        0     1164 2021-03-03 12:14:39.000000 rips-2023.6.0.1/create_pip_package.txt
+-rw-rw-rw-   0        0        0       37 2021-03-03 12:14:39.000000 rips-2023.6.0.1/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips/
+drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips/PythonExamples/
+-rw-rw-rw-   0        0        0     1495 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/all_cases.py
+-rw-rw-rw-   0        0        0     1267 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/all_simulation_wells.py
+-rw-rw-rw-   0        0        0      606 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/all_wells.py
+-rw-rw-rw-   0        0        0      801 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/alter_wbs_plot.py
+-rw-rw-rw-   0        0        0      685 2023-02-10 10:50:44.000000 rips-2023.6.0.1/rips/PythonExamples/case_grid_group.py
+-rw-rw-rw-   0        0        0     1016 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/case_info_streaming_example.py
+-rw-rw-rw-   0        0        0      509 2021-11-18 07:34:03.000000 rips-2023.6.0.1/rips/PythonExamples/cell_result_data.py
+-rw-rw-rw-   0        0        0     1785 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/command_example.py
+-rw-rw-rw-   0        0        0     4227 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/create_and_export_stim_plan_model.py
+-rw-rw-rw-   0        0        0     2433 2022-04-05 06:32:53.000000 rips-2023.6.0.1/rips/PythonExamples/create_intersection.py
+-rw-rw-rw-   0        0        0     3735 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/create_surface_from_thermal_fracture.py
+-rw-rw-rw-   0        0        0     1433 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/create_wbs_plot.py
+-rw-rw-rw-   0        0        0     3230 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/error_handling.py
+-rw-rw-rw-   0        0        0     1171 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/export_contour_maps.py
+-rw-rw-rw-   0        0        0      654 2021-08-17 13:58:38.000000 rips-2023.6.0.1/rips/PythonExamples/export_plots.py
+-rw-rw-rw-   0        0        0     1598 2021-09-02 13:22:54.000000 rips-2023.6.0.1/rips/PythonExamples/export_snapshots.py
+-rw-rw-rw-   0        0        0      701 2023-02-10 14:16:08.000000 rips-2023.6.0.1/rips/PythonExamples/export_well_path_completions.py
+-rw-rw-rw-   0        0        0     2671 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_of_well_logs.py
+-rw-rw-rw-   0        0        0     2056 2021-08-23 10:48:10.000000 rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_surface.py
+-rw-rw-rw-   0        0        0     1149 2021-08-31 13:17:57.000000 rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_surface_optimized.py
+-rw-rw-rw-   0        0        0      590 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/grid_information.py
+-rw-rw-rw-   0        0        0     1073 2022-03-22 10:18:39.000000 rips-2023.6.0.1/rips/PythonExamples/headless_plot_export.py
+-rw-rw-rw-   0        0        0     1617 2023-06-19 06:39:04.000000 rips-2023.6.0.1/rips/PythonExamples/import_case_properties.py
+-rw-rw-rw-   0        0        0     2370 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/import_fractures_on_well.py
+-rw-rw-rw-   0        0        0     1403 2022-10-25 08:32:28.000000 rips-2023.6.0.1/rips/PythonExamples/import_thermal_fracture_on_well.py
+-rw-rw-rw-   0        0        0     1327 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/import_well_paths_and_logs.py
+-rw-rw-rw-   0        0        0     1997 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/input_prop_test_async.py
+-rw-rw-rw-   0        0        0     1223 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/input_prop_test_sync.py
+-rw-rw-rw-   0        0        0      302 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/instance_example.py
+-rw-rw-rw-   0        0        0     1315 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/launch_load_case_snapshot_exit.py
+-rw-rw-rw-   0        0        0      465 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/launch_with_commandline_options.py
+-rw-rw-rw-   0        0        0     1131 2021-09-01 05:50:56.000000 rips-2023.6.0.1/rips/PythonExamples/load_case.py
+-rw-rw-rw-   0        0        0     1057 2021-08-16 06:21:02.000000 rips-2023.6.0.1/rips/PythonExamples/modeled_well_path.py
+-rw-rw-rw-   0        0        0     1725 2021-08-16 06:21:02.000000 rips-2023.6.0.1/rips/PythonExamples/modeled_well_path_lateral.py
+-rw-rw-rw-   0        0        0      467 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/new_summary_plot.py
+-rw-rw-rw-   0        0        0      692 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/open_project.py
+-rw-rw-rw-   0        0        0      393 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/replace_case.py
+-rw-rw-rw-   0        0        0      894 2021-09-29 06:17:01.000000 rips-2023.6.0.1/rips/PythonExamples/save_project.py
+-rw-rw-rw-   0        0        0      768 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/selected_cases.py
+-rw-rw-rw-   0        0        0     2536 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/selected_cells.py
+-rw-rw-rw-   0        0        0      379 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/set_cell_result.py
+-rw-rw-rw-   0        0        0      861 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/set_flow_diagnostics_result.py
+-rw-rw-rw-   0        0        0     1444 2021-11-18 11:24:26.000000 rips-2023.6.0.1/rips/PythonExamples/set_grid_properties.py
+-rw-rw-rw-   0        0        0     1279 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/soil_average_async.py
+-rw-rw-rw-   0        0        0      845 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/soil_average_sync.py
+-rw-rw-rw-   0        0        0     2110 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/soil_porv_async.py
+-rw-rw-rw-   0        0        0     1120 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/soil_porv_sync.py
+-rw-rw-rw-   0        0        0      460 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/summary_cases.py
+-rw-rw-rw-   0        0        0     1710 2022-03-28 07:02:00.000000 rips-2023.6.0.1/rips/PythonExamples/summary_vectors.py
+-rw-rw-rw-   0        0        0     1256 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/surface_import.py
+-rw-rw-rw-   0        0        0     1056 2021-08-31 13:16:54.000000 rips-2023.6.0.1/rips/PythonExamples/view_example.py
+-rw-rw-rw-   0        0        0      679 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/__init__.py
+-rw-rw-rw-   0        0        0    45546 2021-11-18 06:43:06.000000 rips-2023.6.0.1/rips/case.py
+-rw-rw-rw-   0        0        0     2118 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/contour_map.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips/generated/
+-rw-rw-rw-   0        0        0     7280 2023-06-12 07:10:55.000000 rips-2023.6.0.1/rips/generated/App_pb2.py
+-rw-rw-rw-   0        0        0     6724 2023-06-12 07:10:55.000000 rips-2023.6.0.1/rips/generated/App_pb2_grpc.py
+-rw-rw-rw-   0        0        0    40186 2023-06-12 07:10:55.000000 rips-2023.6.0.1/rips/generated/Case_pb2.py
+-rw-rw-rw-   0        0        0    19104 2023-06-12 07:10:55.000000 rips-2023.6.0.1/rips/generated/Case_pb2_grpc.py
+-rw-rw-rw-   0        0        0   154980 2023-06-12 07:10:56.000000 rips-2023.6.0.1/rips/generated/Commands_pb2.py
+-rw-rw-rw-   0        0        0     3360 2023-06-12 07:10:56.000000 rips-2023.6.0.1/rips/generated/Commands_pb2_grpc.py
+-rw-rw-rw-   0        0        0    14439 2023-06-12 07:10:56.000000 rips-2023.6.0.1/rips/generated/Definitions_pb2.py
+-rw-rw-rw-   0        0        0      159 2023-06-12 07:10:56.000000 rips-2023.6.0.1/rips/generated/Definitions_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5614 2023-06-12 07:10:57.000000 rips-2023.6.0.1/rips/generated/Grid_pb2.py
+-rw-rw-rw-   0        0        0     5401 2023-06-12 07:10:57.000000 rips-2023.6.0.1/rips/generated/Grid_pb2_grpc.py
+-rw-rw-rw-   0        0        0    21334 2023-06-12 07:10:57.000000 rips-2023.6.0.1/rips/generated/NNCProperties_pb2.py
+-rw-rw-rw-   0        0        0     7334 2023-06-12 07:10:57.000000 rips-2023.6.0.1/rips/generated/NNCProperties_pb2_grpc.py
+-rw-rw-rw-   0        0        0    37075 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/PdmObject_pb2.py
+-rw-rw-rw-   0        0        0    13870 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/PdmObject_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3755 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/Project_pb2.py
+-rw-rw-rw-   0        0        0     9869 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/Project_pb2_grpc.py
+-rw-rw-rw-   0        0        0    19898 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/Properties_pb2.py
+-rw-rw-rw-   0        0        0    10631 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/Properties_pb2_grpc.py
+-rw-rw-rw-   0        0        0      775 2023-06-12 10:05:22.000000 rips-2023.6.0.1/rips/generated/RiaVersionInfo.py
+-rw-rw-rw-   0        0        0    11113 2023-06-12 07:10:59.000000 rips-2023.6.0.1/rips/generated/SimulationWell_pb2.py
+-rw-rw-rw-   0        0        0     4307 2023-06-12 07:10:59.000000 rips-2023.6.0.1/rips/generated/SimulationWell_pb2_grpc.py
+-rw-rw-rw-   0        0        0    80324 2023-06-12 07:16:16.000000 rips-2023.6.0.1/rips/generated/generated_classes.py
+-rw-rw-rw-   0        0        0     3647 2021-11-18 11:24:26.000000 rips-2023.6.0.1/rips/grid.py
+-rw-rw-rw-   0        0        0     2368 2023-02-10 10:50:44.000000 rips-2023.6.0.1/rips/gridcasegroup.py
+-rw-rw-rw-   0        0        0     1511 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/grpc_retry_interceptor.py
+-rw-rw-rw-   0        0        0    14846 2022-10-04 12:14:47.000000 rips-2023.6.0.1/rips/instance.py
+-rw-rw-rw-   0        0        0    17137 2022-02-08 18:45:33.000000 rips-2023.6.0.1/rips/pdmobject.py
+-rw-rw-rw-   0        0        0      832 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/plot.py
+-rw-rw-rw-   0        0        0    11987 2021-09-29 07:44:28.000000 rips-2023.6.0.1/rips/project.py
+-rw-rw-rw-   0        0        0       59 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/resinsight_classes.py
+-rw-rw-rw-   0        0        0     2508 2022-02-08 18:45:33.000000 rips-2023.6.0.1/rips/retry_policy.py
+-rw-rw-rw-   0        0        0     2515 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/simulation_well.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips/tests/
+-rw-rw-rw-   0        0        0     1428 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/tests/conftest.py
+-rw-rw-rw-   0        0        0      207 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/tests/dataroot.py
+-rw-rw-rw-   0        0        0     8964 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_cases.py
+-rw-rw-rw-   0        0        0      875 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/tests/test_commands.py
+-rw-rw-rw-   0        0        0     2317 2022-02-21 12:46:35.000000 rips-2023.6.0.1/rips/tests/test_create_well_path.py
+-rw-rw-rw-   0        0        0     5755 2023-06-19 06:39:04.000000 rips-2023.6.0.1/rips/tests/test_grids.py
+-rw-rw-rw-   0        0        0     1198 2022-09-28 06:53:25.000000 rips-2023.6.0.1/rips/tests/test_launch.py
+-rw-rw-rw-   0        0        0     2596 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_nnc_properties.py
+-rw-rw-rw-   0        0        0     3042 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/tests/test_project.py
+-rw-rw-rw-   0        0        0     4516 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_properties.py
+-rw-rw-rw-   0        0        0     1816 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_simulation_wells.py
+-rw-rw-rw-   0        0        0     4574 2023-01-24 09:05:18.000000 rips-2023.6.0.1/rips/tests/test_summary_cases.py
+-rw-rw-rw-   0        0        0     1019 2021-08-17 12:15:16.000000 rips-2023.6.0.1/rips/tests/test_surfaces.py
+-rw-rw-rw-   0        0        0     1522 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_well_log_extraction.py
+-rw-rw-rw-   0        0        0     3343 2022-02-08 18:45:33.000000 rips-2023.6.0.1/rips/tests/test_wells.py
+-rw-rw-rw-   0        0        0      678 2021-10-14 08:34:07.000000 rips-2023.6.0.1/rips/tests/test_wells_path_completions.py
+-rw-rw-rw-   0        0        0     7612 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/view.py
+-rw-rw-rw-   0        0        0     2356 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/well_log_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips.egg-info/
+-rw-rw-rw-   0        0        0     1039 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3947 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 12:49:47.000000 rips-2023.6.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-06-12 06:26:22.000000 rips-2023.6.0.1/setup.py
```

### Comparing `rips-2023.3.0.1/LICENSE` & `rips-2023.6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/PKG-INFO` & `rips-2023.6.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: rips
-Version: 2023.3.0.1
+Version: 2023.6.0.1
 Summary: Python Interface for ResInsight
 Home-page: http://www.resinsight.org
 Author: Ceetron Solutions
 Author-email: info@ceetronsolutions.com
 License: Copyright (C) 2019-     Equinor ASA
 
 ResInsight is free software: you can redistribute it andor modify
```

### Comparing `rips-2023.3.0.1/create_pip_package.txt` & `rips-2023.6.0.1/create_pip_package.txt`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/all_cases.py` & `rips-2023.6.0.1/rips/PythonExamples/all_cases.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/all_simulation_wells.py` & `rips-2023.6.0.1/rips/PythonExamples/all_simulation_wells.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/all_wells.py` & `rips-2023.6.0.1/rips/PythonExamples/all_wells.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/alter_wbs_plot.py` & `rips-2023.6.0.1/rips/PythonExamples/alter_wbs_plot.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/case_grid_group.py` & `rips-2023.6.0.1/rips/PythonExamples/case_grid_group.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/case_info_streaming_example.py` & `rips-2023.6.0.1/rips/PythonExamples/case_info_streaming_example.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/command_example.py` & `rips-2023.6.0.1/rips/PythonExamples/command_example.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/create_and_export_stim_plan_model.py` & `rips-2023.6.0.1/rips/PythonExamples/create_and_export_stim_plan_model.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/create_intersection.py` & `rips-2023.6.0.1/rips/PythonExamples/create_intersection.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/create_surface_from_thermal_fracture.py` & `rips-2023.6.0.1/rips/PythonExamples/create_surface_from_thermal_fracture.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/create_wbs_plot.py` & `rips-2023.6.0.1/rips/PythonExamples/create_wbs_plot.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/error_handling.py` & `rips-2023.6.0.1/rips/PythonExamples/error_handling.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/export_contour_maps.py` & `rips-2023.6.0.1/rips/PythonExamples/export_contour_maps.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/export_plots.py` & `rips-2023.6.0.1/rips/PythonExamples/export_plots.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/export_snapshots.py` & `rips-2023.6.0.1/rips/PythonExamples/export_snapshots.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/export_well_path_completions.py` & `rips-2023.6.0.1/rips/PythonExamples/export_well_path_completions.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/generate_ensemble_of_well_logs.py` & `rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_of_well_logs.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/generate_ensemble_surface.py` & `rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_surface.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/generate_ensemble_surface_optimized.py` & `rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_surface_optimized.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/grid_information.py` & `rips-2023.6.0.1/rips/PythonExamples/grid_information.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/headless_plot_export.py` & `rips-2023.6.0.1/rips/PythonExamples/headless_plot_export.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/import_fractures_on_well.py` & `rips-2023.6.0.1/rips/PythonExamples/import_fractures_on_well.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/import_thermal_fracture_on_well.py` & `rips-2023.6.0.1/rips/PythonExamples/import_thermal_fracture_on_well.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/import_well_paths_and_logs.py` & `rips-2023.6.0.1/rips/PythonExamples/import_well_paths_and_logs.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/input_prop_test_async.py` & `rips-2023.6.0.1/rips/PythonExamples/input_prop_test_async.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/input_prop_test_sync.py` & `rips-2023.6.0.1/rips/PythonExamples/input_prop_test_sync.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/launch_load_case_snapshot_exit.py` & `rips-2023.6.0.1/rips/PythonExamples/launch_load_case_snapshot_exit.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/load_case.py` & `rips-2023.6.0.1/rips/PythonExamples/load_case.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/modeled_well_path.py` & `rips-2023.6.0.1/rips/PythonExamples/modeled_well_path.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/modeled_well_path_lateral.py` & `rips-2023.6.0.1/rips/PythonExamples/modeled_well_path_lateral.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/open_project.py` & `rips-2023.6.0.1/rips/PythonExamples/open_project.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/save_project.py` & `rips-2023.6.0.1/rips/PythonExamples/save_project.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/selected_cases.py` & `rips-2023.6.0.1/rips/PythonExamples/selected_cases.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/selected_cells.py` & `rips-2023.6.0.1/rips/PythonExamples/selected_cells.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/set_flow_diagnostics_result.py` & `rips-2023.6.0.1/rips/PythonExamples/set_flow_diagnostics_result.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/set_grid_properties.py` & `rips-2023.6.0.1/rips/PythonExamples/set_grid_properties.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/soil_average_async.py` & `rips-2023.6.0.1/rips/PythonExamples/soil_average_async.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/soil_average_sync.py` & `rips-2023.6.0.1/rips/PythonExamples/soil_average_sync.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/soil_porv_async.py` & `rips-2023.6.0.1/rips/PythonExamples/soil_porv_async.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/soil_porv_sync.py` & `rips-2023.6.0.1/rips/PythonExamples/soil_porv_sync.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/summary_vectors.py` & `rips-2023.6.0.1/rips/PythonExamples/summary_vectors.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/surface_import.py` & `rips-2023.6.0.1/rips/PythonExamples/surface_import.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/PythonExamples/view_example.py` & `rips-2023.6.0.1/rips/PythonExamples/view_example.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/__init__.py` & `rips-2023.6.0.1/rips/__init__.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/case.py` & `rips-2023.6.0.1/rips/case.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/contour_map.py` & `rips-2023.6.0.1/rips/contour_map.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/App_pb2.py` & `rips-2023.6.0.1/rips/generated/App_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/App_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/App_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Case_pb2.py` & `rips-2023.6.0.1/rips/generated/Case_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Case_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/Case_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Commands_pb2.py` & `rips-2023.6.0.1/rips/generated/Commands_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Commands_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/Commands_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Definitions_pb2.py` & `rips-2023.6.0.1/rips/generated/Definitions_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Grid_pb2.py` & `rips-2023.6.0.1/rips/generated/Grid_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Grid_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/Grid_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/NNCProperties_pb2.py` & `rips-2023.6.0.1/rips/generated/NNCProperties_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/NNCProperties_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/NNCProperties_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/PdmObject_pb2.py` & `rips-2023.6.0.1/rips/generated/PdmObject_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/PdmObject_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/PdmObject_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Project_pb2.py` & `rips-2023.6.0.1/rips/generated/Project_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Project_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/Project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Properties_pb2.py` & `rips-2023.6.0.1/rips/generated/Properties_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/Properties_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/Properties_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/RiaVersionInfo.py` & `rips-2023.6.0.1/rips/generated/RiaVersionInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 #  See the GNU General Public License at <http://www.gnu.org/licenses/gpl.html> 
 #  for more details.
 #
 #  Python version of RiaVersionInfo.h
 #  Just sets version constants
 
 RESINSIGHT_MAJOR_VERSION = "2023"
-RESINSIGHT_MINOR_VERSION = "03"
+RESINSIGHT_MINOR_VERSION = "06"
 RESINSIGHT_PATCH_VERSION = "0"
```

### Comparing `rips-2023.3.0.1/rips/generated/SimulationWell_pb2.py` & `rips-2023.6.0.1/rips/generated/SimulationWell_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/SimulationWell_pb2_grpc.py` & `rips-2023.6.0.1/rips/generated/SimulationWell_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/generated/generated_classes.py` & `rips-2023.6.0.1/rips/generated/generated_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,24 +115,36 @@
         self.name_setting = "FULL_CASE_NAME"
         PdmObjectBase.__init__(self, pb2_object, channel)
         if Case.__custom_init__ is not None:
             Case.__custom_init__(self, pb2_object=pb2_object, channel=channel)
 
 class Reservoir(Case):
     """
-    Abtract base class for Eclipse Cases
+    Abstract base class for Eclipse Cases
 
     """
     __custom_init__ = None #: Assign a custom init routine to be run at __init__
 
     def __init__(self, pb2_object=None, channel=None):
         Case.__init__(self, pb2_object, channel)
         if Reservoir.__custom_init__ is not None:
             Reservoir.__custom_init__(self, pb2_object=pb2_object, channel=channel)
 
+    def import_properties(self, file_names=[]):
+        """
+        Import Properties
+
+        Arguments:
+            file_names (List of str): 
+        Returns:
+            
+        """
+        return self._call_pdm_method("import_properties", file_names=file_names)
+
+
     def views(self):
         """All Eclipse Views in the case
 
         Returns:
              List of EclipseView
         """
         return self.children("Views", EclipseView)
@@ -632,21 +644,23 @@
         View.__init__(self, pb2_object, channel)
         if GeoMechView.__custom_init__ is not None:
             GeoMechView.__custom_init__(self, pb2_object=pb2_object, channel=channel)
 
 class GridCaseSurface(SurfaceInterface):
     """
     Attributes:
+        include_inactive_cells (bool): Include Inactive Cells
         slice_index (int): Slice Index (K)
         source_case (str): Source Case
         watertight (bool): Watertight Surface (fill gaps)
     """
     __custom_init__ = None #: Assign a custom init routine to be run at __init__
 
     def __init__(self, pb2_object=None, channel=None):
+        self.include_inactive_cells = False
         self.slice_index = 1
         self.source_case = ""
         self.watertight = False
         SurfaceInterface.__init__(self, pb2_object, channel)
         if GridCaseSurface.__custom_init__ is not None:
             GridCaseSurface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
 
@@ -1361,14 +1375,15 @@
         """
         return self.children("StimPlanModelPlots", StimPlanModelPlot)
 
 
 class StimPlanModelTemplate(NamedObject):
     """
     Attributes:
+        default_facies (str): Default Facies
         default_permeability (float): Default Permeability
         default_porosity (float): Default Porosity
         dynamic_eclipse_case (str): Dynamic Case
         id (int): ID
         initial_pressure_eclipse_case (str): Initial Pressure Case
         overburden_facies (str): Overburden Facies
         overburden_fluid_density (float): Overburden Fluid Density [g/cm^3]
@@ -1390,14 +1405,15 @@
         underburden_porosity (float): Underburden Porosity
         vertical_stress (float): Vertical Stress
         vertical_stress_gradient (float): Vertical Stress Gradient
     """
     __custom_init__ = None #: Assign a custom init routine to be run at __init__
 
     def __init__(self, pb2_object=None, channel=None):
+        self.default_facies = ""
         self.default_permeability = 0.0001
         self.default_porosity = 0.01
         self.dynamic_eclipse_case = ""
         self.id = -1
         self.initial_pressure_eclipse_case = ""
         self.overburden_facies = ""
         self.overburden_fluid_density = 1.03
```

### Comparing `rips-2023.3.0.1/rips/grid.py` & `rips-2023.6.0.1/rips/grid.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/gridcasegroup.py` & `rips-2023.6.0.1/rips/gridcasegroup.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/grpc_retry_interceptor.py` & `rips-2023.6.0.1/rips/grpc_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/instance.py` & `rips-2023.6.0.1/rips/instance.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/pdmobject.py` & `rips-2023.6.0.1/rips/pdmobject.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/plot.py` & `rips-2023.6.0.1/rips/plot.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/project.py` & `rips-2023.6.0.1/rips/project.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/retry_policy.py` & `rips-2023.6.0.1/rips/retry_policy.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/simulation_well.py` & `rips-2023.6.0.1/rips/simulation_well.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/conftest.py` & `rips-2023.6.0.1/rips/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_cases.py` & `rips-2023.6.0.1/rips/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_commands.py` & `rips-2023.6.0.1/rips/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_create_well_path.py` & `rips-2023.6.0.1/rips/tests/test_create_well_path.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_launch.py` & `rips-2023.6.0.1/rips/tests/test_launch.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_nnc_properties.py` & `rips-2023.6.0.1/rips/tests/test_nnc_properties.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_project.py` & `rips-2023.6.0.1/rips/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_properties.py` & `rips-2023.6.0.1/rips/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_simulation_wells.py` & `rips-2023.6.0.1/rips/tests/test_simulation_wells.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_summary_cases.py` & `rips-2023.6.0.1/rips/tests/test_summary_cases.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_surfaces.py` & `rips-2023.6.0.1/rips/tests/test_surfaces.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_well_log_extraction.py` & `rips-2023.6.0.1/rips/tests/test_well_log_extraction.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_wells.py` & `rips-2023.6.0.1/rips/tests/test_wells.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/tests/test_wells_path_completions.py` & `rips-2023.6.0.1/rips/tests/test_wells_path_completions.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/view.py` & `rips-2023.6.0.1/rips/view.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips/well_log_plot.py` & `rips-2023.6.0.1/rips/well_log_plot.py`

 * *Files identical despite different names*

### Comparing `rips-2023.3.0.1/rips.egg-info/PKG-INFO` & `rips-2023.6.0.1/rips.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: rips
-Version: 2023.3.0.1
+Version: 2023.6.0.1
 Summary: Python Interface for ResInsight
 Home-page: http://www.resinsight.org
 Author: Ceetron Solutions
 Author-email: info@ceetronsolutions.com
 License: Copyright (C) 2019-     Equinor ASA
 
 ResInsight is free software: you can redistribute it andor modify
```

### Comparing `rips-2023.3.0.1/rips.egg-info/SOURCES.txt` & `rips-2023.6.0.1/rips.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 rips/PythonExamples/export_snapshots.py
 rips/PythonExamples/export_well_path_completions.py
 rips/PythonExamples/generate_ensemble_of_well_logs.py
 rips/PythonExamples/generate_ensemble_surface.py
 rips/PythonExamples/generate_ensemble_surface_optimized.py
 rips/PythonExamples/grid_information.py
 rips/PythonExamples/headless_plot_export.py
+rips/PythonExamples/import_case_properties.py
 rips/PythonExamples/import_fractures_on_well.py
 rips/PythonExamples/import_thermal_fracture_on_well.py
 rips/PythonExamples/import_well_paths_and_logs.py
 rips/PythonExamples/input_prop_test_async.py
 rips/PythonExamples/input_prop_test_sync.py
 rips/PythonExamples/instance_example.py
 rips/PythonExamples/launch_load_case_snapshot_exit.py
```

### Comparing `rips-2023.3.0.1/setup.py` & `rips-2023.6.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('LICENSE') as f:
 	license = f.read()
 
 RIPS_DIST_VERSION = '1'
 	
 setup(
     name='rips',
-    version='2023.03.0.' + RIPS_DIST_VERSION,
+    version='2023.06.0.' + RIPS_DIST_VERSION,
     description='Python Interface for ResInsight',
     long_description=readme,
     author='Ceetron Solutions',
     author_email='info@ceetronsolutions.com',
     url='http://www.resinsight.org',
     license=license,
     packages=['rips'],
```

